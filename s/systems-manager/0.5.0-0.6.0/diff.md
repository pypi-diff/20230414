# Comparing `tmp/systems_manager-0.5.0-py2.py3-none-any.whl.zip` & `tmp/systems_manager-0.6.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 22744 bytes, number of entries: 9
--rw-r--r--  2.0 unx      335 b- defN 23-Jan-01 22:03 systems_manager/__init__.py
--rw-r--r--  2.0 unx    34181 b- defN 23-Jan-08 06:08 systems_manager/systems_manager.py
--rw-r--r--  2.0 unx      116 b- defN 23-Jan-08 06:08 systems_manager/version.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jan-08 06:08 systems_manager-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2359 b- defN 23-Jan-08 06:08 systems_manager-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jan-08 06:08 systems_manager-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       74 b- defN 23-Jan-08 06:08 systems_manager-0.5.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Jan-08 06:08 systems_manager-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      788 b- defN 23-Jan-08 06:08 systems_manager-0.5.0.dist-info/RECORD
-9 files, 73128 bytes uncompressed, 21370 bytes compressed:  70.8%
+Zip file size: 22067 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      335 b- defN 23-Apr-14 02:11 systems_manager/__init__.py
+-rw-r--r--  2.0 unx    32579 b- defN 23-Apr-14 02:11 systems_manager/systems_manager.py
+-rw-r--r--  2.0 unx      116 b- defN 23-Apr-14 02:11 systems_manager/version.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Apr-14 02:11 systems_manager-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2359 b- defN 23-Apr-14 02:11 systems_manager-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-14 02:11 systems_manager-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       74 b- defN 23-Apr-14 02:11 systems_manager-0.6.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-14 02:11 systems_manager-0.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      788 b- defN 23-Apr-14 02:11 systems_manager-0.6.0.dist-info/RECORD
+9 files, 71526 bytes uncompressed, 20693 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: systems_manager/systems_manager.py
 Comment: 
 
 Filename: systems_manager/version.py
 Comment: 
 
-Filename: systems_manager-0.5.0.dist-info/LICENSE
+Filename: systems_manager-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: systems_manager-0.5.0.dist-info/METADATA
+Filename: systems_manager-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: systems_manager-0.5.0.dist-info/WHEEL
+Filename: systems_manager-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: systems_manager-0.5.0.dist-info/entry_points.txt
+Filename: systems_manager-0.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: systems_manager-0.5.0.dist-info/top_level.txt
+Filename: systems_manager-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: systems_manager-0.5.0.dist-info/RECORD
+Filename: systems_manager-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## systems_manager/systems_manager.py

