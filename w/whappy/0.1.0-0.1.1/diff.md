# Comparing `tmp/whappy-0.1.0.tar.gz` & `tmp/whappy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whappy-0.1.0.tar", last modified: Fri Apr 14 19:37:18 2023, max compression
+gzip compressed data, was "whappy-0.1.1.tar", last modified: Fri Apr 14 20:01:27 2023, max compression
```

## Comparing `whappy-0.1.0.tar` & `whappy-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxr-x   0 harshraj  (1000) harshraj  (1000)        0 2023-04-14 19:37:18.443952 whappy-0.1.0/
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      585 2023-04-14 19:37:18.443952 whappy-0.1.0/PKG-INFO
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      138 2023-04-14 10:20:51.000000 whappy-0.1.0/README.md
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)       38 2023-04-14 19:37:18.443952 whappy-0.1.0/setup.cfg
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      719 2023-04-14 19:36:58.000000 whappy-0.1.0/setup.py
-drwxrwxr-x   0 harshraj  (1000) harshraj  (1000)        0 2023-04-14 19:37:18.443952 whappy-0.1.0/whappy.egg-info/
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      585 2023-04-14 19:37:18.000000 whappy-0.1.0/whappy.egg-info/PKG-INFO
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      167 2023-04-14 19:37:18.000000 whappy-0.1.0/whappy.egg-info/SOURCES.txt
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        1 2023-04-14 19:37:18.000000 whappy-0.1.0/whappy.egg-info/dependency_links.txt
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        9 2023-04-14 19:37:18.000000 whappy-0.1.0/whappy.egg-info/requires.txt
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        1 2023-04-14 19:37:18.000000 whappy-0.1.0/whappy.egg-info/top_level.txt
+drwxrwxr-x   0 harshraj  (1000) harshraj  (1000)        0 2023-04-14 20:01:27.291551 whappy-0.1.1/
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)       35 2023-04-14 19:57:25.000000 whappy-0.1.1/MANIFEST.in
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      585 2023-04-14 20:01:27.291551 whappy-0.1.1/PKG-INFO
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      138 2023-04-14 10:20:51.000000 whappy-0.1.1/README.md
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)     1917 2023-04-14 19:17:38.000000 whappy-0.1.1/api.py
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)       66 2023-04-14 10:24:45.000000 whappy-0.1.1/constants.py
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)       38 2023-04-14 20:01:27.291551 whappy-0.1.1/setup.cfg
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      757 2023-04-14 20:00:15.000000 whappy-0.1.1/setup.py
+drwxrwxr-x   0 harshraj  (1000) harshraj  (1000)        0 2023-04-14 20:01:27.291551 whappy-0.1.1/whappy.egg-info/
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      585 2023-04-14 20:01:27.000000 whappy-0.1.1/whappy.egg-info/PKG-INFO
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      199 2023-04-14 20:01:27.000000 whappy-0.1.1/whappy.egg-info/SOURCES.txt
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        1 2023-04-14 20:01:27.000000 whappy-0.1.1/whappy.egg-info/dependency_links.txt
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        9 2023-04-14 20:01:27.000000 whappy-0.1.1/whappy.egg-info/requires.txt
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        1 2023-04-14 20:01:27.000000 whappy-0.1.1/whappy.egg-info/top_level.txt
```

### Comparing `whappy-0.1.0/PKG-INFO` & `whappy-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whappy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for WhatsApp API
 Home-page: https://github.com/saketharshraj/whappy
 Author: Harsh Raj
 Author-email: saketharshraj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `whappy-0.1.0/setup.py` & `whappy-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="whappy",
-    version="0.1.0",
+    version="0.1.1",
     author="Harsh Raj",
     author_email="saketharshraj@gmail.com",
     description="A Python wrapper for WhatsApp API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/saketharshraj/whappy",
     packages=find_packages(),
+    package_dir={"whappy": "whappy"},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "requests",
```

### Comparing `whappy-0.1.0/whappy.egg-info/PKG-INFO` & `whappy-0.1.1/whappy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whappy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for WhatsApp API
 Home-page: https://github.com/saketharshraj/whappy
 Author: Harsh Raj
 Author-email: saketharshraj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

