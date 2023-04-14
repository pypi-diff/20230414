# Comparing `tmp/datamachine-0.0.1.tar.gz` & `tmp/datamachine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamachine-0.0.1.tar", last modified: Thu Apr 13 18:45:44 2023, max compression
+gzip compressed data, was "datamachine-0.0.2.tar", last modified: Fri Apr 14 02:08:11 2023, max compression
```

## Comparing `datamachine-0.0.1.tar` & `datamachine-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:45:44.930845 datamachine-0.0.1/
--rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      755 2023-04-13 18:45:44.930845 datamachine-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      139 2023-04-13 18:21:44.000000 datamachine-0.0.1/README.md
--rw-rw-rw-   0        0        0      674 2023-04-13 18:31:43.000000 datamachine-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      634 2023-04-13 18:45:44.932846 datamachine-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 18:45:44.912371 datamachine-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 18:45:44.917613 datamachine-0.0.1/src/datamachine/
--rw-rw-rw-   0        0        0      121 2023-04-13 17:50:17.000000 datamachine-0.0.1/src/datamachine/__init__.py
--rw-rw-rw-   0        0        0     3538 2023-04-13 18:31:43.000000 datamachine-0.0.1/src/datamachine/modular.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:45:44.929922 datamachine-0.0.1/src/datamachine.egg-info/
--rw-rw-rw-   0        0        0      755 2023-04-13 18:45:44.000000 datamachine-0.0.1/src/datamachine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-04-13 18:45:44.000000 datamachine-0.0.1/src/datamachine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:45:44.000000 datamachine-0.0.1/src/datamachine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 18:45:44.000000 datamachine-0.0.1/src/datamachine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-13 18:45:44.000000 datamachine-0.0.1/src/datamachine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 02:08:11.410140 datamachine-0.0.2/
+-rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      755 2023-04-14 02:08:11.411132 datamachine-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      139 2023-04-13 18:21:44.000000 datamachine-0.0.2/README.md
+-rw-rw-rw-   0        0        0      652 2023-04-14 02:07:49.000000 datamachine-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      634 2023-04-14 02:08:11.411851 datamachine-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 02:08:11.399408 datamachine-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 02:08:11.403128 datamachine-0.0.2/src/datamachine/
+-rw-rw-rw-   0        0        0      121 2023-04-13 17:50:17.000000 datamachine-0.0.2/src/datamachine/__init__.py
+-rw-rw-rw-   0        0        0     4644 2023-04-14 02:00:26.000000 datamachine-0.0.2/src/datamachine/modular.py
+drwxrwxrwx   0        0        0        0 2023-04-14 02:08:11.410140 datamachine-0.0.2/src/datamachine.egg-info/
+-rw-rw-rw-   0        0        0      755 2023-04-14 02:08:11.000000 datamachine-0.0.2/src/datamachine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-14 02:08:11.000000 datamachine-0.0.2/src/datamachine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 02:08:11.000000 datamachine-0.0.2/src/datamachine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 02:08:11.000000 datamachine-0.0.2/src/datamachine.egg-info/top_level.txt
```

### Comparing `datamachine-0.0.1/LICENSE` & `datamachine-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datamachine-0.0.1/PKG-INFO` & `datamachine-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.1
+Version: 0.0.2
 Summary: A data machine made of modular Python notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datamachine-0.0.1/pyproject.toml` & `datamachine-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamachine"
-version = "0.0.1"
-dependencies = [
-  'ipynb >= 0.5.1'
-]
+version = "0.0.2"
+dependencies = []
 authors = [
   { name="Dave Killough", email="dave.killough@gmail.com" },
 ]
 description = "A data machine made of modular Python notebooks"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `datamachine-0.0.1/setup.cfg` & `datamachine-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6174 616d 6163 6869 6e65 0d0a   = datamachine..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 310d  version = 0.0.1.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 320d  version = 0.0.2.
 00000030: 0a61 7574 686f 7220 3d20 4461 7665 204b  .author = Dave K
 00000040: 696c 6c6f 7567 680d 0a61 7574 686f 725f  illough..author_
 00000050: 656d 6169 6c20 3d20 6461 7665 2e6b 696c  email = dave.kil
 00000060: 6c6f 7567 6840 676d 6169 6c2e 636f 6d0d  lough@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 2064 6174 6120 6d61 6368 696e 6520 6d61   data machine ma
 00000090: 6465 206f 6620 6d6f 6475 6c61 7220 5079  de of modular Py
```

### Comparing `datamachine-0.0.1/src/datamachine.egg-info/PKG-INFO` & `datamachine-0.0.2/src/datamachine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamachine
-Version: 0.0.1
+Version: 0.0.2
 Summary: A data machine made of modular Python notebooks
 Home-page: https://pypi.org/project/datamachine
 Author: Dave Killough
 Author-email: Dave Killough <dave.killough@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
```

