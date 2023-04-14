# Comparing `tmp/scaleway_functions_python-0.1.0.tar.gz` & `tmp/scaleway_functions_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway_functions_python-0.1.0.tar", max compression
+gzip compressed data, was "scaleway_functions_python-0.1.1.tar", max compression
```

## Comparing `scaleway_functions_python-0.1.0.tar` & `scaleway_functions_python-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      363 2023-03-02 17:28:58.287711 scaleway_functions_python-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2023-03-02 17:28:58.287711 scaleway_functions_python-0.1.0/LICENSE
--rw-r--r--   0        0        0     4488 2023-03-02 17:28:58.287711 scaleway_functions_python-0.1.0/README.md
--rw-r--r--   0        0        0     2291 2023-03-02 17:28:58.291711 scaleway_functions_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      119 2023-03-02 17:28:58.291711 scaleway_functions_python-0.1.0/scaleway_functions_python/__init__.py
--rw-r--r--   0        0        0       23 2023-03-02 17:28:58.291711 scaleway_functions_python-0.1.0/scaleway_functions_python/framework/__init__.py
--rw-r--r--   0        0        0       29 2023-03-02 17:28:58.291711 scaleway_functions_python-0.1.0/scaleway_functions_python/framework/v1/__init__.py
--rw-r--r--   0        0        0     1370 2023-03-02 17:28:58.291711 scaleway_functions_python-0.1.0/scaleway_functions_python/framework/v1/hints.py
--rw-r--r--   0        0        0       52 2023-03-02 17:28:58.291711 scaleway_functions_python-0.1.0/scaleway_functions_python/local/__init__.py
--rw-r--r--   0        0        0      341 2023-03-02 17:28:58.291711 scaleway_functions_python-0.1.0/scaleway_functions_python/local/context.py
--rw-r--r--   0        0        0     1421 2023-03-02 17:28:58.291711 scaleway_functions_python-0.1.0/scaleway_functions_python/local/event.py
--rw-r--r--   0        0        0     1281 2023-03-02 17:28:58.291711 scaleway_functions_python-0.1.0/scaleway_functions_python/local/infra.py
--rw-r--r--   0        0        0     6104 2023-03-02 17:28:58.291711 scaleway_functions_python-0.1.0/scaleway_functions_python/local/serving.py
--rw-r--r--   0        0        0     5815 1970-01-01 00:00:00.000000 scaleway_functions_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      510 2023-04-14 13:11:30.987608 scaleway_functions_python-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2023-04-14 13:11:30.987608 scaleway_functions_python-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4976 2023-04-14 13:11:30.987608 scaleway_functions_python-0.1.1/README.md
+-rw-r--r--   0        0        0     2298 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/framework/__init__.py
+-rw-r--r--   0        0        0       29 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/framework/v1/__init__.py
+-rw-r--r--   0        0        0     1370 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/framework/v1/hints.py
+-rw-r--r--   0        0        0       52 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/local/__init__.py
+-rw-r--r--   0        0        0      341 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/local/context.py
+-rw-r--r--   0        0        0     1421 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/local/event.py
+-rw-r--r--   0        0        0     1263 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/local/infra.py
+-rw-r--r--   0        0        0     6104 2023-04-14 13:11:30.991608 scaleway_functions_python-0.1.1/scaleway_functions_python/local/serving.py
+-rw-r--r--   0        0        0     6302 1970-01-01 00:00:00.000000 scaleway_functions_python-0.1.1/PKG-INFO
```

### Comparing `scaleway_functions_python-0.1.0/LICENSE` & `scaleway_functions_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scaleway_functions_python-0.1.0/README.md` & `scaleway_functions_python-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Serverless Functions Python 💜
 
