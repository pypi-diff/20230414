# Comparing `tmp/globus-compute-sdk-2.0.0a1.tar.gz` & `tmp/globus-compute-sdk-2.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.0.0a1.tar", last modified: Mon Apr  3 22:15:05 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.0.1a0.tar", last modified: Fri Apr 14 15:04:12 2023, max compression
```

## Comparing `globus-compute-sdk-2.0.0a1.tar` & `globus-compute-sdk-2.0.1a0.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.923487 globus-compute-sdk-2.0.0a1/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)      770 2023-04-03 22:15:05.923533 globus-compute-sdk-2.0.0a1/PKG-INFO
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.919263 globus-compute-sdk-2.0.0a1/globus_compute_sdk/
--rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.920152 globus-compute-sdk-2.0.0a1/globus_compute_sdk/errors/
--rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/errors/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/errors/error_types.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.921161 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      970 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/_environments.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.921628 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-r--r--   0 lei        (501) staff       (20)      723 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-r--r--   0 lei        (501) staff       (20)    11442 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
--rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/batch.py
--rw-r--r--   0 lei        (501) staff       (20)    27431 2023-04-03 17:23:22.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/client.py
--rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/container_spec.py
--rw-r--r--   0 lei        (501) staff       (20)    46343 2023-04-03 17:23:20.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/executor.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.922695 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/
--rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 lei        (501) staff       (20)     7544 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 lei        (501) staff       (20)      783 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 lei        (501) staff       (20)     2476 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/whoami.py
--rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/search.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.922924 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/utils/
--rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/utils/printing.py
--rw-r--r--   0 lei        (501) staff       (20)     8421 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/web_client.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.923385 globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      100 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1680 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/base.py
--rw-r--r--   0 lei        (501) staff       (20)     7511 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/concretes.py
--rw-r--r--   0 lei        (501) staff       (20)     3737 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/facade.py
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/utils.py
--rw-r--r--   0 lei        (501) staff       (20)      834 2023-04-03 22:12:27.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:05.919895 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)      770 2023-04-03 22:15:05.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1590 2023-04-03 22:15:05.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-03 22:15:05.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      379 2023-04-03 22:15:05.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       19 2023-04-03 22:15:05.000000 globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-03 22:15:05.923778 globus-compute-sdk-2.0.0a1/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     2691 2023-04-03 17:17:07.000000 globus-compute-sdk-2.0.0a1/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:12.251062 globus-compute-sdk-2.0.1a0/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)      770 2023-04-14 15:04:12.251126 globus-compute-sdk-2.0.1a0/PKG-INFO
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:12.244442 globus-compute-sdk-2.0.1a0/globus_compute_sdk/
+-rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:12.245303 globus-compute-sdk-2.0.1a0/globus_compute_sdk/errors/
+-rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/errors/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/errors/error_types.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:12.247471 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      970 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/_environments.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:12.248032 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/asynchronous/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-r--r--   0 lei        (501) staff       (20)    11442 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
+-rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/batch.py
+-rw-r--r--   0 lei        (501) staff       (20)    26362 2023-04-13 13:57:47.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/client.py
+-rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/container_spec.py
+-rw-r--r--   0 lei        (501) staff       (20)    46344 2023-04-14 15:02:34.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/executor.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:12.249928 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/
+-rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 lei        (501) staff       (20)     7287 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 lei        (501) staff       (20)     2887 2023-04-13 00:34:31.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/whoami.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:12.250231 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/utils/
+-rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/utils/printing.py
+-rw-r--r--   0 lei        (501) staff       (20)     8618 2023-04-13 13:57:47.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/web_client.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:12.250888 globus-compute-sdk-2.0.1a0/globus_compute_sdk/serialize/
+-rw-r--r--   0 lei        (501) staff       (20)      100 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/serialize/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1680 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/serialize/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     7511 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/serialize/concretes.py
+-rw-r--r--   0 lei        (501) staff       (20)     3737 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/serialize/facade.py
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/utils.py
+-rw-r--r--   0 lei        (501) staff       (20)      834 2023-04-14 15:02:34.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:12.245033 globus-compute-sdk-2.0.1a0/globus_compute_sdk.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)      770 2023-04-14 15:04:12.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1557 2023-04-14 15:04:12.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-14 15:04:12.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      397 2023-04-14 15:04:12.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       19 2023-04-14 15:04:12.000000 globus-compute-sdk-2.0.1a0/globus_compute_sdk.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-14 15:04:12.251431 globus-compute-sdk-2.0.1a0/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     2707 2023-04-13 00:34:31.000000 globus-compute-sdk-2.0.1a0/setup.py
```

### Comparing `globus-compute-sdk-2.0.0a1/LICENSE` & `globus-compute-sdk-2.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/PKG-INFO` & `globus-compute-sdk-2.0.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.0.0a1
+Version: 2.0.1a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/_environments.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/_environments.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.task_id = task_id
 
     def __str__(self):
         return "Globus Compute Task ID " + self.task_id
 
     async def get_result(self):
         """
-        Coroutine to wait on the Globus Compute task to complete and then
+        Coroutine waiting for the Globus Compute task to complete and then
         return the result
 
         :return:
             result : Any
         """
         await self
         return self.result()
