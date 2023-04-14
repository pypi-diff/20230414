# Comparing `tmp/warpzone_sdk-5.0.2.tar.gz` & `tmp/warpzone_sdk-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-5.0.2.tar", max compression
+gzip compressed data, was "warpzone_sdk-6.0.0.tar", max compression
```

## Comparing `warpzone_sdk-5.0.2.tar` & `warpzone_sdk-6.0.0.tar`

### file list

```diff
@@ -1,26 +1,36 @@
--rw-r--r--   0        0        0     1121 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/pyproject.toml
--rw-r--r--   0        0        0     1050 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2877 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      187 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/function/__init__.py
--rw-r--r--   0        0        0     2606 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2108 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0      117 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     2496 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/monitor/function.py
--rw-r--r--   0        0        0     1650 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5373 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       47 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/tablestorage/__init__.py
--rw-r--r--   0        0        0     2882 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/tablestorage/client.py
--rw-r--r--   0        0        0     2509 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/tablestorage/client_async.py
--rw-r--r--   0        0        0      521 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/tablestorage/helpers.py
--rw-r--r--   0        0        0     2446 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/tablestorage/operations.py
--rw-r--r--   0        0        0       19 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-04-04 09:57:07.806916 warpzone_sdk-5.0.2/warpzone/transform/data.py
--rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1185 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2877 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       27 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     1501 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     2606 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     1482 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/function/process.py
+-rw-r--r--   0        0        0       32 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1157 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/function/signature.py
+-rw-r--r--   0        0        0       80 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5433 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       47 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/tablestorage/__init__.py
+-rw-r--r--   0        0        0     2882 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/tablestorage/client.py
+-rw-r--r--   0        0        0     2509 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/tablestorage/client_async.py
+-rw-r--r--   0        0        0      521 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/tablestorage/helpers.py
+-rw-r--r--   0        0        0     2446 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/tablestorage/operations.py
+-rw-r--r--   0        0        0      176 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-14 13:37:53.973062 warpzone_sdk-6.0.0/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3499 2023-04-14 13:37:53.977062 warpzone_sdk-6.0.0/warpzone/testing/data.py
+-rw-r--r--   0        0        0       19 2023-04-14 13:37:53.977062 warpzone_sdk-6.0.0/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-04-14 13:37:53.977062 warpzone_sdk-6.0.0/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 warpzone_sdk-6.0.0/PKG-INFO
```

### Comparing `warpzone_sdk-5.0.2/pyproject.toml` & `warpzone_sdk-6.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "5.0.2"
+version = "6.0.0"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Anders Launer Baek-Petersen <alp@energinet.dk>", "Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `warpzone_sdk-5.0.2/warpzone/__init__.py` & `warpzone_sdk-6.0.0/warpzone/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from warpzone import healthchecks
+from warpzone import healthchecks, testing
 from warpzone.blobstorage.client import BlobData, WarpzoneStorageClient
 from warpzone.enums.topicenum import Topic
+from warpzone.function.functionize import functionize
 from warpzone.function.integrations import (
     func_msg_to_data,
     func_msg_to_event,
     func_msg_to_pandas,
     get_data_client,
     get_event_client,
+    get_table_client,
     get_table_client_async,
     read_pandas,
     send_data,
     send_event,
     send_pandas,
 )
+from warpzone.function.processors import outputs, triggers
 from warpzone.healthchecks import HealthCheckResult, HealthStatus
-from warpzone.monitor import get_logger, get_tracer, monitor
+from warpzone.monitor import get_logger, get_tracer
 from warpzone.servicebus.data.client import DataMessage, WarpzoneDataClient
 from warpzone.servicebus.events.client import EventMessage, WarpzoneEventClient
 from warpzone.tablestorage.client import WarpzoneTableClient
 from warpzone.tablestorage.client_async import WarpzoneTableClientAsync
 from warpzone.tablestorage.operations import TableOperations
 from warpzone.transform.data import (
     arrow_to_pandas,
```

### Comparing `warpzone_sdk-5.0.2/warpzone/blobstorage/client.py` & `warpzone_sdk-6.0.0/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/function/integrations.py` & `warpzone_sdk-6.0.0/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/healthchecks/__init__.py` & `warpzone_sdk-6.0.0/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/healthchecks/model.py` & `warpzone_sdk-6.0.0/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/monitor/function.py` & `warpzone_sdk-6.0.0/warpzone/function/monitor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import asyncio
 import logging
 from contextlib import contextmanager
-from functools import wraps
 from typing import Callable
 
-from . import logs, traces
+import azure.functions as func
+
+from warpzone.function.types import SingleArgumentCallable
+from warpzone.monitor import logs, traces
 