```diff
@@ -25,15 +25,15 @@
         self.bash_profile = ""
         self.ubuntu_install_command = []
         self.windows_install_command = []
         self.set_applications(self.applications)
         self.ubuntu_update_command = [['apt', 'update'], ['apt', 'upgrade', '-y'], ['apt', 'autoremove', '-y']]
         if os.path.isfile(os.path.expanduser("~\AppData\Local\Microsoft\WindowsApps\winget.exe")):
             self.windows_update_command = [
-                ['winget', 'upgrade', '--all'], ["powershell.exe", 'Install-Module', 'PSWindowsUpdate', 'Force'],
+                ['winget', 'upgrade', '--all', '--silent', '--accept-package-agreements', '--accept-source-agreements'], ["powershell.exe", 'Install-Module', 'PSWindowsUpdate', 'Force'],
                 ["powershell.exe", 'Get-WindowsUpdate'], ["powershell.exe", 'Install-WindowsUpdate']
             ]
         else:
             self.windows_update_command = [
                 ["powershell.exe", 'Start-Process', '"ms-appinstaller:?source=https://aka.ms/getwinget"'],
                 ["powershell.exe", '$nid', '=', '(Get-Process AppInstaller).Id'],
                 ["powershell.exe", 'Wait-Process', '-Id', '$nid'], ['winget', 'upgrade', '--all'],
@@ -442,59 +442,42 @@
             elif self.operating_system == "Windows":
                 self.applications = ["Python.Python.3"]
         elif applications == "all":
             if self.operating_system == "Ubuntu":
                 self.applications = [
                     "atomicparsley", "audacity", "curl", "dialog", "discord", "containerd", "docker.io",
                     "ddclient", "docker-compose", "dos2unix", "enscript", "ffmpeg", "fstab", "gimp", "git",
-                    "gnome-shell",
+                    "gnome-shell", "rustc",
                     "ubuntu-gnome-desktop", "gnome-theme", "gnucobol", "ghostscript", "gparted", "gramps", "jq", "kexi",
                     "kvm", "lm-sensors", "mediainfo", "mkvtoolnix", "neofetch", "nfs-common", "nfs-kernel-server", "net-tools",
                     "openjdk-8-jdk", "nmap", "openssh-server", "openvpn", "preload", "poppler-utils", "python3",
                     "python3-is-python", "pycharm", "rygel", "samba", "samba-common", "smbclient samba-common-bin",
                     "smbclient", "cifs-utils", "scrcpy", "sysstat", "net-tools", "numactl",
                     "linux-tools-common", "steam", "startup-disk-creator", "update-manager", "synaptic", "telegram",
                     "tesseract", "tigervnc", "tmux", "transmission", "translate-shell", "trash-cli", "tree", "unzip",
                     "udisks2", "vlc", "wine", "wireshark", "wget", "xdotool", "xpaint", "xsel", "yq"
                 ]
             elif self.operating_system == "Windows":
                 self.applications = [
-                    "Git.Git", "oh-my-posh", "Discord.Discord", "Google.Chrome",
-                    "Microsoft.VCRedist.2015+.x64", "Microsoft.VCRedist.2015+.x86", "Microsoft.VCRedist.2013.x64",
-                    "Microsoft.Teams", "Oracle.VirtualBox", "ParadoxInteractive.ParadoxLauncher",
-                    "Nvidia.GeForceExperience", "Zoom.Zoom", "Mojang.MinecraftLauncher", "Microsoft.VisualStudioCode",
-                    "Samsung.DeX", "TheDocumentFoundation.LibreOffice", "Adobe.Acrobat.Reader.64-bit",
-                    "Famatech.AdvancedIPScanner", "GitHub.Atom", "Audacity.Audacity", "Lexikos.AutoHotkey",
-                    "BraveSoftware.BraveBrowser", "Google.Chrome", "TorProject.TorBrowser",
-                    "voidtools.Everything --source winget", "Balena.Etcher", "Mozilla.Firefox", "GIMP.GIMP",
-                    "DuongDieuPhap.ImageGlass", "AdoptOpenJDK.OpenJDK.8", "AdoptOpenJDK.OpenJDK.16", "Oracle.JDK.18",
+                    "Git.Git", "oh-my-posh", "Discord.Discord", "Microsoft.VCRedist.2015+.x64", "Microsoft.VCRedist.2015+.x86", 
+                    "Microsoft.VCRedist.2013.x64", "Microsoft.VisualStudioCode", "TheDocumentFoundation.LibreOffice", 
+                    "Adobe.Acrobat.Reader.64-bit", "Audacity.Audacity", "Google.Chrome", "Balena.Etcher", "Mozilla.Firefox", 
+                    "GIMP.GIMP", "AdoptOpenJDK.OpenJDK.8", "AdoptOpenJDK.OpenJDK.16", "Oracle.JDK.18",
                     "JetBrains.Toolbox", "OpenJS.NodeJS", "OpenJS.NodeJS.LTS", "clsid2.mpc-hc", "Notepad++.Notepad++",
-                    "Microsoft.PowerToys", "PuTTY.PuTTY", "7zip.7zip", "Rustlang.Rust.MSVC", "SublimeHQ.SublimeText.4",
-                    "SumatraPDF.SumatraPDF", "Microsoft.WindowsTerminal", "ShareX.ShareX",
-                    "Tonec.InternetDownloadManager", "Alacritty.Alacritty", "VideoLAN.VLC", "KDE.Kdenlive",
-                    "Microsoft.VisualStudioCode --source winget", "VSCodium.VSCodium", "WinSCP.WinSCP",
-                    "Bitwarden.Bitwarden", "AnyDeskSoftwareGmbH.AnyDesk", "BlenderFoundation.Blender", "CPUID.CPU-Z",
-                    "eloston.ungoogled-chromium", "File-New-Project.EarTrumpet", "EpicGames.EpicGamesLauncher",
-                    "Flameshot.Flameshot", "PeterPawlowski.foobar2000", "GOG.Galaxy", "TechPowerUp.GPU-Z",
-                    "Glarysoft.GlaryUtilities", "Greenshot.Greenshot", "HandBrake.HandBrake", "HexChat.HexChat",
-                    "REALiX.HWiNFO", "Inkscape.Inkscape", "KeePassXCTeam.KeePassXC", "LibreWolf.LibreWolf",
-                    "Malwarebytes.Malwarebytes", "Element.Element", "mRemoteNG.mRemoteNG", "TechPowerUp.NVCleanstall",
-                    "OBSProject.OBSStudio", "Obsidian.Obsidian", "RevoUninstaller.RevoUninstaller", "Rufus.Rufus",
-                    "OpenWhisperSystems.Signal", "Microsoft.Skype", "SlackTechnologies.Slack", "Spotify.Spotify",
-                    "Valve.Steam", "TeamViewer.TeamViewer", "Microsoft.Teams", "JAMSoftware.TreeSize.Free",
-                    "Microsoft.VisualStudio.2022.Community", "VivaldiTechnologies.Vivaldi", "VB-Audio.Voicemeeter",
-                    "WinDirStat.WinDirStat", "AntibodySoftware.WizTree", "WiresharkFoundation.Wireshark",
-                    "Henry++.simplewall", "Zoom.Zoom", "Viber.Viber", "xanderfrangos.twinkletray"
+                    "Microsoft.PowerToys", "PuTTY.PuTTY", "7zip.7zip", "Rustlang.Rust.MSVC", "Microsoft.WindowsTerminal", 
+                    "Rustlang.Rust.GNU", "VideoLAN.VLC", "VSCodium.VSCodium", "BlenderFoundation.Blender", "Element.Element", 
+                    "mRemoteNG.mRemoteNG", "TechPowerUp.NVCleanstall", "OBSProject.OBSStudio", "Obsidian.Obsidian", 
+                    "RevoUninstaller.RevoUninstaller", "Rufus.Rufus", "Valve.Steam", "WiresharkFoundation.Wireshark"
                 ]
         else:
             self.applications = applications
 
         for application in self.applications:
             self.ubuntu_install_command.append(['apt', 'install', '-y', f'{application}'])
-            self.windows_install_command.append(['winget', 'install', '-y', f'{application}'])
+            self.windows_install_command.append(['winget', 'install', '--accept-package-agreements', '--accept-source-agreements', f'{application}'])
 
     def get_features(self):
         return self.windows_features
 
     def set_features(self, features):
         if features is None or len(features) == 0:
             self.windows_features = [
```

