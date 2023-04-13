# Comparing `tmp/llvm-installer-1.2.8.tar.gz` & `tmp/llvm-installer-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llvm-installer-1.2.8.tar", last modified: Sat Apr  8 06:23:23 2023, max compression
+gzip compressed data, was "llvm-installer-1.2.9.tar", last modified: Wed Apr 12 07:39:14 2023, max compression
```

## Comparing `llvm-installer-1.2.8.tar` & `llvm-installer-1.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-04-08 06:23:23.848201 llvm-installer-1.2.8/
--rw-r--r--   0 mikhail    (503) staff       (20)    11358 2022-05-26 15:06:09.000000 llvm-installer-1.2.8/LICENSE
--rw-r--r--   0 mikhail    (503) staff       (20)      989 2023-04-08 06:23:23.848061 llvm-installer-1.2.8/PKG-INFO
--rw-r--r--   0 mikhail    (503) staff       (20)      643 2022-07-07 03:18:16.000000 llvm-installer-1.2.8/README.md
--rw-r--r--   0 mikhail    (503) staff       (20)       38 2023-04-08 06:23:23.848256 llvm-installer-1.2.8/setup.cfg
--rw-r--r--   0 mikhail    (503) staff       (20)     2235 2023-04-08 06:23:09.000000 llvm-installer-1.2.8/setup.py
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-04-08 06:23:23.845205 llvm-installer-1.2.8/src/
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-04-08 06:23:23.846725 llvm-installer-1.2.8/src/llvm_installer/
--rw-r--r--   0 mikhail    (503) staff       (20)    11455 2022-08-17 05:24:37.000000 llvm-installer-1.2.8/src/llvm_installer/__init__.py
--rw-r--r--   0 mikhail    (503) staff       (20)     1641 2022-07-07 03:54:15.000000 llvm-installer-1.2.8/src/llvm_installer/__main__.py
--rw-r--r--   0 mikhail    (503) staff       (20)        0 2022-05-26 15:06:09.000000 llvm-installer-1.2.8/src/llvm_installer/py.typed
--rw-r--r--   0 mikhail    (503) staff       (20)    68302 2023-04-08 06:22:37.000000 llvm-installer-1.2.8/src/llvm_installer/release_tags.json
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-04-08 06:23:23.847844 llvm-installer-1.2.8/src/llvm_installer.egg-info/
--rw-r--r--   0 mikhail    (503) staff       (20)      989 2023-04-08 06:23:23.000000 llvm-installer-1.2.8/src/llvm_installer.egg-info/PKG-INFO
--rw-r--r--   0 mikhail    (503) staff       (20)      407 2023-04-08 06:23:23.000000 llvm-installer-1.2.8/src/llvm_installer.egg-info/SOURCES.txt
--rw-r--r--   0 mikhail    (503) staff       (20)        1 2023-04-08 06:23:23.000000 llvm-installer-1.2.8/src/llvm_installer.egg-info/dependency_links.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       64 2023-04-08 06:23:23.000000 llvm-installer-1.2.8/src/llvm_installer.egg-info/entry_points.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       86 2023-04-08 06:23:23.000000 llvm-installer-1.2.8/src/llvm_installer.egg-info/requires.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       15 2023-04-08 06:23:23.000000 llvm-installer-1.2.8/src/llvm_installer.egg-info/top_level.txt
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-04-12 07:39:14.351849 llvm-installer-1.2.9/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11358 2022-05-26 15:06:09.000000 llvm-installer-1.2.9/LICENSE
+-rw-r--r--   0 mikhail    (503) staff       (20)     1026 2023-04-12 07:39:14.351736 llvm-installer-1.2.9/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      643 2022-07-07 03:18:16.000000 llvm-installer-1.2.9/README.md
+-rw-r--r--   0 mikhail    (503) staff       (20)       38 2023-04-12 07:39:14.351896 llvm-installer-1.2.9/setup.cfg
+-rw-r--r--   0 mikhail    (503) staff       (20)     2235 2023-04-12 07:38:45.000000 llvm-installer-1.2.9/setup.py
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-04-12 07:39:14.349249 llvm-installer-1.2.9/src/
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-04-12 07:39:14.350619 llvm-installer-1.2.9/src/llvm_installer/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11455 2022-08-17 05:24:37.000000 llvm-installer-1.2.9/src/llvm_installer/__init__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)     1641 2022-07-07 03:54:15.000000 llvm-installer-1.2.9/src/llvm_installer/__main__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)        0 2022-05-26 15:06:09.000000 llvm-installer-1.2.9/src/llvm_installer/py.typed
+-rw-r--r--   0 mikhail    (503) staff       (20)    70058 2023-04-12 07:24:35.000000 llvm-installer-1.2.9/src/llvm_installer/release_tags.json
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2023-04-12 07:39:14.351541 llvm-installer-1.2.9/src/llvm_installer.egg-info/
+-rw-r--r--   0 mikhail    (503) staff       (20)     1026 2023-04-12 07:39:14.000000 llvm-installer-1.2.9/src/llvm_installer.egg-info/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      407 2023-04-12 07:39:14.000000 llvm-installer-1.2.9/src/llvm_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)        1 2023-04-12 07:39:14.000000 llvm-installer-1.2.9/src/llvm_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       65 2023-04-12 07:39:14.000000 llvm-installer-1.2.9/src/llvm_installer.egg-info/entry_points.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       86 2023-04-12 07:39:14.000000 llvm-installer-1.2.9/src/llvm_installer.egg-info/requires.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       15 2023-04-12 07:39:14.000000 llvm-installer-1.2.9/src/llvm_installer.egg-info/top_level.txt
```

### Comparing `llvm-installer-1.2.8/LICENSE` & `llvm-installer-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.2.8/PKG-INFO` & `llvm-installer-1.2.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: llvm-installer
-Version: 1.2.8
+Version: 1.2.9
 Summary: Allows installing pre-built LLVM packages for various operating systems
 Home-page: https://github.com/yugabyte/llvm-installer
 Author: Mikhail Bautin
 Author-email: mbautin@users.noreply.github.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # llvm-installer
 
 https://pypi.org/project/llvm-installer/
