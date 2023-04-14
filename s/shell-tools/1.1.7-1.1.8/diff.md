# Comparing `tmp/shell-tools-1.1.7.tar.gz` & `tmp/shell-tools-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell-tools-1.1.7.tar", last modified: Fri Apr 14 20:16:59 2023, max compression
+gzip compressed data, was "shell-tools-1.1.8.tar", last modified: Fri Apr 14 20:30:55 2023, max compression
```

## Comparing `shell-tools-1.1.7.tar` & `shell-tools-1.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.121035 shell-tools-1.1.7/
--rw-rw-rw-   0        0        0     1092 2022-10-22 15:21:38.000000 shell-tools-1.1.7/LICENSE
--rw-rw-rw-   0        0        0      813 2023-04-14 20:16:59.121035 shell-tools-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      317 2022-10-31 12:41:27.000000 shell-tools-1.1.7/README.md
--rw-rw-rw-   0        0        0      217 2022-10-22 15:31:18.000000 shell-tools-1.1.7/pyproject.toml
--rw-rw-rw-   0        0        0      790 2023-04-14 20:16:59.122035 shell-tools-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0       75 2022-10-22 14:57:09.000000 shell-tools-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.113035 shell-tools-1.1.7/shell_tools/
--rw-rw-rw-   0        0        0        0 2023-04-14 17:42:52.000000 shell-tools-1.1.7/shell_tools/__init__.py
--rw-rw-rw-   0        0        0     4714 2023-04-14 19:43:59.000000 shell-tools-1.1.7/shell_tools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.118035 shell-tools-1.1.7/shell_tools/dirs/
--rw-rw-rw-   0        0        0        0 2023-04-14 17:43:35.000000 shell-tools-1.1.7/shell_tools/dirs/__init__.py
--rw-rw-rw-   0        0        0      734 2023-04-14 20:14:05.000000 shell-tools-1.1.7/shell_tools/dirs/search.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.119036 shell-tools-1.1.7/shell_tools/files/
--rw-rw-rw-   0        0        0        0 2023-04-14 17:37:14.000000 shell-tools-1.1.7/shell_tools/files/__init__.py
--rw-rw-rw-   0        0        0     1092 2023-04-14 18:44:31.000000 shell-tools-1.1.7/shell_tools/files/random.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.120035 shell-tools-1.1.7/shell_tools/git/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:00:31.000000 shell-tools-1.1.7/shell_tools/git/__init__.py
--rw-rw-rw-   0        0        0     1089 2023-04-14 19:43:59.000000 shell-tools-1.1.7/shell_tools/git/misc.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.117035 shell-tools-1.1.7/shell_tools.egg-info/
--rw-rw-rw-   0        0        0      813 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 20:30:55.470859 shell-tools-1.1.8/
+-rw-rw-rw-   0        0        0     1092 2022-10-22 15:21:38.000000 shell-tools-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0      813 2023-04-14 20:30:55.470859 shell-tools-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2022-10-31 12:41:27.000000 shell-tools-1.1.8/README.md
+-rw-rw-rw-   0        0        0      217 2022-10-22 15:31:18.000000 shell-tools-1.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0      790 2023-04-14 20:30:55.471857 shell-tools-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0       75 2022-10-22 14:57:09.000000 shell-tools-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:30:55.462857 shell-tools-1.1.8/shell_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-14 17:42:52.000000 shell-tools-1.1.8/shell_tools/__init__.py
+-rw-rw-rw-   0        0        0     4714 2023-04-14 19:43:59.000000 shell-tools-1.1.8/shell_tools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:30:55.467857 shell-tools-1.1.8/shell_tools/dirs/
+-rw-rw-rw-   0        0        0        0 2023-04-14 17:43:35.000000 shell-tools-1.1.8/shell_tools/dirs/__init__.py
+-rw-rw-rw-   0        0        0      847 2023-04-14 20:27:47.000000 shell-tools-1.1.8/shell_tools/dirs/search.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:30:55.468857 shell-tools-1.1.8/shell_tools/files/
+-rw-rw-rw-   0        0        0        0 2023-04-14 17:37:14.000000 shell-tools-1.1.8/shell_tools/files/__init__.py
+-rw-rw-rw-   0        0        0     1106 2023-04-14 20:26:28.000000 shell-tools-1.1.8/shell_tools/files/random.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:30:55.469856 shell-tools-1.1.8/shell_tools/git/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:00:31.000000 shell-tools-1.1.8/shell_tools/git/__init__.py
+-rw-rw-rw-   0        0        0     1167 2023-04-14 20:23:00.000000 shell-tools-1.1.8/shell_tools/git/misc.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:30:55.466857 shell-tools-1.1.8/shell_tools.egg-info/
+-rw-rw-rw-   0        0        0      813 2023-04-14 20:30:55.000000 shell-tools-1.1.8/shell_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-04-14 20:30:55.000000 shell-tools-1.1.8/shell_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 20:30:55.000000 shell-tools-1.1.8/shell_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-04-14 20:30:55.000000 shell-tools-1.1.8/shell_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 20:30:55.000000 shell-tools-1.1.8/shell_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 20:30:55.000000 shell-tools-1.1.8/shell_tools.egg-info/top_level.txt
```

### Comparing `shell-tools-1.1.7/LICENSE` & `shell-tools-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shell-tools-1.1.7/PKG-INFO` & `shell-tools-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-tools
-Version: 1.1.7
+Version: 1.1.8
 Summary: set of python applications/scripts for different purposes
 Home-page: https://github.com/stanykey/shell-tools
 Author: Sergii Lovygin
 Author-email: sergey.lovygin@yahoo.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shell-tools-1.1.7/setup.cfg` & `shell-tools-1.1.8/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6865 6c6c 2d74 6f6f 6c73 0d0a   = shell-tools..
