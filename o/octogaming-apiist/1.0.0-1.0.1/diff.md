# Comparing `tmp/octogaming-apiist-1.0.0.tar.gz` & `tmp/octogaming-apiist-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octogaming-apiist-1.0.0.tar", last modified: Sun Jan 29 12:05:51 2023, max compression
+gzip compressed data, was "octogaming-apiist-1.0.1.tar", last modified: Fri Apr 14 07:13:24 2023, max compression
```

## Comparing `octogaming-apiist-1.0.0.tar` & `octogaming-apiist-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-29 12:05:51.249658 octogaming-apiist-1.0.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11357 2023-01-27 20:29:10.000000 octogaming-apiist-1.0.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12456 2023-01-29 12:05:51.249658 octogaming-apiist-1.0.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12090 2023-01-29 11:44:31.000000 octogaming-apiist-1.0.0/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-29 12:05:51.249658 octogaming-apiist-1.0.0/apiist/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1685 2023-01-27 22:43:32.000000 octogaming-apiist-1.0.0/apiist/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       66 2023-01-27 22:41:42.000000 octogaming-apiist-1.0.0/apiist/__main__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1874 2023-01-27 22:47:05.000000 octogaming-apiist-1.0.0/apiist/action_plugins.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4835 2023-01-27 22:54:48.000000 octogaming-apiist-1.0.0/apiist/csv.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    37412 2023-01-29 11:28:40.000000 octogaming-apiist-1.0.0/apiist/http.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19228 2023-01-27 22:57:24.000000 octogaming-apiist-1.0.0/apiist/loadgen.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3880 2023-01-27 22:56:14.000000 octogaming-apiist-1.0.0/apiist/pytest_plugin.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12558 2023-01-27 22:57:24.000000 octogaming-apiist-1.0.0/apiist/samples.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4187 2023-01-27 22:41:42.000000 octogaming-apiist-1.0.0/apiist/ssl_adapter.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3978 2023-01-27 22:57:24.000000 octogaming-apiist-1.0.0/apiist/store.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2819 2023-01-27 22:41:42.000000 octogaming-apiist-1.0.0/apiist/thread.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3640 2023-01-27 22:14:05.000000 octogaming-apiist-1.0.0/apiist/utilities.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2495 2023-01-27 22:57:24.000000 octogaming-apiist-1.0.0/apiist/utils.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-01-29 12:05:51.249658 octogaming-apiist-1.0.0/octogaming_apiist.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12456 2023-01-29 12:05:51.000000 octogaming-apiist-1.0.0/octogaming_apiist.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      542 2023-01-29 12:05:51.000000 octogaming-apiist-1.0.0/octogaming_apiist.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-01-29 12:05:51.000000 octogaming-apiist-1.0.0/octogaming_apiist.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       48 2023-01-29 12:05:51.000000 octogaming-apiist-1.0.0/octogaming_apiist.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       96 2023-01-29 12:05:51.000000 octogaming-apiist-1.0.0/octogaming_apiist.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        7 2023-01-29 12:05:51.000000 octogaming-apiist-1.0.0/octogaming_apiist.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-01-27 22:41:33.000000 octogaming-apiist-1.0.0/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      197 2023-01-29 12:05:51.253658 octogaming-apiist-1.0.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1449 2023-01-29 12:05:09.000000 octogaming-apiist-1.0.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-14 07:13:24.719140 octogaming-apiist-1.0.1/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11357 2023-01-27 20:29:10.000000 octogaming-apiist-1.0.1/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12632 2023-04-14 07:13:24.719140 octogaming-apiist-1.0.1/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12266 2023-01-29 12:09:52.000000 octogaming-apiist-1.0.1/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-14 07:13:24.719140 octogaming-apiist-1.0.1/apiist/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1685 2023-01-27 22:43:32.000000 octogaming-apiist-1.0.1/apiist/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       66 2023-01-27 22:41:42.000000 octogaming-apiist-1.0.1/apiist/__main__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1874 2023-01-27 22:47:05.000000 octogaming-apiist-1.0.1/apiist/action_plugins.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4835 2023-01-27 22:54:48.000000 octogaming-apiist-1.0.1/apiist/csv.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    37412 2023-01-29 11:28:40.000000 octogaming-apiist-1.0.1/apiist/http.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19228 2023-01-27 22:57:24.000000 octogaming-apiist-1.0.1/apiist/loadgen.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3880 2023-01-27 22:56:14.000000 octogaming-apiist-1.0.1/apiist/pytest_plugin.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12558 2023-01-27 22:57:24.000000 octogaming-apiist-1.0.1/apiist/samples.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4187 2023-01-27 22:41:42.000000 octogaming-apiist-1.0.1/apiist/ssl_adapter.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3978 2023-01-27 22:57:24.000000 octogaming-apiist-1.0.1/apiist/store.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2819 2023-01-27 22:41:42.000000 octogaming-apiist-1.0.1/apiist/thread.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3640 2023-01-27 22:14:05.000000 octogaming-apiist-1.0.1/apiist/utilities.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2495 2023-04-12 19:45:48.000000 octogaming-apiist-1.0.1/apiist/utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-14 07:13:24.719140 octogaming-apiist-1.0.1/octogaming_apiist.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12632 2023-04-14 07:13:24.000000 octogaming-apiist-1.0.1/octogaming_apiist.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      542 2023-04-14 07:13:24.000000 octogaming-apiist-1.0.1/octogaming_apiist.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-14 07:13:24.000000 octogaming-apiist-1.0.1/octogaming_apiist.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       48 2023-04-14 07:13:24.000000 octogaming-apiist-1.0.1/octogaming_apiist.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       88 2023-04-14 07:13:24.000000 octogaming-apiist-1.0.1/octogaming_apiist.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        7 2023-04-14 07:13:24.000000 octogaming-apiist-1.0.1/octogaming_apiist.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-01-27 22:41:33.000000 octogaming-apiist-1.0.1/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      197 2023-04-14 07:13:24.719140 octogaming-apiist-1.0.1/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1449 2023-01-29 12:05:09.000000 octogaming-apiist-1.0.1/setup.py
```

### Comparing `octogaming-apiist-1.0.0/LICENSE` & `octogaming-apiist-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/PKG-INFO` & `octogaming-apiist-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: octogaming-apiist
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python framework for API testing
 Home-page: https://github.com/BetOnYou/apiist
 Download-URL: https://github.com/BetOnYou/apiist
 Author: Titouan FREVILLE
 Author-email: titouan@bet-on-you.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: pytest
 License-File: LICENSE
 
 # Apiist
 
