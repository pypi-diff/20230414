# Comparing `tmp/flask_pydantic_api-0.9.2-py3-none-any.whl.zip` & `tmp/flask_pydantic_api-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11264 bytes, number of entries: 12
--rw-r--r--  2.0 unx       52 b- defN 23-Mar-09 23:20 flask_pydantic_api/__init__.py
--rw-r--r--  2.0 unx     6383 b- defN 23-Mar-19 02:00 flask_pydantic_api/api_wrapper.py
+Zip file size: 12719 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       98 b- defN 23-Apr-06 01:39 flask_pydantic_api/__init__.py
+-rw-r--r--  2.0 unx     6964 b- defN 23-Apr-06 02:20 flask_pydantic_api/api_wrapper.py
 -rw-r--r--  2.0 unx      819 b- defN 23-Mar-18 20:39 flask_pydantic_api/apidocs_views.py
--rw-r--r--  2.0 unx     4654 b- defN 23-Apr-01 23:22 flask_pydantic_api/openapi.py
+-rw-r--r--  2.0 unx     7386 b- defN 23-Apr-13 22:12 flask_pydantic_api/openapi.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-19 03:04 flask_pydantic_api/py.typed
--rw-r--r--  2.0 unx     1464 b- defN 23-Mar-18 23:25 flask_pydantic_api/utils.py
+-rw-r--r--  2.0 unx     2342 b- defN 23-Apr-06 02:14 flask_pydantic_api/utils.py
 -rw-r--r--  2.0 unx      447 b- defN 23-Mar-18 20:21 flask_pydantic_api/templates/rapidoc.html
--rw-r--r--  2.0 unx     1073 b- defN 23-Apr-02 01:16 flask_pydantic_api-0.9.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    11027 b- defN 23-Apr-02 01:16 flask_pydantic_api-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-02 01:16 flask_pydantic_api-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Apr-02 01:16 flask_pydantic_api-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1056 b- defN 23-Apr-02 01:16 flask_pydantic_api-0.9.2.dist-info/RECORD
-12 files, 27086 bytes uncompressed, 9458 bytes compressed:  65.1%
+-rw-r--r--  2.0 unx     1073 b- defN 23-Apr-13 22:18 flask_pydantic_api-0.9.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11905 b- defN 23-Apr-13 22:18 flask_pydantic_api-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 22:18 flask_pydantic_api-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Apr-13 22:18 flask_pydantic_api-0.9.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1056 b- defN 23-Apr-13 22:18 flask_pydantic_api-0.9.3.dist-info/RECORD
+12 files, 32201 bytes uncompressed, 10913 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: flask_pydantic_api/utils.py
 Comment: 
 
 Filename: flask_pydantic_api/templates/rapidoc.html
 Comment: 
 
-Filename: flask_pydantic_api-0.9.2.dist-info/LICENSE
+Filename: flask_pydantic_api-0.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: flask_pydantic_api-0.9.2.dist-info/METADATA
+Filename: flask_pydantic_api-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: flask_pydantic_api-0.9.2.dist-info/WHEEL
+Filename: flask_pydantic_api-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: flask_pydantic_api-0.9.2.dist-info/top_level.txt
+Filename: flask_pydantic_api-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: flask_pydantic_api-0.9.2.dist-info/RECORD
+Filename: flask_pydantic_api-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_pydantic_api/__init__.py

```diff
@@ -1 +1,2 @@
 from .api_wrapper import pydantic_api  # noqa: F401
+from .utils import UploadedFile  # noqa: F401
```

## flask_pydantic_api/api_wrapper.py