```

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/batch.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,25 +16,24 @@
 from globus_compute_sdk.sdk._environments import (
     get_web_service_url,
     get_web_socket_url,
     urls_might_mismatch,
 )
 from globus_compute_sdk.sdk.asynchronous.compute_task import ComputeTask
 from globus_compute_sdk.sdk.asynchronous.ws_polling_task import WebSocketPollingTask
-from globus_compute_sdk.sdk.search import SearchHelper
 from globus_compute_sdk.sdk.web_client import FunctionRegistrationData
 from globus_compute_sdk.serialize import ComputeSerializer
 from globus_compute_sdk.version import __version__, compare_versions
 
 from .batch import Batch
 from .login_manager import LoginManager, LoginManagerProtocol, requires_login
 
 logger = logging.getLogger(__name__)
 
-_FUNCX_HOME = os.path.join("~", ".funcx")
+_FUNCX_HOME = os.path.join("~", ".globus_compute")
 
 
 class Client:
     """Main class for interacting with the Globus Compute service
 
     Holds helper operations for performing common tasks with the Globus Compute service.
     """
@@ -195,24 +194,14 @@
                 self.loop,
                 init_task_group_id=self.session_task_group_id,
                 results_ws_uri=self.results_ws_uri,
             )
         else:
             self.loop = None
 
-        # TODO: remove this
-        self._searcher = None
-
-    @property
-    def searcher(self):
-        # TODO: remove this
-        if self._searcher is None:
-            self._searcher = SearchHelper(self.login_manager.get_search_client())
-        return self._searcher
-
     def version_check(self, endpoint_version: str | None = None) -> None:
         """Check this client version meets the service's minimum supported version.
 
         Raises a VersionMismatch error on failure.
         """
         data = self.web_client.get_version()
 
@@ -475,14 +464,15 @@
     @requires_login
     def register_endpoint(
         self,
         name,
         endpoint_id,
         metadata=None,
         multi_tenant=False,
+        display_name=None,
     ):
         """Register an endpoint with the Globus Compute service.
 
         Parameters
         ----------
         :param name str Name of the endpoint
         :param endpoint_id str The uuid of the endpoint
@@ -499,14 +489,15 @@
         self.version_check()
 
         r = self.web_client.register_endpoint(
             endpoint_name=name,
             endpoint_id=endpoint_id,
             metadata=metadata,
             multi_tenant=multi_tenant,
+            display_name=display_name,
         )
         return r.data
 
     @requires_login
     def get_result_amqp_url(self) -> dict[str, str]:
         r = self.web_client.get_result_amqp_url()
         return r.data
@@ -608,15 +599,15 @@
         self,
         function,
         function_name=None,
         container_uuid=None,
         description=None,
         public=False,
         group=None,
-        searchable=True,
+        searchable=None,
     ) -> str:
         """Register a function code with the Globus Compute service.
 
         Parameters
         ----------
         function : Python Function
             The function to be registered for remote execution
@@ -630,75 +621,41 @@
             Whether or not the function is publicly accessible. Default = False
         group : str
             A globus group uuid to share this function with
         searchable : bool
             If true, the function will be indexed into globus search with the
             appropriate permissions
 
+            DEPRECATED - ingesting functions to Globus Search is not currently supported
+
         Returns
         -------
         function uuid : str
             UUID identifier for the registered function
         """
+        if searchable is not None:
+            warnings.warn(
+                "The 'searchable' argument is deprecated and no longer functional. "
+                "It will be removed in a future release."
+            )
+
         data = FunctionRegistrationData(
             function=function,
             container_uuid=container_uuid,
             entry_point=function_name,
             description=description,
             public=public,
             group=group,
-            searchable=searchable,
             serializer=self.fx_serializer,
         )
         logger.info(f"Registering function : {data}")
         r = self.web_client.register_function(data)
         return r.data["function_uuid"]
 
     @requires_login
-    def search_function(self, q, offset=0, limit=10, advanced=False):
-        """Search for function via the Globus Compute service
-
-        Parameters
-        ----------
-        q : str
-            free-form query string
-        offset : int
-            offset into total results
-        limit : int
-            max number of results to return
-        advanced : bool
-            allows elastic-search like syntax in query string
-
-        Returns
-        -------
-        FunctionSearchResults
-        """
-        return self.searcher.search_function(
-            q, offset=offset, limit=limit, advanced=advanced
-        )
-
-    @requires_login
-    def search_endpoint(self, q, scope="all", owner_id=None):
-        """
-
-        Parameters
-        ----------
-        q
-        scope : str
-            Can be one of {'all', 'my-endpoints', 'shared-with-me'}
-        owner_id
-            should be urn like f"urn:globus:auth:identity:{owner_uuid}"
-
-        Returns
-        -------
-
-        """
-        return self.searcher.search_endpoint(q, scope=scope, owner_id=owner_id)
-
-    @requires_login
     def register_container(self, location, container_type, name="", description=""):
         """Register a container with the Globus Compute service.
 
         Parameters
         ----------
         location : str
             The location of the container (e.g., its docker url). Required
```

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -713,15 +713,15 @@
 
         rw.watch_for_task_results(some_list_of_futures)
 
     When there are no more open futures and no more results, the thread
     will opportunistically shutdown; the caller must handle this scenario
     if new futures arrive, and create a new _ResultWatcher instance.
 
