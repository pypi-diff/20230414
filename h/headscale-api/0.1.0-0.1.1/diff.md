# Comparing `tmp/headscale_api-0.1.0.tar.gz` & `tmp/headscale_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headscale_api-0.1.0.tar", max compression
+gzip compressed data, was "headscale_api-0.1.1.tar", max compression
```

## Comparing `headscale_api-0.1.0.tar` & `headscale_api-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-04-05 14:11:04.015295 headscale_api-0.1.0/LICENSE
--rw-r--r--   0        0        0       68 2023-04-05 14:11:04.015295 headscale_api-0.1.0/README.md
--rw-r--r--   0        0        0      391 2023-04-05 14:11:04.015295 headscale_api-0.1.0/headscale_api/__init__.py
--rw-r--r--   0        0        0      449 2023-04-05 14:11:04.015295 headscale_api-0.1.0/headscale_api/config.py
--rw-r--r--   0        0        0     9594 2023-04-05 14:11:04.015295 headscale_api-0.1.0/headscale_api/endpoints.py
--rw-r--r--   0        0        0     5603 2023-04-05 14:11:04.015295 headscale_api-0.1.0/headscale_api/headscale.py
--rw-r--r--   0        0        0        0 2023-04-05 14:11:04.015295 headscale_api-0.1.0/headscale_api/py.typed
--rw-r--r--   0        0        0        0 2023-04-05 14:11:04.015295 headscale_api-0.1.0/headscale_api/schema/__init__.py
--rw-r--r--   0        0        0     3967 2023-04-05 14:11:04.015295 headscale_api-0.1.0/headscale_api/schema/config.py
--rw-r--r--   0        0        0        0 2023-04-05 14:11:04.015295 headscale_api-0.1.0/headscale_api/schema/google/__init__.py
--rw-r--r--   0        0        0    14509 2023-04-05 14:11:04.019295 headscale_api-0.1.0/headscale_api/schema/google/api.py
--rw-r--r--   0        0        0        0 2023-04-05 14:11:04.019295 headscale_api-0.1.0/headscale_api/schema/headscale/__init__.py
--rw-r--r--   0        0        0    20923 2023-04-05 14:11:04.019295 headscale_api-0.1.0/headscale_api/schema/headscale/v1.py
--rw-r--r--   0        0        0     1555 2023-04-05 14:11:04.019295 headscale_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 headscale_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-13 22:41:45.194685 headscale_api-0.1.1/LICENSE
+-rw-r--r--   0        0        0       68 2023-04-13 22:41:45.194685 headscale_api-0.1.1/README.md
+-rw-r--r--   0        0        0      447 2023-04-13 22:41:45.194685 headscale_api-0.1.1/headscale_api/__init__.py
+-rw-r--r--   0        0        0      428 2023-04-13 22:41:45.194685 headscale_api-0.1.1/headscale_api/config.py
+-rw-r--r--   0        0        0     9775 2023-04-13 22:41:45.194685 headscale_api-0.1.1/headscale_api/endpoints.py
+-rw-r--r--   0        0        0     6179 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/headscale.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/py.typed
+-rw-r--r--   0        0        0        0 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/__init__.py
+-rw-r--r--   0        0        0     3967 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/config.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/google/__init__.py
+-rw-r--r--   0        0        0    15302 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/google/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/headscale/__init__.py
+-rw-r--r--   0        0        0    48167 2023-04-13 22:41:45.198685 headscale_api-0.1.1/headscale_api/schema/headscale/v1/__init__.py
+-rw-r--r--   0        0        0     1684 2023-04-13 22:41:45.198685 headscale_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 headscale_api-0.1.1/PKG-INFO
```

### Comparing `headscale_api-0.1.0/LICENSE` & `headscale_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.0/headscale_api/endpoints.py` & `headscale_api-0.1.1/headscale_api/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Headscale API endpoint information."""
 
 __authors__ = ["Marek Pikuła <marek@serenitycode.dev>"]
 
 from dataclasses import dataclass
-from typing import Any, Dict, Generic, Literal, Optional, Type, TypeVar
+from typing import Generic, Literal, Optional, Type, TypeVar
 
-from betterproto import Message
+from betterproto import Message, ProtoClassMetadata
+from betterproto.casing import camel_case
 
 from .schema.headscale import v1 as schema
 
 RequestT = TypeVar("RequestT", bound=Message)
 ResponseT = TypeVar("ResponseT", bound=Message)
 
 
@@ -80,20 +81,25 @@
 
     def check_logger_format(self):
         """Check logger format for wrong keys.
 
         Raises:
             KeyError: if unsupported key is detected in the message.
         """
-        request_dict: Dict[str, Any] = self.request_schema().to_dict(  # type: ignore
-            include_default_values=True
-        )
-        response_dict: Dict[str, Any] = self.response_schema().to_dict(  # type: ignore
-            include_default_values=True
-        )
+
+        def schema_to_dict(schema_class: Type[Message]):
+            return {
+                camel_case(field_name).rstrip("_"): ""
+                for field_name, _ in ProtoClassMetadata(
+                    schema_class
+                ).meta_by_field_name.items()
+            }
+
+        request_dict = schema_to_dict(self.request_schema)
+        response_dict = schema_to_dict(self.response_schema)
 
         self.api_url.format_map(request_dict)
         self.logger_start_message.format_map(request_dict)
 
         if self.logger_success_message is not None:
             self.logger_success_message.format_map(dict(request_dict, **response_dict))
```

### Comparing `headscale_api-0.1.0/headscale_api/headscale.py` & `headscale_api-0.1.1/headscale_api/headscale.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Headscale API abstraction."""
 
 __authors__ = ["Marek Pikuła <marek@serenitycode.dev>"]
 
 import logging
 from dataclasses import dataclass
 from json import JSONDecodeError
