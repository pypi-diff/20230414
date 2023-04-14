# Comparing `tmp/statistics_core-0.0.5.tar.gz` & `tmp/statistics_core-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statistics_core-0.0.5.tar", last modified: Fri Apr 14 18:07:04 2023, max compression
+gzip compressed data, was "statistics_core-0.0.6.tar", last modified: Fri Apr 14 19:08:42 2023, max compression
```

## Comparing `statistics_core-0.0.5.tar` & `statistics_core-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 18:07:04.485673 statistics_core-0.0.5/
--rw-rw-r--   0 lokas     (1000) lokas     (1000)     1087 2023-04-14 13:51:29.000000 statistics_core-0.0.5/LICENSE
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      775 2023-04-14 18:07:04.485673 statistics_core-0.0.5/PKG-INFO
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      206 2023-04-14 18:06:01.000000 statistics_core-0.0.5/README.md
--rw-rw-r--   0 lokas     (1000) lokas     (1000)       38 2023-04-14 18:07:04.485673 statistics_core-0.0.5/setup.cfg
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      929 2023-04-14 18:06:39.000000 statistics_core-0.0.5/setup.py
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 18:07:04.485673 statistics_core-0.0.5/src/
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 18:07:04.485673 statistics_core-0.0.5/src/statistics_core/
--rw-rw-r--   0 lokas     (1000) lokas     (1000)        0 2023-04-14 13:04:33.000000 statistics_core-0.0.5/src/statistics_core/__init__.py
--rw-rw-r--   0 lokas     (1000) lokas     (1000)     6999 2023-04-14 13:38:43.000000 statistics_core-0.0.5/src/statistics_core/module.py
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 18:07:04.485673 statistics_core-0.0.5/src/statistics_core.egg-info/
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      775 2023-04-14 18:07:04.000000 statistics_core-0.0.5/src/statistics_core.egg-info/PKG-INFO
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      260 2023-04-14 18:07:04.000000 statistics_core-0.0.5/src/statistics_core.egg-info/SOURCES.txt
--rw-rw-r--   0 lokas     (1000) lokas     (1000)        1 2023-04-14 18:07:04.000000 statistics_core-0.0.5/src/statistics_core.egg-info/dependency_links.txt
--rw-rw-r--   0 lokas     (1000) lokas     (1000)       16 2023-04-14 18:07:04.000000 statistics_core-0.0.5/src/statistics_core.egg-info/top_level.txt
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:08:42.860601 statistics_core-0.0.6/
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)     1087 2023-04-14 13:51:29.000000 statistics_core-0.0.6/LICENSE
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)     2595 2023-04-14 19:08:42.860601 statistics_core-0.0.6/PKG-INFO
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)     2026 2023-04-14 18:50:52.000000 statistics_core-0.0.6/README.md
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)       38 2023-04-14 19:08:42.860601 statistics_core-0.0.6/setup.cfg
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)      929 2023-04-14 19:08:39.000000 statistics_core-0.0.6/setup.py
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:08:42.860601 statistics_core-0.0.6/src/
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:08:42.860601 statistics_core-0.0.6/src/statistics_core/
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)        0 2023-04-14 13:04:33.000000 statistics_core-0.0.6/src/statistics_core/__init__.py
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)    15249 2023-04-14 18:50:10.000000 statistics_core-0.0.6/src/statistics_core/module.py
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:08:42.860601 statistics_core-0.0.6/src/statistics_core.egg-info/
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)     2595 2023-04-14 19:08:42.000000 statistics_core-0.0.6/src/statistics_core.egg-info/PKG-INFO
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)      260 2023-04-14 19:08:42.000000 statistics_core-0.0.6/src/statistics_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)        1 2023-04-14 19:08:42.000000 statistics_core-0.0.6/src/statistics_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)       16 2023-04-14 19:08:42.000000 statistics_core-0.0.6/src/statistics_core.egg-info/top_level.txt
```

### Comparing `statistics_core-0.0.5/LICENSE` & `statistics_core-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `statistics_core-0.0.5/setup.py` & `statistics_core-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "statistics_core",
-    version = "0.0.5",
+    version = "0.0.6",
     author = "LokasWiki",
     # author_email = "author@example.com",
     description = "short package description",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/LokasWiki/statistics-core",
     project_urls = {
```

