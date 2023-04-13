# Comparing `tmp/grafana-api-sdk-0.0.9.tar.gz` & `tmp/grafana-api-sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana-api-sdk-0.0.9.tar", last modified: Mon Mar  6 08:26:54 2023, max compression
+gzip compressed data, was "grafana-api-sdk-0.1.0.tar", last modified: Thu Apr 13 22:24:54 2023, max compression
```

## Comparing `grafana-api-sdk-0.0.9.tar` & `grafana-api-sdk-0.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 08:26:54.508985 grafana-api-sdk-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-03-06 08:26:54.508985 grafana-api-sdk-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 08:26:54.508985 grafana-api-sdk-0.0.9/grafana_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    41670 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/alerting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/alerting_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    32117 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/alerting_provisioning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/correlations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22349 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    21121 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/external_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/legacy_alerting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/legacy_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/licensing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25416 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/organisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/other_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/query_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/rbac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/short_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/grafana_api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 08:26:54.508985 grafana-api-sdk-0.0.9/grafana_api_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-03-06 08:26:54.000000 grafana-api-sdk-0.0.9/grafana_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-06 08:26:54.000000 grafana-api-sdk-0.0.9/grafana_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 08:26:54.000000 grafana-api-sdk-0.0.9/grafana_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-06 08:26:54.000000 grafana-api-sdk-0.0.9/grafana_api_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-06 08:26:54.000000 grafana-api-sdk-0.0.9/grafana_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 08:26:54.508985 grafana-api-sdk-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-06 08:26:22.000000 grafana-api-sdk-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:54.854884 grafana-api-sdk-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-04-13 22:24:54.854884 grafana-api-sdk-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:54.854884 grafana-api-sdk-0.1.0/grafana_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41670 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/alerting_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32117 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/alerting_provisioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22349 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21121 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/external_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/legacy_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/legacy_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/licensing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/organisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/other_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/query_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/short_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:54.854884 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-04-13 22:24:54.000000 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-13 22:24:54.000000 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:24:54.000000 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 22:24:54.000000 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 22:24:54.000000 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:24:54.854884 grafana-api-sdk-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/setup.py
```

### Comparing `grafana-api-sdk-0.0.9/LICENSE` & `grafana-api-sdk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/PKG-INFO` & `grafana-api-sdk-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-api-sdk
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Grafana API SDK
 Home-page: https://github.com/ZPascal/grafana_api_sdk
 Author: Pascal Zimmermann
 Author-email: info@theiotstudio.com
 Project-URL: Source, https://github.com/ZPascal/grafana_api_sdk
 Project-URL: Bug Tracker, https://github.com/ZPascal/grafana_api_sdk/issues
 Project-URL: Documentation, https://zpascal.github.io/grafana_api_sdk/
```

### Comparing `grafana-api-sdk-0.0.9/README.md` & `grafana-api-sdk-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/admin.py` & `grafana-api-sdk-0.1.0/grafana_api/admin.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/alerting.py` & `grafana-api-sdk-0.1.0/grafana_api/alerting.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/alerting_notifications.py` & `grafana-api-sdk-0.1.0/grafana_api/alerting_notifications.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/alerting_provisioning.py` & `grafana-api-sdk-0.1.0/grafana_api/alerting_provisioning.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/annotations.py` & `grafana-api-sdk-0.1.0/grafana_api/annotations.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/api.py` & `grafana-api-sdk-0.1.0/grafana_api/api.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/authentication.py` & `grafana-api-sdk-0.1.0/grafana_api/authentication.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/correlations.py` & `grafana-api-sdk-0.1.0/grafana_api/correlations.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/dashboard.py` & `grafana-api-sdk-0.1.0/grafana_api/dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/datasource.py` & `grafana-api-sdk-0.1.0/grafana_api/datasource.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/external_group.py` & `grafana-api-sdk-0.1.0/grafana_api/external_group.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/folder.py` & `grafana-api-sdk-0.1.0/grafana_api/folder.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/legacy_alerting.py` & `grafana-api-sdk-0.1.0/grafana_api/legacy_alerting.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/legacy_playlist.py` & `grafana-api-sdk-0.1.0/grafana_api/legacy_playlist.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/library.py` & `grafana-api-sdk-0.1.0/grafana_api/library.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/licensing.py` & `grafana-api-sdk-0.1.0/grafana_api/licensing.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/model.py` & `grafana-api-sdk-0.1.0/grafana_api/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from enum import Enum
 from typing import List, TypeVar
 from dataclasses import dataclass, field
 
 Self = TypeVar("Self", bound="Route")
 
 # The constant includes all necessary error messages that can occurs, if you establish a connection to the Grafana API.
-ERROR_MESSAGES: list = ["invalid API key"]
+ERROR_MESSAGES: list = ["invalid API key", "Expired API key"]
 
 
 class APIEndpoints(Enum):
     """The class includes all necessary API endpoint strings to connect the Grafana API"""
 
     api_prefix: str = "/api"
     version_1: str = "v1"
```

### Comparing `grafana-api-sdk-0.0.9/grafana_api/organisation.py` & `grafana-api-sdk-0.1.0/grafana_api/organisation.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/other_http.py` & `grafana-api-sdk-0.1.0/grafana_api/other_http.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/playlist.py` & `grafana-api-sdk-0.1.0/grafana_api/playlist.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/preferences.py` & `grafana-api-sdk-0.1.0/grafana_api/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/query_history.py` & `grafana-api-sdk-0.1.0/grafana_api/query_history.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/rbac.py` & `grafana-api-sdk-0.1.0/grafana_api/rbac.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/reporting.py` & `grafana-api-sdk-0.1.0/grafana_api/reporting.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/search.py` & `grafana-api-sdk-0.1.0/grafana_api/search.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/service_account.py` & `grafana-api-sdk-0.1.0/grafana_api/service_account.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/short_url.py` & `grafana-api-sdk-0.1.0/grafana_api/short_url.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/snapshot.py` & `grafana-api-sdk-0.1.0/grafana_api/snapshot.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/team.py` & `grafana-api-sdk-0.1.0/grafana_api/team.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api/user.py` & `grafana-api-sdk-0.1.0/grafana_api/user.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/grafana_api_sdk.egg-info/PKG-INFO` & `grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-api-sdk
-Version: 0.0.9
+Version: 0.1.0
 Summary: A Grafana API SDK
 Home-page: https://github.com/ZPascal/grafana_api_sdk
 Author: Pascal Zimmermann
 Author-email: info@theiotstudio.com
 Project-URL: Source, https://github.com/ZPascal/grafana_api_sdk
 Project-URL: Bug Tracker, https://github.com/ZPascal/grafana_api_sdk/issues
 Project-URL: Documentation, https://zpascal.github.io/grafana_api_sdk/
```

### Comparing `grafana-api-sdk-0.0.9/grafana_api_sdk.egg-info/SOURCES.txt` & `grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.0.9/setup.py` & `grafana-api-sdk-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     coverage_string: str = "![Coverage report](https://github.com/ZPascal/grafana_api_sdk/blob/main/docs/coverage.svg)"
     long_description: str = fh.read()
 
 long_description = long_description.replace(coverage_string, "")
 
 setuptools.setup(
     name="grafana-api-sdk",
-    version="0.0.9",
+    version="0.1.0",
     author="Pascal Zimmermann",
     author_email="info@theiotstudio.com",
     description="A Grafana API SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ZPascal/grafana_api_sdk",
     project_urls={
```

