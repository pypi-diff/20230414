# Comparing `tmp/htmlpack-0.1.1.tar.gz` & `tmp/htmlpack-0.1.2.tar.gz`

## Comparing `htmlpack-0.1.1.tar` & `htmlpack-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    20569 2020-02-02 00:00:00.000000 htmlpack-0.1.1/.pylintrc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 htmlpack-0.1.1/htmlpack/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 htmlpack-0.1.1/htmlpack/__main__.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 htmlpack-0.1.1/htmlpack/htmlpack.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 htmlpack-0.1.1/test_data/nested_example.html.txt
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 htmlpack-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 htmlpack-0.1.1/LICENSE
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 htmlpack-0.1.1/README.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 htmlpack-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 htmlpack-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    20569 2020-02-02 00:00:00.000000 htmlpack-0.1.2/.pylintrc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 htmlpack-0.1.2/htmlpack/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 htmlpack-0.1.2/htmlpack/__main__.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 htmlpack-0.1.2/htmlpack/htmlpack.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 htmlpack-0.1.2/test_data/nested_example.html.txt
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 htmlpack-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 htmlpack-0.1.2/LICENSE
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 htmlpack-0.1.2/README.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 htmlpack-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 htmlpack-0.1.2/PKG-INFO
```

### Comparing `htmlpack-0.1.1/.pylintrc` & `htmlpack-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `htmlpack-0.1.1/htmlpack/htmlpack.py` & `htmlpack-0.1.2/htmlpack/htmlpack.py`

 * *Files identical despite different names*

### Comparing `htmlpack-0.1.1/.gitignore` & `htmlpack-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `htmlpack-0.1.1/LICENSE` & `htmlpack-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `htmlpack-0.1.1/README.md` & `htmlpack-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # htmlpack
 The htmlpack module can be used to help preprocess HTML files for production environments. It can be used to strip HTML comments, minify HTML,
 and more.
 
 ```
-usage: htmlpack.py [-h] [-s] [-v] [-d] path
+usage: python -m htmlpack [-h] [-s] [-v] [-d] path
 
 positional arguments:
   path                  Path to file or folder
 
 optional arguments:
   -h, --help            show this help message and exit
   -s, --strip-comments  Whether to strip HTML comments (default: False)
```

### Comparing `htmlpack-0.1.1/pyproject.toml` & `htmlpack-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "htmlpack"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Conor Maguire", email="conormag@gmail.com" },
 ]
 description = "Pre-process HTML files for production environments. Strip HTML comments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `htmlpack-0.1.1/PKG-INFO` & `htmlpack-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htmlpack
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pre-process HTML files for production environments. Strip HTML comments.
 Project-URL: Homepage, https://github.com/conormag/htmlpack
 Project-URL: Bug Tracker, https://github.com/conormag/htmlpack/issues
 Author-email: Conor Maguire <conormag@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 
 # htmlpack
 The htmlpack module can be used to help preprocess HTML files for production environments. It can be used to strip HTML comments, minify HTML,
 and more.
 
 ```
-usage: htmlpack.py [-h] [-s] [-v] [-d] path
+usage: python -m htmlpack [-h] [-s] [-v] [-d] path
 
 positional arguments:
   path                  Path to file or folder
 
 optional arguments:
   -h, --help            show this help message and exit
   -s, --strip-comments  Whether to strip HTML comments (default: False)
```

