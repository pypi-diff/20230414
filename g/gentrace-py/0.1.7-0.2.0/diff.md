# Comparing `tmp/gentrace_py-0.1.7.tar.gz` & `tmp/gentrace_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.1.7.tar", max compression
+gzip compressed data, was "gentrace_py-0.2.0.tar", max compression
```

## Comparing `gentrace_py-0.1.7.tar` & `gentrace_py-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      847 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5629 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     5308 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    32769 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32179 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      153 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/providers/__init__.py
--rw-r--r--   0        0        0      182 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0     5558 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     2963 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     3981 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/providers/step_run.py
--rw-r--r--   0        0        0      171 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    10432 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-14 13:55:48.893108 gentrace_py-0.1.7/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-14 13:55:48.897108 gentrace_py-0.1.7/gentrace/schemas.py
--rw-r--r--   0        0        0     1298 2023-04-14 13:55:48.897108 gentrace_py-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      847 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5629 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     5308 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    32769 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32179 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-14 17:11:44.831022 gentrace_py-0.2.0/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      153 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    12152 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     2963 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     4432 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0      171 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    10432 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/gentrace/schemas.py
+-rw-r--r--   0        0        0     1298 2023-04-14 17:11:44.835022 gentrace_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.2.0/PKG-INFO
```

### Comparing `gentrace_py-0.1.7/gentrace/__init__.py` & `gentrace_py-0.2.0/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/api_client.py` & `gentrace_py-0.2.0/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/configuration.py` & `gentrace_py-0.2.0/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/exceptions.py` & `gentrace_py-0.2.0/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/model/feedback_request.py` & `gentrace_py-0.2.0/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/model/feedback_request.pyi` & `gentrace_py-0.2.0/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/model/feedback_response.py` & `gentrace_py-0.2.0/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/model/feedback_response.pyi` & `gentrace_py-0.2.0/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.2.0/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.2.0/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.2.0/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.2.0/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/models/__init__.py` & `gentrace_py-0.2.0/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.2.0/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.2.0/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/providers/pipeline.py` & `gentrace_py-0.2.0/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/providers/pipeline_run.py` & `gentrace_py-0.2.0/gentrace/providers/pipeline_run.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,29 +21,39 @@
         if "openai" in self.pipeline.pipeline_handlers:
             handler = self.pipeline.pipeline_handlers.get("openai")
             cloned_handler = copy.deepcopy(handler)
             import openai
 
             from .llms.openai import (
                 intercept_chat_completion,
+                intercept_chat_completion_async,
                 intercept_completion,
+                intercept_completion_async,
                 intercept_embedding,
+                intercept_embedding_async,
             )
 
             for name, cls in vars(openai.api_resources).items():
                 if isinstance(cls, type):
                     # Create new class that inherits from the original class, don't directly monkey patch
                     # the original class
                     new_class = type(name, (cls,), {})
                     if name == "Completion":
                         new_class.create = intercept_completion(new_class.create)
+                        new_class.acreate = intercept_completion_async(
+                            new_class.acreate
+                        )
                     elif name == "ChatCompletion":
                         new_class.create = intercept_chat_completion(new_class.create)
+                        new_class.acreate = intercept_chat_completion_async(
+                            new_class.acreate
+                        )
                     elif name == "Embedding":
                         new_class.create = intercept_embedding(new_class.create)
+                        new_class.acreate = intercept_embedding_async(new_class.acreate)
 
                     new_class.pipeline_run = self
 
                     setattr(cloned_handler, name, new_class)
                     # TODO: must work on a acreate() method, check that streaming works
 
             cloned_handler.set_pipeline_run(self)
@@ -90,16 +100,14 @@
                 "elapsedTime": step_run.elapsed_time,
                 "startTime": step_run.start_time,
                 "endTime": step_run.end_time,
             }
             for step_run in self.step_runs
         ]
 
-        print("Step run: ", json.dumps(step_runs_data, indent=2))
-
         pipeline_post_response = ingestion_api.pipeline_run_post(
             {"name": self.pipeline.id, "stepRuns": step_runs_data}
         )
 
         return {
             "pipelineRunId": pipeline_post_response.body.get_item_oapg("pipelineRunId")
         }
```

### Comparing `gentrace_py-0.1.7/gentrace/providers/step_run.py` & `gentrace_py-0.2.0/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.2.0/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/rest.py` & `gentrace_py-0.2.0/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/gentrace/schemas.py` & `gentrace_py-0.2.0/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.7/pyproject.toml` & `gentrace_py-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.1.7"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 pydantic = ">=1.10.2"
 pystache = "^0.6.0"
 python = ">=3.8.1,<4.0"
```

### Comparing `gentrace_py-0.1.7/PKG-INFO` & `gentrace_py-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.1.7
+Version: 0.2.0
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

