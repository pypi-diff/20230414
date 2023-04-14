# Comparing `tmp/magyar-2.7.0.tar.gz` & `tmp/magyar-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.7.0.tar", last modified: Fri Apr 14 16:27:17 2023, max compression
+gzip compressed data, was "magyar-2.8.0.tar", last modified: Fri Apr 14 16:37:19 2023, max compression
```

## Comparing `magyar-2.7.0.tar` & `magyar-2.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 16:27:17.017003 magyar-2.7.0/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1535 2023-04-14 16:27:17.017003 magyar-2.7.0/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     1164 2023-04-13 19:21:03.000000 magyar-2.7.0/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 16:27:17.017003 magyar-2.7.0/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1535 2023-04-14 16:27:16.000000 magyar-2.7.0/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-14 16:27:16.000000 magyar-2.7.0/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-14 16:27:16.000000 magyar-2.7.0/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-14 16:27:16.000000 magyar-2.7.0/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)     9057 2023-04-13 19:56:03.000000 magyar-2.7.0/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-14 16:27:17.017003 magyar-2.7.0/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-14 16:26:47.000000 magyar-2.7.0/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 16:37:19.105306 magyar-2.8.0/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1535 2023-04-14 16:37:19.105306 magyar-2.8.0/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1164 2023-04-13 19:21:03.000000 magyar-2.8.0/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 16:37:19.105306 magyar-2.8.0/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1535 2023-04-14 16:37:19.000000 magyar-2.8.0/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-14 16:37:19.000000 magyar-2.8.0/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-14 16:37:19.000000 magyar-2.8.0/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-14 16:37:19.000000 magyar-2.8.0/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)     9057 2023-04-13 19:56:03.000000 magyar-2.8.0/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-14 16:37:19.105306 magyar-2.8.0/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-14 16:35:12.000000 magyar-2.8.0/setup.py
```

### Comparing `magyar-2.7.0/PKG-INFO` & `magyar-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.7.0
+Version: 2.8.0
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `magyar-2.7.0/README.md` & `magyar-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `magyar-2.7.0/magyar.egg-info/PKG-INFO` & `magyar-2.8.0/magyar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.7.0
+Version: 2.8.0
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `magyar-2.7.0/magyar.py` & `magyar-2.8.0/magyar.py`

 * *Files identical despite different names*

### Comparing `magyar-2.7.0/setup.py` & `magyar-2.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.7.0",
+    version="2.8.0",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian names...",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

