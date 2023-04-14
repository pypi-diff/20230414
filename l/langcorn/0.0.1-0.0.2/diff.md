# Comparing `tmp/langcorn-0.0.1.tar.gz` & `tmp/langcorn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcorn-0.0.1.tar", max compression
+gzip compressed data, was "langcorn-0.0.2.tar", max compression
```

## Comparing `langcorn-0.0.1.tar` & `langcorn-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     2576 2023-04-14 16:52:32.643729 langcorn-0.0.1/Readme.md
--rw-r--r--   0        0        0      380 2023-04-14 16:52:32.643729 langcorn-0.0.1/langcorn/__main__.py
--rw-r--r--   0        0        0      945 2023-04-14 16:52:32.647729 langcorn-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 16:52:32.647729 langcorn-0.0.1/server/__init__.py
--rw-r--r--   0        0        0     1149 2023-04-14 16:52:32.647729 langcorn-0.0.1/server/api.py
--rw-r--r--   0        0        0      949 2023-04-14 16:52:32.647729 langcorn-0.0.1/server/test_api.py
--rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 langcorn-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2576 2023-04-14 16:57:08.257402 langcorn-0.0.2/Readme.md
+-rw-r--r--   0        0        0       47 2023-04-14 16:57:08.257402 langcorn-0.0.2/langcorn/__init__.py
+-rw-r--r--   0        0        0      389 2023-04-14 16:57:08.257402 langcorn-0.0.2/langcorn/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:57:08.257402 langcorn-0.0.2/langcorn/server/__init__.py
+-rw-r--r--   0        0        0     1149 2023-04-14 16:57:08.257402 langcorn-0.0.2/langcorn/server/api.py
+-rw-r--r--   0        0        0      943 2023-04-14 16:57:08.257402 langcorn-0.0.2/langcorn/server/test_api.py
+-rw-r--r--   0        0        0      923 2023-04-14 16:57:08.257402 langcorn-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 langcorn-0.0.2/PKG-INFO
```

### Comparing `langcorn-0.0.1/Readme.md` & `langcorn-0.0.2/Readme.md`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.1/pyproject.toml` & `langcorn-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "langcorn"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Python package creating rest api interface for LangChain"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = [
     "Alexander Miasoiedov <msoedov@gmail.com>",
 ]
 repository = "https://github.com/msoedov/langcorn"
 license = "MIT"
 readme = "Readme.md"
 keywords = ["nlp", "langchain", "openai", "gpt", "fastapi"]
 packages = [{ include = "langcorn", from = "." }]
-include = ["server*"]
 
 
 [tool.poetry.scripts]
 langcorn = "langcorn.__main__:entrypoint"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `langcorn-0.0.1/server/api.py` & `langcorn-0.0.2/langcorn/server/api.py`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.1/server/test_api.py` & `langcorn-0.0.2/langcorn/server/test_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pytest
 from fastapi.testclient import TestClient
 from loguru import logger
 
 # from mirakuru import AlreadyRunning, TCPExecutor
 
-from server.api import create_service
+from .api import create_service
 
 
 FN_PORT = 7172
 
 
 client = TestClient(create_service("examples.ex1:chain"))
```

### Comparing `langcorn-0.0.1/PKG-INFO` & `langcorn-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langcorn
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package creating rest api interface for LangChain
 Home-page: https://github.com/msoedov/langcorn
 License: MIT
 Keywords: nlp,langchain,openai,gpt,fastapi
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
```

