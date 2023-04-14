# Comparing `tmp/houston-client-1.3.0.tar.gz` & `tmp/houston-client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "houston-client-1.3.0.tar", last modified: Thu Mar 16 17:03:59 2023, max compression
+gzip compressed data, was "houston-client-1.3.1.tar", last modified: Fri Apr 14 08:09:37 2023, max compression
```

## Comparing `houston-client-1.3.0.tar` & `houston-client-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-03-16 17:03:59.826052 houston-client-1.3.0/
--rw-r--r--   0 matt       (501) staff       (20)     1084 2023-03-03 11:09:26.000000 houston-client-1.3.0/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     3796 2023-03-16 17:03:59.825859 houston-client-1.3.0/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     1787 2023-03-16 15:48:40.000000 houston-client-1.3.0/README.md
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-03-16 17:03:59.823486 houston-client-1.3.0/houston/
--rw-r--r--   0 matt       (501) staff       (20)      355 2023-03-03 11:09:26.000000 houston-client-1.3.0/houston/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     5115 2023-03-16 16:51:35.000000 houston-client-1.3.0/houston/__main__.py
--rw-r--r--   0 matt       (501) staff       (20)    19730 2023-03-16 16:57:05.000000 houston-client-1.3.0/houston/client.py
--rw-r--r--   0 matt       (501) staff       (20)    15417 2023-03-16 16:07:22.000000 houston-client-1.3.0/houston/commands.py
--rw-r--r--   0 matt       (501) staff       (20)      597 2023-03-03 11:09:26.000000 houston-client-1.3.0/houston/exceptions.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-03-16 17:03:59.824636 houston-client-1.3.0/houston/gcp/
--rw-r--r--   0 matt       (501) staff       (20)       70 2023-03-07 15:59:08.000000 houston-client-1.3.0/houston/gcp/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     6915 2023-03-16 15:54:57.000000 houston-client-1.3.0/houston/gcp/client.py
--rw-r--r--   0 matt       (501) staff       (20)     4297 2023-03-16 15:57:30.000000 houston-client-1.3.0/houston/gcp/cloud_function.py
--rw-r--r--   0 matt       (501) staff       (20)      813 2023-03-03 11:09:26.000000 houston-client-1.3.0/houston/gcp/cloud_storage.py
--rw-r--r--   0 matt       (501) staff       (20)     1150 2023-03-03 11:09:26.000000 houston-client-1.3.0/houston/gcp/secret_manager.py
--rw-r--r--   0 matt       (501) staff       (20)     4642 2023-03-07 17:47:20.000000 houston-client-1.3.0/houston/interface.py
--rw-r--r--   0 matt       (501) staff       (20)      149 2023-03-03 11:09:26.000000 houston-client-1.3.0/houston/plan.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-03-16 17:03:59.825121 houston-client-1.3.0/houston/plugin/
--rwxr-xr-x   0 matt       (501) staff       (20)        1 2023-03-03 11:09:26.000000 houston-client-1.3.0/houston/plugin/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     3388 2023-03-16 15:54:57.000000 houston-client-1.3.0/houston/plugin/azure.py
--rw-r--r--   0 matt       (501) staff       (20)     1041 2023-03-03 11:09:26.000000 houston-client-1.3.0/houston/plugin/gcp.py
--rw-r--r--   0 matt       (501) staff       (20)     4426 2023-03-03 11:09:26.000000 houston-client-1.3.0/houston/service.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-03-16 17:03:59.825713 houston-client-1.3.0/houston_client.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     3796 2023-03-16 17:03:59.000000 houston-client-1.3.0/houston_client.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      594 2023-03-16 17:03:59.000000 houston-client-1.3.0/houston_client.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-03-16 17:03:59.000000 houston-client-1.3.0/houston_client.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)      263 2023-03-16 17:03:59.000000 houston-client-1.3.0/houston_client.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)        8 2023-03-16 17:03:59.000000 houston-client-1.3.0/houston_client.egg-info/top_level.txt
--rw-r--r--   0 matt       (501) staff       (20)     1185 2023-03-16 17:02:50.000000 houston-client-1.3.0/pyproject.toml
--rw-r--r--   0 matt       (501) staff       (20)       38 2023-03-16 17:03:59.826087 houston-client-1.3.0/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)       38 2023-03-03 11:09:26.000000 houston-client-1.3.0/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-04-14 08:09:37.904454 houston-client-1.3.1/
+-rw-r--r--   0 matt       (501) staff       (20)     1084 2023-03-03 11:09:26.000000 houston-client-1.3.1/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)     3796 2023-04-14 08:09:37.904326 houston-client-1.3.1/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     1787 2023-04-14 08:08:26.000000 houston-client-1.3.1/README.md
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-04-14 08:09:37.901933 houston-client-1.3.1/houston/
+-rw-r--r--   0 matt       (501) staff       (20)      355 2023-03-03 11:09:26.000000 houston-client-1.3.1/houston/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     5115 2023-04-14 08:08:26.000000 houston-client-1.3.1/houston/__main__.py
+-rw-r--r--   0 matt       (501) staff       (20)    19730 2023-04-14 08:08:26.000000 houston-client-1.3.1/houston/client.py
+-rw-r--r--   0 matt       (501) staff       (20)    15417 2023-04-14 08:08:26.000000 houston-client-1.3.1/houston/commands.py
+-rw-r--r--   0 matt       (501) staff       (20)      597 2023-03-03 11:09:26.000000 houston-client-1.3.1/houston/exceptions.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-04-14 08:09:37.902896 houston-client-1.3.1/houston/gcp/
+-rw-r--r--   0 matt       (501) staff       (20)       70 2023-04-13 08:12:34.000000 houston-client-1.3.1/houston/gcp/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     6915 2023-04-14 08:08:26.000000 houston-client-1.3.1/houston/gcp/client.py
+-rw-r--r--   0 matt       (501) staff       (20)     4297 2023-04-14 08:08:26.000000 houston-client-1.3.1/houston/gcp/cloud_function.py
+-rw-r--r--   0 matt       (501) staff       (20)      813 2023-03-03 11:09:26.000000 houston-client-1.3.1/houston/gcp/cloud_storage.py
+-rw-r--r--   0 matt       (501) staff       (20)     1150 2023-03-03 11:09:26.000000 houston-client-1.3.1/houston/gcp/secret_manager.py
+-rw-r--r--   0 matt       (501) staff       (20)     4817 2023-04-14 08:08:26.000000 houston-client-1.3.1/houston/interface.py
+-rw-r--r--   0 matt       (501) staff       (20)      149 2023-03-03 11:09:26.000000 houston-client-1.3.1/houston/plan.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-04-14 08:09:37.903455 houston-client-1.3.1/houston/plugin/
+-rwxr-xr-x   0 matt       (501) staff       (20)        1 2023-03-03 11:09:26.000000 houston-client-1.3.1/houston/plugin/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     3388 2023-04-14 08:08:26.000000 houston-client-1.3.1/houston/plugin/azure.py
+-rw-r--r--   0 matt       (501) staff       (20)     1041 2023-03-03 11:09:26.000000 houston-client-1.3.1/houston/plugin/gcp.py
+-rw-r--r--   0 matt       (501) staff       (20)     4426 2023-03-03 11:09:26.000000 houston-client-1.3.1/houston/service.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-04-14 08:09:37.904125 houston-client-1.3.1/houston_client.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)     3796 2023-04-14 08:09:37.000000 houston-client-1.3.1/houston_client.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      594 2023-04-14 08:09:37.000000 houston-client-1.3.1/houston_client.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-04-14 08:09:37.000000 houston-client-1.3.1/houston_client.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)      263 2023-04-14 08:09:37.000000 houston-client-1.3.1/houston_client.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)        8 2023-04-14 08:09:37.000000 houston-client-1.3.1/houston_client.egg-info/top_level.txt
+-rw-r--r--   0 matt       (501) staff       (20)     1185 2023-04-14 08:08:26.000000 houston-client-1.3.1/pyproject.toml
+-rw-r--r--   0 matt       (501) staff       (20)       38 2023-04-14 08:09:37.904492 houston-client-1.3.1/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)       38 2023-03-03 11:09:26.000000 houston-client-1.3.1/setup.py
```

### Comparing `houston-client-1.3.0/LICENSE` & `houston-client-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/PKG-INFO` & `houston-client-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: houston-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Houston Python Client
 Author-email: James Watkinson <info@datasparq.ai>, Matt Simmons <info@datasparq.ai>
 License: MIT License
         
         Copyright (c) 2020, 2021, 2022, 2023 Datasparq
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `houston-client-1.3.0/README.md` & `houston-client-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/__main__.py` & `houston-client-1.3.1/houston/__main__.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/client.py` & `houston-client-1.3.1/houston/client.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/commands.py` & `houston-client-1.3.1/houston/commands.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/exceptions.py` & `houston-client-1.3.1/houston/exceptions.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/gcp/client.py` & `houston-client-1.3.1/houston/gcp/client.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/gcp/cloud_function.py` & `houston-client-1.3.1/houston/gcp/cloud_function.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/gcp/cloud_storage.py` & `houston-client-1.3.1/houston/gcp/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/gcp/secret_manager.py` & `houston-client-1.3.1/houston/gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/interface.py` & `houston-client-1.3.1/houston/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     def __init__(self, key):
         self.headers = {"x-access-key": key, "Content-Type": "application/json"}
 
     def request(self, method, uri, params=None, data=None, retry=3, safe=False, fire_and_forget=False):
         """
         Request a Houston resource
 
-        :param string method: Http method required for request (e.g. GET, POST, DELETE etc)
+        :param string method: Http method required for request (e.g. GET, POST, DELETE etc.)
         :param string uri: Complete URL of request, including schema (e.g. https://)
         :param dict params: Parameters to be sent with request (will be json encoded)
         :param dict data: Parameters to be sent with request (will be form encoded)
         :param int retry: Number of retries to attempt with request (only used by 429 server responses)
-        :param bool safe: Do not raise errors in-case of client error
+        :param bool safe: Do not raise errors in case of client error
         :param bool fire_and_forget: If true, do not wait for a response
         :return: HTTP response code and response payload parsed as dict
         """
 
         timeout = None
         if fire_and_forget:
             timeout = 1
@@ -42,24 +42,28 @@
 
         except requests.exceptions.ReadTimeout:
             if fire_and_forget:
                 return 200, dict()
             else:
                 raise
         except requests.exceptions.ConnectionError:
-            raise HoustonServerError(
-                f"Unable to connect to Houston API server at url: {uri}. Is your Houston server running?"
-            )
+            if retry > 0:
+                time.sleep(random())
+                return self.request(method, uri, params, data, retry - 1)
+            else:
+                raise HoustonServerError(
+                    f"Unable to connect to Houston API server at url: {uri}. Is your Houston server running?"
+                )
 
         # retry if server busy - this can be common in a large workflow due to operations being immutable. 572 is the
         # Houston API's code for DagLockedError. 429 is 'Too Many Requests'.
         if response.status_code in (429, 572):
             if retry > 0:
                 time.sleep(random())
-                self.request(method, uri, params, data, retry - 1)
+                return self.request(method, uri, params, data, retry - 1)
             else:
                 raise HoustonServerBusy(
                     "received too many 429 responses from server, please reduce the number of requests"
                 )
 
         if 400 <= response.status_code < 500 and not safe:
             err_msg, err_type = self._parse_error(response)
```

### Comparing `houston-client-1.3.0/houston/plugin/azure.py` & `houston-client-1.3.1/houston/plugin/azure.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/plugin/gcp.py` & `houston-client-1.3.1/houston/plugin/gcp.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston/service.py` & `houston-client-1.3.1/houston/service.py`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/houston_client.egg-info/PKG-INFO` & `houston-client-1.3.1/houston_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: houston-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Houston Python Client
 Author-email: James Watkinson <info@datasparq.ai>, Matt Simmons <info@datasparq.ai>
 License: MIT License
         
         Copyright (c) 2020, 2021, 2022, 2023 Datasparq
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `houston-client-1.3.0/houston_client.egg-info/SOURCES.txt` & `houston-client-1.3.1/houston_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `houston-client-1.3.0/pyproject.toml` & `houston-client-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "houston-client"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="James Watkinson", email="info@datasparq.ai" },
   { name="Matt Simmons", email="info@datasparq.ai" },
 ]
 description = "Houston Python Client"
 keywords = ["houston"]
 readme = "README.md"
```

