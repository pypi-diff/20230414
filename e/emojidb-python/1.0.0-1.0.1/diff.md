# Comparing `tmp/emojidb-python-1.0.0.tar.gz` & `tmp/emojidb-python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emojidb-python-1.0.0.tar", last modified: Thu Apr 13 23:41:41 2023, max compression
+gzip compressed data, was "emojidb-python-1.0.1.tar", last modified: Fri Apr 14 00:00:49 2023, max compression
```

## Comparing `emojidb-python-1.0.0.tar` & `emojidb-python-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:41:41.913671 emojidb-python-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-13 23:41:30.000000 emojidb-python-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 23:41:30.000000 emojidb-python-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 23:41:41.913671 emojidb-python-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:41:41.909671 emojidb-python-1.0.0/emojidb/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-13 23:41:30.000000 emojidb-python-1.0.0/emojidb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-13 23:41:30.000000 emojidb-python-1.0.0/emojidb/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:41:41.909671 emojidb-python-1.0.0/emojidb/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:41:30.000000 emojidb-python-1.0.0/emojidb/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 23:41:30.000000 emojidb-python-1.0.0/emojidb/test/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:41:41.913671 emojidb-python-1.0.0/emojidb_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-13 23:41:41.000000 emojidb-python-1.0.0/emojidb_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-13 23:41:41.000000 emojidb-python-1.0.0/emojidb_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:41:41.000000 emojidb-python-1.0.0/emojidb_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:41:41.000000 emojidb-python-1.0.0/emojidb_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 23:41:41.000000 emojidb-python-1.0.0/emojidb_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 23:41:41.000000 emojidb-python-1.0.0/emojidb_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 23:41:41.913671 emojidb-python-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-13 23:41:30.000000 emojidb-python-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:00:49.211893 emojidb-python-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-14 00:00:38.000000 emojidb-python-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 00:00:38.000000 emojidb-python-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-14 00:00:49.211893 emojidb-python-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:00:49.211893 emojidb-python-1.0.1/emojidb/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 00:00:38.000000 emojidb-python-1.0.1/emojidb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-14 00:00:38.000000 emojidb-python-1.0.1/emojidb/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:00:49.211893 emojidb-python-1.0.1/emojidb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:00:38.000000 emojidb-python-1.0.1/emojidb/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-14 00:00:38.000000 emojidb-python-1.0.1/emojidb/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:00:49.211893 emojidb-python-1.0.1/emojidb_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-14 00:00:49.000000 emojidb-python-1.0.1/emojidb_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-14 00:00:49.000000 emojidb-python-1.0.1/emojidb_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:00:49.000000 emojidb-python-1.0.1/emojidb_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:00:49.000000 emojidb-python-1.0.1/emojidb_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 00:00:49.000000 emojidb-python-1.0.1/emojidb_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 00:00:49.000000 emojidb-python-1.0.1/emojidb_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:00:49.211893 emojidb-python-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-14 00:00:38.000000 emojidb-python-1.0.1/setup.py
```

### Comparing `emojidb-python-1.0.0/LICENSE` & `emojidb-python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emojidb-python-1.0.0/PKG-INFO` & `emojidb-python-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emojidb-python
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple python wrapper for emojidb.com
 Home-page: https://github.com/yedhrab/emojidb-python
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/emojidb-python/
 Project-URL: Changelog, https://github.com/yedhrab/emojidb-python/releases
```

### Comparing `emojidb-python-1.0.0/emojidb/client.py` & `emojidb-python-1.0.1/emojidb/client.py`

 * *Files identical despite different names*

### Comparing `emojidb-python-1.0.0/emojidb_python.egg-info/PKG-INFO` & `emojidb-python-1.0.1/emojidb_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emojidb-python
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simple python wrapper for emojidb.com
 Home-page: https://github.com/yedhrab/emojidb-python
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/emojidb-python/
 Project-URL: Changelog, https://github.com/yedhrab/emojidb-python/releases
```

### Comparing `emojidb-python-1.0.0/setup.py` & `emojidb-python-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 """
 
 from glob import glob
 from os.path import basename, splitext
 from setuptools import find_packages, setup
 from pathlib import Path
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = "Simple python wrapper for emojidb.com"
 README_PATH = "docs/README.md"
 USERNAME = "yedhrab"
 REPOSITORY = "emojidb-python"
 KEYWORDS = [
     "emoji",
     "emojidb",
     "emojidb.com",
     "emojidb-client",
     "emojidb-client-python",
 ]
 INSTALL_REQUIRES = [
-    "aiohttp==3.8.1",
-    "beautifulsoup4==4.11.1",
+    "aiohttp==3.8.4",
+    "beautifulsoup4==4.12.2",
 ]
 EXSTRAS_REQUIRE = {
     "dev": [
         "black==23.3.0",
         "autoflake==2.0.2",
         "pytest==7.3.0",
         "pytest-asyncio==0.21.0",
```

