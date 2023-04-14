# Comparing `tmp/gentrace_py-0.1.5.tar.gz` & `tmp/gentrace_py-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.1.5.tar", max compression
+gzip compressed data, was "gentrace_py-0.1.6.tar", max compression
```

## Comparing `gentrace_py-0.1.5.tar` & `gentrace_py-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      847 2023-04-12 21:46:37.940295 gentrace_py-0.1.5/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-04-12 21:46:37.940295 gentrace_py-0.1.5/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-04-12 21:46:37.940295 gentrace_py-0.1.5/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5629 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     5308 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    32769 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32179 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      153 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/providers/__init__.py
--rw-r--r--   0        0        0      182 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0     5558 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     2963 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     3764 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/providers/step_run.py
--rw-r--r--   0        0        0      171 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    10432 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-04-12 21:46:37.944295 gentrace_py-0.1.5/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-04-12 21:46:37.948295 gentrace_py-0.1.5/gentrace/schemas.py
--rw-r--r--   0        0        0     1322 2023-04-12 21:46:37.948295 gentrace_py-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      847 2023-04-14 10:38:20.267137 gentrace_py-0.1.6/gentrace/__init__.py
+-rw-r--r--   0        0        0    59420 2023-04-14 10:38:20.267137 gentrace_py-0.1.6/gentrace/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-14 10:38:20.267137 gentrace_py-0.1.6/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-14 10:38:20.267137 gentrace_py-0.1.6/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-14 10:38:20.267137 gentrace_py-0.1.6/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-14 10:38:20.267137 gentrace_py-0.1.6/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0      459 2023-04-14 10:38:20.267137 gentrace_py-0.1.6/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      335 2023-04-14 10:38:20.267137 gentrace_py-0.1.6/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/apis/tags/ingestion_api.py
+-rw-r--r--   0        0        0    15476 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/configuration.py
+-rw-r--r--   0        0        0     4444 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     5629 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     5308 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2144 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2121 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    32769 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    32179 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2779 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2739 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0      640 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12578 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12355 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      153 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0     5558 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     2963 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     3764 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0      171 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    10432 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10398 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/rest.py
+-rw-r--r--   0        0        0   103185 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/gentrace/schemas.py
+-rw-r--r--   0        0        0     1322 2023-04-14 10:38:20.271137 gentrace_py-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.1.6/PKG-INFO
```

### Comparing `gentrace_py-0.1.5/gentrace/__init__.py` & `gentrace_py-0.1.6/gentrace/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/api_client.py` & `gentrace_py-0.1.6/gentrace/api_client.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/configuration.py` & `gentrace_py-0.1.6/gentrace/configuration.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/exceptions.py` & `gentrace_py-0.1.6/gentrace/exceptions.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/model/feedback_request.py` & `gentrace_py-0.1.6/gentrace/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/model/feedback_request.pyi` & `gentrace_py-0.1.6/gentrace/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/model/feedback_response.py` & `gentrace_py-0.1.6/gentrace/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/model/feedback_response.pyi` & `gentrace_py-0.1.6/gentrace/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.1.6/gentrace/model/pipeline_run_request.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/model/pipeline_run_request.pyi` & `gentrace_py-0.1.6/gentrace/model/pipeline_run_request.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.1.6/gentrace/model/pipeline_run_response.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.1.6/gentrace/model/pipeline_run_response.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/models/__init__.py` & `gentrace_py-0.1.6/gentrace/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.1.6/gentrace/paths/pipeline_run/post.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.1.6/gentrace/paths/pipeline_run/post.pyi`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/providers/llms/openai.py` & `gentrace_py-0.1.6/gentrace/providers/llms/openai.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/providers/pipeline.py` & `gentrace_py-0.1.6/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/providers/pipeline_run.py` & `gentrace_py-0.1.6/gentrace/providers/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/providers/step_run.py` & `gentrace_py-0.1.6/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.1.6/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/rest.py` & `gentrace_py-0.1.6/gentrace/rest.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/gentrace/schemas.py` & `gentrace_py-0.1.6/gentrace/schemas.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.1.5/pyproject.toml` & `gentrace_py-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 pydantic = ">=1.10.2"
 python = ">=3.8.1,<4.0"
 python_dateutil = ">=2.5.3"
 setuptools = ">=21.0.0"
```

### Comparing `gentrace_py-0.1.5/PKG-INFO` & `gentrace_py-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

