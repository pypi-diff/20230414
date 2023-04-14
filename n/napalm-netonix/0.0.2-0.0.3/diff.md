# Comparing `tmp/napalm_netonix-0.0.2.tar.gz` & `tmp/napalm_netonix-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm_netonix-0.0.2.tar", last modified: Fri Apr 14 00:21:53 2023, max compression
+gzip compressed data, was "napalm_netonix-0.0.3.tar", last modified: Fri Apr 14 02:40:03 2023, max compression
```

## Comparing `napalm_netonix-0.0.2.tar` & `napalm_netonix-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 00:21:53.372792 napalm_netonix-0.0.2/
--rw-rw-r--   0 salathe   (1000) salathe   (1000)     1211 2022-12-06 10:30:01.000000 napalm_netonix-0.0.2/LICENSE
--rw-r--r--   0 salathe   (1000) salathe   (1000)     2213 2023-04-14 00:21:53.372792 napalm_netonix-0.0.2/PKG-INFO
--rw-rw-r--   0 salathe   (1000) salathe   (1000)      374 2022-12-06 18:02:01.000000 napalm_netonix-0.0.2/README.md
-drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 00:21:53.370792 napalm_netonix-0.0.2/napalm_netonix/
--rw-r--r--   0 salathe   (1000) salathe   (1000)       64 2022-12-06 10:31:53.000000 napalm_netonix-0.0.2/napalm_netonix/__init__.py
--rw-r--r--   0 salathe   (1000) salathe   (1000)    14185 2023-04-14 00:18:41.000000 napalm_netonix-0.0.2/napalm_netonix/netonix.py
-drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 00:21:53.371792 napalm_netonix-0.0.2/napalm_netonix.egg-info/
--rw-rw-r--   0 salathe   (1000) salathe   (1000)     2213 2023-04-14 00:21:53.000000 napalm_netonix-0.0.2/napalm_netonix.egg-info/PKG-INFO
--rw-rw-r--   0 salathe   (1000) salathe   (1000)      274 2023-04-14 00:21:53.000000 napalm_netonix-0.0.2/napalm_netonix.egg-info/SOURCES.txt
--rw-rw-r--   0 salathe   (1000) salathe   (1000)        1 2023-04-14 00:21:53.000000 napalm_netonix-0.0.2/napalm_netonix.egg-info/dependency_links.txt
--rw-rw-r--   0 salathe   (1000) salathe   (1000)       35 2023-04-14 00:21:53.000000 napalm_netonix-0.0.2/napalm_netonix.egg-info/requires.txt
--rw-rw-r--   0 salathe   (1000) salathe   (1000)       24 2023-04-14 00:21:53.000000 napalm_netonix-0.0.2/napalm_netonix.egg-info/top_level.txt
--rw-r--r--   0 salathe   (1000) salathe   (1000)      665 2023-04-14 00:19:36.000000 napalm_netonix-0.0.2/pyproject.toml
--rw-r--r--   0 salathe   (1000) salathe   (1000)       38 2023-04-14 00:21:53.372792 napalm_netonix-0.0.2/setup.cfg
+drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 02:40:03.796917 napalm_netonix-0.0.3/
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)     1211 2022-12-06 10:30:01.000000 napalm_netonix-0.0.3/LICENSE
+-rw-r--r--   0 salathe   (1000) salathe   (1000)     2213 2023-04-14 02:40:03.795917 napalm_netonix-0.0.3/PKG-INFO
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)      374 2022-12-06 18:02:01.000000 napalm_netonix-0.0.3/README.md
+drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 02:40:03.792917 napalm_netonix-0.0.3/napalm_netonix/
+-rw-r--r--   0 salathe   (1000) salathe   (1000)       64 2022-12-06 10:31:53.000000 napalm_netonix-0.0.3/napalm_netonix/__init__.py
+-rw-r--r--   0 salathe   (1000) salathe   (1000)    14284 2023-04-14 02:39:09.000000 napalm_netonix-0.0.3/napalm_netonix/netonix.py
+drwxr-xr-x   0 salathe   (1000) salathe   (1000)        0 2023-04-14 02:40:03.795917 napalm_netonix-0.0.3/napalm_netonix.egg-info/
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)     2213 2023-04-14 02:40:03.000000 napalm_netonix-0.0.3/napalm_netonix.egg-info/PKG-INFO
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)      274 2023-04-14 02:40:03.000000 napalm_netonix-0.0.3/napalm_netonix.egg-info/SOURCES.txt
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)        1 2023-04-14 02:40:03.000000 napalm_netonix-0.0.3/napalm_netonix.egg-info/dependency_links.txt
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)       35 2023-04-14 02:40:03.000000 napalm_netonix-0.0.3/napalm_netonix.egg-info/requires.txt
+-rw-rw-r--   0 salathe   (1000) salathe   (1000)       24 2023-04-14 02:40:03.000000 napalm_netonix-0.0.3/napalm_netonix.egg-info/top_level.txt
+-rw-r--r--   0 salathe   (1000) salathe   (1000)      665 2023-04-14 02:39:27.000000 napalm_netonix-0.0.3/pyproject.toml
+-rw-r--r--   0 salathe   (1000) salathe   (1000)       38 2023-04-14 02:40:03.796917 napalm_netonix-0.0.3/setup.cfg
```

### Comparing `napalm_netonix-0.0.2/LICENSE` & `napalm_netonix-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm_netonix-0.0.2/PKG-INFO` & `napalm_netonix-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm_netonix
-Version: 0.0.2
+Version: 0.0.3
 Summary: NAPALM module for Netonix WISP switches
 Author-email: shrank <info@murxs.ch>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `napalm_netonix-0.0.2/napalm_netonix/netonix.py` & `napalm_netonix-0.0.3/napalm_netonix/netonix.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,17 @@
                     'static'    : False,
                     'active'    : True,
                     'moves'     : None,
                     'last_move' : None
                 }
             ]
         """
-        self.n.getMAC()
+        self.n.getMAC() 
+        if(len(self.n.mac) == 0): # first run returns an empty result
+            self.n.getMAC()
         res = []
         for a in self.n.mac:
             res.append(
                 {
                     'mac'       : a["MAC"].replace("-", ":"),
                     'interface' : self._port_fmt(a["Port"]),
                     'vlan'      : a["VLAN_ID"],
```

### Comparing `napalm_netonix-0.0.2/napalm_netonix.egg-info/PKG-INFO` & `napalm_netonix-0.0.3/napalm_netonix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-netonix
-Version: 0.0.2
+Version: 0.0.3
 Summary: NAPALM module for Netonix WISP switches
 Author-email: shrank <info@murxs.ch>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `napalm_netonix-0.0.2/pyproject.toml` & `napalm_netonix-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "napalm_netonix"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="shrank", email="info@murxs.ch" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 description = "NAPALM module for Netonix WISP switches"
 requires-python = ">=3.0"
```

