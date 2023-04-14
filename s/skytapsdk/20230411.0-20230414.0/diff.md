# Comparing `tmp/skytapsdk-20230411.0.tar.gz` & `tmp/skytapsdk-20230414.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytapsdk-20230411.0.tar", last modified: Tue Apr 11 14:14:39 2023, max compression
+gzip compressed data, was "skytapsdk-20230414.0.tar", last modified: Fri Apr 14 16:29:59 2023, max compression
```

## Comparing `skytapsdk-20230411.0.tar` & `skytapsdk-20230414.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-11 14:14:39.908495 skytapsdk-20230411.0/
--rw-r--r--   0 dmickelson   (503) staff       (20)     1500 2022-12-05 15:16:30.000000 skytapsdk-20230411.0/LICENSE.md
--rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-04-11 14:14:39.908558 skytapsdk-20230411.0/PKG-INFO
--rw-r--r--   0 dmickelson   (503) staff       (20)       91 2023-04-11 14:14:39.908757 skytapsdk-20230411.0/setup.cfg
--rw-r--r--   0 dmickelson   (503) staff       (20)     1389 2023-04-11 14:11:52.000000 skytapsdk-20230411.0/setup.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-11 14:14:39.907018 skytapsdk-20230411.0/skytapsdk/
--rw-r--r--   0 dmickelson   (503) staff       (20)      102 2023-02-07 14:36:46.000000 skytapsdk-20230411.0/skytapsdk/__init__.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-11 14:14:39.908382 skytapsdk-20230411.0/skytapsdk/api_endpoints/
--rw-r--r--   0 dmickelson   (503) staff       (20)        0 2023-02-07 14:36:46.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/__init__.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1068 2023-02-07 14:36:46.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/assets.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1141 2023-02-07 14:36:46.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/environments.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1609 2023-04-10 15:37:33.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/projects.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1138 2023-04-10 15:37:33.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/reports.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1102 2023-02-07 14:36:46.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/templates.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1316 2023-04-11 14:12:27.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/users.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1481 2023-02-07 15:11:48.000000 skytapsdk-20230411.0/skytapsdk/helpers.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     3286 2023-04-10 15:37:33.000000 skytapsdk-20230411.0/skytapsdk/skytap.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-11 14:14:39.907609 skytapsdk-20230411.0/skytapsdk.egg-info/
--rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-04-11 14:14:39.000000 skytapsdk-20230411.0/skytapsdk.egg-info/PKG-INFO
--rw-r--r--   0 dmickelson   (503) staff       (20)      507 2023-04-11 14:14:39.000000 skytapsdk-20230411.0/skytapsdk.egg-info/SOURCES.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)        1 2023-04-11 14:14:39.000000 skytapsdk-20230411.0/skytapsdk.egg-info/dependency_links.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)        8 2023-04-11 14:14:39.000000 skytapsdk-20230411.0/skytapsdk.egg-info/requires.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)       10 2023-04-11 14:14:39.000000 skytapsdk-20230411.0/skytapsdk.egg-info/top_level.txt
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-14 16:29:59.835550 skytapsdk-20230414.0/
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1500 2022-12-05 15:16:30.000000 skytapsdk-20230414.0/LICENSE.md
+-rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-04-14 16:29:59.835615 skytapsdk-20230414.0/PKG-INFO
+-rw-r--r--   0 dmickelson   (503) staff       (20)       91 2023-04-14 16:29:59.835822 skytapsdk-20230414.0/setup.cfg
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1389 2023-04-14 16:28:55.000000 skytapsdk-20230414.0/setup.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-14 16:29:59.833889 skytapsdk-20230414.0/skytapsdk/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      165 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/__init__.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1334 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/course_manager.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-14 16:29:59.834722 skytapsdk-20230414.0/skytapsdk/course_manager_endpoints/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      116 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/course_manager_endpoints/__init__.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1277 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/course_manager_endpoints/events.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      374 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/course_manager_endpoints/self_learners.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1481 2023-02-07 15:11:48.000000 skytapsdk-20230414.0/skytapsdk/helpers.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     3204 2023-04-14 16:29:25.000000 skytapsdk-20230414.0/skytapsdk/skytap.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-14 16:29:59.835457 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      294 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/__init__.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1068 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/assets.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1141 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/environments.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1609 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/projects.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1138 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/reports.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1102 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/templates.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1316 2023-04-14 16:28:41.000000 skytapsdk-20230414.0/skytapsdk/skytap_endpoints/users.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-14 16:29:59.834409 skytapsdk-20230414.0/skytapsdk.egg-info/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-04-14 16:29:59.000000 skytapsdk-20230414.0/skytapsdk.egg-info/PKG-INFO
+-rw-r--r--   0 dmickelson   (503) staff       (20)      700 2023-04-14 16:29:59.000000 skytapsdk-20230414.0/skytapsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)        1 2023-04-14 16:29:59.000000 skytapsdk-20230414.0/skytapsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)        8 2023-04-14 16:29:59.000000 skytapsdk-20230414.0/skytapsdk.egg-info/requires.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)       10 2023-04-14 16:29:59.000000 skytapsdk-20230414.0/skytapsdk.egg-info/top_level.txt
```

### Comparing `skytapsdk-20230411.0/LICENSE.md` & `skytapsdk-20230414.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230411.0/PKG-INFO` & `skytapsdk-20230414.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytapsdk
-Version: 20230411.0
+Version: 20230414.0
 Summary: SDK for interacting with Skytap's APIs.
 Home-page: 
 Author: Dax Mickelson
 Author-email: dmickelson@zscaler.com
 License: BSD
 Keywords: skytap
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `skytapsdk-20230411.0/setup.py` & `skytapsdk-20230414.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version = "20230411.0"
+__version = "20230414.0"
 __author = "Dax Mickelson"
 __author_email = "dmickelson@zscaler.com"
 __license = "BSD"
 __name = "skytapsdk"
 __description = "SDK for interacting with Skytap's APIs."
 __long_description = __description
 __url = ""
```

