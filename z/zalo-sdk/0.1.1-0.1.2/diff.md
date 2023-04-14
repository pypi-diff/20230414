# Comparing `tmp/zalo_sdk-0.1.1-py3-none-any.whl.zip` & `tmp/zalo_sdk-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4509 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1297 b- defN 23-Apr-14 11:21 zalo_sdk/BaseClient.py
+Zip file size: 4464 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1242 b- defN 23-Apr-14 11:31 zalo_sdk/BaseClient.py
 -rw-r--r--  2.0 unx       34 b- defN 23-Apr-14 09:29 zalo_sdk/__init__.py
--rw-r--r--  2.0 unx     4778 b- defN 23-Apr-14 09:29 zalo_sdk/oa/Client.py
+-rw-r--r--  2.0 unx     4711 b- defN 23-Apr-14 11:32 zalo_sdk/oa/Client.py
 -rw-r--r--  2.0 unx       26 b- defN 23-Apr-14 09:29 zalo_sdk/oa/__init__.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Apr-14 11:23 zalo_sdk-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1445 b- defN 23-Apr-14 11:23 zalo_sdk-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 11:23 zalo_sdk-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-14 11:23 zalo_sdk-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      700 b- defN 23-Apr-14 11:23 zalo_sdk-0.1.1.dist-info/RECORD
-9 files, 9445 bytes uncompressed, 3303 bytes compressed:  65.0%
+-rw-r--r--  2.0 unx     1064 b- defN 23-Apr-14 11:40 zalo_sdk-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1445 b- defN 23-Apr-14 11:40 zalo_sdk-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 11:40 zalo_sdk-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-14 11:40 zalo_sdk-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      700 b- defN 23-Apr-14 11:40 zalo_sdk-0.1.2.dist-info/RECORD
+9 files, 9323 bytes uncompressed, 3258 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: zalo_sdk/oa/Client.py
 Comment: 
 
 Filename: zalo_sdk/oa/__init__.py
 Comment: 
 
-Filename: zalo_sdk-0.1.1.dist-info/LICENSE
+Filename: zalo_sdk-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: zalo_sdk-0.1.1.dist-info/METADATA
+Filename: zalo_sdk-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: zalo_sdk-0.1.1.dist-info/WHEEL
+Filename: zalo_sdk-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: zalo_sdk-0.1.1.dist-info/top_level.txt
+Filename: zalo_sdk-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: zalo_sdk-0.1.1.dist-info/RECORD
+Filename: zalo_sdk-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zalo_sdk/BaseClient.py

```diff
@@ -1,13 +1,13 @@
 import requests
 import json
 
 
 class BaseClient:
-    def __init__(self, access_token: str = "", refresh_token: str = ""):
+    def __init__(self, access_token = "", refresh_token = ""):
         self._refresh_token = refresh_token
         self._access_token = access_token
 
     @property
     def refresh_token(self):
         return self._refresh_token
 
@@ -19,15 +19,15 @@
     def access_token(self):
         return self._access_token
 
     @access_token.setter
     def access_token(self, token):
         self._access_token = token
 
-    def send_request(self, method: str, url: str, body: object | str) -> requests.Response:
+    def send_request(self, method, url, body):
         if method == "POST":
             headers = {
                 'Content-Type': "application/json",
                 'access_token': self._access_token
             }
             response = requests.post(
                 url,
```

## zalo_sdk/oa/Client.py

