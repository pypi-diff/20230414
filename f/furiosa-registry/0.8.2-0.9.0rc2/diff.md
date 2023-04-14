# Comparing `tmp/furiosa-registry-0.8.2.tar.gz` & `tmp/furiosa-registry-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-registry-0.8.2.tar", last modified: Wed Nov  9 06:14:45 2022, max compression
+gzip compressed data, was "furiosa-registry-0.9.0rc2.tar", last modified: Fri Apr 14 20:48:38 2023, max compression
```

## Comparing `furiosa-registry-0.8.2.tar` & `furiosa-registry-0.9.0rc2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      353 2022-07-09 17:15:10.784990 furiosa-registry-0.8.2/Makefile
--rw-r--r--   0        0        0     1623 2022-07-09 17:15:10.784990 furiosa-registry-0.8.2/README.md
--rw-r--r--   0        0        0      223 2022-10-26 21:05:59.737773 furiosa-registry-0.8.2/furiosa/registry/__init__.py
--rw-r--r--   0        0        0     2600 2022-07-09 17:15:10.784990 furiosa-registry-0.8.2/furiosa/registry/client/__init__.py
--rw-r--r--   0        0        0     2986 2022-05-12 03:15:52.457378 furiosa-registry-0.8.2/furiosa/registry/client/transport/__init__.py
--rw-r--r--   0        0        0     2059 2022-11-03 20:35:29.971030 furiosa-registry-0.8.2/furiosa/registry/client/transport/base.py
--rw-r--r--   0        0        0     1543 2022-07-09 17:15:10.784990 furiosa-registry-0.8.2/furiosa/registry/client/transport/file.py
--rw-r--r--   0        0        0     2720 2022-11-03 20:35:29.971030 furiosa-registry-0.8.2/furiosa/registry/client/transport/github.py
--rw-r--r--   0        0        0     1569 2022-03-23 02:46:22.111317 furiosa-registry-0.8.2/furiosa/registry/client/transport/http.py
--rw-r--r--   0        0        0     1293 2022-03-23 02:46:22.111317 furiosa-registry-0.8.2/furiosa/registry/client/transport/s3.py
--rw-r--r--   0        0        0      535 2022-03-23 02:46:22.111317 furiosa-registry-0.8.2/furiosa/registry/errors.py
--rw-r--r--   0        0        0       30 2022-11-04 01:37:43.613344 furiosa-registry-0.8.2/furiosa/registry/git_version.txt
--rw-r--r--   0        0        0     2464 2022-11-09 03:34:52.827700 furiosa-registry-0.8.2/furiosa/registry/model.py
--rw-r--r--   0        0        0        0 2022-03-23 02:46:22.111317 furiosa-registry-0.8.2/furiosa/registry/py.typed
--rw-r--r--   0        0        0     1926 2022-11-03 20:35:29.971030 furiosa-registry-0.8.2/furiosa/registry/utils.py
--rw-r--r--   0        0        0     3158 2022-09-23 14:58:27.130844 furiosa-registry-0.8.2/model_schema.json
--rw-r--r--   0        0        0     2565 2022-11-09 06:13:28.290252 furiosa-registry-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      454 2022-05-04 06:07:47.315119 furiosa-registry-0.8.2/tests/unit/conftest.py
--rw-r--r--   0        0        0      883 2022-10-12 21:24:46.943088 furiosa-registry-0.8.2/tests/unit/fixtures/artifacts.py
--rw-r--r--   0        0        0    16154 2022-10-12 21:24:46.943088 furiosa-registry-0.8.2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.dfg
--rw-r--r--   0        0        0   172884 2022-10-12 21:24:46.943088 furiosa-registry-0.8.2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.enf
--rw-r--r--   0        0        0    18136 2022-05-04 06:07:47.315119 furiosa-registry-0.8.2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.tflite
--rw-r--r--   0        0        0      927 2022-11-03 20:35:29.971030 furiosa-registry-0.8.2/tests/unit/test_file_transport.py
--rw-r--r--   0        0        0     1623 2022-11-03 20:35:29.971030 furiosa-registry-0.8.2/tests/unit/test_http_transport.py
--rw-r--r--   0        0        0     1182 2022-05-04 06:07:47.315119 furiosa-registry-0.8.2/tests/unit/test_s3_transport.py
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 furiosa-registry-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/Makefile
+-rw-r--r--   0        0        0     1623 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/README.md
+-rw-r--r--   0        0        0      223 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/__init__.py
+-rw-r--r--   0        0        0     2600 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/client/__init__.py
+-rw-r--r--   0        0        0     2986 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/__init__.py
+-rw-r--r--   0        0        0     2059 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/base.py
+-rw-r--r--   0        0        0     1543 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/file.py
+-rw-r--r--   0        0        0     2720 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/github.py
+-rw-r--r--   0        0        0     1569 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/http.py
+-rw-r--r--   0        0        0     1293 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/s3.py
+-rw-r--r--   0        0        0      535 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/errors.py
+-rw-r--r--   0        0        0       17 2023-04-14 20:43:51.884589 furiosa-registry-0.9.0rc2/furiosa/registry/git_version.txt
+-rw-r--r--   0        0        0     2464 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/model.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/py.typed
+-rw-r--r--   0        0        0     1926 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/furiosa/registry/utils.py
+-rw-r--r--   0        0        0     3158 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/model_schema.json
+-rw-r--r--   0        0        0     2571 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      454 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/tests/unit/conftest.py
+-rw-r--r--   0        0        0      883 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/tests/unit/fixtures/artifacts.py
+-rw-r--r--   0        0        0    16154 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.dfg
+-rw-r--r--   0        0        0   172884 2023-04-14 20:42:32.777315 furiosa-registry-0.9.0rc2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.enf
+-rw-r--r--   0        0        0    18136 2023-04-14 20:42:32.781315 furiosa-registry-0.9.0rc2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.tflite
+-rw-r--r--   0        0        0      927 2023-04-14 20:42:32.781315 furiosa-registry-0.9.0rc2/tests/unit/test_file_transport.py
+-rw-r--r--   0        0        0     1623 2023-04-14 20:42:32.781315 furiosa-registry-0.9.0rc2/tests/unit/test_http_transport.py
+-rw-r--r--   0        0        0     1182 2023-04-14 20:42:32.781315 furiosa-registry-0.9.0rc2/tests/unit/test_s3_transport.py
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 furiosa-registry-0.9.0rc2/PKG-INFO
```

### Comparing `furiosa-registry-0.8.2/README.md` & `furiosa-registry-0.9.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/furiosa/registry/client/__init__.py` & `furiosa-registry-0.9.0rc2/furiosa/registry/client/__init__.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/furiosa/registry/client/transport/__init__.py` & `furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/furiosa/registry/client/transport/base.py` & `furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/base.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/furiosa/registry/client/transport/file.py` & `furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/file.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/furiosa/registry/client/transport/github.py` & `furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/github.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/furiosa/registry/client/transport/http.py` & `furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/http.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/furiosa/registry/client/transport/s3.py` & `furiosa-registry-0.9.0rc2/furiosa/registry/client/transport/s3.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/furiosa/registry/errors.py` & `furiosa-registry-0.9.0rc2/furiosa/registry/errors.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/furiosa/registry/model.py` & `furiosa-registry-0.9.0rc2/furiosa/registry/model.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/furiosa/registry/utils.py` & `furiosa-registry-0.9.0rc2/furiosa/registry/utils.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/model_schema.json` & `furiosa-registry-0.9.0rc2/model_schema.json`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/pyproject.toml` & `furiosa-registry-0.9.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-registry"
-version = "0.8.2"
+version = "0.9.0.rc2"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dynamic = ["description"]
-requires-python = "~=3.7"
+requires-python = "~=3.8"
 dependencies = [
     "PyYAML",
     "aiofiles",
     "aiohttp ~= 3.8.3",
     "multipledispatch",
     "pydantic",
     "toml",
@@ -54,15 +54,15 @@
 
 [tool.flit.module]
 name = "furiosa.registry"
 
 [tool.black]
 skip-string-normalization = true
 line-length = 100
-target-version = ["py37", "py38", "py39"]
+target-version = ["py38", "py39", "py310"]
 extend-exclude = "/generated/"
 
 [tool.isort]
 force_sort_within_sections = true
 known_first_party = ["furiosa"]
 line_length = 100
 profile = "black"
```