-    :param funcx_executor: A Executor instance
+    :param funcx_executor: An Executor instance
     :param poll_period_s: [default: 0.5] how frequently to check for and
         handle events.  For example, if the thread should stop due to user
         request or if there are results to match.
     :param connect_attempt_limit: [default: 3] how many times to attempt
         connecting to the AMQP server before bailing.
     :param channel_close_window_s: [default: 10] how large a window to
         tally channel open events.
```

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import os
 import sys
 import threading
 import typing as t
 
 import globus_sdk
-from globus_sdk.scopes import AuthScopes, ScopeBuilder, SearchScopes
+from globus_sdk.scopes import AuthScopes, ScopeBuilder
 
 from ..web_client import WebClient
 from .client_login import get_client_login, is_client_login
 from .globus_auth import internal_auth_client
 from .login_flow import do_link_auth_flow
 from .tokenstore import get_token_storage_adapter
 
@@ -55,15 +55,14 @@
     - methods for building SDK client objects with correct RefreshTokenAuthorizer
       authorizers
     """
 
     SCOPES: dict[str, list[str]] = {
         ComputeScopes.resource_server: [ComputeScopes.all],
         AuthScopes.resource_server: [AuthScopes.openid],
-        SearchScopes.resource_server: [SearchScopes.all],
     }
 
     def __init__(self, *, environment: str | None = None) -> None:
         self._token_storage = get_token_storage_adapter(environment=environment)
         self._access_lock = threading.Lock()
 
     @property
@@ -181,19 +180,14 @@
                 )
 
     def get_auth_client(self) -> globus_sdk.AuthClient:
         return globus_sdk.AuthClient(
             authorizer=self._get_authorizer(AuthScopes.resource_server)
         )
 
-    def get_search_client(self) -> globus_sdk.SearchClient:
-        return globus_sdk.SearchClient(
-            authorizer=self._get_authorizer(SearchScopes.resource_server)
-        )
-
     def get_web_client(
         self, *, base_url: str | None = None, app_name: str | None = None
     ) -> WebClient:
         return WebClient(
             base_url=base_url,
             app_name=app_name,
             authorizer=self._get_authorizer(ComputeScopes.resource_server),
```

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,12 +21,9 @@
 
     def logout(self) -> bool:
         ...
 
     def get_auth_client(self) -> globus_sdk.AuthClient:
         ...
 
-    def get_search_client(self) -> globus_sdk.SearchClient:
-        ...
-
     def get_web_client(self, *, base_url: str | None = None) -> WebClient:
         ...
