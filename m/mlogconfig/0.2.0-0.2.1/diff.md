# Comparing `tmp/mlogconfig-0.2.0.tar.gz` & `tmp/mlogconfig-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlogconfig-0.2.0.tar", last modified: Sat Apr  8 00:25:59 2023, max compression
+gzip compressed data, was "mlogconfig-0.2.1.tar", last modified: Thu Apr 13 21:42:27 2023, max compression
```

## Comparing `mlogconfig-0.2.0.tar` & `mlogconfig-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:25:59.375560 mlogconfig-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-08 00:25:46.000000 mlogconfig-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-08 00:25:46.000000 mlogconfig-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-08 00:25:59.375560 mlogconfig-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-08 00:25:46.000000 mlogconfig-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:25:59.375560 mlogconfig-0.2.0/mlogconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-08 00:25:59.000000 mlogconfig-0.2.0/mlogconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-08 00:25:59.000000 mlogconfig-0.2.0/mlogconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:25:59.000000 mlogconfig-0.2.0/mlogconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:25:59.000000 mlogconfig-0.2.0/mlogconfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 00:25:59.375560 mlogconfig-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-08 00:25:46.000000 mlogconfig-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:42:27.843931 mlogconfig-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-13 21:42:18.000000 mlogconfig-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 21:42:18.000000 mlogconfig-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-13 21:42:27.843931 mlogconfig-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-13 21:42:18.000000 mlogconfig-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:42:27.843931 mlogconfig-0.2.1/mlogconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-13 21:42:27.000000 mlogconfig-0.2.1/mlogconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-13 21:42:27.000000 mlogconfig-0.2.1/mlogconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:42:27.000000 mlogconfig-0.2.1/mlogconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:42:27.000000 mlogconfig-0.2.1/mlogconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:42:27.843931 mlogconfig-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-13 21:42:18.000000 mlogconfig-0.2.1/setup.py
```

### Comparing `mlogconfig-0.2.0/LICENSE.md` & `mlogconfig-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlogconfig-0.2.0/PKG-INFO` & `mlogconfig-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlogconfig
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple logging setup utility that configures logging with file, console, syslog, and Windows event log handlers.
 Home-page: https://github.com/talltechy/mlogconfig
 Author: Matt Wyen
 Author-email: matt@mattwyen.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -31,15 +31,15 @@
 
 - Logging to console, file, syslog, and Windows Event Log
 - Enable or disable each logging method as needed
 - Easy setup and configuration
 
 ## Requirements
 
-- Python 3.6 or higher
+- Python 3.9 or higher
 
 For Windows Event Log support, the following packages are required:
 
 - pywin32
 
 Install the required packages by running:
```

### Comparing `mlogconfig-0.2.0/README.md` & `mlogconfig-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 - Logging to console, file, syslog, and Windows Event Log
 - Enable or disable each logging method as needed
 - Easy setup and configuration
 
 ## Requirements
 
-- Python 3.6 or higher
+- Python 3.9 or higher
 
 For Windows Event Log support, the following packages are required:
 
 - pywin32
 
 Install the required packages by running:
```

### Comparing `mlogconfig-0.2.0/mlogconfig.egg-info/PKG-INFO` & `mlogconfig-0.2.1/mlogconfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlogconfig
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple logging setup utility that configures logging with file, console, syslog, and Windows event log handlers.
 Home-page: https://github.com/talltechy/mlogconfig
 Author: Matt Wyen
 Author-email: matt@mattwyen.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -31,15 +31,15 @@
 
 - Logging to console, file, syslog, and Windows Event Log
 - Enable or disable each logging method as needed
 - Easy setup and configuration
 
 ## Requirements
 
-- Python 3.6 or higher
+- Python 3.9 or higher
 
 For Windows Event Log support, the following packages are required:
 
 - pywin32
 
 Install the required packages by running:
```

### Comparing `mlogconfig-0.2.0/setup.py` & `mlogconfig-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mlogconfig",
-    version="0.2.0",
+    version="0.2.1",
     author="Matt Wyen",
     author_email="matt@mattwyen.me",
     description="A simple logging setup utility that configures logging with file, console, syslog, and Windows event log handlers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/talltechy/mlogconfig",
     packages=find_packages(),
```

