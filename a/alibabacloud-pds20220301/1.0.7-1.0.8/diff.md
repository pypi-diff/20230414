# Comparing `tmp/alibabacloud_pds20220301-1.0.7.tar.gz` & `tmp/alibabacloud_pds20220301-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pds20220301-1.0.7.tar", last modified: Thu Apr  6 05:57:58 2023, max compression
+gzip compressed data, was "dist/alibabacloud_pds20220301-1.0.8.tar", last modified: Fri Apr 14 06:23:11 2023, max compression
```

## Comparing `alibabacloud_pds20220301-1.0.7.tar` & `alibabacloud_pds20220301-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      441 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301/__init__.py
--rw-r--r--   0 root         (0) root         (0)   292767 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301/client.py
--rw-r--r--   0 root         (0) root         (0)   391576 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      193 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2655 2023-04-06 05:57:58.000000 alibabacloud_pds20220301-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   300379 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301/client.py
+-rw-r--r--   0 root         (0) root         (0)   404832 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      193 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-14 06:23:11.000000 alibabacloud_pds20220301-1.0.8/setup.py
```

### Comparing `alibabacloud_pds20220301-1.0.7/LICENSE` & `alibabacloud_pds20220301-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pds20220301-1.0.7/PKG-INFO` & `alibabacloud_pds20220301-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pds20220301
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud pds (20220301) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pds20220301-1.0.7/README-CN.md` & `alibabacloud_pds20220301-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pds20220301-1.0.7/README.md` & `alibabacloud_pds20220301-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301/client.py` & `alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,14 +557,18 @@
         body = {}
         if not UtilClient.is_unset(request.auto_rename):
             body['auto_rename'] = request.auto_rename
         if not UtilClient.is_unset(request.drive_id):
             body['drive_id'] = request.drive_id
         if not UtilClient.is_unset(request.file_id):
             body['file_id'] = request.file_id
+        if not UtilClient.is_unset(request.share_id):
+            body['share_id'] = request.share_id
+        if not UtilClient.is_unset(request.to_drive_id):
+            body['to_drive_id'] = request.to_drive_id
         if not UtilClient.is_unset(request.to_parent_file_id):
             body['to_parent_file_id'] = request.to_parent_file_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -593,14 +597,18 @@
         body = {}
         if not UtilClient.is_unset(request.auto_rename):
             body['auto_rename'] = request.auto_rename
         if not UtilClient.is_unset(request.drive_id):
             body['drive_id'] = request.drive_id
         if not UtilClient.is_unset(request.file_id):
             body['file_id'] = request.file_id
+        if not UtilClient.is_unset(request.share_id):
+            body['share_id'] = request.share_id
+        if not UtilClient.is_unset(request.to_drive_id):
+            body['to_drive_id'] = request.to_drive_id
         if not UtilClient.is_unset(request.to_parent_file_id):
             body['to_parent_file_id'] = request.to_parent_file_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -1107,14 +1115,16 @@
             body['expiration'] = request.expiration
         if not UtilClient.is_unset(request.file_id_list):
             body['file_id_list'] = request.file_id_list
         if not UtilClient.is_unset(request.preview_limit):
             body['preview_limit'] = request.preview_limit
         if not UtilClient.is_unset(request.save_limit):
             body['save_limit'] = request.save_limit
