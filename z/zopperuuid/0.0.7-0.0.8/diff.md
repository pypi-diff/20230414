# Comparing `tmp/zopperuuid-0.0.7.tar.gz` & `tmp/zopperuuid-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zopperuuid-0.0.7.tar", last modified: Fri Apr 14 09:12:00 2023, max compression
+gzip compressed data, was "zopperuuid-0.0.8.tar", last modified: Fri Apr 14 09:15:04 2023, max compression
```

## Comparing `zopperuuid-0.0.7.tar` & `zopperuuid-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sauravsharma   (501) staff       (20)        0 2023-04-14 09:12:00.281117 zopperuuid-0.0.7/
--rw-r--r--   0 sauravsharma   (501) staff       (20)        0 2023-04-13 07:44:43.000000 zopperuuid-0.0.7/LICENSE
--rw-r--r--   0 sauravsharma   (501) staff       (20)      784 2023-04-14 09:12:00.280829 zopperuuid-0.0.7/PKG-INFO
--rw-r--r--   0 sauravsharma   (501) staff       (20)      370 2023-04-14 09:10:49.000000 zopperuuid-0.0.7/README.md
--rw-r--r--   0 sauravsharma   (501) staff       (20)       38 2023-04-14 09:12:00.281195 zopperuuid-0.0.7/setup.cfg
--rw-r--r--   0 sauravsharma   (501) staff       (20)      775 2023-04-14 09:11:49.000000 zopperuuid-0.0.7/setup.py
-drwxr-xr-x   0 sauravsharma   (501) staff       (20)        0 2023-04-14 09:12:00.279392 zopperuuid-0.0.7/zopperuuid/
--rw-r--r--   0 sauravsharma   (501) staff       (20)        0 2023-04-13 07:50:31.000000 zopperuuid-0.0.7/zopperuuid/__init__.py
--rw-r--r--   0 sauravsharma   (501) staff       (20)       73 2023-04-13 08:20:03.000000 zopperuuid-0.0.7/zopperuuid/uuid.py
-drwxr-xr-x   0 sauravsharma   (501) staff       (20)        0 2023-04-14 09:12:00.280555 zopperuuid-0.0.7/zopperuuid.egg-info/
--rw-r--r--   0 sauravsharma   (501) staff       (20)      784 2023-04-14 09:12:00.000000 zopperuuid-0.0.7/zopperuuid.egg-info/PKG-INFO
--rw-r--r--   0 sauravsharma   (501) staff       (20)      204 2023-04-14 09:12:00.000000 zopperuuid-0.0.7/zopperuuid.egg-info/SOURCES.txt
--rw-r--r--   0 sauravsharma   (501) staff       (20)        1 2023-04-14 09:12:00.000000 zopperuuid-0.0.7/zopperuuid.egg-info/dependency_links.txt
--rw-r--r--   0 sauravsharma   (501) staff       (20)       11 2023-04-14 09:12:00.000000 zopperuuid-0.0.7/zopperuuid.egg-info/top_level.txt
+drwxr-xr-x   0 sauravsharma   (501) staff       (20)        0 2023-04-14 09:15:04.575488 zopperuuid-0.0.8/
+-rw-r--r--   0 sauravsharma   (501) staff       (20)        0 2023-04-13 07:44:43.000000 zopperuuid-0.0.8/LICENSE
+-rw-r--r--   0 sauravsharma   (501) staff       (20)      785 2023-04-14 09:15:04.575203 zopperuuid-0.0.8/PKG-INFO
+-rw-r--r--   0 sauravsharma   (501) staff       (20)      371 2023-04-14 09:13:04.000000 zopperuuid-0.0.8/README.md
+-rw-r--r--   0 sauravsharma   (501) staff       (20)       38 2023-04-14 09:15:04.575563 zopperuuid-0.0.8/setup.cfg
+-rw-r--r--   0 sauravsharma   (501) staff       (20)      775 2023-04-14 09:14:56.000000 zopperuuid-0.0.8/setup.py
+drwxr-xr-x   0 sauravsharma   (501) staff       (20)        0 2023-04-14 09:15:04.573523 zopperuuid-0.0.8/zopperuuid/
+-rw-r--r--   0 sauravsharma   (501) staff       (20)        0 2023-04-13 07:50:31.000000 zopperuuid-0.0.8/zopperuuid/__init__.py
+-rw-r--r--   0 sauravsharma   (501) staff       (20)       74 2023-04-14 09:12:59.000000 zopperuuid-0.0.8/zopperuuid/uuid.py
+drwxr-xr-x   0 sauravsharma   (501) staff       (20)        0 2023-04-14 09:15:04.574909 zopperuuid-0.0.8/zopperuuid.egg-info/
+-rw-r--r--   0 sauravsharma   (501) staff       (20)      785 2023-04-14 09:15:04.000000 zopperuuid-0.0.8/zopperuuid.egg-info/PKG-INFO
+-rw-r--r--   0 sauravsharma   (501) staff       (20)      204 2023-04-14 09:15:04.000000 zopperuuid-0.0.8/zopperuuid.egg-info/SOURCES.txt
+-rw-r--r--   0 sauravsharma   (501) staff       (20)        1 2023-04-14 09:15:04.000000 zopperuuid-0.0.8/zopperuuid.egg-info/dependency_links.txt
+-rw-r--r--   0 sauravsharma   (501) staff       (20)       11 2023-04-14 09:15:04.000000 zopperuuid-0.0.8/zopperuuid.egg-info/top_level.txt
```

### Comparing `zopperuuid-0.0.7/PKG-INFO` & `zopperuuid-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zopperuuid
-Version: 0.0.7
+Version: 0.0.8
 Summary: This Package will help in generating the UUID
 Home-page: https://www.zopper.com
 Author: Saurav Sharma
 Author-email: saurav.sharma@zopper.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,9 +31,9 @@
 ```
 
 ## Usage
 ```
 In [1]: from zopperuuid import uuid
 In [2]: uuid.create_uuid()
 
-Out[2]: 'zopperd2c3a494-dc37-4c0f-aa87-31a6ea2dde23'
+Out[2]: 'zopper-d2c3a494-dc37-4c0f-aa87-31a6ea2dde23'
 ```
```

### Comparing `zopperuuid-0.0.7/setup.py` & `zopperuuid-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zopperuuid", # Name of your pacakage
-    version="0.0.7", # Version of your pacakage
+    version="0.0.8", # Version of your pacakage
     author="Saurav Sharma",
     author_email="saurav.sharma@zopper.com",
     description="This Package will help in generating the UUID",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.zopper.com",
     packages=setuptools.find_packages(),
```

### Comparing `zopperuuid-0.0.7/zopperuuid.egg-info/PKG-INFO` & `zopperuuid-0.0.8/zopperuuid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zopperuuid
-Version: 0.0.7
+Version: 0.0.8
 Summary: This Package will help in generating the UUID
 Home-page: https://www.zopper.com
 Author: Saurav Sharma
 Author-email: saurav.sharma@zopper.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,9 +31,9 @@
 ```
 
 ## Usage
 ```
 In [1]: from zopperuuid import uuid
 In [2]: uuid.create_uuid()
 
-Out[2]: 'zopperd2c3a494-dc37-4c0f-aa87-31a6ea2dde23'
+Out[2]: 'zopper-d2c3a494-dc37-4c0f-aa87-31a6ea2dde23'
 ```
```

