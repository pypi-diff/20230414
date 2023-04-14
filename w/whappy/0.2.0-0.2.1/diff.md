# Comparing `tmp/whappy-0.2.0.tar.gz` & `tmp/whappy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whappy-0.2.0.tar", last modified: Fri Apr 14 20:17:25 2023, max compression
+gzip compressed data, was "whappy-0.2.1.tar", last modified: Fri Apr 14 20:24:21 2023, max compression
```

## Comparing `whappy-0.2.0.tar` & `whappy-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 harshraj  (1000) harshraj  (1000)        0 2023-04-14 20:17:25.543482 whappy-0.2.0/
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      585 2023-04-14 20:17:25.543482 whappy-0.2.0/PKG-INFO
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      138 2023-04-14 10:20:51.000000 whappy-0.2.0/README.md
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)       38 2023-04-14 20:17:25.543482 whappy-0.2.0/setup.cfg
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      758 2023-04-14 20:17:03.000000 whappy-0.2.0/setup.py
-drwxrwxr-x   0 harshraj  (1000) harshraj  (1000)        0 2023-04-14 20:17:25.543482 whappy-0.2.0/whappy/
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)       55 2023-04-14 10:28:59.000000 whappy-0.2.0/whappy/__init__.py
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)     1917 2023-04-14 19:17:38.000000 whappy-0.2.0/whappy/api.py
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)       66 2023-04-14 10:24:45.000000 whappy-0.2.0/whappy/constants.py
-drwxrwxr-x   0 harshraj  (1000) harshraj  (1000)        0 2023-04-14 20:17:25.543482 whappy-0.2.0/whappy.egg-info/
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      585 2023-04-14 20:17:25.000000 whappy-0.2.0/whappy.egg-info/PKG-INFO
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      220 2023-04-14 20:17:25.000000 whappy-0.2.0/whappy.egg-info/SOURCES.txt
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        1 2023-04-14 20:17:25.000000 whappy-0.2.0/whappy.egg-info/dependency_links.txt
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        9 2023-04-14 20:17:25.000000 whappy-0.2.0/whappy.egg-info/requires.txt
--rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        7 2023-04-14 20:17:25.000000 whappy-0.2.0/whappy.egg-info/top_level.txt
+drwxrwxr-x   0 harshraj  (1000) harshraj  (1000)        0 2023-04-14 20:24:21.022228 whappy-0.2.1/
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      585 2023-04-14 20:24:21.022228 whappy-0.2.1/PKG-INFO
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      138 2023-04-14 10:20:51.000000 whappy-0.2.1/README.md
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)       38 2023-04-14 20:24:21.022228 whappy-0.2.1/setup.cfg
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      758 2023-04-14 20:24:17.000000 whappy-0.2.1/setup.py
+drwxrwxr-x   0 harshraj  (1000) harshraj  (1000)        0 2023-04-14 20:24:21.018228 whappy-0.2.1/whappy/
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)       55 2023-04-14 10:28:59.000000 whappy-0.2.1/whappy/__init__.py
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)     1881 2023-04-14 20:23:24.000000 whappy-0.2.1/whappy/api.py
+drwxrwxr-x   0 harshraj  (1000) harshraj  (1000)        0 2023-04-14 20:24:21.022228 whappy-0.2.1/whappy.egg-info/
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      585 2023-04-14 20:24:20.000000 whappy-0.2.1/whappy.egg-info/PKG-INFO
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)      200 2023-04-14 20:24:21.000000 whappy-0.2.1/whappy.egg-info/SOURCES.txt
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        1 2023-04-14 20:24:20.000000 whappy-0.2.1/whappy.egg-info/dependency_links.txt
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        9 2023-04-14 20:24:20.000000 whappy-0.2.1/whappy.egg-info/requires.txt
+-rw-rw-r--   0 harshraj  (1000) harshraj  (1000)        7 2023-04-14 20:24:20.000000 whappy-0.2.1/whappy.egg-info/top_level.txt
```

### Comparing `whappy-0.2.0/PKG-INFO` & `whappy-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whappy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python wrapper for WhatsApp API
 Home-page: https://github.com/saketharshraj/whappy
 Author: Harsh Raj
 Author-email: saketharshraj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `whappy-0.2.0/setup.py` & `whappy-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="whappy",
-    version="0.2.0",
+    version="0.2.1",
     author="Harsh Raj",
     author_email="saketharshraj@gmail.com",
     description="A Python wrapper for WhatsApp API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/saketharshraj/whappy",
     packages=find_packages(),
```

### Comparing `whappy-0.2.0/whappy/api.py` & `whappy-0.2.1/whappy/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from constants import WHATSAPP_API_URL, VERSION
 import requests
 import json
 
 class WhatsAppAPI:
-    def __init__(self, api_key: str, phone_number_id: int or str, api_version: str = VERSION, API_URL: str = WHATSAPP_API_URL)->None:
+    def __init__(self, api_key: str, phone_number_id: int or str, api_version: str = 'v16.0', API_URL: str = 'https://graph.facebook.com')->None:
         self.api_key: str = api_key
         self.phone_number_id: int = phone_number_id
         self.headers: dict = {
             "Content-Type": "application/json",
             "Authorization": f'Bearer {api_key}'
         }
         self.API_URL: str = API_URL
```

### Comparing `whappy-0.2.0/whappy.egg-info/PKG-INFO` & `whappy-0.2.1/whappy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whappy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python wrapper for WhatsApp API
 Home-page: https://github.com/saketharshraj/whappy
 Author: Harsh Raj
 Author-email: saketharshraj@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

