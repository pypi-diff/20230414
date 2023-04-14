# Comparing `tmp/alibabacloud_dypnsapi20170525_py2-1.0.0.tar.gz` & `tmp/alibabacloud_dypnsapi20170525_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dypnsapi20170525_py2-1.0.0.tar", last modified: Wed Sep  8 02:50:55 2021, max compression
+gzip compressed data, was "dist/alibabacloud_dypnsapi20170525_py2-1.0.1.tar", last modified: Fri Apr 14 08:44:09 2023, max compression
```

## Comparing `alibabacloud_dypnsapi20170525_py2-1.0.0.tar` & `alibabacloud_dypnsapi20170525_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     2462 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       94 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2876 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      467 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2462 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       30 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525_py2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525/
--rw-r--r--   0 root         (0) root         (0)       21 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52862 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525/models.py
--rw-r--r--   0 root         (0) root         (0)     7218 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525/client.py
--rw-r--r--   0 root         (0) root         (0)     1048 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      588 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1131 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       28 2021-09-08 02:50:55.000000 alibabacloud_dypnsapi20170525_py2-1.0.0/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:09.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       72 2023-04-14 08:44:08.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-14 08:44:08.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-14 08:44:08.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-04-14 08:44:09.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-14 08:44:08.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-04-14 08:44:08.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:09.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-14 08:44:08.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26020 2023-04-14 08:44:08.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525/client.py
+-rw-r--r--   0 root         (0) root         (0)    92082 2023-04-14 08:44:08.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:09.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-04-14 08:44:09.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-04-14 08:44:09.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 08:44:09.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-14 08:44:09.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-14 08:44:09.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-14 08:44:09.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-04-14 08:44:08.000000 alibabacloud_dypnsapi20170525_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_dypnsapi20170525_py2-1.0.0/PKG-INFO` & `alibabacloud_dypnsapi20170525_py2-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: alibabacloud_dypnsapi20170525_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Dypnsapi (20170525) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -59,7 +59,8 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
```

### Comparing `alibabacloud_dypnsapi20170525_py2-1.0.0/setup.py` & `alibabacloud_dypnsapi20170525_py2-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dypnsapi20170525_py2.
 
-Created on 08/09/2021
+Created on 14/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dypnsapi20170525"
 NAME = "alibabacloud_dypnsapi20170525_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dypnsapi (20170525) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.5, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.0.5, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

### Comparing `alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525_py2.egg-info/PKG-INFO` & `alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525_py2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: alibabacloud-dypnsapi20170525-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Dypnsapi (20170525) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -59,7 +59,8 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
```

### Comparing `alibabacloud_dypnsapi20170525_py2-1.0.0/alibabacloud_dypnsapi20170525/models.py` & `alibabacloud_dypnsapi20170525_py2-1.0.1/alibabacloud_dypnsapi20170525/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,126 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
 class CreateVerifySchemeRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, scheme_name=None,
-                 app_name=None, os_type=None, pack_name=None, pack_sign=None, bundle_id=None):
-        self.owner_id = owner_id  # type: long
-        self.resource_owner_account = resource_owner_account  # type: str
-        self.resource_owner_id = resource_owner_id  # type: long
-        self.scheme_name = scheme_name  # type: str
+    def __init__(self, app_name=None, auth_type=None, bundle_id=None, cm_api_code=None, ct_api_code=None,
+                 cu_api_code=None, email=None, ip_white_list=None, origin=None, os_type=None, owner_id=None, pack_name=None,
+                 pack_sign=None, resource_owner_account=None, resource_owner_id=None, scene_type=None, scheme_name=None,
+                 sms_sign_name=None, url=None):
         self.app_name = app_name  # type: str
+        self.auth_type = auth_type  # type: str
+        self.bundle_id = bundle_id  # type: str
+        self.cm_api_code = cm_api_code  # type: long
+        self.ct_api_code = ct_api_code  # type: long
+        self.cu_api_code = cu_api_code  # type: long
+        self.email = email  # type: str
+        self.ip_white_list = ip_white_list  # type: str
+        self.origin = origin  # type: str
         self.os_type = os_type  # type: str
+        self.owner_id = owner_id  # type: long
         self.pack_name = pack_name  # type: str
         self.pack_sign = pack_sign  # type: str
-        self.bundle_id = bundle_id  # type: str
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+        self.scene_type = scene_type  # type: str
+        self.scheme_name = scheme_name  # type: str
+        self.sms_sign_name = sms_sign_name  # type: str
+        self.url = url  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateVerifySchemeRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.owner_id is not None:
-            result['OwnerId'] = self.owner_id
-        if self.resource_owner_account is not None:
-            result['ResourceOwnerAccount'] = self.resource_owner_account
-        if self.resource_owner_id is not None:
-            result['ResourceOwnerId'] = self.resource_owner_id
-        if self.scheme_name is not None:
-            result['SchemeName'] = self.scheme_name
         if self.app_name is not None:
             result['AppName'] = self.app_name
+        if self.auth_type is not None:
+            result['AuthType'] = self.auth_type
+        if self.bundle_id is not None:
+            result['BundleId'] = self.bundle_id
+        if self.cm_api_code is not None:
+            result['CmApiCode'] = self.cm_api_code
+        if self.ct_api_code is not None:
+            result['CtApiCode'] = self.ct_api_code
+        if self.cu_api_code is not None:
+            result['CuApiCode'] = self.cu_api_code
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.ip_white_list is not None:
+            result['IpWhiteList'] = self.ip_white_list
+        if self.origin is not None:
+            result['Origin'] = self.origin
         if self.os_type is not None:
             result['OsType'] = self.os_type
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
         if self.pack_name is not None:
             result['PackName'] = self.pack_name
         if self.pack_sign is not None:
             result['PackSign'] = self.pack_sign
-        if self.bundle_id is not None:
-            result['BundleId'] = self.bundle_id
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.scene_type is not None:
+            result['SceneType'] = self.scene_type
+        if self.scheme_name is not None:
+            result['SchemeName'] = self.scheme_name
+        if self.sms_sign_name is not None:
+            result['SmsSignName'] = self.sms_sign_name
+        if self.url is not None:
+            result['Url'] = self.url
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('OwnerId') is not None:
-            self.owner_id = m.get('OwnerId')
-        if m.get('ResourceOwnerAccount') is not None:
-            self.resource_owner_account = m.get('ResourceOwnerAccount')
-        if m.get('ResourceOwnerId') is not None:
-            self.resource_owner_id = m.get('ResourceOwnerId')
-        if m.get('SchemeName') is not None:
-            self.scheme_name = m.get('SchemeName')
         if m.get('AppName') is not None:
             self.app_name = m.get('AppName')
