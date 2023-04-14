# Comparing `tmp/gentrace_py-0.2.1.tar.gz` & `tmp/gentrace_py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.2.1.tar", max compression
+gzip compressed data, was "gentrace_py-0.2.2.tar", max compression
```

## Comparing `gentrace_py-0.2.1.tar` & `gentrace_py-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      899 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5629 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     5308 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    32769 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32179 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-14 20:23:12.679993 gentrace_py-0.2.1/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      153 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/providers/__init__.py
--rw-r--r--   0        0        0      182 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    12206 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     2963 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     4606 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/providers/step_run.py
--rw-r--r--   0        0        0      171 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    10432 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/gentrace/schemas.py
--rw-r--r--   0        0        0     1298 2023-04-14 20:23:12.683993 gentrace_py-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      899 2023-04-14 20:27:38.270150 gentrace_py-0.2.2/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5629 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     5308 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    32769 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32179 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      153 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    12220 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     2963 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     4606 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0      201 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    10432 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/gentrace/schemas.py
+-rw-r--r--   0        0        0     1298 2023-04-14 20:27:38.274150 gentrace_py-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.2.2/PKG-INFO
```

### Comparing `gentrace_py-0.2.1/gentrace/__init__.py` & `gentrace_py-0.2.2/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/api_client.py` & `gentrace_py-0.2.2/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/configuration.py` & `gentrace_py-0.2.2/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/exceptions.py` & `gentrace_py-0.2.2/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/model/feedback_request.py` & `gentrace_py-0.2.2/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/model/feedback_request.pyi` & `gentrace_py-0.2.2/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/model/feedback_response.py` & `gentrace_py-0.2.2/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/model/feedback_response.pyi` & `gentrace_py-0.2.2/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.2.2/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.2.2/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.2.2/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.2.2/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/models/__init__.py` & `gentrace_py-0.2.2/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.2.2/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.2.2/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/providers/llms/openai.py` & `gentrace_py-0.2.2/gentrace/providers/llms/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,30 +57,30 @@
         )
     )
 
 
 def intercept_completion(original_fn):
     @classmethod
     def wrapper(cls, *args, **kwargs):
-        prompt_template = kwargs.get("promptTemplate")
-        prompt_inputs = kwargs.get("promptInputs")
+        prompt_template = kwargs.get("prompt_template")
+        prompt_inputs = kwargs.get("prompt_inputs")
         base_completion_options = {
             k: v
             for k, v in kwargs.items()
-            if k not in ["promptTemplate", "promptInputs"]
+            if k not in ["prompt_template", "prompt_inputs"]
         }
 
         if "prompt" in base_completion_options:
             raise ValueError(
-                "The prompt attribute cannot be provided when using the Gentrace SDK. Use promptTemplate and promptInputs instead."
+                "The prompt attribute cannot be provided when using the Gentrace SDK. Use prompt_template and prompt_inputs instead."
             )
 
         if not prompt_template:
             raise ValueError(
-                "The promptTemplate attribute must be provided when using the Gentrace SDK."
+                "The prompt_template attribute must be provided when using the Gentrace SDK."
             )
 
         rendered_prompt = pystache.render(prompt_template, prompt_inputs)
 
         new_completion_options = {**base_completion_options, "prompt": rendered_prompt}
 
         start_time = time.time()
@@ -99,31 +99,31 @@
 
     return wrapper
 
 
 def intercept_completion_async(original_fn):
     @classmethod
     async def wrapper(cls, *args, **kwargs):
-        prompt_template = kwargs.get("promptTemplate")
-        prompt_inputs = kwargs.get("promptInputs")
+        prompt_template = kwargs.get("prompt_template")
+        prompt_inputs = kwargs.get("prompt_inputs")
         stream = kwargs.get("stream")
         base_completion_options = {
             k: v
             for k, v in kwargs.items()
-            if k not in ["promptTemplate", "promptInputs"]
+            if k not in ["prompt_template", "prompt_inputs"]
         }
 
         if "prompt" in base_completion_options:
             raise ValueError(
-                "The prompt attribute cannot be provided when using the Gentrace SDK. Use promptTemplate and promptInputs instead."
+                "The prompt attribute cannot be provided when using the Gentrace SDK. Use prompt_template and prompt_inputs instead."
             )
 
         if not prompt_template:
             raise ValueError(
-                "The promptTemplate attribute must be provided when using the Gentrace SDK."
+                "The prompt_template attribute must be provided when using the Gentrace SDK."
             )
 
         if stream:
             rendered_prompt = pystache.render(prompt_template, prompt_inputs)
 
             new_completion_options = {
                 **base_completion_options,
```

### Comparing `gentrace_py-0.2.1/gentrace/providers/pipeline.py` & `gentrace_py-0.2.2/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/providers/pipeline_run.py` & `gentrace_py-0.2.2/gentrace/providers/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/providers/step_run.py` & `gentrace_py-0.2.2/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.2.2/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/rest.py` & `gentrace_py-0.2.2/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/gentrace/schemas.py` & `gentrace_py-0.2.2/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.2.1/pyproject.toml` & `gentrace_py-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.2.1"
+version = "0.2.2"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 pydantic = ">=1.10.2"
 pystache = "^0.6.0"
 python = ">=3.8.1,<4.0"
```

### Comparing `gentrace_py-0.2.1/PKG-INFO` & `gentrace_py-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

