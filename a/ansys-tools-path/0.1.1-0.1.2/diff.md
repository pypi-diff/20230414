# Comparing `tmp/ansys-tools-path-0.1.1.tar.gz` & `tmp/ansys-tools-path-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-tools-path-0.1.1.tar", last modified: Thu Apr 13 08:14:07 2023, max compression
+gzip compressed data, was "ansys-tools-path-0.1.2.tar", last modified: Fri Apr 14 12:51:30 2023, max compression
```

## Comparing `ansys-tools-path-0.1.1.tar` & `ansys-tools-path-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-04-13 08:13:54.051402 ansys-tools-path-0.1.1/LICENSE
--rw-r--r--   0        0        0     4701 2023-04-13 08:13:54.051402 ansys-tools-path-0.1.1/README.rst
--rw-r--r--   0        0        0     1849 2023-04-13 08:13:54.055402 ansys-tools-path-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      404 2023-04-13 08:13:54.055402 ansys-tools-path-0.1.1/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      194 2023-04-13 08:13:54.055402 ansys-tools-path-0.1.1/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    13628 2023-04-13 08:13:54.055402 ansys-tools-path-0.1.1/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0     6192 1970-01-01 00:00:00.000000 ansys-tools-path-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4701 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/README.rst
+-rw-r--r--   0        0        0     1849 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      194 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    13647 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0     6192 1970-01-01 00:00:00.000000 ansys-tools-path-0.1.2/PKG-INFO
```

### Comparing `ansys-tools-path-0.1.1/LICENSE` & `ansys-tools-path-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.1.1/README.rst` & `ansys-tools-path-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.1.1/pyproject.toml` & `ansys-tools-path-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.1.1"
+version = "0.1.2"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `ansys-tools-path-0.1.1/src/ansys/tools/path/path.py` & `ansys-tools-path-0.1.2/src/ansys/tools/path/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 LINUX_DEFAULT_DIRS = [["/", "usr", "ansys_inc"], ["/", "ansys_inc"]]
 LINUX_DEFAULT_DIRS = [os.path.join(*each) for each in LINUX_DEFAULT_DIRS]
 
 CONFIG_FILE_NAME = "config.txt"
 
 SUPPORTED_ANSYS_VERSIONS = {
+    232: "2023R2",
     231: "2023R1",
     222: "2022R2",
     221: "2022R1",
     212: "2021R2",
     211: "2021R1",
     202: "2020R2",
     201: "2020R1",
```

### Comparing `ansys-tools-path-0.1.1/PKG-INFO` & `ansys-tools-path-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```

