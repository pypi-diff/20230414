# Comparing `tmp/byebyelogger-0.2.0.tar.gz` & `tmp/ByeByeLogger-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byebyelogger-0.2.0.tar", last modified: Fri Apr 14 11:11:41 2023, max compression
+gzip compressed data, was "ByeByeLogger-0.3.0.tar", last modified: Fri Apr 14 11:27:54 2023, max compression
```

## Comparing `byebyelogger-0.2.0.tar` & `ByeByeLogger-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/
--rw-rw-rw-   0        0        0     1159 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-04-14 09:14:53.000000 byebyelogger-0.2.0/README.md
--rw-rw-rw-   0        0        0     1027 2023-04-14 11:07:07.000000 byebyelogger-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.690540 byebyelogger-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.690540 byebyelogger-0.2.0/src/byebyelogger/
--rw-rw-rw-   0        0        0        0 2023-04-11 17:13:48.000000 byebyelogger-0.2.0/src/byebyelogger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/src/byebyelogger/core/
--rw-rw-rw-   0        0        0        0 2023-04-13 15:02:15.000000 byebyelogger-0.2.0/src/byebyelogger/core/__init__.py
--rw-rw-rw-   0        0        0      425 2023-04-14 08:52:54.000000 byebyelogger-0.2.0/src/byebyelogger/core/abstract.py
--rw-rw-rw-   0        0        0      158 2023-04-14 08:54:51.000000 byebyelogger-0.2.0/src/byebyelogger/core/byebyelogger.py
--rw-rw-rw-   0        0        0     1968 2023-04-14 08:45:06.000000 byebyelogger-0.2.0/src/byebyelogger/core/repository.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/src/byebyelogger/presets/
--rw-rw-rw-   0        0        0        0 2023-04-13 15:05:43.000000 byebyelogger-0.2.0/src/byebyelogger/presets/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-13 15:06:01.000000 byebyelogger-0.2.0/src/byebyelogger/presets/custom.py
--rw-rw-rw-   0        0        0     1651 2023-04-14 09:19:07.000000 byebyelogger-0.2.0/src/byebyelogger/presets/datascience.py
--rw-rw-rw-   0        0        0        0 2023-04-14 09:18:58.000000 byebyelogger-0.2.0/src/byebyelogger/presets/default.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/src/byebyelogger/style/
--rw-rw-rw-   0        0        0       69 2023-04-14 09:01:09.000000 byebyelogger-0.2.0/src/byebyelogger/style/__init__.py
--rw-rw-rw-   0        0        0     1058 2023-04-14 06:36:00.000000 byebyelogger-0.2.0/src/byebyelogger/style/colorizer.py
--rw-rw-rw-   0        0        0      500 2023-04-13 15:17:12.000000 byebyelogger-0.2.0/src/byebyelogger/style/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.706153 byebyelogger-0.2.0/src/byebyelogger.egg-info/
--rw-rw-rw-   0        0        0     1159 2023-04-14 11:11:41.000000 byebyelogger-0.2.0/src/byebyelogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2023-04-14 11:11:41.000000 byebyelogger-0.2.0/src/byebyelogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 11:11:41.000000 byebyelogger-0.2.0/src/byebyelogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-14 11:11:41.000000 byebyelogger-0.2.0/src/byebyelogger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 11:11:41.000000 byebyelogger-0.2.0/src/byebyelogger.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 11:11:41.721782 byebyelogger-0.2.0/tests/
--rw-rw-rw-   0        0        0      217 2023-04-14 08:52:33.000000 byebyelogger-0.2.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.996265 ByeByeLogger-0.3.0/
+-rw-rw-rw-   0        0        0     1159 2023-04-14 11:27:54.995266 ByeByeLogger-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-04-14 09:14:53.000000 ByeByeLogger-0.3.0/README.md
+-rw-rw-rw-   0        0        0      959 2023-04-14 11:26:40.000000 ByeByeLogger-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 11:27:54.996265 ByeByeLogger-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.944265 ByeByeLogger-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.968279 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/
+-rw-rw-rw-   0        0        0     1159 2023-04-14 11:27:54.000000 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-04-14 11:27:54.000000 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 11:27:54.000000 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 11:27:54.000000 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 11:27:54.000000 ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.970271 ByeByeLogger-0.3.0/src/byebyelogger/
+-rw-rw-rw-   0        0        0        0 2023-04-11 17:13:48.000000 ByeByeLogger-0.3.0/src/byebyelogger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.984264 ByeByeLogger-0.3.0/src/byebyelogger/core/
+-rw-rw-rw-   0        0        0      154 2023-04-14 11:26:03.000000 ByeByeLogger-0.3.0/src/byebyelogger/core/ByeByeLogger.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 15:02:15.000000 ByeByeLogger-0.3.0/src/byebyelogger/core/__init__.py
+-rw-rw-rw-   0        0        0      425 2023-04-14 08:52:54.000000 ByeByeLogger-0.3.0/src/byebyelogger/core/abstract.py
+-rw-rw-rw-   0        0        0     1968 2023-04-14 08:45:06.000000 ByeByeLogger-0.3.0/src/byebyelogger/core/repository.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.988263 ByeByeLogger-0.3.0/src/byebyelogger/presets/
+-rw-rw-rw-   0        0        0        0 2023-04-13 15:05:43.000000 ByeByeLogger-0.3.0/src/byebyelogger/presets/__init__.py
+-rw-rw-rw-   0        0        0     1579 2023-04-14 11:23:02.000000 ByeByeLogger-0.3.0/src/byebyelogger/presets/datascience.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.992264 ByeByeLogger-0.3.0/src/byebyelogger/style/
+-rw-rw-rw-   0        0        0        0 2023-04-14 11:23:20.000000 ByeByeLogger-0.3.0/src/byebyelogger/style/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-14 06:36:00.000000 ByeByeLogger-0.3.0/src/byebyelogger/style/colorizer.py
+-rw-rw-rw-   0        0        0      500 2023-04-13 15:17:12.000000 ByeByeLogger-0.3.0/src/byebyelogger/style/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:27:54.994263 ByeByeLogger-0.3.0/tests/
+-rw-rw-rw-   0        0        0      217 2023-04-14 08:52:33.000000 ByeByeLogger-0.3.0/tests/test.py
```

### Comparing `byebyelogger-0.2.0/PKG-INFO` & `ByeByeLogger-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: byebyelogger
-Version: 0.2.0
+Name: ByeByeLogger
+Version: 0.3.0
 Summary: A simple, yet powerful Python logging library that makes you say goodbye to your standard logger.
 Author-email: Aleksa Lukic <aleksalukic92@web.de>
 Project-URL: Homepage, https://github.com/N4r0Bs/ByeByeLogger
 Project-URL: Repository, https://github.com/N4r0Bs/ByeByeLogger
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `byebyelogger-0.2.0/pyproject.toml` & `ByeByeLogger-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
-[tool.setuptools_scm]
-write_to = "src/byebyelogger/_version.py"
-
 [project]
-name = "byebyelogger"
-version = "0.2.0"
+name = "ByeByeLogger"
+version = "0.3.0"
 description = "A simple, yet powerful Python logging library that makes you say goodbye to your standard logger."
 authors = [
     {name = "Aleksa Lukic", email = "aleksalukic92@web.de"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `byebyelogger-0.2.0/src/byebyelogger/core/repository.py` & `ByeByeLogger-0.3.0/src/byebyelogger/core/repository.py`

 * *Files identical despite different names*

### Comparing `byebyelogger-0.2.0/src/byebyelogger/presets/datascience.py` & `ByeByeLogger-0.3.0/src/byebyelogger/presets/datascience.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,10 +36,7 @@
 PRESET_INFO = custom.copy()
 PRESET_INFO.attributes["level"] = (LIGHTCYAN_EX("INFO"), SQUARE_BRACKETS)
 
 
 PRESET_ERROR = custom.copy()
 PRESET_ERROR.attributes["level"] = (LIGHTRED_EX("ERROR"), SQUARE_BRACKETS)
 
