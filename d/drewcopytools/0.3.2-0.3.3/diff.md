# Comparing `tmp/drewcopytools-0.3.2.tar.gz` & `tmp/drewcopytools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drewcopytools-0.3.2.tar", max compression
+gzip compressed data, was "drewcopytools-0.3.3.tar", max compression
```

## Comparing `drewcopytools-0.3.2.tar` & `drewcopytools-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2021-11-04 13:41:12.398121 drewcopytools-0.3.2/drewcopytools/__init__.py
--rw-r--r--   0        0        0     1686 2023-02-05 20:27:11.386651 drewcopytools-0.3.2/drewcopytools/datetimetools.py
--rw-r--r--   0        0        0     3183 2023-03-16 19:03:43.335431 drewcopytools-0.3.2/drewcopytools/filetools.py
--rw-r--r--   0        0        0     2143 2023-03-17 23:37:25.736171 drewcopytools-0.3.2/drewcopytools/jsontools.py
--rw-r--r--   0        0        0     2605 2023-02-11 00:37:24.958994 drewcopytools-0.3.2/drewcopytools/logtools.py
--rw-r--r--   0        0        0     2215 2023-04-14 00:48:13.591832 drewcopytools-0.3.2/drewcopytools/tools.py
--rw-r--r--   0        0        0     1097 2023-02-03 17:58:23.504109 drewcopytools-0.3.2/LICENSE
--rw-r--r--   0        0        0      488 2023-04-14 00:48:58.118385 drewcopytools-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      766 2023-04-14 00:50:02.615635 drewcopytools-0.3.2/setup.py
--rw-r--r--   0        0        0      523 2023-04-14 00:50:02.615635 drewcopytools-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2021-11-04 13:41:12.398121 drewcopytools-0.3.3/drewcopytools/__init__.py
+-rw-r--r--   0        0        0     1686 2023-02-05 20:27:11.386651 drewcopytools-0.3.3/drewcopytools/datetimetools.py
+-rw-r--r--   0        0        0     3183 2023-03-16 19:03:43.335431 drewcopytools-0.3.3/drewcopytools/filetools.py
+-rw-r--r--   0        0        0     2143 2023-03-17 23:37:25.736171 drewcopytools-0.3.3/drewcopytools/jsontools.py
+-rw-r--r--   0        0        0     2605 2023-02-11 00:37:24.958994 drewcopytools-0.3.3/drewcopytools/logtools.py
+-rw-r--r--   0        0        0     2232 2023-04-14 00:50:49.273081 drewcopytools-0.3.3/drewcopytools/tools.py
+-rw-r--r--   0        0        0     1097 2023-02-03 17:58:23.504109 drewcopytools-0.3.3/LICENSE
+-rw-r--r--   0        0        0      488 2023-04-14 00:50:56.159746 drewcopytools-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      766 2023-04-14 00:51:25.497682 drewcopytools-0.3.3/setup.py
+-rw-r--r--   0        0        0      523 2023-04-14 00:51:25.498679 drewcopytools-0.3.3/PKG-INFO
```

### Comparing `drewcopytools-0.3.2/drewcopytools/datetimetools.py` & `drewcopytools-0.3.3/drewcopytools/datetimetools.py`

 * *Files identical despite different names*

### Comparing `drewcopytools-0.3.2/drewcopytools/filetools.py` & `drewcopytools-0.3.3/drewcopytools/filetools.py`

 * *Files identical despite different names*

### Comparing `drewcopytools-0.3.2/drewcopytools/jsontools.py` & `drewcopytools-0.3.3/drewcopytools/jsontools.py`

 * *Files identical despite different names*

### Comparing `drewcopytools-0.3.2/drewcopytools/logtools.py` & `drewcopytools-0.3.3/drewcopytools/logtools.py`

 * *Files identical despite different names*

### Comparing `drewcopytools-0.3.2/drewcopytools/tools.py` & `drewcopytools-0.3.3/drewcopytools/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # General tool type functions.
 import subprocess
 import logging
+import logging
 
 # -----------------------------------------------------------------------------
 # Simple function to get the correct name of a program, depending on the current platform.
 # this will pretty much add/remove the .exe extension of a program name as needed depending if
 # you are on window/linux, etc.
 def translate_exe_name(exeName:str):
   from sys import platform
@@ -70,10 +71,10 @@
   logging.debug(f'CALL:{exe}')
 
   if isinstance(exe, str):
     exe = split_cmdline_args(exe)
 
   callres = subprocess.call(exe)
   if callres != 0:
-    logging.info("CALL FAILED!")
+    logging.debug("CALL FAILED!")
     return False
   return True
```

### Comparing `drewcopytools-0.3.2/LICENSE` & `drewcopytools-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drewcopytools-0.3.2/setup.py` & `drewcopytools-0.3.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pathlib>=1.0.1,<2.0.0', 'pytest>=6.2.5,<7.0.0']
 
 setup_kwargs = {
     'name': 'drewcopytools',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Utility code that I use in many of my python projects.  Most of these functions exist to make python work in a predicatble, cross-platform way.',
     'long_description': None,
     'author': 'Andrew Ritz',
     'author_email': 'andrew.a.ritz@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `drewcopytools-0.3.2/PKG-INFO` & `drewcopytools-0.3.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drewcopytools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Utility code that I use in many of my python projects.  Most of these functions exist to make python work in a predicatble, cross-platform way.
 Author: Andrew Ritz
 Author-email: andrew.a.ritz@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

