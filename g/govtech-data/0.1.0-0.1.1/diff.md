# Comparing `tmp/govtech_data-0.1.0.tar.gz` & `tmp/govtech_data-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govtech_data-0.1.0.tar", max compression
+gzip compressed data, was "govtech_data-0.1.1.tar", max compression
```

## Comparing `govtech_data-0.1.0.tar` & `govtech_data-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.0/README.md
--rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.0/govtech_data/__init__.py
--rw-r--r--   0        0        0     2716 2023-04-14 08:18:30.530755 govtech_data-0.1.0/govtech_data/client.py
--rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.0/govtech_data/models/__init__.py
--rw-r--r--   0        0        0      187 2023-04-14 06:22:56.953684 govtech_data-0.1.0/govtech_data/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      541 2023-04-14 07:45:03.424980 govtech_data-0.1.0/govtech_data/models/__pycache__/api.cpython-310.pyc
--rw-r--r--   0        0        0      120 2023-04-14 07:41:30.434938 govtech_data-0.1.0/govtech_data/models/api.py
--rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.0/govtech_data/models/resources/__init__.py
--rw-r--r--   0        0        0      197 2023-04-14 07:45:03.425736 govtech_data-0.1.0/govtech_data/models/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      832 2023-04-14 08:17:29.971383 govtech_data-0.1.0/govtech_data/models/resources/__pycache__/package_list.cpython-310.pyc
--rw-r--r--   0        0        0     4745 2023-04-14 08:17:29.972405 govtech_data-0.1.0/govtech_data/models/resources/__pycache__/package_show.cpython-310.pyc
--rw-r--r--   0        0        0     1176 2023-04-14 08:17:29.976136 govtech_data-0.1.0/govtech_data/models/resources/__pycache__/resource_show.cpython-310.pyc
--rw-r--r--   0        0        0      407 2023-04-14 08:17:30.099221 govtech_data-0.1.0/govtech_data/models/resources/package_list.py
--rw-r--r--   0        0        0     3817 2023-04-14 08:17:30.133220 govtech_data-0.1.0/govtech_data/models/resources/package_show.py
--rw-r--r--   0        0        0      573 2023-04-14 08:17:30.142184 govtech_data-0.1.0/govtech_data/models/resources/resource_show.py
--rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.0/govtech_data/utils/__init__.py
--rw-r--r--   0        0        0      186 2023-04-14 05:44:50.989776 govtech_data-0.1.0/govtech_data/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1392 2023-04-14 08:17:29.977018 govtech_data-0.1.0/govtech_data/utils/__pycache__/models.cpython-310.pyc
--rw-r--r--   0        0        0     1108 2023-04-14 08:17:28.295207 govtech_data-0.1.0/govtech_data/utils/models.py
--rw-r--r--   0        0        0      640 2023-04-14 08:20:15.849994 govtech_data-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 govtech_data-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 08:23:45.035078 govtech_data-0.1.1/README.md
+-rw-r--r--   0        0        0       34 2023-04-14 07:28:36.093561 govtech_data-0.1.1/govtech_data/__init__.py
+-rw-r--r--   0        0        0     3143 2023-04-14 10:06:22.322708 govtech_data-0.1.1/govtech_data/client.py
+-rw-r--r--   0        0        0        0 2023-04-14 06:17:41.589106 govtech_data-0.1.1/govtech_data/models/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-14 06:22:56.953684 govtech_data-0.1.1/govtech_data/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      907 2023-04-14 09:25:09.266500 govtech_data-0.1.1/govtech_data/models/__pycache__/api.cpython-310.pyc
+-rw-r--r--   0        0        0      349 2023-04-14 09:18:13.465611 govtech_data-0.1.1/govtech_data/models/api.py
+-rw-r--r--   0        0        0        0 2023-04-14 07:36:08.250878 govtech_data-0.1.1/govtech_data/models/resources/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-14 07:45:03.425736 govtech_data-0.1.1/govtech_data/models/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      854 2023-04-14 09:27:05.144157 govtech_data-0.1.1/govtech_data/models/resources/__pycache__/package_list.cpython-310.pyc
+-rw-r--r--   0        0        0     5700 2023-04-14 09:27:05.145341 govtech_data-0.1.1/govtech_data/models/resources/__pycache__/package_show.cpython-310.pyc
+-rw-r--r--   0        0        0     2851 2023-04-14 09:27:05.150383 govtech_data-0.1.1/govtech_data/models/resources/__pycache__/resource_show.cpython-310.pyc
+-rw-r--r--   0        0        0     1541 2023-04-14 09:27:05.352977 govtech_data-0.1.1/govtech_data/models/resources/datastore_search.py
+-rw-r--r--   0        0        0      407 2023-04-14 09:27:05.287711 govtech_data-0.1.1/govtech_data/models/resources/package_list.py
+-rw-r--r--   0        0        0     4441 2023-04-14 09:27:05.332541 govtech_data-0.1.1/govtech_data/models/resources/package_show.py
+-rw-r--r--   0        0        0     1994 2023-04-14 09:27:05.372624 govtech_data-0.1.1/govtech_data/models/resources/resource_show.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:44:38.638941 govtech_data-0.1.1/govtech_data/utils/__init__.py
+-rw-r--r--   0        0        0      186 2023-04-14 05:44:50.989776 govtech_data-0.1.1/govtech_data/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1392 2023-04-14 08:17:29.977018 govtech_data-0.1.1/govtech_data/utils/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0        0        0     1109 2023-04-14 09:37:13.383824 govtech_data-0.1.1/govtech_data/utils/models.py
+-rw-r--r--   0        0        0      761 2023-04-14 10:14:52.463452 govtech_data-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 govtech_data-0.1.1/PKG-INFO
```

### Comparing `govtech_data-0.1.0/govtech_data/client.py` & `govtech_data-0.1.1/govtech_data/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from functools import lru_cache
 from typing import Type, Union
 
 import requests
