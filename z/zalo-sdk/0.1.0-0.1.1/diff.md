# Comparing `tmp/zalo_sdk-0.1.0-py3-none-any.whl.zip` & `tmp/zalo_sdk-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4514 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1378 b- defN 23-Apr-14 09:29 zalo_sdk/BaseClient.py
+Zip file size: 4509 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1297 b- defN 23-Apr-14 11:21 zalo_sdk/BaseClient.py
 -rw-r--r--  2.0 unx       34 b- defN 23-Apr-14 09:29 zalo_sdk/__init__.py
 -rw-r--r--  2.0 unx     4778 b- defN 23-Apr-14 09:29 zalo_sdk/oa/Client.py
 -rw-r--r--  2.0 unx       26 b- defN 23-Apr-14 09:29 zalo_sdk/oa/__init__.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Apr-14 09:44 zalo_sdk-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1445 b- defN 23-Apr-14 09:44 zalo_sdk-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 09:44 zalo_sdk-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-14 09:44 zalo_sdk-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      700 b- defN 23-Apr-14 09:44 zalo_sdk-0.1.0.dist-info/RECORD
-9 files, 9526 bytes uncompressed, 3308 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx     1064 b- defN 23-Apr-14 11:23 zalo_sdk-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1445 b- defN 23-Apr-14 11:23 zalo_sdk-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 11:23 zalo_sdk-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-14 11:23 zalo_sdk-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      700 b- defN 23-Apr-14 11:23 zalo_sdk-0.1.1.dist-info/RECORD
+9 files, 9445 bytes uncompressed, 3303 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: zalo_sdk/oa/Client.py
 Comment: 
 
 Filename: zalo_sdk/oa/__init__.py
 Comment: 
 
-Filename: zalo_sdk-0.1.0.dist-info/LICENSE
+Filename: zalo_sdk-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: zalo_sdk-0.1.0.dist-info/METADATA
+Filename: zalo_sdk-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: zalo_sdk-0.1.0.dist-info/WHEEL
+Filename: zalo_sdk-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: zalo_sdk-0.1.0.dist-info/top_level.txt
+Filename: zalo_sdk-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: zalo_sdk-0.1.0.dist-info/RECORD
+Filename: zalo_sdk-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zalo_sdk/BaseClient.py

```diff
@@ -1,10 +1,11 @@
 import requests
 import json
 
+
 class BaseClient:
     def __init__(self, access_token: str = "", refresh_token: str = ""):
         self._refresh_token = refresh_token
         self._access_token = access_token
 
     @property
     def refresh_token(self):
@@ -19,28 +20,27 @@
         return self._access_token
 
     @access_token.setter
     def access_token(self, token):
         self._access_token = token
 
     def send_request(self, method: str, url: str, body: object | str) -> requests.Response:
-        match method:
-            case "POST":
-                headers = {
-                    'Content-Type': "application/json",
-                    'access_token': self._access_token
-                }
-                response = requests.post(
-                    url,
-                    json=body,
-                    headers=headers)
-            case "GET":
-                headers = {
-                    'access_token': self._access_token
-                }
-                response = requests.get(
-                    url,
-                    params={"data": json.dumps(body)},
-                    headers=headers)
-            case _:
-                raise Exception(f"Unknown method '{method}'")
+        if method == "POST":
+            headers = {
+                'Content-Type': "application/json",
+                'access_token': self._access_token
+            }
+            response = requests.post(
+                url,
+                json=body,
+                headers=headers)
+        elif method == "GET":
+            headers = {
+                'access_token': self._access_token
+            }
+            response = requests.get(
+                url,
+                params={"data": json.dumps(body)},
+                headers=headers)
+        else:
+            raise Exception(f"Unknown method '{method}'")
         return response
```

## Comparing `zalo_sdk-0.1.0.dist-info/LICENSE` & `zalo_sdk-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zalo_sdk-0.1.0.dist-info/METADATA` & `zalo_sdk-0.1.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalo-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Zalo SDK
 Home-page: https://github.com/connext_biz
 Author: Khoa Tran
 Author-email: khoa@connext.biz
 License: MIT License
         
         Copyright (c) 2023 Connext
```

## Comparing `zalo_sdk-0.1.0.dist-info/RECORD` & `zalo_sdk-0.1.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-zalo_sdk/BaseClient.py,sha256=_cxQLWuvsxyp6tpV23tqIaEcLGaqoHYXg15kC7wXxfs,1378
+zalo_sdk/BaseClient.py,sha256=jcADecANplRoynXTUWldGgEzekBzPQCOJcahrvapo8E,1297
 zalo_sdk/__init__.py,sha256=eMIRVZSpFkWrKuSRsC_og-vZDGPaGs760mMWttqWIZ0,34
 zalo_sdk/oa/Client.py,sha256=KY3Yz20pMSZhG0WCzD8TKI0yCM1V7stgk3G8NfT_PEE,4778
 zalo_sdk/oa/__init__.py,sha256=uPJxw8bRdtz525KWrBMkyvxS6sNeBbb8EiKTgQ72ytI,26
-zalo_sdk-0.1.0.dist-info/LICENSE,sha256=DosZBEVw1BQ_JPl_v0SoKFYiUV9ehPhbcHh-PBAemKw,1064
-zalo_sdk-0.1.0.dist-info/METADATA,sha256=QOp2d633O2Dr7OZis8li5Qo2KgYRcn13L5eduVWQdKs,1445
-zalo_sdk-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-zalo_sdk-0.1.0.dist-info/top_level.txt,sha256=2y9NKIvYeI81nXRSpnUX3-s0JSTlt_khQZDZYDw3ll0,9
-zalo_sdk-0.1.0.dist-info/RECORD,,
+zalo_sdk-0.1.1.dist-info/LICENSE,sha256=DosZBEVw1BQ_JPl_v0SoKFYiUV9ehPhbcHh-PBAemKw,1064
+zalo_sdk-0.1.1.dist-info/METADATA,sha256=gqRUurGQVv8oACigOC-N8J_B4J2LPU6LoDyv6nl-KLA,1445
+zalo_sdk-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+zalo_sdk-0.1.1.dist-info/top_level.txt,sha256=2y9NKIvYeI81nXRSpnUX3-s0JSTlt_khQZDZYDw3ll0,9
+zalo_sdk-0.1.1.dist-info/RECORD,,
```

