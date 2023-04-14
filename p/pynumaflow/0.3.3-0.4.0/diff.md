# Comparing `tmp/pynumaflow-0.3.3.tar.gz` & `tmp/pynumaflow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumaflow-0.3.3.tar", max compression
+gzip compressed data, was "pynumaflow-0.4.0.tar", max compression
```

## Comparing `pynumaflow-0.3.3.tar` & `pynumaflow-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,43 @@
--rw-r--r--   0        0        0    11357 2023-02-14 18:08:46.454029 pynumaflow-0.3.3/LICENSE
--rw-r--r--   0        0        0     2259 2023-02-14 18:08:46.454029 pynumaflow-0.3.3/README.md
--rw-r--r--   0        0        0      464 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/__init__.py
--rw-r--r--   0        0        0      451 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/_constants.py
--rw-r--r--   0        0        0      357 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/function/__init__.py
--rw-r--r--   0        0        0     5477 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/function/_dtypes.py
--rw-r--r--   0        0        0     1887 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/function/_udfunction_pb2.pyi
--rw-r--r--   0        0        0      512 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/function/asynciter.py
--rw-r--r--   0        0        0        0 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/function/generated/__init__.py
--rw-r--r--   0        0        0     4251 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/function/generated/udfunction_pb2.py
--rw-r--r--   0        0        0     5709 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/function/generated/udfunction_pb2_grpc.py
--rw-r--r--   0        0        0     9952 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/function/server.py
--rw-r--r--   0        0        0      195 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/sink/__init__.py
--rw-r--r--   0        0        0     2947 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/sink/_dtypes.py
--rw-r--r--   0        0        0     2373 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/sink/_udfunction_pb2.pyi
--rw-r--r--   0        0        0        0 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/sink/generated/__init__.py
--rw-r--r--   0        0        0     4660 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/sink/generated/udsink_pb2.py
--rw-r--r--   0        0        0     4109 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/sink/generated/udsink_pb2_grpc.py
--rw-r--r--   0        0        0     5395 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/sink/server.py
--rw-r--r--   0        0        0       79 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/tests/function/__init__.py
--rw-r--r--   0        0        0     8095 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/tests/function/test_async_server.py
--rw-r--r--   0        0        0     4755 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/tests/function/test_datatypes.py
--rw-r--r--   0        0        0     4335 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/tests/function/test_messages.py
--rw-r--r--   0        0        0     7169 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/tests/function/test_server.py
--rw-r--r--   0        0        0        0 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/tests/sink/__init__.py
--rw-r--r--   0        0        0     2984 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/tests/sink/test_datatypes.py
--rw-r--r--   0        0        0     1304 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/tests/sink/test_responses.py
--rw-r--r--   0        0        0     5970 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/tests/sink/test_server.py
--rw-r--r--   0        0        0      169 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pynumaflow/types.py
--rw-r--r--   0        0        0     1294 2023-02-14 18:08:46.458029 pynumaflow-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3350 1970-01-01 00:00:00.000000 pynumaflow-0.3.3/setup.py
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 pynumaflow-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 17:52:54.631606 pynumaflow-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3506 2023-04-14 17:52:54.631606 pynumaflow-0.4.0/README.md
+-rw-r--r--   0        0        0      985 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/__init__.py
+-rw-r--r--   0        0        0      511 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/_constants.py
+-rw-r--r--   0        0        0      248 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/exceptions.py
+-rw-r--r--   0        0        0      521 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/function/__init__.py
+-rw-r--r--   0        0        0     9146 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/function/_dtypes.py
+-rw-r--r--   0        0        0     1779 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/function/_udfunction_pb2.pyi
+-rw-r--r--   0        0        0    11695 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/function/async_server.py
+-rw-r--r--   0        0        0      512 2023-04-14 17:52:54.639607 pynumaflow-0.4.0/pynumaflow/function/asynciter.py
+-rw-r--r--   0        0        0    10262 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/multiproc_server.py
+-rw-r--r--   0        0        0        0 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/proto/__init__.py
+-rw-r--r--   0        0        0     2029 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/proto/udfunction.proto
+-rw-r--r--   0        0        0     3137 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/proto/udfunction_pb2.py
+-rw-r--r--   0        0        0     7522 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/proto/udfunction_pb2_grpc.py
+-rw-r--r--   0        0        0     8370 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/function/server.py
+-rw-r--r--   0        0        0      219 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/__init__.py
+-rw-r--r--   0        0        0     3290 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/_dtypes.py
+-rw-r--r--   0        0        0     2257 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/_udfunction_pb2.pyi
+-rw-r--r--   0        0        0     5429 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/async_sink.py
+-rw-r--r--   0        0        0        0 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/proto/__init__.py
+-rw-r--r--   0        0        0     1716 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/proto/udsink.proto
+-rw-r--r--   0        0        0     2512 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/proto/udsink_pb2.py
+-rw-r--r--   0        0        0     4105 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/proto/udsink_pb2_grpc.py
+-rw-r--r--   0        0        0     4696 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/sink/server.py
+-rw-r--r--   0        0        0       79 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/__init__.py
+-rw-r--r--   0        0        0     2037 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/server_utils.py
+-rw-r--r--   0        0        0    10505 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_async_server.py
+-rw-r--r--   0        0        0     4678 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_async_server_err.py
+-rw-r--r--   0        0        0     6720 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_datatypes.py
+-rw-r--r--   0        0        0     3889 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_messages.py
+-rw-r--r--   0        0        0     3663 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_messagets.py
+-rw-r--r--   0        0        0     9632 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_multiproc.py
+-rw-r--r--   0        0        0     8131 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/function/test_sync_server.py
+-rw-r--r--   0        0        0        0 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/sink/__init__.py
+-rw-r--r--   0        0        0     5153 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/sink/test_async_sink.py
+-rw-r--r--   0        0        0     3327 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/sink/test_datatypes.py
+-rw-r--r--   0        0        0     1305 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/sink/test_responses.py
+-rw-r--r--   0        0        0     5937 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/tests/sink/test_server.py
+-rw-r--r--   0        0        0      170 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pynumaflow/types.py
+-rw-r--r--   0        0        0     1358 2023-04-14 17:52:54.643607 pynumaflow-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4696 1970-01-01 00:00:00.000000 pynumaflow-0.4.0/PKG-INFO
```

### Comparing `pynumaflow-0.3.3/LICENSE` & `pynumaflow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.3.3/pynumaflow/function/_udfunction_pb2.pyi` & `pynumaflow-0.4.0/pynumaflow/function/_udfunction_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from typing import (
     ClassVar as _ClassVar,
-    Mapping as _Mapping,
     Optional as _Optional,
-    Union as _Union,
     List,
 )
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ReadyResponse(_message.Message):
     __slots__ = ["ready"]
     READY_FIELD_NUMBER: _ClassVar[int]
     ready: bool
+
     def __init__(self, ready: _Optional[bool] = ...) -> None: ...
 
 class EventTime(_message.Message):
     __slots__ = ["event_time"]
     EVENT_TIME_FIELD_NUMBER: _ClassVar[int]
     event_time: _timestamp_pb2.Timestamp
+
     def __init__(self, event_time: _Optional[_timestamp_pb2.Timestamp] = ...) -> None: ...
 
 class Watermark(_message.Message):
     __slots__ = ["watermark"]
     WATERMARK_FIELD_NUMBER: _ClassVar[int]
     watermark: _timestamp_pb2.Timestamp
+
     def __init__(self, watermark: _Optional[_timestamp_pb2.Timestamp] = ...) -> None: ...
 
 class Datum(_message.Message):
-    __slots__ = ["key", "value", "event_time", "watermark"]
-    KEY_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["keys", "value", "event_time", "watermark"]
+    KEYS_FIELD_NUMBER: _ClassVar[int]
     VALUE_FIELD_NUMBER: _ClassVar[int]
     EVENT_TIME_FIELD_NUMBER: _ClassVar[int]
     WATERMARK_FIELD_NUMBER: _ClassVar[int]
     key: str
     value: bytes
     event_time: _timestamp_pb2.Timestamp
     watermark: _timestamp_pb2.Timestamp
+
     def __init__(
         self,
-        key: _Optional[str],
+        keys: _Optional[List[str]],
         value: _Optional[bytes],
         event_time: _Optional[_timestamp_pb2.Timestamp] = ...,
         watermark: _Optional[_timestamp_pb2.Timestamp] = ...,
     ) -> None: ...
 
 class DatumList(_message.Message):
     __slots__ = ["elements"]
     ELEMENTS_FIELD_NUMBER: _ClassVar[int]
     elements: List[Datum]
+
     def __init__(self, elements: _Optional[List[Datum]]) -> None: ...
```

### Comparing `pynumaflow-0.3.3/pynumaflow/function/asynciter.py` & `pynumaflow-0.4.0/pynumaflow/function/asynciter.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.3.3/pynumaflow/function/generated/udfunction_pb2_grpc.py` & `pynumaflow-0.4.0/pynumaflow/function/proto/udfunction_pb2_grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,65 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from pynumaflow.function.generated import udfunction_pb2 as udfunction__pb2
+from . import udfunction_pb2 as udfunction__pb2
 
 
 class UserDefinedFunctionStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
