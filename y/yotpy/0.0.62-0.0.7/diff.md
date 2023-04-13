# Comparing `tmp/yotpy-0.0.62.tar.gz` & `tmp/yotpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yotpy-0.0.62.tar", last modified: Thu Apr 13 15:04:03 2023, max compression
+gzip compressed data, was "yotpy-0.0.7.tar", last modified: Thu Apr 13 22:23:56 2023, max compression
```

## Comparing `yotpy-0.0.62.tar` & `yotpy-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.62/.github/workflows/static.yml
--rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.62/.gitignore
--rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.62/LICENSE
--rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.62/README.md
--rw-r--r--   0        0        0        0 2023-04-12 23:07:55.942421 yotpy-0.0.62/__init__.py
--rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.62/docs/index.html
--rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.62/docs/search.js
--rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.62/docs/yotpy.html
--rw-r--r--   0        0        0     1883 2023-04-12 22:50:16.599595 yotpy-0.0.62/exceptions.py
--rw-r--r--   0        0        0      830 2023-04-12 22:19:29.450917 yotpy-0.0.62/pyproject.toml
--rw-r--r--   0        0        0    30725 2023-04-13 15:03:16.110425 yotpy-0.0.62/yotpy.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 yotpy-0.0.62/PKG-INFO
+-rw-r--r--   0        0        0      893 2023-04-12 23:14:08.203084 yotpy-0.0.7/.github/workflows/static.yml
+-rw-r--r--   0        0        0      316 2023-04-12 22:41:53.693273 yotpy-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1085 2023-04-11 18:17:34.364138 yotpy-0.0.7/LICENSE
+-rw-r--r--   0        0        0      223 2023-04-11 18:50:45.784541 yotpy-0.0.7/README.md
+-rw-r--r--   0        0        0      136 2023-04-12 22:59:50.105965 yotpy-0.0.7/docs/index.html
+-rw-r--r--   0        0        0   178839 2023-04-12 22:59:50.175644 yotpy-0.0.7/docs/search.js
+-rw-r--r--   0        0        0   491392 2023-04-12 22:59:50.101919 yotpy-0.0.7/docs/yotpy.html
+-rw-r--r--   0        0        0      830 2023-04-13 22:15:48.351075 yotpy-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      317 2023-04-13 22:19:11.280037 yotpy-0.0.7/yotpy/__init__.py
+-rw-r--r--   0        0        0    30626 2023-04-13 22:19:11.281058 yotpy-0.0.7/yotpy/core.py
+-rw-r--r--   0        0        0     1883 2023-04-13 22:19:11.281572 yotpy-0.0.7/yotpy/exceptions.py
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 yotpy-0.0.7/PKG-INFO
```

### Comparing `yotpy-0.0.62/.github/workflows/static.yml` & `yotpy-0.0.7/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.62/LICENSE` & `yotpy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.62/docs/search.js` & `yotpy-0.0.7/docs/search.js`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.62/docs/yotpy.html` & `yotpy-0.0.7/docs/yotpy.html`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.62/exceptions.py` & `yotpy-0.0.7/yotpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.62/pyproject.toml` & `yotpy-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yotpy-0.0.62/yotpy.py` & `yotpy-0.0.7/yotpy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-"""
-Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
-"""
-
-__version__ = "0.0.62"
-
 import asyncio
 import aiohttp
 
 from json import loads as json_loads
 from csv import DictWriter
 from io import StringIO
 from typing import AsyncGenerator, Iterator, Union, Optional, Callable, Union
```

### Comparing `yotpy-0.0.62/PKG-INFO` & `yotpy-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yotpy
-Version: 0.0.62
+Version: 0.0.7
 Summary: Yotpy: An easy-to-use Python wrapper for the Yotpo web API.
 Home-page: https://github.com/wlk-dev/yotpy
 License: MIT
 Keywords: yotpo, api, wrapper, python, data, transformation, client, integration, review, ecommerce
 Author: William Koelling
 Author-email: william.koelling@gmail.com
 Description-Content-Type: text/markdown
```