@@ -31,7 +33,9 @@
 ```
 
 ## Command-line usage
 
 ```bash
 python3 -m llvm_installer
 ```
+
+
```

### Comparing `llvm-installer-1.2.8/README.md` & `llvm-installer-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.2.8/setup.py` & `llvm-installer-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from os import path
     this_directory = path.abspath(path.dirname(__file__))
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as readme_file:
         long_description = readme_file.read()
 
     setup(
         name='llvm-installer',
-        version='1.2.8',
+        version='1.2.9',
         url='https://github.com/yugabyte/llvm-installer',
         author='Mikhail Bautin',
         author_email='mbautin@users.noreply.github.com',
         description='Allows installing pre-built LLVM packages for various operating systems',
         packages=find_packages(where='src'),
         package_dir={"": "src"},
         package_data={'llvm_installer': ['py.typed', 'release_tags.json']},
```

### Comparing `llvm-installer-1.2.8/src/llvm_installer/__init__.py` & `llvm-installer-1.2.9/src/llvm_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.2.8/src/llvm_installer/__main__.py` & `llvm-installer-1.2.9/src/llvm_installer/__main__.py`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.2.8/src/llvm_installer/release_tags.json` & `llvm-installer-1.2.9/src/llvm_installer/release_tags.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'parsed_tags'": "{insert: [(102, OrderedDict([('architecture', 'aarch64'), "*

 * *                  "('is_old_tag_without_os_and_arch', False), ('major_version', 15), "*

 * *                  "('minor_version', 0), ('patch_version', 7), ('sha1_prefix', '6b9d30d8'), "*

 * *                  "('short_os_name_and_version', 'almalinux9'), ('tag', "*

 * *                  "'v15.0.7-yb-1-1681174901-6b9d30d8-almalinux9-aarch64'), ('timestamp', "*

 * *                  "'1681174901'), ('version', '15.0.7'), ('version_suffix', 'yb-1'), "*

 * * […]*

```diff
@@ -1429,14 +1429,42 @@
             "yb_suffix_version": 1
         },
         {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 15,
             "minor_version": 0,
+            "patch_version": 7,
+            "sha1_prefix": "6b9d30d8",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v15.0.7-yb-1-1681174901-6b9d30d8-almalinux9-aarch64",
+            "timestamp": "1681174901",
+            "version": "15.0.7",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 15,
+            "minor_version": 0,
+            "patch_version": 7,
+            "sha1_prefix": "6b9d30d8",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v15.0.7-yb-1-1681176489-6b9d30d8-almalinux9-x86_64",
+            "timestamp": "1681176489",
+            "version": "15.0.7",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 15,
+            "minor_version": 0,
             "patch_version": 2,
             "sha1_prefix": "64d87194",
             "short_os_name_and_version": "centos7",
             "tag": "v15.0.2-yb-1-1665186035-64d87194-centos7-aarch64",
             "timestamp": "1665186035",
             "version": "15.0.2",
             "version_suffix": "yb-1",
@@ -2027,14 +2055,28 @@
             "tag": "v16.0.1-yb-1-1680849004-58dbb949-almalinux9-x86_64",
             "timestamp": "1680849004",
             "version": "16.0.1",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 1,
+            "sha1_prefix": "58dbb949",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v16.0.1-yb-1-1681181148-58dbb949-almalinux9-x86_64",
+            "timestamp": "1681181148",
+            "version": "16.0.1",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "centos7",
@@ -2097,14 +2139,28 @@
             "tag": "v16.0.0-yb-1-1679991347-7ea85397-macos-arm64",
             "timestamp": "1679991347",
             "version": "16.0.0",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 16,
+            "minor_version": 0,
+            "patch_version": 1,
+            "sha1_prefix": "58dbb949",
+            "short_os_name_and_version": "macos",
+            "tag": "v16.0.1-yb-1-1681256292-58dbb949-macos-x86_64",
+            "timestamp": "1681256292",
+            "version": "16.0.1",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 16,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "7ea85397",
             "short_os_name_and_version": "ubuntu20.04",
```

### Comparing `llvm-installer-1.2.8/src/llvm_installer.egg-info/PKG-INFO` & `llvm-installer-1.2.9/src/llvm_installer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: llvm-installer
-Version: 1.2.8
+Version: 1.2.9
 Summary: Allows installing pre-built LLVM packages for various operating systems
 Home-page: https://github.com/yugabyte/llvm-installer
 Author: Mikhail Bautin
 Author-email: mbautin@users.noreply.github.com
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # llvm-installer
 
 https://pypi.org/project/llvm-installer/
@@ -31,7 +33,9 @@
 ```
 
 ## Command-line usage
 
 ```bash
 python3 -m llvm_installer
 ```
+
+
```

