# Comparing `tmp/statistics_core-0.0.2.tar.gz` & `tmp/statistics_core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statistics_core-0.0.2.tar", last modified: Fri Apr 14 17:52:46 2023, max compression
+gzip compressed data, was "statistics_core-0.0.3.tar", last modified: Fri Apr 14 17:57:07 2023, max compression
```

## Comparing `statistics_core-0.0.2.tar` & `statistics_core-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 17:52:46.214356 statistics_core-0.0.2/
--rw-rw-r--   0 lokas     (1000) lokas     (1000)     1087 2023-04-14 13:51:29.000000 statistics_core-0.0.2/LICENSE
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      605 2023-04-14 17:52:46.214356 statistics_core-0.0.2/PKG-INFO
--rw-rw-r--   0 lokas     (1000) lokas     (1000)       36 2023-04-14 13:01:03.000000 statistics_core-0.0.2/README.md
--rw-rw-r--   0 lokas     (1000) lokas     (1000)       38 2023-04-14 17:52:46.214356 statistics_core-0.0.2/setup.cfg
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      929 2023-04-14 17:49:35.000000 statistics_core-0.0.2/setup.py
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 17:52:46.210356 statistics_core-0.0.2/src/
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 17:52:46.210356 statistics_core-0.0.2/src/module/
--rw-rw-r--   0 lokas     (1000) lokas     (1000)        0 2023-04-14 13:04:33.000000 statistics_core-0.0.2/src/module/__init__.py
--rw-rw-r--   0 lokas     (1000) lokas     (1000)     6999 2023-04-14 13:38:43.000000 statistics_core-0.0.2/src/module/module.py
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 17:52:46.214356 statistics_core-0.0.2/src/statistics_core.egg-info/
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      605 2023-04-14 17:52:46.000000 statistics_core-0.0.2/src/statistics_core.egg-info/PKG-INFO
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      242 2023-04-14 17:52:46.000000 statistics_core-0.0.2/src/statistics_core.egg-info/SOURCES.txt
--rw-rw-r--   0 lokas     (1000) lokas     (1000)        1 2023-04-14 17:52:46.000000 statistics_core-0.0.2/src/statistics_core.egg-info/dependency_links.txt
--rw-rw-r--   0 lokas     (1000) lokas     (1000)        7 2023-04-14 17:52:46.000000 statistics_core-0.0.2/src/statistics_core.egg-info/top_level.txt
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 17:57:07.716809 statistics_core-0.0.3/
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)     1087 2023-04-14 13:51:29.000000 statistics_core-0.0.3/LICENSE
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)      605 2023-04-14 17:57:07.716809 statistics_core-0.0.3/PKG-INFO
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)       36 2023-04-14 13:01:03.000000 statistics_core-0.0.3/README.md
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)       38 2023-04-14 17:57:07.716809 statistics_core-0.0.3/setup.cfg
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)      929 2023-04-14 17:56:57.000000 statistics_core-0.0.3/setup.py
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 17:57:07.716809 statistics_core-0.0.3/src/
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 17:57:07.716809 statistics_core-0.0.3/src/statistics_core/
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)        0 2023-04-14 13:04:33.000000 statistics_core-0.0.3/src/statistics_core/__init__.py
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)     6999 2023-04-14 13:38:43.000000 statistics_core-0.0.3/src/statistics_core/module.py
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 17:57:07.716809 statistics_core-0.0.3/src/statistics_core.egg-info/
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)      605 2023-04-14 17:57:07.000000 statistics_core-0.0.3/src/statistics_core.egg-info/PKG-INFO
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)      260 2023-04-14 17:57:07.000000 statistics_core-0.0.3/src/statistics_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)        1 2023-04-14 17:57:07.000000 statistics_core-0.0.3/src/statistics_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)       16 2023-04-14 17:57:07.000000 statistics_core-0.0.3/src/statistics_core.egg-info/top_level.txt
```

### Comparing `statistics_core-0.0.2/LICENSE` & `statistics_core-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `statistics_core-0.0.2/PKG-INFO` & `statistics_core-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statistics_core
-Version: 0.0.2
+Version: 0.0.3
 Summary: short package description
 Home-page: https://github.com/LokasWiki/statistics-core
 Author: LokasWiki
 Project-URL: Bug Tracker, https://github.com/LokasWiki/statistics-core/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statistics_core-0.0.2/setup.py` & `statistics_core-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "statistics_core",
-    version = "0.0.2",
+    version = "0.0.3",
     author = "LokasWiki",
     # author_email = "author@example.com",
     description = "short package description",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/LokasWiki/statistics-core",
     project_urls = {
```

### Comparing `statistics_core-0.0.2/src/module/module.py` & `statistics_core-0.0.3/src/statistics_core/module.py`

 * *Files identical despite different names*

### Comparing `statistics_core-0.0.2/src/statistics_core.egg-info/PKG-INFO` & `statistics_core-0.0.3/src/statistics_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statistics-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: short package description
 Home-page: https://github.com/LokasWiki/statistics-core
 Author: LokasWiki
 Project-URL: Bug Tracker, https://github.com/LokasWiki/statistics-core/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