```diff
@@ -14,15 +14,15 @@
 
     def get_authoriation_code(self, callback_url):
         escaped_url = urllib.parse.quote(callback_url, safe='')
         auth_url = f"https://oauth.zaloapp.com/v4/oa/permission?app_id={self.app_id}&redirect_uri={escaped_url}"
 
         return auth_url
 
-    def get_access_token(self, authorization_code) -> tuple[str, str]:
+    def get_access_token(self, authorization_code):
         zalo_get_access_token_url = "https://oauth.zaloapp.com/v4/oa/access_token"
         headers = {}
         headers['Content-Type'] = "application/x-www-form-urlencoded"
         headers['secret_key'] = self.secret_key
         body = {
             'code': authorization_code,
             'app_id': self.app_id,
@@ -42,15 +42,15 @@
             raise Exception("Error: 'access_token' not found in the response")
 
         self.refresh_token = zalo_response['refresh_token']
         self.access_token = zalo_response['access_token']
 
         return self.access_token, self.refresh_token
 
-    def refresh_acccess_token(self) -> tuple[str, str]:
+    def refresh_acccess_token(self):
         zalo_get_access_token_url = "https://oauth.zaloapp.com/v4/oa/access_token"
         headers = {}
         headers['Content-Type'] = "application/x-www-form-urlencoded"
         headers['secret_key'] = self.secret_key
         body = {
             'refresh_token': self._refresh_token,
             'app_id': self.app_id,
@@ -69,15 +69,15 @@
             raise Exception("Error: 'access_token' not found in the response")
 
         self.refresh_token = zalo_response['refresh_token']
         self.access_token = zalo_response['access_token']
 
         return self.access_token, self.refresh_token
 
-    def send_message_to_user(self, user_id: str, message: str):
+    def send_message_to_user(self, user_id, message):
         body = {
             "recipient": {
                 "user_id": user_id
             },
             "message": {
                 "text": message
             }
@@ -85,15 +85,15 @@
         response = self.send_request(
             "POST", "https://openapi.zalo.me/v2.0/oa/message", body)
         if response.status_code != 200:
             raise Exception(f"Error {response.status_code}: {response.text}")
         zalo_response = response.json()
         return zalo_response
 
-    def send_response_to_user(self, message_id: str, message: str):
+    def send_response_to_user(self, message_id, message):
         body = {
             "recipient": {
                 "message_id": message_id
             },
             "message": {
                 "text": message
             }
@@ -101,29 +101,29 @@
         response = self.send_request(
             "POST", "https://openapi.zalo.me/v2.0/oa/message", body)
         if response.status_code != 200:
             raise Exception(f"Error {response.status_code}: {response.text}")
         zalo_response = response.json()
         return zalo_response
 
-    def get_free_response_quota(self, message_id: str):
+    def get_free_response_quota(self, message_id):
         body = {
             "message_id": message_id
         }
         response = self.send_request(
             "POST", "https://openapi.zalo.me/v2.0/oa/quota/message", body)
         if response.status_code != 200:
             raise Exception(f"Error {response.status_code}: {response.text}")
         zalo_response = response.json()
         return zalo_response
 
-    def get_profile(self, user_id: str):
+    def get_profile(self, user_id):
         params = {
             "user_id": user_id
         }
         response = self.send_request(
             "GET", "https://openapi.zalo.me/v2.0/oa/getprofile", params
         )
         if response.status_code != 200:
             raise Exception(f"Error {response.status_code}: {response.text}")
         zalo_response = response.json()
-        return zalo_response
+        return zalo_response
```

## Comparing `zalo_sdk-0.1.1.dist-info/LICENSE` & `zalo_sdk-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zalo_sdk-0.1.1.dist-info/METADATA` & `zalo_sdk-0.1.2.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalo-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Zalo SDK
 Home-page: https://github.com/connext_biz
 Author: Khoa Tran
 Author-email: khoa@connext.biz
 License: MIT License
         
         Copyright (c) 2023 Connext
```

## Comparing `zalo_sdk-0.1.1.dist-info/RECORD` & `zalo_sdk-0.1.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-zalo_sdk/BaseClient.py,sha256=jcADecANplRoynXTUWldGgEzekBzPQCOJcahrvapo8E,1297
+zalo_sdk/BaseClient.py,sha256=4gyANmsDIVJofMAYQTGR-iqugsrFPBiyiMy8U0m0uww,1242
 zalo_sdk/__init__.py,sha256=eMIRVZSpFkWrKuSRsC_og-vZDGPaGs760mMWttqWIZ0,34
-zalo_sdk/oa/Client.py,sha256=KY3Yz20pMSZhG0WCzD8TKI0yCM1V7stgk3G8NfT_PEE,4778
+zalo_sdk/oa/Client.py,sha256=bkd6Eg9KwsSRYjLIGiIG1y0lBXxThJhJvgD0Td8Iu6E,4711
 zalo_sdk/oa/__init__.py,sha256=uPJxw8bRdtz525KWrBMkyvxS6sNeBbb8EiKTgQ72ytI,26
-zalo_sdk-0.1.1.dist-info/LICENSE,sha256=DosZBEVw1BQ_JPl_v0SoKFYiUV9ehPhbcHh-PBAemKw,1064
-zalo_sdk-0.1.1.dist-info/METADATA,sha256=gqRUurGQVv8oACigOC-N8J_B4J2LPU6LoDyv6nl-KLA,1445
-zalo_sdk-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-zalo_sdk-0.1.1.dist-info/top_level.txt,sha256=2y9NKIvYeI81nXRSpnUX3-s0JSTlt_khQZDZYDw3ll0,9
-zalo_sdk-0.1.1.dist-info/RECORD,,
+zalo_sdk-0.1.2.dist-info/LICENSE,sha256=DosZBEVw1BQ_JPl_v0SoKFYiUV9ehPhbcHh-PBAemKw,1064
+zalo_sdk-0.1.2.dist-info/METADATA,sha256=AttopjV7N6W1bcEYkG-ulu_WsOk65yQeXQB1FJvvgX8,1445
+zalo_sdk-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+zalo_sdk-0.1.2.dist-info/top_level.txt,sha256=2y9NKIvYeI81nXRSpnUX3-s0JSTlt_khQZDZYDw3ll0,9
+zalo_sdk-0.1.2.dist-info/RECORD,,
```

