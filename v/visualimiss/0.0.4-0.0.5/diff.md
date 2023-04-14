# Comparing `tmp/visualimiss-0.0.4.tar.gz` & `tmp/visualimiss-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualimiss-0.0.4.tar", last modified: Fri Apr 14 16:31:09 2023, max compression
+gzip compressed data, was "visualimiss-0.0.5.tar", last modified: Fri Apr 14 16:41:13 2023, max compression
```

## Comparing `visualimiss-0.0.4.tar` & `visualimiss-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 16:31:09.996724 visualimiss-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-04-14 15:05:45.000000 visualimiss-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      767 2023-04-14 16:31:09.995724 visualimiss-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-04-14 16:28:41.000000 visualimiss-0.0.4/README.md
--rw-rw-rw-   0        0        0      514 2023-04-14 16:30:55.000000 visualimiss-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 16:31:09.996724 visualimiss-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 16:31:09.983693 visualimiss-0.0.4/visualimiss/
--rw-rw-rw-   0        0        0       94 2023-04-14 16:04:41.000000 visualimiss-0.0.4/visualimiss/__init__.py
--rw-rw-rw-   0        0        0      431 2023-04-13 16:51:12.000000 visualimiss-0.0.4/visualimiss/utils.py
--rw-rw-rw-   0        0        0     2467 2023-04-14 02:12:37.000000 visualimiss-0.0.4/visualimiss/visualimiss.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:31:09.994723 visualimiss-0.0.4/visualimiss.egg-info/
--rw-rw-rw-   0        0        0      767 2023-04-14 16:31:09.000000 visualimiss-0.0.4/visualimiss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-14 16:31:09.000000 visualimiss-0.0.4/visualimiss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 16:31:09.000000 visualimiss-0.0.4/visualimiss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 16:31:09.000000 visualimiss-0.0.4/visualimiss.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 16:41:13.574809 visualimiss-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-04-14 15:05:45.000000 visualimiss-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      835 2023-04-14 16:41:13.572796 visualimiss-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-04-14 16:40:40.000000 visualimiss-0.0.5/README.md
+-rw-rw-rw-   0        0        0      514 2023-04-14 16:39:01.000000 visualimiss-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 16:41:13.575816 visualimiss-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 16:41:13.558163 visualimiss-0.0.5/visualimiss/
+-rw-rw-rw-   0        0        0       94 2023-04-14 16:04:41.000000 visualimiss-0.0.5/visualimiss/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-04-13 16:51:12.000000 visualimiss-0.0.5/visualimiss/utils.py
+-rw-rw-rw-   0        0        0     2467 2023-04-14 02:12:37.000000 visualimiss-0.0.5/visualimiss/visualimiss.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:41:13.571282 visualimiss-0.0.5/visualimiss.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-04-14 16:41:13.000000 visualimiss-0.0.5/visualimiss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-04-14 16:41:13.000000 visualimiss-0.0.5/visualimiss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:41:13.000000 visualimiss-0.0.5/visualimiss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 16:41:13.000000 visualimiss-0.0.5/visualimiss.egg-info/top_level.txt
```

### Comparing `visualimiss-0.0.4/LICENSE` & `visualimiss-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `visualimiss-0.0.4/PKG-INFO` & `visualimiss-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualimiss
-Version: 0.0.4
+Version: 0.0.5
 Summary: A missingno clone, use to visualize missing data
 Author: ngntrgduc
 Project-URL: Homepage, https://github.com/ngntrgduc/visualimiss
 Project-URL: Bug Tracker, https://github.com/ngntrgduc/visualimiss/issues
 Keywords: data,data visualization,missing data
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,9 +17,10 @@
 # Installation
 ```python
 pip install visualimiss
 ```
 
 # Features
 Some features differ from the original one:
+- Have `matrix()`, `bar()` modified function from the original one
 - Simpler and faster
 - Maybe more readable?
```

### Comparing `visualimiss-0.0.4/pyproject.toml` & `visualimiss-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "visualimiss"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="ngntrgduc"},
 ]
 description = "A missingno clone, use to visualize missing data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = []
```

### Comparing `visualimiss-0.0.4/visualimiss/visualimiss.py` & `visualimiss-0.0.5/visualimiss/visualimiss.py`

 * *Files identical despite different names*

### Comparing `visualimiss-0.0.4/visualimiss.egg-info/PKG-INFO` & `visualimiss-0.0.5/visualimiss.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualimiss
-Version: 0.0.4
+Version: 0.0.5
 Summary: A missingno clone, use to visualize missing data
 Author: ngntrgduc
 Project-URL: Homepage, https://github.com/ngntrgduc/visualimiss
 Project-URL: Bug Tracker, https://github.com/ngntrgduc/visualimiss/issues
 Keywords: data,data visualization,missing data
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,9 +17,10 @@
 # Installation
 ```python
 pip install visualimiss
 ```
 
 # Features
 Some features differ from the original one:
+- Have `matrix()`, `bar()` modified function from the original one
 - Simpler and faster
 - Maybe more readable?
```

