# Comparing `tmp/finetuner-0.7.4.tar.gz` & `tmp/finetuner-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetuner-0.7.4.tar", last modified: Wed Mar 29 08:26:01 2023, max compression
+gzip compressed data, was "finetuner-0.7.5.tar", last modified: Fri Apr 14 07:39:18 2023, max compression
```

## Comparing `finetuner-0.7.4.tar` & `finetuner-0.7.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:26:01.500404 finetuner-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-03-29 08:25:42.000000 finetuner-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-29 08:25:42.000000 finetuner-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-03-29 08:26:01.500404 finetuner-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-03-29 08:25:42.000000 finetuner-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:26:01.500404 finetuner-0.7.4/finetuner/
--rw-r--r--   0 runner    (1001) docker     (123)    23499 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:26:01.500404 finetuner-0.7.4/finetuner/client/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/excepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/finetuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/hubble.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-03-29 08:25:42.000000 finetuner-0.7.4/finetuner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:26:01.500404 finetuner-0.7.4/finetuner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-03-29 08:26:00.000000 finetuner-0.7.4/finetuner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-29 08:26:01.000000 finetuner-0.7.4/finetuner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:26:00.000000 finetuner-0.7.4/finetuner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:26:00.000000 finetuner-0.7.4/finetuner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-29 08:26:00.000000 finetuner-0.7.4/finetuner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-29 08:26:00.000000 finetuner-0.7.4/finetuner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-29 08:25:42.000000 finetuner-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-29 08:26:01.500404 finetuner-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-03-29 08:25:42.000000 finetuner-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:39:18.047494 finetuner-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-04-14 07:39:08.000000 finetuner-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 07:39:08.000000 finetuner-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-04-14 07:39:18.047494 finetuner-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-14 07:39:08.000000 finetuner-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:39:18.043494 finetuner-0.7.5/finetuner/
+-rw-r--r--   0 runner    (1001) docker     (123)    23608 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:39:18.047494 finetuner-0.7.5/finetuner/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/excepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/finetuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/hubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-04-14 07:39:08.000000 finetuner-0.7.5/finetuner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:39:18.043494 finetuner-0.7.5/finetuner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 07:39:17.000000 finetuner-0.7.5/finetuner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 07:39:08.000000 finetuner-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 07:39:18.047494 finetuner-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-14 07:39:08.000000 finetuner-0.7.5/setup.py
```

### Comparing `finetuner-0.7.4/LICENSE` & `finetuner-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.4/PKG-INFO` & `finetuner-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.7.4
+Version: 0.7.5
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
@@ -212,14 +212,15 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: full
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.7.4 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.7.5 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
 
@@ -91,12 +91,13 @@
 engineers and solution engineers to build the next generation of open-source AI
 ecosystems.  Keywords: jina neural-search neural-network deep-learning
 pretraining fine-tuning pretrained-models triplet-loss metric-learning siamese-
 network few-shot-learning Platform: UNKNOWN Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: License :: OSI Approved ::
-Apache Software License Classifier: Environment :: Console Classifier:
-Operating System :: OS Independent Classifier: Topic :: Scientific/Engineering
-:: Artificial Intelligence Requires-Python: >=3.8.0 Description-Content-Type:
-text/markdown Provides-Extra: full Provides-Extra: test
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Environment :: Console Classifier: Operating System :: OS
+Independent Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
+Provides-Extra: full Provides-Extra: test
```

### Comparing `finetuner-0.7.4/README.md` & `finetuner-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.4/finetuner/__init__.py` & `finetuner-0.7.5/finetuner/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,29 +423,30 @@
         :class:`ONNXINferenceEngine`.
     """
     import torch
     from _finetuner.models.inference import (
         ONNXRuntimeInferenceEngine,
         TorchInferenceEngine,
     )
-    from _finetuner.runner.model import RunnerModel
+    from _finetuner.runner.model import EmbeddingModel
 
     if not device:
         device = 'cuda' if torch.cuda.is_available() else 'cpu'
 
     stub = model_stub.get_stub(
         name, select_model=select_model, model_options=model_options or {}
     )
 
-    model = RunnerModel(stub=stub)
+    model = EmbeddingModel(stub=stub, download_pretrained=True)
     if not is_onnx:
         return TorchInferenceEngine(
             artifact=model,
             batch_size=batch_size,
             device=device,
+            download_pretrained=True,
         )
     else:
         return ONNXRuntimeInferenceEngine(
             artifact=model,
             batch_size=batch_size,
             device=device,
         )
@@ -515,14 +516,15 @@
         inference_engine = TorchInferenceEngine(
             artifact=artifact,
             token=token,
             batch_size=batch_size,
             select_model=select_model,
             device=device,
             logging_level=logging_level,
+            download_pretrained=False,
         )
     return inference_engine
 
 
 def encode(
     model: 'InferenceEngine',
     data: Union[DocumentArray, List[str]],
```

### Comparing `finetuner-0.7.4/finetuner/client/base.py` & `finetuner-0.7.5/finetuner/client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     def _handle_request(
         self,
         url: str,
         method: str,
         params: Optional[dict] = None,
         json_data: Optional[dict] = None,
         stream: bool = False,
+        timeout: Optional[int] = None,
     ) -> Union[dict, List[dict], str, requests.Response]:
         """The base request handler.
 
         :param url: The url of the request.
         :param method: The request type (GET, POST or DELETE).
         :param params: Optional parameters for the request.
         :param json_data: Optional data payloads to be sent along with the request.
