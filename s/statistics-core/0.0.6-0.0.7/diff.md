# Comparing `tmp/statistics_core-0.0.6.tar.gz` & `tmp/statistics_core-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statistics_core-0.0.6.tar", last modified: Fri Apr 14 19:08:42 2023, max compression
+gzip compressed data, was "statistics_core-0.0.7.tar", last modified: Fri Apr 14 19:10:11 2023, max compression
```

## Comparing `statistics_core-0.0.6.tar` & `statistics_core-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:08:42.860601 statistics_core-0.0.6/
--rw-rw-r--   0 lokas     (1000) lokas     (1000)     1087 2023-04-14 13:51:29.000000 statistics_core-0.0.6/LICENSE
--rw-rw-r--   0 lokas     (1000) lokas     (1000)     2595 2023-04-14 19:08:42.860601 statistics_core-0.0.6/PKG-INFO
--rw-rw-r--   0 lokas     (1000) lokas     (1000)     2026 2023-04-14 18:50:52.000000 statistics_core-0.0.6/README.md
--rw-rw-r--   0 lokas     (1000) lokas     (1000)       38 2023-04-14 19:08:42.860601 statistics_core-0.0.6/setup.cfg
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      929 2023-04-14 19:08:39.000000 statistics_core-0.0.6/setup.py
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:08:42.860601 statistics_core-0.0.6/src/
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:08:42.860601 statistics_core-0.0.6/src/statistics_core/
--rw-rw-r--   0 lokas     (1000) lokas     (1000)        0 2023-04-14 13:04:33.000000 statistics_core-0.0.6/src/statistics_core/__init__.py
--rw-rw-r--   0 lokas     (1000) lokas     (1000)    15249 2023-04-14 18:50:10.000000 statistics_core-0.0.6/src/statistics_core/module.py
-drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:08:42.860601 statistics_core-0.0.6/src/statistics_core.egg-info/
--rw-rw-r--   0 lokas     (1000) lokas     (1000)     2595 2023-04-14 19:08:42.000000 statistics_core-0.0.6/src/statistics_core.egg-info/PKG-INFO
--rw-rw-r--   0 lokas     (1000) lokas     (1000)      260 2023-04-14 19:08:42.000000 statistics_core-0.0.6/src/statistics_core.egg-info/SOURCES.txt
--rw-rw-r--   0 lokas     (1000) lokas     (1000)        1 2023-04-14 19:08:42.000000 statistics_core-0.0.6/src/statistics_core.egg-info/dependency_links.txt
--rw-rw-r--   0 lokas     (1000) lokas     (1000)       16 2023-04-14 19:08:42.000000 statistics_core-0.0.6/src/statistics_core.egg-info/top_level.txt
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:10:11.804168 statistics_core-0.0.7/
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)     1087 2023-04-14 13:51:29.000000 statistics_core-0.0.7/LICENSE
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)     3882 2023-04-14 19:10:11.804168 statistics_core-0.0.7/PKG-INFO
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)     3313 2023-04-14 19:09:55.000000 statistics_core-0.0.7/README.md
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)       38 2023-04-14 19:10:11.804168 statistics_core-0.0.7/setup.cfg
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)      929 2023-04-14 19:10:09.000000 statistics_core-0.0.7/setup.py
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:10:11.804168 statistics_core-0.0.7/src/
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:10:11.804168 statistics_core-0.0.7/src/statistics_core/
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)        0 2023-04-14 13:04:33.000000 statistics_core-0.0.7/src/statistics_core/__init__.py
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)    15249 2023-04-14 18:50:10.000000 statistics_core-0.0.7/src/statistics_core/module.py
+drwxrwxr-x   0 lokas     (1000) lokas     (1000)        0 2023-04-14 19:10:11.804168 statistics_core-0.0.7/src/statistics_core.egg-info/
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)     3882 2023-04-14 19:10:11.000000 statistics_core-0.0.7/src/statistics_core.egg-info/PKG-INFO
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)      260 2023-04-14 19:10:11.000000 statistics_core-0.0.7/src/statistics_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)        1 2023-04-14 19:10:11.000000 statistics_core-0.0.7/src/statistics_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 lokas     (1000) lokas     (1000)       16 2023-04-14 19:10:11.000000 statistics_core-0.0.7/src/statistics_core.egg-info/top_level.txt
```

### Comparing `statistics_core-0.0.6/LICENSE` & `statistics_core-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `statistics_core-0.0.6/PKG-INFO` & `statistics_core-0.0.7/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: statistics_core
-Version: 0.0.6
-Summary: short package description
-Home-page: https://github.com/LokasWiki/statistics-core
-Author: LokasWiki
-Project-URL: Bug Tracker, https://github.com/LokasWiki/statistics-core/issues
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # statistics-core
 [![PyPI version](https://badge.fury.io/py/statistics-core.svg)](https://badge.fury.io/py/statistics-core)
 
 Installing `statistics-core` 📊
 -------------------------------
 
 ### Using `pip` 🐍
@@ -67,9 +51,27 @@
 5.  After the installation is complete, you can use `statistics-core` in your Python program by simply importing it using the following command:
 
 ``` python
 import statistics_core
 ```
 After importing the library, you can use the functions and tools provided by `statistics-core` in your Python programs. 🚀
 
+👋 Welcome to this code repository!
+-------------------------------
+Here you'll find a set of classes that allow you to fetch data from a database and display it in a table on a wiki page.
+
+🗃️ The `Database` class connects to a database and runs a query to retrieve data. The results are stored in the `result` attribute, which can be accessed by other classes.
+
+📄 The `File` class reads the contents of a file and stores it in the `contents` attribute. It can also construct a file path based on the location of the script.
+
+📝 The `Page` class represents a wiki page and allows you to set its contents and save it.
+
+📊 The `ArticleTable` class defines a table with columns, a sort column, and optional header and footer text. It can build the table based on the contents of the `result` attribute of the `Database` class.
+
+📚 The `ArticleTables` class allows you to define multiple `ArticleTable` instances and add them to a list.
+
+🔄 The `UpdatePage` class takes a `Database` instance, a file path, a wiki page name, and an `ArticleTables` instance. It reads the contents of the file, replaces a placeholder string with the table content, and saves the updated content to the wiki page.
+
+👨‍💻 Have fun exploring and using these classes in your own projects!
+
 ## شرح الاستخدام 
 ## اسئله شائعه
```

### Comparing `statistics_core-0.0.6/setup.py` & `statistics_core-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "statistics_core",
-    version = "0.0.6",
+    version = "0.0.7",
     author = "LokasWiki",
     # author_email = "author@example.com",
     description = "short package description",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/LokasWiki/statistics-core",
     project_urls = {
```

### Comparing `statistics_core-0.0.6/src/statistics_core/module.py` & `statistics_core-0.0.7/src/statistics_core/module.py`

 * *Files identical despite different names*