+[![PyPI version](https://badge.fury.io/py/scaleway-functions-python.svg)](https://badge.fury.io/py/scaleway-functions-python)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-functions-python/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-functions-python/main)
+![pre-commit.ci status](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11-blue.svg)
+
 Scaleway Serverless Functions Python is a framework that simplifies Scaleway [Serverless Functions](https://www.scaleway.com/fr/serverless-functions/) local development.
 It enables you to debug your function locally and provide the event data format used in Scaleway Serverless Functions.
 
 This library helps you to write functions but for deployment please refer to the documentation.
 
 Get started with Scaleway Functions:
 
@@ -11,14 +15,15 @@
 - [Scaleway Serverless Framework plugin](https://github.com/scaleway/serverless-scaleway-functions)
 - [Scaleway Serverless Examples](https://github.com/scaleway/serverless-examples)
 - [Scaleway Cloud Provider](https://scaleway.com)
 
 Testing frameworks for Scaleway Serverless Functions in other languages can be found here:
 
 - [Go](https://github.com/scaleway/serverless-functions-go)
+- [Node](https://github.com/scaleway/serverless-functions-node)
 
 ## ⚙️ Quickstart
 
 You can use `pip` to install the framework:
 
 ```console
 pip install scaleway-functions-python
```

### Comparing `scaleway_functions_python-0.1.0/pyproject.toml` & `scaleway_functions_python-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "scaleway-functions-python"
-version = "0.1.0"
+version = "0.1.1"
 description = "Utilities for testing your Python handlers for Scaleway Serverless Functions."
 authors = ["Scaleway Serverless Team <opensource@scaleway.com>"]
 
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/scaleway/serverless-functions-python"
 
 keywords = ["serverless", "scaleway", "functions", "cloud", "faas"]
 
 # Should be one of:
 # "Development Status :: 3 - Alpha"
 # "Development Status :: 4 - Beta"
 # "Development Status :: 5 - Production/Stable"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Internet",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
@@ -35,15 +35,15 @@
 typing-extensions = { version = "^4.4.0", python = "<3.11" }
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
-autoflake = "^1.7.7"
+autoflake = ">=1.7.7,<3.0.0"
 black = "^23.01.0"
 flake8 = "^6.0.0"
 isort = "^5.10.1"
 pre-commit = "^3.0.4"
 pylint = "^2.16.2"
 pylint-per-file-ignores = "^1.2.0"
```

### Comparing `scaleway_functions_python-0.1.0/scaleway_functions_python/framework/v1/hints.py` & `scaleway_functions_python-0.1.1/scaleway_functions_python/framework/v1/hints.py`

 * *Files identical despite different names*

### Comparing `scaleway_functions_python-0.1.0/scaleway_functions_python/local/event.py` & `scaleway_functions_python-0.1.1/scaleway_functions_python/local/event.py`

 * *Files identical despite different names*

### Comparing `scaleway_functions_python-0.1.0/scaleway_functions_python/local/infra.py` & `scaleway_functions_python-0.1.1/scaleway_functions_python/local/infra.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         it's simpler to inject them into the event object directly.
     """
     if not request.remote_addr:
         raise RuntimeWarning("remote_addr is not set in the request")
     headers = {
         "Forwarded": f"for={request.remote_addr};proto=http",
         "X-Forwarded-For": request.remote_addr,
-        "X-Envoy-External-Adrdress": request.remote_addr,
+        "K-Proxy-Request": "activator",
         "X-Forwarded-Proto": "http",
         # In this context "X-Forwared-For" == "X-Envoy-External-Address"
         # this property doesn't hold for actual functions
         "X-Envoy-External-Address": request.remote_addr,
         "X-Request-Id": str(uuid.uuid4()),
     }
     # Not using |= to keep compatibility with python 3.8
```

### Comparing `scaleway_functions_python-0.1.0/scaleway_functions_python/local/serving.py` & `scaleway_functions_python-0.1.1/scaleway_functions_python/local/serving.py`

 * *Files identical despite different names*

### Comparing `scaleway_functions_python-0.1.0/PKG-INFO` & `scaleway_functions_python-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: scaleway-functions-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utilities for testing your Python handlers for Scaleway Serverless Functions.
 Home-page: https://github.com/scaleway/serverless-functions-python
 License: MIT
 Keywords: serverless,scaleway,functions,cloud,faas
 Author: Scaleway Serverless Team
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8.1,<3.12
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,14 +25,18 @@
 Requires-Dist: flask (>=2.2.2,<3.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/scaleway/serverless-functions-python
 Description-Content-Type: text/markdown
 
 # Serverless Functions Python 💜
 
+[![PyPI version](https://badge.fury.io/py/scaleway-functions-python.svg)](https://badge.fury.io/py/scaleway-functions-python)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scaleway/serverless-functions-python/main.svg)](https://results.pre-commit.ci/latest/github/scaleway/serverless-functions-python/main)
+![pre-commit.ci status](https://img.shields.io/badge/python-3.8_|_3.9_|_3.10_|_3.11-blue.svg)
+
 Scaleway Serverless Functions Python is a framework that simplifies Scaleway [Serverless Functions](https://www.scaleway.com/fr/serverless-functions/) local development.
 It enables you to debug your function locally and provide the event data format used in Scaleway Serverless Functions.
 
 This library helps you to write functions but for deployment please refer to the documentation.
 
 Get started with Scaleway Functions:
 
@@ -40,14 +44,15 @@
 - [Scaleway Serverless Framework plugin](https://github.com/scaleway/serverless-scaleway-functions)
 - [Scaleway Serverless Examples](https://github.com/scaleway/serverless-examples)
 - [Scaleway Cloud Provider](https://scaleway.com)
 
 Testing frameworks for Scaleway Serverless Functions in other languages can be found here:
 
 - [Go](https://github.com/scaleway/serverless-functions-go)
+- [Node](https://github.com/scaleway/serverless-functions-node)
 
 ## ⚙️ Quickstart
 
 You can use `pip` to install the framework:
 
 ```console
 pip install scaleway-functions-python
```

