# Comparing `tmp/polywrap_http_plugin-0.1.0a2.tar.gz` & `tmp/polywrap_http_plugin-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_http_plugin-0.1.0a2.tar", max compression
+gzip compressed data, was "polywrap_http_plugin-0.1.0a3.tar", max compression
```

## Comparing `polywrap_http_plugin-0.1.0a2.tar` & `polywrap_http_plugin-0.1.0a3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       22 2023-03-02 09:38:06.545592 polywrap_http_plugin-0.1.0a2/README.md
--rw-r--r--   0        0        0     4586 2023-03-04 14:34:43.016426 polywrap_http_plugin-0.1.0a2/polywrap_http_plugin/__init__.py
--rw-r--r--   0        0        0    12372 2023-03-02 10:46:26.547111 polywrap_http_plugin-0.1.0a2/polywrap_http_plugin/manifest.json
--rw-r--r--   0        0        0      983 2023-03-05 08:25:15.363673 polywrap_http_plugin-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a2/setup.py
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-11 11:16:49.724598 polywrap_http_plugin-0.1.0a3/README.md
+-rw-r--r--   0        0        0     3413 2023-04-12 10:16:18.139428 polywrap_http_plugin-0.1.0a3/polywrap_http_plugin/__init__.py
+-rw-r--r--   0        0        0    12372 2023-04-11 11:16:49.723724 polywrap_http_plugin-0.1.0a3/polywrap_http_plugin/manifest.json
+-rw-r--r--   0        0        0     1156 2023-04-14 13:15:24.660446 polywrap_http_plugin-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a3/setup.py
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a3/PKG-INFO
```

### Comparing `polywrap_http_plugin-0.1.0a2/polywrap_http_plugin/__init__.py` & `polywrap_http_plugin-0.1.0a3/polywrap_http_plugin/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,66 @@
 import base64
-from pathlib import Path
-from typing import List, Optional, TypedDict, Union, cast
-from enum import Enum
-import json
-
-from httpx import AsyncClient, Response
-from polywrap_plugin import PluginModule, PluginPackage
-from polywrap_core import Invoker
-from polywrap_result import Ok, Result
-from polywrap_manifest import WrapManifest
-from polywrap_msgpack.generic_map import GenericMap
-
-
-class HttpResponseType(Enum):
-    TEXT = "TEXT"
-    BINARY = "BINARY"
-
-
-class FormDataEntry(TypedDict):
-    name: str
-    value: Optional[str]
-    fileName: Optional[str]
-    type: Optional[str]
-
-
-class HttpRequest(TypedDict):
-    headers: Optional[GenericMap[str, str]]
-    urlParams: Optional[GenericMap[str, str]]
-    responseType: Union[HttpResponseType, str, int]
-    body: Optional[str]
-    formData: Optional[List[FormDataEntry]]
-    timeout: Optional[int]
-
-class HttpResponse(TypedDict):
-    status: int
-    statusText: str
-    headers: Optional[GenericMap[str, str]]
-    body: Optional[str]
-
-
-class ArgsGet(TypedDict):
-    url: str
-    request: Optional[HttpRequest]
-
-
-class ArgsPost(TypedDict):
-    url: str
-    request: Optional[HttpRequest]
+from typing import Optional, cast
+
+from httpx import AsyncClient, Response as HttpxResponse
+from polywrap_plugin import PluginPackage
+from polywrap_core import InvokerClient, UriPackageOrWrapper
+from polywrap_msgpack import GenericMap
+
+from .wrap import HttpHttpResponse, HttpHttpResponseType, ArgsGet, ArgsPost, manifest, Module
 
 
 def isResponseBinary(args: ArgsGet) -> bool:
     if args.get("request") is None:
         return False
     if not args["request"]:
         return False
-    if isinstance(args["request"]["responseType"], int) and args["request"]["responseType"] == 1:
+    if args["request"]["responseType"] == 1:
         return True
-    if isinstance(args["request"]["responseType"], str) and args["request"]["responseType"] == "BINARY":
+    if args["request"]["responseType"] == "BINARY":
         return True
-    return args["request"]["responseType"] == HttpResponseType.BINARY
+    return args["request"]["responseType"] == HttpHttpResponseType.BINARY
 
 
-class HttpPlugin(PluginModule[None]):
+class HttpPlugin(Module[None]):
     def __init__(self):
         super().__init__(None)
         self.client = AsyncClient()
 
-    async def get(self, args: ArgsGet, invoker: Invoker) -> Result[HttpResponse]:
-        res: Response
+    async def get(self, args: ArgsGet, client: InvokerClient[UriPackageOrWrapper], env: None) -> Optional[HttpHttpResponse]:
+        res: HttpxResponse
         if args.get("request") is None:
             res = await self.client.get(args["url"])
         elif args["request"] is not None:
             res = await self.client.get(
                 args["url"],
                 params=args["request"]["urlParams"],
                 headers=args["request"]["headers"],
                 timeout=cast(float, args["request"]["timeout"]),
             )
         else:
             res = await self.client.get(args["url"])
 
         if isResponseBinary(args):
