# Comparing `tmp/secapi-tl-1.1.1.tar.gz` & `tmp/secapi-tl-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secapi-tl-1.1.1.tar", last modified: Fri Apr 14 12:13:09 2023, max compression
+gzip compressed data, was "secapi-tl-1.1.2.tar", last modified: Fri Apr 14 16:46:03 2023, max compression
```

## Comparing `secapi-tl-1.1.1.tar` & `secapi-tl-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.1/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     3698 2023-04-09 10:03:28.000000 secapi-tl-1.1.1/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-14 12:08:01.000000 secapi-tl-1.1.1/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/src/secapi_tl/
--rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.1/src/secapi_tl/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6025 2023-04-08 12:35:48.000000 secapi-tl-1.1.1/src/secapi_tl/filing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-08 12:35:48.000000 secapi-tl-1.1.1/src/secapi_tl/filing_query.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.1/src/secapi_tl/key_mapper.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1206 2023-04-14 12:05:11.000000 secapi-tl-1.1.1/src/secapi_tl/request.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 12:13:09.676576 secapi-tl-1.1.1/src/secapi_tl.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-14 12:13:09.000000 secapi-tl-1.1.1/src/secapi_tl.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-14 12:13:09.000000 secapi-tl-1.1.1/src/secapi_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-14 12:13:09.000000 secapi-tl-1.1.1/src/secapi_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-14 12:13:09.000000 secapi-tl-1.1.1/src/secapi_tl.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-14 12:13:09.000000 secapi-tl-1.1.1/src/secapi_tl.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 16:46:03.746616 secapi-tl-1.1.2/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.2/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-14 16:46:03.746616 secapi-tl-1.1.2/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3698 2023-04-09 10:03:28.000000 secapi-tl-1.1.2/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-14 16:45:56.000000 secapi-tl-1.1.2/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-14 16:46:03.746616 secapi-tl-1.1.2/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 16:46:03.746616 secapi-tl-1.1.2/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 16:46:03.746616 secapi-tl-1.1.2/src/secapi_tl/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.2/src/secapi_tl/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6025 2023-04-08 12:35:48.000000 secapi-tl-1.1.2/src/secapi_tl/filing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-08 12:35:48.000000 secapi-tl-1.1.2/src/secapi_tl/filing_query.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.2/src/secapi_tl/key_mapper.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1037 2023-04-14 16:44:49.000000 secapi-tl-1.1.2/src/secapi_tl/request.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-14 16:46:03.746616 secapi-tl-1.1.2/src/secapi_tl.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-14 16:46:03.000000 secapi-tl-1.1.2/src/secapi_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-14 16:46:03.000000 secapi-tl-1.1.2/src/secapi_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-14 16:46:03.000000 secapi-tl-1.1.2/src/secapi_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-14 16:46:03.000000 secapi-tl-1.1.2/src/secapi_tl.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-14 16:46:03.000000 secapi-tl-1.1.2/src/secapi_tl.egg-info/top_level.txt
```

### Comparing `secapi-tl-1.1.1/LICENSE` & `secapi-tl-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.1/PKG-INFO` & `secapi-tl-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.1
+Version: 1.1.2
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `secapi-tl-1.1.1/README.md` & `secapi-tl-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.1/src/secapi_tl/filing.py` & `secapi-tl-1.1.2/src/secapi_tl/filing.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.1/src/secapi_tl/filing_query.py` & `secapi-tl-1.1.2/src/secapi_tl/filing_query.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.1/src/secapi_tl/key_mapper.py` & `secapi-tl-1.1.2/src/secapi_tl/key_mapper.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.1/src/secapi_tl/request.py` & `secapi-tl-1.1.2/src/secapi_tl/request.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 
 
 class Request:
 
     @staticmethod
     @sleep_and_retry
     @limits(calls=SEC_REQUEST_COUNT, period=SEC_PERIOD)
-    def sec_request(url: str, header: dict = None, retries: int = 5):
+    def sec_request(url: str, header: dict = None):
         if header is None:
             header = SEC_HEADER
         response = requests.get(url=url, headers=header)
-
-        if response.status_code != 200 and retries > 0:
-            response = Request.sec_request(url=url, header=header, retries=retries-1)
-            if response.status_code != 200:
-                raise ConnectionError(f'invalid response status code, status code: {response.status_code}')
+        if response.status_code != 200:
+            raise ConnectionError(f'invalid response status code, status code: {response.status_code}')
         return response
```

### Comparing `secapi-tl-1.1.1/src/secapi_tl.egg-info/PKG-INFO` & `secapi-tl-1.1.2/src/secapi_tl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.1
+Version: 1.1.2
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

