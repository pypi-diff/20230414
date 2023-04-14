# Comparing `tmp/openapify-0.3.6.tar.gz` & `tmp/openapify-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapify-0.3.6.tar", last modified: Fri Apr 14 16:18:23 2023, max compression
+gzip compressed data, was "openapify-0.3.7.tar", last modified: Fri Apr 14 17:04:59 2023, max compression
```

## Comparing `openapify-0.3.6.tar` & `openapify-0.3.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 16:18:23.970220 openapify-0.3.6/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    10763 2023-04-11 22:14:24.000000 openapify-0.3.6/LICENSE
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30587 2023-04-14 16:18:23.969982 openapify-0.3.6/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    29724 2023-04-14 16:11:16.000000 openapify-0.3.6/README.md
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 16:18:23.966699 openapify-0.3.6/openapify/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      488 2023-04-12 20:02:29.000000 openapify-0.3.6/openapify/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 16:18:23.968898 openapify-0.3.6/openapify/core/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.6/openapify/core/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    15787 2023-04-14 15:56:53.000000 openapify-0.3.6/openapify/core/builder.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2120 2023-04-13 11:29:19.000000 openapify-0.3.6/openapify/core/const.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2247 2023-04-14 10:18:14.000000 openapify-0.3.6/openapify/core/document.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1720 2023-04-13 18:04:05.000000 openapify-0.3.6/openapify/core/jsonschema.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1971 2023-04-14 14:51:07.000000 openapify-0.3.6/openapify/core/models.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 16:18:23.969231 openapify-0.3.6/openapify/core/openapi/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.6/openapify/core/openapi/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5299 2023-04-14 15:52:57.000000 openapify-0.3.6/openapify/core/openapi/models.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5287 2023-04-14 15:56:53.000000 openapify-0.3.6/openapify/decorators.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 16:18:23.969432 openapify-0.3.6/openapify/ext/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.6/openapify/ext/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 16:18:23.969623 openapify-0.3.6/openapify/ext/web/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.6/openapify/ext/web/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4767 2023-04-11 22:14:24.000000 openapify-0.3.6/openapify/ext/web/aiohttp.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.6/openapify/py.typed
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 16:18:23.967532 openapify-0.3.6/openapify.egg-info/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30587 2023-04-14 16:18:23.000000 openapify-0.3.6/openapify.egg-info/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      613 2023-04-14 16:18:23.000000 openapify-0.3.6/openapify.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-14 16:18:23.000000 openapify-0.3.6/openapify.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-10 17:48:20.000000 openapify-0.3.6/openapify.egg-info/not-zip-safe
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       42 2023-04-14 16:18:23.000000 openapify-0.3.6/openapify.egg-info/requires.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-14 16:18:23.000000 openapify-0.3.6/openapify.egg-info/top_level.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      364 2023-04-10 08:32:02.000000 openapify-0.3.6/pyproject.toml
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-14 16:18:23.970260 openapify-0.3.6/setup.cfg
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1298 2023-04-14 16:17:43.000000 openapify-0.3.6/setup.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.368747 openapify-0.3.7/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    10763 2023-04-11 22:14:24.000000 openapify-0.3.7/LICENSE
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30587 2023-04-14 17:04:59.368608 openapify-0.3.7/PKG-INFO
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    29724 2023-04-14 16:11:16.000000 openapify-0.3.7/README.md
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.365456 openapify-0.3.7/openapify/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      488 2023-04-12 20:02:29.000000 openapify-0.3.7/openapify/__init__.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.367486 openapify-0.3.7/openapify/core/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.7/openapify/core/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    15787 2023-04-14 15:56:53.000000 openapify-0.3.7/openapify/core/builder.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2120 2023-04-13 11:29:19.000000 openapify-0.3.7/openapify/core/const.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2247 2023-04-14 10:18:14.000000 openapify-0.3.7/openapify/core/document.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1720 2023-04-13 18:04:05.000000 openapify-0.3.7/openapify/core/jsonschema.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1971 2023-04-14 14:51:07.000000 openapify-0.3.7/openapify/core/models.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.367805 openapify-0.3.7/openapify/core/openapi/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.7/openapify/core/openapi/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5299 2023-04-14 15:52:57.000000 openapify-0.3.7/openapify/core/openapi/models.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5399 2023-04-14 16:53:08.000000 openapify-0.3.7/openapify/decorators.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.368048 openapify-0.3.7/openapify/ext/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.7/openapify/ext/__init__.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.368237 openapify-0.3.7/openapify/ext/web/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.7/openapify/ext/web/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4767 2023-04-11 22:14:24.000000 openapify-0.3.7/openapify/ext/web/aiohttp.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.7/openapify/py.typed
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.366291 openapify-0.3.7/openapify.egg-info/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30587 2023-04-14 17:04:59.000000 openapify-0.3.7/openapify.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      613 2023-04-14 17:04:59.000000 openapify-0.3.7/openapify.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-14 17:04:59.000000 openapify-0.3.7/openapify.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-10 17:48:20.000000 openapify-0.3.7/openapify.egg-info/not-zip-safe
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       42 2023-04-14 17:04:59.000000 openapify-0.3.7/openapify.egg-info/requires.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-14 17:04:59.000000 openapify-0.3.7/openapify.egg-info/top_level.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      364 2023-04-10 08:32:02.000000 openapify-0.3.7/pyproject.toml
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-14 17:04:59.368785 openapify-0.3.7/setup.cfg
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1298 2023-04-14 17:03:09.000000 openapify-0.3.7/setup.py
```

### Comparing `openapify-0.3.6/LICENSE` & `openapify-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openapify-0.3.6/PKG-INFO` & `openapify-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.6
+Version: 0.3.7
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `openapify-0.3.6/README.md` & `openapify-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `openapify-0.3.6/openapify/core/builder.py` & `openapify-0.3.7/openapify/core/builder.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.6/openapify/core/const.py` & `openapify-0.3.7/openapify/core/const.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.6/openapify/core/document.py` & `openapify-0.3.7/openapify/core/document.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.6/openapify/core/jsonschema.py` & `openapify-0.3.7/openapify/core/jsonschema.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.6/openapify/core/models.py` & `openapify-0.3.7/openapify/core/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.6/openapify/core/openapi/models.py` & `openapify-0.3.7/openapify/core/openapi/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.6/openapify/decorators.py` & `openapify-0.3.7/openapify/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,71 +2,77 @@
     Any,
     Callable,
     List,
     Mapping,
     Optional,
     Sequence,
     Tuple,
