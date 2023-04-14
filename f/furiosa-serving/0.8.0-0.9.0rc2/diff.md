# Comparing `tmp/furiosa-serving-0.8.0.tar.gz` & `tmp/furiosa-serving-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-serving-0.8.0.tar", last modified: Sat Nov  5 00:14:37 2022, max compression
+gzip compressed data, was "furiosa-serving-0.9.0rc2.tar", last modified: Fri Apr 14 20:49:33 2023, max compression
```

## Comparing `furiosa-serving-0.8.0.tar` & `furiosa-serving-0.9.0rc2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0        0 2022-11-05 00:10:12.314211 furiosa-serving-0.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      378 2022-11-05 00:10:12.314211 furiosa-serving-0.8.0/Makefile
--rw-r--r--   0        0        0    11731 2022-11-05 00:10:12.314211 furiosa-serving-0.8.0/README.md
--rw-r--r--   0        0        0     2636 2022-11-05 00:10:12.314211 furiosa-serving-0.8.0/examples/assets/images/1234567890.jpg
--rw-r--r--   0        0        0     1286 2022-11-05 00:10:12.314211 furiosa-serving-0.8.0/examples/assets/images/6254.jpg
--rw-r--r--   0        0        0    92833 2022-11-05 00:10:12.314211 furiosa-serving-0.8.0/examples/assets/images/car.jpg
--rw-r--r--   0        0        0    10484 2022-11-05 00:10:12.314211 furiosa-serving-0.8.0/examples/assets/labels/ImageNetLabels.txt
--rw-r--r--   0        0        0    18136 2022-11-05 00:10:12.314211 furiosa-serving-0.8.0/examples/assets/models/MNISTnet_uint8_quant_without_softmax.tflite
--rw-r--r--   0        0        0  4275408 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/examples/assets/models/image_classification.onnx
--rw-r--r--   0        0        0     1042 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/examples/image_classify.py
--rw-r--r--   0        0        0     2842 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/examples/number_classify.py
--rw-r--r--   0        0        0      346 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/__init__.py
--rw-r--r--   0        0        0     5960 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/application.py
--rw-r--r--   0        0        0        0 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/apps/__init__.py
--rw-r--r--   0        0        0      539 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/apps/health.py
--rw-r--r--   0        0        0     1088 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/apps/model.py
--rw-r--r--   0        0        0     1018 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/apps/repository.py
--rw-r--r--   0        0        0       14 2022-11-05 00:12:28.110437 furiosa-serving-0.8.0/furiosa/serving/git_version.txt
--rw-r--r--   0        0        0     8908 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/model.py
--rw-r--r--   0        0        0       96 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/processors/__init__.py
--rw-r--r--   0        0        0     2962 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/processors/base.py
--rw-r--r--   0        0        0     2349 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/processors/imagenet.py
--rw-r--r--   0        0        0        0 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/py.typed
--rw-r--r--   0        0        0     6388 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/furiosa/serving/telemetry.py
--rw-r--r--   0        0        0     2875 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      692 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/tests/test_load_models.py
--rw-r--r--   0        0        0     1087 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/tests/test_processors.py
--rw-r--r--   0        0        0      582 2022-11-05 00:10:12.342211 furiosa-serving-0.8.0/tests/test_subapp.py
--rw-r--r--   0        0        0    13484 1970-01-01 00:00:00.000000 furiosa-serving-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 20:42:32.869314 furiosa-serving-0.9.0rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      378 2023-04-14 20:42:32.869314 furiosa-serving-0.9.0rc2/Makefile
+-rw-r--r--   0        0        0    11731 2023-04-14 20:42:32.869314 furiosa-serving-0.9.0rc2/README.md
+-rw-r--r--   0        0        0     2636 2023-04-14 20:42:32.869314 furiosa-serving-0.9.0rc2/examples/assets/images/1234567890.jpg
+-rw-r--r--   0        0        0     1286 2023-04-14 20:42:32.869314 furiosa-serving-0.9.0rc2/examples/assets/images/6254.jpg
+-rw-r--r--   0        0        0    92833 2023-04-14 20:42:32.869314 furiosa-serving-0.9.0rc2/examples/assets/images/car.jpg
+-rw-r--r--   0        0        0    10484 2023-04-14 20:42:32.869314 furiosa-serving-0.9.0rc2/examples/assets/labels/ImageNetLabels.txt
+-rw-r--r--   0        0        0    18136 2023-04-14 20:42:32.869314 furiosa-serving-0.9.0rc2/examples/assets/models/MNISTnet_uint8_quant_without_softmax.tflite
+-rw-r--r--   0        0        0  4275408 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/examples/assets/models/image_classification.onnx
+-rw-r--r--   0        0        0     1042 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/examples/image_classify.py
+-rw-r--r--   0        0        0     2842 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/examples/number_classify.py
+-rw-r--r--   0        0        0      346 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/__init__.py
+-rw-r--r--   0        0        0     5960 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/application.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/apps/__init__.py
+-rw-r--r--   0        0        0      539 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/apps/health.py
+-rw-r--r--   0        0        0     1088 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/apps/model.py
+-rw-r--r--   0        0        0     1018 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/apps/repository.py
+-rw-r--r--   0        0        0       17 2023-04-14 20:44:42.888140 furiosa-serving-0.9.0rc2/furiosa/serving/git_version.txt
+-rw-r--r--   0        0        0     8907 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/model.py
+-rw-r--r--   0        0        0       96 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/processors/__init__.py
+-rw-r--r--   0        0        0     2962 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/processors/base.py
+-rw-r--r--   0        0        0     2349 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/processors/imagenet.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/py.typed
+-rw-r--r--   0        0        0     6388 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/furiosa/serving/telemetry.py
+-rw-r--r--   0        0        0     2882 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      692 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/tests/test_load_models.py
+-rw-r--r--   0        0        0     1087 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/tests/test_processors.py
+-rw-r--r--   0        0        0      582 2023-04-14 20:42:32.897314 furiosa-serving-0.9.0rc2/tests/test_subapp.py
+-rw-r--r--   0        0        0    13488 1970-01-01 00:00:00.000000 furiosa-serving-0.9.0rc2/PKG-INFO
```

### Comparing `furiosa-serving-0.8.0/README.md` & `furiosa-serving-0.9.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/examples/assets/images/1234567890.jpg` & `furiosa-serving-0.9.0rc2/examples/assets/images/1234567890.jpg`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/examples/assets/images/6254.jpg` & `furiosa-serving-0.9.0rc2/examples/assets/images/6254.jpg`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/examples/assets/images/car.jpg` & `furiosa-serving-0.9.0rc2/examples/assets/images/car.jpg`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/examples/assets/labels/ImageNetLabels.txt` & `furiosa-serving-0.9.0rc2/examples/assets/labels/ImageNetLabels.txt`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/examples/assets/models/MNISTnet_uint8_quant_without_softmax.tflite` & `furiosa-serving-0.9.0rc2/examples/assets/models/MNISTnet_uint8_quant_without_softmax.tflite`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/examples/assets/models/image_classification.onnx` & `furiosa-serving-0.9.0rc2/examples/assets/models/image_classification.onnx`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/examples/image_classify.py` & `furiosa-serving-0.9.0rc2/examples/image_classify.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/examples/number_classify.py` & `furiosa-serving-0.9.0rc2/examples/number_classify.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/furiosa/serving/application.py` & `furiosa-serving-0.9.0rc2/furiosa/serving/application.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/furiosa/serving/apps/health.py` & `furiosa-serving-0.9.0rc2/furiosa/serving/apps/health.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/furiosa/serving/apps/model.py` & `furiosa-serving-0.9.0rc2/furiosa/serving/apps/model.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/furiosa/serving/apps/repository.py` & `furiosa-serving-0.9.0rc2/furiosa/serving/apps/repository.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/furiosa/serving/model.py` & `furiosa-serving-0.9.0rc2/furiosa/serving/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,14 @@
 
     @property
     def outputs(self) -> List[TensorDesc]:
         raise NotImplementedError("CPUServerModel outputs() not yet supported")
 
 
 class OpenVINOServeModel(ServeModel):