-
         Args:
             channel: A grpc.Channel.
         """
         self.MapFn = channel.unary_unary(
             "/function.v1.UserDefinedFunction/MapFn",
-            request_serializer=udfunction__pb2.Datum.SerializeToString,
-            response_deserializer=udfunction__pb2.DatumList.FromString,
+            request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
+            response_deserializer=udfunction__pb2.DatumResponseList.FromString,
+        )
+        self.MapTFn = channel.unary_unary(
+            "/function.v1.UserDefinedFunction/MapTFn",
+            request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
+            response_deserializer=udfunction__pb2.DatumResponseList.FromString,
         )
-        self.ReduceFn = channel.stream_unary(
+        self.ReduceFn = channel.stream_stream(
             "/function.v1.UserDefinedFunction/ReduceFn",
-            request_serializer=udfunction__pb2.Datum.SerializeToString,
-            response_deserializer=udfunction__pb2.DatumList.FromString,
+            request_serializer=udfunction__pb2.DatumRequest.SerializeToString,
+            response_deserializer=udfunction__pb2.DatumResponseList.FromString,
         )
         self.IsReady = channel.unary_unary(
             "/function.v1.UserDefinedFunction/IsReady",
             request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             response_deserializer=udfunction__pb2.ReadyResponse.FromString,
         )
 
 
 class UserDefinedFunctionServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def MapFn(self, request, context):
-        """Applies a function to each datum element."""
+        """MapFn applies a function to each datum element."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
+    def MapTFn(self, request, context):
+        """MapTFn applies a function to each datum element.
+        In addition to map function, MapTFn also supports assigning a new event time to datum.
+        MapTFn can be used only at source vertex by source data transformer.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def ReduceFn(self, request_iterator, context):
-        """Applies a reduce function to a datum stream."""
+        """ReduceFn applies a reduce function to a datum stream."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def IsReady(self, request, context):
         """IsReady is the heartbeat endpoint for gRPC."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
@@ -54,21 +67,26 @@
         raise NotImplementedError("Method not implemented!")
 
 
 def add_UserDefinedFunctionServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "MapFn": grpc.unary_unary_rpc_method_handler(
             servicer.MapFn,
-            request_deserializer=udfunction__pb2.Datum.FromString,
-            response_serializer=udfunction__pb2.DatumList.SerializeToString,
+            request_deserializer=udfunction__pb2.DatumRequest.FromString,
+            response_serializer=udfunction__pb2.DatumResponseList.SerializeToString,
         ),
-        "ReduceFn": grpc.stream_unary_rpc_method_handler(
+        "MapTFn": grpc.unary_unary_rpc_method_handler(
+            servicer.MapTFn,
+            request_deserializer=udfunction__pb2.DatumRequest.FromString,
+            response_serializer=udfunction__pb2.DatumResponseList.SerializeToString,
+        ),
+        "ReduceFn": grpc.stream_stream_rpc_method_handler(
             servicer.ReduceFn,
-            request_deserializer=udfunction__pb2.Datum.FromString,
-            response_serializer=udfunction__pb2.DatumList.SerializeToString,
+            request_deserializer=udfunction__pb2.DatumRequest.FromString,
+            response_serializer=udfunction__pb2.DatumResponseList.SerializeToString,
         ),
         "IsReady": grpc.unary_unary_rpc_method_handler(
             servicer.IsReady,
             request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             response_serializer=udfunction__pb2.ReadyResponse.SerializeToString,
         ),
     }
@@ -95,16 +113,45 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.unary_unary(
             request,
             target,
             "/function.v1.UserDefinedFunction/MapFn",
-            udfunction__pb2.Datum.SerializeToString,
-            udfunction__pb2.DatumList.FromString,
+            udfunction__pb2.DatumRequest.SerializeToString,
+            udfunction__pb2.DatumResponseList.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def MapTFn(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/function.v1.UserDefinedFunction/MapTFn",
+            udfunction__pb2.DatumRequest.SerializeToString,
+            udfunction__pb2.DatumResponseList.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -120,20 +167,20 @@
         call_credentials=None,
         insecure=False,
         compression=None,
         wait_for_ready=None,
         timeout=None,
         metadata=None,
     ):
-        return grpc.experimental.stream_unary(
+        return grpc.experimental.stream_stream(
             request_iterator,
             target,
             "/function.v1.UserDefinedFunction/ReduceFn",
-            udfunction__pb2.Datum.SerializeToString,
-            udfunction__pb2.DatumList.FromString,
+            udfunction__pb2.DatumRequest.SerializeToString,
+            udfunction__pb2.DatumResponseList.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
```

### Comparing `pynumaflow-0.3.3/pynumaflow/function/server.py` & `pynumaflow-0.4.0/pynumaflow/function/async_server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,153 +1,184 @@
 import asyncio
 import logging
 import multiprocessing
 import os
-from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timezone
-from typing import Callable, AsyncIterable
+from typing import Callable, AsyncIterable, List
 
 import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import (
     FUNCTION_SOCK_PATH,
-    DATUM_KEY,
     WIN_START_TIME,
     WIN_END_TIME,
     MAX_MESSAGE_SIZE,
     STREAM_EOF,
+    DELIMITER,
 )
-from pynumaflow.function import Messages, Datum, IntervalWindow, Metadata
-from pynumaflow.function._dtypes import ReduceResult
+from pynumaflow.function import Messages, MessageTs, Datum, IntervalWindow, Metadata
+from pynumaflow.function._dtypes import ReduceResult, DatumMetadata
 from pynumaflow.function.asynciter import NonBlockingIterator
-from pynumaflow.function.generated import udfunction_pb2
-from pynumaflow.function.generated import udfunction_pb2_grpc
+from pynumaflow.function.proto import udfunction_pb2
+from pynumaflow.function.proto import udfunction_pb2_grpc
 from pynumaflow.types import NumaflowServicerContext
 
-
 _LOGGER = setup_logging(__name__)
 if os.getenv("PYTHONDEBUG"):
     _LOGGER.setLevel(logging.DEBUG)
 
-UDFMapCallable = Callable[[str, Datum], Messages]
-UDFReduceCallable = Callable[[str, AsyncIterable[Datum], Metadata], Messages]
+UDFMapCallable = Callable[[List[str], Datum], Messages]
+UDFMapTCallable = Callable[[List[str], Datum], MessageTs]
+UDFReduceCallable = Callable[[List[str], AsyncIterable[Datum], Metadata], Messages]
 _PROCESS_COUNT = multiprocessing.cpu_count()
 MAX_THREADS = int(os.getenv("MAX_THREADS", 0)) or (_PROCESS_COUNT * 4)
 
 
-class UserDefinedFunctionServicer(udfunction_pb2_grpc.UserDefinedFunctionServicer):
+async def datum_generator(
+    request_iterator: AsyncIterable[udfunction_pb2.DatumRequest],
+) -> AsyncIterable[Datum]:
+    async for d in request_iterator:
+        datum = Datum(
+            keys=list(d.keys),
+            value=d.value,
+            event_time=d.event_time.event_time.ToDatetime(),
+            watermark=d.watermark.watermark.ToDatetime(),
+            metadata=DatumMetadata(
+                msg_id=d.metadata.id,
+                num_delivered=d.metadata.num_delivered,
+            ),
+        )
+        yield datum
+
+
+class AsyncServer(udfunction_pb2_grpc.UserDefinedFunctionServicer):
     """
     Provides an interface to write a User Defined Function (UDFunction)
     which will be exposed over gRPC.
 
     Args:
         map_handler: Function callable following the type signature of UDFMapCallable
+        mapt_handler: Function callable following the type signature of UDFMapTCallable
         reduce_handler: Function callable following the type signature of UDFReduceCallable
         sock_path: Path to the UNIX Domain Socket
         max_message_size: The max message size in bytes the server can receive and send
         max_threads: The max number of threads to be spawned;
                      defaults to number of processors x4
 
     Example invocation:
     >>> from typing import Iterator
-    >>> from pynumaflow.function import Messages, Message, \
-    ...     Datum, Metadata, UserDefinedFunctionServicer
+    >>> from pynumaflow.function import Messages, Message, MessageTs, MessageT, \
+    ...     Datum, Metadata, AsyncServer
     ... import aiorun
     ...
-    >>> def map_handler(key: str, datum: Datum) -> Messages:
+    >>> async def map_handler(key: [str], datum: Datum) -> Messages:
     ...   val = datum.value
     ...   _ = datum.event_time
     ...   _ = datum.watermark
-    ...   messages = Messages(Message.to_vtx(key, val))
+    ...   messages = Messages(Message(val, keys=keys))
     ...   return messages
     ...
+    ...async def mapT_handler(key: [str], datum: Datum) -> Messages:
+    ...         "Not supported"
+    ...
     >>> async def reduce_handler(key: str, datums: Iterator[Datum], md: Metadata) -> Messages:
     ...   interval_window = md.interval_window
     ...   counter = 0
     ...   async for _ in datums:
     ...     counter += 1
     ...   msg = (
     ...       f"counter:{counter} interval_window_start:{interval_window.start} "
     ...       f"interval_window_end:{interval_window.end}"
     ...   )
-    ...   return Messages(Message.to_vtx(key, str.encode(msg)))
+    ...   return Messages(Message(value=str.encode(msg), keys=keys))
     ...