+
 from fuzzywuzzy import process
-from pydantic import BaseModel
 from loguru import logger
+from pydantic import BaseModel
 
-from govtech_data.models.api import PackageShow, ResourceShow
+from govtech_data.models.api import DatastoreSearch, PackageShow, ResourceShow
+from govtech_data.models.resources.datastore_search import DatastoreSearchModel
 from govtech_data.models.resources.package_list import PackageListModel
 from govtech_data.models.resources.package_show import PackageShowModel
 from govtech_data.models.resources.resource_show import ResourceShowModel
 
 ENDPOINTS = {
-    "ckan_resource_show": "https://data.gov.sg/api/action/resource_show",
     "ckan_datastore_search": "https://data.gov.sg/api/action/datastore_search",
     "ckan_package_show": "https://data.gov.sg/api/action/package_show",
     "ckan_package_list": "https://data.gov.sg/api/action/package_list",
+    "ckan_resource_show": "https://data.gov.sg/api/action/resource_show",
 }
 
 COMMON_HEADERS = {"accept": "application/json"}
 
 DEFAULT_TIMEOUT_IN_SECONDS = 30
 
 
@@ -31,29 +33,37 @@
             cls._instance = super(GovTechClient, cls).__new__(cls, *args, **kwargs)
         return cls._instance
 
     def __init__(self):
         pass
 
     @classmethod
-    def resource_show(cls, id_or_key: str) -> Union[BaseModel, ResourceShowModel]:
+    def datastore_search(
+        cls, resource_id: str, **kwargs
+    ) -> Union[BaseModel, DatastoreSearchModel]:
+        kwargs["resource_id"] = resource_id
         return cls.get_model_from_json_response(
-            ENDPOINTS.get("ckan_package_show"),
-            ResourceShow(**{"id": id_or_key}).dict(),
-            ResourceShowModel,
+            ENDPOINTS.get("ckan_datastore_search"),
+            DatastoreSearch(**kwargs).dict(),
+            DatastoreSearchModel,
         )
 
-    def datastore_search(self):
-        pass
+    @classmethod
+    def resource_show(cls, resource_id: str) -> Union[BaseModel, ResourceShowModel]:
+        return cls.get_model_from_json_response(
+            ENDPOINTS.get("ckan_resource_show"),
+            ResourceShow(**{"id": resource_id}).dict(),
+            ResourceShowModel,
+        )
 
     @classmethod
