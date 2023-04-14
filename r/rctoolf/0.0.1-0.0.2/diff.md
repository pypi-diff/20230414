# Comparing `tmp/rctoolf-0.0.1.tar.gz` & `tmp/rctoolf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rctoolf-0.0.1.tar", last modified: Fri Apr 14 08:26:32 2023, max compression
+gzip compressed data, was "rctoolf-0.0.2.tar", last modified: Fri Apr 14 09:16:29 2023, max compression
```

## Comparing `rctoolf-0.0.1.tar` & `rctoolf-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 08:26:32.486847 rctoolf-0.0.1/
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1068 2023-04-14 08:22:53.000000 rctoolf-0.0.1/LICENSE
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 01:10:38.000000 rctoolf-0.0.1/MANIFEST.in
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1663 2023-04-14 08:26:32.486559 rctoolf-0.0.1/PKG-INFO
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 01:10:55.000000 rctoolf-0.0.1/README.md
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      598 2023-04-14 08:18:14.000000 rctoolf-0.0.1/pyproject.toml
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       38 2023-04-14 08:26:32.486948 rctoolf-0.0.1/setup.cfg
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 08:26:32.481444 rctoolf-0.0.1/src/
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 08:26:32.484208 rctoolf-0.0.1/src/rctoolf/
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       22 2023-04-14 01:14:19.000000 rctoolf-0.0.1/src/rctoolf/__init__.py
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1336 2023-04-14 00:35:51.000000 rctoolf-0.0.1/src/rctoolf/webhook.py
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 08:26:32.486214 rctoolf-0.0.1/src/rctoolf.egg-info/
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1663 2023-04-14 08:26:32.000000 rctoolf-0.0.1/src/rctoolf.egg-info/PKG-INFO
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      265 2023-04-14 08:26:32.000000 rctoolf-0.0.1/src/rctoolf.egg-info/SOURCES.txt
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        1 2023-04-14 08:26:32.000000 rctoolf-0.0.1/src/rctoolf.egg-info/dependency_links.txt
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       12 2023-04-14 08:26:32.000000 rctoolf-0.0.1/src/rctoolf.egg-info/requires.txt
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        8 2023-04-14 08:26:32.000000 rctoolf-0.0.1/src/rctoolf.egg-info/top_level.txt
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 09:16:29.068453 rctoolf-0.0.2/
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1068 2023-04-14 08:22:53.000000 rctoolf-0.0.2/LICENSE
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 01:10:38.000000 rctoolf-0.0.2/MANIFEST.in
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1674 2023-04-14 09:16:29.068210 rctoolf-0.0.2/PKG-INFO
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        9 2023-04-14 09:14:57.000000 rctoolf-0.0.2/README.md
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      584 2023-04-14 09:16:12.000000 rctoolf-0.0.2/pyproject.toml
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       38 2023-04-14 09:16:29.068526 rctoolf-0.0.2/setup.cfg
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 09:16:29.064024 rctoolf-0.0.2/src/
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 09:16:29.066036 rctoolf-0.0.2/src/rctoolf/
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       22 2023-04-14 01:14:19.000000 rctoolf-0.0.2/src/rctoolf/__init__.py
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1336 2023-04-14 00:35:51.000000 rctoolf-0.0.2/src/rctoolf/webhook.py
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 09:16:29.067821 rctoolf-0.0.2/src/rctoolf.egg-info/
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1674 2023-04-14 09:16:29.000000 rctoolf-0.0.2/src/rctoolf.egg-info/PKG-INFO
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      265 2023-04-14 09:16:29.000000 rctoolf-0.0.2/src/rctoolf.egg-info/SOURCES.txt
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        1 2023-04-14 09:16:29.000000 rctoolf-0.0.2/src/rctoolf.egg-info/dependency_links.txt
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        5 2023-04-14 09:16:29.000000 rctoolf-0.0.2/src/rctoolf.egg-info/requires.txt
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        8 2023-04-14 09:16:29.000000 rctoolf-0.0.2/src/rctoolf.egg-info/top_level.txt
```

### Comparing `rctoolf-0.0.1/LICENSE` & `rctoolf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rctoolf-0.0.1/PKG-INFO` & `rctoolf-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rctoolf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tools for RC
 Author-email: Glorin Li <ligr1991@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,7 +28,9 @@
 Keywords: rc,webhook
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# RC tool
```

### Comparing `rctoolf-0.0.1/pyproject.toml` & `rctoolf-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rctoolf"
-version = "0.0.1"
+version = "0.0.2"
 description = "Tools for RC"
 readme = "README.md"
 authors = [{ name = "Glorin Li", email = "ligr1991@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["rc", "webhook"]
 dependencies = [
-    "urllib",
     "json"
 ]
 requires-python = ">=3.0"
 
 [project.urls]
 Homepage = "https://github.com/glorinli/rctoolf"
```

### Comparing `rctoolf-0.0.1/src/rctoolf/webhook.py` & `rctoolf-0.0.2/src/rctoolf/webhook.py`

 * *Files identical despite different names*

### Comparing `rctoolf-0.0.1/src/rctoolf.egg-info/PKG-INFO` & `rctoolf-0.0.2/src/rctoolf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rctoolf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tools for RC
 Author-email: Glorin Li <ligr1991@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,7 +28,9 @@
 Keywords: rc,webhook
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# RC tool
```