-[![build](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml/badge.svg)](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml)[![Coverage Status](https://coveralls.io/repos/github/BetOnYou/apiist/badge.svg?branch=main)](https://coveralls.io/github/BetOnYou/apiist?branch=main)
+[![build](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml/badge.svg)](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml)[![Coverage Status](https://coveralls.io/repos/github/BetOnYou/apiist/badge.svg?branch=main)](https://coveralls.io/github/BetOnYou/apiist?branch=main)[![PyPI version](https://badge.fury.io/py/octogaming-apiist.svg)](https://badge.fury.io/py/octogaming-apiist)
 
 Apiist is an [Apiritif forks](https://github.com/Blazemeter/apiritif). It also aims to simplify python api testing with a set of
 predefined assertions and request methods. The fork was motivated by the project lacks of apparence maintenance and the need to
 support testing using Async methods and Starlette test client related to a FastAPI usage.
 
+Install Apiist:
+
+```
+pip install octogaming-apiist
+```
+
 Check Apiist version with the following command:
 
 ```
-python -m apiist -- version
+python -m octogaming-apiist -- version
 ```
 
 Here described some features of Apiist which can help you to create tests more easily.
 
 ## Overview
 
 ## HTTP Requests
```

### Comparing `octogaming-apiist-1.0.0/README.md` & `octogaming-apiist-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # Apiist
 
-[![build](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml/badge.svg)](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml)[![Coverage Status](https://coveralls.io/repos/github/BetOnYou/apiist/badge.svg?branch=main)](https://coveralls.io/github/BetOnYou/apiist?branch=main)
+[![build](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml/badge.svg)](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml)[![Coverage Status](https://coveralls.io/repos/github/BetOnYou/apiist/badge.svg?branch=main)](https://coveralls.io/github/BetOnYou/apiist?branch=main)[![PyPI version](https://badge.fury.io/py/octogaming-apiist.svg)](https://badge.fury.io/py/octogaming-apiist)
 
 Apiist is an [Apiritif forks](https://github.com/Blazemeter/apiritif). It also aims to simplify python api testing with a set of
 predefined assertions and request methods. The fork was motivated by the project lacks of apparence maintenance and the need to
 support testing using Async methods and Starlette test client related to a FastAPI usage.
 
+Install Apiist:
+
+```
+pip install octogaming-apiist
+```
+
 Check Apiist version with the following command:
 
 ```
-python -m apiist -- version
+python -m octogaming-apiist -- version
 ```
 
 Here described some features of Apiist which can help you to create tests more easily.
 
 ## Overview
 
 ## HTTP Requests
```

### Comparing `octogaming-apiist-1.0.0/apiist/__init__.py` & `octogaming-apiist-1.0.1/apiist/__init__.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/action_plugins.py` & `octogaming-apiist-1.0.1/apiist/action_plugins.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/csv.py` & `octogaming-apiist-1.0.1/apiist/csv.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/http.py` & `octogaming-apiist-1.0.1/apiist/http.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/loadgen.py` & `octogaming-apiist-1.0.1/apiist/loadgen.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/pytest_plugin.py` & `octogaming-apiist-1.0.1/apiist/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/samples.py` & `octogaming-apiist-1.0.1/apiist/samples.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/ssl_adapter.py` & `octogaming-apiist-1.0.1/apiist/ssl_adapter.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/store.py` & `octogaming-apiist-1.0.1/apiist/store.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/thread.py` & `octogaming-apiist-1.0.1/apiist/thread.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/utilities.py` & `octogaming-apiist-1.0.1/apiist/utilities.py`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/apiist/utils.py` & `octogaming-apiist-1.0.1/apiist/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 import logging
 import os
 import re
 import sys
 import traceback
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 log = logging.getLogger("apiist")
 
 
 def get_trace(error):
     if sys.version > "3":
         # noinspection PyArgumentList
```

### Comparing `octogaming-apiist-1.0.0/octogaming_apiist.egg-info/PKG-INFO` & `octogaming-apiist-1.0.1/octogaming_apiist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: octogaming-apiist
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python framework for API testing
 Home-page: https://github.com/BetOnYou/apiist
 Download-URL: https://github.com/BetOnYou/apiist
 Author: Titouan FREVILLE
 Author-email: titouan@bet-on-you.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: pytest
 License-File: LICENSE
 
 # Apiist
 
-[![build](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml/badge.svg)](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml)[![Coverage Status](https://coveralls.io/repos/github/BetOnYou/apiist/badge.svg?branch=main)](https://coveralls.io/github/BetOnYou/apiist?branch=main)
+[![build](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml/badge.svg)](https://github.com/BetOnYou/apiist/actions/workflows/branches.yaml)[![Coverage Status](https://coveralls.io/repos/github/BetOnYou/apiist/badge.svg?branch=main)](https://coveralls.io/github/BetOnYou/apiist?branch=main)[![PyPI version](https://badge.fury.io/py/octogaming-apiist.svg)](https://badge.fury.io/py/octogaming-apiist)
 
 Apiist is an [Apiritif forks](https://github.com/Blazemeter/apiritif). It also aims to simplify python api testing with a set of
 predefined assertions and request methods. The fork was motivated by the project lacks of apparence maintenance and the need to
 support testing using Async methods and Starlette test client related to a FastAPI usage.
 
+Install Apiist:
+
+```
+pip install octogaming-apiist
+```
+
 Check Apiist version with the following command:
 
 ```
-python -m apiist -- version
+python -m octogaming-apiist -- version
 ```
 
 Here described some features of Apiist which can help you to create tests more easily.
 
 ## Overview
 
 ## HTTP Requests
```

### Comparing `octogaming-apiist-1.0.0/octogaming_apiist.egg-info/SOURCES.txt` & `octogaming-apiist-1.0.1/octogaming_apiist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octogaming-apiist-1.0.0/setup.py` & `octogaming-apiist-1.0.1/setup.py`

 * *Files identical despite different names*

