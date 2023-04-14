# Comparing `tmp/furiosa-sdk-0.8.0.tar.gz` & `tmp/furiosa-sdk-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-sdk-0.8.0.tar", last modified: Sat Nov  5 00:14:45 2022, max compression
+gzip compressed data, was "furiosa-sdk-0.9.0rc2.tar", last modified: Fri Apr 14 20:49:40 2023, max compression
```

## Comparing `furiosa-sdk-0.8.0.tar` & `furiosa-sdk-0.9.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      386 2022-11-05 00:10:12.226210 furiosa-sdk-0.8.0/Makefile
--rw-r--r--   0        0        0     2454 2022-11-05 00:10:12.226210 furiosa-sdk-0.8.0/README.md
--rw-r--r--   0        0        0     1107 2022-11-05 00:10:12.226210 furiosa-sdk-0.8.0/docs/Makefile
--rw-r--r--   0        0        0     5330 2022-11-05 00:10:12.226210 furiosa-sdk-0.8.0/docs/conf.py
--rw-r--r--   0        0        0      670 2022-11-05 00:10:12.226210 furiosa-sdk-0.8.0/docs/furiosa.rst
--rw-r--r--   0        0        0      470 2022-11-05 00:10:12.226210 furiosa-sdk-0.8.0/docs/index.rst
--rw-r--r--   0        0        0      795 2022-11-05 00:10:12.226210 furiosa-sdk-0.8.0/docs/make.bat
--rw-r--r--   0        0        0       18 2022-11-05 00:10:12.226210 furiosa-sdk-0.8.0/furiosa/sdk/__init__.py
--rw-r--r--   0        0        0     1763 2022-11-05 00:10:12.226210 furiosa-sdk-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4603 1970-01-01 00:00:00.000000 furiosa-sdk-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      386 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/Makefile
+-rw-r--r--   0        0        0     2542 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/README.md
+-rw-r--r--   0        0        0     1107 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/docs/Makefile
+-rw-r--r--   0        0        0     5330 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/docs/conf.py
+-rw-r--r--   0        0        0      670 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/docs/furiosa.rst
+-rw-r--r--   0        0        0      470 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/docs/make.bat
+-rw-r--r--   0        0        0       18 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/furiosa/sdk/__init__.py
+-rw-r--r--   0        0        0     1833 2023-04-14 20:42:32.781315 furiosa-sdk-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 furiosa-sdk-0.9.0rc2/PKG-INFO
```

### Comparing `furiosa-sdk-0.8.0/README.md` & `furiosa-sdk-0.9.0rc2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -17,34 +17,35 @@
 You can install also furiosa-sdk with extra packages (e.g., litmus, quantizer):
 
 ```sh
 pip install 'furiosa-sdk[litmus,quantizer]'
 ```
 
 The following are the extra packages:
-* models: Library which provides pre-tained models for Furiosa NPU
 * litmus: Command line tool to check if a model is compatible with furiosa-sdk
+* models: Library which provides pretained models for Furiosa NPU
+* quantizer: Library which quantizes and optimizes DNN models
 * server: Serving framework enabling a DNN model to provide HTTP/GRPC endpoints
 * serving: FastAPI-based Serving Library
-* quantizer: Library which allows to quantize DNN models
 
 ## Releases
