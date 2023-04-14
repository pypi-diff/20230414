# Comparing `tmp/shell-tools-1.0.2.tar.gz` & `tmp/shell-tools-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell-tools-1.0.2.tar", last modified: Mon Oct 24 19:48:04 2022, max compression
+gzip compressed data, was "shell-tools-1.1.7.tar", last modified: Fri Apr 14 20:16:59 2023, max compression
```

## Comparing `shell-tools-1.0.2.tar` & `shell-tools-1.1.7.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-10-24 19:48:04.348016 shell-tools-1.0.2/
--rw-rw-rw-   0        0        0     1092 2022-10-22 15:21:38.000000 shell-tools-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      747 2022-10-24 19:48:04.348016 shell-tools-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      250 2022-10-24 19:44:09.000000 shell-tools-1.0.2/README.md
--rw-rw-rw-   0        0        0      217 2022-10-22 15:31:18.000000 shell-tools-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      755 2022-10-24 19:48:04.352015 shell-tools-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0       75 2022-10-22 14:57:09.000000 shell-tools-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-24 19:48:04.333018 shell-tools-1.0.2/shell_tools/
--rw-rw-rw-   0        0        0        0 2022-10-22 18:10:45.000000 shell-tools-1.0.2/shell_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-24 19:48:04.346016 shell-tools-1.0.2/shell_tools/dirs/
--rw-rw-rw-   0        0        0      120 2022-10-23 15:43:54.000000 shell-tools-1.0.2/shell_tools/dirs/__init__.py
--rw-rw-rw-   0        0        0     2863 2022-10-24 19:44:33.000000 shell-tools-1.0.2/shell_tools/dirs/find_empty_dirs.py
-drwxrwxrwx   0        0        0        0 2022-10-24 19:48:04.347015 shell-tools-1.0.2/shell_tools/files/
--rw-rw-rw-   0        0        0      114 2022-10-22 20:58:23.000000 shell-tools-1.0.2/shell_tools/files/__init__.py
--rw-rw-rw-   0        0        0     2420 2022-10-24 19:44:33.000000 shell-tools-1.0.2/shell_tools/files/generate_file.py
-drwxrwxrwx   0        0        0        0 2022-10-24 19:48:04.345016 shell-tools-1.0.2/shell_tools.egg-info/
--rw-rw-rw-   0        0        0      747 2022-10-24 19:48:04.000000 shell-tools-1.0.2/shell_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2022-10-24 19:48:04.000000 shell-tools-1.0.2/shell_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-24 19:48:04.000000 shell-tools-1.0.2/shell_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2022-10-24 19:48:04.000000 shell-tools-1.0.2/shell_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2022-10-24 19:48:04.000000 shell-tools-1.0.2/shell_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-10-24 19:48:04.000000 shell-tools-1.0.2/shell_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.121035 shell-tools-1.1.7/
+-rw-rw-rw-   0        0        0     1092 2022-10-22 15:21:38.000000 shell-tools-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0      813 2023-04-14 20:16:59.121035 shell-tools-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2022-10-31 12:41:27.000000 shell-tools-1.1.7/README.md
+-rw-rw-rw-   0        0        0      217 2022-10-22 15:31:18.000000 shell-tools-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      790 2023-04-14 20:16:59.122035 shell-tools-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0       75 2022-10-22 14:57:09.000000 shell-tools-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.113035 shell-tools-1.1.7/shell_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-14 17:42:52.000000 shell-tools-1.1.7/shell_tools/__init__.py
+-rw-rw-rw-   0        0        0     4714 2023-04-14 19:43:59.000000 shell-tools-1.1.7/shell_tools/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.118035 shell-tools-1.1.7/shell_tools/dirs/
+-rw-rw-rw-   0        0        0        0 2023-04-14 17:43:35.000000 shell-tools-1.1.7/shell_tools/dirs/__init__.py
+-rw-rw-rw-   0        0        0      734 2023-04-14 20:14:05.000000 shell-tools-1.1.7/shell_tools/dirs/search.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.119036 shell-tools-1.1.7/shell_tools/files/
+-rw-rw-rw-   0        0        0        0 2023-04-14 17:37:14.000000 shell-tools-1.1.7/shell_tools/files/__init__.py
+-rw-rw-rw-   0        0        0     1092 2023-04-14 18:44:31.000000 shell-tools-1.1.7/shell_tools/files/random.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.120035 shell-tools-1.1.7/shell_tools/git/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:00:31.000000 shell-tools-1.1.7/shell_tools/git/__init__.py
+-rw-rw-rw-   0        0        0     1089 2023-04-14 19:43:59.000000 shell-tools-1.1.7/shell_tools/git/misc.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:16:59.117035 shell-tools-1.1.7/shell_tools.egg-info/
+-rw-rw-rw-   0        0        0      813 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 20:16:59.000000 shell-tools-1.1.7/shell_tools.egg-info/top_level.txt
```

### Comparing `shell-tools-1.0.2/LICENSE` & `shell-tools-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shell-tools-1.0.2/PKG-INFO` & `shell-tools-1.1.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-tools
-Version: 1.0.2
+Version: 1.1.7
 Summary: set of python applications/scripts for different purposes
 Home-page: https://github.com/stanykey/shell-tools
 Author: Sergii Lovygin
 Author-email: sergey.lovygin@yahoo.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,7 +16,8 @@
 # Shell Tools
 
 The package contains a set of small CLIs for different purposes.
 
 ## List of applications:
 - **generate-file**: allowing to generate files with random 'trash'
 - **find-empty-dir**: allowing find empty dirs and apply some actions