```diff
@@ -1,39 +1,55 @@
 import asyncio
 from functools import wraps
+from itertools import chain
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
 from asgiref.sync import async_to_sync
-from flask import current_app, jsonify, make_response, request
+from flask import abort, current_app, jsonify, make_response, request
 from pydantic import BaseModel, ValidationError
 from pydantic.tools import parse_obj_as
 
-from .utils import get_annotated_models
+from .utils import get_annotated_models, model_has_uploaded_file_type
 
 augment_schema_with_fieldsets: Optional[Callable] = None
 render_fieldset_model: Optional[Callable] = None
 
 try:
     from pydantic_enhanced_serializer import (
         augment_schema_with_fieldsets,
         render_fieldset_model,
     )
 except ImportError:
     pass
 
 
+class EndpointConfig(BaseModel):
+    name: Optional[str]
+    tags: Optional[List[str]]
+    success_status_code: int
+    request_fields_name: str
+
+
 def get_request_args(
     view_kwargs: Dict[str, Any],
     for_model: Optional[Type[BaseModel]] = None,
     merge_path_parameters: Optional[bool] = False,
 ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
     args: Dict[str, Any] = {}
 
-    if request.is_json and request.json:
+    if for_model and model_has_uploaded_file_type(for_model):
+        if not request.content_type.lower().startswith("multipart/form-data"):
+            abort(415, "multipart/form-data expected")
+
+        for name, value in chain(request.files.items(), request.form.items()):
+            args[name] = value
+
+    elif request.is_json and request.json:
         args.update(request.json)
+
     elif request.query_string:
         args.update(request.args.to_dict())
         if for_model:
             args.update(
                 {
                     k: v
                     for k, v in request.args.to_dict(flat=False).items()
@@ -166,16 +182,17 @@
             request_model, *(response_models or [])
         )
 
         # Normally wrapping functions with decorators leaves no easy
         # way to tell who is doing the wrapping and for what purpose.
         # This adds some markers that are useful for introspection of
         # endpoints (such as generating schema).
-        wrapped_endpoint.__pydantic_api__ = {  # type: ignore
-            "name": name,
-            "tags": tags,
-            "success_status_code": success_status_code,
-        }
+        wrapped_endpoint.__pydantic_api__ = EndpointConfig(  # type: ignore
+            name=name,
+            tags=tags,
+            success_status_code=success_status_code,
+            request_fields_name=request_fields_name,
+        )
 
         return wrapped_endpoint
 
     return wrap
```

## flask_pydantic_api/openapi.py

