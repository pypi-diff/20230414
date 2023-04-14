# Comparing `tmp/fastapi_oracle-0.6.1-py3-none-any.whl.zip` & `tmp/fastapi_oracle-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 13242 bytes, number of entries: 11
+Zip file size: 13319 bytes, number of entries: 11
 -rw-r--r--  2.0 unx     1412 b- defN 80-Jan-01 00:00 fastapi_oracle/__init__.py
 -rw-r--r--  2.0 unx      767 b- defN 80-Jan-01 00:00 fastapi_oracle/config.py
--rw-r--r--  2.0 unx      891 b- defN 80-Jan-01 00:00 fastapi_oracle/constants.py
+-rw-r--r--  2.0 unx      893 b- defN 80-Jan-01 00:00 fastapi_oracle/constants.py
 -rw-r--r--  2.0 unx     8671 b- defN 80-Jan-01 00:00 fastapi_oracle/core.py
 -rw-r--r--  2.0 unx     2088 b- defN 80-Jan-01 00:00 fastapi_oracle/errors.py
 -rw-r--r--  2.0 unx      207 b- defN 80-Jan-01 00:00 fastapi_oracle/pools.py
--rw-r--r--  2.0 unx     1793 b- defN 80-Jan-01 00:00 fastapi_oracle/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_oracle-0.6.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx      888 b- defN 16-Jan-01 00:00 fastapi_oracle-0.6.1.dist-info/RECORD
-11 files, 32786 bytes uncompressed, 11746 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx     2004 b- defN 80-Jan-01 00:00 fastapi_oracle/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 80-Jan-01 00:00 fastapi_oracle-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4624 b- defN 80-Jan-01 00:00 fastapi_oracle-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fastapi_oracle-0.7.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      888 b- defN 16-Jan-01 00:00 fastapi_oracle-0.7.0.dist-info/RECORD
+11 files, 32999 bytes uncompressed, 11823 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: fastapi_oracle/pools.py
 Comment: 
 
 Filename: fastapi_oracle/utils.py
 Comment: 
 
-Filename: fastapi_oracle-0.6.1.dist-info/LICENSE
+Filename: fastapi_oracle-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: fastapi_oracle-0.6.1.dist-info/METADATA
+Filename: fastapi_oracle-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_oracle-0.6.1.dist-info/WHEEL
+Filename: fastapi_oracle-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_oracle-0.6.1.dist-info/RECORD
+Filename: fastapi_oracle-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapi_oracle/constants.py

```diff
@@ -25,15 +25,15 @@
 
 
 class DbPoolAndCreatedTime(NamedTuple):
     pool: AsyncPoolWrapper
     created_time: float
 
 
-DEFAULT_MAX_ROWS = 1000
+DEFAULT_MAX_ROWS = 10_000
 
 # Thanks to: https://stackoverflow.com/a/1176023/2066849
 CAMEL_TO_SNAKE_REGEX = re.compile(r"(?<!^)(?=[A-Z])")
 
 PACKAGE_STATE_INVALIDATED_REGEX = re.compile(
     r'existing state of package body "[^"]+" has been invalidated'
 )
```

## fastapi_oracle/utils.py

```diff
@@ -1,12 +1,13 @@
 from collections.abc import AsyncIterable, Mapping
 from typing import Any, AsyncGenerator, Generator
 
 from cx_Oracle import Object
 from cx_Oracle_async.cursors import AsyncCursorWrapper
+from loguru import logger
 
 from fastapi_oracle.constants import DEFAULT_MAX_ROWS
 
 
 def cursor_rows_as_dicts(cursor: AsyncCursorWrapper):
     """Make the specified cursor return its rows as dicts instead of tuples.
 
@@ -20,15 +21,22 @@
 
 async def cursor_rows_as_gen(
     cursor: AsyncCursorWrapper, max_rows: int = DEFAULT_MAX_ROWS
 ) -> AsyncGenerator[Any, None]:
     """Loop through the specified cursor's results in a generator."""
     i = 0
 
-    while (row := await cursor.fetchone()) is not None and i < max_rows:
+    while (row := await cursor.fetchone()) is not None:
+        if i >= max_rows:
+            logger.warning(
+                "Max rows exceeded while looping through cursor results "
+                f"(max_rows={max_rows})"
+            )
+            break
+
         yield row
         i += 1
 
 
 def coll_records_as_dicts(coll: Object) -> Generator[dict[str, Any], None, None]:
     """Make the specified collection of records into simple dicts."""
     for record in coll.aslist():
```

## Comparing `fastapi_oracle-0.6.1.dist-info/LICENSE` & `fastapi_oracle-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapi_oracle-0.6.1.dist-info/METADATA` & `fastapi_oracle-0.7.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-oracle
-Version: 0.6.1
+Version: 0.7.0
 Summary: Helpers for using the cx_Oracle_async library with the FastAPI framework.
 Home-page: https://github.com/Jaza/fastapi-oracle
 License: Apache-2.0
 Author: Jeremy Epstein
 Author-email: jazepstein@gmail.com
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `fastapi_oracle-0.6.1.dist-info/RECORD` & `fastapi_oracle-0.7.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 fastapi_oracle/__init__.py,sha256=zRvlU5zn4jQ1aoh-0hfM7ryDCDwUVkX-J7ykbNk4jBc,1412
 fastapi_oracle/config.py,sha256=hDQbaVzjX2vOb8ujxYWDGM-n39_r5lXQeCJd__Qeo9M,767
-fastapi_oracle/constants.py,sha256=Rg-nkuQXVQQoAeE9AUdsa4RNv0nMKscVvYSa1pqpfeM,891
+fastapi_oracle/constants.py,sha256=Zh3D4PEPSL6SlSdyC2dwDNGz_wBkPACjDNoMre35KLs,893
 fastapi_oracle/core.py,sha256=9LyLb-jhc11JBrId0pxigbHLzNGWAzoe0XHevWoxFqI,8671
 fastapi_oracle/errors.py,sha256=owpkOovw44qoHuqpVkrJuxFIJ5XuGWH2cv_wuFaEQGs,2088
 fastapi_oracle/pools.py,sha256=fVkOPrtwoQMhlI85szk6k7m6tvPUGLmGKCBHGOqyl2U,207
-fastapi_oracle/utils.py,sha256=HhOAibZLmGxEhbouXtFjjjn50NzoTLL7R6EHEyZJcVU,1793
-fastapi_oracle-0.6.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-fastapi_oracle-0.6.1.dist-info/METADATA,sha256=zk_opuPhHw7oxSfCVu30lBjK37afPHU94dPFmn9l8dU,4624
-fastapi_oracle-0.6.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fastapi_oracle-0.6.1.dist-info/RECORD,,
+fastapi_oracle/utils.py,sha256=lrVlggTIL609ND7kJwKhmwYegiFo2AGfrVK-e8wovkI,2004
+fastapi_oracle-0.7.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+fastapi_oracle-0.7.0.dist-info/METADATA,sha256=EQTVSfA8F9hilVpmwgxVzXdQcNnuMfdhVRA9JnUoyzM,4624
+fastapi_oracle-0.7.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+fastapi_oracle-0.7.0.dist-info/RECORD,,
```

