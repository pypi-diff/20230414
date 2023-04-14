# Comparing `tmp/byebyelogger-0.1.0.tar.gz` & `tmp/byebyelogger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byebyelogger-0.1.0.tar", last modified: Fri Apr 14 10:52:07 2023, max compression
+gzip compressed data, was "byebyelogger-0.2.0.tar", last modified: Fri Apr 14 11:11:41 2023, max compression
```

## Comparing `byebyelogger-0.1.0.tar` & `byebyelogger-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:07.995947 byebyelogger-0.1.0/
--rw-rw-rw-   0        0        0     1159 2023-04-14 10:52:07.995947 byebyelogger-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-04-14 09:14:53.000000 byebyelogger-0.1.0/README.md
--rw-rw-rw-   0        0        0     1040 2023-04-14 10:51:09.000000 byebyelogger-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 10:52:07.995947 byebyelogger-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:07.964697 byebyelogger-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:07.964697 byebyelogger-0.1.0/src/byebyelogger/
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:07.980337 byebyelogger-0.1.0/src/byebyelogger/byebyelogger.egg-info/
--rw-rw-rw-   0        0        0     1159 2023-04-14 10:52:07.000000 byebyelogger-0.1.0/src/byebyelogger/byebyelogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      963 2023-04-14 10:52:07.000000 byebyelogger-0.1.0/src/byebyelogger/byebyelogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 10:52:07.000000 byebyelogger-0.1.0/src/byebyelogger/byebyelogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-14 10:52:07.000000 byebyelogger-0.1.0/src/byebyelogger/byebyelogger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-14 10:52:07.000000 byebyelogger-0.1.0/src/byebyelogger/byebyelogger.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:07.995947 byebyelogger-0.1.0/src/byebyelogger/core/
--rw-rw-rw-   0        0        0        0 2023-04-13 15:02:15.000000 byebyelogger-0.1.0/src/byebyelogger/core/__init__.py
--rw-rw-rw-   0        0        0      425 2023-04-14 08:52:54.000000 byebyelogger-0.1.0/src/byebyelogger/core/abstract.py
--rw-rw-rw-   0        0        0      158 2023-04-14 08:54:51.000000 byebyelogger-0.1.0/src/byebyelogger/core/byebyelogger.py
--rw-rw-rw-   0        0        0     1968 2023-04-14 08:45:06.000000 byebyelogger-0.1.0/src/byebyelogger/core/repository.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:07.995947 byebyelogger-0.1.0/src/byebyelogger/presets/
--rw-rw-rw-   0        0        0        0 2023-04-13 15:05:43.000000 byebyelogger-0.1.0/src/byebyelogger/presets/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-13 15:06:01.000000 byebyelogger-0.1.0/src/byebyelogger/presets/custom.py
--rw-rw-rw-   0        0        0     1651 2023-04-14 09:19:07.000000 byebyelogger-0.1.0/src/byebyelogger/presets/datascience.py
--rw-rw-rw-   0        0        0        0 2023-04-14 09:18:58.000000 byebyelogger-0.1.0/src/byebyelogger/presets/default.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:07.995947 byebyelogger-0.1.0/src/byebyelogger/style/
--rw-rw-rw-   0        0        0       69 2023-04-14 09:01:09.000000 byebyelogger-0.1.0/src/byebyelogger/style/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-14 06:36:00.000000 byebyelogger-0.1.0/src/byebyelogger/style/colorizer.py
--rw-rw-rw-   0        0        0      500 2023-04-13 15:17:12.000000 byebyelogger-0.1.0/src/byebyelogger/style/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:52:07.995947 byebyelogger-0.1.0/tests/
--rw-rw-rw-   0        0        0      217 2023-04-14 08:52:33.000000 byebyelogger-0.1.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/
+-rw-rw-rw-   0        0        0     1159 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-04-14 09:14:53.000000 byebyelogger-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1027 2023-04-14 11:07:07.000000 byebyelogger-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.690540 byebyelogger-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.690540 byebyelogger-0.2.0/src/byebyelogger/
+-rw-rw-rw-   0        0        0        0 2023-04-11 17:13:48.000000 byebyelogger-0.2.0/src/byebyelogger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/src/byebyelogger/core/
+-rw-rw-rw-   0        0        0        0 2023-04-13 15:02:15.000000 byebyelogger-0.2.0/src/byebyelogger/core/__init__.py
+-rw-rw-rw-   0        0        0      425 2023-04-14 08:52:54.000000 byebyelogger-0.2.0/src/byebyelogger/core/abstract.py
+-rw-rw-rw-   0        0        0      158 2023-04-14 08:54:51.000000 byebyelogger-0.2.0/src/byebyelogger/core/byebyelogger.py
+-rw-rw-rw-   0        0        0     1968 2023-04-14 08:45:06.000000 byebyelogger-0.2.0/src/byebyelogger/core/repository.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/src/byebyelogger/presets/
+-rw-rw-rw-   0        0        0        0 2023-04-13 15:05:43.000000 byebyelogger-0.2.0/src/byebyelogger/presets/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 15:06:01.000000 byebyelogger-0.2.0/src/byebyelogger/presets/custom.py
+-rw-rw-rw-   0        0        0     1651 2023-04-14 09:19:07.000000 byebyelogger-0.2.0/src/byebyelogger/presets/datascience.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 09:18:58.000000 byebyelogger-0.2.0/src/byebyelogger/presets/default.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/src/byebyelogger/style/
+-rw-rw-rw-   0        0        0       69 2023-04-14 09:01:09.000000 byebyelogger-0.2.0/src/byebyelogger/style/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-14 06:36:00.000000 byebyelogger-0.2.0/src/byebyelogger/style/colorizer.py
+-rw-rw-rw-   0        0        0      500 2023-04-13 15:17:12.000000 byebyelogger-0.2.0/src/byebyelogger/style/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.706153 byebyelogger-0.2.0/src/byebyelogger.egg-info/
+-rw-rw-rw-   0        0        0     1159 2023-04-14 11:11:41.000000 byebyelogger-0.2.0/src/byebyelogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2023-04-14 11:11:41.000000 byebyelogger-0.2.0/src/byebyelogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 11:11:41.000000 byebyelogger-0.2.0/src/byebyelogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 11:11:41.000000 byebyelogger-0.2.0/src/byebyelogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 11:11:41.000000 byebyelogger-0.2.0/src/byebyelogger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/tests/
+-rw-rw-rw-   0        0        0      217 2023-04-14 08:52:33.000000 byebyelogger-0.2.0/tests/test.py
```

### Comparing `byebyelogger-0.1.0/PKG-INFO` & `byebyelogger-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byebyelogger
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple, yet powerful Python logging library that makes you say goodbye to your standard logger.
 Author-email: Aleksa Lukic <aleksalukic92@web.de>
 Project-URL: Homepage, https://github.com/N4r0Bs/ByeByeLogger
 Project-URL: Repository, https://github.com/N4r0Bs/ByeByeLogger
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `byebyelogger-0.1.0/pyproject.toml` & `byebyelogger-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "src/byebyelogger/_version.py"
 
 [project]
 name = "byebyelogger"
-version = "0.1.0"
+version = "0.2.0"
 description = "A simple, yet powerful Python logging library that makes you say goodbye to your standard logger."
 authors = [
     {name = "Aleksa Lukic", email = "aleksalukic92@web.de"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -23,12 +23,12 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",]
     
 dependencies = [
     "colorama==0.4.6",
 ]
 [tool.setuptools.packages.find]
-where = ["src/byebyelogger"]
+where = ["src"]
 
 [project.urls]
 "Homepage" = "https://github.com/N4r0Bs/ByeByeLogger"
 "Repository" = "https://github.com/N4r0Bs/ByeByeLogger"
```

