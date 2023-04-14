# Comparing `tmp/compressbinarytable-0.1.7.tar.gz` & `tmp/compressbinarytable-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compressbinarytable-0.1.7.tar", max compression
+gzip compressed data, was "compressbinarytable-0.1.8.tar", max compression
```

## Comparing `compressbinarytable-0.1.7.tar` & `compressbinarytable-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1095 2023-04-14 12:55:11.652795 compressbinarytable-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-04-14 10:19:30.058694 compressbinarytable-0.1.7/compressbinarytable/__init__.py
--rw-r--r--   0        0        0     7810 2023-04-14 12:41:35.548262 compressbinarytable-0.1.7/compressbinarytable/compressbinarytable.py
--rw-r--r--   0        0        0      625 2023-04-14 12:55:22.915220 compressbinarytable-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 compressbinarytable-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1125 2023-04-14 12:56:55.183428 compressbinarytable-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 10:19:30.058694 compressbinarytable-0.1.8/compressbinarytable/__init__.py
+-rw-r--r--   0        0        0     7810 2023-04-14 12:41:35.548262 compressbinarytable-0.1.8/compressbinarytable/compressbinarytable.py
+-rw-r--r--   0        0        0      625 2023-04-14 12:58:44.122244 compressbinarytable-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 compressbinarytable-0.1.8/PKG-INFO
```

### Comparing `compressbinarytable-0.1.7/compressbinarytable/compressbinarytable.py` & `compressbinarytable-0.1.8/compressbinarytable/compressbinarytable.py`

 * *Files identical despite different names*

### Comparing `compressbinarytable-0.1.7/pyproject.toml` & `compressbinarytable-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "compressbinarytable"
-version = "0.1.7"
+version = "0.1.8"
 repository = ""
 readme = "README.md"
 description = "Compression of binary table"
 authors = ["Alper Yurtseven <alper.yurtseven@helmholtz-hips.de>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: OS Independent"
```

### Comparing `compressbinarytable-0.1.7/PKG-INFO` & `compressbinarytable-0.1.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: compressbinarytable
-Version: 0.1.7
-Summary: Compression of binary table
-Author: Alper Yurtseven
-Author-email: alper.yurtseven@helmholtz-hips.de
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.21.4,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Description-Content-Type: text/markdown
-
 # CompressBinaryTable
  
 ## Basic Usage:
 
 ```console
 
 cbt -i input_file -o output_file -c 
@@ -51,32 +33,43 @@
 
 ```
 
 ## Required file example:
 
 ### CSV:
 
+```
+
 strain_name,mut1,mut2,mut3,mut4,outcome
 strain1,0,1,1,1,1,1
 strain2,0,0,1,1,1,0
 strain3,0,1,0,1,1,0
 strain4,1,1,1,1,1,1
 
+```
+
 ### TSV:
 
+```
+
 strain_name mut1    mut2    mut3    mut4    outcome
 strain1 0   1   1   1   1   1
 strain2 0   0   1   1   1   0
 strain3 0   1   0   1   1   0
 strain4 1   1   1   1   1   1
 
+```
+
 ### CBT:
 
+```
+
 1;mut1;mut2;mut3;mut4;outcome
 strain1;6;43;87;102
 strain2;16;43;87;102
 strain3;6;53;78;112
 strain4;61;413;824;942
 
+```
```

