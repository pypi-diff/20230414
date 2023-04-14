# Comparing `tmp/pyraisdk_test-0.2.8.tar.gz` & `tmp/pyraisdk_test-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyraisdk_test-0.2.8.tar", max compression
+gzip compressed data, was "pyraisdk_test-0.2.9.tar", max compression
```

## Comparing `pyraisdk_test-0.2.8.tar` & `pyraisdk_test-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    10216 2023-04-06 12:20:41.627891 pyraisdk_test-0.2.8/README.md
--rw-r--r--   0        0        0      618 2023-04-11 13:27:16.954874 pyraisdk_test-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       42 2023-03-20 15:30:18.035839 pyraisdk_test-0.2.8/pyraisdk/__init__.py
--rw-r--r--   0        0        0      156 2023-03-20 15:30:18.035839 pyraisdk_test-0.2.8/pyraisdk/dynbatch/__init__.py
--rw-r--r--   0        0        0     1245 2023-04-06 12:20:41.627891 pyraisdk_test-0.2.8/pyraisdk/dynbatch/base.py
--rw-r--r--   0        0        0    15233 2023-04-06 12:20:41.627891 pyraisdk_test-0.2.8/pyraisdk/dynbatch/batch.py
--rw-r--r--   0        0        0     1349 2023-03-20 15:30:18.035839 pyraisdk_test-0.2.8/pyraisdk/dynbatch/config.py
--rw-r--r--   0        0        0     6222 2023-04-11 13:25:58.264897 pyraisdk_test-0.2.8/pyraisdk/rlog/__init__.py
--rw-r--r--   0        0        0     8187 2023-03-20 15:30:18.035839 pyraisdk_test-0.2.8/pyraisdk/rlog/eventhub.py
--rw-r--r--   0        0        0     3659 2023-04-11 11:23:00.566986 pyraisdk_test-0.2.8/pyraisdk/rlog/gputil.py
--rw-r--r--   0        0        0     6497 2023-03-20 15:30:18.035839 pyraisdk_test-0.2.8/pyraisdk/rlog/log.py
--rw-r--r--   0        0        0     8533 2023-04-11 13:27:06.804878 pyraisdk_test-0.2.8/pyraisdk/rlog/logimp.py
--rw-r--r--   0        0        0     5040 2023-04-07 15:46:02.234272 pyraisdk_test-0.2.8/pyraisdk/rlog/reporter.py
--rw-r--r--   0        0        0    11461 1970-01-01 00:00:00.000000 pyraisdk_test-0.2.8/setup.py
--rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 pyraisdk_test-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    10216 2023-04-06 12:20:41.627891 pyraisdk_test-0.2.9/README.md
+-rw-r--r--   0        0        0      618 2023-04-14 13:39:09.803411 pyraisdk_test-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-03-20 15:30:18.035839 pyraisdk_test-0.2.9/pyraisdk/__init__.py
+-rw-r--r--   0        0        0      156 2023-03-20 15:30:18.035839 pyraisdk_test-0.2.9/pyraisdk/dynbatch/__init__.py
+-rw-r--r--   0        0        0     1245 2023-04-06 12:20:41.627891 pyraisdk_test-0.2.9/pyraisdk/dynbatch/base.py
+-rw-r--r--   0        0        0    15233 2023-04-06 12:20:41.627891 pyraisdk_test-0.2.9/pyraisdk/dynbatch/batch.py
+-rw-r--r--   0        0        0     1349 2023-03-20 15:30:18.035839 pyraisdk_test-0.2.9/pyraisdk/dynbatch/config.py
+-rw-r--r--   0        0        0     6240 2023-04-14 12:49:00.234496 pyraisdk_test-0.2.9/pyraisdk/rlog/__init__.py
+-rw-r--r--   0        0        0     8187 2023-03-20 15:30:18.035839 pyraisdk_test-0.2.9/pyraisdk/rlog/eventhub.py
+-rw-r--r--   0        0        0     3659 2023-04-11 11:23:00.566986 pyraisdk_test-0.2.9/pyraisdk/rlog/gputil.py
+-rw-r--r--   0        0        0     6497 2023-03-20 15:30:18.035839 pyraisdk_test-0.2.9/pyraisdk/rlog/log.py
+-rw-r--r--   0        0        0     9451 2023-04-14 13:34:44.423508 pyraisdk_test-0.2.9/pyraisdk/rlog/logimp.py
+-rw-r--r--   0        0        0     5040 2023-04-07 15:46:02.234272 pyraisdk_test-0.2.9/pyraisdk/rlog/reporter.py
+-rw-r--r--   0        0        0    11461 1970-01-01 00:00:00.000000 pyraisdk_test-0.2.9/setup.py
+-rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 pyraisdk_test-0.2.9/PKG-INFO
```

### Comparing `pyraisdk_test-0.2.8/README.md` & `pyraisdk_test-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyraisdk_test-0.2.8/pyproject.toml` & `pyraisdk_test-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyraisdk-test"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["Xiaodong Yang <xiaoyan@microsoft.com>"]
 readme = "README.md"
 packages = [{include = "pyraisdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pyraisdk_test-0.2.8/pyraisdk/dynbatch/base.py` & `pyraisdk_test-0.2.9/pyraisdk/dynbatch/base.py`

 * *Files identical despite different names*

### Comparing `pyraisdk_test-0.2.8/pyraisdk/dynbatch/batch.py` & `pyraisdk_test-0.2.9/pyraisdk/dynbatch/batch.py`

 * *Files identical despite different names*

### Comparing `pyraisdk_test-0.2.8/pyraisdk/dynbatch/config.py` & `pyraisdk_test-0.2.9/pyraisdk/dynbatch/config.py`

 * *Files identical despite different names*

### Comparing `pyraisdk_test-0.2.8/pyraisdk/rlog/__init__.py` & `pyraisdk_test-0.2.9/pyraisdk/rlog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                 print('WARNING: logger eventhub sink is disabled')
         
             # stdout sink
             _logger.add_sink_structured(StdoutSink())
             _logger.add_sink_unstructured(StdoutSink())
 
             # start
-            _logger.start()
+            _logger.start(sys_metrics_enable)
 
             # system auto metrics
             #if sys_metrics_enable:
             #    _sys_metrics_reporter = SystemMetricsReporter(_logger, report_interval=60, measure_interval=5)
 
             # success
             _logger_initialized = True
```

### Comparing `pyraisdk_test-0.2.8/pyraisdk/rlog/eventhub.py` & `pyraisdk_test-0.2.9/pyraisdk/rlog/eventhub.py`

 * *Files identical despite different names*

### Comparing `pyraisdk_test-0.2.8/pyraisdk/rlog/gputil.py` & `pyraisdk_test-0.2.9/pyraisdk/rlog/gputil.py`

 * *Files identical despite different names*

### Comparing `pyraisdk_test-0.2.8/pyraisdk/rlog/log.py` & `pyraisdk_test-0.2.9/pyraisdk/rlog/log.py`

 * *Files identical despite different names*

### Comparing `pyraisdk_test-0.2.8/pyraisdk/rlog/logimp.py` & `pyraisdk_test-0.2.9/pyraisdk/rlog/logimp.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import sys
 import signal
 import threading
 import time
 import traceback
 
 from typing import List, Optional
-import psutil
 
+import psutil
 from pyraisdk.rlog.reporter import SystemMetricsReporter
 
-
 from .log import (
     LOGGING_QUEUE_CAPACITY,
     SINK_BATCH_MAX_IDLE_SECS,
     Event,
     EventLogger,
     EventSink,
     LogLevel,
@@ -31,18 +30,19 @@
     def __init__(self, role: str = '', instance: str=''):
         super(AsyncEventLogger, self).__init__()
         self.role = role 
         self.instance = instance
         self.unstruct_queue: mp.Queue[Event] = mp.Queue(maxsize=LOGGING_QUEUE_CAPACITY)
         self.struct_queue: mp.Queue[Event] = mp.Queue(maxsize=LOGGING_QUEUE_CAPACITY)
         self.backend_loop: Optional[_AsyncEventLoggerBackendLoop] = None
+        self.started: bool = False
     
     def log(self, level: LogLevel, msg: str, corr_id: str='', elem: int=-1):
         # check logger started
-        if self.backend_loop is None:
+        if not self.started:
             return
         evt = UnstructuredEvent(
                 level = level,
                 role = self.role,
                 instance = self.instance,
                 context = '',
                 message = msg,
@@ -53,15 +53,15 @@
             self.unstruct_queue.put_nowait(evt)
         except queue.Full:
             msg = f'{ERR_PREFIX} AsyncEventLogger shedding an event. Unstruct buffer grew faster than stream could be written.'
             print(msg, file=sys.stderr)
 
     def event(self, key: str, code: str, numeric: float, detail: str='', corr_id: str='', elem: int=-1):
         # check logger started
-        if self.backend_loop is None:
+        if not self.started:
             return
         evt = StructuredEvent(
             key = key,
             role = self.role,
             instance = self.instance,
             correlation_id = corr_id,
             element = elem,
@@ -71,27 +71,30 @@
         )
         try:
             self.struct_queue.put_nowait(evt)
         except queue.Full:
             msg = f'{ERR_PREFIX} AsyncEventLogger shedding an event. Struct buffer grew faster than stream could be written.'
             print(msg, file=sys.stderr)
 
-    def start(self):
+    def start(self, sys_metrics_enable: bool = False):
         with self.mutex:
             if self.backend_loop:
                 return
             self.backend_loop = _AsyncEventLoggerBackendLoop(
                 self.unstruct_queue,
                 self.unstruct_sinks,
                 self.struct_queue,
                 self.struct_sinks,
-                self,
+                sys_metrics_enable,
+                role=self.role,
+                instance=self.instance,
             )
             self.backend_loop.start()
-    
+            self.started = True
+
     def close(self):
         with self.mutex:
             if self.backend_loop is not None:
                 self.backend_loop.close()
 
     def __del__(self):
         self.close()
@@ -100,24 +103,31 @@
 class _AsyncEventLoggerBackendLoop:
     def __init__(
         self,
         unstruct_queue: mp.Queue,
         unstruct_sinks: List[EventSink],
         struct_queue: mp.Queue,
         struct_sinks: List[EventSink],
-        logger: AsyncEventLogger,
+        sys_metrics_enable: bool,
+        role: str, 
+        instance: str,
     ):
+        self.unstruct_queue = unstruct_queue
+        self.struct_queue = struct_queue
         self.categories_q: List[mp.Queue[Event]] = [unstruct_queue, struct_queue]
         self.categories_sinks: List[List[EventSink]] = [unstruct_sinks, struct_sinks]
         self.categories_sinks_ready: Optional[List[List[EventSink]]] = None
         self.terminated = mp.Event()
         self.mutex = mp.RLock()
         self.process: Optional[mp.Process] = None
         self.loop_threads: List[threading.Thread] = []
-        self.logger = logger
+        self.sys_metrics_enable = sys_metrics_enable
+        self.role = role
+        self.instance = instance
+        self._sys_metrics_reporter: Optional[SystemMetricsReporter] = None
         
     def start(self):
         with self.mutex:
             if self.process:
                 return
             self.process = mp.Process(target=self.main, daemon=True)
             self.process.start()
@@ -129,17 +139,22 @@
         p = psutil.Process()
         if psutil.LINUX:
             p.nice(10)
             p.ionice(psutil.IOPRIO_CLASS_IDLE)
         elif psutil.WINDOWS:
             p.nice(psutil.IDLE_PRIORITY_CLASS) # type: ignore
             p.ionice(psutil.IOPRIO_LOW) # type: ignore
-
+        
         # init reporter
-        self._sys_metrics_reporter = SystemMetricsReporter(self.logger, report_interval=60, measure_interval=5)
+        if self.sys_metrics_enable:
+            logger = AsyncEventLogger(self.role, self.instance)
+            logger.unstruct_queue = self.unstruct_queue
+            logger.struct_queue = self.struct_queue
+            logger.started = True
+            self._sys_metrics_reporter = SystemMetricsReporter(logger, report_interval=60, measure_interval=5)
         
         with self.mutex:
             # set quit signal
             signal.signal(signal.SIGINT, self.handle_signal)
             signal.signal(signal.SIGTERM, self.handle_signal)
             # start sinks
             self.categories_sinks_ready = [
@@ -150,14 +165,18 @@
                 t = threading.Thread(target=self.run_q, args=(q, sinks), daemon=True)
                 t.start()
                 self.loop_threads.append(t)
 
         for t in self.loop_threads:
             t.join()
         
+        # close reporter
+        if self._sys_metrics_reporter:
+            self._sys_metrics_reporter.close()
+        
         # close sinks at the end (not exit by handle_signal)
         for sinks in self.categories_sinks_ready:
             for sink in sinks:
                 sink.close()
 
     def _get_ready_sinks(self, sinks: List[EventSink]) -> List[EventSink]:
         result = []
@@ -217,14 +236,17 @@
                         msg = ERR_PREFIX + f' AsyncEventLogger failed to call sink of {type(sink)}.\n' + traceback.format_exc()
                         print(msg, file=sys.stderr)
 
             except queue.Empty:
                 break
 
     def handle_signal(self, signum, frame):
+        if self._sys_metrics_reporter:
+            self._sys_metrics_reporter.close()
+            
         with self.mutex:
             self.terminated.set()
             for q in self.categories_q:
                 try:
                     q.put_nowait(TerminateEvent())
                 except queue.Full:
                     pass
```

### Comparing `pyraisdk_test-0.2.8/pyraisdk/rlog/reporter.py` & `pyraisdk_test-0.2.9/pyraisdk/rlog/reporter.py`

 * *Files identical despite different names*

### Comparing `pyraisdk_test-0.2.8/setup.py` & `pyraisdk_test-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 entry_points = \
 {'console_scripts': ['publish_if_not_exists = '
                      'scripts.publish_if_not_exists:main']}
 
 setup_kwargs = {
     'name': 'pyraisdk-test',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': '',
     'long_description': '# pyraisdk\n\n## Overview\n\nAML models are meant to be deployed to GPU instances to provide inference service. If the code that operates the model uses the GPU for inferencing in each request separately,\nthe overall performance of the model will be quite inefficent. This SDK has APIs that can allocate batches of inference requests to run on the GPU in a separate thread, thereby considerably\nimproving the usage efficiency of GPU and making the model more performant. \n\nThe SDK also collects telemetry data for each so the performance of the model can be evaluated and tracked and provides logging primitives that can be used\nto produce additional troubleshooting information.\n\n\n## Using pyraisdk\n\n### Integrating with Model\nFollow the steps below to integrate pyraisdk.\n\n1. In environment configuration, list latest [pyraisdk version](https://github.com/microsoft/rai-orchestrator/blob/master/pyraisdk/pyproject.toml#L3) as a dependency.\n2. Import resources from pyraisdk\n  ```\n  from pyraisdk import rlog\n  from pyraisdk.dynbatch import BaseModel, DynamicBatchModel\n  ```\n3. Implement `BaseModel` class, which includes methods `preprocess()` and `predict()`, to define how data must be preprocessed and how inferences are made.\n4. At process start (e.g. in `init()` function if deploying with scoring script), initialize logging, instantiate object of class that implements `BaseModel`, and define global variable for batched model as shown below. \n  ```\n  rlog.initialize()\n  \n  global batched_model\n  malware_model = MalwareModel()\n  batched_model = DynamicBatchModel(malware_model)\n  ```\n5. In request handler (e.g. in `run()` function if deploying with scoring script), pass list of requests to the batched model\'s `predict()` method and return results. Under-the-hood, pyraisdk creates batches and uses your model\'s `preprocess()` and `predict()` methods to generate results.\n  ```\n  return batched_model.predict(json.loads(request_data)[\'data\'])\n  ```\n6. Optionally log additional structured and unstructured events using `EventLogger` [methods](https://github.com/microsoft/rai-orchestrator/blob/master/pyraisdk/pyraisdk/rlog/log.py). It is not necessary to log latency information, as pyraisdk does so automatically.\n\n### Configuring CD Pipeline\nIn addition to following the CD pipeline\'s [developer guidelines](https://github.com/microsoft/rai-orchestrator/blob/master/cicd/cd/regional/raicd/README.md#prerequisites-to-adding-or-modifying-endpoint-configurations) to onboard your model to RAI\'s deployment infrastructure, you must configure `BatchingConfig` for each deployment target to which your model will be deployed. To do so, \n1. Open the appropriate configuration file under `deployment-target-configs/../*.json`\n2. Configure the model\'s `Version`, `InstanceType` / SKU, and `BatchingConfig` as shown below\n  ```json\n  {\n\t  "Name": "MalwareNeural",\n\t  "Version": 19,\n      "InstanceType": "Standard_NC6s_v3",\n      "BatchingConfig": {\n          "MaxBatchSize": 12,\n          "IdleBatchSize": 5,\n          "MaxBatchInterval": 0.002\n      }\n  }\n  ```\nWhen the CD pipeline deploys the model to an AML online deployment, it exports environment variables for each `BatchingConfig` field, which pyraisdk utilizes at process start to configure batching parameters. The CD pipeline also exports environment variables to enable pyraisdk to log to RAI\'s Azure Data Explorer clusters.\n\n### Test or Deploy without RAI CD Pipeline\n\nTest or Deploy independetly outside of RAI CD Pipeline, it\'s required to set environment variables for `BatchingConfig` manually before object of `DynamicBatchModel` is created. Refer to [Batching Parameter](#batching-parameter-attention). \n\nThe recommended way to set these variables is calling `os.environ.setdefault` in `init()`. Like below:\n\n```python\ndef init():\n    os.environ.setdefault(\'PYRAISDK_MAX_BATCH_SIZE\', \'12\')\n    os.environ.setdefault(\'PYRAISDK_IDLE_BATCH_SIZE\', \'5\')\n    os.environ.setdefault(\'PYRAISDK_MAX_BATCH_INTERVAL\', \'0.002\')\n    ...\n    batch_model = DynamicBatchModel(malware_model)\n```\n\nThis should work well independent of RAI CD Pipeline. And you don\'t need to specifically remove these 3 lines when switching to deploy in CD Pipeline. \n\nBut please note that this kind of code should be **Avoided**: `os.environ[\'PYRAISDK_MAX_BATCH_SIZE\'] = \'12\'`. It will override the configuration from CD pipeline, which is not desirable in most cases.\n\nTo enable log publishing (to eventhub), there are another several environment variables need to be set, refer to following logging part. It\'s optional.\n\n\n## Dynamic Batching Support\n\nThere are APIs you **must** implement in your model to support batching of inference requests for best model performance. Those APIs allow the SDK\nto distribute load efficiently to the GPU instances. The APIs are:\n\n* ```preprocess``` Modifies the input to the model, if necessary. For example, if your model needs the input in a special JSON format instead of as a list\nof strings, you can do that modification in the *preprocess* method.\n* ```predict``` Executes the model inference for a list of input strings\n\n### Batching Parameter (**Attention**)\n\nBatching parameters are mandatory and should be ready before DynamicBatchModel is created. They are set through environment variables:\n- **PYRAISDK_MAX_BATCH_SIZE** (int): Max size of each processing batch.\n- **PYRAISDK_IDLE_BATCH_SIZE** (int): If there\'s no more data in queue, a new batch will be launched when size reaches this value.\n- **PYRAISDK_MAX_BATCH_INTERVAL** (float): Max interval in seconds to wait for items. When waiting time exceeds, will launch a batch immediately.\n\n\n### Usage Examples\n\nBuild `YourModel` class inherited from `pyraisdk.dynbatch.BaseModel`.\n\n```python\nfrom typing import List\nfrom pyraisdk.dynbatch import BaseModel\n\nclass YourModel(BaseModel):\n    def predict(self, items: List[str]) -> List[int]:\n        rs = []\n        for item in items:\n            rs.append(len(item))\n        return rs\n            \n    def preprocess(self, items: List[str]) -> List[str]:\n        rs = []\n        for item in items:\n            rs.append(f\'[{item}]\')\n        return rs\n```\n\nInitialize a `pyraisdk.dynbatch.DynamicBatchModel` with `YourModel` instance, and call `predict / predict_one` for inferencing.\n\n```python\nfrom pyraisdk.dynbatch import DynamicBatchModel\n\n# prepare model\nsimple_model = YourModel()\nbatch_model = DynamicBatchModel(simple_model)\n\n# predict\nitems = [\'abc\', \'123456\', \'xyzcccffaffaaa\']\npredictions = batch_model.predict(items)\nassert predictions == [5, 8, 16]\n\n# predict_one\nitem = \'abc\'\nprediction = batch_model.predict_one(item)\nassert prediction == 5\n```\n\nConcurrent requests to `predict / predict_one`, in different threads.\n\n```python\nfrom threading import Thread\nfrom pyraisdk.dynbatch import DynamicBatchModel\n\n# prepare model\nsimple_model = YourModel()\nbatch_model = DynamicBatchModel(simple_model)\n\n# thread run function\ndef run(name, num):\n    for step in range(num):\n        item = f\'{name}-{step}\'\n        prediction = batch_model.predict_one(item)\n        assert prediction == len(item) + 2\n\n# start concurrent inference\nthreads = [Thread(target=run, args=(f\'{tid}\', 100)) for tid in range(20)]\nfor t in threads:\n    t.start()\nfor t in threads:\n    t.join()\n```\n\n## Loging & Events\n\n### Description\nThis module is for logging and event tracing.\n\n### interface\n\n```python\ndef initialize(\n    eh_hostname: Optional[str] = None,\n    client_id: Optional[str] = None,\n    eh_conn_str: Optional[str] = None,\n    eh_structured: Optional[str] = None,\n    eh_unstructured: Optional[str] = None,\n    role: Optional[str] = None,\n    instance: Optional[str] = None,\n    sys_metrics_enable: bool = True,\n)\n```\n\nParameter description for `initialize`:\n- **eh_hostname**: Fully Qualified Namespace aka EH Endpoint URL (*.servicebus.windows.net). Default, read `${EVENTHUB_NAMESPACE}.servicebus.windows.net`\n- **client_id**: client_id of service principal. Default, read $UAI_CLIENT_ID\n- **eh_conn_str**: connection string of eventhub namespace. Default, read $EVENTHUB_CONN_STRING\n- **eh_structured**: structured eventhub name. Default, read $EVENTHUB_AUX_STRUCTURED\n- **eh_unstructured**: unstructured eventhub name. Default, read $EVENTHUB_AUX_UNSTRUCTURED\n- **role**: role, Default: `RemoteModel`\n- **instance**: instance, Default: `${MODEL_NAME}|${ENDPOINT_VERSION}|{hostname}` or `${MODEL_NAME}|${ENDPOINT_VERSION}|{_probably_unique_id()}`\n- **sys_metrics_enable**: Whether to enable auto metrics reporting periodically for system info like gpu, memory and gpu. Default: True\n\n```python\ndef event(self, key: str, code: str, numeric: float, detail: str=\'\', corr_id: str=\'\', elem: int=-1)\ndef infof(self, format: str, *args: Any)\ndef infocf(self, corr_id: str, elem: int, format: str, *args: Any)\ndef warnf(self, format: str, *args: Any)\ndef warncf(self, corr_id: str, elem: int, format: str, *args: Any)\ndef errorf(self, format: str, *args: Any)\ndef errorcf(self, corr_id: str, elem: int, ex: Optional[Exception], format: str, *args: Any)\ndef fatalf(self, format: str, *args: Any)\ndef fatalcf(self, corr_id: str, elem: int, ex: Optional[Exception], format: str, *args: Any)\n```\n\n### examples\n\n```python\n# export EVENTHUB_AUX_UNSTRUCTURED=\'ehunstruct\'\n# export EVENTHUB_AUX_STRUCTURED=\'ehstruct\'\n# export UAI_CLIENT_ID=\'xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx\'\n# export EVENTHUB_NAMESPACE=\'raieusdev-eh-namespace\'\n\nfrom pyraisdk import rlog\nrlog.initialize()\n\nrlog.infof(\'this is a info message %s\', 123)\nrlog.event(\'LifetimeEvent\', \'STOP_GRACEFUL_SIGNAL\', 0, \'detail info\')\n```\n\n```python\n# export EVENTHUB_AUX_UNSTRUCTURED=\'ehunstruct\'\n# export EVENTHUB_AUX_STRUCTURED=\'ehstruct\'\n# export EVENTHUB_CONN_STRING=\'<connection string>\'\n\nfrom pyraisdk import rlog\nrlog.initialize()\n\nrlog.infocf(\'corrid\', -1, \'this is a info message: %s\', 123)\nrlog.event(\'RequestDuration\', \'200\', 0.01, \'this is duration in seconds\')\n```\n\n```python\nfrom pyraisdk import rlog\nrlog.initialize(eh_structured=\'ehstruct\', eh_unstructured=\'ehunstruct\', eh_conn_str=\'<eventhub-conn-str>\')\n\nrlog.errorcf(\'corrid\', -1, Exception(\'error msg\'), \'error message: %s %s\', 1,2)\nrlog.event(\'CpuUsage\', \'\', 0.314, detail=\'cpu usage\', corr_id=\'corrid\', elem=-1)\n```\n',
     'author': 'Xiaodong Yang',
     'author_email': 'xiaoyan@microsoft.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pyraisdk_test-0.2.8/PKG-INFO` & `pyraisdk_test-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyraisdk-test
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: Xiaodong Yang
 Author-email: xiaoyan@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

