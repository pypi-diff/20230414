# Comparing `tmp/tap_messagebird-0.0.4.tar.gz` & `tmp/tap_messagebird-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_messagebird-0.0.4.tar", max compression
+gzip compressed data, was "tap_messagebird-0.0.5.tar", max compression
```

## Comparing `tap_messagebird-0.0.4.tar` & `tap_messagebird-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-04-12 18:16:04.808337 tap_messagebird-0.0.4/LICENSE
--rw-r--r--   0        0        0     3370 2023-04-12 18:16:04.808489 tap_messagebird-0.0.4/README.md
--rw-r--r--   0        0        0     1163 2023-04-13 23:10:07.507351 tap_messagebird-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      117 2023-04-13 23:10:07.509758 tap_messagebird-0.0.4/tap_messagebird/__init__.py
--rw-r--r--   0        0        0     3857 2023-04-13 23:10:02.016492 tap_messagebird-0.0.4/tap_messagebird/client.py
--rw-r--r--   0        0        0     3044 2023-04-12 18:16:04.810379 tap_messagebird-0.0.4/tap_messagebird/schemas/conversation.json
--rw-r--r--   0        0        0      993 2023-04-12 18:16:04.810653 tap_messagebird-0.0.4/tap_messagebird/schemas/conversation_message.json
--rw-r--r--   0        0        0     4240 2023-04-12 18:16:04.810963 tap_messagebird-0.0.4/tap_messagebird/schemas/message.json
--rw-r--r--   0        0        0     3621 2023-04-13 23:10:02.017188 tap_messagebird-0.0.4/tap_messagebird/streams.py
--rw-r--r--   0        0        0     1590 2023-04-13 23:10:02.017861 tap_messagebird-0.0.4/tap_messagebird/tap.py
--rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 tap_messagebird-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3370 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/README.md
+-rw-r--r--   0        0        0     1163 2023-04-13 13:13:33.065255 tap_messagebird-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      117 2023-04-13 13:13:33.069254 tap_messagebird-0.0.5/tap_messagebird/__init__.py
+-rw-r--r--   0        0        0     3857 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/client.py
+-rw-r--r--   0        0        0     3044 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/schemas/conversation.json
+-rw-r--r--   0        0        0      993 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/schemas/conversation_message.json
+-rw-r--r--   0        0        0     4240 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/schemas/message.json
+-rw-r--r--   0        0        0     3621 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/streams.py
+-rw-r--r--   0        0        0     1590 2023-04-13 13:13:01.769345 tap_messagebird-0.0.5/tap_messagebird/tap.py
+-rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 tap_messagebird-0.0.5/PKG-INFO
```

### Comparing `tap_messagebird-0.0.4/LICENSE` & `tap_messagebird-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.4/README.md` & `tap_messagebird-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.4/pyproject.toml` & `tap_messagebird-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-messagebird"
-version = "0.0.4"
+version = "0.0.5"
 description = "`tap-messagebird` is a Singer tap for Messagebird, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Meltano Team <hello@meltano.com>"]
 keywords = [
     "ELT",
     "Messagebird",
 ]
```

### Comparing `tap_messagebird-0.0.4/tap_messagebird/client.py` & `tap_messagebird-0.0.5/tap_messagebird/client.py`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.4/tap_messagebird/schemas/conversation.json` & `tap_messagebird-0.0.5/tap_messagebird/schemas/conversation.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.4/tap_messagebird/schemas/conversation_message.json` & `tap_messagebird-0.0.5/tap_messagebird/schemas/conversation_message.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.4/tap_messagebird/schemas/message.json` & `tap_messagebird-0.0.5/tap_messagebird/schemas/message.json`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.4/tap_messagebird/streams.py` & `tap_messagebird-0.0.5/tap_messagebird/streams.py`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.4/tap_messagebird/tap.py` & `tap_messagebird-0.0.5/tap_messagebird/tap.py`

 * *Files identical despite different names*

### Comparing `tap_messagebird-0.0.4/PKG-INFO` & `tap_messagebird-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-messagebird
-Version: 0.0.4
+Version: 0.0.5
 Summary: `tap-messagebird` is a Singer tap for Messagebird, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Messagebird
 Author: Meltano Team
 Author-email: hello@meltano.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
```