-    def package_show(cls, id_or_key: str) -> Union[BaseModel, PackageShowModel]:
+    def package_show(cls, package_id: str) -> Union[BaseModel, PackageShowModel]:
         return cls.get_model_from_json_response(
             ENDPOINTS.get("ckan_package_show"),
-            PackageShow(**{"id": id_or_key}).dict(),
+            PackageShow(**{"id": package_id}).dict(),
             PackageShowModel,
         )
 
     @classmethod
     @lru_cache(maxsize=1)
     def package_list(cls) -> Union[BaseModel, PackageListModel]:
         return cls.get_model_from_json_response(
```

### Comparing `govtech_data-0.1.0/govtech_data/models/resources/__pycache__/package_list.cpython-310.pyc` & `govtech_data-0.1.1/govtech_data/models/resources/__pycache__/package_list.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 14 08:16:40 2023 UTC, .py size: 396 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e80b 3964 8c01 0000  o.........9d....
+00000000: 6f0d 0d0a 0000 0000 f51b 3964 9701 0000  o.........9d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6506 8303 5a08 6406 5300 2907  ..d.e...Z.d.S.).
 00000070: e900 0000 0029 01da 0b61 6e6e 6f74 6174  .....)...annotat
@@ -10,43 +10,45 @@
 00000090: 7469 6f6e 616c 2902 da09 4261 7365 4d6f  tional)...BaseMo
 000000a0: 6465 6cda 0545 7874 7261 6300 0000 0000  del..Extrac.....
 000000b0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
 000000c0: 0000 0173 4000 0000 6500 5a01 6400 5a02  ...s@...e.Z.d.Z.
 000000d0: 5500 4700 6401 6402 8400 6402 8302 5a03  U.G.d.d...d...Z.
 000000e0: 6403 5a04 6404 6505 6405 3c00 6403 5a06  d.Z.d.e.d.<.d.Z.
 000000f0: 6406 6505 6407 3c00 6403 5a07 6408 6505  d.e.d.<.d.Z.d.e.