-
-INFO = LogRepository(PRESET_INFO)
-ERROR = LogRepository(PRESET_ERROR)
```

### Comparing `byebyelogger-0.2.0/src/byebyelogger/style/colorizer.py` & `ByeByeLogger-0.3.0/src/byebyelogger/style/colorizer.py`

 * *Files identical despite different names*

### Comparing `byebyelogger-0.2.0/src/byebyelogger.egg-info/PKG-INFO` & `ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: byebyelogger
-Version: 0.2.0
+Name: ByeByeLogger
+Version: 0.3.0
 Summary: A simple, yet powerful Python logging library that makes you say goodbye to your standard logger.
 Author-email: Aleksa Lukic <aleksalukic92@web.de>
 Project-URL: Homepage, https://github.com/N4r0Bs/ByeByeLogger
 Project-URL: Repository, https://github.com/N4r0Bs/ByeByeLogger
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `byebyelogger-0.2.0/src/byebyelogger.egg-info/SOURCES.txt` & `ByeByeLogger-0.3.0/src/ByeByeLogger.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 README.md
 pyproject.toml
+src/ByeByeLogger.egg-info/PKG-INFO
+src/ByeByeLogger.egg-info/SOURCES.txt
+src/ByeByeLogger.egg-info/dependency_links.txt
+src/ByeByeLogger.egg-info/requires.txt
+src/ByeByeLogger.egg-info/top_level.txt
 src/byebyelogger/__init__.py
 src/byebyelogger.egg-info/PKG-INFO
 src/byebyelogger.egg-info/SOURCES.txt
 src/byebyelogger.egg-info/dependency_links.txt
 src/byebyelogger.egg-info/requires.txt
 src/byebyelogger.egg-info/top_level.txt
+src/byebyelogger/core/ByeByeLogger.py
 src/byebyelogger/core/__init__.py
 src/byebyelogger/core/abstract.py
 src/byebyelogger/core/byebyelogger.py
 src/byebyelogger/core/repository.py
 src/byebyelogger/presets/__init__.py
-src/byebyelogger/presets/custom.py
 src/byebyelogger/presets/datascience.py
-src/byebyelogger/presets/default.py
 src/byebyelogger/style/__init__.py
 src/byebyelogger/style/colorizer.py
 src/byebyelogger/style/constants.py
 tests/test.py
```

