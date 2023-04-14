# Comparing `tmp/visier-connector-0.9.2.tar.gz` & `tmp/visier-connector-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visier-connector-0.9.2.tar", last modified: Fri Apr 14 16:57:05 2023, max compression
+gzip compressed data, was "visier-connector-0.9.3.tar", last modified: Fri Apr 14 17:29:26 2023, max compression
```

## Comparing `visier-connector-0.9.2.tar` & `visier-connector-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:57:05.321121 visier-connector-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 16:56:56.000000 visier-connector-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 16:57:05.321121 visier-connector-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-14 16:56:56.000000 visier-connector-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:57:05.317121 visier-connector-0.9.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-14 16:56:56.000000 visier-connector-0.9.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-14 16:56:56.000000 visier-connector-0.9.2/examples/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:57:05.321121 visier-connector-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 16:56:56.000000 visier-connector-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:57:05.317121 visier-connector-0.9.2/visier/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-14 16:56:56.000000 visier-connector-0.9.2/visier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:57:05.317121 visier-connector-0.9.2/visier/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 16:56:56.000000 visier-connector-0.9.2/visier/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-14 16:56:56.000000 visier-connector-0.9.2/visier/connector/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-14 16:56:56.000000 visier-connector-0.9.2/visier/connector/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:57:05.317121 visier-connector-0.9.2/visier_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 16:57:05.000000 visier-connector-0.9.2/visier_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 16:57:05.000000 visier-connector-0.9.2/visier_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:57:05.000000 visier-connector-0.9.2/visier_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 16:57:05.000000 visier-connector-0.9.2/visier_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 16:57:05.000000 visier-connector-0.9.2/visier_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:29:26.989873 visier-connector-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 17:29:15.000000 visier-connector-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 17:29:26.989873 visier-connector-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-14 17:29:15.000000 visier-connector-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:29:26.985873 visier-connector-0.9.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-14 17:29:15.000000 visier-connector-0.9.3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-14 17:29:15.000000 visier-connector-0.9.3/examples/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:29:26.989873 visier-connector-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 17:29:15.000000 visier-connector-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:29:26.985873 visier-connector-0.9.3/visier/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-14 17:29:15.000000 visier-connector-0.9.3/visier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:29:26.985873 visier-connector-0.9.3/visier/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 17:29:15.000000 visier-connector-0.9.3/visier/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-14 17:29:15.000000 visier-connector-0.9.3/visier/connector/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-14 17:29:15.000000 visier-connector-0.9.3/visier/connector/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:29:26.985873 visier-connector-0.9.3/visier_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 17:29:26.000000 visier-connector-0.9.3/visier_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 17:29:26.000000 visier-connector-0.9.3/visier_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:29:26.000000 visier-connector-0.9.3/visier_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 17:29:26.000000 visier-connector-0.9.3/visier_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 17:29:26.000000 visier-connector-0.9.3/visier_connector.egg-info/top_level.txt
```

### Comparing `visier-connector-0.9.2/LICENSE` & `visier-connector-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.2/PKG-INFO` & `visier-connector-0.9.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.2
+Version: 0.9.3
 Summary: Visier People Data connector through the Visier SQL-like API
 Home-page: 
 Author: Visier Research & Development
 Author-email: info@visier.com
 License: Apache License, Version 2.0
 Keywords: Visier Public Platform APIs,Visier SQL-like
 Requires-Python: >=3.7
```

### Comparing `visier-connector-0.9.2/README.md` & `visier-connector-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.2/examples/__init__.py` & `visier-connector-0.9.3/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.2/examples/util.py` & `visier-connector-0.9.3/examples/util.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.2/setup.py` & `visier-connector-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.2/visier/__init__.py` & `visier-connector-0.9.3/visier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Public Python Connector
 """
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
```

### Comparing `visier-connector-0.9.2/visier/connector/__init__.py` & `visier-connector-0.9.3/visier/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.2/visier/connector/authentication.py` & `visier-connector-0.9.3/visier/connector/authentication.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.2/visier/connector/sessions.py` & `visier-connector-0.9.3/visier/connector/sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Session object through which JSON as well as SQL-like queries are executed.
 """
 
-import os
 import json
 import dataclasses
 from typing import Callable
 import requests
 from requests import Session, Response
 from visier.connector.authentication import Authentication
 
@@ -143,16 +142,14 @@
         body = {'username': self._auth.username, 'password': self._auth.password}
         if self._auth.vanity:
             body["vanityName"] = self._auth.vanity
         result = requests.post(url=url, data=body, timeout=30)
         result.raise_for_status()
 
         # Only create a requests.Session once we have a Visier ASID Token
-        # asid_token = result.text
-        print("DEBUG: actual token disregarded. Use expired DSC D3M token instead.")
-        asid_token = os.getenv("DEBUG_TOKEN")
+        asid_token = result.text
         self._session = Session()
         self._session.cookies["VisierASIDToken"] = asid_token
         self._session.headers.update({"apikey": self._auth.api_key})
 
     def _close(self):
         self._session.close()
```

### Comparing `visier-connector-0.9.2/visier_connector.egg-info/PKG-INFO` & `visier-connector-0.9.3/visier_connector.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.2
+Version: 0.9.3
 Summary: Visier People Data connector through the Visier SQL-like API
 Home-page: 
 Author: Visier Research & Development
 Author-email: info@visier.com
 License: Apache License, Version 2.0
 Keywords: Visier Public Platform APIs,Visier SQL-like
 Requires-Python: >=3.7
```

