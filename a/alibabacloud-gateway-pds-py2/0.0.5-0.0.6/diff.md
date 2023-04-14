# Comparing `tmp/alibabacloud_gateway_pds_py2-0.0.5.tar.gz` & `tmp/alibabacloud_gateway_pds_py2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gateway_pds_py2-0.0.5.tar", last modified: Mon Aug  8 04:15:00 2022, max compression
+gzip compressed data, was "dist/alibabacloud_gateway_pds_py2-0.0.6.tar", last modified: Fri Apr 14 06:45:09 2023, max compression
```

## Comparing `alibabacloud_gateway_pds_py2-0.0.5.tar` & `alibabacloud_gateway_pds_py2-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     1020 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds/
--rw-r--r--   0 root         (0) root         (0)       22 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9368 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      339 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      419 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3177 2022-08-08 04:15:00.000000 alibabacloud_gateway_pds_py2-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9440 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      339 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      419 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/setup.py
```

### Comparing `alibabacloud_gateway_pds_py2-0.0.5/PKG-INFO` & `alibabacloud_gateway_pds_py2-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gateway_pds_py2
-Version: 0.0.5
+Version: 0.0.6
 Summary: Alibaba Cloud PDS SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,pds,py2
```

### Comparing `alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds/client.py` & `alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,22 +51,23 @@
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
                 request.headers['Authorization'] = 'Bearer %s' % TeaConverter.to_unicode(bearer_token)
             else:
+                access_key_id = credential.get_access_key_id()
+                access_key_secret = credential.get_access_key_secret()
+                security_token = credential.get_security_token()
                 if not UtilClient.empty(security_token):
                     request.headers['x-acs-security-token'] = security_token
                 request.headers['Authorization'] = self.get_authorization(request.pathname, request.method, request.query, request.headers, access_key_id, access_key_secret)
 
     def modify_response(self, context, attribute_map):
         request = context.request
         response = context.response
```

### Comparing `alibabacloud_gateway_pds_py2-0.0.5/alibabacloud_gateway_pds_py2.egg-info/PKG-INFO` & `alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gateway-pds-py2
-Version: 0.0.5
+Version: 0.0.6
 Summary: Alibaba Cloud PDS SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,pds,py2
```

### Comparing `alibabacloud_gateway_pds_py2-0.0.5/setup.py` & `alibabacloud_gateway_pds_py2-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gateway_pds_py2.
 
-Created on 08/08/2022
+Created on 14/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gateway_pds"
 NAME = "alibabacloud_gateway_pds_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud PDS SDK Library for Python2"
```