-* [Furiosa SDK 0.7.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.7.0) (Latest)
+* [Furiosa SDK 0.8.2](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/0.8.2) (Latest)
+* [Furiosa SDK 0.7.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.7.0)
 * [Furiosa SDK 0.6.3](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.6.3)
 * [Furiosa SDK 0.6.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.6.0)
 * [Furiosa SDK 0.5.2](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.2)
 * [Furiosa SDK 0.5.1](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.1)
 * [Furiosa SDK 0.5.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.0)
 * [Furiosa SDK 0.4.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.4.0)
 * [Furiosa SDK 0.2.1](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.2.1)
 
 ## License
 
 ```
-Copyright 2022 FuriosaAI, Inc.
+Copyright 2023 FuriosaAI, Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `furiosa-sdk-0.8.0/docs/Makefile` & `furiosa-sdk-0.9.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.8.0/docs/conf.py` & `furiosa-sdk-0.9.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.8.0/docs/furiosa.rst` & `furiosa-sdk-0.9.0rc2/docs/furiosa.rst`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.8.0/docs/make.bat` & `furiosa-sdk-0.9.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `furiosa-sdk-0.8.0/pyproject.toml` & `furiosa-sdk-0.9.0rc2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 [build-system]
 requires = ["flit_core"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "furiosa-sdk"
-version = "0.8.0"
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
-    "furiosa-cli == 0.8.*",
-    "furiosa-runtime == 0.8.*",
-    "furiosa-tools == 0.8.*",
+    "furiosa-cli == 0.9.*",
+    "furiosa-runtime == 0.9.*",
+    "furiosa-tools == 0.9.*",
 ]
 
 [project.optional-dependencies]
 test = []
 
-cli = ["furiosa-cli == 0.8.*"]
-litmus = ["furiosa-litmus == 0.8.*"]
-quantizer = ["furiosa-quantizer == 0.8.*"]
-registry = ["furiosa-registry == 0.8.*"]
-server = ["furiosa-server == 0.8.*"]
-serving = ["furiosa-serving == 0.8.*"]
-tool = ["furiosa-tools == 0.8.*"]
+cli = ["furiosa-cli == 0.9.*"]
+litmus = ["furiosa-litmus == 0.9.*"]
+registry = ["furiosa-registry == 0.9.*"]
+quantizer = ["furiosa-optimizer == 0.9.*", "furiosa-quantizer == 0.9.*",]
+server = ["furiosa-server == 0.9.*"]
+serving = ["furiosa-serving == 0.9.*"]
+tool = ["furiosa-tools == 0.9.*"]
 
 full = [
-    "furiosa-cli == 0.8.*",
-    "furiosa-litmus == 0.8.*",
-    "furiosa-quantizer == 0.8.*",
-    "furiosa-registry == 0.8.*",
-    "furiosa-server == 0.8.*",
-    "furiosa-serving == 0.8.*",
-    "furiosa-tools == 0.8.*",
+    "furiosa-cli == 0.9.*",
+    "furiosa-litmus == 0.9.*",
+    "furiosa-registry == 0.9.*",
+    "furiosa-optimizer == 0.9.*",
+    "furiosa-quantizer == 0.9.*",
+    "furiosa-server == 0.9.*",
+    "furiosa-serving == 0.9.*",
+    "furiosa-tools == 0.9.*",
 ]
 
 [project.urls]
 Home = "https://furiosa.ai"
 Documentation = "https://furiosa-ai.github.io/docs"
 "Bug Tracker" = "https://github.com/furiosa-ai/furiosa-sdk/issues"
 "Source Code" = "https://github.com/furiosa-ai/furiosa-sdk"