-
     if TYPE_CHECKING:
         from openvino.runtime.ie_api import ConstOutput
 
     def __init__(
         self,
         app: FastAPI,
         name: str,
```

### Comparing `furiosa-serving-0.8.0/furiosa/serving/processors/base.py` & `furiosa-serving-0.9.0rc2/furiosa/serving/processors/base.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/furiosa/serving/processors/imagenet.py` & `furiosa-serving-0.9.0rc2/furiosa/serving/processors/imagenet.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/furiosa/serving/telemetry.py` & `furiosa-serving-0.9.0rc2/furiosa/serving/telemetry.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/pyproject.toml` & `furiosa-serving-0.9.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-serving"
-version = "0.8.0"
+version = "0.9.0.rc2"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Environment :: Web Environment",
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
-    "furiosa-server == 0.8.*",
-    "furiosa-registry == 0.8.*",
+    "furiosa-server == 0.9.*",
+    "furiosa-registry == 0.9.*",
 
     "Pillow",
     "python-multipart",
 
     "prometheus-client",
     "opentelemetry-instrumentation-fastapi",
     "opentelemetry-instrumentation-logging",
@@ -43,15 +43,15 @@
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-asyncio ~= 0.17.2"
 ]
 openvino = [
-    "furiosa-server[openvino] == 0.8.*",
+    "furiosa-server[openvino] == 0.9.*",
     "transformers"
 ]
 
 [project.urls]
 Home = "https://furiosa.ai"
 Documentation = "https://furiosa-ai.github.io/docs"
 "Bug Tracker" = "https://github.com/furiosa-ai/furiosa-sdk/issues"
