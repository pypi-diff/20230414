# Comparing `tmp/alibabacloud_dypnsapi20170525-1.0.8.tar.gz` & `tmp/alibabacloud_dypnsapi20170525-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dypnsapi20170525-1.0.8.tar", last modified: Tue Dec 27 06:05:41 2022, max compression
+gzip compressed data, was "dist/alibabacloud_dypnsapi20170525-1.0.9.tar", last modified: Fri Apr 14 08:44:43 2023, max compression
```

## Comparing `alibabacloud_dypnsapi20170525-1.0.8.tar` & `alibabacloud_dypnsapi20170525-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      465 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52320 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525/client.py
--rw-r--r--   0 root         (0) root         (0)    79943 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2022-12-27 06:05:41.000000 alibabacloud_dypnsapi20170525-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      533 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60358 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525/client.py
+-rw-r--r--   0 root         (0) root         (0)    91449 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-04-14 08:44:43.000000 alibabacloud_dypnsapi20170525-1.0.9/setup.py
```

### Comparing `alibabacloud_dypnsapi20170525-1.0.8/LICENSE` & `alibabacloud_dypnsapi20170525-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dypnsapi20170525-1.0.8/PKG-INFO` & `alibabacloud_dypnsapi20170525-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dypnsapi20170525
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Dypnsapi (20170525) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dypnsapi20170525-1.0.8/README-CN.md` & `alibabacloud_dypnsapi20170525-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dypnsapi20170525-1.0.8/README.md` & `alibabacloud_dypnsapi20170525-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525/client.py` & `alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -528,14 +528,116 @@
     async def get_authorization_url_async(
         self,
         request: dypnsapi_20170525_models.GetAuthorizationUrlRequest,
     ) -> dypnsapi_20170525_models.GetAuthorizationUrlResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_authorization_url_with_options_async(request, runtime)
 