### Comparing `byebyelogger-0.1.0/src/byebyelogger/byebyelogger.egg-info/PKG-INFO` & `byebyelogger-0.2.0/src/byebyelogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byebyelogger
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple, yet powerful Python logging library that makes you say goodbye to your standard logger.
 Author-email: Aleksa Lukic <aleksalukic92@web.de>
 Project-URL: Homepage, https://github.com/N4r0Bs/ByeByeLogger
 Project-URL: Repository, https://github.com/N4r0Bs/ByeByeLogger
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `byebyelogger-0.1.0/src/byebyelogger/byebyelogger.egg-info/SOURCES.txt` & `byebyelogger-0.2.0/src/byebyelogger.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 README.md
 pyproject.toml
-src/byebyelogger/byebyelogger.egg-info/PKG-INFO
-src/byebyelogger/byebyelogger.egg-info/SOURCES.txt
-src/byebyelogger/byebyelogger.egg-info/dependency_links.txt
-src/byebyelogger/byebyelogger.egg-info/requires.txt
-src/byebyelogger/byebyelogger.egg-info/top_level.txt
-src/byebyelogger/byebyelogger.egg-info/PKG-INFO
-src/byebyelogger/byebyelogger.egg-info/SOURCES.txt
-src/byebyelogger/byebyelogger.egg-info/dependency_links.txt
-src/byebyelogger/byebyelogger.egg-info/requires.txt
-src/byebyelogger/byebyelogger.egg-info/top_level.txt
+src/byebyelogger/__init__.py
+src/byebyelogger.egg-info/PKG-INFO
+src/byebyelogger.egg-info/SOURCES.txt
+src/byebyelogger.egg-info/dependency_links.txt
+src/byebyelogger.egg-info/requires.txt
+src/byebyelogger.egg-info/top_level.txt
 src/byebyelogger/core/__init__.py
 src/byebyelogger/core/abstract.py
 src/byebyelogger/core/byebyelogger.py
 src/byebyelogger/core/repository.py
 src/byebyelogger/presets/__init__.py
 src/byebyelogger/presets/custom.py
 src/byebyelogger/presets/datascience.py
```

### Comparing `byebyelogger-0.1.0/src/byebyelogger/core/repository.py` & `byebyelogger-0.2.0/src/byebyelogger/core/repository.py`

 * *Files identical despite different names*

### Comparing `byebyelogger-0.1.0/src/byebyelogger/presets/datascience.py` & `byebyelogger-0.2.0/src/byebyelogger/presets/datascience.py`

 * *Files identical despite different names*

### Comparing `byebyelogger-0.1.0/src/byebyelogger/style/colorizer.py` & `byebyelogger-0.2.0/src/byebyelogger/style/colorizer.py`

 * *Files identical despite different names*

