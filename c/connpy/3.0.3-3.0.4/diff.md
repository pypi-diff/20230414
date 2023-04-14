# Comparing `tmp/connpy-3.0.3.tar.gz` & `tmp/connpy-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.0.3.tar", last modified: Fri Apr 14 16:42:05 2023, max compression
+gzip compressed data, was "connpy-3.0.4.tar", last modified: Fri Apr 14 16:47:02 2023, max compression
```

## Comparing `connpy-3.0.3.tar` & `connpy-3.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:42:05.418097 connpy-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 16:41:53.000000 connpy-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 16:42:05.418097 connpy-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-14 16:41:53.000000 connpy-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:42:05.414097 connpy-3.0.3/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-14 16:41:53.000000 connpy-3.0.3/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 16:41:53.000000 connpy-3.0.3/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:41:53.000000 connpy-3.0.3/connpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-14 16:41:53.000000 connpy-3.0.3/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-14 16:41:53.000000 connpy-3.0.3/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-14 16:41:53.000000 connpy-3.0.3/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47147 2023-04-14 16:41:53.000000 connpy-3.0.3/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27912 2023-04-14 16:41:53.000000 connpy-3.0.3/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:42:05.418097 connpy-3.0.3/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 16:42:05.000000 connpy-3.0.3/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 16:42:05.000000 connpy-3.0.3/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:42:05.000000 connpy-3.0.3/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 16:42:05.000000 connpy-3.0.3/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 16:42:05.000000 connpy-3.0.3/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 16:42:05.000000 connpy-3.0.3/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 16:42:05.418097 connpy-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 16:41:53.000000 connpy-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:02.919291 connpy-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 16:46:53.000000 connpy-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 16:47:02.919291 connpy-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-14 16:46:53.000000 connpy-3.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:02.919291 connpy-3.0.4/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47147 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27912 2023-04-14 16:46:53.000000 connpy-3.0.4/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:47:02.919291 connpy-3.0.4/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 16:47:02.000000 connpy-3.0.4/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-14 16:47:02.919291 connpy-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 16:46:53.000000 connpy-3.0.4/setup.py
```

### Comparing `connpy-3.0.3/LICENSE` & `connpy-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.0.3/PKG-INFO` & `connpy-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.0.3
+Version: 3.0.4
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.0.3/README.md` & `connpy-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.0.3/connpy/__init__.py` & `connpy-3.0.4/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.3/connpy/api.py` & `connpy-3.0.4/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.3/connpy/completion.py` & `connpy-3.0.4/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.3/connpy/configfile.py` & `connpy-3.0.4/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.3/connpy/connapp.py` & `connpy-3.0.4/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.3/connpy/core.py` & `connpy-3.0.4/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.3/connpy.egg-info/PKG-INFO` & `connpy-3.0.4/connpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.0.3
+Version: 3.0.4
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.0.3/setup.cfg` & `connpy-3.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 packages = find:
 install_requires = 
 	inquirer
 	pexpect
 	pycryptodome
 	Flask
 	waitress
+	PyYAML
 
 [options.extras_require]
 fuzzysearch = pyfzf
 
 [options.entry_points]
 console_scripts = 
 	conn = connpy.__main__:main
```

