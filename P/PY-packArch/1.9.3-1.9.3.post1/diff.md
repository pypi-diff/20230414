# Comparing `tmp/PY-packArch-1.9.3.tar.gz` & `tmp/PY-packArch-1.9.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PY-packArch-1.9.3.tar", last modified: Sat Apr  8 18:18:40 2023, max compression
+gzip compressed data, was "PY-packArch-1.9.3.post1.tar", last modified: Fri Apr 14 07:43:10 2023, max compression
```

## Comparing `PY-packArch-1.9.3.tar` & `PY-packArch-1.9.3.post1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-08 18:18:40.251784 PY-packArch-1.9.3/
--rw-r--r--   0 angel     (1000) users      (984)    35149 2023-03-07 00:39:50.000000 PY-packArch-1.9.3/LICENSE
--rw-r--r--   0 angel     (1000) users      (984)    10671 2023-04-08 18:18:40.251784 PY-packArch-1.9.3/PKG-INFO
-drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-08 18:18:40.249784 PY-packArch-1.9.3/PY_packArch.egg-info/
--rw-r--r--   0 angel     (1000) users      (984)    10671 2023-04-08 18:18:40.000000 PY-packArch-1.9.3/PY_packArch.egg-info/PKG-INFO
--rw-r--r--   0 angel     (1000) users      (984)      184 2023-04-08 18:18:40.000000 PY-packArch-1.9.3/PY_packArch.egg-info/SOURCES.txt
--rw-r--r--   0 angel     (1000) users      (984)        1 2023-04-08 18:18:40.000000 PY-packArch-1.9.3/PY_packArch.egg-info/dependency_links.txt
--rw-r--r--   0 angel     (1000) users      (984)        9 2023-04-08 18:18:40.000000 PY-packArch-1.9.3/PY_packArch.egg-info/top_level.txt
--rw-r--r--   0 angel     (1000) users      (984)     9810 2023-03-16 20:36:50.000000 PY-packArch-1.9.3/README.md
--rw-r--r--   0 angel     (1000) users      (984)     8087 2023-04-08 18:14:37.000000 PY-packArch-1.9.3/packarch.py
--rw-r--r--   0 angel     (1000) users      (984)      848 2023-04-08 18:17:31.000000 PY-packArch-1.9.3/pyproject.toml
--rw-r--r--   0 angel     (1000) users      (984)       38 2023-04-08 18:18:40.251784 PY-packArch-1.9.3/setup.cfg
+drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 07:43:10.693722 PY-packArch-1.9.3.post1/
+-rw-r--r--   0 angel     (1000) users      (984)    35149 2023-03-07 00:39:50.000000 PY-packArch-1.9.3.post1/LICENSE
+-rw-r--r--   0 angel     (1000) users      (984)    10671 2023-04-14 07:43:10.693722 PY-packArch-1.9.3.post1/PKG-INFO
+drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 07:43:10.693722 PY-packArch-1.9.3.post1/PY_packArch.egg-info/
+-rw-r--r--   0 angel     (1000) users      (984)    10671 2023-04-14 07:43:10.000000 PY-packArch-1.9.3.post1/PY_packArch.egg-info/PKG-INFO
+-rw-r--r--   0 angel     (1000) users      (984)      212 2023-04-14 07:43:10.000000 PY-packArch-1.9.3.post1/PY_packArch.egg-info/SOURCES.txt
+-rw-r--r--   0 angel     (1000) users      (984)        1 2023-04-14 07:43:10.000000 PY-packArch-1.9.3.post1/PY_packArch.egg-info/dependency_links.txt
+-rw-r--r--   0 angel     (1000) users      (984)       12 2023-04-14 07:43:10.000000 PY-packArch-1.9.3.post1/PY_packArch.egg-info/requires.txt
+-rw-r--r--   0 angel     (1000) users      (984)        9 2023-04-14 07:43:10.000000 PY-packArch-1.9.3.post1/PY_packArch.egg-info/top_level.txt
+-rw-r--r--   0 angel     (1000) users      (984)     9810 2023-03-16 20:36:50.000000 PY-packArch-1.9.3.post1/README.md
+-rw-r--r--   0 angel     (1000) users      (984)     7873 2023-04-14 07:03:26.000000 PY-packArch-1.9.3.post1/packarch.py
+-rw-r--r--   0 angel     (1000) users      (984)       38 2023-04-14 07:43:10.693722 PY-packArch-1.9.3.post1/setup.cfg
+-rw-r--r--   0 angel     (1000) users      (984)     1080 2023-04-14 07:42:12.000000 PY-packArch-1.9.3.post1/setup.py
```

### Comparing `PY-packArch-1.9.3/LICENSE` & `PY-packArch-1.9.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `PY-packArch-1.9.3/PKG-INFO` & `PY-packArch-1.9.3.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: PY-packArch
-Version: 1.9.3
+Version: 1.9.3.post1
 Summary: Small library to manage pacman package manager and install packages from AUR
-Author-email: Tom5521 <mismarttv321@gmail.com>
+Home-page: https://github.com/Tom5521/PY-PackArch
+Author: Tom5521
+Author-email: mismarttv321@gmail.com
 License: GPL-3.0
-Project-URL: Homepage, https://github.com/Tom5521/PY-PackArch
 Project-URL: Bug Tracker, https://github.com/Tom5521/PY-PackArch/issues
 Project-URL: Documentation, https://github.com/Tom5521/PY-PackArch/blob/master/README.md
 Project-URL: Download-url, https://github.com/Tom5521/PY-PackArch/archive/refs/heads/master.zip
 Keywords: pacman,arch linux,linux,AUR
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Topic :: System :: Software Distribution
```