```

### Comparing `furiosa-sdk-0.8.0/PKG-INFO` & `furiosa-sdk-0.9.0rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: furiosa-sdk
-Version: 0.8.0
+Version: 0.9.0rc2
 Summary: Furiosa SDK
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
-Requires-Dist: furiosa-cli == 0.8.*
-Requires-Dist: furiosa-runtime == 0.8.*
-Requires-Dist: furiosa-tools == 0.8.*
-Requires-Dist: furiosa-cli == 0.8.* ; extra == "cli"
-Requires-Dist: furiosa-cli == 0.8.* ; extra == "full"
-Requires-Dist: furiosa-litmus == 0.8.* ; extra == "full"
-Requires-Dist: furiosa-quantizer == 0.8.* ; extra == "full"
-Requires-Dist: furiosa-registry == 0.8.* ; extra == "full"
-Requires-Dist: furiosa-server == 0.8.* ; extra == "full"
-Requires-Dist: furiosa-serving == 0.8.* ; extra == "full"
-Requires-Dist: furiosa-tools == 0.8.* ; extra == "full"
-Requires-Dist: furiosa-litmus == 0.8.* ; extra == "litmus"
-Requires-Dist: furiosa-quantizer == 0.8.* ; extra == "quantizer"
-Requires-Dist: furiosa-registry == 0.8.* ; extra == "registry"
-Requires-Dist: furiosa-server == 0.8.* ; extra == "server"
-Requires-Dist: furiosa-serving == 0.8.* ; extra == "serving"
-Requires-Dist: furiosa-tools == 0.8.* ; extra == "tool"
+Requires-Dist: furiosa-cli == 0.9.*
+Requires-Dist: furiosa-runtime == 0.9.*
+Requires-Dist: furiosa-tools == 0.9.*
+Requires-Dist: furiosa-cli == 0.9.* ; extra == "cli"
+Requires-Dist: furiosa-cli == 0.9.* ; extra == "full"
+Requires-Dist: furiosa-litmus == 0.9.* ; extra == "full"
+Requires-Dist: furiosa-registry == 0.9.* ; extra == "full"
+Requires-Dist: furiosa-optimizer == 0.9.* ; extra == "full"
+Requires-Dist: furiosa-quantizer == 0.9.* ; extra == "full"
+Requires-Dist: furiosa-server == 0.9.* ; extra == "full"
+Requires-Dist: furiosa-serving == 0.9.* ; extra == "full"
+Requires-Dist: furiosa-tools == 0.9.* ; extra == "full"
+Requires-Dist: furiosa-litmus == 0.9.* ; extra == "litmus"
+Requires-Dist: furiosa-optimizer == 0.9.* ; extra == "quantizer"
+Requires-Dist: furiosa-quantizer == 0.9.* ; extra == "quantizer"
+Requires-Dist: furiosa-registry == 0.9.* ; extra == "registry"
+Requires-Dist: furiosa-server == 0.9.* ; extra == "server"
+Requires-Dist: furiosa-serving == 0.9.* ; extra == "serving"
+Requires-Dist: furiosa-tools == 0.9.* ; extra == "tool"
 Project-URL: Bug Tracker, https://github.com/furiosa-ai/furiosa-sdk/issues
 Project-URL: Documentation, https://furiosa-ai.github.io/docs
 Project-URL: Home, https://furiosa.ai
 Project-URL: Source Code, https://github.com/furiosa-ai/furiosa-sdk
 Provides-Extra: cli
 Provides-Extra: full
 Provides-Extra: litmus
@@ -66,34 +68,35 @@
 You can install also furiosa-sdk with extra packages (e.g., litmus, quantizer):
 
 ```sh
 pip install 'furiosa-sdk[litmus,quantizer]'
 ```
 
 The following are the extra packages:
-* models: Library which provides pre-tained models for Furiosa NPU
 * litmus: Command line tool to check if a model is compatible with furiosa-sdk
+* models: Library which provides pretained models for Furiosa NPU
+* quantizer: Library which quantizes and optimizes DNN models
 * server: Serving framework enabling a DNN model to provide HTTP/GRPC endpoints
 * serving: FastAPI-based Serving Library
-* quantizer: Library which allows to quantize DNN models
 
 ## Releases
-* [Furiosa SDK 0.7.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.7.0) (Latest)
+* [Furiosa SDK 0.8.2](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/0.8.2) (Latest)
+* [Furiosa SDK 0.7.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.7.0)
 * [Furiosa SDK 0.6.3](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.6.3)
 * [Furiosa SDK 0.6.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.6.0)
 * [Furiosa SDK 0.5.2](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.2)
 * [Furiosa SDK 0.5.1](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.1)
 * [Furiosa SDK 0.5.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.5.0)
 * [Furiosa SDK 0.4.0](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.4.0)
 * [Furiosa SDK 0.2.1](https://github.com/furiosa-ai/furiosa-sdk/releases/tag/v0.2.1)
 
 ## License
 
 ```
-Copyright 2022 FuriosaAI, Inc.
+Copyright 2023 FuriosaAI, Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

