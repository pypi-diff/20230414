# Comparing `tmp/pyvts-0.2.5.tar.gz` & `tmp/pyvts-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvts-0.2.5.tar", last modified: Fri Apr 14 15:48:21 2023, max compression
+gzip compressed data, was "pyvts-0.2.6.tar", last modified: Fri Apr 14 15:51:33 2023, max compression
```

## Comparing `pyvts-0.2.5.tar` & `pyvts-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:48:21.472714 pyvts-0.2.5/
--rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.2.5/LICENSE
--rw-r--r--   0 genteki    (501) staff       (20)     3503 2023-04-14 15:48:21.472612 pyvts-0.2.5/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)     2658 2023-04-14 15:36:17.000000 pyvts-0.2.5/README.md
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:48:21.471926 pyvts-0.2.5/pyvts/
--rw-r--r--   0 genteki    (501) staff       (20)      218 2023-04-14 15:47:22.000000 pyvts-0.2.5/pyvts/__init__.py
--rw-r--r--   0 genteki    (501) staff       (20)      258 2023-03-02 20:34:19.000000 pyvts-0.2.5/pyvts/config.py
--rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.2.5/pyvts/error.py
--rw-r--r--   0 genteki    (501) staff       (20)     6349 2023-04-11 05:55:48.000000 pyvts-0.2.5/pyvts/vts.py
--rw-r--r--   0 genteki    (501) staff       (20)    10148 2023-04-14 15:36:17.000000 pyvts-0.2.5/pyvts/vts_request.py
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:48:21.472449 pyvts-0.2.5/pyvts.egg-info/
--rw-r--r--   0 genteki    (501) staff       (20)     3503 2023-04-14 15:48:21.000000 pyvts-0.2.5/pyvts.egg-info/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)      253 2023-04-14 15:48:21.000000 pyvts-0.2.5/pyvts.egg-info/SOURCES.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-14 15:48:21.000000 pyvts-0.2.5/pyvts.egg-info/dependency_links.txt
--rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-14 15:48:21.000000 pyvts-0.2.5/pyvts.egg-info/requires.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-14 15:48:21.000000 pyvts-0.2.5/pyvts.egg-info/top_level.txt
--rw-r--r--   0 genteki    (501) staff       (20)       38 2023-04-14 15:48:21.472748 pyvts-0.2.5/setup.cfg
--rw-r--r--   0 genteki    (501) staff       (20)     1222 2023-04-14 15:47:24.000000 pyvts-0.2.5/setup.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:51:33.183619 pyvts-0.2.6/
+-rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.2.6/LICENSE
+-rw-r--r--   0 genteki    (501) staff       (20)     3503 2023-04-14 15:51:33.183493 pyvts-0.2.6/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)     2658 2023-04-14 15:36:17.000000 pyvts-0.2.6/README.md
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:51:33.181875 pyvts-0.2.6/pyvts/
+-rw-r--r--   0 genteki    (501) staff       (20)      218 2023-04-14 15:51:19.000000 pyvts-0.2.6/pyvts/__init__.py
+-rw-r--r--   0 genteki    (501) staff       (20)      258 2023-03-02 20:34:19.000000 pyvts-0.2.6/pyvts/config.py
+-rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.2.6/pyvts/error.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:51:33.183098 pyvts-0.2.6/pyvts/tests/
+-rw-r--r--   0 genteki    (501) staff       (20)        0 2023-02-28 10:07:07.000000 pyvts-0.2.6/pyvts/tests/__init__.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:51:33.183312 pyvts-0.2.6/pyvts/tests/integration/
+-rw-r--r--   0 genteki    (501) staff       (20)        0 2023-03-02 07:55:23.000000 pyvts-0.2.6/pyvts/tests/integration/__init__.py
+-rw-r--r--   0 genteki    (501) staff       (20)      864 2023-03-02 20:34:19.000000 pyvts-0.2.6/pyvts/tests/integration/test_integration.py
+-rw-r--r--   0 genteki    (501) staff       (20)     4448 2023-03-26 06:13:29.000000 pyvts-0.2.6/pyvts/tests/test_utils.py
+-rw-r--r--   0 genteki    (501) staff       (20)     4207 2023-04-10 05:03:27.000000 pyvts-0.2.6/pyvts/tests/test_vts.py
+-rw-r--r--   0 genteki    (501) staff       (20)      477 2023-03-25 05:41:19.000000 pyvts-0.2.6/pyvts/tests/test_vts_request.py
+-rw-r--r--   0 genteki    (501) staff       (20)     6349 2023-04-11 05:55:48.000000 pyvts-0.2.6/pyvts/vts.py
+-rw-r--r--   0 genteki    (501) staff       (20)    10148 2023-04-14 15:36:17.000000 pyvts-0.2.6/pyvts/vts_request.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:51:33.182502 pyvts-0.2.6/pyvts.egg-info/
+-rw-r--r--   0 genteki    (501) staff       (20)     3503 2023-04-14 15:51:33.000000 pyvts-0.2.6/pyvts.egg-info/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)      439 2023-04-14 15:51:33.000000 pyvts-0.2.6/pyvts.egg-info/SOURCES.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-14 15:51:33.000000 pyvts-0.2.6/pyvts.egg-info/dependency_links.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-14 15:51:33.000000 pyvts-0.2.6/pyvts.egg-info/requires.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        6 2023-04-14 15:51:33.000000 pyvts-0.2.6/pyvts.egg-info/top_level.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       38 2023-04-14 15:51:33.183662 pyvts-0.2.6/setup.cfg
+-rw-r--r--   0 genteki    (501) staff       (20)     1207 2023-04-14 15:51:17.000000 pyvts-0.2.6/setup.py
```

### Comparing `pyvts-0.2.5/LICENSE` & `pyvts-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.5/PKG-INFO` & `pyvts-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.2.5
+Version: 0.2.6
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyvts-0.2.5/README.md` & `pyvts-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.5/pyvts/vts.py` & `pyvts-0.2.6/pyvts/vts.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.5/pyvts/vts_request.py` & `pyvts-0.2.6/pyvts/vts_request.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.5/pyvts.egg-info/PKG-INFO` & `pyvts-0.2.6/pyvts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.2.5
+Version: 0.2.6
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyvts-0.2.5/setup.py` & `pyvts-0.2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A python library for interacting with the VTube Studio API"""
 
 from setuptools import setup, find_packages
 
 DESCRIPTION = "A python library for interacting with the VTube Studio API"
-VERSION = "v0.2.5"
+VERSION = "v0.2.6"
 
 setup(
     name="pyvts",
     version=VERSION,
     description=DESCRIPTION,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
@@ -25,10 +25,10 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11"
     ],
     author="Genteki Zhang",
     author_email="zhangkaiyuan.null@gmail.com",
     url="https://github.com/Genteki/pyvts",
     license="MIT",
-    packages=find_packages(where="pyvts", exclude=["tests.*", "tests"]),
+    packages=find_packages(exclude=["tests.*", "tests"]),
     install_requires=["websockets", "aiofile"],
 )
```

