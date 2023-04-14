# Comparing `tmp/pyvts-0.2.6.tar.gz` & `tmp/pyvts-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvts-0.2.6.tar", last modified: Fri Apr 14 15:51:33 2023, max compression
+gzip compressed data, was "pyvts-0.2.7.tar", last modified: Fri Apr 14 15:58:42 2023, max compression
```

## Comparing `pyvts-0.2.6.tar` & `pyvts-0.2.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:51:33.183619 pyvts-0.2.6/
--rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.2.6/LICENSE
--rw-r--r--   0 genteki    (501) staff       (20)     3503 2023-04-14 15:51:33.183493 pyvts-0.2.6/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)     2658 2023-04-14 15:36:17.000000 pyvts-0.2.6/README.md
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:51:33.181875 pyvts-0.2.6/pyvts/
--rw-r--r--   0 genteki    (501) staff       (20)      218 2023-04-14 15:51:19.000000 pyvts-0.2.6/pyvts/__init__.py
--rw-r--r--   0 genteki    (501) staff       (20)      258 2023-03-02 20:34:19.000000 pyvts-0.2.6/pyvts/config.py
--rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.2.6/pyvts/error.py
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:51:33.183098 pyvts-0.2.6/pyvts/tests/
--rw-r--r--   0 genteki    (501) staff       (20)        0 2023-02-28 10:07:07.000000 pyvts-0.2.6/pyvts/tests/__init__.py
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:51:33.183312 pyvts-0.2.6/pyvts/tests/integration/
--rw-r--r--   0 genteki    (501) staff       (20)        0 2023-03-02 07:55:23.000000 pyvts-0.2.6/pyvts/tests/integration/__init__.py
--rw-r--r--   0 genteki    (501) staff       (20)      864 2023-03-02 20:34:19.000000 pyvts-0.2.6/pyvts/tests/integration/test_integration.py
--rw-r--r--   0 genteki    (501) staff       (20)     4448 2023-03-26 06:13:29.000000 pyvts-0.2.6/pyvts/tests/test_utils.py
--rw-r--r--   0 genteki    (501) staff       (20)     4207 2023-04-10 05:03:27.000000 pyvts-0.2.6/pyvts/tests/test_vts.py
--rw-r--r--   0 genteki    (501) staff       (20)      477 2023-03-25 05:41:19.000000 pyvts-0.2.6/pyvts/tests/test_vts_request.py
--rw-r--r--   0 genteki    (501) staff       (20)     6349 2023-04-11 05:55:48.000000 pyvts-0.2.6/pyvts/vts.py
--rw-r--r--   0 genteki    (501) staff       (20)    10148 2023-04-14 15:36:17.000000 pyvts-0.2.6/pyvts/vts_request.py
-drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:51:33.182502 pyvts-0.2.6/pyvts.egg-info/
--rw-r--r--   0 genteki    (501) staff       (20)     3503 2023-04-14 15:51:33.000000 pyvts-0.2.6/pyvts.egg-info/PKG-INFO
--rw-r--r--   0 genteki    (501) staff       (20)      439 2023-04-14 15:51:33.000000 pyvts-0.2.6/pyvts.egg-info/SOURCES.txt
--rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-14 15:51:33.000000 pyvts-0.2.6/pyvts.egg-info/dependency_links.txt
--rw-r--r--   0 genteki    (501) staff       (20)       19 2023-04-14 15:51:33.000000 pyvts-0.2.6/pyvts.egg-info/requires.txt
--rw-r--r--   0 genteki    (501) staff       (20)        6 2023-04-14 15:51:33.000000 pyvts-0.2.6/pyvts.egg-info/top_level.txt
--rw-r--r--   0 genteki    (501) staff       (20)       38 2023-04-14 15:51:33.183662 pyvts-0.2.6/setup.cfg
--rw-r--r--   0 genteki    (501) staff       (20)     1207 2023-04-14 15:51:17.000000 pyvts-0.2.6/setup.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:58:42.848146 pyvts-0.2.7/
+-rw-r--r--   0 genteki    (501) staff       (20)     1064 2023-02-09 07:28:50.000000 pyvts-0.2.7/LICENSE
+-rw-r--r--   0 genteki    (501) staff       (20)     3503 2023-04-14 15:58:42.847936 pyvts-0.2.7/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)     2658 2023-04-14 15:36:17.000000 pyvts-0.2.7/README.md
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:58:42.846462 pyvts-0.2.7/pyvts/
+-rw-r--r--   0 genteki    (501) staff       (20)      216 2023-04-14 15:58:36.000000 pyvts-0.2.7/pyvts/__init__.py
+-rw-r--r--   0 genteki    (501) staff       (20)      258 2023-03-02 20:34:19.000000 pyvts-0.2.7/pyvts/config.py
+-rw-r--r--   0 genteki    (501) staff       (20)      355 2023-03-26 06:13:29.000000 pyvts-0.2.7/pyvts/error.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:58:42.847516 pyvts-0.2.7/pyvts/tests/
+-rw-r--r--   0 genteki    (501) staff       (20)        0 2023-02-28 10:07:07.000000 pyvts-0.2.7/pyvts/tests/__init__.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:58:42.847723 pyvts-0.2.7/pyvts/tests/integration/
+-rw-r--r--   0 genteki    (501) staff       (20)        0 2023-03-02 07:55:23.000000 pyvts-0.2.7/pyvts/tests/integration/__init__.py
+-rw-r--r--   0 genteki    (501) staff       (20)      864 2023-03-02 20:34:19.000000 pyvts-0.2.7/pyvts/tests/integration/test_integration.py
+-rw-r--r--   0 genteki    (501) staff       (20)     4448 2023-03-26 06:13:29.000000 pyvts-0.2.7/pyvts/tests/test_utils.py
+-rw-r--r--   0 genteki    (501) staff       (20)     4207 2023-04-10 05:03:27.000000 pyvts-0.2.7/pyvts/tests/test_vts.py
+-rw-r--r--   0 genteki    (501) staff       (20)      477 2023-03-25 05:41:19.000000 pyvts-0.2.7/pyvts/tests/test_vts_request.py
+-rw-r--r--   0 genteki    (501) staff       (20)     6349 2023-04-11 05:55:48.000000 pyvts-0.2.7/pyvts/vts.py
+-rw-r--r--   0 genteki    (501) staff       (20)    10148 2023-04-14 15:36:17.000000 pyvts-0.2.7/pyvts/vts_request.py
+drwxr-xr-x   0 genteki    (501) staff       (20)        0 2023-04-14 15:58:42.847026 pyvts-0.2.7/pyvts.egg-info/
+-rw-r--r--   0 genteki    (501) staff       (20)     3503 2023-04-14 15:58:42.000000 pyvts-0.2.7/pyvts.egg-info/PKG-INFO
+-rw-r--r--   0 genteki    (501) staff       (20)      439 2023-04-14 15:58:42.000000 pyvts-0.2.7/pyvts.egg-info/SOURCES.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        1 2023-04-14 15:58:42.000000 pyvts-0.2.7/pyvts.egg-info/dependency_links.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       20 2023-04-14 15:58:42.000000 pyvts-0.2.7/pyvts.egg-info/requires.txt
+-rw-r--r--   0 genteki    (501) staff       (20)        6 2023-04-14 15:58:42.000000 pyvts-0.2.7/pyvts.egg-info/top_level.txt
+-rw-r--r--   0 genteki    (501) staff       (20)       38 2023-04-14 15:58:42.848229 pyvts-0.2.7/setup.cfg
+-rw-r--r--   0 genteki    (501) staff       (20)     1208 2023-04-14 15:58:25.000000 pyvts-0.2.7/setup.py
```

### Comparing `pyvts-0.2.6/LICENSE` & `pyvts-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.6/PKG-INFO` & `pyvts-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.2.6
+Version: 0.2.7
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyvts-0.2.6/README.md` & `pyvts-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.6/pyvts/tests/integration/test_integration.py` & `pyvts-0.2.7/pyvts/tests/integration/test_integration.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.6/pyvts/tests/test_utils.py` & `pyvts-0.2.7/pyvts/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.6/pyvts/tests/test_vts.py` & `pyvts-0.2.7/pyvts/tests/test_vts.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.6/pyvts/vts.py` & `pyvts-0.2.7/pyvts/vts.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.6/pyvts/vts_request.py` & `pyvts-0.2.7/pyvts/vts_request.py`

 * *Files identical despite different names*

### Comparing `pyvts-0.2.6/pyvts.egg-info/PKG-INFO` & `pyvts-0.2.7/pyvts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvts
-Version: 0.2.6
+Version: 0.2.7
 Summary: A python library for interacting with the VTube Studio API
 Home-page: https://github.com/Genteki/pyvts
 Author: Genteki Zhang
 Author-email: zhangkaiyuan.null@gmail.com
 License: MIT
 Keywords: vtubestudio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyvts-0.2.6/setup.py` & `pyvts-0.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """A python library for interacting with the VTube Studio API"""
 
 from setuptools import setup, find_packages
 
 DESCRIPTION = "A python library for interacting with the VTube Studio API"
-VERSION = "v0.2.6"
+VERSION = "v0.2.7"
 
 setup(
     name="pyvts",
     version=VERSION,
     description=DESCRIPTION,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
@@ -26,9 +26,9 @@
         "Programming Language :: Python :: 3.11"
     ],
     author="Genteki Zhang",
     author_email="zhangkaiyuan.null@gmail.com",
     url="https://github.com/Genteki/pyvts",
     license="MIT",
     packages=find_packages(exclude=["tests.*", "tests"]),
-    install_requires=["websockets", "aiofile"],
+    install_requires=["websockets", "aiofiles"],
 )
```