## systems_manager/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.5.0'
+__version__ = '0.6.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `systems_manager-0.5.0.dist-info/LICENSE` & `systems_manager-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `systems_manager-0.5.0.dist-info/METADATA` & `systems_manager-0.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systems-manager
-Version: 0.5.0
+Version: 0.6.0
 Summary: Systems-Manager will update your system and install/upgrade applications.
 Home-page: https://github.com/Knuckles-Team/systems-manager
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (>=2.28.1)
 
 # Systems-Manager
-*Version: 0.5.0*
+*Version: 0.6.0*
 
 Systems-Manager will update your system and install/upgrade applications.
 
 ### Usage:
 | Short Flag | Long Flag         | Description                                   |
 |------------|-------------------|-----------------------------------------------|
 | -h         | --help            | See usage for script                          |
```

## Comparing `systems_manager-0.5.0.dist-info/RECORD` & `systems_manager-0.6.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 systems_manager/__init__.py,sha256=uWwoY0W8q86L6py_9DSgjxt8bqy6jRmJ_BbzEU9mVSU,335
-systems_manager/systems_manager.py,sha256=N40xHXi1Nr4Qsv8u8kTuSuyj2EUOpxqc1e_i8fBsf8Q,34181
-systems_manager/version.py,sha256=6IhjTbl3T306PyVy-FZE4rpQc3haUwFDchvvd4igGpw,116
-systems_manager-0.5.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-systems_manager-0.5.0.dist-info/METADATA,sha256=YMFmRAD5VmMplhy2ZXfkzFPoHVCrxSaMP7h8Ya3Nrbw,2359
-systems_manager-0.5.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-systems_manager-0.5.0.dist-info/entry_points.txt,sha256=nw6W7EqOUK-gVmX8o1T12ZFBysvpt0aXWat9rNzpP58,74
-systems_manager-0.5.0.dist-info/top_level.txt,sha256=4BlAsWtCOTIoxPSPyeacWxqt0ahm5qbO4sgcOvHQ-RI,16
-systems_manager-0.5.0.dist-info/RECORD,,
+systems_manager/systems_manager.py,sha256=tFMqaQ8JiNwtWr3fBC2ndWvK3lKhZsSayuMIRAXQChY,32579
+systems_manager/version.py,sha256=gO8BLKzpTbVdwjtv4mzScee0RMbIoAvk8PCBFoR5gMQ,116
+systems_manager-0.6.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+systems_manager-0.6.0.dist-info/METADATA,sha256=MgUGHP-2PurAauU5rxSqJipUoQSUDZbNHvow9xzIXTk,2359
+systems_manager-0.6.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+systems_manager-0.6.0.dist-info/entry_points.txt,sha256=nw6W7EqOUK-gVmX8o1T12ZFBysvpt0aXWat9rNzpP58,74
+systems_manager-0.6.0.dist-info/top_level.txt,sha256=4BlAsWtCOTIoxPSPyeacWxqt0ahm5qbO4sgcOvHQ-RI,16
+systems_manager-0.6.0.dist-info/RECORD,,
```