-            return Ok(
-                HttpResponse(
-                    status=res.status_code,
-                    statusText=res.reason_phrase,
-                    headers=GenericMap(dict(res.headers)),
-                    body=base64.b64encode(res.content).decode(),
-                )
-            )
-
-        return Ok(
-            HttpResponse(
+            return HttpHttpResponse(
                 status=res.status_code,
                 statusText=res.reason_phrase,
                 headers=GenericMap(dict(res.headers)),
-                body=res.text,
+                body=base64.b64encode(res.content).decode(),
             )
+
+        return HttpHttpResponse(
+            status=res.status_code,
+            statusText=res.reason_phrase,
+            headers=GenericMap(dict(res.headers)),
+            body=res.text,
         )
 
-    async def post(self, args: ArgsPost, invoker: Invoker) -> Result[HttpResponse]:
-        res: Response
+    async def post(self, args: ArgsPost, client: InvokerClient[UriPackageOrWrapper], env: None) -> Optional[HttpHttpResponse]:
+        res: HttpxResponse
         if args.get("request") is None:
             res = await self.client.post(args["url"])
         elif args["request"] is not None:
             content = (
                 args["request"]["body"].encode()
                 if args["request"]["body"] is not None
                 else None
@@ -115,33 +71,25 @@
                 params=args["request"]["urlParams"],
                 headers=args["request"]["headers"],
                 timeout=cast(float, args["request"]["timeout"]),
             )
         else:
             res = await self.client.post(args["url"])
 
-        if args["request"] is not None and args["request"]["responseType"] == HttpResponseType.BINARY:
-            return Ok(
-                HttpResponse(
-                    status=res.status_code,
-                    statusText=res.reason_phrase,
-                    headers=GenericMap(dict(res.headers)),
-                    body=base64.b64encode(res.content).decode(),
-                )
+        if args["request"] is not None and args["request"]["responseType"] == HttpHttpResponseType.BINARY:
+            return HttpHttpResponse(
+                status=res.status_code,
+                statusText=res.reason_phrase,
+                headers=GenericMap(dict(res.headers)),
+                body=base64.b64encode(res.content).decode(),
             )
 
-        return Ok(
-            HttpResponse(
+        return HttpHttpResponse(
                 status=res.status_code,
                 statusText=res.reason_phrase,
                 headers=GenericMap(dict(res.headers)),
                 body=res.text,
             )
-        )
 
 
 def http_plugin():
-    manifest_path = Path(__file__).parent.joinpath("manifest.json")
-    with open(manifest_path, "r") as f:
-        json_manifest = json.load(f)
-        manifest = WrapManifest(**json_manifest)
     return PluginPackage(module=HttpPlugin(), manifest=manifest)
```

### Comparing `polywrap_http_plugin-0.1.0a2/polywrap_http_plugin/manifest.json` & `polywrap_http_plugin-0.1.0a3/polywrap_http_plugin/manifest.json`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0a2/pyproject.toml` & `polywrap_http_plugin-0.1.0a3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-http-plugin"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = ""
 authors = ["Niraj Kamdar <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [{include = "polywrap_http_plugin"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-client = "0.1.0a11"
-polywrap-plugin = "0.1.0a11"
+polywrap-plugin = "0.1.0a28"
 httpx = "^0.23.3"
+polywrap-core = "^0.1.0a28"
+polywrap-msgpack = "^0.1.0a28"
+polywrap-manifest = "^0.1.0a28"
 
 [tool.poetry.group.dev.dependencies]
+polywrap-client = "0.1.0a28"
 black = "^23.1.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 isort = "^5.12.0"
 bandit = "^1.7.4"
 pyright = "^1.1.296"
 pylint = "^2.16.3"
+polywrap-uri-resolvers = "^0.1.0a28"
+polywrap-client-config-builder = "^0.1.0a28"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.black]
 target-version = ["py310"]
```

### Comparing `polywrap_http_plugin-0.1.0a2/setup.py` & `polywrap_http_plugin-0.1.0a3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 ['polywrap_http_plugin']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.23.3,<0.24.0',
- 'polywrap-client==0.1.0a11',
- 'polywrap-plugin==0.1.0a11']
+ 'polywrap-core>=0.1.0a28,<0.2.0',
+ 'polywrap-manifest>=0.1.0a28,<0.2.0',
+ 'polywrap-msgpack>=0.1.0a28,<0.2.0',
+ 'polywrap-plugin==0.1.0a28']
 
 setup_kwargs = {
     'name': 'polywrap-http-plugin',
-    'version': '0.1.0a2',
+    'version': '0.1.0a3',
     'description': '',
     'long_description': '# Polywrap HTTP Plugin',
     'author': 'Niraj Kamdar',
     'author_email': 'niraj@polywrap.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