### Comparing `PY-packArch-1.9.3/PY_packArch.egg-info/PKG-INFO` & `PY-packArch-1.9.3.post1/PY_packArch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: PY-packArch
-Version: 1.9.3
+Version: 1.9.3.post1
 Summary: Small library to manage pacman package manager and install packages from AUR
-Author-email: Tom5521 <mismarttv321@gmail.com>
+Home-page: https://github.com/Tom5521/PY-PackArch
+Author: Tom5521
+Author-email: mismarttv321@gmail.com
 License: GPL-3.0
-Project-URL: Homepage, https://github.com/Tom5521/PY-PackArch
 Project-URL: Bug Tracker, https://github.com/Tom5521/PY-PackArch/issues
 Project-URL: Documentation, https://github.com/Tom5521/PY-PackArch/blob/master/README.md
 Project-URL: Download-url, https://github.com/Tom5521/PY-PackArch/archive/refs/heads/master.zip
 Keywords: pacman,arch linux,linux,AUR
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Topic :: System :: Software Distribution
```

### Comparing `PY-packArch-1.9.3/README.md` & `PY-packArch-1.9.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `PY-packArch-1.9.3/packarch.py` & `PY-packArch-1.9.3.post1/packarch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # Created by Tom5521 or Angel
 # Under the GPL license 3.0
 
 from os import getcwd, chdir, listdir, system as sys
 from time import sleep as sl
+from Toolbox.ansi_colors import *
+from Toolbox.tools import command_read
+
 
 current_directoy = getcwd()
 
 hide = [">/dev/null 2>&1", "|ls > .out && rm -rf .out", "clear"]
 sp = " "
 All_text_cond = True
 words = [
-    "Installing ",  # 0
-    "Installed",  # 1
-    "Update Complete",  # 2
-    "Updating repos",  # 3
+    c.yellow("Installing "),  # 0
+    c.green("Installed"),  # 1
+    bc.green("Update Complete"),  # 2
+    c.yellow("Updating repos"),  # 3
     "...",  # 4
-    "Updating",  # 5
-    "Searching",  # 6
+    c.yellow("Updating"),  # 5
+    c.yellow("Searching"),  # 6
 ]
 
 
 def clear():
     sys(hide[2])
 
 
@@ -46,26 +49,18 @@
 
 
 def installed():
     print(words[1])
 
 
 def check(nombre_check):
-    comprobator = False
-    chdir(current_directoy)
-    clear()
-    sys("pacman -Q " + nombre_check + "> /tmp/tmp-check")
-    optemp = open("/tmp/tmp-check", "r")
-    readtemp = optemp.read()
-    if nombre_check in readtemp:
-        comprobator = True
+    if check in command_read(f"pacman -Qs {check}"):
+        return True
     else:
-        comprobator = False
-    sys("rm /tmp/tmp-check")
-    return comprobator
+        return False
 
 
 def install(nombre_pacman, cond_1="", cond_2=""):
     match cond_1:
         case "-v":
             print(words[0] + nombre_pacman + words[4])
             sys("sudo pacman -S " + nombre_pacman + sp + cond_2 + sp + " --noconfirm")
@@ -99,15 +94,15 @@
             pass
             hide[0] = ""
         if "f" in cond_1:
             sys("sudo pacman -Rdd" + sp + removes + " --noconfirm" + hide[0])
         else:
             sys("sudo pacman -R" + sp + removes + " --noconfirm" + hide[0])
     else:
-        print("El o los paquetes no se encontraron en su totalidad")
+        print("The package or packages were not found in their entirety")
     hide[0] = ">/dev/null 2>&1"
 
 
 class aur:
     def install(apps_aur, cond_1=""):
         global force
         force = False
@@ -265,28 +260,27 @@
 
 def upgrade_me():
     sys("pip install py-packarch --upgrade")
     sys("pip3 install py-packarch --upgrade")
 
 
 def version():
-    print("PY-PackArch \nCreated by Tom5521 \nVersion 1.9.2\nUnder the gpl-3.0 licence")
+    print(
+        "PY-PackArch \nCreated by Tom5521 \nVersion 1.9.3-1\nUnder the gpl-3.0 licence"
+    )
 
 
 def info(package):
     sys("pacman -Si " + package)
 
 
 def get_version(packages, cond=""):
     for i in packages.split():
-        sys("pacman -Q " + i + " > /tmp/transpaced_data")
-        opendata = open("/tmp/transpaced_data", "r")
-        readata = opendata.read()
+        readata = command_read("pacman -Q " + i)
         if "h" in cond:
             print(readata.split()[1])
         else:
             print(i + " is in version", (readata.split()[1]))
-    sys("rm /tmp/transpaced_data")
 
 
 def manual():
-    sys("firefox https://github.com/Tom5521/PY-PackArch/blob/master/README.md")
+    sys("xdg-open https://github.com/Tom5521/PY-PackArch/blob/master/README.md")
```