-from typing import Any, Dict, List, Optional, Type, TypeVar, Union
+from typing import Any, Dict, Generator, List, Optional, Tuple, Type, TypeVar, Union
 
 import requests
 from betterproto import Message
+from betterproto.casing import safe_snake_case
 
 from .endpoints import ENDPOINTS, Endpoint
 from .schema.headscale import v1 as model
 
 
 @dataclass
 class ErrorResponse(RuntimeError):
@@ -89,15 +90,27 @@
                 "Accept": "application/json",
                 "Authorization": f"Bearer {new_api_key}",
             },
             timeout=self.timeout,
         )
         return response.status_code == 200
 
-    async def _unary_unary(
+    def _safe_snake_case_recursive(
+        self, dictionary: Dict[Any, Any]
+    ) -> Generator[Tuple[Any, Any], None, None]:
+        assert isinstance(dictionary, dict)
+        for key, value in dictionary.items():
+            if isinstance(value, dict):
+                yield key, dict(self._safe_snake_case_recursive(value))  # type: ignore
+            elif isinstance(key, str):
+                yield safe_snake_case(key), value
+            else:
+                yield key, value
+
+    async def _unary_unary(  # type: ignore
         self,
         route: str,
         request: Message,
         response_type: Type[MessageT],
         *,
         timeout: Optional[Any] = None,
         deadline: Optional[Any] = None,
@@ -123,15 +136,15 @@
             endpoint.request_type,
             f"{self._base_url}{api_url}",
             params=request_dict,
             headers={
                 "Accept": "application/json",
                 "Authorization": f"Bearer {self.api_key}",
             },
-            timeout=self.timeout,
+            timeout=self.timeout if timeout is None else timeout,
         )
 
         def error_message():
             message = (
                 endpoint.logger_fail_message.format_map(request_dict)
                 if endpoint.logger_fail_message is not None
                 else f'Request to "{api_url}" failed.'
@@ -145,17 +158,16 @@
                 raise ErrorResponse(**response.json())
             except JSONDecodeError as error:
                 raise ErrorResponse(
                     response.status_code, response.content.decode(), []
                 ) from error
 
         try:
-            response_dict = response.json()
-            assert isinstance(response_dict, dict)
-            response_parsed = response_type().from_dict(response_dict)  # type: ignore
+            response_dict = dict(self._safe_snake_case_recursive(response.json()))
+            response_parsed = response_type(**response_dict)  # type: ignore
         except (JSONDecodeError, AssertionError, ValueError) as error:
             raise ErrorResponse(response.status_code, error_message(), []) from error
 
         if endpoint.logger_success_message is not None:
             self._logger.info(
                 endpoint.logger_success_message.format_map(
                     dict(request_dict, **response_dict)
```

### Comparing `headscale_api-0.1.0/headscale_api/schema/config.py` & `headscale_api-0.1.1/headscale_api/schema/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  config-example.yaml
-#   timestamp: 2023-04-04T19:48:32+00:00
+#   timestamp: 2023-04-13T20:47:48+00:00
 
 from __future__ import annotations
 
 from typing import List, Optional
 
 from pydantic import BaseModel, Extra
```

### Comparing `headscale_api-0.1.0/headscale_api/schema/google/api.py` & `headscale_api-0.1.1/headscale_api/schema/google/api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: google/api/http.proto, google/api/annotations.proto
+# sources: google/api/annotations.proto, google/api/http.proto
 # plugin: python-betterproto
-from dataclasses import dataclass
-from typing import List
+# This file has been @generated
+
+from typing import TYPE_CHECKING
+
+
+if TYPE_CHECKING:
+    from dataclasses import dataclass
+else:
+    from pydantic.dataclasses import dataclass
+
+from typing import (
+    List,
+    Optional,
+)
 
 import betterproto
+from pydantic import root_validator
 
 
-@dataclass
+@dataclass(eq=False, repr=False)
 class Http(betterproto.Message):
     """
     Defines the HTTP configuration for an API service. It contains a list of
     [HttpRule][google.api.HttpRule], each specifying the mapping of an RPC
     method to one or more HTTP REST API methods.
     """
 
-    # A list of HTTP configuration rules that apply to individual API methods.
-    # **NOTE:** All service configuration rules follow "last one wins" order.
     rules: List["HttpRule"] = betterproto.message_field(1)
-    # When set to true, URL path parameters will be fully URI-decoded except in
-    # cases of single segment matches in reserved expansion, where "%2F" will be
-    # left encoded. The default behavior is to not decode RFC 6570 reserved
-    # characters in multi segment matches.
+    """
+    A list of HTTP configuration rules that apply to individual API methods.
+    **NOTE:** All service configuration rules follow "last one wins" order.
+    """
+
     fully_decode_reserved_expansion: bool = betterproto.bool_field(2)
+    """
+    When set to true, URL path parameters will be fully URI-decoded except in
+    cases of single segment matches in reserved expansion, where "%2F" will be
+    left encoded. The default behavior is to not decode RFC 6570 reserved
+    characters in multi segment matches.
+    """
 
 
-@dataclass
+@dataclass(eq=False, repr=False)
 class HttpRule(betterproto.Message):
     """
     # gRPC Transcoding gRPC Transcoding is a feature for mapping between a gRPC
     method and one or more HTTP REST endpoints. It allows developers to build a
     single API service that supports both gRPC APIs and REST APIs. Many
     systems, including [Google APIs](https://github.com/googleapis/googleapis),
     [Cloud Endpoints](https://cloud.google.com/endpoints), [gRPC
@@ -174,50 +192,84 @@
     must not be mapped to URL query parameters, because no client library can
     support such complicated mapping. If an API needs to use a JSON array for
     request or response body, it can map the request or response body to a
     repeated field. However, some gRPC Transcoding implementations may not
     support this feature.
     """
 
-    # Selects a method to which this rule applies. Refer to
-    # [selector][google.api.DocumentationRule.selector] for syntax details.
     selector: str = betterproto.string_field(1)
-    # Maps to HTTP GET. Used for listing and getting information about resources.
-    get: str = betterproto.string_field(2, group="pattern")
-    # Maps to HTTP PUT. Used for replacing a resource.
-    put: str = betterproto.string_field(3, group="pattern")
-    # Maps to HTTP POST. Used for creating a resource or performing an action.
-    post: str = betterproto.string_field(4, group="pattern")
-    # Maps to HTTP DELETE. Used for deleting a resource.
-    delete: str = betterproto.string_field(5, group="pattern")
-    # Maps to HTTP PATCH. Used for updating a resource.
-    patch: str = betterproto.string_field(6, group="pattern")
-    # The custom pattern is used for specifying an HTTP method that is not
-    # included in the `pattern` field, such as HEAD, or "*" to leave the HTTP
-    # method unspecified for this rule. The wild-card rule is useful for services
-    # that provide content to Web (HTML) clients.
-    custom: "CustomHttpPattern" = betterproto.message_field(8, group="pattern")
-    # The name of the request field whose value is mapped to the HTTP request
-    # body, or `*` for mapping all request fields not captured by the path
-    # pattern to the HTTP body, or omitted for not having any HTTP request body.
-    # NOTE: the referred field must be present at the top-level of the request
-    # message type.
+    """
+    Selects a method to which this rule applies. Refer to
+    [selector][google.api.DocumentationRule.selector] for syntax details.
+    """
+
+    get: Optional[str] = betterproto.string_field(2, optional=True, group="pattern")
+    """
+    Maps to HTTP GET. Used for listing and getting information about resources.
+    """
+
+    put: Optional[str] = betterproto.string_field(3, optional=True, group="pattern")
+    """Maps to HTTP PUT. Used for replacing a resource."""
+
+    post: Optional[str] = betterproto.string_field(4, optional=True, group="pattern")
+    """
+    Maps to HTTP POST. Used for creating a resource or performing an action.
+    """
+
+    delete: Optional[str] = betterproto.string_field(5, optional=True, group="pattern")
+    """Maps to HTTP DELETE. Used for deleting a resource."""
+
+    patch: Optional[str] = betterproto.string_field(6, optional=True, group="pattern")
+    """Maps to HTTP PATCH. Used for updating a resource."""
+
+    custom: Optional["CustomHttpPattern"] = betterproto.message_field(
+        8, optional=True, group="pattern"
+    )
+    """
+    The custom pattern is used for specifying an HTTP method that is not
+    included in the `pattern` field, such as HEAD, or "*" to leave the HTTP
+    method unspecified for this rule. The wild-card rule is useful for services
+    that provide content to Web (HTML) clients.
+    """
+
     body: str = betterproto.string_field(7)
-    # Optional. The name of the response field whose value is mapped to the HTTP
-    # response body. When omitted, the entire response message will be used as
-    # the HTTP response body. NOTE: The referred field must be present at the
-    # top-level of the response message type.
+    """
+    The name of the request field whose value is mapped to the HTTP request
+    body, or `*` for mapping all request fields not captured by the path
+    pattern to the HTTP body, or omitted for not having any HTTP request body.
+    NOTE: the referred field must be present at the top-level of the request
+    message type.
+    """
+
     response_body: str = betterproto.string_field(12)
-    # Additional HTTP bindings for the selector. Nested bindings must not contain
-    # an `additional_bindings` field themselves (that is, the nesting may only be
-    # one level deep).
+    """
+    Optional. The name of the response field whose value is mapped to the HTTP
+    response body. When omitted, the entire response message will be used as
+    the HTTP response body. NOTE: The referred field must be present at the
+    top-level of the response message type.
+    """
+
     additional_bindings: List["HttpRule"] = betterproto.message_field(11)
+    """
+    Additional HTTP bindings for the selector. Nested bindings must not contain
+    an `additional_bindings` field themselves (that is, the nesting may only be
+    one level deep).
+    """
 
+    @root_validator()
+    def check_oneof(cls, values):
+        return cls._validate_field_groups(values)
 
-@dataclass
+
+@dataclass(eq=False, repr=False)
 class CustomHttpPattern(betterproto.Message):
     """A custom pattern is used for defining custom HTTP verb."""
 
-    # The name of this custom HTTP verb.
     kind: str = betterproto.string_field(1)
-    # The path matched by this custom verb.
+    """The name of this custom HTTP verb."""
+
     path: str = betterproto.string_field(2)
+    """The path matched by this custom verb."""
+
+
+Http.__pydantic_model__.update_forward_refs()  # type: ignore
+HttpRule.__pydantic_model__.update_forward_refs()  # type: ignore
```

### Comparing `headscale_api-0.1.0/pyproject.toml` & `headscale_api-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "headscale-api"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python Headscale API and configuration abstraction."
 authors = ["Marek Pikuła <marek@serenitycode.dev>"]
 maintainers = ["Marek Pikuła <marek@serenitycode.dev>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -14,16 +14,16 @@
 # documentation = "https://python-headscale-api.readthedocs.io"
 readme = "README.md"
 packages = [
     {include = "headscale_api"},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"  # Change to 3.7 once datetime parsing is fixed.
-betterproto = {extras = ["compiler"], version = "^1.2.5"}
+python = "^3.11"  # TODO: Change to 3.7 once datetime parsing is fixed.
+betterproto = {version = "2.0.0b5", extras = ["compiler"]} # TODO: Change after release.
 requests = "^2.28.2"
 pydantic = "^1.10.7"
 pydantic-yaml = {extras = ["ruamel"], version = "^0.11.2"}
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
 mypy = "^1.1.1"
@@ -46,16 +46,20 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
+skip_glob = ["headscale_api/schema"]
 
 [tool.pydocstyle]
 match_dir = '^(?:(headscale_api\/schema)|(\.)).*$'
 
 [tool.pylint.main]
 ignore-paths = ["headscale_api/schema"]
 
 [tool.ruff]
 exclude = ["headscale_api/schema"]
+
+[tool.mypy]
+exclude = ['^headscale_api\/schema\/.*$']
```

### Comparing `headscale_api-0.1.0/PKG-INFO` & `headscale_api-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: headscale-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Headscale API and configuration abstraction.
 Home-page: https://github.com/MarekPikula/python-headscale-api
 License: MIT
 Author: Marek Pikuła
 Author-email: marek@serenitycode.dev
 Maintainer: Marek Pikuła
 Maintainer-email: marek@serenitycode.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: betterproto[compiler] (>=1.2.5,<2.0.0)
+Requires-Dist: betterproto[compiler] (==2.0.0b5)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pydantic-yaml[ruamel] (>=0.11.2,<0.12.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/MarekPikula/python-headscale-api
 Description-Content-Type: text/markdown
 
 # python-headscale-api
```

