# Comparing `tmp/pydantic_aiohttp-0.7.0.tar.gz` & `tmp/pydantic_aiohttp-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_aiohttp-0.7.0.tar", max compression
+gzip compressed data, was "pydantic_aiohttp-0.7.1.tar", max compression
```

## Comparing `pydantic_aiohttp-0.7.0.tar` & `pydantic_aiohttp-0.7.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1865 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1064 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/LICENSE
--rw-r--r--   0        0        0     4527 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/README.md
--rw-r--r--   0        0        0      136 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/__init__.py
--rw-r--r--   0        0        0    11310 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/client.py
--rw-r--r--   0        0        0    11770 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/encoders.py
--rw-r--r--   0        0        0     8394 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/errors.py
--rw-r--r--   0        0        0     2375 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/responses.py
--rw-r--r--   0        0        0      506 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/types.py
--rw-r--r--   0        0        0     1664 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pydantic_aiohttp/utils.py
--rw-r--r--   0        0        0      967 2023-04-11 09:37:43.792677 pydantic_aiohttp-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 pydantic_aiohttp-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1992 2023-04-14 06:33:32.652866 pydantic_aiohttp-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1064 2023-04-14 06:33:32.652866 pydantic_aiohttp-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4527 2023-04-14 06:33:32.652866 pydantic_aiohttp-0.7.1/README.md
+-rw-r--r--   0        0        0      136 2023-04-14 06:33:32.652866 pydantic_aiohttp-0.7.1/pydantic_aiohttp/__init__.py
+-rw-r--r--   0        0        0    11310 2023-04-14 06:33:32.652866 pydantic_aiohttp-0.7.1/pydantic_aiohttp/client.py
+-rw-r--r--   0        0        0    11770 2023-04-14 06:33:32.652866 pydantic_aiohttp-0.7.1/pydantic_aiohttp/encoders.py
+-rw-r--r--   0        0        0     8394 2023-04-14 06:33:32.652866 pydantic_aiohttp-0.7.1/pydantic_aiohttp/errors.py
+-rw-r--r--   0        0        0     2547 2023-04-14 06:33:32.652866 pydantic_aiohttp-0.7.1/pydantic_aiohttp/responses.py
+-rw-r--r--   0        0        0      506 2023-04-14 06:33:32.652866 pydantic_aiohttp-0.7.1/pydantic_aiohttp/types.py
+-rw-r--r--   0        0        0     1664 2023-04-14 06:33:32.656866 pydantic_aiohttp-0.7.1/pydantic_aiohttp/utils.py
+-rw-r--r--   0        0        0      967 2023-04-14 06:33:32.656866 pydantic_aiohttp-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 pydantic_aiohttp-0.7.1/PKG-INFO
```

### Comparing `pydantic_aiohttp-0.7.0/CHANGELOG.md` & `pydantic_aiohttp-0.7.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 0.7.1
+
+* Added new `RawResponseClass` which returns raw `aiohttp.ClientResponse` instance with no modification and parsing
+
 ## 0.7.0
 
 ### **BREAKING**
 
 * All types moved from `client` to separate `types` module
 
 * Removed unused `error_response_class` from `Client` constructur parameters
```

### Comparing `pydantic_aiohttp-0.7.0/LICENSE` & `pydantic_aiohttp-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_aiohttp-0.7.0/README.md` & `pydantic_aiohttp-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_aiohttp-0.7.0/pydantic_aiohttp/client.py` & `pydantic_aiohttp-0.7.1/pydantic_aiohttp/client.py`

 * *Files identical despite different names*

### Comparing `pydantic_aiohttp-0.7.0/pydantic_aiohttp/encoders.py` & `pydantic_aiohttp-0.7.1/pydantic_aiohttp/encoders.py`

 * *Files identical despite different names*

### Comparing `pydantic_aiohttp-0.7.0/pydantic_aiohttp/errors.py` & `pydantic_aiohttp-0.7.1/pydantic_aiohttp/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_aiohttp-0.7.0/pydantic_aiohttp/responses.py` & `pydantic_aiohttp-0.7.1/pydantic_aiohttp/responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,7 +74,12 @@
             **kwargs
     ) -> PathLike:
         async with aiofiles.open(filepath, 'wb') as fd:
             async for chunk in self.aiohttp_response.content.iter_chunked(chunk_size):
                 await fd.write(chunk)
 
         return filepath
+
+
+class RawResponseClass(ResponseClass[aiohttp.ClientResponse]):
+    async def parse(self, *args, **kwargs) -> aiohttp.ClientResponse:
+        return self.aiohttp_response
```

### Comparing `pydantic_aiohttp-0.7.0/pydantic_aiohttp/utils.py` & `pydantic_aiohttp-0.7.1/pydantic_aiohttp/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_aiohttp-0.7.0/pyproject.toml` & `pydantic_aiohttp-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_aiohttp"
-version = "0.7.0"
+version = "0.7.1"
 description = "Simple HTTP Client based on aiohttp with integration of pydantic"
 authors = ["pylakey <pylakey@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pylakey/pydantic_aiohttp"
 repository = "https://github.com/pylakey/pydantic_aiohttp"
 packages = [
```

### Comparing `pydantic_aiohttp-0.7.0/PKG-INFO` & `pydantic_aiohttp-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-aiohttp
-Version: 0.7.0
+Version: 0.7.1
 Summary: Simple HTTP Client based on aiohttp with integration of pydantic
 Home-page: https://github.com/pylakey/pydantic_aiohttp
 License: MIT
 Author: pylakey
 Author-email: pylakey@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: AsyncIO
```