-    >>> grpc_server = UserDefinedFunctionServicer(
+    >>> grpc_server = AsyncServer(
     ...   reduce_handler=reduce_handler,
     ...   map_handler=map_handler,
     ... )
-    >>> aiorun.run(grpc_server.start_async())
+    >>> aiorun.run(grpc_server.start())
     """
 
     def __init__(
         self,
         map_handler: UDFMapCallable = None,
+        mapt_handler: UDFMapTCallable = None,
         reduce_handler: UDFReduceCallable = None,
         sock_path=FUNCTION_SOCK_PATH,
         max_message_size=MAX_MESSAGE_SIZE,
         max_threads=MAX_THREADS,
     ):
-
-        if not (map_handler or reduce_handler):
-            raise ValueError("Require a valid map handler and/or a valid reduce handler.")
+        if not (map_handler or mapt_handler or reduce_handler):
+            raise ValueError("Require a valid map/mapt handler and/or a valid reduce handler.")
 
         self.__map_handler: UDFMapCallable = map_handler
+        self.__mapt_handler: UDFMapTCallable = mapt_handler
         self.__reduce_handler: UDFReduceCallable = reduce_handler
         self.sock_path = f"unix://{sock_path}"
         self._max_message_size = max_message_size
         self._max_threads = max_threads
         self.cleanup_coroutines = []
+        # Collection for storing strong references to all running tasks.
+        # Event loop only keeps a weak reference, which can cause it to
+        # get lost during execution.
+        self.background_tasks = set()
 
         self._server_options = [
             ("grpc.max_send_message_length", self._max_message_size),
             ("grpc.max_receive_message_length", self._max_message_size),
         ]
 
-    def MapFn(
-        self, request: udfunction_pb2.Datum, context: NumaflowServicerContext
-    ) -> udfunction_pb2.DatumList:
+    async def MapFn(
+        self, request: udfunction_pb2.DatumRequest, context: NumaflowServicerContext
+    ) -> udfunction_pb2.DatumResponseList:
         """
         Applies a function to each datum element.
-        The pascal case function name comes from the generated udfunction_pb2_grpc.py file.
+        The pascal case function name comes from the proto udfunction_pb2_grpc.py file.
         """
-        key = ""
-        for metadata_key, metadata_value in context.invocation_metadata():
-            if metadata_key == DATUM_KEY:
-                key = metadata_value
+        # proto repeated field(keys) is of type google._upb._message.RepeatedScalarContainer
+        # we need to explicitly convert it to list
+        res = await self.__invoke_map(
+            list(request.keys),
+            Datum(
+                keys=list(request.keys),
+                value=request.value,
+                event_time=request.event_time.event_time.ToDatetime(),
+                watermark=request.watermark.watermark.ToDatetime(),
+                metadata=DatumMetadata(
+                    msg_id=request.metadata.id,
+                    num_delivered=request.metadata.num_delivered,
+                ),
+            ),
+        )
+        return udfunction_pb2.DatumResponseList(elements=res)
 
+    async def __invoke_map(self, keys: List[str], req: Datum):
         try:
-            msgs = self.__map_handler(
-                key,
-                Datum(
-                    key=key,
-                    value=request.value,
-                    event_time=request.event_time.event_time.ToDatetime(),
-                    watermark=request.watermark.watermark.ToDatetime(),
-                ),
-            )
+            msgs = await self.__map_handler(keys, req)
         except Exception as err:
-            _LOGGER.critical("UDFError, dropping message on the floor: %r", err, exc_info=True)
-
-            # a neat hack to drop
-            msgs = Messages.as_forward_all(None)
-
+            _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
+            raise err
         datums = []
         for msg in msgs.items():
-            datums.append(udfunction_pb2.Datum(key=msg.key, value=msg.value))
+            datums.append(
+                udfunction_pb2.DatumResponse(keys=msg.keys, value=msg.value, tags=msg.tags)
+            )
 
-        return udfunction_pb2.DatumList(elements=datums)
+        return datums
 
     async def ReduceFn(
-        self, request_iterator: AsyncIterable[Datum], context: NumaflowServicerContext
-    ) -> udfunction_pb2.DatumList:
+        self,
+        request_iterator: AsyncIterable[udfunction_pb2.DatumRequest],
+        context: NumaflowServicerContext,
+    ) -> udfunction_pb2.DatumResponseList:
         """
         Applies a reduce function to a datum stream.
-        The pascal case function name comes from the generated udfunction_pb2_grpc.py file.
+        The pascal case function name comes from the proto udfunction_pb2_grpc.py file.
         """
 
         start, end = None, None
         for metadata_key, metadata_value in context.invocation_metadata():
             if metadata_key == WIN_START_TIME:
                 start = metadata_value
             elif metadata_key == WIN_END_TIME:
@@ -158,78 +189,102 @@
                 f"got start: {start}, end: {end}."
             )
 
         start_dt = datetime.fromtimestamp(int(start) / 1e3, timezone.utc)
         end_dt = datetime.fromtimestamp(int(end) / 1e3, timezone.utc)
         interval_window = IntervalWindow(start=start_dt, end=end_dt)
 
+        datum_iterator = datum_generator(request_iterator=request_iterator)
+
         response_task = asyncio.create_task(
-            self.__async_reduce_handler(interval_window, request_iterator)
+            self.__async_reduce_handler(interval_window, datum_iterator)
         )
 
+        # Save a reference to the result of this function, to avoid a
+        # task disappearing mid-execution.
+        self.background_tasks.add(response_task)
+        response_task.add_done_callback(lambda t: self.background_tasks.remove(t))
+
         await response_task
-        return response_task.result()
+        results_futures = response_task.result()
 
-    async def __async_reduce_handler(self, interval_window, request_iterator: AsyncIterable[Datum]):
+        for fut in results_futures:
+            await fut
+            yield udfunction_pb2.DatumResponseList(elements=fut.result())
+
+    async def __async_reduce_handler(self, interval_window, datum_iterator: AsyncIterable[Datum]):
         callable_dict = {}
         # iterate through all the values
-        async for d in request_iterator:
-            key = d.key
-            result = callable_dict.get(key, None)
+        async for d in datum_iterator:
+            keys = d.keys()
+            unified_key = DELIMITER.join(keys)
+            result = callable_dict.get(unified_key, None)
 
             if not result:
                 niter = NonBlockingIterator()
                 riter = niter.read_iterator()
-                # schedule a async task for consumer
+                # schedule an async task for consumer
                 # returns a future that will give the results later.
                 task = asyncio.create_task(
-                    self.__invoke_reduce(key, riter, Metadata(interval_window=interval_window))
+                    self.__invoke_reduce(keys, riter, Metadata(interval_window=interval_window))
                 )
-                result = ReduceResult(task, niter, key)
+                # Save a reference to the result of this function, to avoid a
+                # task disappearing mid-execution.
+                self.background_tasks.add(task)
+                task.add_done_callback(lambda t: self.background_tasks.remove(t))
+                result = ReduceResult(task, niter, keys)
 
-                callable_dict[key] = result
+                callable_dict[unified_key] = result
 
             await result.iterator.put(d)
-        datums = []
-        for key in callable_dict:
-            await callable_dict[key].iterator.put(STREAM_EOF)
 
-        for key in callable_dict:
-            fut = callable_dict[key].future
-            await fut
-            datums = datums + fut.result()
-        return udfunction_pb2.DatumList(elements=datums)
+        for unified_key in callable_dict:
+            await callable_dict[unified_key].iterator.put(STREAM_EOF)
+
+        tasks = []
+        for unified_key in callable_dict:
+            fut = callable_dict[unified_key].future
+            tasks.append(fut)
 
-    async def __invoke_reduce(self, key: str, request_iterator: AsyncIterable[Datum], md: Metadata):
+        return tasks
+
+    async def __invoke_reduce(
+        self, keys: List[str], request_iterator: AsyncIterable[Datum], md: Metadata
+    ):
         try:
-            msgs = await self.__reduce_handler(key, request_iterator, md)
+            msgs = await self.__reduce_handler(keys, request_iterator, md)
         except Exception as err:
-            _LOGGER.critical("UDFError, dropping message on the floor: %r", err, exc_info=True)
+            _LOGGER.critical("UDFError, re-raising the error: %r", err, exc_info=True)
+            raise err
 
-            # a neat hack to drop
-            msgs = Messages.as_forward_all(None)
-
-        datums = []
+        datum_responses = []
         for msg in msgs.items():
-            datums.append(udfunction_pb2.Datum(key=msg.key, value=msg.value))
+            datum_responses.append(
+                udfunction_pb2.DatumResponse(keys=msg.keys, value=msg.value, tags=msg.tags)
+            )
 
-        return datums
+        return datum_responses
 
-    def IsReady(
+    async def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> udfunction_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
-        The pascal case function name comes from the generated udfunction_pb2_grpc.py file.
+        The pascal case function name comes from the proto udfunction_pb2_grpc.py file.
         """
         return udfunction_pb2.ReadyResponse(ready=True)
 
     async def __serve_async(self, server) -> None:
         udfunction_pb2_grpc.add_UserDefinedFunctionServicer_to_server(
-            UserDefinedFunctionServicer(self.__map_handler, self.__reduce_handler), server
+            AsyncServer(
+                map_handler=self.__map_handler,
+                mapt_handler=self.__mapt_handler,
+                reduce_handler=self.__reduce_handler,
+            ),
+            server,
         )
         server.add_insecure_port(self.sock_path)
         _LOGGER.info("GRPC Async Server listening on: %s", self.sock_path)
         await server.start()
 
         async def server_graceful_shutdown():
             """
@@ -239,26 +294,11 @@
             """
             _LOGGER.info("Starting graceful shutdown...")
             await server.stop(5)
 
         self.cleanup_coroutines.append(server_graceful_shutdown())
         await server.wait_for_termination()
 
-    async def start_async(self) -> None:
+    async def start(self) -> None:
         """Starts the Async gRPC server on the given UNIX socket."""
         server = grpc.aio.server(options=self._server_options)
         await self.__serve_async(server)
-
-    def start(self) -> None:
-        """
-        Starts the gRPC server on the given UNIX socket with given max threads.
-        """
-        server = grpc.server(
-            ThreadPoolExecutor(max_workers=self._max_threads), options=self._server_options
-        )
-        udfunction_pb2_grpc.add_UserDefinedFunctionServicer_to_server(self, server)
-        server.add_insecure_port(self.sock_path)
-        server.start()
-        _LOGGER.info(
-            "GRPC Server listening on: %s with max threads: %s", self.sock_path, self._max_threads
-        )
-        server.wait_for_termination()
```

### Comparing `pynumaflow-0.3.3/pynumaflow/sink/_dtypes.py` & `pynumaflow-0.4.0/pynumaflow/sink/_dtypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,54 +41,70 @@
         return str(self)
 
 
 class Datum:
     """
     Class to define the important information for the event.
     Args:
+        keys: the keys of the event.
         value: the payload of the event.
         event_time: the event time of the event.
         watermark: the watermark of the event.
     >>> # Example usage
     >>> from pynumaflow.function import Datum
     >>> from datetime import datetime, timezone
     >>> payload = bytes("test_mock_message", encoding="utf-8")
     >>> t1 = datetime.fromtimestamp(1662998400, timezone.utc)
     >>> t2 = datetime.fromtimestamp(1662998460, timezone.utc)
     >>> msg_id = "test_id"
-    >>> d = Datum(sink_msg_id=msg_id, value=payload, event_time=t1, watermark=t2)
+    >>> output_keys = ["test_key"]
+    >>> d = Datum(keys=output_keys, sink_msg_id=msg_id, value=payload, event_time=t1, watermark=t2)
     """
 
-    def __init__(self, sink_msg_id: str, value: bytes, event_time: datetime, watermark: datetime):
+    def __init__(
+        self,
+        keys: List[str],
+        sink_msg_id: str,
+        value: bytes,
+        event_time: datetime,
+        watermark: datetime,
+    ):
+        self._keys = keys
         self._id = sink_msg_id or ""
         self._value = value or b""
         if not isinstance(event_time, datetime):
             raise TypeError(f"Wrong data type: {type(event_time)} for Datum.event_time")
         self._event_time = event_time
         if not isinstance(watermark, datetime):
             raise TypeError(f"Wrong data type: {type(watermark)} for Datum.watermark")
         self._watermark = watermark
 
     def __str__(self):
         value_string = self._value.decode("utf-8")
         return (
+            f"keys: {self._keys}, "
             f"id: {self._id}, value: {value_string}, "
             f"event_time: {str(self._event_time)}, "
             f"watermark: {str(self._watermark)}"
         )
 
     def __repr__(self):
         return str(self)
 
     @property
     def id(self) -> str:
         """Returns the id of the event."""
         return self._id
 
     @property
+    def keys(self) -> List[str]:
+        """Returns the keys of the event."""
+        return self._keys
+
+    @property
     def value(self) -> bytes:
         """Returns the value of the event."""
         return self._value
 
     @property
     def event_time(self) -> datetime:
         """Returns the event time of the event."""
```

### Comparing `pynumaflow-0.3.3/pynumaflow/sink/_udfunction_pb2.pyi` & `pynumaflow-0.4.0/pynumaflow/sink/_udfunction_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from typing import (
     ClassVar as _ClassVar,
-    Mapping as _Mapping,
     Optional as _Optional,
-    Union as _Union,
     List,
 )
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ReadyResponse(_message.Message):
     __slots__ = ["ready"]
     READY_FIELD_NUMBER: _ClassVar[int]
     ready: bool
+
     def __init__(self, ready: _Optional[bool] = ...) -> None: ...
 
 class EventTime(_message.Message):
     __slots__ = ["event_time"]
     EVENT_TIME_FIELD_NUMBER: _ClassVar[int]
     event_time: _timestamp_pb2.Timestamp
+
     def __init__(self, event_time: _Optional[_timestamp_pb2.Timestamp] = ...) -> None: ...
 
 class Watermark(_message.Message):
     __slots__ = ["watermark"]
     WATERMARK_FIELD_NUMBER: _ClassVar[int]
     watermark: _timestamp_pb2.Timestamp
+
     def __init__(self, watermark: _Optional[_timestamp_pb2.Timestamp] = ...) -> None: ...
 
 class Datum(_message.Message):
     __slots__ = ["key", "value", "event_time", "watermark", "id"]
     KEY_FIELD_NUMBER: _ClassVar[int]
     VALUE_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     EVENT_TIME_FIELD_NUMBER: _ClassVar[int]
     WATERMARK_FIELD_NUMBER: _ClassVar[int]
     key: str
     value: bytes
     id: str
     event_time: _timestamp_pb2.Timestamp
     watermark: _timestamp_pb2.Timestamp
+
     def __init__(
         self,
         key: _Optional[str],
         value: _Optional[bytes],
         id: _Optional[str],
         event_time: _Optional[_timestamp_pb2.Timestamp] = ...,
         watermark: _Optional[_timestamp_pb2.Timestamp] = ...,
@@ -55,19 +56,21 @@
     __slots__ = ["id", "success", "err_msg"]
     ID_FIELD_NUMBER: _ClassVar[int]
     SUCCESS_FIELD_NUMBER: _ClassVar[int]
     ERR_MSG_FIELD_NUMBER: _ClassVar[int]
     id: str
     success: bool
     err_msg: str
+
     def __init__(
         self,
         id: _Optional[str],
         success: _Optional[bool],
         err_msg: _Optional[str],
     ) -> None: ...
 
 class ResponseList(_message.Message):
     __slots__ = ["responses"]
     RESPONSES_FIELD_NUMBER: _ClassVar[int]
     responses: List[Response]
+
     def __init__(self, responses: _Optional[List[Response]]) -> None: ...
```

### Comparing `pynumaflow-0.3.3/pynumaflow/sink/generated/udsink_pb2_grpc.py` & `pynumaflow-0.4.0/pynumaflow/sink/proto/udsink_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from pynumaflow.sink.generated import udsink_pb2 as udsink__pb2
+from . import udsink_pb2 as udsink__pb2
 
 
 class UserDefinedSinkStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
-
         Args:
             channel: A grpc.Channel.
         """
         self.SinkFn = channel.stream_unary(
             "/sink.v1.UserDefinedSink/SinkFn",
-            request_serializer=udsink__pb2.Datum.SerializeToString,
+            request_serializer=udsink__pb2.DatumRequest.SerializeToString,
             response_deserializer=udsink__pb2.ResponseList.FromString,
         )
         self.IsReady = channel.unary_unary(
             "/sink.v1.UserDefinedSink/IsReady",
             request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             response_deserializer=udsink__pb2.ReadyResponse.FromString,
         )
@@ -43,15 +42,15 @@
         raise NotImplementedError("Method not implemented!")
 
 
 def add_UserDefinedSinkServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "SinkFn": grpc.stream_unary_rpc_method_handler(
             servicer.SinkFn,
-            request_deserializer=udsink__pb2.Datum.FromString,
+            request_deserializer=udsink__pb2.DatumRequest.FromString,
             response_serializer=udsink__pb2.ResponseList.SerializeToString,
         ),
         "IsReady": grpc.unary_unary_rpc_method_handler(
             servicer.IsReady,
             request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             response_serializer=udsink__pb2.ReadyResponse.SerializeToString,
         ),
@@ -79,15 +78,15 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.stream_unary(
             request_iterator,
             target,
             "/sink.v1.UserDefinedSink/SinkFn",
-            udsink__pb2.Datum.SerializeToString,
+            udsink__pb2.DatumRequest.SerializeToString,
             udsink__pb2.ResponseList.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
```

### Comparing `pynumaflow-0.3.3/pynumaflow/sink/server.py` & `pynumaflow-0.4.0/pynumaflow/sink/async_sink.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,115 +1,133 @@
 import logging
 import multiprocessing
 import os
-from concurrent.futures import ThreadPoolExecutor
-from typing import Callable, Iterator
+from typing import Callable, Iterator, AsyncIterable
 
 import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow import setup_logging
 from pynumaflow._constants import (
     SINK_SOCK_PATH,
     MAX_MESSAGE_SIZE,
 )
 from pynumaflow.sink import Responses, Datum, Response
-from pynumaflow.sink.generated import udsink_pb2_grpc, udsink_pb2
+from pynumaflow.sink.proto import udsink_pb2_grpc, udsink_pb2
 from pynumaflow.types import NumaflowServicerContext
 
-
 _LOGGER = setup_logging(__name__)
 if os.getenv("PYTHONDEBUG"):
     _LOGGER.setLevel(logging.DEBUG)
 
-
 UDSinkCallable = Callable[[Iterator[Datum]], Responses]
 _PROCESS_COUNT = multiprocessing.cpu_count()
 MAX_THREADS = int(os.getenv("MAX_THREADS", 0)) or (_PROCESS_COUNT * 4)
 
 
-class UserDefinedSinkServicer(udsink_pb2_grpc.UserDefinedSinkServicer):
+async def datum_generator(
+    request_iterator: AsyncIterable[udsink_pb2.DatumRequest],
+) -> AsyncIterable[Datum]:
+    async for d in request_iterator:
+        datum = Datum(
+            keys=list(d.keys),
+            sink_msg_id=d.id,
+            value=d.value,
+            event_time=d.event_time.event_time.ToDatetime(),
+            watermark=d.watermark.watermark.ToDatetime(),
+        )
+        yield datum
+
+
+class AsyncSink(udsink_pb2_grpc.UserDefinedSinkServicer):
     """
     Provides an interface to write a User Defined Sink (UDSink)
-    which will be exposed over gRPC.
+    which will be exposed over an Asyncronous gRPC server.
 
     Args:
         sink_handler: Function callable following the type signature of UDSinkCallable
         sock_path: Path to the UNIX Domain Socket
         max_message_size: The max message size in bytes the server can receive and send
         max_threads: The max number of threads to be spawned;
                      defaults to number of processors x 4
 
     Example invocation:
     >>> from typing import List
-    >>> from pynumaflow.sink import Datum, Responses, Response, UserDefinedSinkServicer
-    >>> def my_handler(datums: Iterator[Datum]) -> Responses:
+    >>> from pynumaflow.sink import Datum, Responses, Response, Sink
+    >>> async def my_handler(datums: AsyncIterable[Datum]) -> Responses:
     ...   responses = Responses()
-    ...   for msg in datums:
+    ...   async for msg in datums:
     ...     responses.append(Response.as_success(msg.id))
     ...   return responses
-    >>> grpc_server = UserDefinedSinkServicer(my_handler)
-    >>> grpc_server.start()
+    >>> grpc_server = AsyncSink(my_handler)
+    >>> aiorun.run(grpc_server.start())
     """
 
     def __init__(
         self,
         sink_handler: UDSinkCallable,
         sock_path=SINK_SOCK_PATH,
         max_message_size=MAX_MESSAGE_SIZE,
         max_threads=MAX_THREADS,
     ):
+        self.background_tasks = set()
         self.__sink_handler: UDSinkCallable = sink_handler
         self.sock_path = f"unix://{sock_path}"
         self._max_message_size = max_message_size
         self._max_threads = max_threads
         self.cleanup_coroutines = []
 
         self._server_options = [
             ("grpc.max_send_message_length", self._max_message_size),
             ("grpc.max_receive_message_length", self._max_message_size),
         ]
 
-    def SinkFn(
-        self, request_iterator: Iterator[Datum], context: NumaflowServicerContext
+    async def SinkFn(
+        self,
+        request_iterator: AsyncIterable[udsink_pb2.DatumRequest],
+        context: NumaflowServicerContext,
     ) -> udsink_pb2.ResponseList:
         """
         Applies a sink function to a list of datum elements.
-        The pascal case function name comes from the generated udsink_pb2_grpc.py file.
+        The pascal case function name comes from the proto udsink_pb2_grpc.py file.
         """
         # if there is an exception, we will mark all the responses as a failure
+        datum_iterator = datum_generator(request_iterator=request_iterator)
+        results = await self.__invoke_sink(datum_iterator)
+
+        return udsink_pb2.ResponseList(responses=results)
+
+    async def __invoke_sink(self, datum_iterator: AsyncIterable[Datum]):
         try:
-            rspns = self.__sink_handler(request_iterator)
+            rspns = await self.__sink_handler(datum_iterator)
         except Exception as err:
             err_msg = "UDSinkError: %r" % err
             _LOGGER.critical(err_msg, exc_info=True)
             rspns = Responses()
-            for _datum in request_iterator:
+            async for _datum in datum_iterator:
                 rspns.append(Response.as_failure(_datum.id, err_msg))
-
         responses = []
         for rspn in rspns.items():
             responses.append(
                 udsink_pb2.Response(id=rspn.id, success=rspn.success, err_msg=rspn.err)
             )
+        return responses
 
-        return udsink_pb2.ResponseList(responses=responses)
-
-    def IsReady(
+    async def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> udsink_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
-        The pascal case function name comes from the generated udsink_pb2_grpc.py file.
+        The pascal case function name comes from the proto udsink_pb2_grpc.py file.
         """
         return udsink_pb2.ReadyResponse(ready=True)
 
     async def __serve_async(self, server) -> None:
         udsink_pb2_grpc.add_UserDefinedSinkServicer_to_server(
-            UserDefinedSinkServicer(self.__sink_handler), server
+            AsyncSink(self.__sink_handler), server
         )
         server.add_insecure_port(self.sock_path)
         _LOGGER.info("GRPC Async Server listening on: %s", self.sock_path)
         await server.start()
 
         async def server_graceful_shutdown():
             _LOGGER.info("Starting graceful shutdown...")
@@ -119,28 +137,11 @@
             existing RPCs to continue within the grace period.
             await server.stop(5)
             """
 
         self.cleanup_coroutines.append(server_graceful_shutdown())
         await server.wait_for_termination()
 
-    async def start_async(self) -> None:
+    async def start(self) -> None:
         """Starts the Async gRPC server on the given UNIX socket."""
         server = grpc.aio.server(options=self._server_options)
         await self.__serve_async(server)
-
-    def start(self) -> None:
-        """
-        Starts the gRPC server on the given UNIX socket with given max threads.
-        """
-        server = grpc.server(
-            ThreadPoolExecutor(max_workers=self._max_threads), options=self._server_options
-        )
-        udsink_pb2_grpc.add_UserDefinedSinkServicer_to_server(
-            UserDefinedSinkServicer(self.__sink_handler), server
-        )
-        server.add_insecure_port(self.sock_path)
-        server.start()
-        _LOGGER.info(
-            "GRPC Server listening on: %s with max threads: %s", self.sock_path, self._max_threads
-        )
-        server.wait_for_termination()
```

### Comparing `pynumaflow-0.3.3/pynumaflow/tests/function/test_async_server.py` & `pynumaflow-0.4.0/pynumaflow/tests/function/test_multiproc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,242 +1,245 @@
-import asyncio
-import logging
-import threading
+import os
 import unittest
-from typing import AsyncIterable
+from unittest import mock
 
 import grpc
-
+from google.protobuf import empty_pb2 as _empty_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
-from grpc.aio._server import Server
+from grpc import StatusCode
+from grpc_testing import server_from_dictionary, strict_real_time
 
-from pynumaflow import setup_logging
-from pynumaflow._constants import DATUM_KEY, WIN_START_TIME, WIN_END_TIME
-from pynumaflow.function import Messages, Message, Datum, Metadata, UserDefinedFunctionServicer
-from pynumaflow.function.generated import udfunction_pb2, udfunction_pb2_grpc
-from pynumaflow.tests.function.test_server import (
+from pynumaflow.function.multiproc_server import MultiProcServer
+from pynumaflow.function.proto import udfunction_pb2_grpc, udfunction_pb2
+from pynumaflow.tests.function.server_utils import (
+    mapt_handler,
     map_handler,
+    err_map_handler,
     mock_event_time,
     mock_watermark,
     mock_message,
-    mock_interval_window_start,
-    mock_interval_window_end,
+    mock_new_event_time,
+    err_mapt_handler,
 )
+from pynumaflow.tests.function.test_async_server import async_reduce_handler
+
+
+def mockenv(**envvars):
+    return mock.patch.dict(os.environ, envvars)
+
+
+class TestMultiProcMethods(unittest.TestCase):
+    def setUp(self) -> None:
+        my_servicer = MultiProcServer(
+            map_handler=map_handler, mapt_handler=mapt_handler, reduce_handler=async_reduce_handler
+        )
+        services = {udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"]: my_servicer}
+        self.test_server = server_from_dictionary(services, strict_real_time())
+
+    @mockenv(NUM_CPU_MULTIPROC="3")
+    def test_multiproc_init(self) -> None:
+        server = MultiProcServer(
+            reduce_handler=async_reduce_handler, map_handler=map_handler, mapt_handler=mapt_handler
+        )
+        self.assertEqual(server._sock_path, 55551)
+        self.assertEqual(server._process_count, 3)
 
-LOGGER = setup_logging(__name__)
+    # To test the reuse property for the grpc servers which allow multiple
+    # bindings to the same server
+    def test_reuse_port(self):
+        serv_options = [("grpc.so_reuseport", 1), ("grpc.so_reuseaddr", 1)]
 
+        server = MultiProcServer(
+            reduce_handler=async_reduce_handler, map_handler=map_handler, mapt_handler=mapt_handler
+        )
+
+        with server._reserve_port() as port:
+            print(port)
+            bind_address = f"localhost:{port}"
+            server1 = grpc.server(thread_pool=None, options=serv_options)
+            udfunction_pb2_grpc.add_UserDefinedFunctionServicer_to_server(server, server1)
+            server1.add_insecure_port(bind_address)
+
+            # so_reuseport=0 -> the bind should raise an error
+            server2 = grpc.server(thread_pool=None, options=(("grpc.so_reuseport", 0),))
+            udfunction_pb2_grpc.add_UserDefinedFunctionServicer_to_server(server, server2)
+            self.assertRaises(RuntimeError, server2.add_insecure_port, bind_address)
+
+            # so_reuseport=1 -> should allow server to bind to port again
+            server3 = grpc.server(thread_pool=None, options=(("grpc.so_reuseport", 1),))
+            udfunction_pb2_grpc.add_UserDefinedFunctionServicer_to_server(server, server3)
+            server3.add_insecure_port(bind_address)
+
+    def test_udf_map_err(self):
+        my_servicer = MultiProcServer(map_handler=err_map_handler)
+        services = {udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"]: my_servicer}
+        self.test_server = server_from_dictionary(services, strict_real_time())
 
-async def async_reduce_handler(key: str, datums: AsyncIterable[Datum], md: Metadata) -> Messages:
-    interval_window = md.interval_window
-    counter = 0
-    async for _ in datums:
-        counter += 1
-    msg = (
-        f"counter:{counter} interval_window_start:{interval_window.start} "
-        f"interval_window_end:{interval_window.end}"
-    )
-
-    return Messages(Message.to_vtx(key, str.encode(msg)))
-
-
-def request_generator(count, request, resetkey: bool = False):
-    for i in range(count):
-        if resetkey:
-            request.key = f"key-{i}"
-        yield request
-
-
-def start_reduce_streaming_request() -> (Datum, tuple):
-    event_time_timestamp = _timestamp_pb2.Timestamp()
-    event_time_timestamp.FromDatetime(dt=mock_event_time())
-    watermark_timestamp = _timestamp_pb2.Timestamp()
-    watermark_timestamp.FromDatetime(dt=mock_watermark())
-
-    request = udfunction_pb2.Datum(
-        value=mock_message(),
-        event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
-        watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
-    )
-
-    metadata = (
-        (DATUM_KEY, "test"),
-        (WIN_START_TIME, f"{mock_interval_window_start()}"),
-        (WIN_END_TIME, f"{mock_interval_window_end()}"),
-    )
-    return request, metadata
-
-
-_s: Server = None
-_channel = grpc.insecure_channel("localhost:50051")
-_loop = None
-
-
-def startup_callable(loop):
-    asyncio.set_event_loop(loop)
-    loop.run_forever()
-
-
-async def start_server():
-    server = grpc.aio.server()
-    udfs = UserDefinedFunctionServicer(
-        reduce_handler=async_reduce_handler,
-        map_handler=map_handler,
-    )
-    udfunction_pb2_grpc.add_UserDefinedFunctionServicer_to_server(udfs, server)
-    listen_addr = "[::]:50051"
-    server.add_insecure_port(listen_addr)
-    logging.info("Starting server on %s", listen_addr)
-    global _s
-    _s = server
-    await server.start()
-    await server.wait_for_termination()
-
-
-class TestAsyncServer(unittest.TestCase):
-    @classmethod
-    def setUpClass(cls) -> None:
-        global _loop
-        loop = asyncio.new_event_loop()
-        _loop = loop
-        _thread = threading.Thread(target=startup_callable, args=(loop,), daemon=True)
-        _thread.start()
-        asyncio.run_coroutine_threadsafe(start_server(), loop=loop)
-        while True:
-            try:
-                with grpc.insecure_channel("localhost:50051") as channel:
-                    f = grpc.channel_ready_future(channel)
-                    f.result(timeout=10)
-                    if f.done():
-                        break
-            except grpc.FutureTimeoutError as e:
-                LOGGER.error("error trying to connect to grpc server")
-                LOGGER.error(e)
-
-    @classmethod
-    def tearDownClass(cls) -> None:
-        try:
-            _loop.stop()
-            LOGGER.info("stopped the event loop")
-        except Exception as e:
-            LOGGER.error(e)
-
-    def test_run_server(self) -> None:
-        with grpc.insecure_channel("localhost:50051") as channel:
-            stub = udfunction_pb2_grpc.UserDefinedFunctionStub(channel)
-            event_time_timestamp = _timestamp_pb2.Timestamp()
-            event_time_timestamp.FromDatetime(dt=mock_event_time())
-            watermark_timestamp = _timestamp_pb2.Timestamp()
-            watermark_timestamp.FromDatetime(dt=mock_watermark())
-
-            request = udfunction_pb2.Datum(
-                value=mock_message(),
-                event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
-                watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
-            )
+        event_time_timestamp = _timestamp_pb2.Timestamp()
+        event_time_timestamp.FromDatetime(dt=mock_event_time())
+        watermark_timestamp = _timestamp_pb2.Timestamp()
+        watermark_timestamp.FromDatetime(dt=mock_watermark())
 
-            metadata = (
-                (DATUM_KEY, "test"),
+        request = udfunction_pb2.DatumRequest(
+            value=mock_message(),
+            event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
+            watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
+        )
+
+        method = self.test_server.invoke_unary_unary(
+            method_descriptor=(
+                udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"].methods_by_name[
+                    "MapFn"
+                ]
+            ),
+            invocation_metadata={
                 ("this_metadata_will_be_skipped", "test_ignore"),
-            )
-            response = None
-            try:
-                response = stub.MapFn(request=request, metadata=metadata)
-            except grpc.RpcError as e:
-                logging.error(e)
-
-            self.assertEqual(1, len(response.elements))
-            self.assertEqual("test", response.elements[0].key)
-            self.assertEqual(
-                bytes(
-                    "payload:test_mock_message "
-                    "event_time:2022-09-12 16:00:00 watermark:2022-09-12 16:01:00",
-                    encoding="utf-8",
-                ),
-                response.elements[0].value,
-            )
-            LOGGER.info("Successfully validated the server")
+            },
+            request=request,
+            timeout=1,
+        )
+        response, metadata, code, details = method.termination()
+        self.assertEqual(None, response)
+
+    def test_udf_mapt_err(self):
+        my_servicer = MultiProcServer(mapt_handler=err_mapt_handler)
+        services = {udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"]: my_servicer}
+        self.test_server = server_from_dictionary(services, strict_real_time())
 
-    def test_map(self) -> None:
-        stub = udfunction_pb2_grpc.UserDefinedFunctionStub(_channel)
         event_time_timestamp = _timestamp_pb2.Timestamp()
         event_time_timestamp.FromDatetime(dt=mock_event_time())
         watermark_timestamp = _timestamp_pb2.Timestamp()
         watermark_timestamp.FromDatetime(dt=mock_watermark())
 
-        request = udfunction_pb2.Datum(
+        request = udfunction_pb2.DatumRequest(
             value=mock_message(),
             event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
             watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
         )
 
-        metadata = (
-            (DATUM_KEY, "test"),
-            ("this_metadata_will_be_skipped", "test_ignore"),
+        method = self.test_server.invoke_unary_unary(
+            method_descriptor=(
+                udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"].methods_by_name[
+                    "MapTFn"
+                ]
+            ),
+            invocation_metadata={
+                ("this_metadata_will_be_skipped", "test_ignore"),
+            },
+            request=request,
+            timeout=1,
         )
+        response, metadata, code, details = method.termination()
+        self.assertEqual(None, response)
 
-        response = None
-        try:
-            response = stub.MapFn(request=request, metadata=metadata)
-        except grpc.RpcError as e:
-            LOGGER.error(e)
+    def test_is_ready(self):
+        method = self.test_server.invoke_unary_unary(
+            method_descriptor=(
+                udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"].methods_by_name[
+                    "IsReady"
+                ]
+            ),
+            invocation_metadata={},
+            request=_empty_pb2.Empty(),
+            timeout=1,
+        )
 
+        response, metadata, code, details = method.termination()
+        expected = udfunction_pb2.ReadyResponse(ready=True)
+        self.assertEqual(expected, response)
+        self.assertEqual(code, StatusCode.OK)
+
+    def test_map_forward_message(self):
+        event_time_timestamp = _timestamp_pb2.Timestamp()
+        event_time_timestamp.FromDatetime(dt=mock_event_time())
+        watermark_timestamp = _timestamp_pb2.Timestamp()
+        watermark_timestamp.FromDatetime(dt=mock_watermark())
+
+        request = udfunction_pb2.DatumRequest(
+            keys=["test"],
+            value=mock_message(),
+            event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
+            watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
+        )
+
+        method = self.test_server.invoke_unary_unary(
+            method_descriptor=(
+                udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"].methods_by_name[
+                    "MapFn"
+                ]
+            ),
+            invocation_metadata={
+                ("this_metadata_will_be_skipped", "test_ignore"),
+            },
+            request=request,
+            timeout=1,
+        )
+
+        response, metadata, code, details = method.termination()
         self.assertEqual(1, len(response.elements))
-        self.assertEqual("test", response.elements[0].key)
+        self.assertEqual(["test"], response.elements[0].keys)
         self.assertEqual(
             bytes(
                 "payload:test_mock_message "
                 "event_time:2022-09-12 16:00:00 watermark:2022-09-12 16:01:00",
                 encoding="utf-8",
             ),
             response.elements[0].value,
         )
+        self.assertEqual(code, StatusCode.OK)
 
-    def test_reduce(self) -> None:
-        stub = self.__stub()
-        request, metadata = start_reduce_streaming_request()
-        response = None
-        try:
-            response = stub.ReduceFn(
-                request_iterator=request_generator(count=10, request=request), metadata=metadata
-            )
-        except grpc.RpcError as e:
-            logging.error(e)
+    def test_mapt_assign_new_event_time(self, test_server=None):
+        event_time_timestamp = _timestamp_pb2.Timestamp()
+        event_time_timestamp.FromDatetime(dt=mock_event_time())
+        watermark_timestamp = _timestamp_pb2.Timestamp()
+        watermark_timestamp.FromDatetime(dt=mock_watermark())
 
-        self.assertEqual(1, len(response.elements))
-        self.assertEqual(
-            bytes(
-                "counter:10 interval_window_start:2022-09-12 16:00:00+00:00 "
-                "interval_window_end:2022-09-12 16:01:00+00:00",
-                encoding="utf-8",
+        request = udfunction_pb2.DatumRequest(
+            keys=["test"],
+            value=mock_message(),
+            event_time=udfunction_pb2.EventTime(event_time=event_time_timestamp),
+            watermark=udfunction_pb2.Watermark(watermark=watermark_timestamp),
+        )
+        serv = self.test_server
+        if test_server:
+            serv = test_server
+
+        method = serv.invoke_unary_unary(
+            method_descriptor=(
+                udfunction_pb2.DESCRIPTOR.services_by_name["UserDefinedFunction"].methods_by_name[
+                    "MapTFn"
+                ]
             ),
-            response.elements[0].value,
+            invocation_metadata={
+                ("this_metadata_will_be_skipped", "test_ignore"),
+            },
+            request=request,
+            timeout=1,
         )
 
-    def test_reduce_with_multiple_keys(self) -> None:
-        stub = self.__stub()
-        request, metadata = start_reduce_streaming_request()
-        response = None
-        try:
-            response = stub.ReduceFn(
-                request_iterator=request_generator(count=10, request=request, resetkey=True),
-                metadata=metadata,
-            )
-        except grpc.RpcError as e:
-            print(e)
-
-        self.assertEqual(10, len(response.elements))
+        response, metadata, code, details = method.termination()
+        self.assertEqual(1, len(response.elements))
+        self.assertEqual(["test"], response.elements[0].keys)
         self.assertEqual(
             bytes(
-                "counter:1 interval_window_start:2022-09-12 16:00:00+00:00 "
-                "interval_window_end:2022-09-12 16:01:00+00:00",
+                "payload:test_mock_message "
+                "event_time:2022-09-12 16:00:00 watermark:2022-09-12 16:01:00",
                 encoding="utf-8",
             ),
             response.elements[0].value,
         )
+        # Verify new event time gets assigned.
+        updated_event_time_timestamp = _timestamp_pb2.Timestamp()
+        updated_event_time_timestamp.FromDatetime(dt=mock_new_event_time())
+        self.assertEqual(
+            udfunction_pb2.EventTime(event_time=updated_event_time_timestamp),
+            response.elements[0].event_time,
+        )
+        self.assertEqual(code, StatusCode.OK)
 
-    def __stub(self):
-        return udfunction_pb2_grpc.UserDefinedFunctionStub(_channel)
+    def test_invalid_input(self):
+        with self.assertRaises(ValueError):
+            MultiProcServer()
 
 
 if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
     unittest.main()
```

### Comparing `pynumaflow-0.3.3/pynumaflow/tests/function/test_messages.py` & `pynumaflow-0.4.0/pynumaflow/tests/function/test_messages.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,112 +1,101 @@
 import unittest
-from dataclasses import FrozenInstanceError
 
-from pynumaflow.function import Messages, Message, ALL, DROP
+from pynumaflow.function import Messages, Message, DROP
 
 
 def mock_message():
     msg = bytes("test_mock_message", encoding="utf-8")
     return msg
 
 
 class TestMessage(unittest.TestCase):
     def test_key(self):
-        mock_obj = {"Key": ALL, "Value": mock_message()}
-        msg = Message(key=mock_obj["Key"], value=mock_obj["Value"])
+        mock_obj = {"Keys": "test-key", "Value": mock_message()}
+        msg = Message(value=mock_obj["Value"], keys=mock_obj["Keys"])
         print(msg)
-        self.assertEqual(mock_obj["Key"], msg.key)
-
-    def test_immutable(self):
-        msg = Message(ALL, mock_message())
-        with self.assertRaises(FrozenInstanceError):
-            msg.key = DROP
+        self.assertEqual(mock_obj["Keys"], msg.keys)
 
     def test_value(self):
-        mock_obj = {"Key": ALL, "Value": mock_message()}
-        msgs = Message(key=mock_obj["Key"], value=mock_obj["Value"])
-        self.assertEqual(mock_obj["Value"], msgs.value)
+        mock_obj = {"Keys": "test-key", "Value": mock_message()}
+        msg = Message(value=mock_obj["Value"], keys=mock_obj["Keys"])
+        self.assertEqual(mock_obj["Value"], msg.value)
 
     def test_message_to_all(self):
-        mock_obj = {"Key": ALL, "Value": mock_message()}
-        msg = Message.to_all(mock_obj["Value"])
+        mock_obj = {"Keys": [], "Value": mock_message(), "Tags": []}
+        msg = Message(mock_obj["Value"])
         self.assertEqual(Message, type(msg))
-        self.assertEqual(mock_obj["Key"], msg.key)
+        self.assertEqual(mock_obj["Keys"], msg.keys)
         self.assertEqual(mock_obj["Value"], msg.value)
+        self.assertEqual(mock_obj["Tags"], msg.tags)
 
     def test_message_to_drop(self):
-        mock_obj = {"Key": DROP, "Value": b""}
-        msgs = Message.to_drop()
-        self.assertEqual(Message, type(msgs))
-        self.assertEqual(mock_obj["Key"], msgs.key)
-        self.assertEqual(mock_obj["Value"], msgs.value)
+        mock_obj = {"Keys": [], "Value": b"", "Tags": [DROP]}
+        msg = Message(b"").to_drop()
+        self.assertEqual(Message, type(msg))
+        self.assertEqual(mock_obj["Keys"], msg.keys)
+        self.assertEqual(mock_obj["Value"], msg.value)
+        self.assertEqual(mock_obj["Tags"], msg.tags)
 
     def test_message_to(self):
-        mock_obj = {"Key": "__KEY__", "Value": mock_message()}
-        msgs = Message.to_vtx(key=mock_obj["Key"], value=mock_obj["Value"])
-        self.assertEqual(Message, type(msgs))
-        self.assertEqual(mock_obj["Key"], msgs.key)
-        self.assertEqual(mock_obj["Value"], msgs.value)
+        mock_obj = {"Keys": ["__KEY__"], "Value": mock_message(), "Tags": ["__TAG__"]}
+        msg = Message(value=mock_obj["Value"], keys=mock_obj["Keys"], tags=mock_obj["Tags"])
+        self.assertEqual(Message, type(msg))
+        self.assertEqual(mock_obj["Keys"], msg.keys)
+        self.assertEqual(mock_obj["Value"], msg.value)
+        self.assertEqual(mock_obj["Tags"], msg.tags)
 
 
 class TestMessages(unittest.TestCase):
     @staticmethod
     def mock_message_object():
         value = mock_message()
-        return Message(ALL, value)
+        return Message(value=value)
 
     def test_items(self):
         mock_obj = [
-            {"Key": b"U+005C__ALL__", "Value": mock_message()},
-            {"Key": b"U+005C__ALL__", "Value": mock_message()},
+            {"Keys": ["test_key"], "Value": mock_message()},
+            {"Keys": ["test_key"], "Value": mock_message()},
         ]
         msgs = Messages(*mock_obj)
         self.assertEqual(len(mock_obj), len(msgs.items()))
-        self.assertEqual(mock_obj[0]["Key"], msgs.items()[0]["Key"])
+        self.assertEqual(mock_obj[0]["Keys"], msgs.items()[0]["Keys"])
         self.assertEqual(mock_obj[0]["Value"], msgs.items()[0]["Value"])
         self.assertEqual(
-            "[{'Key': b'U+005C__ALL__', 'Value': b'test_mock_message'}, "
-            "{'Key': b'U+005C__ALL__', 'Value': b'test_mock_message'}]",
+            "[{'Keys': ['test_key'], 'Value': b'test_mock_message'}, "
+            "{'Keys': ['test_key'], 'Value': b'test_mock_message'}]",
             repr(msgs),
         )
 
     def test_append(self):
         msgs = Messages()
         self.assertEqual(0, len(msgs.items()))
         msgs.append(self.mock_message_object())
         self.assertEqual(1, len(msgs.items()))
         msgs.append(self.mock_message_object())
         self.assertEqual(2, len(msgs.items()))
 
-    def test_message_forward(self):
-        mock_obj = Messages(self.mock_message_object())
-        true_obj = Messages.as_forward_all(mock_message())
-        self.assertEqual(type(mock_obj), type(true_obj))
-        for i in range(len(true_obj.items())):
-            self.assertEqual(type(mock_obj.items()[i]), type(true_obj.items()[i]))
-            self.assertEqual(mock_obj.items()[i].key, true_obj.items()[i].key)
-            self.assertEqual(mock_obj.items()[i].value, true_obj.items()[i].value)
-
     def test_message_forward_to_drop(self):
         mock_obj = Messages()
-        mock_obj.append(Message(DROP, bytes()))
-        true_obj = Messages.as_forward_all(bytes())
+        mock_obj.append(Message(b"").to_drop())
+        true_obj = Messages()
+        true_obj.append(mock_obj.items()[0])
         self.assertEqual(type(mock_obj), type(true_obj))
         for i in range(len(true_obj.items())):
             self.assertEqual(type(mock_obj.items()[i]), type(true_obj.items()[i]))
-            self.assertEqual(mock_obj.items()[i].key, true_obj.items()[i].key)
+            self.assertEqual(mock_obj.items()[i].keys, true_obj.items()[i].keys)
             self.assertEqual(mock_obj.items()[i].value, true_obj.items()[i].value)
 
     def test_dump(self):
         msgs = Messages()
         msgs.append(self.mock_message_object())
         msgs.append(self.mock_message_object())
         self.assertEqual(
-            "[Message(key=b'U+005C__ALL__', value=b'test_mock_message'), "
-            "Message(key=b'U+005C__ALL__', value=b'test_mock_message')]",
+            "[Message(_keys=[], _tags=[], _value=b'test_mock_message'), "
+            "Message(_keys=[], _tags=[], _value=b'test_mock_message')]",
             msgs.dumps(),
         )
 
     def test_load(self):
         # to improve codecov
         msgs = Messages()
         msgs.loads()
```

### Comparing `pynumaflow-0.3.3/pynumaflow/tests/sink/test_datatypes.py` & `pynumaflow-0.4.0/pynumaflow/tests/sink/test_datatypes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from datetime import datetime, timezone
-from google.protobuf import timestamp_pb2 as _timestamp_pb2
 
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
 
 from pynumaflow.sink._dtypes import (
     Datum,
 )
 
 
 def mock_message():
@@ -24,77 +24,90 @@
 
 
 class TestDatum(unittest.TestCase):
     def test_err_event_time(self):
         ts = _timestamp_pb2.Timestamp()
         ts.GetCurrentTime()
         with self.assertRaises(Exception) as context:
-            Datum(sink_msg_id="test_id_0", value=mock_message(), event_time=ts, watermark=ts)
+            Datum(
+                keys=["test_key"],
+                sink_msg_id="test_id_0",
+                value=mock_message(),
+                event_time=ts,
+                watermark=ts,
+            )
         self.assertEqual(
             "Wrong data type: <class 'google.protobuf.timestamp_pb2.Timestamp'> "
             "for Datum.event_time",
             str(context.exception),
         )
 
     def test_err_watermark(self):
         ts = _timestamp_pb2.Timestamp()
         ts.GetCurrentTime()
         with self.assertRaises(Exception) as context:
             Datum(
+                keys=["test_key"],
                 sink_msg_id="test_id_0",
                 value=mock_message(),
                 event_time=mock_event_time(),
                 watermark=ts,
             )
         self.assertEqual(
             "Wrong data type: <class 'google.protobuf.timestamp_pb2.Timestamp'> "
             "for Datum.watermark",
             str(context.exception),
         )
 
     def test_value(self):
         d = Datum(
+            keys=["test_key"],
             sink_msg_id="test_id_0",
             value=mock_message(),
             event_time=mock_event_time(),
             watermark=mock_watermark(),
         )
         self.assertEqual(mock_message(), d.value)
         self.assertEqual(
+            "keys: ['test_key'], "
             "id: test_id_0, value: test_mock_message, "
             "event_time: 2022-09-12 16:00:00+00:00, watermark: 2022-09-12 16:01:00+00:00",
             str(d),
         )
         self.assertEqual(
+            "keys: ['test_key'], "
             "id: test_id_0, value: test_mock_message, "
             "event_time: 2022-09-12 16:00:00+00:00, "
             "watermark: 2022-09-12 16:01:00+00:00",
             repr(d),
         )
 
     def test_id(self):
         d = Datum(
+            keys=["test_key"],
             sink_msg_id="test_id_0",
             value=mock_message(),
             event_time=mock_event_time(),
             watermark=mock_watermark(),
         )
         self.assertEqual("test_id_0", d.id)
 
     def test_event_time(self):
         d = Datum(
+            keys=["test_key"],
             sink_msg_id="test_id_0",
             value=mock_message(),
             event_time=mock_event_time(),
             watermark=mock_watermark(),
         )
         self.assertEqual(mock_event_time(), d.event_time)
 
     def test_watermark(self):
         d = Datum(
+            keys=["test_key"],
             sink_msg_id="test_id_0",
             value=mock_message(),
             event_time=mock_event_time(),
             watermark=mock_watermark(),
         )
         self.assertEqual(mock_watermark(), d.watermark)
```

### Comparing `pynumaflow-0.3.3/pynumaflow/tests/sink/test_responses.py` & `pynumaflow-0.4.0/pynumaflow/tests/sink/test_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+
 from pynumaflow.sink import Response, Responses
 
 
 class TestResponse(unittest.TestCase):
     def test_as_success(self):
         succ_response = Response.as_success("2")
         self.assertTrue(succ_response.success)
```

### Comparing `pynumaflow-0.3.3/pynumaflow/tests/sink/test_server.py` & `pynumaflow-0.4.0/pynumaflow/tests/sink/test_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Iterator
 
 from google.protobuf import empty_pb2 as _empty_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from grpc import StatusCode
 from grpc_testing import server_from_dictionary, strict_real_time
 
-from pynumaflow.sink import Responses, Datum, Response, UserDefinedSinkServicer
-from pynumaflow.sink.generated import udsink_pb2
+from pynumaflow.sink import Responses, Datum, Response, Sink
+from pynumaflow.sink.proto import udsink_pb2
 
 
 def udsink_handler(datums: Iterator[Datum]) -> Responses:
     responses = Responses()
     for msg in datums:
         if "err" in msg.value.decode("utf-8"):
             responses.append(Response.as_failure(msg.id, "mock sink message error"))
@@ -43,15 +43,15 @@
 def mock_watermark():
     t = datetime.fromtimestamp(1662998460, timezone.utc)
     return t
 
 
 class TestServer(unittest.TestCase):
     def setUp(self) -> None:
-        my_servicer = UserDefinedSinkServicer(udsink_handler)
+        my_servicer = Sink(udsink_handler)
         services = {udsink_pb2.DESCRIPTOR.services_by_name["UserDefinedSink"]: my_servicer}
         self.test_server = server_from_dictionary(services, strict_real_time())
 
     def test_is_ready(self):
         method = self.test_server.invoke_unary_unary(
             method_descriptor=(
                 udsink_pb2.DESCRIPTOR.services_by_name["UserDefinedSink"].methods_by_name["IsReady"]
@@ -63,31 +63,31 @@
 
         response, metadata, code, details = method.termination()
         expected = udsink_pb2.ReadyResponse(ready=True)
         self.assertEqual(expected, response)
         self.assertEqual(code, StatusCode.OK)
 
     def test_udsink_err(self):
-        my_servicer = UserDefinedSinkServicer(err_udsink_handler)
+        my_servicer = Sink(err_udsink_handler)
         services = {udsink_pb2.DESCRIPTOR.services_by_name["UserDefinedSink"]: my_servicer}
         self.test_server = server_from_dictionary(services, strict_real_time())
 
         event_time_timestamp = _timestamp_pb2.Timestamp()
         event_time_timestamp.FromDatetime(dt=mock_event_time())
         watermark_timestamp = _timestamp_pb2.Timestamp()
         watermark_timestamp.FromDatetime(dt=mock_watermark())
 
         test_datums = [
-            udsink_pb2.Datum(
+            udsink_pb2.DatumRequest(
                 id="test_id_0",
                 value=mock_message(),
                 event_time=udsink_pb2.EventTime(event_time=event_time_timestamp),
                 watermark=udsink_pb2.Watermark(watermark=watermark_timestamp),
             ),
-            udsink_pb2.Datum(
+            udsink_pb2.DatumRequest(
                 id="test_id_1",
                 value=mock_err_message(),
                 event_time=udsink_pb2.EventTime(event_time=event_time_timestamp),
                 watermark=udsink_pb2.Watermark(watermark=watermark_timestamp),
             ),
         ]
 
@@ -116,21 +116,21 @@
     def test_forward_message(self):
         event_time_timestamp = _timestamp_pb2.Timestamp()
         event_time_timestamp.FromDatetime(dt=mock_event_time())
         watermark_timestamp = _timestamp_pb2.Timestamp()
         watermark_timestamp.FromDatetime(dt=mock_watermark())
 
         test_datums = [
-            udsink_pb2.Datum(
+            udsink_pb2.DatumRequest(
                 id="test_id_0",
                 value=mock_message(),
                 event_time=udsink_pb2.EventTime(event_time=event_time_timestamp),
                 watermark=udsink_pb2.Watermark(watermark=watermark_timestamp),
             ),
-            udsink_pb2.Datum(
+            udsink_pb2.DatumRequest(
                 id="test_id_1",
                 value=mock_err_message(),
                 event_time=udsink_pb2.EventTime(event_time=event_time_timestamp),
                 watermark=udsink_pb2.Watermark(watermark=watermark_timestamp),
             ),
         ]
```

### Comparing `pynumaflow-0.3.3/pyproject.toml` & `pynumaflow-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "pynumaflow"
-version = "0.3.3"
+version = "0.4.0"
 description = "Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow."
 authors = ["NumaFlow Developers"]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Vigith Maurice <vigith@gmail.com>",
 ]
 classifiers = [
     "Topic :: Software Development :: Libraries",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
 ]
+repository = "https://github.com/numaproj/numaflow-python"
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.11"
+python = ">=3.9, <3.12"
 grpcio = "^1.48.1"
 grpcio-tools = "^1.48.1"
 google-cloud = "^0.34.0"
 google-api-core = "^2.11.0"
-protobuf = "~3.20.0"
+protobuf = ">=3.20,<5.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^3.0"
```

### Comparing `pynumaflow-0.3.3/setup.py` & `pynumaflow-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,117 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# Python SDK for Numaflow
 
-packages = \
-['pynumaflow',
- 'pynumaflow.function',
- 'pynumaflow.function.generated',
- 'pynumaflow.sink',
- 'pynumaflow.sink.generated',
- 'pynumaflow.tests',
- 'pynumaflow.tests.function',
- 'pynumaflow.tests.sink']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['google-api-core>=2.11.0,<3.0.0',
- 'google-cloud>=0.34.0,<0.35.0',
- 'grpcio-tools>=1.48.1,<2.0.0',
- 'grpcio>=1.48.1,<2.0.0',
- 'protobuf>=3.20.0,<3.21.0']
-
-setup_kwargs = {
-    'name': 'pynumaflow',
-    'version': '0.3.3',
-    'description': 'Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow.',
-    'long_description': '# Python SDK for Numaflow\n\nThis SDK provides the interface for writing [UDFs](https://numaflow.numaproj.io/user-guide/user-defined-functions/) \nand [UDSinks](https://numaflow.numaproj.io/user-guide/sinks/user-defined-sinks/) in Python.\n\n## Implement a User Defined Function (UDF)\n\n\n### Map\n\n```python\nfrom pynumaflow.function import Messages, Message, Datum, UserDefinedFunctionServicer\n\n\ndef my_handler(key: str, datum: Datum) -> Messages:\n    val = datum.value\n    _ = datum.event_time\n    _ = datum.watermark\n    messages = Messages(Message.to_vtx(key, val))\n    return messages\n\n\nif __name__ == "__main__":\n    grpc_server = UserDefinedFunctionServicer(map_handler=my_handler)\n    grpc_server.start()\n```\n\n### Reduce\n\n```python\nimport asyncio\nfrom typing import Iterator\nfrom pynumaflow.function import Messages, Message, Datum, Metadata, UserDefinedFunctionServicer\n\n\nasync def my_handler(key: str, datums: Iterator[Datum], md: Metadata) -> Messages:\n    interval_window = md.interval_window\n    counter = 0\n    async for _ in datums:\n        counter += 1\n    msg = (\n        f"counter:{counter} interval_window_start:{interval_window.start} "\n        f"interval_window_end:{interval_window.end}"\n    )\n    return Messages(Message.to_vtx(key, str.encode(msg)))\n\n\nif __name__ == "__main__":\n    grpc_server = UserDefinedFunctionServicer(reduce_handler=my_handler)\n    asyncio.run(grpc_server.start())\n    asyncio.run(*grpc_server.cleanup_coroutines)\n```\n\n### Sample Image\nA sample UDF [Dockerfile](examples/function/forward_message/Dockerfile) is provided \nunder [examples](examples/function/forward_message).\n\n## Implement a User Defined Sink (UDSink)\n\n```python\nfrom typing import Iterator\nfrom pynumaflow.sink import Datum, Responses, Response, UserDefinedSinkServicer\n\n\ndef my_handler(datums: Iterator[Datum]) -> Responses:\n    responses = Responses()\n    for msg in datums:\n        print("User Defined Sink", msg.value.decode("utf-8"))\n        responses.append(Response.as_success(msg.id))\n    return responses\n\n\nif __name__ == "__main__":\n    grpc_server = UserDefinedSinkServicer(my_handler)\n    grpc_server.start()\n```\n\n### Sample Image\n\nA sample UDSink [Dockerfile](examples/sink/log/Dockerfile) is provided \nunder [examples](examples/sink/log).\n',
-    'author': 'NumaFlow Developers',
-    'author_email': 'None',
-    'maintainer': 'Avik Basu',
-    'maintainer_email': 'avikbasu93@gmail.com',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
+This SDK provides the interface for writing [UDFs](https://numaflow.numaproj.io/user-guide/user-defined-functions/user-defined-functions/) 
+and [UDSinks](https://numaflow.numaproj.io/user-guide/sinks/user-defined-sinks/) in Python.
 
+## Implement a User Defined Function (UDF)
 
-setup(**setup_kwargs)
+
+### Map
+
+```python
+from pynumaflow.function import Messages, Message, Datum, Server
+from typing import List
+
+
+def my_handler(keys: List[str], datum: Datum) -> Messages:
+    val = datum.value
+    _ = datum.event_time
+    _ = datum.watermark
+    messages = Messages(Message(value=val, keys=keys))
+    return messages
+
+
+if __name__ == "__main__":
+    grpc_server = Server(map_handler=my_handler)
+    grpc_server.start()
+```
+### MapT - Map with event time assignment capability
+In addition to the regular Map function, MapT supports assigning a new event time to the message.
+MapT is only supported at source vertex to enable (a) early data filtering and (b) watermark assignment by extracting new event time from the message payload.
+
+```python
+import datetime
+from pynumaflow.function import MessageTs, MessageT, Datum, Server
+from typing import List
+
+
+def mapt_handler(keys: List[str], datum: Datum) -> MessageTs:
+    val = datum.value
+    new_event_time = datetime.time()
+    _ = datum.watermark
+    message_t_s = MessageTs(MessageT(new_event_time, val, keys))
+    return message_t_s
+
+
+if __name__ == "__main__":
+    grpc_server = Server(mapt_handler=mapt_handler)
+    grpc_server.start()
+```
+
+### Reduce
+
+```python
+import aiorun
+import asyncio
+from typing import Iterator, List
+from pynumaflow.function import Messages, Message, Datum, Metadata, AsyncServer
+
+
+async def my_handler(keys: List[str], datums: Iterator[Datum], md: Metadata) -> Messages:
+    interval_window = md.interval_window
+    counter = 0
+    async for _ in datums:
+        counter += 1
+    msg = (
+        f"counter:{counter} interval_window_start:{interval_window.start} "
+        f"interval_window_end:{interval_window.end}"
+    )
+    return Messages(Message(str.encode(msg), keys))
+
+
+if __name__ == "__main__":
+    grpc_server = AsyncServer(reduce_handler=my_handler)
+    aiorun.run(grpc_server.start())
+```
+
+### Sample Image
+A sample UDF [Dockerfile](examples/function/forward_message/Dockerfile) is provided 
+under [examples](examples/function/forward_message).
+
+## Implement a User Defined Sink (UDSink)
+
+```python
+from typing import Iterator
+from pynumaflow.sink import Datum, Responses, Response, Sink
+
+
+def my_handler(datums: Iterator[Datum]) -> Responses:
+    responses = Responses()
+    for msg in datums:
+        print("User Defined Sink", msg.value.decode("utf-8"))
+        responses.append(Response.as_success(msg.id))
+    return responses
+
+
+if __name__ == "__main__":
+    grpc_server = Sink(my_handler)
+    grpc_server.start()
+```
+
+### Sample Image
+
+A sample UDSink [Dockerfile](examples/sink/log/Dockerfile) is provided 
+under [examples](examples/sink/log).
+
+### Datum Metadata
+The Datum object contains the message payload and metadata. Currently, there are two fields
+in metadata: the message ID, the message delivery count to indicate how many times the message
+has been delivered. You can use these metadata to implement customized logic. For example,
+```python
+...
+def my_handler(keys: List[str], datum: Datum) -> Messages:
+    num_delivered = datum.metadata.num_delivered
+    # Choose to do specific actions, if the message delivery count reaches a certain threshold.
+    if num_delivered > 3:
+        ...
+```
```

### Comparing `pynumaflow-0.3.3/PKG-INFO` & `pynumaflow-0.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,145 @@
 Metadata-Version: 2.1
 Name: pynumaflow
-Version: 0.3.3
+Version: 0.4.0
 Summary: Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow.
+Home-page: https://github.com/numaproj/numaflow-python
 License: Apache-2.0
 Author: NumaFlow Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: google-api-core (>=2.11.0,<3.0.0)
 Requires-Dist: google-cloud (>=0.34.0,<0.35.0)
 Requires-Dist: grpcio (>=1.48.1,<2.0.0)
 Requires-Dist: grpcio-tools (>=1.48.1,<2.0.0)
-Requires-Dist: protobuf (>=3.20.0,<3.21.0)
+Requires-Dist: protobuf (>=3.20,<5.0)
+Project-URL: Repository, https://github.com/numaproj/numaflow-python
 Description-Content-Type: text/markdown
 
 # Python SDK for Numaflow
 
-This SDK provides the interface for writing [UDFs](https://numaflow.numaproj.io/user-guide/user-defined-functions/) 
+This SDK provides the interface for writing [UDFs](https://numaflow.numaproj.io/user-guide/user-defined-functions/user-defined-functions/) 
 and [UDSinks](https://numaflow.numaproj.io/user-guide/sinks/user-defined-sinks/) in Python.
 
 ## Implement a User Defined Function (UDF)
 
 
 ### Map
 
 ```python
-from pynumaflow.function import Messages, Message, Datum, UserDefinedFunctionServicer
+from pynumaflow.function import Messages, Message, Datum, Server
+from typing import List
 
 
-def my_handler(key: str, datum: Datum) -> Messages:
+def my_handler(keys: List[str], datum: Datum) -> Messages:
     val = datum.value
     _ = datum.event_time
     _ = datum.watermark
-    messages = Messages(Message.to_vtx(key, val))
+    messages = Messages(Message(value=val, keys=keys))
     return messages
 
 
 if __name__ == "__main__":
-    grpc_server = UserDefinedFunctionServicer(map_handler=my_handler)
+    grpc_server = Server(map_handler=my_handler)
+    grpc_server.start()
+```
+### MapT - Map with event time assignment capability
+In addition to the regular Map function, MapT supports assigning a new event time to the message.
+MapT is only supported at source vertex to enable (a) early data filtering and (b) watermark assignment by extracting new event time from the message payload.
+
+```python
+import datetime
+from pynumaflow.function import MessageTs, MessageT, Datum, Server
+from typing import List
+
+
+def mapt_handler(keys: List[str], datum: Datum) -> MessageTs:
+    val = datum.value
+    new_event_time = datetime.time()
+    _ = datum.watermark
+    message_t_s = MessageTs(MessageT(new_event_time, val, keys))
+    return message_t_s
+
+
+if __name__ == "__main__":
+    grpc_server = Server(mapt_handler=mapt_handler)
     grpc_server.start()
 ```
 
 ### Reduce
 
 ```python
+import aiorun
 import asyncio
-from typing import Iterator
-from pynumaflow.function import Messages, Message, Datum, Metadata, UserDefinedFunctionServicer
+from typing import Iterator, List
+from pynumaflow.function import Messages, Message, Datum, Metadata, AsyncServer
 
 
-async def my_handler(key: str, datums: Iterator[Datum], md: Metadata) -> Messages:
+async def my_handler(keys: List[str], datums: Iterator[Datum], md: Metadata) -> Messages:
     interval_window = md.interval_window
     counter = 0
     async for _ in datums:
         counter += 1
     msg = (
         f"counter:{counter} interval_window_start:{interval_window.start} "
         f"interval_window_end:{interval_window.end}"
     )
-    return Messages(Message.to_vtx(key, str.encode(msg)))
+    return Messages(Message(str.encode(msg), keys))
 
 
 if __name__ == "__main__":
-    grpc_server = UserDefinedFunctionServicer(reduce_handler=my_handler)
-    asyncio.run(grpc_server.start())
-    asyncio.run(*grpc_server.cleanup_coroutines)
+    grpc_server = AsyncServer(reduce_handler=my_handler)
+    aiorun.run(grpc_server.start())
 ```
 
 ### Sample Image
 A sample UDF [Dockerfile](examples/function/forward_message/Dockerfile) is provided 
 under [examples](examples/function/forward_message).
 
 ## Implement a User Defined Sink (UDSink)
 
 ```python
 from typing import Iterator
-from pynumaflow.sink import Datum, Responses, Response, UserDefinedSinkServicer
+from pynumaflow.sink import Datum, Responses, Response, Sink
 
 
 def my_handler(datums: Iterator[Datum]) -> Responses:
     responses = Responses()
     for msg in datums:
         print("User Defined Sink", msg.value.decode("utf-8"))
         responses.append(Response.as_success(msg.id))
     return responses
 
 
 if __name__ == "__main__":
-    grpc_server = UserDefinedSinkServicer(my_handler)
+    grpc_server = Sink(my_handler)
     grpc_server.start()
 ```
 
 ### Sample Image
 
 A sample UDSink [Dockerfile](examples/sink/log/Dockerfile) is provided 
 under [examples](examples/sink/log).
 
+### Datum Metadata
+The Datum object contains the message payload and metadata. Currently, there are two fields
+in metadata: the message ID, the message delivery count to indicate how many times the message
+has been delivered. You can use these metadata to implement customized logic. For example,
+```python
+...
+def my_handler(keys: List[str], datum: Datum) -> Messages:
+    num_delivered = datum.metadata.num_delivered
+    # Choose to do specific actions, if the message delivery count reaches a certain threshold.
+    if num_delivered > 3:
+        ...
+```
```