@@ -59,15 +59,15 @@
 
 [tool.flit.module]
 name = "furiosa.serving"
 
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
@@ -88,8 +88,8 @@
 
 [tool.flit.sdist]
 include = ["furiosa/serving/git_version.txt"]
 
 [tool.pydocstyle]
 convention = "google"
 # http://www.pydocstyle.org/en/stable/error_codes.html
-add_ignore = ["D100", "D101", "D102", "D103", "D106"]
+add_ignore = ["D100", "D101", "D102", "D103", "D106"]
```

### Comparing `furiosa-serving-0.8.0/tests/test_load_models.py` & `furiosa-serving-0.9.0rc2/tests/test_load_models.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/tests/test_processors.py` & `furiosa-serving-0.9.0rc2/tests/test_processors.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/tests/test_subapp.py` & `furiosa-serving-0.9.0rc2/tests/test_subapp.py`

 * *Files identical despite different names*

### Comparing `furiosa-serving-0.8.0/PKG-INFO` & `furiosa-serving-0.9.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: furiosa-serving
-Version: 0.8.0
+Version: 0.9.0rc2
 Summary: Furiosa serving framework, easy to use inference server.
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
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
-Requires-Dist: furiosa-server == 0.8.*
-Requires-Dist: furiosa-registry == 0.8.*
+Requires-Dist: furiosa-server == 0.9.*
+Requires-Dist: furiosa-registry == 0.9.*
 Requires-Dist: Pillow
 Requires-Dist: python-multipart
 Requires-Dist: prometheus-client
 Requires-Dist: opentelemetry-instrumentation-fastapi
 Requires-Dist: opentelemetry-instrumentation-logging
 Requires-Dist: opentelemetry-exporter-otlp
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-sdk
-Requires-Dist: furiosa-server[openvino] == 0.8.* ; extra == "openvino"
+Requires-Dist: furiosa-server[openvino] == 0.9.* ; extra == "openvino"
 Requires-Dist: transformers ; extra == "openvino"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-asyncio ~= 0.17.2 ; extra == "test"
 Project-URL: Bug Tracker, https://github.com/furiosa-ai/furiosa-sdk/issues
 Project-URL: Documentation, https://furiosa-ai.github.io/docs
 Project-URL: Home, https://furiosa.ai
 Project-URL: Source Code, https://github.com/furiosa-ai/furiosa-sdk
```

