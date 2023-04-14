# Comparing `tmp/alibabacloud_gateway_pds-0.0.5.tar.gz` & `tmp/alibabacloud_gateway_pds-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gateway_pds-0.0.5.tar", last modified: Mon Aug  8 04:15:05 2022, max compression
+gzip compressed data, was "dist/alibabacloud_gateway_pds-0.0.6.tar", last modified: Fri Apr 14 06:45:06 2023, max compression
```

## Comparing `alibabacloud_gateway_pds-0.0.5.tar` & `alibabacloud_gateway_pds-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/
--rw-r--r--   0 root         (0) root         (0)      886 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds/
--rw-r--r--   0 root         (0) root         (0)       22 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18144 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds.egg-info/
--rw-r--r--   0 root         (0) root         (0)      886 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      383 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2865 2022-08-08 04:15:05.000000 alibabacloud_gateway_pds-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)      886 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18288 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      886 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/setup.py
```

### Comparing `alibabacloud_gateway_pds-0.0.5/PKG-INFO` & `alibabacloud_gateway_pds-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gateway_pds
-Version: 0.0.5
+Version: 0.0.6
 Summary: Alibaba Cloud PDS SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,pds
```

### Comparing `alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds/client.py` & `alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,22 +66,23 @@
                 else:
                     m = UtilClient.assert_as_map(request.body)
                     form_obj = OpenApiUtilClient.to_form(m)
                     request.stream = form_obj
                     request.headers['content-type'] = 'application/x-www-form-urlencoded'
         if not UtilClient.equal_string(request.auth_type, 'Anonymous'):
             credential = request.credential
-            access_key_id = credential.get_access_key_id()
-            access_key_secret = credential.get_access_key_secret()
-            security_token = credential.get_security_token()
-            bearer_token = credential.get_bearer_token()
-            if not UtilClient.empty(bearer_token):
+            auth_type = credential.get_type()
+            if UtilClient.equal_string(auth_type, 'bearer'):
+                bearer_token = credential.get_bearer_token()
                 request.headers['x-acs-bearer-token'] = bearer_token
                 request.headers['Authorization'] = f'Bearer {bearer_token}'
             else:
+                access_key_id = credential.get_access_key_id()
+                access_key_secret = credential.get_access_key_secret()
+                security_token = credential.get_security_token()
                 if not UtilClient.empty(security_token):
                     request.headers['x-acs-security-token'] = security_token
                 request.headers['Authorization'] = self.get_authorization(request.pathname, request.method, request.query, request.headers, access_key_id, access_key_secret)
 
     async def modify_request_async(
         self,
         context: spi_models.InterceptorContext,
@@ -113,22 +114,23 @@
                 else:
                     m = UtilClient.assert_as_map(request.body)
                     form_obj = OpenApiUtilClient.to_form(m)
                     request.stream = form_obj
                     request.headers['content-type'] = 'application/x-www-form-urlencoded'
         if not UtilClient.equal_string(request.auth_type, 'Anonymous'):
             credential = request.credential
-            access_key_id = await credential.get_access_key_id_async()
-            access_key_secret = await credential.get_access_key_secret_async()
-            security_token = await credential.get_security_token_async()
-            bearer_token = credential.get_bearer_token()
-            if not UtilClient.empty(bearer_token):
+            auth_type = credential.get_type()
+            if UtilClient.equal_string(auth_type, 'bearer'):
+                bearer_token = credential.get_bearer_token()
                 request.headers['x-acs-bearer-token'] = bearer_token
                 request.headers['Authorization'] = f'Bearer {bearer_token}'
             else:
+                access_key_id = await credential.get_access_key_id_async()
+                access_key_secret = await credential.get_access_key_secret_async()
+                security_token = await credential.get_security_token_async()
                 if not UtilClient.empty(security_token):
                     request.headers['x-acs-security-token'] = security_token
                 request.headers['Authorization'] = await self.get_authorization_async(request.pathname, request.method, request.query, request.headers, access_key_id, access_key_secret)
 
     def modify_response(
         self,
         context: spi_models.InterceptorContext,
```

### Comparing `alibabacloud_gateway_pds-0.0.5/alibabacloud_gateway_pds.egg-info/PKG-INFO` & `alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gateway-pds
-Version: 0.0.5
+Version: 0.0.6
 Summary: Alibaba Cloud PDS SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,pds
```

### Comparing `alibabacloud_gateway_pds-0.0.5/setup.py` & `alibabacloud_gateway_pds-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gateway_pds.
 
-Created on 08/08/2022
+Created on 14/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gateway_pds"
 NAME = "alibabacloud_gateway_pds" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud PDS SDK Library for Python"
```

