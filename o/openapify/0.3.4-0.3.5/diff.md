# Comparing `tmp/openapify-0.3.4.tar.gz` & `tmp/openapify-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapify-0.3.4.tar", last modified: Thu Apr 13 11:18:36 2023, max compression
+gzip compressed data, was "openapify-0.3.5.tar", last modified: Thu Apr 13 19:05:48 2023, max compression
```

## Comparing `openapify-0.3.4.tar` & `openapify-0.3.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.663397 openapify-0.3.4/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-04-11 15:10:01.000000 openapify-0.3.4/LICENSE
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    30260 2023-04-13 11:18:36.663248 openapify-0.3.4/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    29397 2023-04-12 18:43:50.000000 openapify-0.3.4/README.md
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.660069 openapify-0.3.4/openapify/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      488 2023-04-12 18:41:02.000000 openapify-0.3.4/openapify/__init__.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.662005 openapify-0.3.4/openapify/core/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-04-03 13:14:57.000000 openapify-0.3.4/openapify/core/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    15575 2023-04-13 11:17:48.000000 openapify-0.3.4/openapify/core/builder.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2120 2023-04-13 11:17:48.000000 openapify-0.3.4/openapify/core/const.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2018 2023-04-12 18:41:02.000000 openapify-0.3.4/openapify/core/document.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1630 2023-04-09 15:42:39.000000 openapify-0.3.4/openapify/core/jsonschema.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1748 2023-04-09 15:04:29.000000 openapify-0.3.4/openapify/core/models.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.662345 openapify-0.3.4/openapify/core/openapi/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-20 12:12:59.000000 openapify-0.3.4/openapify/core/openapi/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5261 2023-04-13 10:15:38.000000 openapify-0.3.4/openapify/core/openapi/models.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5197 2023-04-12 18:41:02.000000 openapify-0.3.4/openapify/decorators.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.662562 openapify-0.3.4/openapify/ext/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 15:48:32.000000 openapify-0.3.4/openapify/ext/__init__.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.662735 openapify-0.3.4/openapify/ext/web/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-18 09:45:46.000000 openapify-0.3.4/openapify/ext/web/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     4767 2023-04-11 10:22:05.000000 openapify-0.3.4/openapify/ext/web/aiohttp.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-03-17 11:19:37.000000 openapify-0.3.4/openapify/py.typed
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-04-13 11:18:36.660891 openapify-0.3.4/openapify.egg-info/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    30260 2023-04-13 11:18:36.000000 openapify-0.3.4/openapify.egg-info/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      613 2023-04-13 11:18:36.000000 openapify-0.3.4/openapify.egg-info/SOURCES.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-13 11:18:36.000000 openapify-0.3.4/openapify.egg-info/dependency_links.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-04-11 15:01:19.000000 openapify-0.3.4/openapify.egg-info/not-zip-safe
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       42 2023-04-13 11:18:36.000000 openapify-0.3.4/openapify.egg-info/requires.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-04-13 11:18:36.000000 openapify-0.3.4/openapify.egg-info/top_level.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      364 2023-04-07 11:44:47.000000 openapify-0.3.4/pyproject.toml
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-04-13 11:18:36.663433 openapify-0.3.4/setup.cfg
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1298 2023-04-13 11:18:03.000000 openapify-0.3.4/setup.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 19:05:48.728789 openapify-0.3.5/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    10763 2023-04-11 22:14:24.000000 openapify-0.3.5/LICENSE
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30292 2023-04-13 19:05:48.728650 openapify-0.3.5/PKG-INFO
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    29429 2023-04-13 11:29:19.000000 openapify-0.3.5/README.md
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 19:05:48.725611 openapify-0.3.5/openapify/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      488 2023-04-12 20:02:29.000000 openapify-0.3.5/openapify/__init__.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 19:05:48.727574 openapify-0.3.5/openapify/core/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.5/openapify/core/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    15657 2023-04-13 18:37:41.000000 openapify-0.3.5/openapify/core/builder.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2120 2023-04-13 11:29:19.000000 openapify-0.3.5/openapify/core/const.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2018 2023-04-12 20:02:29.000000 openapify-0.3.5/openapify/core/document.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1720 2023-04-13 18:04:05.000000 openapify-0.3.5/openapify/core/jsonschema.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1863 2023-04-13 14:38:41.000000 openapify-0.3.5/openapify/core/models.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 19:05:48.727888 openapify-0.3.5/openapify/core/openapi/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.5/openapify/core/openapi/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5261 2023-04-13 11:29:19.000000 openapify-0.3.5/openapify/core/openapi/models.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5197 2023-04-12 20:02:29.000000 openapify-0.3.5/openapify/decorators.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 19:05:48.728110 openapify-0.3.5/openapify/ext/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.5/openapify/ext/__init__.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 19:05:48.728297 openapify-0.3.5/openapify/ext/web/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.5/openapify/ext/web/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4767 2023-04-11 22:14:24.000000 openapify-0.3.5/openapify/ext/web/aiohttp.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.5/openapify/py.typed
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-13 19:05:48.726439 openapify-0.3.5/openapify.egg-info/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30292 2023-04-13 19:05:48.000000 openapify-0.3.5/openapify.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      613 2023-04-13 19:05:48.000000 openapify-0.3.5/openapify.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-13 19:05:48.000000 openapify-0.3.5/openapify.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-10 17:48:20.000000 openapify-0.3.5/openapify.egg-info/not-zip-safe
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       42 2023-04-13 19:05:48.000000 openapify-0.3.5/openapify.egg-info/requires.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-13 19:05:48.000000 openapify-0.3.5/openapify.egg-info/top_level.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      364 2023-04-10 08:32:02.000000 openapify-0.3.5/pyproject.toml
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-13 19:05:48.728825 openapify-0.3.5/setup.cfg
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1298 2023-04-13 19:03:11.000000 openapify-0.3.5/setup.py
```

### Comparing `openapify-0.3.4/LICENSE` & `openapify-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openapify-0.3.4/PKG-INFO` & `openapify-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: openapify
-Version: 0.3.4
-Summary: Framework agnostic OpenAPI Specification generation for code lovers
-Home-page: https://github.com/Fatal1ty/openapify
-Author: Alexander Tikhonov
-Author-email: random.gauss@gmail.com
-License: Apache License, Version 2.0
-Platform: all
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: aiohttp
-License-File: LICENSE
-
 # openapify
 
 ###### Framework agnostic OpenAPI Specification generation for code lovers
 
 [![Build Status](https://github.com/Fatal1ty/openapify/workflows/tests/badge.svg)](https://github.com/Fatal1ty/openapify/actions)
 [![Latest Version](https://img.shields.io/pypi/v/openapify.svg)](https://pypi.python.org/pypi/openapify)
 [![Python Version](https://img.shields.io/pypi/pyversions/openapify.svg)](https://pypi.python.org/pypi/openapify)
@@ -146,14 +123,15 @@
       parameters:
       - name: count
         in: query
         schema:
           type: integer
       responses:
         '200':
+          description: OK
           content:
             application/json:
               schema:
                 type: array
                 items:
                   $ref: '#/components/schemas/Book'
 components:
@@ -332,14 +310,15 @@
   title: API
   version: 1.0.0
 paths:
   /:
     post:
       responses:
         '200':
+          description: OK
           content:
             text/plain:
               schema:
                 type: string
 ```
 
 ### Writing your own integration
@@ -1045,15 +1024,14 @@
 openapi: 3.1.0
 info:
   title: API
   version: 1.0.0
 paths:
   /secure_path:
     get:
-      responses: {}
       security:
       - x-auth-token: []
 components:
   securitySchemes:
     x-auth-token:
       type: apiKey
       name: X-Auh-Token
```

### Comparing `openapify-0.3.4/README.md` & `openapify-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: openapify
+Version: 0.3.5
+Summary: Framework agnostic OpenAPI Specification generation for code lovers
+Home-page: https://github.com/Fatal1ty/openapify
+Author: Alexander Tikhonov
+Author-email: random.gauss@gmail.com
+License: Apache License, Version 2.0
+Platform: all
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: aiohttp
+License-File: LICENSE
+
 # openapify
 
 ###### Framework agnostic OpenAPI Specification generation for code lovers
 
 [![Build Status](https://github.com/Fatal1ty/openapify/workflows/tests/badge.svg)](https://github.com/Fatal1ty/openapify/actions)
 [![Latest Version](https://img.shields.io/pypi/v/openapify.svg)](https://pypi.python.org/pypi/openapify)
 [![Python Version](https://img.shields.io/pypi/pyversions/openapify.svg)](https://pypi.python.org/pypi/openapify)
@@ -123,14 +146,15 @@
       parameters:
       - name: count
         in: query
         schema:
           type: integer
       responses:
         '200':
+          description: OK
           content:
             application/json:
               schema:
                 type: array
                 items:
                   $ref: '#/components/schemas/Book'
 components:
@@ -309,14 +333,15 @@
   title: API
   version: 1.0.0
 paths:
   /:
     post:
       responses:
         '200':
+          description: OK
           content:
             text/plain:
               schema:
                 type: string
 ```
 
 ### Writing your own integration
@@ -1022,15 +1047,14 @@
 openapi: 3.1.0
 info:
   title: API
   version: 1.0.0
 paths:
   /secure_path:
     get:
-      responses: {}
       security:
       - x-auth-token: []
 components:
   securitySchemes:
     x-auth-token:
       type: apiKey
       name: X-Auh-Token
```

### Comparing `openapify-0.3.4/openapify/core/builder.py` & `openapify-0.3.5/openapify/core/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,16 @@
                     name=name,
                     location=openapi.ParameterLocation.QUERY,
                     description=param.description,
                     required=param.required,
                     deprecated=param.deprecated,
                     allowEmptyValue=param.allowEmptyValue,
                     schema=parameter_schema,
+                    style=param.style,
+                    explode=param.explode,
                     example=param.example,
                     examples=self._build_examples(param.examples),
                 )
             )
         return result
 
     def _build_request_headers(
```

### Comparing `openapify-0.3.4/openapify/core/const.py` & `openapify-0.3.5/openapify/core/const.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.4/openapify/core/document.py` & `openapify-0.3.5/openapify/core/document.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.4/openapify/core/jsonschema.py` & `openapify-0.3.5/openapify/core/jsonschema.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 
 
 def _build_json_schema_with_mashumaro(
     instance_type: Type,
     spec: Optional[APISpec] = None,
     component_type: ComponentType = ComponentType.SCHEMA,
 ) -> Optional[Dict[str, Any]]:
-    builder = JSONSchemaBuilder(dialect=OPEN_API_3_1)
+    builder = JSONSchemaBuilder(
+        dialect=OPEN_API_3_1,
+        ref_prefix=f"#/components/{ComponentTypeSpecKey[component_type]}",
+    )
     try:
         json_schema = builder.build(instance_type)
     except Exception:
         return None
     if spec is not None:
         scope = getattr(spec.components, ComponentTypeSpecKey[component_type])
         for name, schema in builder.context.definitions.items():
```

### Comparing `openapify-0.3.4/openapify/core/models.py` & `openapify-0.3.5/openapify/core/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from dataclasses import dataclass
 from typing import Any, List, Mapping, NamedTuple, Optional, Type, Union
 
 from typing_extensions import TypeAlias
 
-from openapify.core.openapi.models import Example, Parameter, SecurityScheme
+from openapify.core.openapi.models import (
+    Example,
+    Parameter,
+    ParameterStyle,
+    SecurityScheme,
+)
 
 SecurityRequirement: TypeAlias = Mapping[str, "SecurityScheme"]
 
 
 @dataclass
 class RouteDef:
     path: str
@@ -54,9 +59,11 @@
 class QueryParam:
     value_type: Type = str
     default: Optional[Any] = None
     required: Optional[bool] = None
     description: Optional[str] = None
     deprecated: Optional[bool] = None
     allowEmptyValue: Optional[bool] = None
+    style: Optional[ParameterStyle] = None
+    explode: Optional[bool] = None
     example: Optional[Any] = None
     examples: Optional[Mapping[str, Union[Example, Any]]] = None
```

### Comparing `openapify-0.3.4/openapify/core/openapi/models.py` & `openapify-0.3.5/openapify/core/openapi/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.4/openapify/decorators.py` & `openapify-0.3.5/openapify/decorators.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.4/openapify/ext/web/aiohttp.py` & `openapify-0.3.5/openapify/ext/web/aiohttp.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.4/openapify.egg-info/PKG-INFO` & `openapify-0.3.5/openapify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.4
+Version: 0.3.5
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -146,14 +146,15 @@
       parameters:
       - name: count
         in: query
         schema:
           type: integer
       responses:
         '200':
+          description: OK
           content:
             application/json:
               schema:
                 type: array
                 items:
                   $ref: '#/components/schemas/Book'
 components:
@@ -332,14 +333,15 @@
   title: API
   version: 1.0.0
 paths:
   /:
     post:
       responses:
         '200':
+          description: OK
           content:
             text/plain:
               schema:
                 type: string
 ```
 
 ### Writing your own integration
@@ -1045,15 +1047,14 @@
 openapi: 3.1.0
 info:
   title: API
   version: 1.0.0
 paths:
   /secure_path:
     get:
-      responses: {}
       security:
       - x-auth-token: []
 components:
   securitySchemes:
     x-auth-token:
       type: apiKey
       name: X-Auh-Token
```

### Comparing `openapify-0.3.4/openapify.egg-info/SOURCES.txt` & `openapify-0.3.5/openapify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openapify-0.3.4/setup.py` & `openapify-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="openapify",
-    version="0.3.4",
+    version="0.3.5",
     description=(
         "Framework agnostic OpenAPI Specification generation for code lovers"
     ),
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
@@ -27,14 +27,14 @@
     author_email="random.gauss@gmail.com",
     url="https://github.com/Fatal1ty/openapify",
     packages=find_packages(include=("openapify", "openapify.*")),
     package_data={"openapify": ["py.typed"]},
     python_requires=">=3.7",
     install_requires=[
         "apispec",
-        "mashumaro>=3.6",
+        "mashumaro>=3.7",
     ],
     extras_require={
         "aiohttp": ["aiohttp"],
     },
     zip_safe=False,
 )
```