-00000020: 7665 7273 696f 6e20 3d20 312e 312e 370d  version = 1.1.7.
+00000020: 7665 7273 696f 6e20 3d20 312e 312e 380d  version = 1.1.8.
 00000030: 0a61 7574 686f 7220 3d20 5365 7267 6969  .author = Sergii
 00000040: 204c 6f76 7967 696e 0d0a 6175 7468 6f72   Lovygin..author
 00000050: 5f65 6d61 696c 203d 2073 6572 6765 792e  _email = sergey.
 00000060: 6c6f 7679 6769 6e40 7961 686f 6f2e 636f  lovygin@yahoo.co
 00000070: 6d0d 0a73 756d 6d61 7279 203d 2073 6574  m..summary = set
 00000080: 206f 6620 7079 7468 6f6e 2061 7070 6c69   of python appli
 00000090: 6361 7469 6f6e 732f 7363 7269 7074 7320  cations/scripts
```

### Comparing `shell-tools-1.1.7/shell_tools/cli.py` & `shell-tools-1.1.8/shell_tools/cli.py`

 * *Files identical despite different names*

### Comparing `shell-tools-1.1.7/shell_tools/dirs/search.py` & `shell-tools-1.1.8/shell_tools/dirs/search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from os import PathLike
 from pathlib import Path
 
 
-def find_empty_dirs(root: Path, ignore_empty_files: bool = False) -> list[Path]:
+def find_empty_dirs(root: str | PathLike[str], ignore_empty_files: bool = False) -> list[Path]:
     """Find all empty dirs recursively from given `root` directory."""
-    result = []
+    root = Path(root)
+    if not root.is_dir():
+        return list()
 
+    result = []
     items = [path for path in root.iterdir()]
     dirs = [path for path in items if path.is_dir()]
     if not dirs:
         files = [path for path in items if path.is_file()]
         if not files:
             result.append(root)
         elif ignore_empty_files:
```

### Comparing `shell-tools-1.1.7/shell_tools/files/random.py` & `shell-tools-1.1.8/shell_tools/files/random.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pathlib import Path
+from os import PathLike
 from random import choice
 from string import ascii_uppercase
 from string import digits
 from typing import TextIO
 
 
 def make_trash_string(size: int = 1024, allowed_chars: str = ascii_uppercase + digits) -> str:
@@ -18,11 +18,11 @@
         io.write(generated_line)
 
     if remains:
         generated_line = make_trash_string(remains - 1) + "\n"
         io.write(generated_line)
 
 
-def make_random_file(path: Path, size: int, line_length: int = 1024) -> None:
+def make_random_file(path: str | PathLike[str], size: int, line_length: int = 1024) -> None:
     """Write random data to the `file` in the amount equal to `size`."""
     with open(path, "w") as file:
         write_random_data(file, size, line_length)
```

### Comparing `shell-tools-1.1.7/shell_tools/git/misc.py` & `shell-tools-1.1.8/shell_tools/git/misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+from os import PathLike
 from pathlib import Path
 from subprocess import PIPE
 from subprocess import Popen
 
 
-def find_repositories(root: Path, recursive: bool = False) -> list[Path]:
+def find_repositories(root: str | PathLike[str], recursive: bool = False) -> list[Path]:
     """
     Find all git repositories in `root` directory.
 
     The main criterion is the presence of the **.git** directory inside.
     """
+    root = Path(root)
     if not root.is_dir():
         return list()
 
     pattern = r"**/.git" if recursive else r"*/.git"
     return [folder.parent for folder in root.glob(pattern)]
 
 
 def execute_command(*arguments: str) -> list[str]:
     """Execute `arguments` as the single shell command."""
     with Popen(arguments, stdout=PIPE) as shell:
         stdout, _ = shell.communicate()
         return stdout.decode("utf-8").strip().split("\n")
 
 
-def update_repository(path: Path, submodules: bool) -> list[str]:
+def update_repository(path: str | PathLike[str], submodules: bool) -> list[str]:
     """Pull the latest changes for given repository at `path`."""
     output = execute_command("git", "-C", str(path), "pull")
     if submodules:
         output += execute_command("git", "-C", str(path), "submodule", "update", "--init", "--recursive")
     return output
```

### Comparing `shell-tools-1.1.7/shell_tools.egg-info/PKG-INFO` & `shell-tools-1.1.8/shell_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-tools
-Version: 1.1.7
+Version: 1.1.8
 Summary: set of python applications/scripts for different purposes
 Home-page: https://github.com/stanykey/shell-tools
 Author: Sergii Lovygin
 Author-email: sergey.lovygin@yahoo.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

