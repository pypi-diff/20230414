# Comparing `tmp/traffix-0.1.8a0.tar.gz` & `tmp/traffix-0.1.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traffix-0.1.8a0.tar", last modified: Thu Apr 13 19:30:08 2023, max compression
+gzip compressed data, was "traffix-0.1.9a0.tar", last modified: Thu Apr 13 19:42:35 2023, max compression
```

## Comparing `traffix-0.1.8a0.tar` & `traffix-0.1.9a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 19:30:08.455361 traffix-0.1.8a0/
--rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 traffix-0.1.8a0/LICENSE
--rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 traffix-0.1.8a0/MANIFEST.in
--rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 19:30:08.454792 traffix-0.1.8a0/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 traffix-0.1.8a0/README.md
--rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 19:30:08.455546 traffix-0.1.8a0/setup.cfg
--rwxr-xr-x   0 maman      (501) staff       (20)     1182 2023-04-13 19:25:57.000000 traffix-0.1.8a0/setup.py
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 19:30:08.450335 traffix-0.1.8a0/traffix/
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.8a0/traffix/.___init__.py
--rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.8a0/traffix/.__version.py
--rw-r--r--   0 maman      (501) staff       (20)      579 2023-04-13 17:29:48.000000 traffix-0.1.8a0/traffix/OD.py
--rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 18:53:38.000000 traffix-0.1.8a0/traffix/__init__.py
--rw-r--r--   0 maman      (501) staff       (20)       60 2023-04-13 19:25:53.000000 traffix-0.1.8a0/traffix/_version.py
--rw-r--r--   0 maman      (501) staff       (20)     5278 2023-04-13 17:31:32.000000 traffix-0.1.8a0/traffix/add.py
--rw-r--r--   0 maman      (501) staff       (20)     1343 2023-04-13 17:33:07.000000 traffix-0.1.8a0/traffix/flow.py
--rw-r--r--   0 maman      (501) staff       (20)      712 2023-04-13 17:34:01.000000 traffix-0.1.8a0/traffix/lpr.py
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 19:30:08.453871 traffix-0.1.8a0/traffix/traffix.egg-info/
--rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 19:30:08.000000 traffix-0.1.8a0/traffix/traffix.egg-info/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)      409 2023-04-13 19:30:08.000000 traffix-0.1.8a0/traffix/traffix.egg-info/SOURCES.txt
--rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 19:30:08.000000 traffix-0.1.8a0/traffix/traffix.egg-info/dependency_links.txt
--rw-r--r--   0 maman      (501) staff       (20)       39 2023-04-13 19:30:08.000000 traffix-0.1.8a0/traffix/traffix.egg-info/requires.txt
--rw-r--r--   0 maman      (501) staff       (20)       45 2023-04-13 19:30:08.000000 traffix-0.1.8a0/traffix/traffix.egg-info/top_level.txt
--rw-r--r--   0 maman      (501) staff       (20)     9927 2023-04-13 19:28:42.000000 traffix-0.1.8a0/traffix/traffix.py
--rw-r--r--   0 maman      (501) staff       (20)     2183 2023-04-13 17:35:01.000000 traffix-0.1.8a0/traffix/ue.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 19:42:35.710316 traffix-0.1.9a0/
+-rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 traffix-0.1.9a0/LICENSE
+-rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 traffix-0.1.9a0/MANIFEST.in
+-rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 19:42:35.709688 traffix-0.1.9a0/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 traffix-0.1.9a0/README.md
+-rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 19:42:35.710524 traffix-0.1.9a0/setup.cfg
+-rwxr-xr-x   0 maman      (501) staff       (20)     1180 2023-04-13 19:41:51.000000 traffix-0.1.9a0/setup.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 19:42:35.693690 traffix-0.1.9a0/traffix/
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.9a0/traffix/.___init__.py
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-04-13 16:58:26.000000 traffix-0.1.9a0/traffix/.__version.py
+-rw-r--r--   0 maman      (501) staff       (20)      579 2023-04-13 17:29:48.000000 traffix-0.1.9a0/traffix/OD.py
+-rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 18:53:38.000000 traffix-0.1.9a0/traffix/__init__.py
+-rw-r--r--   0 maman      (501) staff       (20)       60 2023-04-13 19:41:13.000000 traffix-0.1.9a0/traffix/_version.py
+-rw-r--r--   0 maman      (501) staff       (20)     5278 2023-04-13 17:31:32.000000 traffix-0.1.9a0/traffix/add.py
+-rw-r--r--   0 maman      (501) staff       (20)     1343 2023-04-13 17:33:07.000000 traffix-0.1.9a0/traffix/flow.py
+-rw-r--r--   0 maman      (501) staff       (20)      712 2023-04-13 17:34:01.000000 traffix-0.1.9a0/traffix/lpr.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 19:42:35.703656 traffix-0.1.9a0/traffix/traffix.egg-info/
+-rw-r--r--   0 maman      (501) staff       (20)     2744 2023-04-13 19:42:35.000000 traffix-0.1.9a0/traffix/traffix.egg-info/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)      409 2023-04-13 19:42:35.000000 traffix-0.1.9a0/traffix/traffix.egg-info/SOURCES.txt
+-rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 19:42:35.000000 traffix-0.1.9a0/traffix/traffix.egg-info/dependency_links.txt
+-rw-r--r--   0 maman      (501) staff       (20)       37 2023-04-13 19:42:35.000000 traffix-0.1.9a0/traffix/traffix.egg-info/requires.txt
+-rw-r--r--   0 maman      (501) staff       (20)       45 2023-04-13 19:42:35.000000 traffix-0.1.9a0/traffix/traffix.egg-info/top_level.txt
+-rw-r--r--   0 maman      (501) staff       (20)     9927 2023-04-13 19:28:42.000000 traffix-0.1.9a0/traffix/traffix.py
+-rw-r--r--   0 maman      (501) staff       (20)     2183 2023-04-13 17:35:01.000000 traffix-0.1.9a0/traffix/ue.py
```

### Comparing `traffix-0.1.8a0/LICENSE` & `traffix-0.1.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `traffix-0.1.8a0/PKG-INFO` & `traffix-0.1.9a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffix
-Version: 0.1.8a0
+Version: 0.1.9a0
 Summary: A package for macroscopic transportation assignment.
 Home-page: https://github.com/Ultios/traffix
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `traffix-0.1.8a0/README.md` & `traffix-0.1.9a0/README.md`

 * *Files identical despite different names*

### Comparing `traffix-0.1.8a0/setup.py` & `traffix-0.1.9a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from setuptools import setup
 
 
 setup(
     name="traffix", 
-    version = "0.1.8-alpha",
+    version = "0.1.9-alpha",
     description = "A package for macroscopic transportation assignment.",
     package_dir = {"":"traffix"},
     author = "Aulia Rahman",
     author_email = "rahmancs02@gmail.com",
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
     url="https://github.com/Ultios/traffix",
@@ -25,11 +25,11 @@
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: GIS",
         "Operating System :: OS Independent",
     ],
     install_requires = [
         "python >=3.6",
         "osmnx ~= 1.3.0",
-        "pandas ~= 1.2.4",
+        "pandas ~= 1.5",
     ],
     keywords = ["Traffic Assignment", "Transportation Planning", "Macroscopic Transportation Planning"],
 )
```

### Comparing `traffix-0.1.8a0/traffix/.___init__.py` & `traffix-0.1.9a0/traffix/.___init__.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.8a0/traffix/.__version.py` & `traffix-0.1.9a0/traffix/.__version.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.8a0/traffix/OD.py` & `traffix-0.1.9a0/traffix/OD.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.8a0/traffix/add.py` & `traffix-0.1.9a0/traffix/add.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.8a0/traffix/flow.py` & `traffix-0.1.9a0/traffix/flow.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.8a0/traffix/lpr.py` & `traffix-0.1.9a0/traffix/lpr.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.8a0/traffix/traffix.egg-info/PKG-INFO` & `traffix-0.1.9a0/traffix/traffix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffix
-Version: 0.1.8a0
+Version: 0.1.9a0
 Summary: A package for macroscopic transportation assignment.
 Home-page: https://github.com/Ultios/traffix
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `traffix-0.1.8a0/traffix/traffix.py` & `traffix-0.1.9a0/traffix/traffix.py`

 * *Files identical despite different names*

### Comparing `traffix-0.1.8a0/traffix/ue.py` & `traffix-0.1.9a0/traffix/ue.py`

 * *Files identical despite different names*

