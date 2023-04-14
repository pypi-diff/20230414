# Comparing `tmp/napalm_netonix-0.0.1.tar.gz` & `tmp/napalm_netonix-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm_netonix-0.0.1.tar", last modified: Tue Dec  6 18:09:34 2022, max compression
+gzip compressed data, was "napalm_netonix-0.0.2.tar", last modified: Fri Apr 14 00:21:53 2023, max compression
```

## Comparing `napalm_netonix-0.0.1.tar` & `napalm_netonix-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 salathe   (1000) salathe   (1000)        0 2022-12-06 18:09:34.504035 napalm_netonix-0.0.1/
--rw-rw-r--   0 salathe   (1000) salathe   (1000)     1211 2022-12-06 10:30:01.000000 napalm_netonix-0.0.1/LICENSE
--rw-rw-r--   0 salathe   (1000) salathe   (1000)     2213 2022-12-06 18:09:34.504035 napalm_netonix-0.0.1/PKG-INFO
--rw-rw-r--   0 salathe   (1000) salathe   (1000)      374 2022-12-06 18:02:01.000000 napalm_netonix-0.0.1/README.md
-drwxrwxr-x   0 salathe   (1000) salathe   (1000)        0 2022-12-06 18:09:34.503035 napalm_netonix-0.0.1/napalm_netonix/
--rw-r--r--   0 salathe   (1000) salathe   (1000)       64 2022-12-06 10:31:53.000000 napalm_netonix-0.0.1/napalm_netonix/__init__.py
--rw-r--r--   0 salathe   (1000) salathe   (1000)    14089 2022-12-06 10:42:35.000000 napalm_netonix-0.0.1/napalm_netonix/netonix.py
-drwxrwxr-x   0 salathe   (1000) salathe   (1000)        0 2022-12-06 18:09:34.504035 napalm_netonix-0.0.1/napalm_netonix.egg-info/
--rw-rw-r--   0 salathe   (1000) salathe   (1000)     2213 2022-12-06 18:09:34.000000 napalm_netonix-0.0.1/napalm_netonix.egg-info/PKG-INFO
--rw-rw-r--   0 salathe   (1000) salathe   (1000)      274 2022-12-06 18:09:34.000000 napalm_netonix-0.0.1/napalm_netonix.egg-info/SOURCES.txt
--rw-rw-r--   0 salathe   (1000) salathe   (1000)        1 2022-12-06 18:09:34.000000 napalm_netonix-0.0.1/napalm_netonix.egg-info/dependency_links.txt
--rw-rw-r--   0 salathe   (1000) salathe   (1000)       35 2022-12-06 18:09:34.000000 napalm_netonix-0.0.1/napalm_netonix.egg-info/requires.txt
--rw-rw-r--   0 salathe   (1000) salathe   (1000)       24 2022-12-06 18:09:34.000000 napalm_netonix-0.0.1/napalm_netonix.egg-info/top_level.txt
--rw-r--r--   0 salathe   (1000) salathe   (1000)      665 2022-12-06 18:09:23.000000 napalm_netonix-0.0.1/pyproject.toml
--rw-rw-r--   0 salathe   (1000) salathe   (1000)       38 2022-12-06 18:09:34.504035 napalm_netonix-0.0.1/setup.cfg
+drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 00:21:53.372792 napalm_netonix-0.0.2/
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)     1211 2022-12-06 10:30:01.000000 napalm_netonix-0.0.2/LICENSE
+-rw-r--r--   0 salathe   (1000) salathe   (1000)     2213 2023-04-14 00:21:53.372792 napalm_netonix-0.0.2/PKG-INFO
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)      374 2022-12-06 18:02:01.000000 napalm_netonix-0.0.2/README.md
+drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 00:21:53.370792 napalm_netonix-0.0.2/napalm_netonix/
+-rw-r--r--   0 salathe   (1000) salathe   (1000)       64 2022-12-06 10:31:53.000000 napalm_netonix-0.0.2/napalm_netonix/__init__.py
+-rw-r--r--   0 salathe   (1000) salathe   (1000)    14185 2023-04-14 00:18:41.000000 napalm_netonix-0.0.2/napalm_netonix/netonix.py
+drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 00:21:53.371792 napalm_netonix-0.0.2/napalm_netonix.egg-info/
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)     2213 2023-04-14 00:21:53.000000 napalm_netonix-0.0.2/napalm_netonix.egg-info/PKG-INFO
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)      274 2023-04-14 00:21:53.000000 napalm_netonix-0.0.2/napalm_netonix.egg-info/SOURCES.txt
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)        1 2023-04-14 00:21:53.000000 napalm_netonix-0.0.2/napalm_netonix.egg-info/dependency_links.txt
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)       35 2023-04-14 00:21:53.000000 napalm_netonix-0.0.2/napalm_netonix.egg-info/requires.txt
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)       24 2023-04-14 00:21:53.000000 napalm_netonix-0.0.2/napalm_netonix.egg-info/top_level.txt
+-rw-r--r--   0 salathe   (1000) salathe   (1000)      665 2023-04-14 00:19:36.000000 napalm_netonix-0.0.2/pyproject.toml
+-rw-r--r--   0 salathe   (1000) salathe   (1000)       38 2023-04-14 00:21:53.372792 napalm_netonix-0.0.2/setup.cfg
```

### Comparing `napalm_netonix-0.0.1/LICENSE` & `napalm_netonix-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm_netonix-0.0.1/PKG-INFO` & `napalm_netonix-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm_netonix
-Version: 0.0.1
+Version: 0.0.2
 Summary: NAPALM module for Netonix WISP switches
 Author-email: shrank <info@murxs.ch>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `napalm_netonix-0.0.1/napalm_netonix/netonix.py` & `napalm_netonix-0.0.2/napalm_netonix/netonix.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 from napalm.base import models
 
 
 class NetonixDriver(NetworkDriver):
 
     _speed = {
         "1G": 1000.0,
+        "100M-F": 100.0,
+        "100M-H": 100.0,
         "1M-F": 1.0,
         "1M-H": 1.0,
+        "10M-F": 10.0,
+        "10M-H": 10.0,
         "Down": 0.0
     }
 
     def __init__(
         self,
         hostname: str,
         username: str,
```

### Comparing `napalm_netonix-0.0.1/napalm_netonix.egg-info/PKG-INFO` & `napalm_netonix-0.0.2/napalm_netonix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-netonix
-Version: 0.0.1
+Version: 0.0.2
 Summary: NAPALM module for Netonix WISP switches
 Author-email: shrank <info@murxs.ch>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `napalm_netonix-0.0.1/pyproject.toml` & `napalm_netonix-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "napalm_netonix"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="shrank", email="info@murxs.ch" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 description = "NAPALM module for Netonix WISP switches"
 requires-python = ">=3.0"
```