```

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,25 +31,39 @@
                     auth_client.oauth2_revoke_token(token_data["access_token"])
                 if "refresh_token" in token_data:
                     auth_client.oauth2_revoke_token(token_data["refresh_token"])
         finally:
             os.remove(token_file)
 
 
-def _ensure_funcx_dir() -> pathlib.Path:
-    dirname = _home() / ".funcx"
-    try:
-        os.makedirs(dirname)
-    except FileExistsError:
+def ensure_compute_dir() -> pathlib.Path:
+    legacy_dirname = _home() / ".funcx"
+    dirname = _home() / ".globus_compute"
+
+    if dirname.is_dir():
         pass
+
+    elif dirname.is_file():
+        raise FileExistsError(
+            f"Error creating directory {dirname}, "
+            "please remove or rename the conflicting file"
+        )
+
+    elif legacy_dirname.is_dir():
+        legacy_dirname.replace(dirname)
+        legacy_dirname.symlink_to(dirname, target_is_directory=True)
+
+    else:
+        dirname.mkdir(mode=0o700, parents=True, exist_ok=True)
+
     return dirname
 
 
 def _get_storage_filename():
-    datadir = _ensure_funcx_dir()
+    datadir = ensure_compute_dir()
     return os.path.join(datadir, "storage.db")
 
 
 def _resolve_namespace(environment: str | None) -> str:
     """
     Return the namespace used to save tokens. This will check
     if a client login is being used and return either:
```

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/sdk/web_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         function_name: t.Optional[str] = None,
         function_code: t.Optional[str] = None,
         container_uuid: t.Optional[ID_PARAM_T] = None,
         entry_point: t.Optional[str] = None,
         description: t.Optional[str] = None,
         public: bool = False,
         group: t.Optional[str] = None,
-        searchable: bool = True,
         serializer: t.Optional[ComputeSerializer] = None,
     ):
         if function is not None:
             function_name = function.__name__
             function_code = _get_packed_code(function, serializer=serializer)
 
         if function_name is None or function_code is None:
@@ -56,26 +55,24 @@
         self.container_uuid = (
             str(container_uuid) if container_uuid is not None else container_uuid
         )
         self.entry_point = entry_point if entry_point is not None else function_name
         self.description = description
         self.public = public
         self.group = group
-        self.searchable = searchable
 
     def to_dict(self):
         return {
             "function_name": self.function_name,
             "function_code": self.function_code,
             "container_uuid": self.container_uuid,
             "entry_point": self.entry_point,
             "description": self.description,
             "public": self.public,
             "group": self.group,
-            "searchable": self.searchable,
         }
 
     def __str__(self):
         return "FunctionRegistrationData(" + json.dumps(self.to_dict()) + ")"
 
 
 class WebClient(globus_sdk.BaseClient):
@@ -155,21 +152,28 @@
     def register_endpoint(
         self,
         endpoint_name: str,
         endpoint_id: ID_PARAM_T,
         *,
         metadata: t.Optional[dict] = None,
         multi_tenant: t.Optional[bool] = None,
+        display_name: t.Optional[str] = None,
         additional_fields: t.Optional[t.Dict[str, t.Any]] = None,
     ) -> globus_sdk.GlobusHTTPResponse:
         data: t.Dict[str, t.Any] = {
             "endpoint_name": endpoint_name,
             "endpoint_uuid": str(endpoint_id),
         }
 
+        # Only populate if not None.  "" is valid and will be included
+        # No value or a 'None' on an existing endpoint will leave
+        # the old display_name unchanged
+        if display_name is not None:
+            data["display_name"] = display_name
+
         # Only send this param if True.  Will have to change to
         # `if multi_tenant is not None` if we want to always pass it
         if multi_tenant:
             data["multi_tenant"] = multi_tenant
 
         if metadata:
             data["metadata"] = metadata
```

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/serialize/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/concretes.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/serialize/facade.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk/version.py` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.0a1"
+__version__ = "2.0.1a0"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.0.0a1
+Version: 2.0.1a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `globus-compute-sdk-2.0.0a1/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.0.1a0/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 globus_compute_sdk/errors/error_types.py
 globus_compute_sdk/sdk/__init__.py
 globus_compute_sdk/sdk/_environments.py
 globus_compute_sdk/sdk/batch.py
 globus_compute_sdk/sdk/client.py
 globus_compute_sdk/sdk/container_spec.py
 globus_compute_sdk/sdk/executor.py
-globus_compute_sdk/sdk/search.py
 globus_compute_sdk/sdk/web_client.py
 globus_compute_sdk/sdk/asynchronous/__init__.py
 globus_compute_sdk/sdk/asynchronous/compute_future.py
 globus_compute_sdk/sdk/asynchronous/compute_task.py
 globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
 globus_compute_sdk/sdk/login_manager/__init__.py
 globus_compute_sdk/sdk/login_manager/client_login.py
```

### Comparing `globus-compute-sdk-2.0.0a1/setup.py` & `globus-compute-sdk-2.0.1a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "furo==2021.09.08",
 ]
 
 TEST_REQUIRES = [
     "flake8==3.8.0",
     "pytest>=7.2",
     "pytest-mock",
+    "pyfakefs",
     "coverage",
     # easy mocking of the `requests` library
     "responses",
 ]
 DEV_REQUIRES = TEST_REQUIRES + [
     "pre-commit",
 ]
```