```diff
@@ -1,56 +1,86 @@
 import re
 from collections import defaultdict
-from typing import Any, Dict, Optional, Type
+from functools import partial
+from typing import Any, Callable, Dict, Optional, Type, Union
 
 from flask import current_app
 from openapi_schema_pydantic import Info, MediaType, OpenAPI, Response
 from openapi_schema_pydantic.util import (
     PydanticSchema,
     construct_open_api_with_schema_class,
 )
 from pydantic import BaseModel
 
-from .utils import get_annotated_models
+from .api_wrapper import EndpointConfig
+from .utils import get_annotated_models, model_has_uploaded_file_type
 
 HTTP_METHODS = set(["get", "post", "patch", "delete", "put"])
 
+model_has_fieldsets_defined: Optional[Callable] = None
+try:
+    from pydantic_enhanced_serializer.schema import model_has_fieldsets_defined
+except ImportError:
+    pass
+
 
 def get_pydantic_api_path_operations() -> Any:
     paths: Dict[str, dict] = defaultdict(dict)
 
     for rule in current_app.url_map.iter_rules():
         view_func = current_app.view_functions[rule.endpoint]
-        if not getattr(view_func, "__pydantic_api__", None):
+        view_func_config: Optional[EndpointConfig] = getattr(
+            view_func, "__pydantic_api__", None
+        )
+
+        if not view_func_config:
             continue
 
         if not rule.methods:
             continue
 
         path = re.sub(r"<([\w_]+)>", "{\\1}", rule.rule)
 
         parameters = []
         request_body: Optional[Dict[str, Any]] = None
         responses: Dict[str, dict] = {}
 
-        success_status_code = str(
-            view_func.__pydantic_api__.get("success_status_code", "200")  # type: ignore
-        )
+        success_status_code = str(view_func_config.success_status_code)
 
         request_model_param_name, request_model, response_models = get_annotated_models(
             view_func
         )
+
+        need_fields_parameter = bool(
+            model_has_fieldsets_defined
+            and response_models
+            and model_has_fieldsets_defined(response_models[0])
+        )
+
         if request_model:
             title = request_model.__config__.title or request_model.__name__
+            content_type = (
+                "multipart/form-data"
+                if model_has_uploaded_file_type(request_model)
+                else "application/json"
+            )
+
+            if need_fields_parameter:
+                current_schema_extra: Union[Callable, dict, None] = getattr(
+                    request_model.__config__, "schema_extra", None
+                )
+
+                request_model.__config__.schema_extra = partial(
+                    request_body_add_fields_extra_schema, current_schema_extra
+                )
+
             request_body = {
                 "description": f"A {title}",
                 "content": {
-                    "application/json": {
-                        "schema": PydanticSchema(schema_class=request_model)
-                    }
+                    content_type: {"schema": PydanticSchema(schema_class=request_model)}
                 },
                 "required": True,
             }
 
         if response_models:
             title = response_models[0].__config__.title or response_models[0].__name__
 
@@ -58,14 +88,15 @@
                 "description": f"A {title}",
                 "content": {
                     "application/json": {
                         "schema": PydanticSchema(schema_class=response_models[0])
                     }
                 },
             }
+
         else:
             responses[success_status_code] = {
                 "description": "Empty Response",
             }
 
         # path parameters
         for name in view_func.__annotations__.keys():
@@ -89,18 +120,34 @@
             responses[success_status_code] = {"description": None}
 
         for method in rule.methods:
             method = method.lower()
             if method not in HTTP_METHODS:
                 continue
 
+            if method.lower() == "get" and need_fields_parameter and not request_body:
+                parameters.append(
+                    {
+                        "name": "fields",
+                        "description": (
+                            "Comma separated list of fields, fieldset and/or "
+                            "expansions to return in the response"
+                        ),
+                        "in": "query",
+                        "required": False,
+                        "schema": {
+                            "type": "string",
+                        },
+                    }
+                )
+
             paths[path][method] = {
-                "summary": view_func.__pydantic_api__.get("name"),  # type: ignore
+                "summary": view_func_config.name,
                 "requestBody": request_body,
-                "tags": view_func.__pydantic_api__.get("tags") or [],  # type: ignore
+                "tags": view_func_config.tags or [],
                 "parameters": parameters,
                 "responses": responses,
             }
 
     return paths
 
 
@@ -144,7 +191,44 @@
             {
                 "info": info,
                 "paths": paths,
                 **kwargs,
             }
         )
     )
+
+
+def request_body_add_fields_extra_schema(
+    original_schema_extra: Union[Callable, dict, None],
+    schema: Dict[str, Any],
+    model: Type[BaseModel],
+) -> None:
+    if "properties" not in schema:
+        schema["properties"] = {}
+
+    if "fields" not in schema["properties"]:
+        schema["properties"]["fields"] = {
+            "title": "fields",
+            "description": "List of fields, fieldset and/or expansions to return in the response",
+            "type": "array",
+            "items": {
+                "type": "string",
+            },
+        }
+
+    if callable(original_schema_extra):
+        _deep_update(schema, original_schema_extra(schema, model) or {})
+
+    elif isinstance(original_schema_extra, dict):
+        _deep_update(schema, original_schema_extra)
+
+
+def _deep_update(into_dict: Dict[Any, Any], from_dict: Dict[Any, Any]) -> None:
+    for key in from_dict.keys():
+        if (
+            key in into_dict
+            and isinstance(from_dict[key], dict)
+            and isinstance(into_dict[key], dict)
+        ):
+            _deep_update(into_dict[key], from_dict[key])
+        else:
+            into_dict[key] = from_dict[key]
```

