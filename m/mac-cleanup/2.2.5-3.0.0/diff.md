# Comparing `tmp/mac_cleanup-2.2.5.tar.gz` & `tmp/mac_cleanup-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mac_cleanup-2.2.5.tar", max compression
+gzip compressed data, was "mac_cleanup-3.0.0.tar", max compression
```

## Comparing `mac_cleanup-2.2.5.tar` & `mac_cleanup-3.0.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0    11357 2022-08-09 13:15:49.497915 mac_cleanup-2.2.5/LICENSE
--rw-r--r--   0        0        0     3355 2023-02-25 12:12:01.969803 mac_cleanup-2.2.5/README.md
--rw-r--r--   0        0        0      280 2023-02-25 12:09:47.230804 mac_cleanup-2.2.5/mac_cleanup/__init__.py
--rw-r--r--   0        0        0      181 2023-02-25 12:09:47.231565 mac_cleanup-2.2.5/mac_cleanup/__version__.py
--rw-r--r--   0        0        0     2950 2023-02-25 12:09:47.231943 mac_cleanup-2.2.5/mac_cleanup/cli.py
--rw-r--r--   0        0        0     4339 2023-02-25 12:09:47.232338 mac_cleanup-2.2.5/mac_cleanup/config.py
--rw-r--r--   0        0        0     1642 2023-02-25 12:09:47.232715 mac_cleanup-2.2.5/mac_cleanup/console.py
--rw-r--r--   0        0        0    12015 2023-02-25 12:09:47.233127 mac_cleanup-2.2.5/mac_cleanup/default_modules.py
--rw-r--r--   0        0        0     1456 2023-02-25 12:09:47.233510 mac_cleanup-2.2.5/mac_cleanup/modules.py
--rwxr-xr-x   0        0        0    11244 2023-02-25 12:09:47.234197 mac_cleanup-2.2.5/mac_cleanup/utils.py
--rw-r--r--   0        0        0     1923 2023-02-25 12:11:27.066350 mac_cleanup-2.2.5/pyproject.toml
--rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 mac_cleanup-2.2.5/setup.py
--rw-r--r--   0        0        0     4554 1970-01-01 00:00:00.000000 mac_cleanup-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-08-09 13:15:49.497915 mac_cleanup-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3795 2023-04-13 13:54:59.884936 mac_cleanup-3.0.0/README.md
+-rw-r--r--   0        0        0      425 2023-04-10 17:33:48.121290 mac_cleanup-3.0.0/mac_cleanup/__init__.py
+-rw-r--r--   0        0        0      181 2023-03-26 22:15:29.161722 mac_cleanup-3.0.0/mac_cleanup/__version__.py
+-rw-r--r--   0        0        0     8333 2023-04-13 22:09:29.474991 mac_cleanup-3.0.0/mac_cleanup/config.py
+-rw-r--r--   0        0        0      653 2023-04-10 18:13:35.057667 mac_cleanup-3.0.0/mac_cleanup/console.py
+-rw-r--r--   0        0        0     7730 2023-04-13 22:09:29.475076 mac_cleanup-3.0.0/mac_cleanup/core.py
+-rw-r--r--   0        0        0     4257 2023-04-13 13:45:07.200604 mac_cleanup-3.0.0/mac_cleanup/core_modules.py
+-rw-r--r--   0        0        0    14351 2023-04-10 17:33:48.122468 mac_cleanup-3.0.0/mac_cleanup/default_modules.py
+-rw-r--r--   0        0        0     3791 2023-04-10 17:33:48.298687 mac_cleanup-3.0.0/mac_cleanup/error_handling.py
+-rw-r--r--   0        0        0     2918 2023-04-11 04:55:56.810107 mac_cleanup-3.0.0/mac_cleanup/main.py
+-rw-r--r--   0        0        0     1181 2023-04-10 17:33:48.299151 mac_cleanup-3.0.0/mac_cleanup/parser.py
+-rw-r--r--   0        0        0     3380 2023-04-13 13:40:37.272889 mac_cleanup-3.0.0/mac_cleanup/progress.py
+-rwxr-xr-x   0        0        0     3181 2023-04-10 17:33:48.299577 mac_cleanup-3.0.0/mac_cleanup/utils.py
+-rw-r--r--   0        0        0     3217 2023-04-13 22:01:45.095001 mac_cleanup-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4935 1970-01-01 00:00:00.000000 mac_cleanup-3.0.0/PKG-INFO
```

### Comparing `mac_cleanup-2.2.5/LICENSE` & `mac_cleanup-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mac_cleanup-2.2.5/README.md` & `mac_cleanup-3.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 # mac-cleanup-py
 
 [![PyPI](https://img.shields.io/pypi/v/mac_cleanup)](https://pypi.org/project/mac-cleanup/)
 [![Tests](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/tox.yml/badge.svg)](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/tox.yml)
 [![CodeQL](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/codeql.yml/badge.svg)](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/codeql.yml)
 
-### 👨‍💻 Python cleanup script for macOS 
+## 🧹 Python cleanup script for macOS
 
-#### [mac-cleanup-sh](https://github.com/mac-cleanup/mac-cleanup-sh) rewritten in Python
+**mac-cleanup-py** is a powerful cleanup script for macOS.\
+This project is a rewrite of the original [mac-cleanup-sh](https://github.com/mac-cleanup/mac-cleanup-sh) rewritten in Python. 
 
 
-### What does script do?
+## 🚀 Features
 
-1. Cleans Trash
-2. Deletes unnecessary logs & files
-3. Removes cache
+**mac-cleanup-py** helps you:
 
-![mac-cleanup_v2_X_X](https://user-images.githubusercontent.com/44712637/184389183-449cae99-4d40-4ca1-9523-1fb3dcf809dd.gif)
+1. Empty Trash 
+2. Delete unnecessary logs & files 
+3. Clear cache
+
+![mac-cleanup-demo](https://user-images.githubusercontent.com/44712637/231780851-d2197255-e24e-46ba-8355-42bcf588376d.gif)
 
 <details>
    <summary>
-   Default modules
+   📦 Default Modules
    </summary>
 
   </br>
 
   - `adobe` - Clears **Adobe** cache files
   - `android` - Clears **Android** caches
   - `brew` - Clears **Homebrew** cache
   - `cacher` - Clears **Cacher** logs
-  - `chrome` - Clears Google Chrome cache
-  - `composer` - Clears composer cache
-  - `dns_cache` - Clears DNS cache
-  - `docker` - Cleanup dangling **Docker Images** and stopped **containers**
+  - `chrome` - Clears **Google Chrome** cache
+  - `composer` - Clears **composer** cache
+  - `dns_cache` - Clears **DNS** cache
+  - `docker` - Cleanup dangling **Docker** Images and stopped containers
   - `dropbox` - Clears **Dropbox** cache
   - `gem` - Cleanup any old versions of **Gems**
   - `go` - Clears **Go** cache
   - `google_drive` - Clears **Google Drive** caches
   - `gradle` - Clears **Gradle** caches
-  - `inactive_memory` - Purge Inactive Memory
+  - `inactive_memory` - Purge **Inactive Memory**
   - `ios_apps` - Cleanup **iOS Applications**
   - `ios_backups` - Removes **iOS Device Backups**
   - `java_cache` - Removes **Java head dumps** from home directory
-  - `jetbrains` - Removes logs from **PhpStorm**, **PyCharm**  etc
+  - `jetbrains` - Removes logs from **PhpStorm**, **PyCharm** etc
   - `kite` - Deletes **Kite** logs
   - `lunarclient` - Removes **Lunar Client** logs and cache
   - `microsoft_teams` - Remove **Microsoft Teams** logs and cache
   - `minecraft` - Remove **Minecraft** logs and cache
   - `npm` - Cleanup **npm** Cache
   - `pod` - Cleanup **CocoaPods** Cache Files
   - `poetry` - Clears **Poetry** cache
@@ -55,62 +58,70 @@
   - `system_log` - Clear **System Log** Files
   - `trash` - Empty the **Trash** on All Mounted Volumes and the Main HDD
   - `wget_logs` - Remove **Wget** logs and hosts
   - `xcode` - Cleanup **Xcode Derived Data** and **Archives**
   - `xcode_simulators` - Reset **iOS simulators**
   - `yarn` - Cleanup **yarn** Cache
 
-
 </details>
 
 
 
-## Install Automatically
+## 📥 Installation
 
-### Using homebrew
+### Using Homebrew
 
 ```bash
 brew tap mac-cleanup/mac-cleanup-py
 brew install mac-cleanup-py
 ```
 
 ### Using pip
 
 ```bash
 pip3 install mac-cleanup
 ```
 
-## Uninstall
+## 🗑️ Uninstallation
 
-### Using homebrew
+### Using Homebrew
 
 ```bash
 brew uninstall mac-cleanup-py
 brew untap mac-cleanup/mac-cleanup-py
 ```
 
 ### Using pip
 
 ```bash
 pip3 uninstall mac-cleanup
 ```
 
-## Usage Options
+## 💡 Usage Options
 
 Help menu:
 
 ```
 $ mac-cleanup -h
 
-usage: mac-cleanup [-h] [-d] [-u] [-c] [-m]
+usage: mac-cleanup [-h] [-n] [-u] [-c] [-p]
 
     A Mac Cleanup Utility in Python
-    v2.2.5
-    https://github.com/mac-cleanup/mac-cleanup-py
+    3.0.0
+    https://github.com/mac-cleanup/mac-cleanup-py    
+
+options:
+  -h, --help         show this help message and exit
+  -n, --dry-run      Dry run without deleting stuff
+  -u, --update       Update HomeBrew on cleanup
+  -c, --configure    Configure default and custom modules
+  -p, --custom-path  Specify path for custom modules
 
-optional arguments:
-  -h, --help       show this help message and exit
-  -d, --dry-run    Shows approx space to be cleaned
-  -u, --update     Script will update brew while cleaning
-  -c, --configure  Launch modules configuration
-  -m, --modules    Specify custom modules' path
 ```
+
+
+## 🌟 Contributing
+Contributions are always welcome!\
+If you have any ideas, suggestions, or bug reports, feel free to submit an issue or open a pull request.
+
+## 📝 License
+This project is licensed under the [Apache-2.0 License](https://github.com/mac-cleanup/mac-cleanup-py/blob/main/LICENSE).
```

### Comparing `mac_cleanup-2.2.5/mac_cleanup/cli.py` & `mac_cleanup-3.0.0/mac_cleanup/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,90 @@
-from . import *
-from .utils import cmd, bytes_to_human, catch_exception
-from .console import console, print_panel
-from .config import load_config
+from pathlib import Path
 
-t = Collector()
+from mac_cleanup.config import Config
+from mac_cleanup.console import console, print_panel
+from mac_cleanup.core import _Collector
+from mac_cleanup.error_handling import catch_exception
+from mac_cleanup.parser import args
+from mac_cleanup.utils import bytes_to_human, cmd
 
 
-@catch_exception
-def main() -> None:
-    # Clear console at the start
-    console.clear()
+class EntryPoint:
+    config_path = Path.home().joinpath(".mac_cleanup_py")
+    base_collector = _Collector()
 
-    # Sets custom modules' path if user prompted to and exits
-    if args.modules:
-        from .config import set_custom_path
+    @staticmethod
+    def count_free_space() -> float:
+        """Get current free space."""
 
-        set_custom_path()
-        raise KeyboardInterrupt
+        return float(cmd("df / | tail -1 | awk '{print $4}'"))
 
-    # Loads all modules
-    load_config(configuration_needed=args.configure)
+    def cleanup(self) -> None:
+        """Launch cleanup and print results."""
 
-    # Exits if configuration was requested
-    if args.configure:
-        raise KeyboardInterrupt
-
-    def count_free_space(
-    ) -> int:
-        return int(cmd("df / | tail -1 | awk '{print $4}'"))
-
-    def cleanup(
-    ) -> None:
-        from rich.progress import track
+        from mac_cleanup.progress import ProgressBar
 
         # Free space before the run
-        oldAvailable = count_free_space()
+        free_space_before = self.count_free_space()
 
-        # Ask for password input in terminal (sudo -E)
-        # Raises AssertionError if prompt fails
-        assert cmd("sudo -E whoami") == "root"
-
-        for module in t.execute_list:
-            if not module.msg or not module.unit_list:
-                continue
-
-            for unit in track(
-                    module.unit_list,
-                    description=module.msg,
-                    transient=True,
-                    total=len(module.unit_list)
-            ):
-                # Doesn't execute dry run query
-                if unit.dry:
-                    continue
-
-                # If not cmd then add "sudo rm -rf"
-                if not unit.cmd:
-                    unit.command = "sudo rm -rf {0}".format(unit.command.replace(" ", "\ "))  # type: ignore # noqa ignore W605
-
-                # There are no tasks w/o command
-                cmd(unit.command)
+        for unit in self.base_collector._execute_list:  # noqa
+            for module in ProgressBar.wrap_iter(unit.modules, description=unit.message, total=len(unit.modules)):
+                # Call for module execution
+                module._execute()  # noqa
 
         # Free space after the run
-        newAvailable = count_free_space()
+        free_space_after = self.count_free_space()
 
         # Print results
         print_panel(
-            text=f"Removed - [success]{bytes_to_human((newAvailable - oldAvailable) * 1024)}",
+            text=f"Removed - [success]{bytes_to_human((free_space_after - free_space_before) * 1024)}",
             title="[info]Success",
         )
 
-    # Straight to clean up if not dry run
-    if not args.dry_run:
-        cleanup()
-    else:
-        from rich.prompt import Confirm
+    @catch_exception
+    def start(self) -> None:
+        """Start mac_cleanup_py by cleaning console, loading config and parsing argument."""
 
-        freed_space = bytes_to_human(t.count_dry())
+        # Clear console at the start
+        console.clear()
 
-        print_panel(
-            text=f"Approx [success]{freed_space}[/success] will be cleaned",
-            title="[info]Dry run results",
-        )
-        try:
-            if Confirm.ask("Continue?", show_default=False, default="y"):
-                console.clear()
-                cleanup()
-            else:
+        # Get config
+        config = Config(config_path_=self.config_path)
+
+        # Sets custom modules' path if user prompted to and exits
+        if args.custom_path:
+            # Set custom path and exit
+            config.set_custom_path()
+
+        # Check config
+        config(configuration_prompted=args.configure)
+
+        # Handle dry runs
+        if args.dry_run:
+            from rich.prompt import Confirm
+
+            freed_space = bytes_to_human(self.base_collector._count_dry())  # noqa
+
+            print_panel(text=f"Approx [success]{freed_space}[/success] will be cleaned", title="[info]Dry run results")
+
+            try:
+                continue_cleanup = Confirm.ask("Continue?", show_default=False, default="y")
+            # Cyrillic symbols may crash rich.Confirm
+            except UnicodeDecodeError:
                 console.clear()
+                console.print("Do not enter symbols that can't be decoded to UTF-8", style="danger")
                 console.print("Exiting...")
-        # At least Cyrillic symbols will crash rich.Confirm
-        except UnicodeDecodeError:
+                return
+
             console.clear()
-            console.print(
-                "Do not enter symbols that can't be decoded to utf8",
-                style="danger",
-            )
-            console.print("Exiting...")
+
+            # Exit if user doesn't want to continue
+            if not continue_cleanup:
+                console.print("Exiting...")
+                return
+
+        # Clean stuff up
+        self.cleanup()
 
 
 if __name__ == "__main__":
-    main()
+    EntryPoint().start()  # pragma: no cover (coverage marks line as untested)
```

### Comparing `mac_cleanup-2.2.5/setup.py` & `mac_cleanup-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,155 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mac-cleanup
+Version: 3.0.0
+Summary: Python cleanup script for macOS
+Home-page: https://github.com/mac-cleanup/mac-cleanup-py
+License: Apache-2.0
+Keywords: macos,script,cleanup,cleaner
+Author: Drugsosos
+Requires-Python: >=3.10,<3.12
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=22.2.0,<23.0.0)
+Requires-Dist: beartype (>=0.13.1,<0.14.0)
+Requires-Dist: inquirer (>=3.1.3,<4.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Documentation, https://github.com/mac-cleanup/mac-cleanup-py#install-automatically
+Project-URL: Issue Tracker, https://github.com/mac-cleanup/mac-cleanup-py/issues
+Project-URL: Repository, https://github.com/mac-cleanup/mac-cleanup-py
+Description-Content-Type: text/markdown
+
+# mac-cleanup-py
+
+[![PyPI](https://img.shields.io/pypi/v/mac_cleanup)](https://pypi.org/project/mac-cleanup/)
+[![Tests](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/tox.yml/badge.svg)](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/tox.yml)
+[![CodeQL](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/codeql.yml/badge.svg)](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/codeql.yml)
+
+## 🧹 Python cleanup script for macOS
+
+**mac-cleanup-py** is a powerful cleanup script for macOS.\
+This project is a rewrite of the original [mac-cleanup-sh](https://github.com/mac-cleanup/mac-cleanup-sh) rewritten in Python. 
+
+
+## 🚀 Features
+
+**mac-cleanup-py** helps you:
+
+1. Empty Trash 
+2. Delete unnecessary logs & files 
+3. Clear cache
+
+![mac-cleanup-demo](https://user-images.githubusercontent.com/44712637/231780851-d2197255-e24e-46ba-8355-42bcf588376d.gif)
+
+<details>
+   <summary>
+   📦 Default Modules
+   </summary>
+
+  </br>
+
+  - `adobe` - Clears **Adobe** cache files
+  - `android` - Clears **Android** caches
+  - `brew` - Clears **Homebrew** cache
+  - `cacher` - Clears **Cacher** logs
+  - `chrome` - Clears **Google Chrome** cache
+  - `composer` - Clears **composer** cache
+  - `dns_cache` - Clears **DNS** cache
+  - `docker` - Cleanup dangling **Docker** Images and stopped containers
+  - `dropbox` - Clears **Dropbox** cache
+  - `gem` - Cleanup any old versions of **Gems**
+  - `go` - Clears **Go** cache
+  - `google_drive` - Clears **Google Drive** caches
+  - `gradle` - Clears **Gradle** caches
+  - `inactive_memory` - Purge **Inactive Memory**
+  - `ios_apps` - Cleanup **iOS Applications**
+  - `ios_backups` - Removes **iOS Device Backups**
+  - `java_cache` - Removes **Java head dumps** from home directory
+  - `jetbrains` - Removes logs from **PhpStorm**, **PyCharm** etc
+  - `kite` - Deletes **Kite** logs
+  - `lunarclient` - Removes **Lunar Client** logs and cache
+  - `microsoft_teams` - Remove **Microsoft Teams** logs and cache
+  - `minecraft` - Remove **Minecraft** logs and cache
+  - `npm` - Cleanup **npm** Cache
+  - `pod` - Cleanup **CocoaPods** Cache Files
+  - `poetry` - Clears **Poetry** cache
+  - `pyenv` - Cleanup **Pyenv-VirtualEnv** Cache
+  - `steam` - Remove **Steam** logs and cache
+  - `system_caches` - Clear **System cache**
+  - `system_log` - Clear **System Log** Files
+  - `trash` - Empty the **Trash** on All Mounted Volumes and the Main HDD
+  - `wget_logs` - Remove **Wget** logs and hosts
+  - `xcode` - Cleanup **Xcode Derived Data** and **Archives**
+  - `xcode_simulators` - Reset **iOS simulators**
+  - `yarn` - Cleanup **yarn** Cache
+
+</details>
+
+
+
+## 📥 Installation
+
+### Using Homebrew
+
+```bash
+brew tap mac-cleanup/mac-cleanup-py
+brew install mac-cleanup-py
+```
+
+### Using pip
+
+```bash
+pip3 install mac-cleanup
+```
+
+## 🗑️ Uninstallation
+
+### Using Homebrew
+
+```bash
+brew uninstall mac-cleanup-py
+brew untap mac-cleanup/mac-cleanup-py
+```
+
+### Using pip
+
+```bash
+pip3 uninstall mac-cleanup
+```
+
+## 💡 Usage Options
+
+Help menu:
+
+```
+$ mac-cleanup -h
+
+usage: mac-cleanup [-h] [-n] [-u] [-c] [-p]
+
+    A Mac Cleanup Utility in Python
+    3.0.0
+    https://github.com/mac-cleanup/mac-cleanup-py    
+
+options:
+  -h, --help         show this help message and exit
+  -n, --dry-run      Dry run without deleting stuff
+  -u, --update       Update HomeBrew on cleanup
+  -c, --configure    Configure default and custom modules
+  -p, --custom-path  Specify path for custom modules
+
+```
+
+
+## 🌟 Contributing
+Contributions are always welcome!\
+If you have any ideas, suggestions, or bug reports, feel free to submit an issue or open a pull request.
 
-packages = \
-['mac_cleanup']
+## 📝 License
+This project is licensed under the [Apache-2.0 License](https://github.com/mac-cleanup/mac-cleanup-py/blob/main/LICENSE).
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=22.1.0,<23.0.0',
- 'inquirer>=2.10.0,<3.0.0',
- 'rich>=12.2,<14.0',
- 'toml>=0.10.2,<0.11.0']
-
-entry_points = \
-{'console_scripts': ['mac-cleanup = mac_cleanup:main']}
-
-setup_kwargs = {
-    'name': 'mac-cleanup',
-    'version': '2.2.5',
-    'description': 'Python cleanup script for macOS',
-    'long_description': "# mac-cleanup-py\n\n[![PyPI](https://img.shields.io/pypi/v/mac_cleanup)](https://pypi.org/project/mac-cleanup/)\n[![Tests](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/tox.yml/badge.svg)](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/tox.yml)\n[![CodeQL](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/codeql.yml/badge.svg)](https://github.com/mac-cleanup/mac-cleanup-py/actions/workflows/codeql.yml)\n\n### 👨\u200d💻 Python cleanup script for macOS \n\n#### [mac-cleanup-sh](https://github.com/mac-cleanup/mac-cleanup-sh) rewritten in Python\n\n\n### What does script do?\n\n1. Cleans Trash\n2. Deletes unnecessary logs & files\n3. Removes cache\n\n![mac-cleanup_v2_X_X](https://user-images.githubusercontent.com/44712637/184389183-449cae99-4d40-4ca1-9523-1fb3dcf809dd.gif)\n\n<details>\n   <summary>\n   Default modules\n   </summary>\n\n  </br>\n\n  - `adobe` - Clears **Adobe** cache files\n  - `android` - Clears **Android** caches\n  - `brew` - Clears **Homebrew** cache\n  - `cacher` - Clears **Cacher** logs\n  - `chrome` - Clears Google Chrome cache\n  - `composer` - Clears composer cache\n  - `dns_cache` - Clears DNS cache\n  - `docker` - Cleanup dangling **Docker Images** and stopped **containers**\n  - `dropbox` - Clears **Dropbox** cache\n  - `gem` - Cleanup any old versions of **Gems**\n  - `go` - Clears **Go** cache\n  - `google_drive` - Clears **Google Drive** caches\n  - `gradle` - Clears **Gradle** caches\n  - `inactive_memory` - Purge Inactive Memory\n  - `ios_apps` - Cleanup **iOS Applications**\n  - `ios_backups` - Removes **iOS Device Backups**\n  - `java_cache` - Removes **Java head dumps** from home directory\n  - `jetbrains` - Removes logs from **PhpStorm**, **PyCharm**  etc\n  - `kite` - Deletes **Kite** logs\n  - `lunarclient` - Removes **Lunar Client** logs and cache\n  - `microsoft_teams` - Remove **Microsoft Teams** logs and cache\n  - `minecraft` - Remove **Minecraft** logs and cache\n  - `npm` - Cleanup **npm** Cache\n  - `pod` - Cleanup **CocoaPods** Cache Files\n  - `poetry` - Clears **Poetry** cache\n  - `pyenv` - Cleanup **Pyenv-VirtualEnv** Cache\n  - `steam` - Remove **Steam** logs and cache\n  - `system_caches` - Clear **System cache**\n  - `system_log` - Clear **System Log** Files\n  - `trash` - Empty the **Trash** on All Mounted Volumes and the Main HDD\n  - `wget_logs` - Remove **Wget** logs and hosts\n  - `xcode` - Cleanup **Xcode Derived Data** and **Archives**\n  - `xcode_simulators` - Reset **iOS simulators**\n  - `yarn` - Cleanup **yarn** Cache\n\n\n</details>\n\n\n\n## Install Automatically\n\n### Using homebrew\n\n```bash\nbrew tap mac-cleanup/mac-cleanup-py\nbrew install mac-cleanup-py\n```\n\n### Using pip\n\n```bash\npip3 install mac-cleanup\n```\n\n## Uninstall\n\n### Using homebrew\n\n```bash\nbrew uninstall mac-cleanup-py\nbrew untap mac-cleanup/mac-cleanup-py\n```\n\n### Using pip\n\n```bash\npip3 uninstall mac-cleanup\n```\n\n## Usage Options\n\nHelp menu:\n\n```\n$ mac-cleanup -h\n\nusage: mac-cleanup [-h] [-d] [-u] [-c] [-m]\n\n    A Mac Cleanup Utility in Python\n    v2.2.5\n    https://github.com/mac-cleanup/mac-cleanup-py\n\noptional arguments:\n  -h, --help       show this help message and exit\n  -d, --dry-run    Shows approx space to be cleaned\n  -u, --update     Script will update brew while cleaning\n  -c, --configure  Launch modules configuration\n  -m, --modules    Specify custom modules' path\n```\n",
-    'author': 'Drugsosos',
-    'author_email': '44712637+Drugsosos@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/mac-cleanup/mac-cleanup-py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