### Comparing `furiosa-registry-0.8.2/tests/unit/fixtures/artifacts.py` & `furiosa-registry-0.9.0rc2/tests/unit/fixtures/artifacts.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.dfg` & `furiosa-registry-0.9.0rc2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.dfg`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.enf` & `furiosa-registry-0.9.0rc2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.enf`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.tflite` & `furiosa-registry-0.9.0rc2/tests/unit/fixtures/models/MNISTnet_uint8_quant_without_softmax.tflite`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/tests/unit/test_file_transport.py` & `furiosa-registry-0.9.0rc2/tests/unit/test_file_transport.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/tests/unit/test_http_transport.py` & `furiosa-registry-0.9.0rc2/tests/unit/test_http_transport.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/tests/unit/test_s3_transport.py` & `furiosa-registry-0.9.0rc2/tests/unit/test_s3_transport.py`

 * *Files identical despite different names*

### Comparing `furiosa-registry-0.8.2/PKG-INFO` & `furiosa-registry-0.9.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: furiosa-registry
-Version: 0.8.2
+Version: 0.9.0rc2
 Summary: FuriosaAI model registry
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: PyYAML
 Requires-Dist: aiofiles
 Requires-Dist: aiohttp ~= 3.8.3
 Requires-Dist: multipledispatch
 Requires-Dist: pydantic
```