+        if m.get('AuthType') is not None:
+            self.auth_type = m.get('AuthType')
+        if m.get('BundleId') is not None:
+            self.bundle_id = m.get('BundleId')
+        if m.get('CmApiCode') is not None:
+            self.cm_api_code = m.get('CmApiCode')
+        if m.get('CtApiCode') is not None:
+            self.ct_api_code = m.get('CtApiCode')
+        if m.get('CuApiCode') is not None:
+            self.cu_api_code = m.get('CuApiCode')
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('IpWhiteList') is not None:
+            self.ip_white_list = m.get('IpWhiteList')
+        if m.get('Origin') is not None:
+            self.origin = m.get('Origin')
         if m.get('OsType') is not None:
             self.os_type = m.get('OsType')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
         if m.get('PackName') is not None:
             self.pack_name = m.get('PackName')
         if m.get('PackSign') is not None:
             self.pack_sign = m.get('PackSign')
-        if m.get('BundleId') is not None:
-            self.bundle_id = m.get('BundleId')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('SceneType') is not None:
+            self.scene_type = m.get('SceneType')
+        if m.get('SchemeName') is not None:
+            self.scheme_name = m.get('SchemeName')
+        if m.get('SmsSignName') is not None:
+            self.sms_sign_name = m.get('SmsSignName')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
         return self
 
 
 class CreateVerifySchemeResponseBodyGateVerifySchemeDTO(TeaModel):
     def __init__(self, scheme_code=None):
         self.scheme_code = scheme_code  # type: str
 
@@ -89,129 +141,146 @@
         m = m or dict()
         if m.get('SchemeCode') is not None:
             self.scheme_code = m.get('SchemeCode')
         return self
 
 
 class CreateVerifySchemeResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, gate_verify_scheme_dto=None):
+    def __init__(self, code=None, gate_verify_scheme_dto=None, http_status_code=None, message=None, request_id=None,
+                 success=None):
         self.code = code  # type: str
+        self.gate_verify_scheme_dto = gate_verify_scheme_dto  # type: CreateVerifySchemeResponseBodyGateVerifySchemeDTO
+        self.http_status_code = http_status_code  # type: long
         self.message = message  # type: str
         self.request_id = request_id  # type: str
-        self.gate_verify_scheme_dto = gate_verify_scheme_dto  # type: CreateVerifySchemeResponseBodyGateVerifySchemeDTO
+        self.success = success  # type: bool
 
     def validate(self):
         if self.gate_verify_scheme_dto:
             self.gate_verify_scheme_dto.validate()
 
     def to_map(self):
         _map = super(CreateVerifySchemeResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        if self.gate_verify_scheme_dto is not None:
+            result['GateVerifySchemeDTO'] = self.gate_verify_scheme_dto.to_map()
+        if self.http_status_code is not None:
+            result['HttpStatusCode'] = self.http_status_code
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.gate_verify_scheme_dto is not None:
-            result['GateVerifySchemeDTO'] = self.gate_verify_scheme_dto.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('GateVerifySchemeDTO') is not None:
+            temp_model = CreateVerifySchemeResponseBodyGateVerifySchemeDTO()
+            self.gate_verify_scheme_dto = temp_model.from_map(m['GateVerifySchemeDTO'])
+        if m.get('HttpStatusCode') is not None:
+            self.http_status_code = m.get('HttpStatusCode')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('GateVerifySchemeDTO') is not None:
-            temp_model = CreateVerifySchemeResponseBodyGateVerifySchemeDTO()
-            self.gate_verify_scheme_dto = temp_model.from_map(m['GateVerifySchemeDTO'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
         return self
 
 
 class CreateVerifySchemeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: CreateVerifySchemeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateVerifySchemeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateVerifySchemeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteVerifySchemeRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, scheme_code=None,
-                 customer_id=None):
+    def __init__(self, customer_id=None, owner_id=None, resource_owner_account=None, resource_owner_id=None,
+                 scheme_code=None):
+        self.customer_id = customer_id  # type: long
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         self.scheme_code = scheme_code  # type: str
-        self.customer_id = customer_id  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteVerifySchemeRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.customer_id is not None:
+            result['CustomerId'] = self.customer_id
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
         if self.scheme_code is not None:
             result['SchemeCode'] = self.scheme_code
-        if self.customer_id is not None:
-            result['CustomerId'] = self.customer_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('CustomerId') is not None:
+            self.customer_id = m.get('CustomerId')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
         if m.get('SchemeCode') is not None:
             self.scheme_code = m.get('SchemeCode')
-        if m.get('CustomerId') is not None:
-            self.customer_id = m.get('CustomerId')
         return self
 
 
 class DeleteVerifySchemeResponseBody(TeaModel):
     def __init__(self, code=None, message=None, request_id=None, result=None):
         self.code = code  # type: str
         self.message = message  # type: str
@@ -247,88 +316,94 @@
             self.request_id = m.get('RequestId')
         if m.get('Result') is not None:
             self.result = m.get('Result')
         return self
 
 
 class DeleteVerifySchemeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DeleteVerifySchemeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteVerifySchemeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteVerifySchemeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeVerifySchemeRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, scheme_code=None,
-                 customer_id=None):
+    def __init__(self, customer_id=None, owner_id=None, resource_owner_account=None, resource_owner_id=None,
+                 scheme_code=None):
+        self.customer_id = customer_id  # type: long
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
         self.scheme_code = scheme_code  # type: str
-        self.customer_id = customer_id  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeVerifySchemeRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.customer_id is not None:
+            result['CustomerId'] = self.customer_id
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
         if self.scheme_code is not None:
             result['SchemeCode'] = self.scheme_code
-        if self.customer_id is not None:
-            result['CustomerId'] = self.customer_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('CustomerId') is not None:
+            self.customer_id = m.get('CustomerId')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
         if m.get('SchemeCode') is not None:
             self.scheme_code = m.get('SchemeCode')
-        if m.get('CustomerId') is not None:
-            self.customer_id = m.get('CustomerId')
         return self
 
 
 class DescribeVerifySchemeResponseBodySchemeQueryResultDTO(TeaModel):
     def __init__(self, app_encrypt_info=None):
         self.app_encrypt_info = app_encrypt_info  # type: str
 
@@ -390,93 +465,252 @@
         if m.get('SchemeQueryResultDTO') is not None:
             temp_model = DescribeVerifySchemeResponseBodySchemeQueryResultDTO()
             self.scheme_query_result_dto = temp_model.from_map(m['SchemeQueryResultDTO'])
         return self
 
 
 class DescribeVerifySchemeResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: DescribeVerifySchemeResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeVerifySchemeResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeVerifySchemeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetAuthorizationUrlRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, phone_no=None,
-                 scheme_id=None, end_date=None):
+class GetAuthTokenRequest(TeaModel):
+    def __init__(self, origin=None, owner_id=None, resource_owner_account=None, resource_owner_id=None, url=None):
+        self.origin = origin  # type: str
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
+        self.url = url  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetAuthTokenRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.origin is not None:
+            result['Origin'] = self.origin
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.url is not None:
+            result['Url'] = self.url
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Origin') is not None:
+            self.origin = m.get('Origin')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        return self
+
+
+class GetAuthTokenResponseBodyTokenInfo(TeaModel):
+    def __init__(self, access_token=None, jwt_token=None):
+        self.access_token = access_token  # type: str
+        self.jwt_token = jwt_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetAuthTokenResponseBodyTokenInfo, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_token is not None:
+            result['AccessToken'] = self.access_token
+        if self.jwt_token is not None:
+            result['JwtToken'] = self.jwt_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AccessToken') is not None:
+            self.access_token = m.get('AccessToken')
+        if m.get('JwtToken') is not None:
+            self.jwt_token = m.get('JwtToken')
+        return self
+
+
+class GetAuthTokenResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, request_id=None, token_info=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.token_info = token_info  # type: GetAuthTokenResponseBodyTokenInfo
+
+    def validate(self):
+        if self.token_info:
+            self.token_info.validate()
+
+    def to_map(self):
+        _map = super(GetAuthTokenResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.token_info is not None:
+            result['TokenInfo'] = self.token_info.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TokenInfo') is not None:
+            temp_model = GetAuthTokenResponseBodyTokenInfo()
+            self.token_info = temp_model.from_map(m['TokenInfo'])
+        return self
+
+
+class GetAuthTokenResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetAuthTokenResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetAuthTokenResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetAuthTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetAuthorizationUrlRequest(TeaModel):
+    def __init__(self, end_date=None, owner_id=None, phone_no=None, resource_owner_account=None,
+                 resource_owner_id=None, scheme_id=None):
+        self.end_date = end_date  # type: str
+        self.owner_id = owner_id  # type: long
         self.phone_no = phone_no  # type: str
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
         self.scheme_id = scheme_id  # type: long
-        self.end_date = end_date  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAuthorizationUrlRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.end_date is not None:
+            result['EndDate'] = self.end_date
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
+        if self.phone_no is not None:
+            result['PhoneNo'] = self.phone_no
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
-        if self.phone_no is not None:
-            result['PhoneNo'] = self.phone_no
         if self.scheme_id is not None:
             result['SchemeId'] = self.scheme_id
-        if self.end_date is not None:
-            result['EndDate'] = self.end_date
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('EndDate') is not None:
+            self.end_date = m.get('EndDate')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
+        if m.get('PhoneNo') is not None:
+            self.phone_no = m.get('PhoneNo')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
-        if m.get('PhoneNo') is not None:
-            self.phone_no = m.get('PhoneNo')
         if m.get('SchemeId') is not None:
             self.scheme_id = m.get('SchemeId')
-        if m.get('EndDate') is not None:
-            self.end_date = m.get('EndDate')
         return self
 
 
 class GetAuthorizationUrlResponseBodyData(TeaModel):
     def __init__(self, authorization_url=None):
         self.authorization_url = authorization_url  # type: str
 
@@ -497,983 +731,1747 @@
         m = m or dict()
         if m.get('AuthorizationUrl') is not None:
             self.authorization_url = m.get('AuthorizationUrl')
         return self
 
 
 class GetAuthorizationUrlResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, data=None):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
         self.code = code  # type: str