+    def get_fusion_auth_token_with_options(
+        self,
+        request: dypnsapi_20170525_models.GetFusionAuthTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dypnsapi_20170525_models.GetFusionAuthTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.bundle_id):
+            query['BundleId'] = request.bundle_id
+        if not UtilClient.is_unset(request.duration_seconds):
+            query['DurationSeconds'] = request.duration_seconds
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.package_name):
+            query['PackageName'] = request.package_name
+        if not UtilClient.is_unset(request.package_sign):
+            query['PackageSign'] = request.package_sign
+        if not UtilClient.is_unset(request.platform):
+            query['Platform'] = request.platform
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.scheme_code):
+            query['SchemeCode'] = request.scheme_code
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetFusionAuthToken',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dypnsapi_20170525_models.GetFusionAuthTokenResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_fusion_auth_token_with_options_async(
+        self,
+        request: dypnsapi_20170525_models.GetFusionAuthTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dypnsapi_20170525_models.GetFusionAuthTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.bundle_id):
+            query['BundleId'] = request.bundle_id
+        if not UtilClient.is_unset(request.duration_seconds):
+            query['DurationSeconds'] = request.duration_seconds
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.package_name):
+            query['PackageName'] = request.package_name
+        if not UtilClient.is_unset(request.package_sign):
+            query['PackageSign'] = request.package_sign
+        if not UtilClient.is_unset(request.platform):
+            query['Platform'] = request.platform
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.scheme_code):
+            query['SchemeCode'] = request.scheme_code
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetFusionAuthToken',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dypnsapi_20170525_models.GetFusionAuthTokenResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_fusion_auth_token(
+        self,
+        request: dypnsapi_20170525_models.GetFusionAuthTokenRequest,
+    ) -> dypnsapi_20170525_models.GetFusionAuthTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_fusion_auth_token_with_options(request, runtime)
+
+    async def get_fusion_auth_token_async(
+        self,
+        request: dypnsapi_20170525_models.GetFusionAuthTokenRequest,
+    ) -> dypnsapi_20170525_models.GetFusionAuthTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_fusion_auth_token_with_options_async(request, runtime)
+
     def get_mobile_with_options(
         self,
         request: dypnsapi_20170525_models.GetMobileRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dypnsapi_20170525_models.GetMobileResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1235,7 +1337,89 @@
 
     async def verify_sms_code_async(
         self,
         request: dypnsapi_20170525_models.VerifySmsCodeRequest,
     ) -> dypnsapi_20170525_models.VerifySmsCodeResponse:
         runtime = util_models.RuntimeOptions()
         return await self.verify_sms_code_with_options_async(request, runtime)
+
+    def verify_with_fusion_auth_token_with_options(
+        self,
+        request: dypnsapi_20170525_models.VerifyWithFusionAuthTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dypnsapi_20170525_models.VerifyWithFusionAuthTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.verify_token):
+            query['VerifyToken'] = request.verify_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='VerifyWithFusionAuthToken',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dypnsapi_20170525_models.VerifyWithFusionAuthTokenResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def verify_with_fusion_auth_token_with_options_async(
+        self,
+        request: dypnsapi_20170525_models.VerifyWithFusionAuthTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dypnsapi_20170525_models.VerifyWithFusionAuthTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.verify_token):
+            query['VerifyToken'] = request.verify_token
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='VerifyWithFusionAuthToken',
+            version='2017-05-25',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dypnsapi_20170525_models.VerifyWithFusionAuthTokenResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def verify_with_fusion_auth_token(
+        self,
+        request: dypnsapi_20170525_models.VerifyWithFusionAuthTokenRequest,
+    ) -> dypnsapi_20170525_models.VerifyWithFusionAuthTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.verify_with_fusion_auth_token_with_options(request, runtime)
+
+    async def verify_with_fusion_auth_token_async(
+        self,
+        request: dypnsapi_20170525_models.VerifyWithFusionAuthTokenRequest,
+    ) -> dypnsapi_20170525_models.VerifyWithFusionAuthTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.verify_with_fusion_auth_token_with_options_async(request, runtime)
```

### Comparing `alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525/models.py` & `alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -924,14 +924,184 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetAuthorizationUrlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetFusionAuthTokenRequest(TeaModel):
+    def __init__(
+        self,
+        bundle_id: str = None,
+        duration_seconds: int = None,
+        owner_id: int = None,
+        package_name: str = None,
+        package_sign: str = None,
+        platform: str = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+        scheme_code: str = None,
+    ):
+        self.bundle_id = bundle_id
+        self.duration_seconds = duration_seconds
+        self.owner_id = owner_id
+        self.package_name = package_name
+        self.package_sign = package_sign
+        self.platform = platform
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
+        self.scheme_code = scheme_code
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.bundle_id is not None:
+            result['BundleId'] = self.bundle_id
+        if self.duration_seconds is not None:
+            result['DurationSeconds'] = self.duration_seconds
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.package_name is not None:
+            result['PackageName'] = self.package_name
+        if self.package_sign is not None:
+            result['PackageSign'] = self.package_sign
+        if self.platform is not None:
+            result['Platform'] = self.platform
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        if self.scheme_code is not None:
+            result['SchemeCode'] = self.scheme_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BundleId') is not None:
+            self.bundle_id = m.get('BundleId')
+        if m.get('DurationSeconds') is not None:
+            self.duration_seconds = m.get('DurationSeconds')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('PackageName') is not None:
+            self.package_name = m.get('PackageName')
+        if m.get('PackageSign') is not None:
+            self.package_sign = m.get('PackageSign')
+        if m.get('Platform') is not None:
+            self.platform = m.get('Platform')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        if m.get('SchemeCode') is not None:
+            self.scheme_code = m.get('SchemeCode')
+        return self
+
+
+class GetFusionAuthTokenResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        model: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.model = model
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetFusionAuthTokenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
 class GetMobileRequest(TeaModel):
     def __init__(
         self,
         access_token: str = None,
         out_id: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
@@ -2467,7 +2637,188 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = VerifySmsCodeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class VerifyWithFusionAuthTokenRequest(TeaModel):
+    def __init__(
+        self,
+        owner_id: int = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+        verify_token: str = None,
+    ):
+        self.owner_id = owner_id
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
+        self.verify_token = verify_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        phone_number: str = None,
+        phone_score: int = None,
+        verify_result: str = None,
+    ):
+        self.phone_number = phone_number
+        self.phone_score = phone_score
+        self.verify_result = verify_result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+        model: VerifyWithFusionAuthTokenResponseBodyModel = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.model = model
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.model:
+            self.model.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: VerifyWithFusionAuthTokenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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

### Comparing `alibabacloud_dypnsapi20170525-1.0.8/alibabacloud_dypnsapi20170525.egg-info/PKG-INFO` & `alibabacloud_dypnsapi20170525-1.0.9/alibabacloud_dypnsapi20170525.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dypnsapi20170525
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Dypnsapi (20170525) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dypnsapi20170525-1.0.8/setup.py` & `alibabacloud_dypnsapi20170525-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dypnsapi20170525.
 
-Created on 27/12/2022
+Created on 14/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dypnsapi20170525"
 NAME = "alibabacloud_dypnsapi20170525" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dypnsapi (20170525) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