+        if not UtilClient.is_unset(request.share_all_files):
+            body['share_all_files'] = request.share_all_files
         if not UtilClient.is_unset(request.share_name):
             body['share_name'] = request.share_name
         if not UtilClient.is_unset(request.share_pwd):
             body['share_pwd'] = request.share_pwd
         if not UtilClient.is_unset(request.user_id):
             body['user_id'] = request.user_id
         req = open_api_models.OpenApiRequest(
@@ -1161,14 +1171,16 @@
             body['expiration'] = request.expiration
         if not UtilClient.is_unset(request.file_id_list):
             body['file_id_list'] = request.file_id_list
         if not UtilClient.is_unset(request.preview_limit):
             body['preview_limit'] = request.preview_limit
         if not UtilClient.is_unset(request.save_limit):
             body['save_limit'] = request.save_limit
+        if not UtilClient.is_unset(request.share_all_files):
+            body['share_all_files'] = request.share_all_files
         if not UtilClient.is_unset(request.share_name):
             body['share_name'] = request.share_name
         if not UtilClient.is_unset(request.share_pwd):
             body['share_pwd'] = request.share_pwd
         if not UtilClient.is_unset(request.user_id):
             body['user_id'] = request.user_id
         req = open_api_models.OpenApiRequest(
@@ -1319,14 +1331,98 @@
         self,
         request: pds_20220301_models.CreateUserRequest,
     ) -> pds_20220301_models.CreateUserResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_user_with_options_async(request, headers, runtime)
 
+    def csi_get_file_info_with_options(
+        self,
+        request: pds_20220301_models.CsiGetFileInfoRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pds_20220301_models.CsiGetFileInfoResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.drive_id):
+            body['drive_id'] = request.drive_id
+        if not UtilClient.is_unset(request.file_id):
+            body['file_id'] = request.file_id
+        if not UtilClient.is_unset(request.url_expire_sec):
+            body['url_expire_sec'] = request.url_expire_sec
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CsiGetFileInfo',
+            version='2022-03-01',
+            protocol='HTTPS',
+            pathname=f'/v2/csi/get_file_info',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pds_20220301_models.CsiGetFileInfoResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def csi_get_file_info_with_options_async(
+        self,
+        request: pds_20220301_models.CsiGetFileInfoRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pds_20220301_models.CsiGetFileInfoResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.drive_id):
+            body['drive_id'] = request.drive_id
+        if not UtilClient.is_unset(request.file_id):
+            body['file_id'] = request.file_id
+        if not UtilClient.is_unset(request.url_expire_sec):
+            body['url_expire_sec'] = request.url_expire_sec
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CsiGetFileInfo',
+            version='2022-03-01',
+            protocol='HTTPS',
+            pathname=f'/v2/csi/get_file_info',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pds_20220301_models.CsiGetFileInfoResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def csi_get_file_info(
+        self,
+        request: pds_20220301_models.CsiGetFileInfoRequest,
+    ) -> pds_20220301_models.CsiGetFileInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.csi_get_file_info_with_options(request, headers, runtime)
+
+    async def csi_get_file_info_async(
+        self,
+        request: pds_20220301_models.CsiGetFileInfoRequest,
+    ) -> pds_20220301_models.CsiGetFileInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.csi_get_file_info_with_options_async(request, headers, runtime)
+
     def delete_domain_with_options(
         self,
         request: pds_20220301_models.DeleteDomainRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pds_20220301_models.DeleteDomainResponse:
         UtilClient.validate_model(request)
@@ -1883,14 +1979,16 @@
             body['drive_id'] = request.drive_id
         if not UtilClient.is_unset(request.file_id):
             body['file_id'] = request.file_id
         if not UtilClient.is_unset(request.image_thumbnail_process):
             body['image_thumbnail_process'] = request.image_thumbnail_process
         if not UtilClient.is_unset(request.office_thumbnail_process):
             body['office_thumbnail_process'] = request.office_thumbnail_process
+        if not UtilClient.is_unset(request.share_id):
+            body['share_id'] = request.share_id
         if not UtilClient.is_unset(request.video_thumbnail_process):
             body['video_thumbnail_process'] = request.video_thumbnail_process
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -1921,14 +2019,16 @@
             body['drive_id'] = request.drive_id
         if not UtilClient.is_unset(request.file_id):
             body['file_id'] = request.file_id
         if not UtilClient.is_unset(request.image_thumbnail_process):
             body['image_thumbnail_process'] = request.image_thumbnail_process
         if not UtilClient.is_unset(request.office_thumbnail_process):
             body['office_thumbnail_process'] = request.office_thumbnail_process
+        if not UtilClient.is_unset(request.share_id):
+            body['share_id'] = request.share_id
         if not UtilClient.is_unset(request.video_thumbnail_process):
             body['video_thumbnail_process'] = request.video_thumbnail_process
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -2623,14 +2723,16 @@
             body['drive_id'] = request.drive_id
         if not UtilClient.is_unset(request.expire_sec):
             body['expire_sec'] = request.expire_sec
         if not UtilClient.is_unset(request.file_id):
             body['file_id'] = request.file_id
         if not UtilClient.is_unset(request.file_name):
             body['file_name'] = request.file_name
+        if not UtilClient.is_unset(request.share_id):
+            body['share_id'] = request.share_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='GetDownloadUrl',
             version='2022-03-01',
@@ -2659,14 +2761,16 @@
             body['drive_id'] = request.drive_id
         if not UtilClient.is_unset(request.expire_sec):
             body['expire_sec'] = request.expire_sec
         if not UtilClient.is_unset(request.file_id):
             body['file_id'] = request.file_id
         if not UtilClient.is_unset(request.file_name):
             body['file_name'] = request.file_name
+        if not UtilClient.is_unset(request.share_id):
+            body['share_id'] = request.share_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='GetDownloadUrl',
             version='2022-03-01',
@@ -2785,14 +2889,16 @@
         body = {}
         if not UtilClient.is_unset(request.drive_id):
             body['drive_id'] = request.drive_id
         if not UtilClient.is_unset(request.fields):
             body['fields'] = request.fields
         if not UtilClient.is_unset(request.file_id):
             body['file_id'] = request.file_id
+        if not UtilClient.is_unset(request.share_id):
+            body['share_id'] = request.share_id
         if not UtilClient.is_unset(request.url_expire_sec):
             body['url_expire_sec'] = request.url_expire_sec
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -2821,14 +2927,16 @@
         body = {}
         if not UtilClient.is_unset(request.drive_id):
             body['drive_id'] = request.drive_id
         if not UtilClient.is_unset(request.fields):
             body['fields'] = request.fields
         if not UtilClient.is_unset(request.file_id):
             body['file_id'] = request.file_id
+        if not UtilClient.is_unset(request.share_id):
+            body['share_id'] = request.share_id
         if not UtilClient.is_unset(request.url_expire_sec):
             body['url_expire_sec'] = request.url_expire_sec
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -3883,14 +3991,90 @@
         self,
         request: pds_20220301_models.ImportUserRequest,
     ) -> pds_20220301_models.ImportUserResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.import_user_with_options_async(request, headers, runtime)
 
+    def investigate_file_with_options(
+        self,
+        request: pds_20220301_models.InvestigateFileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pds_20220301_models.InvestigateFileResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.drive_file_ids):
+            body['drive_file_ids'] = request.drive_file_ids
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='InvestigateFile',
+            version='2022-03-01',
+            protocol='HTTPS',
+            pathname=f'/v2/csi/investigate_file',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pds_20220301_models.InvestigateFileResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def investigate_file_with_options_async(
+        self,
+        request: pds_20220301_models.InvestigateFileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pds_20220301_models.InvestigateFileResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.drive_file_ids):
+            body['drive_file_ids'] = request.drive_file_ids
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='InvestigateFile',
+            version='2022-03-01',
+            protocol='HTTPS',
+            pathname=f'/v2/csi/investigate_file',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pds_20220301_models.InvestigateFileResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def investigate_file(
+        self,
+        request: pds_20220301_models.InvestigateFileRequest,
+    ) -> pds_20220301_models.InvestigateFileResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.investigate_file_with_options(request, headers, runtime)
+
+    async def investigate_file_async(
+        self,
+        request: pds_20220301_models.InvestigateFileRequest,
+    ) -> pds_20220301_models.InvestigateFileResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.investigate_file_with_options_async(request, headers, runtime)
+
     def link_account_with_options(
         self,
         request: pds_20220301_models.LinkAccountRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pds_20220301_models.LinkAccountResponse:
         UtilClient.validate_model(request)
@@ -4435,14 +4619,16 @@
             body['marker'] = request.marker
         if not UtilClient.is_unset(request.order_by):
             body['order_by'] = request.order_by
         if not UtilClient.is_unset(request.order_direction):
             body['order_direction'] = request.order_direction
         if not UtilClient.is_unset(request.parent_file_id):
             body['parent_file_id'] = request.parent_file_id
+        if not UtilClient.is_unset(request.share_id):
+            body['share_id'] = request.share_id
         if not UtilClient.is_unset(request.status):
             body['status'] = request.status
         if not UtilClient.is_unset(request.type):
             body['type'] = request.type
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -4483,14 +4669,16 @@
             body['marker'] = request.marker
         if not UtilClient.is_unset(request.order_by):
             body['order_by'] = request.order_by
         if not UtilClient.is_unset(request.order_direction):
             body['order_direction'] = request.order_direction
         if not UtilClient.is_unset(request.parent_file_id):
             body['parent_file_id'] = request.parent_file_id
+        if not UtilClient.is_unset(request.share_id):
+            body['share_id'] = request.share_id
         if not UtilClient.is_unset(request.status):
             body['status'] = request.status
         if not UtilClient.is_unset(request.type):
             body['type'] = request.type
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -6959,14 +7147,16 @@
         body = {}
         if not UtilClient.is_unset(request.description):
             body['description'] = request.description
         if not UtilClient.is_unset(request.drive_id):
             body['drive_id'] = request.drive_id
         if not UtilClient.is_unset(request.drive_name):
             body['drive_name'] = request.drive_name
+        if not UtilClient.is_unset(request.owner):
+            body['owner'] = request.owner
         if not UtilClient.is_unset(request.status):
             body['status'] = request.status
         if not UtilClient.is_unset(request.total_size):
             body['total_size'] = request.total_size
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -6997,14 +7187,16 @@
         body = {}
         if not UtilClient.is_unset(request.description):
             body['description'] = request.description
         if not UtilClient.is_unset(request.drive_id):
             body['drive_id'] = request.drive_id
         if not UtilClient.is_unset(request.drive_name):
             body['drive_name'] = request.drive_name
+        if not UtilClient.is_unset(request.owner):
+            body['owner'] = request.owner
         if not UtilClient.is_unset(request.status):
             body['status'] = request.status
         if not UtilClient.is_unset(request.total_size):
             body['total_size'] = request.total_size
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
```

### Comparing `alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301/models.py` & `alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,14 +574,47 @@
         if m.get('remarks') is not None:
             self.remarks = m.get('remarks')
         if m.get('updated_at') is not None:
             self.updated_at = m.get('updated_at')
         return self
 
 
+class FileInvestigationInfo(TeaModel):
+    def __init__(
+        self,
+        status: int = None,
+        suggestion: str = None,
+    ):
+        self.status = status
+        self.suggestion = suggestion
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
+        if self.status is not None:
+            result['status'] = self.status
+        if self.suggestion is not None:
+            result['suggestion'] = self.suggestion
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('suggestion') is not None:
+            self.suggestion = m.get('suggestion')
+        return self
+
+
 class File(TeaModel):
     def __init__(
         self,
         category: str = None,
         content_hash: str = None,
         content_hash_name: str = None,
         content_type: str = None,
@@ -590,14 +623,15 @@
         description: str = None,
         domain_id: str = None,
         download_url: str = None,
         drive_id: str = None,
         file_extension: str = None,
         file_id: str = None,
         hidden: bool = None,
+        investigation_info: FileInvestigationInfo = None,
         labels: str = None,
         local_created_at: str = None,
         local_modified_at: str = None,
         name: str = None,
         parent_file_id: str = None,
         revision_id: str = None,
         size: int = None,
@@ -618,14 +652,15 @@
         self.description = description
         self.domain_id = domain_id
         self.download_url = download_url
         self.drive_id = drive_id
         self.file_extension = file_extension
         self.file_id = file_id
         self.hidden = hidden
+        self.investigation_info = investigation_info
         self.labels = labels
         self.local_created_at = local_created_at
         self.local_modified_at = local_modified_at
         self.name = name
         self.parent_file_id = parent_file_id
         self.revision_id = revision_id
         self.size = size
@@ -634,15 +669,16 @@
         self.thumbnail = thumbnail
         self.trashed_at = trashed_at
         self.type = type
         self.updated_at = updated_at
         self.upload_id = upload_id
 
     def validate(self):
-        pass
+        if self.investigation_info:
+            self.investigation_info.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -668,14 +704,16 @@
             result['drive_id'] = self.drive_id
         if self.file_extension is not None:
             result['file_extension'] = self.file_extension
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.hidden is not None:
             result['hidden'] = self.hidden
+        if self.investigation_info is not None:
+            result['investigation_info'] = self.investigation_info.to_map()
         if self.labels is not None:
             result['labels'] = self.labels
         if self.local_created_at is not None:
             result['local_created_at'] = self.local_created_at
         if self.local_modified_at is not None:
             result['local_modified_at'] = self.local_modified_at
         if self.name is not None:
@@ -726,14 +764,17 @@
             self.drive_id = m.get('drive_id')
         if m.get('file_extension') is not None:
             self.file_extension = m.get('file_extension')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('hidden') is not None:
             self.hidden = m.get('hidden')
+        if m.get('investigation_info') is not None:
+            temp_model = FileInvestigationInfo()
+            self.investigation_info = temp_model.from_map(m['investigation_info'])
         if m.get('labels') is not None:
             self.labels = m.get('labels')
         if m.get('local_created_at') is not None:
             self.local_created_at = m.get('local_created_at')
         if m.get('local_modified_at') is not None:
             self.local_modified_at = m.get('local_modified_at')
         if m.get('name') is not None:
@@ -1171,14 +1212,129 @@
         if m.get('cover_url') is not None:
             self.cover_url = m.get('cover_url')
         if m.get('name') is not None:
             self.name = m.get('name')
         return self
 
 
+class InvestigationInfoVideoDetailBlockFrames(TeaModel):
+    def __init__(
+        self,
+        label: str = None,
+        offset: int = None,
+        rate: float = None,
+    ):
+        self.label = label
+        self.offset = offset
+        self.rate = rate
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
+        if self.label is not None:
+            result['label'] = self.label
+        if self.offset is not None:
+            result['offset'] = self.offset
+        if self.rate is not None:
+            result['rate'] = self.rate
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('label') is not None:
+            self.label = m.get('label')
+        if m.get('offset') is not None:
+            self.offset = m.get('offset')
+        if m.get('rate') is not None:
+            self.rate = m.get('rate')
+        return self
+
+
+class InvestigationInfoVideoDetail(TeaModel):
+    def __init__(
+        self,
+        block_frames: List[InvestigationInfoVideoDetailBlockFrames] = None,
+    ):
+        self.block_frames = block_frames
+
+    def validate(self):
+        if self.block_frames:
+            for k in self.block_frames:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['block_frames'] = []
+        if self.block_frames is not None:
+            for k in self.block_frames:
+                result['block_frames'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.block_frames = []
+        if m.get('block_frames') is not None:
+            for k in m.get('block_frames'):
+                temp_model = InvestigationInfoVideoDetailBlockFrames()
+                self.block_frames.append(temp_model.from_map(k))
+        return self
+
+
+class InvestigationInfo(TeaModel):
+    def __init__(
+        self,
+        status: int = None,
+        suggestion: str = None,
+        video_detail: InvestigationInfoVideoDetail = None,
+    ):
+        self.status = status
+        self.suggestion = suggestion
+        self.video_detail = video_detail
+
+    def validate(self):
+        if self.video_detail:
+            self.video_detail.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.status is not None:
+            result['status'] = self.status
+        if self.suggestion is not None:
+            result['suggestion'] = self.suggestion
+        if self.video_detail is not None:
+            result['video_detail'] = self.video_detail.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('suggestion') is not None:
+            self.suggestion = m.get('suggestion')
+        if m.get('video_detail') is not None:
+            temp_model = InvestigationInfoVideoDetail()
+            self.video_detail = temp_model.from_map(m['video_detail'])
+        return self
+
+
 class JWTPayload(TeaModel):
     def __init__(
         self,
         aud: str = None,
         auto_create: bool = None,
         exp: int = None,
         iat: int = None,
@@ -1396,20 +1552,21 @@
         disable_preview: bool = None,
         disable_save: bool = None,
         download_count: int = None,
         download_limit: int = None,
         drive_id: str = None,
         expiration: str = None,
         expired: bool = None,
-        file_id_list: str = None,
+        file_id_list: List[str] = None,
         preview_count: int = None,
         preview_limit: int = None,
         report_count: int = None,
         save_count: int = None,
         save_limit: int = None,
+        share_all_files: bool = None,
         share_id: str = None,
         share_name: str = None,
         share_pwd: str = None,
         status: str = None,
         updated_at: str = None,
         video_preview_count: int = None,
     ):
@@ -1427,14 +1584,15 @@
         self.expired = expired
         self.file_id_list = file_id_list
         self.preview_count = preview_count
         self.preview_limit = preview_limit
         self.report_count = report_count
         self.save_count = save_count
         self.save_limit = save_limit
+        self.share_all_files = share_all_files
         self.share_id = share_id
         self.share_name = share_name
         self.share_pwd = share_pwd
         self.status = status
         self.updated_at = updated_at
         self.video_preview_count = video_preview_count
 
@@ -1479,14 +1637,16 @@
             result['preview_limit'] = self.preview_limit
         if self.report_count is not None:
             result['report_count'] = self.report_count
         if self.save_count is not None:
             result['save_count'] = self.save_count
         if self.save_limit is not None:
             result['save_limit'] = self.save_limit
+        if self.share_all_files is not None:
+            result['share_all_files'] = self.share_all_files
         if self.share_id is not None:
             result['share_id'] = self.share_id
         if self.share_name is not None:
             result['share_name'] = self.share_name
         if self.share_pwd is not None:
             result['share_pwd'] = self.share_pwd
         if self.status is not None:
@@ -1531,14 +1691,16 @@
             self.preview_limit = m.get('preview_limit')
         if m.get('report_count') is not None:
             self.report_count = m.get('report_count')
         if m.get('save_count') is not None:
             self.save_count = m.get('save_count')
         if m.get('save_limit') is not None:
             self.save_limit = m.get('save_limit')
+        if m.get('share_all_files') is not None:
+            self.share_all_files = m.get('share_all_files')
         if m.get('share_id') is not None:
             self.share_id = m.get('share_id')
         if m.get('share_name') is not None:
             self.share_name = m.get('share_name')
         if m.get('share_pwd') is not None:
             self.share_pwd = m.get('share_pwd')
         if m.get('status') is not None:
@@ -2856,19 +3018,23 @@
 
 class CopyFileRequest(TeaModel):
     def __init__(
         self,
         auto_rename: bool = None,
         drive_id: str = None,
         file_id: str = None,
+        share_id: str = None,
+        to_drive_id: str = None,
         to_parent_file_id: str = None,
     ):
         self.auto_rename = auto_rename
         self.drive_id = drive_id
         self.file_id = file_id
+        self.share_id = share_id
+        self.to_drive_id = to_drive_id
         self.to_parent_file_id = to_parent_file_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2878,26 +3044,34 @@
         result = dict()
         if self.auto_rename is not None:
             result['auto_rename'] = self.auto_rename
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.file_id is not None:
             result['file_id'] = self.file_id
+        if self.share_id is not None:
+            result['share_id'] = self.share_id
+        if self.to_drive_id is not None:
+            result['to_drive_id'] = self.to_drive_id
         if self.to_parent_file_id is not None:
             result['to_parent_file_id'] = self.to_parent_file_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auto_rename') is not None:
             self.auto_rename = m.get('auto_rename')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
+        if m.get('share_id') is not None:
+            self.share_id = m.get('share_id')
+        if m.get('to_drive_id') is not None:
+            self.to_drive_id = m.get('to_drive_id')
         if m.get('to_parent_file_id') is not None:
             self.to_parent_file_id = m.get('to_parent_file_id')
         return self
 
 
 class CopyFileResponseBody(TeaModel):
     def __init__(
@@ -3675,28 +3849,30 @@
         disable_save: bool = None,
         download_limit: int = None,
         drive_id: str = None,
         expiration: str = None,
         file_id_list: List[str] = None,
         preview_limit: int = None,
         save_limit: int = None,
+        share_all_files: bool = None,
         share_name: str = None,
         share_pwd: str = None,
         user_id: str = None,
     ):
         self.description = description
         self.disable_download = disable_download
         self.disable_preview = disable_preview
         self.disable_save = disable_save
         self.download_limit = download_limit
         self.drive_id = drive_id
         self.expiration = expiration
         self.file_id_list = file_id_list
         self.preview_limit = preview_limit
         self.save_limit = save_limit
+        self.share_all_files = share_all_files
         self.share_name = share_name
         self.share_pwd = share_pwd
         self.user_id = user_id
 
     def validate(self):
         pass
 
@@ -3722,14 +3898,16 @@
             result['expiration'] = self.expiration
         if self.file_id_list is not None:
             result['file_id_list'] = self.file_id_list
         if self.preview_limit is not None:
             result['preview_limit'] = self.preview_limit
         if self.save_limit is not None:
             result['save_limit'] = self.save_limit
+        if self.share_all_files is not None:
+            result['share_all_files'] = self.share_all_files
         if self.share_name is not None:
             result['share_name'] = self.share_name
         if self.share_pwd is not None:
             result['share_pwd'] = self.share_pwd
         if self.user_id is not None:
             result['user_id'] = self.user_id
         return result
@@ -3752,14 +3930,16 @@
             self.expiration = m.get('expiration')
         if m.get('file_id_list') is not None:
             self.file_id_list = m.get('file_id_list')
         if m.get('preview_limit') is not None:
             self.preview_limit = m.get('preview_limit')
         if m.get('save_limit') is not None:
             self.save_limit = m.get('save_limit')
+        if m.get('share_all_files') is not None:
+            self.share_all_files = m.get('share_all_files')
         if m.get('share_name') is not None:
             self.share_name = m.get('share_name')
         if m.get('share_pwd') is not None:
             self.share_pwd = m.get('share_pwd')
         if m.get('user_id') is not None:
             self.user_id = m.get('user_id')
         return self
@@ -4082,14 +4262,132 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CsiGetFileInfoRequest(TeaModel):
+    def __init__(
+        self,
+        drive_id: str = None,
+        file_id: str = None,
+        url_expire_sec: int = None,
+    ):
+        self.drive_id = drive_id
+        self.file_id = file_id
+        self.url_expire_sec = url_expire_sec
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
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.url_expire_sec is not None:
+            result['url_expire_sec'] = self.url_expire_sec
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('url_expire_sec') is not None:
+            self.url_expire_sec = m.get('url_expire_sec')
+        return self
+
+
+class CsiGetFileInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        investigation_info: InvestigationInfo = None,
+        url: str = None,
+    ):
+        self.investigation_info = investigation_info
+        self.url = url
+
+    def validate(self):
+        if self.investigation_info:
+            self.investigation_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.investigation_info is not None:
+            result['investigation_info'] = self.investigation_info.to_map()
+        if self.url is not None:
+            result['url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('investigation_info') is not None:
+            temp_model = InvestigationInfo()
+            self.investigation_info = temp_model.from_map(m['investigation_info'])
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        return self
+
+
+class CsiGetFileInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CsiGetFileInfoResponseBody = None,
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
+            temp_model = CsiGetFileInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteDomainRequest(TeaModel):
     def __init__(
         self,
         domain_id: str = None,
     ):
         # domain id
         self.domain_id = domain_id
@@ -4633,20 +4931,22 @@
 class DownloadFileRequest(TeaModel):
     def __init__(
         self,
         drive_id: str = None,
         file_id: str = None,
         image_thumbnail_process: str = None,
         office_thumbnail_process: str = None,
+        share_id: str = None,
         video_thumbnail_process: str = None,
     ):
         self.drive_id = drive_id
         self.file_id = file_id
         self.image_thumbnail_process = image_thumbnail_process
         self.office_thumbnail_process = office_thumbnail_process
+        self.share_id = share_id
         self.video_thumbnail_process = video_thumbnail_process
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4658,28 +4958,32 @@
             result['drive_id'] = self.drive_id
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.image_thumbnail_process is not None:
             result['image_thumbnail_process'] = self.image_thumbnail_process
         if self.office_thumbnail_process is not None:
             result['office_thumbnail_process'] = self.office_thumbnail_process
+        if self.share_id is not None:
+            result['share_id'] = self.share_id
         if self.video_thumbnail_process is not None:
             result['video_thumbnail_process'] = self.video_thumbnail_process
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('image_thumbnail_process') is not None:
             self.image_thumbnail_process = m.get('image_thumbnail_process')
         if m.get('office_thumbnail_process') is not None:
             self.office_thumbnail_process = m.get('office_thumbnail_process')
+        if m.get('share_id') is not None:
+            self.share_id = m.get('share_id')
         if m.get('video_thumbnail_process') is not None:
             self.video_thumbnail_process = m.get('video_thumbnail_process')
         return self
 
 
 class DownloadFileResponse(TeaModel):
     def __init__(
@@ -5506,19 +5810,21 @@
 class GetDownloadUrlRequest(TeaModel):
     def __init__(
         self,
         drive_id: str = None,
         expire_sec: int = None,
         file_id: str = None,
         file_name: str = None,
+        share_id: str = None,
     ):
         self.drive_id = drive_id
         self.expire_sec = expire_sec
         self.file_id = file_id
         self.file_name = file_name
+        self.share_id = share_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -5529,26 +5835,30 @@
             result['drive_id'] = self.drive_id
         if self.expire_sec is not None:
             result['expire_sec'] = self.expire_sec
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.file_name is not None:
             result['file_name'] = self.file_name
+        if self.share_id is not None:
+            result['share_id'] = self.share_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('expire_sec') is not None:
             self.expire_sec = m.get('expire_sec')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('file_name') is not None:
             self.file_name = m.get('file_name')
+        if m.get('share_id') is not None:
+            self.share_id = m.get('share_id')
         return self
 
 
 class GetDownloadUrlResponseBody(TeaModel):
     def __init__(
         self,
         cdn_url: str = None,
@@ -5734,19 +6044,21 @@
 
 class GetFileRequest(TeaModel):
     def __init__(
         self,
         drive_id: str = None,
         fields: str = None,
         file_id: str = None,
+        share_id: str = None,
         url_expire_sec: int = None,
     ):
         self.drive_id = drive_id
         self.fields = fields
         self.file_id = file_id
+        self.share_id = share_id
         self.url_expire_sec = url_expire_sec
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5756,26 +6068,30 @@
         result = dict()
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.fields is not None:
             result['fields'] = self.fields
         if self.file_id is not None:
             result['file_id'] = self.file_id
+        if self.share_id is not None:
+            result['share_id'] = self.share_id
         if self.url_expire_sec is not None:
             result['url_expire_sec'] = self.url_expire_sec
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('fields') is not None:
             self.fields = m.get('fields')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
+        if m.get('share_id') is not None:
+            self.share_id = m.get('share_id')
         if m.get('url_expire_sec') is not None:
             self.url_expire_sec = m.get('url_expire_sec')
         return self
 
 
 class GetFileResponse(TeaModel):
     def __init__(
@@ -7293,14 +7609,116 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = User()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class InvestigateFileRequestDriveFileIds(TeaModel):
+    def __init__(
+        self,
+        drive_id: str = None,
+        file_id: str = None,
+    ):
+        self.drive_id = drive_id
+        self.file_id = file_id
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
+        if self.drive_id is not None:
+            result['drive_id'] = self.drive_id
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('drive_id') is not None:
+            self.drive_id = m.get('drive_id')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        return self
+
+
+class InvestigateFileRequest(TeaModel):
+    def __init__(
+        self,
+        drive_file_ids: List[InvestigateFileRequestDriveFileIds] = None,
+    ):
+        self.drive_file_ids = drive_file_ids
+
+    def validate(self):
+        if self.drive_file_ids:
+            for k in self.drive_file_ids:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['drive_file_ids'] = []
+        if self.drive_file_ids is not None:
+            for k in self.drive_file_ids:
+                result['drive_file_ids'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.drive_file_ids = []
+        if m.get('drive_file_ids') is not None:
+            for k in m.get('drive_file_ids'):
+                temp_model = InvestigateFileRequestDriveFileIds()
+                self.drive_file_ids.append(temp_model.from_map(k))
+        return self
+
+
+class InvestigateFileResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
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
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
 class LinkAccountRequest(TeaModel):
     def __init__(
         self,
         extra: str = None,
         identity: str = None,
         type: str = None,
         user_id: str = None,
@@ -8090,25 +8508,27 @@
         drive_id: str = None,
         fields: str = None,
         limit: int = None,
         marker: str = None,
         order_by: str = None,
         order_direction: str = None,
         parent_file_id: str = None,
+        share_id: str = None,
         status: str = None,
         type: str = None,
     ):
         self.category = category
         self.drive_id = drive_id
         self.fields = fields
         self.limit = limit
         self.marker = marker
         self.order_by = order_by
         self.order_direction = order_direction
         self.parent_file_id = parent_file_id
+        self.share_id = share_id
         self.status = status
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -8129,14 +8549,16 @@
             result['marker'] = self.marker
         if self.order_by is not None:
             result['order_by'] = self.order_by
         if self.order_direction is not None:
             result['order_direction'] = self.order_direction
         if self.parent_file_id is not None:
             result['parent_file_id'] = self.parent_file_id
+        if self.share_id is not None:
+            result['share_id'] = self.share_id
         if self.status is not None:
             result['status'] = self.status
         if self.type is not None:
             result['type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
@@ -8153,14 +8575,16 @@
             self.marker = m.get('marker')
         if m.get('order_by') is not None:
             self.order_by = m.get('order_by')
         if m.get('order_direction') is not None:
             self.order_direction = m.get('order_direction')
         if m.get('parent_file_id') is not None:
             self.parent_file_id = m.get('parent_file_id')
+        if m.get('share_id') is not None:
+            self.share_id = m.get('share_id')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
@@ -11654,20 +12078,22 @@
 
 class UpdateDriveRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
         drive_id: str = None,
         drive_name: str = None,
+        owner: str = None,
         status: str = None,
         total_size: int = None,
     ):
         self.description = description
         self.drive_id = drive_id
         self.drive_name = drive_name
+        self.owner = owner
         self.status = status
         self.total_size = total_size
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -11678,28 +12104,32 @@
         result = dict()
         if self.description is not None:
             result['description'] = self.description
         if self.drive_id is not None:
             result['drive_id'] = self.drive_id
         if self.drive_name is not None:
             result['drive_name'] = self.drive_name
+        if self.owner is not None:
+            result['owner'] = self.owner
         if self.status is not None:
             result['status'] = self.status
         if self.total_size is not None:
             result['total_size'] = self.total_size
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('description') is not None:
             self.description = m.get('description')
         if m.get('drive_id') is not None:
             self.drive_id = m.get('drive_id')
         if m.get('drive_name') is not None:
             self.drive_name = m.get('drive_name')
+        if m.get('owner') is not None:
+            self.owner = m.get('owner')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('total_size') is not None:
             self.total_size = m.get('total_size')
         return self
```

### Comparing `alibabacloud_pds20220301-1.0.7/alibabacloud_pds20220301.egg-info/PKG-INFO` & `alibabacloud_pds20220301-1.0.8/alibabacloud_pds20220301.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pds20220301
-Version: 1.0.7
+Version: 1.0.8
 Summary: Alibaba Cloud pds (20220301) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pds20220301-1.0.7/setup.py` & `alibabacloud_pds20220301-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pds20220301.
 
-Created on 06/04/2023
+Created on 14/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pds20220301"
 NAME = "alibabacloud_pds20220301" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud pds (20220301) SDK Library for Python"
```