@@ -68,14 +69,15 @@
         response = self._session.request(
             url=url,
             method=method,
             json=json_data,
             params=params,
             allow_redirects=True,
             stream=stream,
+            timeout=timeout,
         )
         if not response.ok:
             raise FinetunerServerError(
                 message=response.reason,
                 code=response.status_code,
                 details=response.json()['detail'],
             )
```

### Comparing `finetuner-0.7.4/finetuner/client/client.py` & `finetuner-0.7.5/finetuner/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, Iterator, List, Optional
 
 import pkg_resources
+from requests.exceptions import ReadTimeout
 
 from finetuner.client.base import _BaseClient
 from finetuner.constants import (
     API_VERSION,
     CONFIG,
     CPUS,
     DELETE,
@@ -164,15 +165,21 @@
             API_VERSION,
             EXPERIMENTS,
             experiment_name,
             RUNS,
             run_name,
             STATUS,
         )
-        return self._handle_request(url=url, method=GET)
+
+        try:
+            response = self._handle_request(url=url, method=GET, timeout=10)
+        # In the event that the request times out, attempt the request one more time.
+        except ReadTimeout:
+            response = self._handle_request(url=url, method=GET, timeout=10)
+        return response
 
     def get_run_logs(self, experiment_name: str, run_name: str) -> str:
         """Get a run logs by its name and experiment.
 
         :param experiment_name: The name of the experiment.
         :param run_name: The name of the run.
         :return: Run logs.
```

### Comparing `finetuner-0.7.4/finetuner/client/session.py` & `finetuner-0.7.5/finetuner/client/session.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.4/finetuner/console.py` & `finetuner-0.7.5/finetuner/console.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.4/finetuner/constants.py` & `finetuner-0.7.5/finetuner/constants.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.4/finetuner/data.py` & `finetuner-0.7.5/finetuner/data.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.4/finetuner/experiment.py` & `finetuner-0.7.5/finetuner/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         )
         if query_data or index_data:
             eval_callback.query_data = query_data
             eval_callback.index_data = index_data
 
         kwargs[EVAL_DATA] = eval_data
 
-        config = self._create_config_for_run(
+        config = self._create_finetuning_config(
             model=model,
             train_data=train_data,
             experiment_name=self._name,
             run_name=run_name,
             **kwargs,
         )
 
@@ -205,15 +205,15 @@
             config=run[CONFIG],
             created_at=run[CREATED_AT],
             description=run[DESCRIPTION],
         )
         return run
 
     @staticmethod
-    def _create_config_for_run(
+    def _create_finetuning_config(
         model: str,
         train_data: str,
         experiment_name: str,
         run_name: str,
         **kwargs,
     ) -> Dict[str, Any]:
         """Create config for a :class:`Run`.
@@ -283,18 +283,18 @@
         if kwargs.get(SCHEDULER_OPTIONS):
             hyper_parameters.scheduler_options = kwargs.get(SCHEDULER_OPTIONS)
         if kwargs.get(LOSS_OPTIMIZER):
             hyper_parameters.loss_optimizer = kwargs.get(LOSS_OPTIMIZER)
         if kwargs.get(LOSS_OPTIMIZER_OPTIONS):
             hyper_parameters.loss_optimizer_options = kwargs.get(LOSS_OPTIMIZER_OPTIONS)
 
