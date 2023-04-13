# Comparing `tmp/yotpy-0.0.7.tar.gz` & `tmp/yotpy-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.7.tar", last modified: Thu Apr 13 22:23:56 2023, max compression
+gzip compressed data, was "yotpy-0.0.71.tar", last modified: Thu Apr 13 22:28:44 2023, max compression
```

## Comparing `yotpy-0.0.7.tar` & `yotpy-0.0.71.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.7/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.7/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.7/LICENSE
--rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.7/README.md
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.7/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.7/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.7/docs/yotpy.html
--rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      317 2023-04-13 22:19:11.280037 yotpy-0.0.7/yotpy/__init__.py
--rw-r--r--   0        0        0    30626 2023-04-13 22:19:11.281058 yotpy-0.0.7/yotpy/core.py
--rw-r--r--   0        0        0     1883 2023-04-13 22:19:11.281572 yotpy-0.0.7/yotpy/exceptions.py
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 yotpy-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.71/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.71/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.71/LICENSE
+-rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.71/README.md
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.71/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.71/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.71/docs/yotpy.html
+-rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.71/pyproject.toml
+-rw-r--r--   0        0        0      318 2023-04-13 22:27:56.610493 yotpy-0.0.71/yotpy/__init__.py
+-rw-r--r--   0        0        0    30788 2023-04-13 22:27:35.135323 yotpy-0.0.71/yotpy/core.py
+-rw-r--r--   0        0        0     1953 2023-04-13 22:27:49.518980 yotpy-0.0.71/yotpy/exceptions.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 yotpy-0.0.71/PKG-INFO
```

### Comparing `yotpy-0.0.7/.github/workflows/static.yml` & `yotpy-0.0.71/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.7/LICENSE` & `yotpy-0.0.71/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.7/docs/search.js` & `yotpy-0.0.71/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.7/docs/yotpy.html` & `yotpy-0.0.71/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.7/pyproject.toml` & `yotpy-0.0.71/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.7/yotpy/core.py` & `yotpy-0.0.71/yotpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Include's the core YotpoAPIWrapper class. As well as the JSONTransformer class, which can be used in tandem to easier convert data for your needs.
+"""
+
+
 import asyncio
 import aiohttp
 
 from json import loads as json_loads
 from csv import DictWriter
 from io import StringIO
 from typing import AsyncGenerator, Iterator, Union, Optional, Callable, Union
```

### Comparing `yotpy-0.0.7/yotpy/exceptions.py` & `yotpy-0.0.71/yotpy/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Includes custom exceptions for use with the yotpy package.
+"""
 
 class CustomException(Exception):
     """A custom exception to be used with request processing utility methods."""
     pass
 
 class SessionNotCreatedError(CustomException):
     """Raised when the aiohttp.ClientSession has not been created before making a request."""
```

### Comparing `yotpy-0.0.7/PKG-INFO` & `yotpy-0.0.71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.7
+Version: 0.0.71
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