-00000100: 6409 3c00 6403 5300 290a da05 4d6f 6465  d.<.d.S.)...Mode
-00000110: 6c63 0000 0000 0000 0000 0000 0000 0000  lc..............
-00000120: 0000 0100 0000 4000 0001 7312 0000 0065  ......@...s....e
-00000130: 005a 0164 005a 0265 036a 045a 0564 0153  .Z.d.Z.e.j.Z.d.S
-00000140: 0029 027a 0c4d 6f64 656c 2e43 6f6e 6669  .).z.Model.Confi
-00000150: 674e 2906 da08 5f5f 6e61 6d65 5f5f da0a  gN)...__name__..
-00000160: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000170: 616c 6e61 6d65 5f5f 7206 0000 00da 0561  alname__r......a
-00000180: 6c6c 6f77 da05 6578 7472 61a9 0072 0d00  llow..extra..r..
-00000190: 0000 720d 0000 00fa 6c2f 5573 6572 732f  ..r.....l/Users/
-000001a0: 7275 6269 6b2f 4472 6f70 626f 782f 7275  rubik/Dropbox/ru
-000001b0: 6269 6b2f 6375 7272 656e 742f 6f67 702d  bik/current/ogp-
-000001c0: 706c 6179 6772 6f75 6e64 2f67 6f76 7465  playground/govte
-000001d0: 6368 2d64 6174 612f 676f 7674 6563 685f  ch-data/govtech_
-000001e0: 6461 7461 2f6d 6f64 656c 732f 7265 736f  data/models/reso
-000001f0: 7572 6365 732f 7061 636b 6167 655f 6c69  urces/package_li
-00000200: 7374 2e70 79da 0643 6f6e 6669 670d 0000  st.py..Config...
-00000210: 0073 0400 0000 0800 0a01 720f 0000 004e  .s........r....N
-00000220: 7a0d 4f70 7469 6f6e 616c 5b73 7472 5dda  z.Optional[str].
-00000230: 0468 656c 707a 0e4f 7074 696f 6e61 6c5b  .helpz.Optional[
-00000240: 626f 6f6c 5dda 0773 7563 6365 7373 7a13  bool]..successz.
-00000250: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
-00000260: 725d 5dda 0672 6573 756c 7429 0872 0800  r]]..result).r..
-00000270: 0000 7209 0000 0072 0a00 0000 720f 0000  ..r....r....r...
-00000280: 0072 1000 0000 da0f 5f5f 616e 6e6f 7461  .r......__annota
-00000290: 7469 6f6e 735f 5f72 1100 0000 7212 0000  tions__r....r...
-000002a0: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-000002b0: 720e 0000 0072 0700 0000 0c00 0000 730a  r....r........s.
-000002c0: 0000 000a 000e 010c 030c 0110 0172 0700  .............r..
-000002d0: 0000 4e29 09da 0a5f 5f66 7574 7572 655f  ..N)...__future_
-000002e0: 5f72 0200 0000 da06 7479 7069 6e67 7203  _r......typingr.
-000002f0: 0000 0072 0400 0000 da08 7079 6461 6e74  ...r......pydant
-00000300: 6963 7205 0000 0072 0600 0000 7207 0000  icr....r....r...
-00000310: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00000320: 720e 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000330: 0000 0073 0800 0000 0c04 1002 1002 1403  ...s............
+00000100: 6409 3c00 6403 5300 290a da10 5061 636b  d.<.d.S.)...Pack
+00000110: 6167 654c 6973 744d 6f64 656c 6300 0000  ageListModelc...
+00000120: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00000130: 0040 0000 0173 1200 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000140: 5a02 6503 6a04 5a05 6401 5300 2902 7a17  Z.e.j.Z.d.S.).z.
+00000150: 5061 636b 6167 654c 6973 744d 6f64 656c  PackageListModel
+00000160: 2e43 6f6e 6669 674e 2906 da08 5f5f 6e61  .ConfigN)...__na
+00000170: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000180: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7206  ..__qualname__r.
+00000190: 0000 00da 0561 6c6c 6f77 da05 6578 7472  .....allow..extr
+000001a0: 61a9 0072 0d00 0000 720d 0000 00fa 6c2f  a..r....r.....l/
+000001b0: 5573 6572 732f 7275 6269 6b2f 4472 6f70  Users/rubik/Drop
+000001c0: 626f 782f 7275 6269 6b2f 6375 7272 656e  box/rubik/curren
+000001d0: 742f 6f67 702d 706c 6179 6772 6f75 6e64  t/ogp-playground
+000001e0: 2f67 6f76 7465 6368 2d64 6174 612f 676f  /govtech-data/go
+000001f0: 7674 6563 685f 6461 7461 2f6d 6f64 656c  vtech_data/model
+00000200: 732f 7265 736f 7572 6365 732f 7061 636b  s/resources/pack
+00000210: 6167 655f 6c69 7374 2e70 79da 0643 6f6e  age_list.py..Con
+00000220: 6669 670d 0000 0073 0400 0000 0800 0a01  fig....s........
+00000230: 720f 0000 004e 7a0d 4f70 7469 6f6e 616c  r....Nz.Optional
+00000240: 5b73 7472 5dda 0468 656c 707a 0e4f 7074  [str]..helpz.Opt
+00000250: 696f 6e61 6c5b 626f 6f6c 5dda 0773 7563  ional[bool]..suc
+00000260: 6365 7373 7a13 4f70 7469 6f6e 616c 5b4c  cessz.Optional[L
+00000270: 6973 745b 7374 725d 5dda 0672 6573 756c  ist[str]]..resul
+00000280: 7429 0872 0800 0000 7209 0000 0072 0a00  t).r....r....r..
+00000290: 0000 720f 0000 0072 1000 0000 da0f 5f5f  ..r....r......__
+000002a0: 616e 6e6f 7461 7469 6f6e 735f 5f72 1100  annotations__r..
+000002b0: 0000 7212 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+000002c0: 0072 0d00 0000 720e 0000 0072 0700 0000  .r....r....r....
+000002d0: 0c00 0000 730a 0000 000a 000e 010c 030c  ....s...........
+000002e0: 0110 0172 0700 0000 4e29 09da 0a5f 5f66  ...r....N)...__f
+000002f0: 7574 7572 655f 5f72 0200 0000 da06 7479  uture__r......ty
+00000300: 7069 6e67 7203 0000 0072 0400 0000 da08  pingr....r......
+00000310: 7079 6461 6e74 6963 7205 0000 0072 0600  pydanticr....r..
+00000320: 0000 7207 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000330: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
+00000340: 6475 6c65 3e01 0000 0073 0800 0000 0c04  dule>....s......
+00000350: 1002 1002 1403                           ......
```

### Comparing `govtech_data-0.1.0/govtech_data/models/resources/package_show.py` & `govtech_data-0.1.1/govtech_data/models/resources/package_show.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,68 @@
 # generated by datamodel-codegen:
 #   filename:  package_show.json
-#   timestamp: 2023-04-14T08:17:30+00:00
+#   timestamp: 2023-04-14T09:27:05+00:00
 
 from __future__ import annotations
 
 from typing import Any, List, Optional
 
 from pydantic import BaseModel, Extra
 
 