### Comparing `skytapsdk-20230411.0/skytapsdk/api_endpoints/assets.py` & `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230411.0/skytapsdk/api_endpoints/environments.py` & `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230411.0/skytapsdk/api_endpoints/projects.py` & `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/projects.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230411.0/skytapsdk/api_endpoints/reports.py` & `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/reports.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230411.0/skytapsdk/api_endpoints/templates.py` & `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/templates.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230411.0/skytapsdk/api_endpoints/users.py` & `skytapsdk-20230414.0/skytapsdk/skytap_endpoints/users.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230411.0/skytapsdk/helpers.py` & `skytapsdk-20230414.0/skytapsdk/helpers.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230411.0/skytapsdk/skytap.py` & `skytapsdk-20230414.0/skytapsdk/skytap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import logging
 
 from restfly.session import APISession
 
-from skytapsdk.api_endpoints.assets import Assets
-from skytapsdk.api_endpoints.environments import Environments
-from skytapsdk.api_endpoints.projects import Projects
-from skytapsdk.api_endpoints.reports import Reports
-from skytapsdk.api_endpoints.templates import Templates
-from skytapsdk.api_endpoints.users import Users
+from .skytap_endpoints import (Assets, Environments, Projects, Reports,
+                               Templates, Users)
 
 
 class Skytap(APISession):
     """A controller to access Endpoints in the Skytap API."""
 
     BASE_URL = "https://cloud.skytap.com"
     API_VERSION = 1
@@ -38,28 +34,35 @@
         self._password = password
         self._token = token
         self._api_version = self.API_VERSION
         self._url = self.BASE_URL
 
         # Use setter to update the self._api_version AND rewrite the self._url.
         self.api_version = kwargs.get("api_version", self.API_VERSION)
+
         super(Skytap, self).__init__(
             username=self._username,
             password=self._password,
             token=self._token,
             **kwargs,
         )
         self.login()
 
     def login(self):
         if self._username:
             if self._token:
-                self._session.auth = (self._username, self._token)
+                self._session.auth = (
+                    self._username,
+                    self._token,
+                )
             elif self._password:
-                self._session.auth = (self._username, self._password)
+                self._session.auth = (
+                    self._username,
+                    self._password,
+                )
             else:
                 logging.warning("Token or Password is required for authentication.")
         self._session.headers.update(
             {
                 "Accept": "application/json",
                 "Content-Type": "application/json",
             }
```

### Comparing `skytapsdk-20230411.0/skytapsdk.egg-info/PKG-INFO` & `skytapsdk-20230414.0/skytapsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytapsdk
-Version: 20230411.0
+Version: 20230414.0
 Summary: SDK for interacting with Skytap's APIs.
 Home-page: 
 Author: Dax Mickelson
 Author-email: dmickelson@zscaler.com
 License: BSD
 Keywords: skytap
 Classifier: Development Status :: 5 - Production/Stable
```