-        run_config = config.RunConfig(
+        finetuning_config = config.FinetuningConfig(
             model=model,
             data=data,
             callbacks=callbacks,
             hyper_parameters=hyper_parameters,
             public=public,
             experiment_name=experiment_name,
             run_name=run_name,
         )
 
-        return run_config.dict()
+        return finetuning_config.dict()
```

### Comparing `finetuner-0.7.4/finetuner/finetuner.py` & `finetuner-0.7.5/finetuner/finetuner.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,14 +181,21 @@
 
         :return: A `Run` object.
         """
         if not experiment_name:
             experiment = self._default_experiment
         else:
             experiment = self.get_experiment(name=experiment_name)
+        if not experiment:
+            raise ValueError(
+                (
+                    'Unable to start finetuning run as experiment is `None`. '
+                    'Make sure you have logged in using `finetuner.login(force=True)`.'
+                )
+            )
         return experiment.create_run(
             model=model,
             train_data=train_data,
             eval_data=eval_data,
             val_split=val_split,
             model_artifact=model_artifact,
             run_name=run_name,
```

### Comparing `finetuner-0.7.4/finetuner/hubble.py` & `finetuner-0.7.5/finetuner/hubble.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.4/finetuner/model.py` & `finetuner-0.7.5/finetuner/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from _finetuner.runner.stubs import model
 from _finetuner.runner.stubs.model import *  # noqa F401
+from _finetuner.runner.stubs.model import _EmbeddingModelStub
 
 
 def get_header() -> Tuple[str, ...]:
     """Get table header."""
     return 'name', 'task', 'output_dim', 'architecture', 'description'
 
 
@@ -18,10 +19,15 @@
     )
 
 
 def list_model_classes() -> Dict[str, ModelStubType]:
     rv = {}
     members = inspect.getmembers(model, inspect.isclass)
     for name, stub in members:
-        if name != 'MLPStub' and not name.startswith('_') and type(stub) != type:
+        if (
+            name != 'MLPStub'
+            and not name.startswith('_')
+            and type(stub) != type
+            and issubclass(stub, _EmbeddingModelStub)
+        ):
             rv[name] = stub
     return rv
```

### Comparing `finetuner-0.7.4/finetuner/names.py` & `finetuner-0.7.5/finetuner/names.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.4/finetuner/run.py` & `finetuner-0.7.5/finetuner/run.py`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.4/finetuner.egg-info/PKG-INFO` & `finetuner-0.7.5/finetuner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuner
-Version: 0.7.4
+Version: 0.7.5
 Summary: Task-oriented finetuning for better embeddings on neural search.
 Home-page: https://github.com/jina-ai/finetuner/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai
@@ -212,14 +212,15 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: full
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: finetuner Version: 0.7.4 Summary: Task-oriented
+Metadata-Version: 2.1 Name: finetuner Version: 0.7.5 Summary: Task-oriented
 finetuning for better embeddings on neural search. Home-page: https://
 github.com/jina-ai/finetuner/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/finetuner/tags
 Project-URL: Documentation, https://finetuner.jina.ai Project-URL: Source,
 https://github.com/jina-ai/finetuner/ Project-URL: Tracker, https://github.com/
 jina-ai/finetuner/issues Description:
 
@@ -91,12 +91,13 @@
 engineers and solution engineers to build the next generation of open-source AI
 ecosystems.  Keywords: jina neural-search neural-network deep-learning
 pretraining fine-tuning pretrained-models triplet-loss metric-learning siamese-
 network few-shot-learning Platform: UNKNOWN Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: License :: OSI Approved ::
-Apache Software License Classifier: Environment :: Console Classifier:
-Operating System :: OS Independent Classifier: Topic :: Scientific/Engineering
-:: Artificial Intelligence Requires-Python: >=3.8.0 Description-Content-Type:
-text/markdown Provides-Extra: full Provides-Extra: test
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Environment :: Console Classifier: Operating System :: OS
+Independent Classifier: Topic :: Scientific/Engineering :: Artificial
+Intelligence Requires-Python: >=3.8.0 Description-Content-Type: text/markdown
+Provides-Extra: full Provides-Extra: test
```

### Comparing `finetuner-0.7.4/finetuner.egg-info/SOURCES.txt` & `finetuner-0.7.5/finetuner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finetuner-0.7.4/setup.py` & `finetuner-0.7.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,20 +25,20 @@
         long_description=_long_description,
         long_description_content_type='text/markdown',
         zip_safe=False,
         setup_requires=['setuptools>=18.0', 'wheel'],
         install_requires=[
             'docarray[common]>=0.21.0',
             'trimesh==3.16.4',
-            'finetuner-stubs==0.13.0',
+            'finetuner-stubs==0.13.3',
             'jina-hubble-sdk==0.33.1',
         ],
         extras_require={
             'full': [
-                'finetuner-commons==0.13.0',
+                'finetuner-commons==0.13.3',
             ],
             'test': [
                 'black==22.3.0',
                 'flake8==5.0.4',
                 'isort==5.10.1',
                 'pytest==7.0.0',
                 'pytest-cov==3.0.0',
@@ -49,14 +49,15 @@
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Intended Audience :: Developers',
             'Intended Audience :: Education',
             'Intended Audience :: Science/Research',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
             'License :: OSI Approved :: Apache Software License',
             'Environment :: Console',
             'Operating System :: OS Independent',
             'Topic :: Scientific/Engineering :: Artificial Intelligence',
         ],
         project_urls={
             'Documentation': 'https://finetuner.jina.ai',
```