+- **sync-repos**: allowing to sync multiple repositories at once
```

### Comparing `shell-tools-1.0.2/setup.cfg` & `shell-tools-1.1.7/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6865 6c6c 2d74 6f6f 6c73 0d0a   = shell-tools..
-00000020: 7665 7273 696f 6e20 3d20 312e 302e 320d  version = 1.0.2.
+00000020: 7665 7273 696f 6e20 3d20 312e 312e 370d  version = 1.1.7.
 00000030: 0a61 7574 686f 7220 3d20 5365 7267 6969  .author = Sergii
 00000040: 204c 6f76 7967 696e 0d0a 6175 7468 6f72   Lovygin..author
 00000050: 5f65 6d61 696c 203d 2073 6572 6765 792e  _email = sergey.
 00000060: 6c6f 7679 6769 6e40 7961 686f 6f2e 636f  lovygin@yahoo.co
 00000070: 6d0d 0a73 756d 6d61 7279 203d 2073 6574  m..summary = set
 00000080: 206f 6620 7079 7468 6f6e 2061 7070 6c69   of python appli
 00000090: 6361 7469 6f6e 732f 7363 7269 7074 7320  cations/scripts 
@@ -33,16 +33,18 @@
 00000200: 6573 203d 203e 3d33 2e31 300d 0a69 6e73  es = >=3.10..ins
 00000210: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
 00000220: 0d0a 0963 6c69 636b 0d0a 0d0a 5b6f 7074  ...click....[opt
 00000230: 696f 6e73 2e65 6e74 7279 5f70 6f69 6e74  ions.entry_point
 00000240: 735d 0d0a 636f 6e73 6f6c 655f 7363 7269  s]..console_scri
 00000250: 7074 7320 3d20 0d0a 0967 656e 6572 6174  pts = ...generat
 00000260: 652d 6669 6c65 203d 2073 6865 6c6c 5f74  e-file = shell_t
-00000270: 6f6f 6c73 2e66 696c 6573 2e67 656e 6572  ools.files.gener
-00000280: 6174 655f 6669 6c65 3a63 6c69 0d0a 0966  ate_file:cli...f
-00000290: 696e 642d 656d 7074 792d 6469 7273 203d  ind-empty-dirs =
-000002a0: 2073 6865 6c6c 5f74 6f6f 6c73 2e64 6972   shell_tools.dir
-000002b0: 732e 6669 6e64 5f65 6d70 7479 5f64 6972  s.find_empty_dir
-000002c0: 733a 636c 690d 0a0d 0a5b 6567 675f 696e  s:cli....[egg_in
-000002d0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000002e0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000002f0: 0a0d 0a                                  ...
+00000270: 6f6f 6c73 2e63 6c69 3a67 656e 6572 6174  ools.cli:generat
+00000280: 655f 6669 6c65 0d0a 0966 696e 642d 656d  e_file...find-em
+00000290: 7074 792d 6469 7273 203d 2073 6865 6c6c  pty-dirs = shell
+000002a0: 5f74 6f6f 6c73 2e63 6c69 3a64 6973 636f  _tools.cli:disco
+000002b0: 7665 725f 656d 7074 795f 6469 7273 0d0a  ver_empty_dirs..
+000002c0: 0973 796e 632d 7265 706f 7320 3d20 7368  .sync-repos = sh
+000002d0: 656c 6c5f 746f 6f6c 732e 636c 693a 7379  ell_tools.cli:sy
+000002e0: 6e63 5f72 6570 6f73 0d0a 0d0a 5b65 6767  nc_repos....[egg
+000002f0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000300: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000310: 2030 0d0a 0d0a                            0....
```

### Comparing `shell-tools-1.0.2/shell_tools.egg-info/PKG-INFO` & `shell-tools-1.1.7/shell_tools.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-tools
-Version: 1.0.2
+Version: 1.1.7
 Summary: set of python applications/scripts for different purposes
 Home-page: https://github.com/stanykey/shell-tools
 Author: Sergii Lovygin
 Author-email: sergey.lovygin@yahoo.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,7 +16,8 @@
 # Shell Tools
 
 The package contains a set of small CLIs for different purposes.
 
 ## List of applications:
 - **generate-file**: allowing to generate files with random 'trash'
 - **find-empty-dir**: allowing find empty dirs and apply some actions
+- **sync-repos**: allowing to sync multiple repositories at once
```