## flask_pydantic_api/utils.py

```diff
@@ -1,11 +1,43 @@
 from inspect import isclass
-from typing import Callable, List, Optional, Tuple, Type, Union, get_args, get_origin
+from typing import (
+    Any,
+    Callable,
+    Generator,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    get_args,
+    get_origin,
+)
 
 from pydantic import BaseModel
+from werkzeug.datastructures import FileStorage
+
+
+class UploadedFile(FileStorage):
+    """A pydantic custom type wrapper for uploaded file streams in Flask/Werkzeug"""
+
+    @classmethod
+    def __get_validators__(cls) -> Generator[Callable, None, None]:
+        yield cls.validate
+
+    @classmethod
+    def __modify_schema__(cls, field_schema: dict) -> None:
+        field_schema["type"] = "string"
+        field_schema["format"] = "binary"
+
+    @classmethod
+    def validate(cls, value: Any) -> FileStorage:
+        if not isinstance(value, FileStorage):
+            raise TypeError("file required")
+
+        return value
 
 
 def get_annotated_models(
     func: Callable,
 ) -> Tuple[Optional[str], Optional[Type[BaseModel]], Optional[List[Type[BaseModel]]]]:
     request_model = None
     request_model_param_name = None
@@ -37,7 +69,15 @@
             if isclass(type_) and issubclass(type_, BaseModel)
         ]
 
     elif isclass(return_annotation) and issubclass(return_annotation, BaseModel):
         response_models = [return_annotation]
 
     return request_model_param_name, request_model, response_models
+
+
+def model_has_uploaded_file_type(model: Type[BaseModel]) -> bool:
+    for field in model.__fields__.values():
+        if field.type_ == UploadedFile:
+            return True
+
+    return False
```

## Comparing `flask_pydantic_api-0.9.2.dist-info/LICENSE` & `flask_pydantic_api-0.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flask_pydantic_api-0.9.2.dist-info/METADATA` & `flask_pydantic_api-0.9.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-pydantic-api
-Version: 0.9.2
+Version: 0.9.3
 Summary: Pydantic based API support for Flask
 Home-page: https://github.com/adamsussman/flask-pydantic-api
 Author: Adam Sussman
 Author-email: adam.sussman@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