+class NullValues(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    count: Optional[int] = None
+
+
+class Field(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    name: Optional[str] = None
+    format: Optional[str] = None
+    coordinate_system: Optional[str] = None
+    null_values: Optional[NullValues] = None
+    detected_types: Optional[str] = None
+    title: Optional[str] = None
+    total: Optional[int] = None
+    type: Optional[str] = None
+    sub_type: Optional[str] = None
+    unit_of_measure: Optional[str] = None
+
+
 class Resource(BaseModel):
     class Config:
         extra = Extra.allow
 
     cache_last_updated: Optional[Any] = None
     coverage_start: Optional[str] = None
-    documentation_url: Optional[str] = None
     package_id: Optional[str] = None
-    update_frequency: Optional[str] = None
+    validation_state: Optional[str] = None
+    coverage_end: Optional[str] = None
     datastore_active: Optional[bool] = None
     id: Optional[str] = None
     size: Optional[Any] = None
-    realtime: Optional[bool] = None
+    reject_reason: Optional[str] = None
+    redo_approval: Optional[bool] = None
     state: Optional[str] = None
     hash: Optional[str] = None
     description: Optional[str] = None
     format: Optional[str] = None
-    last_modified: Optional[Any] = None
-    url_type: Optional[Any] = None
+    mimetype_inner: Optional[Any] = None
+    url_type: Optional[str] = None
     mimetype: Optional[Any] = None
     cache_url: Optional[Any] = None
     name: Optional[str] = None
     created: Optional[str] = None
     url: Optional[str] = None
-    mimetype_inner: Optional[Any] = None
+    fields: Optional[List[Field]] = None
+    last_modified: Optional[str] = None
     position: Optional[int] = None
     revision_id: Optional[str] = None
     resource_type: Optional[Any] = None
 
 
 class Tag(BaseModel):
     class Config:
@@ -79,40 +104,40 @@
     approval_status: Optional[str] = None
 
 
 class Result(BaseModel):
     class Config:
         extra = Extra.allow
 
-    license_title: Optional[Any] = None
-    maintainer: Optional[Any] = None
-    sysadmin_edit_only: Optional[str] = None
-    relationships_as_object: Optional[List] = None
+    license_title: Optional[str] = None
+    maintainer: Optional[str] = None
+    coverage_start: Optional[str] = None
     topics: Optional[List[str]] = None
     private: Optional[bool] = None
-    maintainer_email: Optional[Any] = None
+    maintainer_email: Optional[str] = None
     num_tags: Optional[int] = None
     sources: Optional[List[str]] = None
     frequency: Optional[str] = None
+    coverage_end: Optional[str] = None
     id: Optional[str] = None
     metadata_modified: Optional[str] = None
-    author: Optional[Any] = None
-    author_email: Optional[Any] = None
+    author: Optional[str] = None
+    author_email: Optional[str] = None
     state: Optional[str] = None
-    version: Optional[Any] = None
+    version: Optional[str] = None
     metadata_created: Optional[str] = None
-    coverage_start: Optional[str] = None
+    relationships_as_object: Optional[List] = None
     creator_user_id: Optional[str] = None
     type: Optional[str] = None
     resources: Optional[List[Resource]] = None
     num_resources: Optional[int] = None
     description: Optional[str] = None
     tags: Optional[List[Tag]] = None
     groups: Optional[List[Group]] = None
-    license_id: Optional[Any] = None
+    license_id: Optional[str] = None
     relationships_as_subject: Optional[List] = None
     organization: Optional[Organization] = None
     name: Optional[str] = None
     isopen: Optional[bool] = None
     url: Optional[str] = None
     notes: Optional[str] = None
     owner_org: Optional[str] = None
```

### Comparing `govtech_data-0.1.0/govtech_data/utils/__pycache__/models.cpython-310.pyc` & `govtech_data-0.1.1/govtech_data/utils/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `govtech_data-0.1.0/govtech_data/utils/models.py` & `govtech_data-0.1.1/govtech_data/utils/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 from datamodel_code_generator import __main__ as dcg_main
 from loguru import logger
 
 JSON_RESPONSE_PATH = "./json/models"
 OUTPUT_MODELS_PATH = "./govtech_data/models/resources/"
```

### Comparing `govtech_data-0.1.0/PKG-INFO` & `govtech_data-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: govtech-data
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library to easily access and read data from data.gov.sg
 License: Singapore Open Data License
 Author: Khee-Chin Chua
+Author-email: kheechin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: datamodel-code-generator (>=0.17.2,<0.18.0)
 Requires-Dist: fuzzywuzzy (>=0.18.0,<0.19.0)
+Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-levenshtein (>=0.20.9,<0.21.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
```