-    Type,
     TypeVar,
     Union,
     overload,
 )
 
 from openapify.core.models import (
     Body,
     Cookie,
     Header,
     QueryParam,
     SecurityRequirement,
+    TypeAnnotation,
 )
 from openapify.core.openapi.models import Example, HttpCode
 
 __openapify__ = "__openapify__"
 
 
 Handler = TypeVar("Handler")
 
 
 @overload
 def request_schema(
     body: Optional[Body] = None,
     *,
-    query_params: Optional[Mapping[str, Union[Type, QueryParam]]] = None,
+    query_params: Optional[
+        Mapping[str, Union[TypeAnnotation, QueryParam]]
+    ] = None,
     headers: Optional[Mapping[str, Union[str, Header]]] = None,
     cookies: Optional[Mapping[str, Union[str, Cookie]]] = None,
 ) -> Callable[[Handler], Handler]:
     ...
 
 
 @overload
 def request_schema(
-    body: Optional[Type] = None,
+    body: Optional[TypeAnnotation] = None,
     *,
     media_type: str = "application/json",
     body_required: bool = False,
     body_description: Optional[str] = None,
     body_example: Optional[Any] = None,
     body_examples: Optional[Mapping[str, Union[Example, Any]]] = None,
-    query_params: Optional[Mapping[str, Union[Type, QueryParam]]] = None,
+    query_params: Optional[
+        Mapping[str, Union[TypeAnnotation, QueryParam]]
+    ] = None,
     headers: Optional[Mapping[str, Union[str, Header]]] = None,
     cookies: Optional[Mapping[str, Union[str, Cookie]]] = None,
 ) -> Callable[[Handler], Handler]:
     ...
 
 
 def request_schema(  # type: ignore[misc]
-    body: Optional[Type] = None,
+    body: Optional[TypeAnnotation] = None,
     *,
     media_type: str = "application/json",
     body_required: bool = False,
     body_description: Optional[str] = None,
     body_example: Optional[Any] = None,
     body_examples: Optional[Mapping[str, Union[Example, Any]]] = None,
-    query_params: Optional[Mapping[str, Union[Type, QueryParam]]] = None,
+    query_params: Optional[
+        Mapping[str, Union[TypeAnnotation, QueryParam]]
+    ] = None,
     headers: Optional[Mapping[str, Union[str, Header]]] = None,
     cookies: Optional[Mapping[str, Union[str, Cookie]]] = None,
 ) -> Callable[[Handler], Handler]:
     def decorator(handler: Handler) -> Handler:
         meta = getattr(handler, __openapify__, [])
         if not meta:
             handler.__openapify__ = meta  # type: ignore[attr-defined]
@@ -88,15 +94,15 @@
         )
         return handler
 
     return decorator
 
 
 def response_schema(
-    body: Optional[Type] = None,
+    body: Optional[TypeAnnotation] = None,
     http_code: HttpCode = 200,
     media_type: str = "application/json",
     description: Optional[str] = None,
     # TODO: Generate a required description depending on http_code
     # https://spec.openapis.org/oas/v3.1.0#response-object
     headers: Optional[Mapping[str, Union[str, Header]]] = None,
     example: Optional[Any] = None,
```

### Comparing `openapify-0.3.6/openapify/ext/web/aiohttp.py` & `openapify-0.3.7/openapify/ext/web/aiohttp.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.6/openapify.egg-info/PKG-INFO` & `openapify-0.3.7/openapify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.6
+Version: 0.3.7
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `openapify-0.3.6/openapify.egg-info/SOURCES.txt` & `openapify-0.3.7/openapify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openapify-0.3.6/setup.py` & `openapify-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="openapify",
-    version="0.3.6",
+    version="0.3.7",
     description=(
         "Framework agnostic OpenAPI Specification generation for code lovers"
     ),
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
```

