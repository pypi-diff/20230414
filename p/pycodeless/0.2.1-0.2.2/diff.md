# Comparing `tmp/pycodeless-0.2.1.tar.gz` & `tmp/pycodeless-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodeless-0.2.1.tar", max compression
+gzip compressed data, was "pycodeless-0.2.2.tar", max compression
```

## Comparing `pycodeless-0.2.1.tar` & `pycodeless-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.1/LICENSE
--rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.1/pycodeless/__init__.py
--rw-r--r--   0        0        0      665 2023-04-13 22:50:33.299322 pycodeless-0.2.1/pycodeless/_api.py
--rw-r--r--   0        0        0     5142 2023-04-14 11:57:05.819090 pycodeless-0.2.1/pycodeless/_generate.py
--rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.1/pycodeless/_llm.py
--rw-r--r--   0        0        0      436 2023-04-13 22:40:30.195789 pycodeless-0.2.1/pycodeless/_load.py
--rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.1/pycodeless/_openai_llm.py
--rw-r--r--   0        0        0     4491 2023-04-14 11:38:36.064128 pycodeless-0.2.1/pycodeless/_parse.py
--rw-r--r--   0        0        0      391 2023-04-14 14:09:57.862401 pycodeless-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1777 2023-04-14 13:39:10.384582 pycodeless-0.2.1/README.md
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 pycodeless-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.2/LICENSE
+-rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.2/pycodeless/__init__.py
+-rw-r--r--   0        0        0      829 2023-04-14 20:16:01.148962 pycodeless-0.2.2/pycodeless/_api.py
+-rw-r--r--   0        0        0     5142 2023-04-14 11:57:05.819090 pycodeless-0.2.2/pycodeless/_generate.py
+-rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.2/pycodeless/_llm.py
+-rw-r--r--   0        0        0      436 2023-04-13 22:40:30.195789 pycodeless-0.2.2/pycodeless/_load.py
+-rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.2/pycodeless/_openai_llm.py
+-rw-r--r--   0        0        0     4518 2023-04-14 20:15:27.918408 pycodeless-0.2.2/pycodeless/_parse.py
+-rw-r--r--   0        0        0      391 2023-04-14 20:08:17.397947 pycodeless-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3855 2023-04-14 20:30:07.129969 pycodeless-0.2.2/README.md
+-rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 pycodeless-0.2.2/PKG-INFO
```

### Comparing `pycodeless-0.2.1/LICENSE` & `pycodeless-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.1/pycodeless/_api.py` & `pycodeless-0.2.2/pycodeless/_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,22 +5,30 @@
 from ._generate import generate
 from ._load import load_module
 from ._openai_llm import OpenAiLanguageModel
 
 
 def codeless(function: Callable) -> Callable:
     if not codeless.openai_api_key:
-        raise RuntimeError
+        raise RuntimeError("OpenAI API key was not set")
+
+    llm = OpenAiLanguageModel(
+        codeless.openai_api_key,
+        codeless.openai_model_name
+    )
 
-    llm = OpenAiLanguageModel(codeless.openai_api_key, "gpt-3.5-turbo")
     result = generate(llm, function)
 
     def wrapper(*args, **kwargs):
         module = load_module(*result)
         callable = getattr(module, function.__name__)
 
         return callable(*args, **kwargs)
 
     return wrapper
 
 
 codeless.openai_api_key: Optional[str] = os.getenv("OPENAI_API_KEY")
+codeless.openai_model_name: str = os.getenv(
+    "OPENAI_MODEL_NAME",
+    "gpt-3.5-turbo"
+)
```

### Comparing `pycodeless-0.2.1/pycodeless/_generate.py` & `pycodeless-0.2.2/pycodeless/_generate.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.1/pycodeless/_llm.py` & `pycodeless-0.2.2/pycodeless/_llm.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.1/pycodeless/_openai_llm.py` & `pycodeless-0.2.2/pycodeless/_openai_llm.py`

 * *Files identical despite different names*

### Comparing `pycodeless-0.2.1/pycodeless/_parse.py` & `pycodeless-0.2.2/pycodeless/_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,10 +166,10 @@
 
         if is_last_line:
             break
 
         line_index += 1
 
     if not isinstance(state, _ModuleSeekingState):
-        raise RuntimeError
+        raise RuntimeError("Unexpected parser state")
 
     return Module(module_source, docstring, functions)
```

