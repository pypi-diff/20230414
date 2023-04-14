# Comparing `tmp/ppa_api-2.6.0-py3-none-any.whl.zip` & `tmp/ppa_api-2.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9803 bytes, number of entries: 11
+Zip file size: 9850 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-29 06:49 ppa_api/__init__.py
--rw-r--r--  2.0 unx     4972 b- defN 23-Mar-20 14:31 ppa_api/_client.py
--rw-r--r--  2.0 unx    11706 b- defN 23-Mar-23 08:16 ppa_api/client.py
+-rw-r--r--  2.0 unx     4972 b- defN 23-Apr-14 10:13 ppa_api/_client.py
+-rw-r--r--  2.0 unx    11706 b- defN 23-Apr-14 10:13 ppa_api/client.py
 -rw-r--r--  2.0 unx     3645 b- defN 23-Feb-24 13:11 ppa_api/create.py
--rw-r--r--  2.0 unx     3478 b- defN 23-Feb-24 13:11 ppa_api/exceptions.py
--rw-r--r--  2.0 unx     1684 b- defN 23-Mar-23 08:12 ppa_api/models.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Mar-23 08:20 ppa_api-2.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      807 b- defN 23-Mar-23 08:20 ppa_api-2.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-23 08:20 ppa_api-2.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Mar-23 08:20 ppa_api-2.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      833 b- defN 23-Mar-23 08:20 ppa_api-2.6.0.dist-info/RECORD
-11 files, 28292 bytes uncompressed, 8409 bytes compressed:  70.3%
+-rw-r--r--  2.0 unx     3650 b- defN 23-Apr-14 10:20 ppa_api/exceptions.py
+-rw-r--r--  2.0 unx     1684 b- defN 23-Apr-14 10:13 ppa_api/models.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-14 10:21 ppa_api-2.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      807 b- defN 23-Apr-14 10:21 ppa_api-2.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 10:21 ppa_api-2.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-14 10:21 ppa_api-2.6.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      833 b- defN 23-Apr-14 10:21 ppa_api-2.6.1.dist-info/RECORD
+11 files, 28464 bytes uncompressed, 8456 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ppa_api/exceptions.py
 Comment: 
 
 Filename: ppa_api/models.py
 Comment: 
 
-Filename: ppa_api-2.6.0.dist-info/LICENSE
+Filename: ppa_api-2.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: ppa_api-2.6.0.dist-info/METADATA
+Filename: ppa_api-2.6.1.dist-info/METADATA
 Comment: 
 
-Filename: ppa_api-2.6.0.dist-info/WHEEL
+Filename: ppa_api-2.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: ppa_api-2.6.0.dist-info/top_level.txt
+Filename: ppa_api-2.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ppa_api-2.6.0.dist-info/RECORD
+Filename: ppa_api-2.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ppa_api/exceptions.py

```diff
@@ -19,31 +19,35 @@
         self.address = urljoin(
             prepend_scheme_if_needed(address, "https"),
             f"/backend/v1/{api}/{endpoint}" if api else f"/backend/v1/{endpoint}",
         )
         self.status_code = status_code
         self.response_json = response_json
 
-        # Response JSON looks like this:
+        # Response JSON usually looks like this:
         #
         # {
         #   'hint': 'application/json; charset=utf-8',
         #   'details': '{"message":"Invalid Kerberos configuration", "error": {"secret":["Invalid password"]}}'
         # }
         #
         # The 'details' key is a string so it needs to be JSON-loaded.
 
         self.details, self.message, self.error = None, None, None  # Defaults
         if details := self.response_json.get("details"):
             try:
                 self.details = json.loads(details)
                 # Setting these makes it easier to catch specific errors in the client methods.
-                self.message, self.error = [self.details.get(k) for k in ["message", "error"]]
+                if isinstance(self.details, dict):
+                    self.message, self.error = [self.details.get(k) for k in ["message", "error"]]
+                else:
+                    # Unexpected format, leave error & message as None.
+                    pass
             except json.JSONDecodeError:
-                # The details key is not JSON, take the raw string instead & leave details & message as None.
+                # The details key is not JSON, take the raw string & leave error & message as None.
                 self.details = details
             exception_message = (
                 f"({self.status_code}) Request to {self.address} failed: {self.details}"
             )
         else:
             exception_message = (
                 f"({self.status_code}) Request to {self.address} failed: {self.response_json}"
```

## Comparing `ppa_api-2.6.0.dist-info/LICENSE` & `ppa_api-2.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ppa_api-2.6.0.dist-info/METADATA` & `ppa_api-2.6.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppa-api
-Version: 2.6.0
+Version: 2.6.1
 Summary: UNKNOWN
 Home-page: https://github.com/tomguyatt/ppa-api
 Author: Osirium
 Author-email: supportdesk@osirium.com
 Maintainer: Tom Guyatt
 Maintainer-email: tom.guyatt@osirium.com
 License: UNKNOWN
```

