# Comparing `tmp/connpy-3.0.1.tar.gz` & `tmp/connpy-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.0.1.tar", last modified: Fri Apr 14 14:58:17 2023, max compression
+gzip compressed data, was "connpy-3.0.2.tar", last modified: Fri Apr 14 16:36:22 2023, max compression
```

## Comparing `connpy-3.0.1.tar` & `connpy-3.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:58:17.987786 connpy-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 14:58:08.000000 connpy-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 14:58:17.987786 connpy-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-14 14:58:08.000000 connpy-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:58:17.987786 connpy-3.0.1/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-14 14:58:08.000000 connpy-3.0.1/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 14:58:08.000000 connpy-3.0.1/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 14:58:08.000000 connpy-3.0.1/connpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-14 14:58:08.000000 connpy-3.0.1/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-14 14:58:08.000000 connpy-3.0.1/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-14 14:58:08.000000 connpy-3.0.1/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47147 2023-04-14 14:58:08.000000 connpy-3.0.1/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27912 2023-04-14 14:58:08.000000 connpy-3.0.1/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:58:17.987786 connpy-3.0.1/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 14:58:17.000000 connpy-3.0.1/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 14:58:17.000000 connpy-3.0.1/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:58:17.000000 connpy-3.0.1/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 14:58:17.000000 connpy-3.0.1/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 14:58:17.000000 connpy-3.0.1/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 14:58:17.000000 connpy-3.0.1/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-14 14:58:17.991786 connpy-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 14:58:08.000000 connpy-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:36:22.170427 connpy-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 16:36:12.000000 connpy-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 16:36:22.170427 connpy-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-14 16:36:12.000000 connpy-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:36:22.166427 connpy-3.0.2/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-14 16:36:12.000000 connpy-3.0.2/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 16:36:12.000000 connpy-3.0.2/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:36:12.000000 connpy-3.0.2/connpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-14 16:36:12.000000 connpy-3.0.2/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-14 16:36:12.000000 connpy-3.0.2/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-14 16:36:12.000000 connpy-3.0.2/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47147 2023-04-14 16:36:12.000000 connpy-3.0.2/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27912 2023-04-14 16:36:12.000000 connpy-3.0.2/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:36:22.166427 connpy-3.0.2/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 16:36:22.000000 connpy-3.0.2/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 16:36:22.000000 connpy-3.0.2/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:36:22.000000 connpy-3.0.2/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 16:36:22.000000 connpy-3.0.2/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 16:36:22.000000 connpy-3.0.2/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 16:36:22.000000 connpy-3.0.2/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-14 16:36:22.170427 connpy-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 16:36:12.000000 connpy-3.0.2/setup.py
```

### Comparing `connpy-3.0.1/LICENSE` & `connpy-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.0.1/PKG-INFO` & `connpy-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.0.1
+Version: 3.0.2
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.0.1/README.md` & `connpy-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.0.1/connpy/__init__.py` & `connpy-3.0.2/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.1/connpy/api.py` & `connpy-3.0.2/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.1/connpy/completion.py` & `connpy-3.0.2/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.1/connpy/configfile.py` & `connpy-3.0.2/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.1/connpy/connapp.py` & `connpy-3.0.2/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.1/connpy/core.py` & `connpy-3.0.2/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.1/connpy.egg-info/PKG-INFO` & `connpy-3.0.2/connpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.0.1
+Version: 3.0.2
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.0.1/setup.cfg` & `connpy-3.0.2/setup.cfg`

 * *Files identical despite different names*