-MESSAGE_PARAM_NAME = "msg"
 SUBJECT_IDENTIFIER = "<Subject>"
 
 tracer = traces.get_tracer(__name__)
 logger = logs.get_logger(__name__)
 
 
 def configure_monitoring():
     """
     Configure logging and tracing on Azure Function to
     - export telemetry to App Insights
-    - supress spamming logs
+    - suppress spamming logs
     """
     # disable logging for HTTP calls to avoid log spamming
     logging.getLogger("azure.core.pipeline.policies.http_logging_policy").setLevel(
         logging.WARNING
     )
 
     # disable logging for Service Bus underlying uAMQP library to avoid log spamming
@@ -31,68 +32,50 @@
     traces.configure_tracing()
 
     # configure logger provider
     logs.configure_logging()
 
 
 @contextmanager
-def setup_monitoring(kwargs):
-    try:
-        context = kwargs["context"]
-    except KeyError:
-        raise KeyError(
-            "Azure Function must contain argument named `context` to use monitoring"
-        )
-
+def run_in_trace_context(context: func.Context):
     configure_monitoring()
 
     trace_context = context.trace_context
     with traces.set_trace_context(
         trace_context.trace_parent, trace_context.trace_state
     ):
         yield
 
 
-def monitor(main: Callable):
-    """Wrapper for running Azure Function
-    with telemetry settings for exporting
-    to App Insights.
+def monitor(main: SingleArgumentCallable) -> Callable:
+    """Wrap Azure function with logging and tracing
+    configured for monitoring in App Insights.
 
     Args:
-        main (Callable): Azure Function main function
+        f (SingleArgumentCallable): Azure function to be wrapped
+
+    Returns:
+        Callable: Azure function with
+            - argument
+                name: "arg"
+                description: argument of the original function
+            - argument
+                name: "context"
+                description: Azure function context
+            - return value
+                description: return value of original function
     """
 
-    # The `wraps` decorator ensures the resulting function has the same signature
-    # as the original one, to avoid errors form the Azure Function worker.
-    @wraps(main)
-    async def wrapper_async(*args, **kwargs):
-        with setup_monitoring(kwargs):
-            pre_function(kwargs)
-            result = await main(*args, **kwargs)
-            post_function(kwargs)
+    async def wrapper_async(arg, context: func.Context):
+        with run_in_trace_context(context):
+            result = await main(arg)
             return result
 
-    @wraps(main)
-    def wrapper(*args, **kwargs):
-        with setup_monitoring(kwargs):
-            pre_function(kwargs)
-            result = main(*args, **kwargs)
-            post_function(kwargs)
+    def wrapper(arg, context: func.Context):
+        with run_in_trace_context(context):
+            result = main(arg)
             return result
 
     if asyncio.iscoroutinefunction(main):
         return wrapper_async
     else:
         return wrapper
-
-
-def pre_function(kwargs):
-    if MESSAGE_PARAM_NAME in kwargs:
-        log_subject(kwargs[MESSAGE_PARAM_NAME].label)
-
-
-def post_function(kwargs):
-    pass
-
-
-def log_subject(subject):
-    logger.info(f"{SUBJECT_IDENTIFIER}{subject}")
```

### Comparing `warpzone_sdk-5.0.2/warpzone/monitor/logs.py` & `warpzone_sdk-6.0.0/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/monitor/traces.py` & `warpzone_sdk-6.0.0/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/servicebus/data/client.py` & `warpzone_sdk-6.0.0/warpzone/servicebus/data/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,18 +37,19 @@
     def from_pandas(
         cls,
         df: pd.DataFrame,
         subject: str,
         schema: dict = None,
         message_id: str = None,
         metadata: dict = None,
+        timestamp: Optional[dt.datetime] = None,
     ):
         content = data.pandas_to_parquet(df, schema=schema)
         extension = "parquet"
-        return cls(content, extension, subject, message_id, metadata)
+        return cls(content, extension, subject, message_id, metadata, timestamp)
 
     def to_pandas(self) -> pd.DataFrame:
         return data.parquet_to_pandas(self.content)
 
 
 class WarpzoneDataClient:
     """
```

### Comparing `warpzone_sdk-5.0.2/warpzone/servicebus/events/client.py` & `warpzone_sdk-6.0.0/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/tablestorage/client.py` & `warpzone_sdk-6.0.0/warpzone/tablestorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/tablestorage/client_async.py` & `warpzone_sdk-6.0.0/warpzone/tablestorage/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/tablestorage/helpers.py` & `warpzone_sdk-6.0.0/warpzone/tablestorage/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/tablestorage/operations.py` & `warpzone_sdk-6.0.0/warpzone/tablestorage/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/warpzone/transform/data.py` & `warpzone_sdk-6.0.0/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-5.0.2/PKG-INFO` & `warpzone_sdk-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 5.0.2
+Version: 6.0.0
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Anders Launer Baek-Petersen
 Author-email: alp@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