@@ -42,16 +42,17 @@
 
 ## Features
 
 1. Use pydantic models for request data validation (post bodies and query strings) as well as for formatting responses
 2. Type annotation driven on the view function instead of the decorator.
 3. OpenAPI schema generation and documentation
 4. Smart response fields and expansions using [pydantic-enhanced-serializer](https://github.com/adamsussman/pydantic-enhanced-serializer).
-5. Async views
-6. Fold path parameters into input Pydantic models
+5. Fold path parameters into input Pydantic models
+6. File Uploads into Pydantic model fields
+7. Async views
 
 ## Installation
 
 ```console
 $ pip install flask-pydantic-api
 ```
 
@@ -290,18 +291,18 @@
         field2: str
 
         class Config:
             fieldsets = [
                 default: ["field2"],
             ]
 
-        @app.get("/something")
-        @pydantic_api()
-        def get_something() -> MyResponse:
-            return MyResponse(field1="value1", field2="value2")
+    @app.get("/something")
+    @pydantic_api()
+    def get_something() -> MyResponse:
+        return MyResponse(field1="value1", field2="value2")
 ```
 
 ```console
 
     curl http://localhost:8080/something?fields=field1,field2
     curl http://localhost:8080/something?fields=field1&fields=field2
 
@@ -312,10 +313,41 @@
 
 ```
 
 See [Pydantic Enhanced Serializer](https://github.com/adamsussman/pydantic-enhanced-serializer)
 for more information.
 
 
+<a name="fileuploads"></a>
+### File Uploads
+
+File uploading with `multipart/form-data` content into pydantic request models is supported and
+the usual required and type checks will be done.
+
+Multiple files can be uploaded in the same request so long as each has a distinct field name.
+
+```python
+
+    from pydantic import BaseModel
+    from pydantic_api import UploadedFile, pydantic_api
+
+    class MyRequest(BaseModel):
+        photo: UploadedFile
+        caption: str
+
+    @app.post("/upload-photo"
+    @pyantic_api()
+    def upload_photo(body: MyRequest) -> MyResponse:
+        binary_file_data = body.photo.read()  # body.photo is werkzeug.datastructures.FileStorage object
+        file_name = body.photo.filename
+
+        ...
+```
+
+```console
+    curl -F photo=@some_file.jpg -F caption="A great picture!" http://localhsot:8080/upload-photo
+```
+
+
 ## License
 
 This project is licensed under the terms of the MIT license.
```

## Comparing `flask_pydantic_api-0.9.2.dist-info/RECORD` & `flask_pydantic_api-0.9.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-flask_pydantic_api/__init__.py,sha256=BP5saqY56EY6BsRIQxWnFy3oBB1VZPM9fJNJ4ngJnj8,52
-flask_pydantic_api/api_wrapper.py,sha256=y0O0hmcBF2sZgqa3sJVE89EFWwS_0Jed0o3_MzxgASw,6383
+flask_pydantic_api/__init__.py,sha256=KICwgGx_FRhKuNBAcoy1GHBo9C4Jn0QUEwChlmdGS18,98
+flask_pydantic_api/api_wrapper.py,sha256=LHeUF5qzpPXaIv3gj70qL1wV7X0QlMLfRw_Za32KTXY,6964
 flask_pydantic_api/apidocs_views.py,sha256=sSsr1zVE35UtVPHH0on6HRoZO1vYO1xXRMETq4Fcp1U,819
-flask_pydantic_api/openapi.py,sha256=-fgL3Imbf9tUxuxpwe3BHzOiu89HMxml7nqmwThPQ2k,4654
+flask_pydantic_api/openapi.py,sha256=EXMBLFDTERHUkCu-p2ov2qrHi17ZJf8hgqB2wE57tig,7386
 flask_pydantic_api/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-flask_pydantic_api/utils.py,sha256=LcH3X9ZsGRyXVaQXcX1qUJd8xmi0lHzUG_ByQBWevYs,1464
+flask_pydantic_api/utils.py,sha256=mQ-33XUZ_VOHjSgxv2hCyAIIeOCZnCeemRsyDW6D-ng,2342
 flask_pydantic_api/templates/rapidoc.html,sha256=VLYAdPmRJ7dVQmpLmykMUA8KsVEF77tP-Xo2mbBHbBw,447
-flask_pydantic_api-0.9.2.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
-flask_pydantic_api-0.9.2.dist-info/METADATA,sha256=C6OckTXuBaieKY5DqrTPqyZ864GwKH8RVaHAMOB00Uw,11027
-flask_pydantic_api-0.9.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-flask_pydantic_api-0.9.2.dist-info/top_level.txt,sha256=lFmuWAb1KRWKxzT1wPHWpS8eUwnDY1WPWAzqkUDVlU4,19
-flask_pydantic_api-0.9.2.dist-info/RECORD,,
+flask_pydantic_api-0.9.3.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
+flask_pydantic_api-0.9.3.dist-info/METADATA,sha256=cyG-8RbhQHHTKfj3nGkaTWuKrmBI2gKwXtSSvb_zaF0,11905
+flask_pydantic_api-0.9.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+flask_pydantic_api-0.9.3.dist-info/top_level.txt,sha256=lFmuWAb1KRWKxzT1wPHWpS8eUwnDY1WPWAzqkUDVlU4,19
+flask_pydantic_api-0.9.3.dist-info/RECORD,,
```