+        self.data = data  # type: GetAuthorizationUrlResponseBodyData
         self.message = message  # type: str
         self.request_id = request_id  # type: str
-        self.data = data  # type: GetAuthorizationUrlResponseBodyData
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
         _map = super(GetAuthorizationUrlResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.data is not None:
-            result['Data'] = self.data.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetAuthorizationUrlResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('Data') is not None:
-            temp_model = GetAuthorizationUrlResponseBodyData()
-            self.data = temp_model.from_map(m['Data'])
         return self
 
 
 class GetAuthorizationUrlResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: GetAuthorizationUrlResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetAuthorizationUrlResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetAuthorizationUrlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetAuthTokenRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, url=None, origin=None):
+class GetFusionAuthTokenRequest(TeaModel):
+    def __init__(self, bundle_id=None, duration_seconds=None, owner_id=None, package_name=None, package_sign=None,
+                 platform=None, resource_owner_account=None, resource_owner_id=None, scheme_code=None):
+        self.bundle_id = bundle_id  # type: str
+        self.duration_seconds = duration_seconds  # type: long
         self.owner_id = owner_id  # type: long
+        self.package_name = package_name  # type: str
+        self.package_sign = package_sign  # type: str
+        self.platform = platform  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
-        self.url = url  # type: str
-        self.origin = origin  # type: str
+        self.scheme_code = scheme_code  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super(GetAuthTokenRequest, self).to_map()
+        _map = super(GetFusionAuthTokenRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.bundle_id is not None:
+            result['BundleId'] = self.bundle_id
+        if self.duration_seconds is not None:
+            result['DurationSeconds'] = self.duration_seconds
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
+        if self.package_name is not None:
+            result['PackageName'] = self.package_name
+        if self.package_sign is not None:
+            result['PackageSign'] = self.package_sign
+        if self.platform is not None:
+            result['Platform'] = self.platform
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
-        if self.url is not None:
-            result['Url'] = self.url
-        if self.origin is not None:
-            result['Origin'] = self.origin
+        if self.scheme_code is not None:
+            result['SchemeCode'] = self.scheme_code
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('BundleId') is not None:
+            self.bundle_id = m.get('BundleId')
+        if m.get('DurationSeconds') is not None:
+            self.duration_seconds = m.get('DurationSeconds')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
+        if m.get('PackageName') is not None:
+            self.package_name = m.get('PackageName')
+        if m.get('PackageSign') is not None:
+            self.package_sign = m.get('PackageSign')
+        if m.get('Platform') is not None:
+            self.platform = m.get('Platform')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
-        if m.get('Url') is not None:
-            self.url = m.get('Url')
-        if m.get('Origin') is not None:
-            self.origin = m.get('Origin')
+        if m.get('SchemeCode') is not None:
+            self.scheme_code = m.get('SchemeCode')
         return self
 
 
-class GetAuthTokenResponseBodyTokenInfo(TeaModel):
-    def __init__(self, access_token=None, jwt_token=None):
+class GetFusionAuthTokenResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, model=None, request_id=None, success=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.model = model  # type: str
+        self.request_id = request_id  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetFusionAuthTokenResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.model is not None:
+            result['Model'] = self.model
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('Model') is not None:
+            self.model = m.get('Model')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetFusionAuthTokenResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetFusionAuthTokenResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetFusionAuthTokenResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetFusionAuthTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetMobileRequest(TeaModel):
+    def __init__(self, access_token=None, out_id=None, owner_id=None, resource_owner_account=None,
+                 resource_owner_id=None):
         self.access_token = access_token  # type: str
-        self.jwt_token = jwt_token  # type: str
+        self.out_id = out_id  # type: str
+        self.owner_id = owner_id  # type: long
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super(GetAuthTokenResponseBodyTokenInfo, self).to_map()
+        _map = super(GetMobileRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.access_token is not None:
             result['AccessToken'] = self.access_token
-        if self.jwt_token is not None:
-            result['JwtToken'] = self.jwt_token
+        if self.out_id is not None:
+            result['OutId'] = self.out_id
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AccessToken') is not None:
             self.access_token = m.get('AccessToken')
-        if m.get('JwtToken') is not None:
-            self.jwt_token = m.get('JwtToken')
+        if m.get('OutId') is not None:
+            self.out_id = m.get('OutId')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
         return self
 
 
-class GetAuthTokenResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, token_info=None):
+class GetMobileResponseBodyGetMobileResultDTO(TeaModel):
+    def __init__(self, mobile=None):
+        self.mobile = mobile  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetMobileResponseBodyGetMobileResultDTO, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.mobile is not None:
+            result['Mobile'] = self.mobile
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
+        return self
+
+
+class GetMobileResponseBody(TeaModel):
+    def __init__(self, code=None, get_mobile_result_dto=None, message=None, request_id=None):
         self.code = code  # type: str
+        self.get_mobile_result_dto = get_mobile_result_dto  # type: GetMobileResponseBodyGetMobileResultDTO
         self.message = message  # type: str
         self.request_id = request_id  # type: str
-        self.token_info = token_info  # type: GetAuthTokenResponseBodyTokenInfo
 
     def validate(self):
-        if self.token_info:
-            self.token_info.validate()
+        if self.get_mobile_result_dto:
+            self.get_mobile_result_dto.validate()
 
     def to_map(self):
-        _map = super(GetAuthTokenResponseBody, self).to_map()
+        _map = super(GetMobileResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        if self.get_mobile_result_dto is not None:
+            result['GetMobileResultDTO'] = self.get_mobile_result_dto.to_map()
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.token_info is not None:
-            result['TokenInfo'] = self.token_info.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('GetMobileResultDTO') is not None:
+            temp_model = GetMobileResponseBodyGetMobileResultDTO()
+            self.get_mobile_result_dto = temp_model.from_map(m['GetMobileResultDTO'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('TokenInfo') is not None:
-            temp_model = GetAuthTokenResponseBodyTokenInfo()
-            self.token_info = temp_model.from_map(m['TokenInfo'])
         return self
 
 
-class GetAuthTokenResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+class GetMobileResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: GetAuthTokenResponseBody
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetMobileResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
-        _map = super(GetAuthTokenResponse, self).to_map()
+        _map = super(GetMobileResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetAuthTokenResponseBody()
+            temp_model = GetMobileResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetCertifyResultRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, token=None):
+class GetPhoneWithTokenRequest(TeaModel):
+    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, sp_token=None):
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
-        self.token = token  # type: str
+        self.sp_token = sp_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super(GetCertifyResultRequest, self).to_map()
+        _map = super(GetPhoneWithTokenRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
-        if self.token is not None:
-            result['Token'] = self.token
+        if self.sp_token is not None:
+            result['SpToken'] = self.sp_token
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
-        if m.get('Token') is not None:
-            self.token = m.get('Token')
+        if m.get('SpToken') is not None:
+            self.sp_token = m.get('SpToken')
         return self
 
 
-class GetCertifyResultResponseBodyData(TeaModel):
-    def __init__(self, material_info=None, identity_info=None, verify_desc=None, verify_result=None,
-                 device_token=None):
-        self.material_info = material_info  # type: str
-        self.identity_info = identity_info  # type: str
-        self.verify_desc = verify_desc  # type: str
-        self.verify_result = verify_result  # type: str
-        self.device_token = device_token  # type: str
+class GetPhoneWithTokenResponseBodyData(TeaModel):
+    def __init__(self, mobile=None):
+        self.mobile = mobile  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super(GetCertifyResultResponseBodyData, self).to_map()
+        _map = super(GetPhoneWithTokenResponseBodyData, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.material_info is not None:
-            result['MaterialInfo'] = self.material_info
-        if self.identity_info is not None:
-            result['IdentityInfo'] = self.identity_info
-        if self.verify_desc is not None:
-            result['VerifyDesc'] = self.verify_desc
-        if self.verify_result is not None:
-            result['VerifyResult'] = self.verify_result
-        if self.device_token is not None:
-            result['DeviceToken'] = self.device_token
+        if self.mobile is not None:
+            result['Mobile'] = self.mobile
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('MaterialInfo') is not None:
-            self.material_info = m.get('MaterialInfo')
-        if m.get('IdentityInfo') is not None:
-            self.identity_info = m.get('IdentityInfo')
-        if m.get('VerifyDesc') is not None:
-            self.verify_desc = m.get('VerifyDesc')
-        if m.get('VerifyResult') is not None:
-            self.verify_result = m.get('VerifyResult')
-        if m.get('DeviceToken') is not None:
-            self.device_token = m.get('DeviceToken')
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
         return self
 
 
-class GetCertifyResultResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, data=None):
+class GetPhoneWithTokenResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
         self.code = code  # type: str
+        self.data = data  # type: GetPhoneWithTokenResponseBodyData
         self.message = message  # type: str
         self.request_id = request_id  # type: str
-        self.data = data  # type: list[GetCertifyResultResponseBodyData]
 
     def validate(self):
         if self.data:
-            for k in self.data:
-                if k:
-                    k.validate()
+            self.data.validate()
 
     def to_map(self):
-        _map = super(GetCertifyResultResponseBody, self).to_map()
+        _map = super(GetPhoneWithTokenResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        result['Data'] = []
-        if self.data is not None:
-            for k in self.data:
-                result['Data'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetPhoneWithTokenResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        self.data = []
-        if m.get('Data') is not None:
-            for k in m.get('Data'):
-                temp_model = GetCertifyResultResponseBodyData()
-                self.data.append(temp_model.from_map(k))
         return self
 
 
-class GetCertifyResultResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+class GetPhoneWithTokenResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: GetCertifyResultResponseBody
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetPhoneWithTokenResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
-        _map = super(GetCertifyResultResponse, self).to_map()
+        _map = super(GetPhoneWithTokenResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetCertifyResultResponseBody()
+            temp_model = GetPhoneWithTokenResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetMobileRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, access_token=None,
-                 out_id=None):
+class GetSmsAuthTokensRequest(TeaModel):
+    def __init__(self, bundle_id=None, expire=None, os_type=None, owner_id=None, package_name=None,
+                 resource_owner_account=None, resource_owner_id=None, scene_code=None, sign_name=None, sms_code_expire=None,
+                 sms_template_code=None):
+        self.bundle_id = bundle_id  # type: str
+        self.expire = expire  # type: long
+        self.os_type = os_type  # type: str
         self.owner_id = owner_id  # type: long
+        self.package_name = package_name  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
-        self.access_token = access_token  # type: str
-        self.out_id = out_id  # type: str
+        self.scene_code = scene_code  # type: str
+        self.sign_name = sign_name  # type: str
+        self.sms_code_expire = sms_code_expire  # type: int
+        self.sms_template_code = sms_template_code  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super(GetMobileRequest, self).to_map()
+        _map = super(GetSmsAuthTokensRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.bundle_id is not None:
+            result['BundleId'] = self.bundle_id
+        if self.expire is not None:
+            result['Expire'] = self.expire
+        if self.os_type is not None:
+            result['OsType'] = self.os_type
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
+        if self.package_name is not None:
+            result['PackageName'] = self.package_name
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
-        if self.access_token is not None:
-            result['AccessToken'] = self.access_token
-        if self.out_id is not None:
-            result['OutId'] = self.out_id
+        if self.scene_code is not None:
+            result['SceneCode'] = self.scene_code
+        if self.sign_name is not None:
+            result['SignName'] = self.sign_name
+        if self.sms_code_expire is not None:
+            result['SmsCodeExpire'] = self.sms_code_expire
+        if self.sms_template_code is not None:
+            result['SmsTemplateCode'] = self.sms_template_code
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('BundleId') is not None:
+            self.bundle_id = m.get('BundleId')
+        if m.get('Expire') is not None:
+            self.expire = m.get('Expire')
+        if m.get('OsType') is not None:
+            self.os_type = m.get('OsType')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
+        if m.get('PackageName') is not None:
+            self.package_name = m.get('PackageName')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
-        if m.get('AccessToken') is not None:
-            self.access_token = m.get('AccessToken')
-        if m.get('OutId') is not None:
-            self.out_id = m.get('OutId')
+        if m.get('SceneCode') is not None:
+            self.scene_code = m.get('SceneCode')
+        if m.get('SignName') is not None:
+            self.sign_name = m.get('SignName')
+        if m.get('SmsCodeExpire') is not None:
+            self.sms_code_expire = m.get('SmsCodeExpire')
+        if m.get('SmsTemplateCode') is not None:
+            self.sms_template_code = m.get('SmsTemplateCode')
         return self
 
 
-class GetMobileResponseBodyGetMobileResultDTO(TeaModel):
-    def __init__(self, mobile=None):
-        self.mobile = mobile  # type: str
+class GetSmsAuthTokensResponseBodyData(TeaModel):
+    def __init__(self, biz_token=None, expire_time=None, sts_access_key_id=None, sts_access_key_secret=None,
+                 sts_token=None):
+        self.biz_token = biz_token  # type: str
+        self.expire_time = expire_time  # type: long
+        self.sts_access_key_id = sts_access_key_id  # type: str
+        self.sts_access_key_secret = sts_access_key_secret  # type: str
+        self.sts_token = sts_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super(GetMobileResponseBodyGetMobileResultDTO, self).to_map()
+        _map = super(GetSmsAuthTokensResponseBodyData, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.mobile is not None:
-            result['Mobile'] = self.mobile
+        if self.biz_token is not None:
+            result['BizToken'] = self.biz_token
+        if self.expire_time is not None:
+            result['ExpireTime'] = self.expire_time
+        if self.sts_access_key_id is not None:
+            result['StsAccessKeyId'] = self.sts_access_key_id
+        if self.sts_access_key_secret is not None:
+            result['StsAccessKeySecret'] = self.sts_access_key_secret
+        if self.sts_token is not None:
+            result['StsToken'] = self.sts_token
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('Mobile') is not None:
-            self.mobile = m.get('Mobile')
+        if m.get('BizToken') is not None:
+            self.biz_token = m.get('BizToken')
+        if m.get('ExpireTime') is not None:
+            self.expire_time = m.get('ExpireTime')
+        if m.get('StsAccessKeyId') is not None:
+            self.sts_access_key_id = m.get('StsAccessKeyId')
+        if m.get('StsAccessKeySecret') is not None:
+            self.sts_access_key_secret = m.get('StsAccessKeySecret')
+        if m.get('StsToken') is not None:
+            self.sts_token = m.get('StsToken')
         return self
 
 
-class GetMobileResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, get_mobile_result_dto=None):
+class GetSmsAuthTokensResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
         self.code = code  # type: str
+        self.data = data  # type: GetSmsAuthTokensResponseBodyData
         self.message = message  # type: str
         self.request_id = request_id  # type: str
-        self.get_mobile_result_dto = get_mobile_result_dto  # type: GetMobileResponseBodyGetMobileResultDTO
 
     def validate(self):
-        if self.get_mobile_result_dto:
-            self.get_mobile_result_dto.validate()
+        if self.data:
+            self.data.validate()
 
     def to_map(self):
-        _map = super(GetMobileResponseBody, self).to_map()
+        _map = super(GetSmsAuthTokensResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.get_mobile_result_dto is not None:
-            result['GetMobileResultDTO'] = self.get_mobile_result_dto.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetSmsAuthTokensResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('GetMobileResultDTO') is not None:
-            temp_model = GetMobileResponseBodyGetMobileResultDTO()
-            self.get_mobile_result_dto = temp_model.from_map(m['GetMobileResultDTO'])
         return self
 
 
-class GetMobileResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+class GetSmsAuthTokensResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: GetMobileResponseBody
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetSmsAuthTokensResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
-        _map = super(GetMobileResponse, self).to_map()
+        _map = super(GetSmsAuthTokensResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetMobileResponseBody()
+            temp_model = GetSmsAuthTokensResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class TwiceTelVerifyRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, since=None,
-                 phone_number=None):
+class QueryGateVerifyBillingPublicRequest(TeaModel):
+    def __init__(self, authentication_type=None, month=None, owner_id=None, resource_owner_account=None):
+        self.authentication_type = authentication_type  # type: int
+        self.month = month  # type: str
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
-        self.resource_owner_id = resource_owner_id  # type: long
-        self.since = since  # type: str
-        self.phone_number = phone_number  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super(TwiceTelVerifyRequest, self).to_map()
+        _map = super(QueryGateVerifyBillingPublicRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.authentication_type is not None:
+            result['AuthenticationType'] = self.authentication_type
+        if self.month is not None:
+            result['Month'] = self.month
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
-        if self.resource_owner_id is not None:
-            result['ResourceOwnerId'] = self.resource_owner_id
-        if self.since is not None:
-            result['Since'] = self.since
-        if self.phone_number is not None:
-            result['PhoneNumber'] = self.phone_number
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('AuthenticationType') is not None:
+            self.authentication_type = m.get('AuthenticationType')
+        if m.get('Month') is not None:
+            self.month = m.get('Month')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
-        if m.get('ResourceOwnerId') is not None:
-            self.resource_owner_id = m.get('ResourceOwnerId')
-        if m.get('Since') is not None:
-            self.since = m.get('Since')
-        if m.get('PhoneNumber') is not None:
-            self.phone_number = m.get('PhoneNumber')
         return self
 
 
-class TwiceTelVerifyResponseBodyTwiceTelVerifyResult(TeaModel):
-    def __init__(self, carrier=None, verify_result=None):
-        self.carrier = carrier  # type: str
-        self.verify_result = verify_result  # type: int
+class QueryGateVerifyBillingPublicResponseBodyDataSceneBillingList(TeaModel):
+    def __init__(self, add=None, amount=None, app_name=None, item_name=None, scene_code=None, scene_name=None,
+                 single_price=None):
+        self.add = add  # type: str
+        self.amount = amount  # type: str
+        self.app_name = app_name  # type: str
+        self.item_name = item_name  # type: str
+        self.scene_code = scene_code  # type: str
+        self.scene_name = scene_name  # type: str
+        self.single_price = single_price  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
-        _map = super(TwiceTelVerifyResponseBodyTwiceTelVerifyResult, self).to_map()
+        _map = super(QueryGateVerifyBillingPublicResponseBodyDataSceneBillingList, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.carrier is not None:
-            result['Carrier'] = self.carrier
-        if self.verify_result is not None:
-            result['VerifyResult'] = self.verify_result
+        if self.add is not None:
+            result['Add'] = self.add
+        if self.amount is not None:
+            result['Amount'] = self.amount
+        if self.app_name is not None:
+            result['AppName'] = self.app_name
+        if self.item_name is not None:
+            result['ItemName'] = self.item_name
+        if self.scene_code is not None:
+            result['SceneCode'] = self.scene_code
+        if self.scene_name is not None:
+            result['SceneName'] = self.scene_name
+        if self.single_price is not None:
+            result['SinglePrice'] = self.single_price
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('Carrier') is not None:
-            self.carrier = m.get('Carrier')
-        if m.get('VerifyResult') is not None:
-            self.verify_result = m.get('VerifyResult')
+        if m.get('Add') is not None:
+            self.add = m.get('Add')
+        if m.get('Amount') is not None:
+            self.amount = m.get('Amount')
+        if m.get('AppName') is not None:
+            self.app_name = m.get('AppName')
+        if m.get('ItemName') is not None:
+            self.item_name = m.get('ItemName')
+        if m.get('SceneCode') is not None:
+            self.scene_code = m.get('SceneCode')
+        if m.get('SceneName') is not None:
+            self.scene_name = m.get('SceneName')
+        if m.get('SinglePrice') is not None:
+            self.single_price = m.get('SinglePrice')
         return self
 
 
-class TwiceTelVerifyResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, twice_tel_verify_result=None):
+class QueryGateVerifyBillingPublicResponseBodyData(TeaModel):
+    def __init__(self, amount_sum=None, scene_billing_list=None):
+        self.amount_sum = amount_sum  # type: str
+        self.scene_billing_list = scene_billing_list  # type: list[QueryGateVerifyBillingPublicResponseBodyDataSceneBillingList]
+
+    def validate(self):
+        if self.scene_billing_list:
+            for k in self.scene_billing_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(QueryGateVerifyBillingPublicResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.amount_sum is not None:
+            result['AmountSum'] = self.amount_sum
+        result['SceneBillingList'] = []
+        if self.scene_billing_list is not None:
+            for k in self.scene_billing_list:
+                result['SceneBillingList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AmountSum') is not None:
+            self.amount_sum = m.get('AmountSum')
+        self.scene_billing_list = []
+        if m.get('SceneBillingList') is not None:
+            for k in m.get('SceneBillingList'):
+                temp_model = QueryGateVerifyBillingPublicResponseBodyDataSceneBillingList()
+                self.scene_billing_list.append(temp_model.from_map(k))
+        return self
+
+
+class QueryGateVerifyBillingPublicResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
         self.code = code  # type: str
+        self.data = data  # type: QueryGateVerifyBillingPublicResponseBodyData
         self.message = message  # type: str
         self.request_id = request_id  # type: str
-        self.twice_tel_verify_result = twice_tel_verify_result  # type: TwiceTelVerifyResponseBodyTwiceTelVerifyResult
 
     def validate(self):
-        if self.twice_tel_verify_result:
-            self.twice_tel_verify_result.validate()
+        if self.data:
+            self.data.validate()
 
     def to_map(self):
-        _map = super(TwiceTelVerifyResponseBody, self).to_map()
+        _map = super(QueryGateVerifyBillingPublicResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.twice_tel_verify_result is not None:
-            result['TwiceTelVerifyResult'] = self.twice_tel_verify_result.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = QueryGateVerifyBillingPublicResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('TwiceTelVerifyResult') is not None:
-            temp_model = TwiceTelVerifyResponseBodyTwiceTelVerifyResult()
-            self.twice_tel_verify_result = temp_model.from_map(m['TwiceTelVerifyResult'])
         return self
 
 
-class TwiceTelVerifyResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+class QueryGateVerifyBillingPublicResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
-        self.body = body  # type: TwiceTelVerifyResponseBody
+        self.status_code = status_code  # type: int
+        self.body = body  # type: QueryGateVerifyBillingPublicResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
-        _map = super(TwiceTelVerifyResponse, self).to_map()
+        _map = super(QueryGateVerifyBillingPublicResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = TwiceTelVerifyResponseBody()
+            temp_model = QueryGateVerifyBillingPublicResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class VerifyMobileRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, access_code=None,
-                 phone_number=None, out_id=None):
+class QueryGateVerifyStatisticPublicRequest(TeaModel):
+    def __init__(self, authentication_type=None, end_date=None, os_type=None, owner_id=None,
+                 resource_owner_account=None, scene_code=None, start_date=None):
+        self.authentication_type = authentication_type  # type: int
+        self.end_date = end_date  # type: str
+        self.os_type = os_type  # type: str
         self.owner_id = owner_id  # type: long
         self.resource_owner_account = resource_owner_account  # type: str
-        self.resource_owner_id = resource_owner_id  # type: long
+        self.scene_code = scene_code  # type: str
+        self.start_date = start_date  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryGateVerifyStatisticPublicRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.authentication_type is not None:
+            result['AuthenticationType'] = self.authentication_type
+        if self.end_date is not None:
+            result['EndDate'] = self.end_date
+        if self.os_type is not None:
+            result['OsType'] = self.os_type
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.scene_code is not None:
+            result['SceneCode'] = self.scene_code
+        if self.start_date is not None:
+            result['StartDate'] = self.start_date
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AuthenticationType') is not None:
+            self.authentication_type = m.get('AuthenticationType')
+        if m.get('EndDate') is not None:
+            self.end_date = m.get('EndDate')
+        if m.get('OsType') is not None:
+            self.os_type = m.get('OsType')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('SceneCode') is not None:
+            self.scene_code = m.get('SceneCode')
+        if m.get('StartDate') is not None:
+            self.start_date = m.get('StartDate')
+        return self
+
+
+class QueryGateVerifyStatisticPublicResponseBodyDataDayStatistic(TeaModel):
+    def __init__(self, statistic_date_str=None, total_fail=None, total_success=None, total_unknown=None):
+        self.statistic_date_str = statistic_date_str  # type: str
+        self.total_fail = total_fail  # type: long
+        self.total_success = total_success  # type: long
+        self.total_unknown = total_unknown  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryGateVerifyStatisticPublicResponseBodyDataDayStatistic, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.statistic_date_str is not None:
+            result['StatisticDateStr'] = self.statistic_date_str
+        if self.total_fail is not None:
+            result['TotalFail'] = self.total_fail
+        if self.total_success is not None:
+            result['TotalSuccess'] = self.total_success
+        if self.total_unknown is not None:
+            result['TotalUnknown'] = self.total_unknown
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('StatisticDateStr') is not None:
+            self.statistic_date_str = m.get('StatisticDateStr')
+        if m.get('TotalFail') is not None:
+            self.total_fail = m.get('TotalFail')
+        if m.get('TotalSuccess') is not None:
+            self.total_success = m.get('TotalSuccess')
+        if m.get('TotalUnknown') is not None:
+            self.total_unknown = m.get('TotalUnknown')
+        return self
+
+
+class QueryGateVerifyStatisticPublicResponseBodyData(TeaModel):
+    def __init__(self, day_statistic=None, total=None, total_fail=None, total_success=None, total_unknown=None):
+        self.day_statistic = day_statistic  # type: list[QueryGateVerifyStatisticPublicResponseBodyDataDayStatistic]
+        self.total = total  # type: long
+        self.total_fail = total_fail  # type: long
+        self.total_success = total_success  # type: long
+        self.total_unknown = total_unknown  # type: long
+
+    def validate(self):
+        if self.day_statistic:
+            for k in self.day_statistic:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(QueryGateVerifyStatisticPublicResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DayStatistic'] = []
+        if self.day_statistic is not None:
+            for k in self.day_statistic:
+                result['DayStatistic'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['Total'] = self.total
+        if self.total_fail is not None:
+            result['TotalFail'] = self.total_fail
+        if self.total_success is not None:
+            result['TotalSuccess'] = self.total_success
+        if self.total_unknown is not None:
+            result['TotalUnknown'] = self.total_unknown
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.day_statistic = []
+        if m.get('DayStatistic') is not None:
+            for k in m.get('DayStatistic'):
+                temp_model = QueryGateVerifyStatisticPublicResponseBodyDataDayStatistic()
+                self.day_statistic.append(temp_model.from_map(k))
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        if m.get('TotalFail') is not None:
+            self.total_fail = m.get('TotalFail')
+        if m.get('TotalSuccess') is not None:
+            self.total_success = m.get('TotalSuccess')
+        if m.get('TotalUnknown') is not None:
+            self.total_unknown = m.get('TotalUnknown')
+        return self
+
+
+class QueryGateVerifyStatisticPublicResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
+        self.code = code  # type: str
+        self.data = data  # type: QueryGateVerifyStatisticPublicResponseBodyData
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(QueryGateVerifyStatisticPublicResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = QueryGateVerifyStatisticPublicResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class QueryGateVerifyStatisticPublicResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: QueryGateVerifyStatisticPublicResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(QueryGateVerifyStatisticPublicResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryGateVerifyStatisticPublicResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class VerifyMobileRequest(TeaModel):
+    def __init__(self, access_code=None, out_id=None, owner_id=None, phone_number=None, resource_owner_account=None,
+                 resource_owner_id=None):
         self.access_code = access_code  # type: str
-        self.phone_number = phone_number  # type: str
         self.out_id = out_id  # type: str
+        self.owner_id = owner_id  # type: long
+        self.phone_number = phone_number  # type: str
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(VerifyMobileRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.access_code is not None:
+            result['AccessCode'] = self.access_code
+        if self.out_id is not None:
+            result['OutId'] = self.out_id
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
-        if self.access_code is not None:
-            result['AccessCode'] = self.access_code
-        if self.phone_number is not None:
-            result['PhoneNumber'] = self.phone_number
-        if self.out_id is not None:
-            result['OutId'] = self.out_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('AccessCode') is not None:
+            self.access_code = m.get('AccessCode')
+        if m.get('OutId') is not None:
+            self.out_id = m.get('OutId')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
-        if m.get('AccessCode') is not None:
-            self.access_code = m.get('AccessCode')
-        if m.get('PhoneNumber') is not None:
-            self.phone_number = m.get('PhoneNumber')
-        if m.get('OutId') is not None:
-            self.out_id = m.get('OutId')
         return self
 
 
 class VerifyMobileResponseBodyGateVerifyResultDTO(TeaModel):
-    def __init__(self, verify_result=None, verify_id=None):
-        self.verify_result = verify_result  # type: str
+    def __init__(self, verify_id=None, verify_result=None):
         self.verify_id = verify_id  # type: str
+        self.verify_result = verify_result  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(VerifyMobileResponseBodyGateVerifyResultDTO, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.verify_result is not None:
-            result['VerifyResult'] = self.verify_result
         if self.verify_id is not None:
             result['VerifyId'] = self.verify_id
+        if self.verify_result is not None:
+            result['VerifyResult'] = self.verify_result
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('VerifyResult') is not None:
-            self.verify_result = m.get('VerifyResult')
         if m.get('VerifyId') is not None:
             self.verify_id = m.get('VerifyId')
+        if m.get('VerifyResult') is not None:
+            self.verify_result = m.get('VerifyResult')
         return self
 
 
 class VerifyMobileResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, gate_verify_result_dto=None):
+    def __init__(self, code=None, gate_verify_result_dto=None, message=None, request_id=None):
         self.code = code  # type: str
+        self.gate_verify_result_dto = gate_verify_result_dto  # type: VerifyMobileResponseBodyGateVerifyResultDTO
         self.message = message  # type: str
         self.request_id = request_id  # type: str
-        self.gate_verify_result_dto = gate_verify_result_dto  # type: VerifyMobileResponseBodyGateVerifyResultDTO
 
     def validate(self):
         if self.gate_verify_result_dto:
             self.gate_verify_result_dto.validate()
 
     def to_map(self):
         _map = super(VerifyMobileResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        if self.gate_verify_result_dto is not None:
+            result['GateVerifyResultDTO'] = self.gate_verify_result_dto.to_map()
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.gate_verify_result_dto is not None:
-            result['GateVerifyResultDTO'] = self.gate_verify_result_dto.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('GateVerifyResultDTO') is not None:
+            temp_model = VerifyMobileResponseBodyGateVerifyResultDTO()
+            self.gate_verify_result_dto = temp_model.from_map(m['GateVerifyResultDTO'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('GateVerifyResultDTO') is not None:
-            temp_model = VerifyMobileResponseBodyGateVerifyResultDTO()
-            self.gate_verify_result_dto = temp_model.from_map(m['GateVerifyResultDTO'])
         return self
 
 
 class VerifyMobileResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: VerifyMobileResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(VerifyMobileResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = VerifyMobileResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class VerifyPhoneWithTokenRequest(TeaModel):
-    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, phone_number=None,
+    def __init__(self, owner_id=None, phone_number=None, resource_owner_account=None, resource_owner_id=None,
                  sp_token=None):
         self.owner_id = owner_id  # type: long
+        self.phone_number = phone_number  # type: str
         self.resource_owner_account = resource_owner_account  # type: str
         self.resource_owner_id = resource_owner_id  # type: long
-        self.phone_number = phone_number  # type: str
         self.sp_token = sp_token  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(VerifyPhoneWithTokenRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
         if self.resource_owner_account is not None:
             result['ResourceOwnerAccount'] = self.resource_owner_account
         if self.resource_owner_id is not None:
             result['ResourceOwnerId'] = self.resource_owner_id
-        if self.phone_number is not None:
-            result['PhoneNumber'] = self.phone_number
         if self.sp_token is not None:
             result['SpToken'] = self.sp_token
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
         if m.get('ResourceOwnerAccount') is not None:
             self.resource_owner_account = m.get('ResourceOwnerAccount')
         if m.get('ResourceOwnerId') is not None:
             self.resource_owner_id = m.get('ResourceOwnerId')
-        if m.get('PhoneNumber') is not None:
-            self.phone_number = m.get('PhoneNumber')
         if m.get('SpToken') is not None:
             self.sp_token = m.get('SpToken')
         return self
 
 
 class VerifyPhoneWithTokenResponseBodyGateVerify(TeaModel):
-    def __init__(self, verify_result=None, verify_id=None):
-        self.verify_result = verify_result  # type: str
+    def __init__(self, verify_id=None, verify_result=None):
         self.verify_id = verify_id  # type: str
+        self.verify_result = verify_result  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(VerifyPhoneWithTokenResponseBodyGateVerify, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.verify_result is not None:
-            result['VerifyResult'] = self.verify_result
         if self.verify_id is not None:
             result['VerifyId'] = self.verify_id
+        if self.verify_result is not None:
+            result['VerifyResult'] = self.verify_result
         return result
 
     def from_map(self, m=None):
         m = m or dict()
-        if m.get('VerifyResult') is not None:
-            self.verify_result = m.get('VerifyResult')
         if m.get('VerifyId') is not None:
             self.verify_id = m.get('VerifyId')
+        if m.get('VerifyResult') is not None:
+            self.verify_result = m.get('VerifyResult')
         return self
 
 
 class VerifyPhoneWithTokenResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, gate_verify=None):
+    def __init__(self, code=None, gate_verify=None, message=None, request_id=None):
         self.code = code  # type: str
+        self.gate_verify = gate_verify  # type: VerifyPhoneWithTokenResponseBodyGateVerify
         self.message = message  # type: str
         self.request_id = request_id  # type: str
-        self.gate_verify = gate_verify  # type: VerifyPhoneWithTokenResponseBodyGateVerify
 
     def validate(self):
         if self.gate_verify:
             self.gate_verify.validate()
 
     def to_map(self):
         _map = super(VerifyPhoneWithTokenResponseBody, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        if self.gate_verify is not None:
+            result['GateVerify'] = self.gate_verify.to_map()
         if self.message is not None:
             result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.gate_verify is not None:
-            result['GateVerify'] = self.gate_verify.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        if m.get('GateVerify') is not None:
+            temp_model = VerifyPhoneWithTokenResponseBodyGateVerify()
+            self.gate_verify = temp_model.from_map(m['GateVerify'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('GateVerify') is not None:
-            temp_model = VerifyPhoneWithTokenResponseBodyGateVerify()
-            self.gate_verify = temp_model.from_map(m['GateVerify'])
         return self
 
 
 class VerifyPhoneWithTokenResponse(TeaModel):
-    def __init__(self, headers=None, body=None):
+    def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
         self.body = body  # type: VerifyPhoneWithTokenResponseBody
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
         self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(VerifyPhoneWithTokenResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = VerifyPhoneWithTokenResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class VerifySmsCodeRequest(TeaModel):
+    def __init__(self, phone_number=None, sms_code=None, sms_token=None):
+        self.phone_number = phone_number  # type: str
+        self.sms_code = sms_code  # type: str
+        self.sms_token = sms_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VerifySmsCodeRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
+        if self.sms_code is not None:
+            result['SmsCode'] = self.sms_code
+        if self.sms_token is not None:
+            result['SmsToken'] = self.sms_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
+        if m.get('SmsCode') is not None:
+            self.sms_code = m.get('SmsCode')
+        if m.get('SmsToken') is not None:
+            self.sms_token = m.get('SmsToken')
+        return self
+
+
+class VerifySmsCodeResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
+        self.code = code  # type: str
+        self.data = data  # type: bool
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VerifySmsCodeResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class VerifySmsCodeResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: VerifySmsCodeResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(VerifySmsCodeResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = VerifySmsCodeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class VerifyWithFusionAuthTokenRequest(TeaModel):
+    def __init__(self, owner_id=None, resource_owner_account=None, resource_owner_id=None, verify_token=None):
+        self.owner_id = owner_id  # type: long
+        self.resource_owner_account = resource_owner_account  # type: str
+        self.resource_owner_id = resource_owner_id  # type: long
+        self.verify_token = verify_token  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VerifyWithFusionAuthTokenRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.verify_token is not None:
+            result['VerifyToken'] = self.verify_token
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('VerifyToken') is not None:
+            self.verify_token = m.get('VerifyToken')
+        return self
+
+
+class VerifyWithFusionAuthTokenResponseBodyModel(TeaModel):
+    def __init__(self, phone_number=None, phone_score=None, verify_result=None):
+        self.phone_number = phone_number  # type: str
+        self.phone_score = phone_score  # type: long
+        self.verify_result = verify_result  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VerifyWithFusionAuthTokenResponseBodyModel, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.phone_number is not None:
+            result['PhoneNumber'] = self.phone_number
+        if self.phone_score is not None:
+            result['PhoneScore'] = self.phone_score
+        if self.verify_result is not None:
+            result['VerifyResult'] = self.verify_result
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('PhoneNumber') is not None:
+            self.phone_number = m.get('PhoneNumber')
+        if m.get('PhoneScore') is not None:
+            self.phone_score = m.get('PhoneScore')
+        if m.get('VerifyResult') is not None:
+            self.verify_result = m.get('VerifyResult')
+        return self
+
+
+class VerifyWithFusionAuthTokenResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, model=None, request_id=None, success=None):
+        self.code = code  # type: str
+        self.message = message  # type: str
+        self.model = model  # type: VerifyWithFusionAuthTokenResponseBodyModel
+        self.request_id = request_id  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        if self.model:
+            self.model.validate()
+
+    def to_map(self):
+        _map = super(VerifyWithFusionAuthTokenResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.model is not None:
+            result['Model'] = self.model.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('Model') is not None:
+            temp_model = VerifyWithFusionAuthTokenResponseBodyModel()
+            self.model = temp_model.from_map(m['Model'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class VerifyWithFusionAuthTokenResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: VerifyWithFusionAuthTokenResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(VerifyWithFusionAuthTokenResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = VerifyWithFusionAuthTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_dypnsapi20170525_py2-1.0.0/README-CN.md` & `alibabacloud_dypnsapi20170525_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dypnsapi20170525_py2-1.0.0/LICENSE` & `alibabacloud_dypnsapi20170525_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dypnsapi20170525_py2-1.0.0/README.md` & `alibabacloud_dypnsapi20170525_py2-1.0.1/README.md`

 * *Files identical despite different names*

