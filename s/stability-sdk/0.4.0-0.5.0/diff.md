# Comparing `tmp/stability-sdk-0.4.0.tar.gz` & `tmp/stability-sdk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability-sdk-0.4.0.tar", last modified: Mon Mar 13 20:59:44 2023, max compression
+gzip compressed data, was "stability-sdk-0.5.0.tar", last modified: Fri Apr 14 04:22:17 2023, max compression
```

## Comparing `stability-sdk-0.4.0.tar` & `stability-sdk-0.5.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.335622 stability-sdk-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-13 20:59:19.000000 stability-sdk-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-03-13 20:59:44.335622 stability-sdk-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-03-13 20:59:19.000000 stability-sdk-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-13 20:59:19.000000 stability-sdk-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 20:59:44.335622 stability-sdk-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-13 20:59:19.000000 stability-sdk-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.327622 stability-sdk-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.331622 stability-sdk-0.4.0/src/stability_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-13 20:59:19.000000 stability-sdk-0.4.0/src/stability_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-03-13 20:59:19.000000 stability-sdk-0.4.0/src/stability_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-03-13 20:59:19.000000 stability-sdk-0.4.0/src/stability_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.331622 stability-sdk-0.4.0/src/stability_sdk/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.331622 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.331622 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)    20051 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.331622 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.335622 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27356 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.335622 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/project/
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-03-13 20:59:21.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.327622 stability-sdk-0.4.0/src/stability_sdk/interfaces/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.335622 stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:23.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-03-13 20:59:23.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-03-13 20:59:23.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.335622 stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:23.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-13 20:59:23.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-13 20:59:23.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-13 20:59:23.000000 stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-13 20:59:19.000000 stability-sdk-0.4.0/src/stability_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.331622 stability-sdk-0.4.0/src/stability_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-03-13 20:59:44.000000 stability-sdk-0.4.0/src/stability_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-13 20:59:44.000000 stability-sdk-0.4.0/src/stability_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 20:59:44.000000 stability-sdk-0.4.0/src/stability_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-13 20:59:44.000000 stability-sdk-0.4.0/src/stability_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-13 20:59:44.000000 stability-sdk-0.4.0/src/stability_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 20:59:44.335622 stability-sdk-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-13 20:59:19.000000 stability-sdk-0.4.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-03-13 20:59:19.000000 stability-sdk-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.206665 stability-sdk-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21637 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25811 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37463 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/project/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/project/project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.206665 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-14 04:21:56.000000 stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/src/stability_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.210665 stability-sdk-0.5.0/src/stability_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-14 04:22:17.000000 stability-sdk-0.5.0/src/stability_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-14 04:22:17.000000 stability-sdk-0.5.0/src/stability_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:22:17.000000 stability-sdk-0.5.0/src/stability_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 04:22:17.000000 stability-sdk-0.5.0/src/stability_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 04:22:17.000000 stability-sdk-0.5.0/src/stability_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:22:17.214665 stability-sdk-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-14 04:21:55.000000 stability-sdk-0.5.0/tests/test_utils.py
```

### Comparing `stability-sdk-0.4.0/LICENSE` & `stability-sdk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/PKG-INFO` & `stability-sdk-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
-Author: Wes Brown
-Author-email: wesbrown18@gmail.com
-Maintainer: David Marx
-Maintainer-email: david@stability.ai
+Author: Stability AI
+Author-email: support@stability.ai
+Maintainer: Stability AI
+Maintainer-email: support@stability.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Education
@@ -31,26 +31,27 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # stability-sdk
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stability-ai/stability-sdk/blob/main/nbs/demo_colab.ipynb)
 
-Client implementations that interact with the Stability Generator API
+Client implementations that interact with the Stability API. 
 
-# Installation
+## Getting an API key
 
-Install the PyPI package via:
+Follow the [instructions](https://platform.stability.ai/docs/getting-started/authentication) on [Platform](https://platform.stability.ai) to obtain an API key.
 
-`pip install stability-sdk`
+## PyPI Package Installation
+
+Install the [PyPI](https://pypi.org/project/stability-sdk/) package via:
 
-# Getting an API key
-You can manage API keys in your dreamstudio account [here](https://beta.dreamstudio.ai/membership?tab=apiKeys)
+`pip install stability-sdk`
 
-# Python client
+## Python Client
 
 `client.py` is both a command line client and an API class that wraps the gRPC based API. To try the client:
 
 - Use Python venv: `python3 -m venv pyenv`
 - Set up in venv dependencies: `pyenv/bin/pip3 install -e .`
 - `pyenv/bin/activate` to use the venv.
 - Set the `STABILITY_HOST` environment variable. This is by default set to the production endpoint `grpc.stability.ai:443`.
@@ -63,15 +64,15 @@
 It will generate and put PNGs in your current directory.
 
 To upscale:
 `python3 -m stability_sdk upscale -i "/path/to/image.png"`
 
 ## SDK Usage
 
-See usage demo notebooks in ./nbs
+Be sure to check out [Platform](https://platform.stability.ai) for comprehensive documentation on how to interact with our API.
 
 ## Command line usage
 
 ```
 usage: python -m stability_sdk generate [-h] [--height HEIGHT] [--width WIDTH] [--start_schedule START_SCHEDULE]
                  [--end_schedule END_SCHEDULE] [--cfg_scale CFG_SCALE] [--sampler SAMPLER]
                  [--steps STEPS] [--seed SEED] [--prefix PREFIX] [--engine ENGINE]
@@ -141,26 +142,21 @@
   --engine ENGINE, -e ENGINE
                         engine to use for upscale
 ```
 
 
 ## Connecting to the API using languages other than Python
 
-The `src` subdirectory contains pre-compiled gRPC stubs for the following languages:
-
-- [Javascript/Typescript](https://github.com/Stability-AI/stability-sdk/tree/main/src/js)
-
-If a language you would like to connect to the API with is not listed above, you can use the following
+If a language you would like to connect to the API with is not currently documented on [Platform](https://platform.stability.ai) you can use the following
 protobuf definition to compile stubs for your language:
 
 - [protobuf spec](https://github.com/Stability-AI/api-interfaces/blob/main/src/proto/)
 
 ## Community-contributed clients
 
 * Typescript client: https://github.com/jakiestfu/stability-ts
 * Guide to building for Ruby: https://github.com/kmcphillips/stability-sdk/blob/main/src/ruby/README.md
 
-## DreamStudio API TOS
-
-Unless otherwise specified, usage of the dreamstudio API falls under the same usage terms as the dreamstudio web interface: 
+## Stability API TOS
 
-* https://beta.dreamstudio.ai/terms-of-service
+Usage of the Stability API falls under the [STABILITY AI API Terms of Service.
+](https://platform.stability.ai/docs/terms-of-service)
```

### Comparing `stability-sdk-0.4.0/README.md` & `stability-sdk-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # stability-sdk
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stability-ai/stability-sdk/blob/main/nbs/demo_colab.ipynb)
 
-Client implementations that interact with the Stability Generator API
+Client implementations that interact with the Stability API. 
 
-# Installation
+## Getting an API key
 
-Install the PyPI package via:
+Follow the [instructions](https://platform.stability.ai/docs/getting-started/authentication) on [Platform](https://platform.stability.ai) to obtain an API key.
 
-`pip install stability-sdk`
+## PyPI Package Installation
+
+Install the [PyPI](https://pypi.org/project/stability-sdk/) package via:
 
-# Getting an API key
-You can manage API keys in your dreamstudio account [here](https://beta.dreamstudio.ai/membership?tab=apiKeys)
+`pip install stability-sdk`
 
-# Python client
+## Python Client
 
 `client.py` is both a command line client and an API class that wraps the gRPC based API. To try the client:
 
 - Use Python venv: `python3 -m venv pyenv`
 - Set up in venv dependencies: `pyenv/bin/pip3 install -e .`
 - `pyenv/bin/activate` to use the venv.
 - Set the `STABILITY_HOST` environment variable. This is by default set to the production endpoint `grpc.stability.ai:443`.
@@ -30,15 +31,15 @@
 It will generate and put PNGs in your current directory.
 
 To upscale:
 `python3 -m stability_sdk upscale -i "/path/to/image.png"`
 
 ## SDK Usage
 
-See usage demo notebooks in ./nbs
+Be sure to check out [Platform](https://platform.stability.ai) for comprehensive documentation on how to interact with our API.
 
 ## Command line usage
 
 ```
 usage: python -m stability_sdk generate [-h] [--height HEIGHT] [--width WIDTH] [--start_schedule START_SCHEDULE]
                  [--end_schedule END_SCHEDULE] [--cfg_scale CFG_SCALE] [--sampler SAMPLER]
                  [--steps STEPS] [--seed SEED] [--prefix PREFIX] [--engine ENGINE]
@@ -108,26 +109,21 @@
   --engine ENGINE, -e ENGINE
                         engine to use for upscale
 ```
 
 
 ## Connecting to the API using languages other than Python
 
-The `src` subdirectory contains pre-compiled gRPC stubs for the following languages:
-
-- [Javascript/Typescript](https://github.com/Stability-AI/stability-sdk/tree/main/src/js)
-
-If a language you would like to connect to the API with is not listed above, you can use the following
+If a language you would like to connect to the API with is not currently documented on [Platform](https://platform.stability.ai) you can use the following
 protobuf definition to compile stubs for your language:
 
 - [protobuf spec](https://github.com/Stability-AI/api-interfaces/blob/main/src/proto/)
 
 ## Community-contributed clients
 
 * Typescript client: https://github.com/jakiestfu/stability-ts
 * Guide to building for Ruby: https://github.com/kmcphillips/stability-sdk/blob/main/src/ruby/README.md
 
-## DreamStudio API TOS
-
-Unless otherwise specified, usage of the dreamstudio API falls under the same usage terms as the dreamstudio web interface: 
+## Stability API TOS
 
-* https://beta.dreamstudio.ai/terms-of-service
+Usage of the Stability API falls under the [STABILITY AI API Terms of Service.
+](https://platform.stability.ai/docs/terms-of-service)
```

### Comparing `stability-sdk-0.4.0/setup.py` & `stability-sdk-0.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from setuptools import setup, find_namespace_packages
 
 with open('README.md','r') as f:
     README = f.read()
 
 setup(
     name='stability-sdk',
-    version='0.4.0',
-    author='Wes Brown',
-    author_email='wesbrown18@gmail.com',
-    maintainer='David Marx',
-    maintainer_email='david@stability.ai',
+    version='0.5.0',
+    author='Stability AI',
+    author_email='support@stability.ai',
+    maintainer='Stability AI',
+    maintainer_email='support@stability.ai',
     url='https://beta.dreamstudio.ai/',
     download_url='https://github.com/Stability-AI/stability-sdk/',
 
     description='Python SDK for interacting with stability.ai APIs',
     long_description=README,
     long_description_content_type="text/markdown",
```

### Comparing `stability-sdk-0.4.0/src/stability_sdk/__main__.py` & `stability-sdk-0.5.0/src/stability_sdk/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 )
 parser.add_argument("--show", action="store_true", help="open artifacts using PIL")
 parser.add_argument(
     "--engine",
     "-e",
     type=str,
     help="engine to use for inference",
-    default="stable-diffusion-v1-5",
+    default="stable-diffusion-xl-beta-v2-2-2",
 )
 parser.add_argument(
     "--init_image",
     "-i",
     type=str,
     help="Init image",
 )
```

### Comparing `stability-sdk-0.4.0/src/stability_sdk/client.py` & `stability-sdk-0.5.0/src/stability_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 
 class StabilityInference:
     def __init__(
         self,
         host: str = "grpc.stability.ai:443",
         key: str = "",
-        engine: str = "stable-diffusion-v1-5",
+        engine: str = "stable-diffusion-xl-beta-v2-2-2",
         upscale_engine: str = "esrgan-v1-x2plus",
         verbose: bool = False,
         wait_for_ready: bool = True,
     ):
         """
         Initialize the client.
 
@@ -510,15 +510,15 @@
     )
     parser_generate.add_argument("--show", action="store_true", help="open artifacts using PIL")
     parser_generate.add_argument(
         "--engine",
         "-e",
         type=str,
         help="engine to use for inference",
-        default="stable-diffusion-v1-5",
+        default="stable-diffusion-xl-beta-v2-2-2",
     )
     parser_generate.add_argument(
         "--init_image",
         "-i",
         type=str,
         help="Init image",
     )
```

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0f\x64\x61shboard.proto\x12\x07gooseai\"\xa9\x01\n\x12OrganizationMember\x12+\n\x0corganization\x18\x01 \x01(\x0b\x32\x15.gooseai.Organization\x12 \n\x04user\x18\x02 \x01(\x0b\x32\r.gooseai.UserH\x00\x88\x01\x01\x12\'\n\x04role\x18\x03 \x01(\x0e\x32\x19.gooseai.OrganizationRole\x12\x12\n\nis_default\x18\x04 \x01(\x08\x42\x07\n\x05_user\"h\n\x11OrganizationGrant\x12\x16\n\x0e\x61mount_granted\x18\x01 \x01(\x01\x12\x13\n\x0b\x61mount_used\x18\x02 \x01(\x01\x12\x12\n\nexpires_at\x18\x03 \x01(\x04\x12\x12\n\ngranted_at\x18\x04 \x01(\x04\"V\n\x17OrganizationPaymentInfo\x12\x0f\n\x07\x62\x61lance\x18\x01 \x01(\x01\x12*\n\x06grants\x18\x02 \x03(\x0b\x32\x1a.gooseai.OrganizationGrant\"I\n\x16OrganizationAutoCharge\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02id\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x04\"\xbc\x02\n\x0cOrganization\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12,\n\x07members\x18\x04 \x03(\x0b\x32\x1b.gooseai.OrganizationMember\x12;\n\x0cpayment_info\x18\x05 \x01(\x0b\x32 .gooseai.OrganizationPaymentInfoH\x00\x88\x01\x01\x12\x1f\n\x12stripe_customer_id\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x39\n\x0b\x61uto_charge\x18\x07 \x01(\x0b\x32\x1f.gooseai.OrganizationAutoChargeH\x02\x88\x01\x01\x42\x0f\n\r_payment_infoB\x15\n\x13_stripe_customer_idB\x0e\n\x0c_auto_charge\"<\n\x06\x41PIKey\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x11\n\tis_secret\x18\x02 \x01(\x08\x12\x12\n\ncreated_at\x18\x03 \x01(\x04\"\xf7\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x07\x61uth_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x17\n\x0fprofile_picture\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x32\n\rorganizations\x18\x05 \x03(\x0b\x32\x1b.gooseai.OrganizationMember\x12!\n\x08\x61pi_keys\x18\x07 \x03(\x0b\x32\x0f.gooseai.APIKey\x12\x12\n\ncreated_at\x18\x08 \x01(\x04\x12\x1b\n\x0e\x65mail_verified\x18\t \x01(\x08H\x01\x88\x01\x01\x42\n\n\x08_auth_idB\x11\n\x0f_email_verified\"9\n\x08\x43ostData\x12\x15\n\ramount_tokens\x18\x01 \x01(\r\x12\x16\n\x0e\x61mount_credits\x18\x02 \x01(\x01\"\xba\x01\n\x0bUsageMetric\x12\x11\n\toperation\x18\x01 \x01(\t\x12\x0e\n\x06\x65ngine\x18\x02 \x01(\t\x12%\n\ninput_cost\x18\x03 \x01(\x0b\x32\x11.gooseai.CostData\x12&\n\x0boutput_cost\x18\x04 \x01(\x0b\x32\x11.gooseai.CostData\x12\x11\n\x04user\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x1d\n\x15\x61ggregation_timestamp\x18\x06 \x01(\x04\x42\x07\n\x05_user\":\n\tCostTotal\x12\x15\n\ramount_tokens\x18\x01 \x01(\r\x12\x16\n\x0e\x61mount_credits\x18\x02 \x01(\x01\"e\n\x10TotalMetricsData\x12\'\n\x0binput_total\x18\x01 \x01(\x0b\x32\x12.gooseai.CostTotal\x12(\n\x0coutput_total\x18\x02 \x01(\x0b\x32\x12.gooseai.CostTotal\"Z\n\x07Metrics\x12%\n\x07metrics\x18\x01 \x03(\x0b\x32\x14.gooseai.UsageMetric\x12(\n\x05total\x18\x02 \x01(\x0b\x32\x19.gooseai.TotalMetricsData\"\x0e\n\x0c\x45mptyRequest\"$\n\x16GetOrganizationRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x99\x01\n\x11GetMetricsRequest\x12\x17\n\x0forganization_id\x18\x01 \x01(\t\x12\x14\n\x07user_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\nrange_from\x18\x03 \x01(\x04\x12\x10\n\x08range_to\x18\x04 \x01(\x04\x12#\n\x1binclude_per_request_metrics\x18\x05 \x01(\x08\x42\n\n\x08_user_id\"\"\n\rAPIKeyRequest\x12\x11\n\tis_secret\x18\x01 \x01(\x08\"\x1f\n\x11\x41PIKeyFindRequest\x12\n\n\x02id\x18\x01 \x01(\t\";\n UpdateDefaultOrganizationRequest\x12\x17\n\x0forganization_id\x18\x01 \x01(\t\"\"\n\x0e\x43lientSettings\x12\x10\n\x08settings\x18\x01 \x01(\x0c\"\x80\x01\n\x1d\x43reateAutoChargeIntentRequest\x12\x17\n\x0forganization_id\x18\x01 \x01(\t\x12\x17\n\x0fmonthly_maximum\x18\x02 \x01(\x04\x12\x15\n\rminimum_value\x18\x03 \x01(\x04\x12\x16\n\x0e\x61mount_credits\x18\x04 \x01(\x04\">\n\x13\x43reateChargeRequest\x12\x0e\n\x06\x61mount\x18\x01 \x01(\x04\x12\x17\n\x0forganization_id\x18\x02 \x01(\t\"R\n\x11GetChargesRequest\x12\x17\n\x0forganization_id\x18\x01 \x01(\t\x12\x12\n\nrange_from\x18\x02 \x01(\x04\x12\x10\n\x08range_to\x18\x03 \x01(\x04\"z\n\x06\x43harge\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04paid\x18\x02 \x01(\x08\x12\x14\n\x0creceipt_link\x18\x03 \x01(\t\x12\x14\n\x0cpayment_link\x18\x04 \x01(\t\x12\x12\n\ncreated_at\x18\x05 \x01(\x04\x12\x16\n\x0e\x61mount_credits\x18\x06 \x01(\x04\"+\n\x07\x43harges\x12 \n\x07\x63harges\x18\x01 \x03(\x0b\x32\x0f.gooseai.Charge\"/\n\x14GetAutoChargeRequest\x12\x17\n\x0forganization_id\x18\x01 \x01(\t\"\x90\x01\n\x10\x41utoChargeIntent\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x0cpayment_link\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x04\x12\x17\n\x0fmonthly_maximum\x18\x04 \x01(\x04\x12\x15\n\rminimum_value\x18\x05 \x01(\x04\x12\x16\n\x0e\x61mount_credits\x18\x06 \x01(\x04\"5\n\x15UpdateUserInfoRequest\x12\x12\n\x05\x65mail\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_email\"*\n\x18UserPasswordChangeTicket\x12\x0e\n\x06ticket\x18\x01 \x01(\t*9\n\x10OrganizationRole\x12\n\n\x06MEMBER\x10\x00\x12\x0e\n\nACCOUNTANT\x10\x01\x12\t\n\x05OWNER\x10\x02\x32\xf7\x08\n\x10\x44\x61shboardService\x12-\n\x05GetMe\x12\x15.gooseai.EmptyRequest\x1a\r.gooseai.User\x12I\n\x0fGetOrganization\x12\x1f.gooseai.GetOrganizationRequest\x1a\x15.gooseai.Organization\x12:\n\nGetMetrics\x12\x1a.gooseai.GetMetricsRequest\x1a\x10.gooseai.Metrics\x12\x37\n\x0c\x43reateAPIKey\x12\x16.gooseai.APIKeyRequest\x1a\x0f.gooseai.APIKey\x12;\n\x0c\x44\x65leteAPIKey\x12\x1a.gooseai.APIKeyFindRequest\x1a\x0f.gooseai.APIKey\x12U\n\x19UpdateDefaultOrganization\x12).gooseai.UpdateDefaultOrganizationRequest\x1a\r.gooseai.User\x12\x43\n\x11GetClientSettings\x12\x15.gooseai.EmptyRequest\x1a\x17.gooseai.ClientSettings\x12\x45\n\x11SetClientSettings\x12\x17.gooseai.ClientSettings\x1a\x17.gooseai.ClientSettings\x12?\n\x0eUpdateUserInfo\x12\x1e.gooseai.UpdateUserInfoRequest\x1a\r.gooseai.User\x12V\n\x1a\x43reatePasswordChangeTicket\x12\x15.gooseai.EmptyRequest\x1a!.gooseai.UserPasswordChangeTicket\x12\x35\n\rDeleteAccount\x12\x15.gooseai.EmptyRequest\x1a\r.gooseai.User\x12=\n\x0c\x43reateCharge\x12\x1c.gooseai.CreateChargeRequest\x1a\x0f.gooseai.Charge\x12:\n\nGetCharges\x12\x1a.gooseai.GetChargesRequest\x1a\x10.gooseai.Charges\x12[\n\x16\x43reateAutoChargeIntent\x12&.gooseai.CreateAutoChargeIntentRequest\x1a\x19.gooseai.AutoChargeIntent\x12[\n\x16UpdateAutoChargeIntent\x12&.gooseai.CreateAutoChargeIntentRequest\x1a\x19.gooseai.AutoChargeIntent\x12O\n\x13GetAutoChargeIntent\x12\x1d.gooseai.GetAutoChargeRequest\x1a\x19.gooseai.AutoChargeIntentB\x0eZ\x0c./;dashboardb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0f\x64\x61shboard.proto\x12\x07gooseai\"\xa9\x01\n\x12OrganizationMember\x12+\n\x0corganization\x18\x01 \x01(\x0b\x32\x15.gooseai.Organization\x12 \n\x04user\x18\x02 \x01(\x0b\x32\r.gooseai.UserH\x00\x88\x01\x01\x12\'\n\x04role\x18\x03 \x01(\x0e\x32\x19.gooseai.OrganizationRole\x12\x12\n\nis_default\x18\x04 \x01(\x08\x42\x07\n\x05_user\"h\n\x11OrganizationGrant\x12\x16\n\x0e\x61mount_granted\x18\x01 \x01(\x01\x12\x13\n\x0b\x61mount_used\x18\x02 \x01(\x01\x12\x12\n\nexpires_at\x18\x03 \x01(\x04\x12\x12\n\ngranted_at\x18\x04 \x01(\x04\"V\n\x17OrganizationPaymentInfo\x12\x0f\n\x07\x62\x61lance\x18\x01 \x01(\x01\x12*\n\x06grants\x18\x02 \x03(\x0b\x32\x1a.gooseai.OrganizationGrant\"I\n\x16OrganizationAutoCharge\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\n\n\x02id\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x04\"\xbc\x02\n\x0cOrganization\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12,\n\x07members\x18\x04 \x03(\x0b\x32\x1b.gooseai.OrganizationMember\x12;\n\x0cpayment_info\x18\x05 \x01(\x0b\x32 .gooseai.OrganizationPaymentInfoH\x00\x88\x01\x01\x12\x1f\n\x12stripe_customer_id\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x39\n\x0b\x61uto_charge\x18\x07 \x01(\x0b\x32\x1f.gooseai.OrganizationAutoChargeH\x02\x88\x01\x01\x42\x0f\n\r_payment_infoB\x15\n\x13_stripe_customer_idB\x0e\n\x0c_auto_charge\"<\n\x06\x41PIKey\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x11\n\tis_secret\x18\x02 \x01(\x08\x12\x12\n\ncreated_at\x18\x03 \x01(\x04\"\xf7\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x07\x61uth_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x17\n\x0fprofile_picture\x18\x03 \x01(\t\x12\r\n\x05\x65mail\x18\x04 \x01(\t\x12\x32\n\rorganizations\x18\x05 \x03(\x0b\x32\x1b.gooseai.OrganizationMember\x12!\n\x08\x61pi_keys\x18\x07 \x03(\x0b\x32\x0f.gooseai.APIKey\x12\x12\n\ncreated_at\x18\x08 \x01(\x04\x12\x1b\n\x0e\x65mail_verified\x18\t \x01(\x08H\x01\x88\x01\x01\x42\n\n\x08_auth_idB\x11\n\x0f_email_verified\"9\n\x08\x43ostData\x12\x15\n\ramount_tokens\x18\x01 \x01(\r\x12\x16\n\x0e\x61mount_credits\x18\x02 \x01(\x01\"\xba\x01\n\x0bUsageMetric\x12\x11\n\toperation\x18\x01 \x01(\t\x12\x0e\n\x06\x65ngine\x18\x02 \x01(\t\x12%\n\ninput_cost\x18\x03 \x01(\x0b\x32\x11.gooseai.CostData\x12&\n\x0boutput_cost\x18\x04 \x01(\x0b\x32\x11.gooseai.CostData\x12\x11\n\x04user\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x1d\n\x15\x61ggregation_timestamp\x18\x06 \x01(\x04\x42\x07\n\x05_user\":\n\tCostTotal\x12\x15\n\ramount_tokens\x18\x01 \x01(\r\x12\x16\n\x0e\x61mount_credits\x18\x02 \x01(\x01\"e\n\x10TotalMetricsData\x12\'\n\x0binput_total\x18\x01 \x01(\x0b\x32\x12.gooseai.CostTotal\x12(\n\x0coutput_total\x18\x02 \x01(\x0b\x32\x12.gooseai.CostTotal\"Z\n\x07Metrics\x12%\n\x07metrics\x18\x01 \x03(\x0b\x32\x14.gooseai.UsageMetric\x12(\n\x05total\x18\x02 \x01(\x0b\x32\x19.gooseai.TotalMetricsData\"\x0e\n\x0c\x45mptyRequest\"$\n\x16GetOrganizationRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x99\x01\n\x11GetMetricsRequest\x12\x17\n\x0forganization_id\x18\x01 \x01(\t\x12\x14\n\x07user_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x12\n\nrange_from\x18\x03 \x01(\x04\x12\x10\n\x08range_to\x18\x04 \x01(\x04\x12#\n\x1binclude_per_request_metrics\x18\x05 \x01(\x08\x42\n\n\x08_user_id\"\"\n\rAPIKeyRequest\x12\x11\n\tis_secret\x18\x01 \x01(\x08\"\x1f\n\x11\x41PIKeyFindRequest\x12\n\n\x02id\x18\x01 \x01(\t\";\n UpdateDefaultOrganizationRequest\x12\x17\n\x0forganization_id\x18\x01 \x01(\t\"\"\n\x0e\x43lientSettings\x12\x10\n\x08settings\x18\x01 \x01(\x0c\"\x80\x01\n\x1d\x43reateAutoChargeIntentRequest\x12\x17\n\x0forganization_id\x18\x01 \x01(\t\x12\x17\n\x0fmonthly_maximum\x18\x02 \x01(\x04\x12\x15\n\rminimum_value\x18\x03 \x01(\x04\x12\x16\n\x0e\x61mount_credits\x18\x04 \x01(\x04\">\n\x13\x43reateChargeRequest\x12\x0e\n\x06\x61mount\x18\x01 \x01(\x04\x12\x17\n\x0forganization_id\x18\x02 \x01(\t\"R\n\x11GetChargesRequest\x12\x17\n\x0forganization_id\x18\x01 \x01(\t\x12\x12\n\nrange_from\x18\x02 \x01(\x04\x12\x10\n\x08range_to\x18\x03 \x01(\x04\"z\n\x06\x43harge\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04paid\x18\x02 \x01(\x08\x12\x14\n\x0creceipt_link\x18\x03 \x01(\t\x12\x14\n\x0cpayment_link\x18\x04 \x01(\t\x12\x12\n\ncreated_at\x18\x05 \x01(\x04\x12\x16\n\x0e\x61mount_credits\x18\x06 \x01(\x04\"+\n\x07\x43harges\x12 \n\x07\x63harges\x18\x01 \x03(\x0b\x32\x0f.gooseai.Charge\"/\n\x14GetAutoChargeRequest\x12\x17\n\x0forganization_id\x18\x01 \x01(\t\"\x90\x01\n\x10\x41utoChargeIntent\x12\n\n\x02id\x18\x01 \x01(\t\x12\x14\n\x0cpayment_link\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x04\x12\x17\n\x0fmonthly_maximum\x18\x04 \x01(\x04\x12\x15\n\rminimum_value\x18\x05 \x01(\x04\x12\x16\n\x0e\x61mount_credits\x18\x06 \x01(\x04\"5\n\x15UpdateUserInfoRequest\x12\x12\n\x05\x65mail\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_email\"*\n\x18UserPasswordChangeTicket\x12\x0e\n\x06ticket\x18\x01 \x01(\t*9\n\x10OrganizationRole\x12\n\n\x06MEMBER\x10\x00\x12\x0e\n\nACCOUNTANT\x10\x01\x12\t\n\x05OWNER\x10\x02\x32\xf7\x08\n\x10\x44\x61shboardService\x12-\n\x05GetMe\x12\x15.gooseai.EmptyRequest\x1a\r.gooseai.User\x12I\n\x0fGetOrganization\x12\x1f.gooseai.GetOrganizationRequest\x1a\x15.gooseai.Organization\x12:\n\nGetMetrics\x12\x1a.gooseai.GetMetricsRequest\x1a\x10.gooseai.Metrics\x12\x37\n\x0c\x43reateAPIKey\x12\x16.gooseai.APIKeyRequest\x1a\x0f.gooseai.APIKey\x12;\n\x0c\x44\x65leteAPIKey\x12\x1a.gooseai.APIKeyFindRequest\x1a\x0f.gooseai.APIKey\x12U\n\x19UpdateDefaultOrganization\x12).gooseai.UpdateDefaultOrganizationRequest\x1a\r.gooseai.User\x12\x43\n\x11GetClientSettings\x12\x15.gooseai.EmptyRequest\x1a\x17.gooseai.ClientSettings\x12\x45\n\x11SetClientSettings\x12\x17.gooseai.ClientSettings\x1a\x17.gooseai.ClientSettings\x12?\n\x0eUpdateUserInfo\x12\x1e.gooseai.UpdateUserInfoRequest\x1a\r.gooseai.User\x12V\n\x1a\x43reatePasswordChangeTicket\x12\x15.gooseai.EmptyRequest\x1a!.gooseai.UserPasswordChangeTicket\x12\x35\n\rDeleteAccount\x12\x15.gooseai.EmptyRequest\x1a\r.gooseai.User\x12=\n\x0c\x43reateCharge\x12\x1c.gooseai.CreateChargeRequest\x1a\x0f.gooseai.Charge\x12:\n\nGetCharges\x12\x1a.gooseai.GetChargesRequest\x1a\x10.gooseai.Charges\x12[\n\x16\x43reateAutoChargeIntent\x12&.gooseai.CreateAutoChargeIntentRequest\x1a\x19.gooseai.AutoChargeIntent\x12[\n\x16UpdateAutoChargeIntent\x12&.gooseai.CreateAutoChargeIntentRequest\x1a\x19.gooseai.AutoChargeIntent\x12O\n\x13GetAutoChargeIntent\x12\x1d.gooseai.GetAutoChargeRequest\x1a\x19.gooseai.AutoChargeIntentB:Z8github.com/stability-ai/api-interfaces/gooseai/dashboardb\x06proto3')
 
 _ORGANIZATIONROLE = DESCRIPTOR.enum_types_by_name['OrganizationRole']
 OrganizationRole = enum_type_wrapper.EnumTypeWrapper(_ORGANIZATIONROLE)
 MEMBER = 0
 ACCOUNTANT = 1
 OWNER = 2
 
@@ -248,15 +248,15 @@
   })
 _sym_db.RegisterMessage(UserPasswordChangeTicket)
 
 _DASHBOARDSERVICE = DESCRIPTOR.services_by_name['DashboardService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\014./;dashboard'
+  DESCRIPTOR._serialized_options = b'Z8github.com/stability-ai/api-interfaces/gooseai/dashboard'
   _ORGANIZATIONROLE._serialized_start=2722
   _ORGANIZATIONROLE._serialized_end=2779
   _ORGANIZATIONMEMBER._serialized_start=29
   _ORGANIZATIONMEMBER._serialized_end=198
   _ORGANIZATIONGRANT._serialized_start=200
   _ORGANIZATIONGRANT._serialized_end=304
   _ORGANIZATIONPAYMENTINFO._serialized_start=306
```

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/dashboard/dashboard_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rengines.proto\x12\x07gooseai\"\xa9\x01\n\nEngineInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12\r\n\x05ready\x18\x03 \x01(\x08\x12!\n\x04type\x18\x04 \x01(\x0e\x32\x13.gooseai.EngineType\x12+\n\ttokenizer\x18\x05 \x01(\x0e\x32\x18.gooseai.EngineTokenizer\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\"\x14\n\x12ListEnginesRequest\".\n\x07\x45ngines\x12#\n\x06\x65ngine\x18\x01 \x03(\x0b\x32\x13.gooseai.EngineInfo*Z\n\nEngineType\x12\x08\n\x04TEXT\x10\x00\x12\x0b\n\x07PICTURE\x10\x01\x12\t\n\x05\x41UDIO\x10\x02\x12\t\n\x05VIDEO\x10\x03\x12\x12\n\x0e\x43LASSIFICATION\x10\x04\x12\x0b\n\x07STORAGE\x10\x05*%\n\x0f\x45ngineTokenizer\x12\x08\n\x04GPT2\x10\x00\x12\x08\n\x04PILE\x10\x01\x32P\n\x0e\x45nginesService\x12>\n\x0bListEngines\x12\x1b.gooseai.ListEnginesRequest\x1a\x10.gooseai.Engines\"\x00\x42\x0cZ\n./;enginesb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rengines.proto\x12\x07gooseai\"\xa9\x01\n\nEngineInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12\r\n\x05ready\x18\x03 \x01(\x08\x12!\n\x04type\x18\x04 \x01(\x0e\x32\x13.gooseai.EngineType\x12+\n\ttokenizer\x18\x05 \x01(\x0e\x32\x18.gooseai.EngineTokenizer\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\"\x14\n\x12ListEnginesRequest\".\n\x07\x45ngines\x12#\n\x06\x65ngine\x18\x01 \x03(\x0b\x32\x13.gooseai.EngineInfo*Z\n\nEngineType\x12\x08\n\x04TEXT\x10\x00\x12\x0b\n\x07PICTURE\x10\x01\x12\t\n\x05\x41UDIO\x10\x02\x12\t\n\x05VIDEO\x10\x03\x12\x12\n\x0e\x43LASSIFICATION\x10\x04\x12\x0b\n\x07STORAGE\x10\x05*%\n\x0f\x45ngineTokenizer\x12\x08\n\x04GPT2\x10\x00\x12\x08\n\x04PILE\x10\x01\x32P\n\x0e\x45nginesService\x12>\n\x0bListEngines\x12\x1b.gooseai.ListEnginesRequest\x1a\x10.gooseai.Engines\"\x00\x42\x38Z6github.com/stability-ai/api-interfaces/gooseai/enginesb\x06proto3')
 
 _ENGINETYPE = DESCRIPTOR.enum_types_by_name['EngineType']
 EngineType = enum_type_wrapper.EnumTypeWrapper(_ENGINETYPE)
 _ENGINETOKENIZER = DESCRIPTOR.enum_types_by_name['EngineTokenizer']
 EngineTokenizer = enum_type_wrapper.EnumTypeWrapper(_ENGINETOKENIZER)
 TEXT = 0
 PICTURE = 1
@@ -55,15 +55,15 @@
   })
 _sym_db.RegisterMessage(Engines)
 
 _ENGINESSERVICE = DESCRIPTOR.services_by_name['EnginesService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\n./;engines'
+  DESCRIPTOR._serialized_options = b'Z6github.com/stability-ai/api-interfaces/gooseai/engines'
   _ENGINETYPE._serialized_start=268
   _ENGINETYPE._serialized_end=358
   _ENGINETOKENIZER._serialized_start=360
   _ENGINETOKENIZER._serialized_end=397
   _ENGINEINFO._serialized_start=27
   _ENGINEINFO._serialized_end=196
   _LISTENGINESREQUEST._serialized_start=198
```

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/engines/engines_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 import tensors_pb2 as tensors__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10generation.proto\x12\x07gooseai\x1a\rtensors.proto\"/\n\x05Token\x12\x11\n\x04text\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\n\n\x02id\x18\x02 \x01(\rB\x07\n\x05_text\"T\n\x06Tokens\x12\x1e\n\x06tokens\x18\x01 \x03(\x0b\x32\x0e.gooseai.Token\x12\x19\n\x0ctokenizer_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0f\n\r_tokenizer_id\"\xf3\x02\n\x08\x41rtifact\x12\n\n\x02id\x18\x01 \x01(\x04\x12#\n\x04type\x18\x02 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x0c\n\x04mime\x18\x03 \x01(\t\x12\x12\n\x05magic\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x06\x62inary\x18\x05 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x06 \x01(\tH\x00\x12!\n\x06tokens\x18\x07 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12\x33\n\nclassifier\x18\x0b \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12!\n\x06tensor\x18\x0e \x01(\x0b\x32\x0f.tensors.TensorH\x00\x12\r\n\x05index\x18\x08 \x01(\r\x12,\n\rfinish_reason\x18\t \x01(\x0e\x32\x15.gooseai.FinishReason\x12\x0c\n\x04seed\x18\n \x01(\r\x12\x0c\n\x04uuid\x18\x0c \x01(\t\x12\x0c\n\x04size\x18\r \x01(\x04\x42\x06\n\x04\x64\x61taB\x08\n\x06_magic\"N\n\x10PromptParameters\x12\x11\n\x04init\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x13\n\x06weight\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x07\n\x05_initB\t\n\x07_weight\"\xaf\x01\n\x06Prompt\x12\x32\n\nparameters\x18\x01 \x01(\x0b\x32\x19.gooseai.PromptParametersH\x01\x88\x01\x01\x12\x0e\n\x04text\x18\x02 \x01(\tH\x00\x12!\n\x06tokens\x18\x03 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12%\n\x08\x61rtifact\x18\x04 \x01(\x0b\x32\x11.gooseai.ArtifactH\x00\x42\x08\n\x06promptB\r\n\x0b_parameters\"\xa3\x02\n\x11SamplerParameters\x12\x10\n\x03\x65ta\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x1b\n\x0esampling_steps\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x1c\n\x0flatent_channels\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12 \n\x13\x64ownsampling_factor\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x16\n\tcfg_scale\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12\x1d\n\x10init_noise_scale\x18\x06 \x01(\x02H\x05\x88\x01\x01\x42\x06\n\x04_etaB\x11\n\x0f_sampling_stepsB\x12\n\x10_latent_channelsB\x16\n\x14_downsampling_factorB\x0c\n\n_cfg_scaleB\x13\n\x11_init_noise_scale\"\x8b\x01\n\x15\x43onditionerParameters\x12 \n\x13vector_adjust_prior\x18\x01 \x01(\tH\x00\x88\x01\x01\x12(\n\x0b\x63onditioner\x18\x02 \x01(\x0b\x32\x0e.gooseai.ModelH\x01\x88\x01\x01\x42\x16\n\x14_vector_adjust_priorB\x0e\n\x0c_conditioner\"j\n\x12ScheduleParameters\x12\x12\n\x05start\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x10\n\x03\x65nd\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05value\x18\x03 \x01(\x02H\x02\x88\x01\x01\x42\x08\n\x06_startB\x06\n\x04_endB\x08\n\x06_value\"\xe4\x01\n\rStepParameter\x12\x13\n\x0bscaled_step\x18\x01 \x01(\x02\x12\x30\n\x07sampler\x18\x02 \x01(\x0b\x32\x1a.gooseai.SamplerParametersH\x00\x88\x01\x01\x12\x32\n\x08schedule\x18\x03 \x01(\x0b\x32\x1b.gooseai.ScheduleParametersH\x01\x88\x01\x01\x12\x32\n\x08guidance\x18\x04 \x01(\x0b\x32\x1b.gooseai.GuidanceParametersH\x02\x88\x01\x01\x42\n\n\x08_samplerB\x0b\n\t_scheduleB\x0b\n\t_guidance\"\x97\x01\n\x05Model\x12\x30\n\x0c\x61rchitecture\x18\x01 \x01(\x0e\x32\x1a.gooseai.ModelArchitecture\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\x02\x12\x18\n\x10semantic_version\x18\x05 \x01(\t\x12\r\n\x05\x61lias\x18\x06 \x01(\t\"\xbc\x01\n\x10\x43utoutParameters\x12*\n\x07\x63utouts\x18\x01 \x03(\x0b\x32\x19.gooseai.CutoutParameters\x12\x12\n\x05\x63ount\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x11\n\x04gray\x18\x03 \x01(\x02H\x01\x88\x01\x01\x12\x11\n\x04\x62lur\x18\x04 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsize_power\x18\x05 \x01(\x02H\x03\x88\x01\x01\x42\x08\n\x06_countB\x07\n\x05_grayB\x07\n\x05_blurB\r\n\x0b_size_power\"=\n\x1aGuidanceScheduleParameters\x12\x10\n\x08\x64uration\x18\x01 \x01(\x02\x12\r\n\x05value\x18\x02 \x01(\x02\"\x97\x02\n\x1aGuidanceInstanceParameters\x12\x1e\n\x06models\x18\x02 \x03(\x0b\x32\x0e.gooseai.Model\x12\x1e\n\x11guidance_strength\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12\x35\n\x08schedule\x18\x04 \x03(\x0b\x32#.gooseai.GuidanceScheduleParameters\x12/\n\x07\x63utouts\x18\x05 \x01(\x0b\x32\x19.gooseai.CutoutParametersH\x01\x88\x01\x01\x12$\n\x06prompt\x18\x06 \x01(\x0b\x32\x0f.gooseai.PromptH\x02\x88\x01\x01\x42\x14\n\x12_guidance_strengthB\n\n\x08_cutoutsB\t\n\x07_prompt\"~\n\x12GuidanceParameters\x12\x30\n\x0fguidance_preset\x18\x01 \x01(\x0e\x32\x17.gooseai.GuidancePreset\x12\x36\n\tinstances\x18\x02 \x03(\x0b\x32#.gooseai.GuidanceInstanceParameters\"n\n\rTransformType\x12.\n\tdiffusion\x18\x01 \x01(\x0e\x32\x19.gooseai.DiffusionSamplerH\x00\x12%\n\x08upscaler\x18\x02 \x01(\x0e\x32\x11.gooseai.UpscalerH\x00\x42\x06\n\x04type\"\xd4\x02\n\x0fImageParameters\x12\x13\n\x06height\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05width\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x0c\n\x04seed\x18\x03 \x03(\r\x12\x14\n\x07samples\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x12\n\x05steps\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12.\n\ttransform\x18\x06 \x01(\x0b\x32\x16.gooseai.TransformTypeH\x04\x88\x01\x01\x12*\n\nparameters\x18\x07 \x03(\x0b\x32\x16.gooseai.StepParameter\x12\x36\n\x10masked_area_init\x18\x08 \x01(\x0e\x32\x17.gooseai.MaskedAreaInitH\x05\x88\x01\x01\x42\t\n\x07_heightB\x08\n\x06_widthB\n\n\x08_samplesB\x08\n\x06_stepsB\x0c\n\n_transformB\x13\n\x11_masked_area_init\"J\n\x11\x43lassifierConcept\x12\x0f\n\x07\x63oncept\x18\x01 \x01(\t\x12\x16\n\tthreshold\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\x0c\n\n_threshold\"\xf4\x01\n\x12\x43lassifierCategory\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x1a.gooseai.ClassifierConcept\x12\x17\n\nadjustment\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x0f.gooseai.ActionH\x01\x88\x01\x01\x12\x35\n\x0f\x63lassifier_mode\x18\x05 \x01(\x0e\x32\x17.gooseai.ClassifierModeH\x02\x88\x01\x01\x42\r\n\x0b_adjustmentB\t\n\x07_actionB\x12\n\x10_classifier_mode\"\xb8\x01\n\x14\x43lassifierParameters\x12/\n\ncategories\x18\x01 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12,\n\x07\x65xceeds\x18\x02 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12-\n\x0frealized_action\x18\x03 \x01(\x0e\x32\x0f.gooseai.ActionH\x00\x88\x01\x01\x42\x12\n\x10_realized_action\"k\n\x0f\x41ssetParameters\x12$\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\x14.gooseai.AssetAction\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x1e\n\x03use\x18\x03 \x01(\x0e\x32\x11.gooseai.AssetUse\"\x94\x01\n\nAnswerMeta\x12\x13\n\x06gpu_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06\x63pu_id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x07node_id\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tengine_id\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\t\n\x07_gpu_idB\t\n\x07_cpu_idB\n\n\x08_node_idB\x0c\n\n_engine_id\"\xa9\x01\n\x06\x41nswer\x12\x11\n\tanswer_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x10\n\x08received\x18\x03 \x01(\x04\x12\x0f\n\x07\x63reated\x18\x04 \x01(\x04\x12&\n\x04meta\x18\x06 \x01(\x0b\x32\x13.gooseai.AnswerMetaH\x00\x88\x01\x01\x12$\n\tartifacts\x18\x07 \x03(\x0b\x32\x11.gooseai.ArtifactB\x07\n\x05_meta\"\xc8\x03\n\x07Request\x12\x11\n\tengine_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12-\n\x0erequested_type\x18\x03 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x1f\n\x06prompt\x18\x04 \x03(\x0b\x32\x0f.gooseai.Prompt\x12)\n\x05image\x18\x05 \x01(\x0b\x32\x18.gooseai.ImageParametersH\x00\x12\x33\n\nclassifier\x18\x07 \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12)\n\x05\x61sset\x18\x08 \x01(\x0b\x32\x18.gooseai.AssetParametersH\x00\x12\x38\n\x0b\x63onditioner\x18\x06 \x01(\x0b\x32\x1e.gooseai.ConditionerParametersH\x01\x88\x01\x01\x12\x31\n\rweight_method\x18\t \x01(\x0e\x32\x15.gooseai.WeightMethodH\x02\x88\x01\x01\x12\"\n\tuc_prompt\x18\n \x03(\x0b\x32\x0f.gooseai.PromptB\x08\n\x06paramsB\x0e\n\x0c_conditionerB\x10\n\x0e_weight_method\"w\n\x08OnStatus\x12%\n\x06reason\x18\x01 \x03(\x0e\x32\x15.gooseai.FinishReason\x12\x13\n\x06target\x18\x02 \x01(\tH\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x03 \x03(\x0e\x32\x14.gooseai.StageActionB\t\n\x07_target\"\\\n\x05Stage\x12\n\n\x02id\x18\x01 \x01(\t\x12!\n\x07request\x18\x02 \x01(\x0b\x32\x10.gooseai.Request\x12$\n\ton_status\x18\x03 \x03(\x0b\x32\x11.gooseai.OnStatus\"A\n\x0c\x43hainRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\x1d\n\x05stage\x18\x02 \x03(\x0b\x32\x0e.gooseai.Stage*E\n\x0c\x46inishReason\x12\x08\n\x04NULL\x10\x00\x12\n\n\x06LENGTH\x10\x01\x12\x08\n\x04STOP\x10\x02\x12\t\n\x05\x45RROR\x10\x03\x12\n\n\x06\x46ILTER\x10\x04*\xe4\x01\n\x0c\x41rtifactType\x12\x11\n\rARTIFACT_NONE\x10\x00\x12\x12\n\x0e\x41RTIFACT_IMAGE\x10\x01\x12\x12\n\x0e\x41RTIFACT_VIDEO\x10\x02\x12\x11\n\rARTIFACT_TEXT\x10\x03\x12\x13\n\x0f\x41RTIFACT_TOKENS\x10\x04\x12\x16\n\x12\x41RTIFACT_EMBEDDING\x10\x05\x12\x1c\n\x18\x41RTIFACT_CLASSIFICATIONS\x10\x06\x12\x11\n\rARTIFACT_MASK\x10\x07\x12\x13\n\x0f\x41RTIFACT_LATENT\x10\x08\x12\x13\n\x0f\x41RTIFACT_TENSOR\x10\t*g\n\x0eMaskedAreaInit\x12\x19\n\x15MASKED_AREA_INIT_ZERO\x10\x00\x12\x1b\n\x17MASKED_AREA_INIT_RANDOM\x10\x01\x12\x1d\n\x19MASKED_AREA_INIT_ORIGINAL\x10\x02*5\n\x0cWeightMethod\x12\x10\n\x0cTEXT_ENCODER\x10\x00\x12\x13\n\x0f\x43ROSS_ATTENTION\x10\x01*\xff\x01\n\x10\x44iffusionSampler\x12\x10\n\x0cSAMPLER_DDIM\x10\x00\x12\x10\n\x0cSAMPLER_DDPM\x10\x01\x12\x13\n\x0fSAMPLER_K_EULER\x10\x02\x12\x1d\n\x19SAMPLER_K_EULER_ANCESTRAL\x10\x03\x12\x12\n\x0eSAMPLER_K_HEUN\x10\x04\x12\x13\n\x0fSAMPLER_K_DPM_2\x10\x05\x12\x1d\n\x19SAMPLER_K_DPM_2_ANCESTRAL\x10\x06\x12\x11\n\rSAMPLER_K_LMS\x10\x07\x12 \n\x1cSAMPLER_K_DPMPP_2S_ANCESTRAL\x10\x08\x12\x16\n\x12SAMPLER_K_DPMPP_2M\x10\t*F\n\x08Upscaler\x12\x10\n\x0cUPSCALER_RGB\x10\x00\x12\x13\n\x0fUPSCALER_GFPGAN\x10\x01\x12\x13\n\x0fUPSCALER_ESRGAN\x10\x02*\xd8\x01\n\x0eGuidancePreset\x12\x18\n\x14GUIDANCE_PRESET_NONE\x10\x00\x12\x1a\n\x16GUIDANCE_PRESET_SIMPLE\x10\x01\x12\x1d\n\x19GUIDANCE_PRESET_FAST_BLUE\x10\x02\x12\x1e\n\x1aGUIDANCE_PRESET_FAST_GREEN\x10\x03\x12\x18\n\x14GUIDANCE_PRESET_SLOW\x10\x04\x12\x1a\n\x16GUIDANCE_PRESET_SLOWER\x10\x05\x12\x1b\n\x17GUIDANCE_PRESET_SLOWEST\x10\x06*\x91\x01\n\x11ModelArchitecture\x12\x1b\n\x17MODEL_ARCHITECTURE_NONE\x10\x00\x12\x1f\n\x1bMODEL_ARCHITECTURE_CLIP_VIT\x10\x01\x12\"\n\x1eMODEL_ARCHITECTURE_CLIP_RESNET\x10\x02\x12\x1a\n\x16MODEL_ARCHITECTURE_LDM\x10\x03*\xa2\x01\n\x06\x41\x63tion\x12\x16\n\x12\x41\x43TION_PASSTHROUGH\x10\x00\x12\x1f\n\x1b\x41\x43TION_REGENERATE_DUPLICATE\x10\x01\x12\x15\n\x11\x41\x43TION_REGENERATE\x10\x02\x12\x1e\n\x1a\x41\x43TION_OBFUSCATE_DUPLICATE\x10\x03\x12\x14\n\x10\x41\x43TION_OBFUSCATE\x10\x04\x12\x12\n\x0e\x41\x43TION_DISCARD\x10\x05*D\n\x0e\x43lassifierMode\x12\x17\n\x13\x43LSFR_MODE_ZEROSHOT\x10\x00\x12\x19\n\x15\x43LSFR_MODE_MULTICLASS\x10\x01*=\n\x0b\x41ssetAction\x12\r\n\tASSET_PUT\x10\x00\x12\r\n\tASSET_GET\x10\x01\x12\x10\n\x0c\x41SSET_DELETE\x10\x02*\x81\x01\n\x08\x41ssetUse\x12\x17\n\x13\x41SSET_USE_UNDEFINED\x10\x00\x12\x13\n\x0f\x41SSET_USE_INPUT\x10\x01\x12\x14\n\x10\x41SSET_USE_OUTPUT\x10\x02\x12\x1a\n\x16\x41SSET_USE_INTERMEDIATE\x10\x03\x12\x15\n\x11\x41SSET_USE_PROJECT\x10\x04*W\n\x0bStageAction\x12\x15\n\x11STAGE_ACTION_PASS\x10\x00\x12\x18\n\x14STAGE_ACTION_DISCARD\x10\x01\x12\x17\n\x13STAGE_ACTION_RETURN\x10\x02\x32\x83\x01\n\x11GenerationService\x12\x31\n\x08Generate\x12\x10.gooseai.Request\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x12;\n\rChainGenerate\x12\x15.gooseai.ChainRequest\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x42\x0fZ\r./;generationb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10generation.proto\x12\x07gooseai\x1a\x1cgoogle/protobuf/struct.proto\x1a\rtensors.proto\"/\n\x05Token\x12\x11\n\x04text\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\n\n\x02id\x18\x02 \x01(\rB\x07\n\x05_text\"T\n\x06Tokens\x12\x1e\n\x06tokens\x18\x01 \x03(\x0b\x32\x0e.gooseai.Token\x12\x19\n\x0ctokenizer_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0f\n\r_tokenizer_id\"\xf3\x02\n\x08\x41rtifact\x12\n\n\x02id\x18\x01 \x01(\x04\x12#\n\x04type\x18\x02 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x0c\n\x04mime\x18\x03 \x01(\t\x12\x12\n\x05magic\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x10\n\x06\x62inary\x18\x05 \x01(\x0cH\x00\x12\x0e\n\x04text\x18\x06 \x01(\tH\x00\x12!\n\x06tokens\x18\x07 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12\x33\n\nclassifier\x18\x0b \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12!\n\x06tensor\x18\x0e \x01(\x0b\x32\x0f.tensors.TensorH\x00\x12\r\n\x05index\x18\x08 \x01(\r\x12,\n\rfinish_reason\x18\t \x01(\x0e\x32\x15.gooseai.FinishReason\x12\x0c\n\x04seed\x18\n \x01(\r\x12\x0c\n\x04uuid\x18\x0c \x01(\t\x12\x0c\n\x04size\x18\r \x01(\x04\x42\x06\n\x04\x64\x61taB\x08\n\x06_magic\"N\n\x10PromptParameters\x12\x11\n\x04init\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x13\n\x06weight\x18\x02 \x01(\x02H\x01\x88\x01\x01\x42\x07\n\x05_initB\t\n\x07_weight\"\xaf\x01\n\x06Prompt\x12\x32\n\nparameters\x18\x01 \x01(\x0b\x32\x19.gooseai.PromptParametersH\x01\x88\x01\x01\x12\x0e\n\x04text\x18\x02 \x01(\tH\x00\x12!\n\x06tokens\x18\x03 \x01(\x0b\x32\x0f.gooseai.TokensH\x00\x12%\n\x08\x61rtifact\x18\x04 \x01(\x0b\x32\x11.gooseai.ArtifactH\x00\x42\x08\n\x06promptB\r\n\x0b_parameters\"\xd7\x02\n\x11SamplerParameters\x12\x10\n\x03\x65ta\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x1b\n\x0esampling_steps\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x1c\n\x0flatent_channels\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12 \n\x13\x64ownsampling_factor\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x16\n\tcfg_scale\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12\x1d\n\x10init_noise_scale\x18\x06 \x01(\x02H\x05\x88\x01\x01\x12\x1d\n\x10step_noise_scale\x18\x07 \x01(\x02H\x06\x88\x01\x01\x42\x06\n\x04_etaB\x11\n\x0f_sampling_stepsB\x12\n\x10_latent_channelsB\x16\n\x14_downsampling_factorB\x0c\n\n_cfg_scaleB\x13\n\x11_init_noise_scaleB\x13\n\x11_step_noise_scale\"\x8b\x01\n\x15\x43onditionerParameters\x12 \n\x13vector_adjust_prior\x18\x01 \x01(\tH\x00\x88\x01\x01\x12(\n\x0b\x63onditioner\x18\x02 \x01(\x0b\x32\x0e.gooseai.ModelH\x01\x88\x01\x01\x42\x16\n\x14_vector_adjust_priorB\x0e\n\x0c_conditioner\"j\n\x12ScheduleParameters\x12\x12\n\x05start\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x10\n\x03\x65nd\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x12\n\x05value\x18\x03 \x01(\x02H\x02\x88\x01\x01\x42\x08\n\x06_startB\x06\n\x04_endB\x08\n\x06_value\"\xe4\x01\n\rStepParameter\x12\x13\n\x0bscaled_step\x18\x01 \x01(\x02\x12\x30\n\x07sampler\x18\x02 \x01(\x0b\x32\x1a.gooseai.SamplerParametersH\x00\x88\x01\x01\x12\x32\n\x08schedule\x18\x03 \x01(\x0b\x32\x1b.gooseai.ScheduleParametersH\x01\x88\x01\x01\x12\x32\n\x08guidance\x18\x04 \x01(\x0b\x32\x1b.gooseai.GuidanceParametersH\x02\x88\x01\x01\x42\n\n\x08_samplerB\x0b\n\t_scheduleB\x0b\n\t_guidance\"\x97\x01\n\x05Model\x12\x30\n\x0c\x61rchitecture\x18\x01 \x01(\x0e\x32\x1a.gooseai.ModelArchitecture\x12\x11\n\tpublisher\x18\x02 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\x02\x12\x18\n\x10semantic_version\x18\x05 \x01(\t\x12\r\n\x05\x61lias\x18\x06 \x01(\t\"\xbc\x01\n\x10\x43utoutParameters\x12*\n\x07\x63utouts\x18\x01 \x03(\x0b\x32\x19.gooseai.CutoutParameters\x12\x12\n\x05\x63ount\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x11\n\x04gray\x18\x03 \x01(\x02H\x01\x88\x01\x01\x12\x11\n\x04\x62lur\x18\x04 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsize_power\x18\x05 \x01(\x02H\x03\x88\x01\x01\x42\x08\n\x06_countB\x07\n\x05_grayB\x07\n\x05_blurB\r\n\x0b_size_power\"=\n\x1aGuidanceScheduleParameters\x12\x10\n\x08\x64uration\x18\x01 \x01(\x02\x12\r\n\x05value\x18\x02 \x01(\x02\"\x97\x02\n\x1aGuidanceInstanceParameters\x12\x1e\n\x06models\x18\x02 \x03(\x0b\x32\x0e.gooseai.Model\x12\x1e\n\x11guidance_strength\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12\x35\n\x08schedule\x18\x04 \x03(\x0b\x32#.gooseai.GuidanceScheduleParameters\x12/\n\x07\x63utouts\x18\x05 \x01(\x0b\x32\x19.gooseai.CutoutParametersH\x01\x88\x01\x01\x12$\n\x06prompt\x18\x06 \x01(\x0b\x32\x0f.gooseai.PromptH\x02\x88\x01\x01\x42\x14\n\x12_guidance_strengthB\n\n\x08_cutoutsB\t\n\x07_prompt\"~\n\x12GuidanceParameters\x12\x30\n\x0fguidance_preset\x18\x01 \x01(\x0e\x32\x17.gooseai.GuidancePreset\x12\x36\n\tinstances\x18\x02 \x03(\x0b\x32#.gooseai.GuidanceInstanceParameters\"n\n\rTransformType\x12.\n\tdiffusion\x18\x01 \x01(\x0e\x32\x19.gooseai.DiffusionSamplerH\x00\x12%\n\x08upscaler\x18\x02 \x01(\x0e\x32\x11.gooseai.UpscalerH\x00\x42\x06\n\x04type\"\xbd\x03\n\x0fImageParameters\x12\x13\n\x06height\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05width\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x0c\n\x04seed\x18\x03 \x03(\r\x12\x14\n\x07samples\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x12\n\x05steps\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12.\n\ttransform\x18\x06 \x01(\x0b\x32\x16.gooseai.TransformTypeH\x04\x88\x01\x01\x12*\n\nparameters\x18\x07 \x03(\x0b\x32\x16.gooseai.StepParameter\x12\x36\n\x10masked_area_init\x18\x08 \x01(\x0e\x32\x17.gooseai.MaskedAreaInitH\x05\x88\x01\x01\x12\x31\n\rweight_method\x18\t \x01(\x0e\x32\x15.gooseai.WeightMethodH\x06\x88\x01\x01\x12\x15\n\x08quantize\x18\n \x01(\x08H\x07\x88\x01\x01\x42\t\n\x07_heightB\x08\n\x06_widthB\n\n\x08_samplesB\x08\n\x06_stepsB\x0c\n\n_transformB\x13\n\x11_masked_area_initB\x10\n\x0e_weight_methodB\x0b\n\t_quantize\"J\n\x11\x43lassifierConcept\x12\x0f\n\x07\x63oncept\x18\x01 \x01(\t\x12\x16\n\tthreshold\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\x0c\n\n_threshold\"\xf4\x01\n\x12\x43lassifierCategory\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\x08\x63oncepts\x18\x02 \x03(\x0b\x32\x1a.gooseai.ClassifierConcept\x12\x17\n\nadjustment\x18\x03 \x01(\x02H\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x0f.gooseai.ActionH\x01\x88\x01\x01\x12\x35\n\x0f\x63lassifier_mode\x18\x05 \x01(\x0e\x32\x17.gooseai.ClassifierModeH\x02\x88\x01\x01\x42\r\n\x0b_adjustmentB\t\n\x07_actionB\x12\n\x10_classifier_mode\"\xb8\x01\n\x14\x43lassifierParameters\x12/\n\ncategories\x18\x01 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12,\n\x07\x65xceeds\x18\x02 \x03(\x0b\x32\x1b.gooseai.ClassifierCategory\x12-\n\x0frealized_action\x18\x03 \x01(\x0e\x32\x0f.gooseai.ActionH\x00\x88\x01\x01\x42\x12\n\x10_realized_action\"]\n\x15InterpolateParameters\x12\x0e\n\x06ratios\x18\x01 \x03(\x02\x12+\n\x04mode\x18\x02 \x01(\x0e\x32\x18.gooseai.InterpolateModeH\x00\x88\x01\x01\x42\x07\n\x05_mode\"\x9c\x03\n\x14TransformColorAdjust\x12\x17\n\nbrightness\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x15\n\x08\x63ontrast\x18\x02 \x01(\x02H\x01\x88\x01\x01\x12\x10\n\x03hue\x18\x03 \x01(\x02H\x02\x88\x01\x01\x12\x17\n\nsaturation\x18\x04 \x01(\x02H\x03\x88\x01\x01\x12\x16\n\tlightness\x18\x05 \x01(\x02H\x04\x88\x01\x01\x12+\n\x0bmatch_image\x18\x06 \x01(\x0b\x32\x11.gooseai.ArtifactH\x05\x88\x01\x01\x12\x30\n\nmatch_mode\x18\x07 \x01(\x0e\x32\x17.gooseai.ColorMatchModeH\x06\x88\x01\x01\x12\x19\n\x0cnoise_amount\x18\x08 \x01(\x02H\x07\x88\x01\x01\x12\x17\n\nnoise_seed\x18\t \x01(\rH\x08\x88\x01\x01\x42\r\n\x0b_brightnessB\x0b\n\t_contrastB\x06\n\x04_hueB\r\n\x0b_saturationB\x0c\n\n_lightnessB\x0e\n\x0c_match_imageB\r\n\x0b_match_modeB\x0f\n\r_noise_amountB\r\n\x0b_noise_seed\"\x8c\x01\n\x12TransformDepthCalc\x12\x19\n\x0c\x62lend_weight\x18\x01 \x01(\x02H\x00\x88\x01\x01\x12\x18\n\x0b\x62lur_radius\x18\x02 \x01(\rH\x01\x88\x01\x01\x12\x14\n\x07reverse\x18\x03 \x01(\x08H\x02\x88\x01\x01\x42\x0f\n\r_blend_weightB\x0e\n\x0c_blur_radiusB\n\n\x08_reverse\"#\n\x0fTransformMatrix\x12\x10\n\x04\x64\x61ta\x18\x01 \x03(\x02\x42\x02\x10\x01\"\x86\x02\n\x11TransformResample\x12(\n\x0b\x62order_mode\x18\x01 \x01(\x0e\x32\x13.gooseai.BorderMode\x12+\n\ttransform\x18\x02 \x01(\x0b\x32\x18.gooseai.TransformMatrix\x12\x35\n\x0eprev_transform\x18\x03 \x01(\x0b\x32\x18.gooseai.TransformMatrixH\x00\x88\x01\x01\x12\x17\n\ndepth_warp\x18\x04 \x01(\x02H\x01\x88\x01\x01\x12\x18\n\x0b\x65xport_mask\x18\x05 \x01(\x08H\x02\x88\x01\x01\x42\x11\n\x0f_prev_transformB\r\n\x0b_depth_warpB\x0e\n\x0c_export_mask\"}\n\x10\x43\x61meraParameters\x12(\n\x0b\x63\x61mera_type\x18\x01 \x01(\x0e\x32\x13.gooseai.CameraType\x12\x12\n\nnear_plane\x18\x02 \x01(\x02\x12\x11\n\tfar_plane\x18\x03 \x01(\x02\x12\x10\n\x03\x66ov\x18\x04 \x01(\x02H\x00\x88\x01\x01\x42\x06\n\x04_fov\"\x82\x02\n\x13TransformCameraPose\x12\x36\n\x14world_to_view_matrix\x18\x01 \x01(\x0b\x32\x18.gooseai.TransformMatrix\x12\x34\n\x11\x63\x61mera_parameters\x18\x02 \x01(\x0b\x32\x19.gooseai.CameraParameters\x12\x12\n\ndo_prefill\x18\x05 \x01(\x08\x12.\n\x11image_render_mode\x18\x06 \x01(\x0e\x32\x13.gooseai.RenderMode\x12-\n\x10mask_render_mode\x18\x07 \x01(\x0e\x32\x13.gooseai.RenderModeJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05\"\xf1\x01\n\x13TransformParameters\x12\x35\n\x0c\x63olor_adjust\x18\x02 \x01(\x0b\x32\x1d.gooseai.TransformColorAdjustH\x00\x12\x31\n\ndepth_calc\x18\x04 \x01(\x0b\x32\x1b.gooseai.TransformDepthCalcH\x00\x12.\n\x08resample\x18\x05 \x01(\x0b\x32\x1a.gooseai.TransformResampleH\x00\x12\x33\n\x0b\x63\x61mera_pose\x18\x06 \x01(\x0b\x32\x1c.gooseai.TransformCameraPoseH\x00\x42\x0b\n\ttransform\"k\n\x0f\x41ssetParameters\x12$\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32\x14.gooseai.AssetAction\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x1e\n\x03use\x18\x03 \x01(\x0e\x32\x11.gooseai.AssetUse\"\x94\x01\n\nAnswerMeta\x12\x13\n\x06gpu_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x13\n\x06\x63pu_id\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x14\n\x07node_id\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x16\n\tengine_id\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\t\n\x07_gpu_idB\t\n\x07_cpu_idB\n\n\x08_node_idB\x0c\n\n_engine_id\"\xa9\x01\n\x06\x41nswer\x12\x11\n\tanswer_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x10\n\x08received\x18\x03 \x01(\x04\x12\x0f\n\x07\x63reated\x18\x04 \x01(\x04\x12&\n\x04meta\x18\x06 \x01(\x0b\x32\x13.gooseai.AnswerMetaH\x00\x88\x01\x01\x12$\n\tartifacts\x18\x07 \x03(\x0b\x32\x11.gooseai.ArtifactB\x07\n\x05_meta\"A\n\x0b\x41nswerBatch\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12 \n\x07\x61nswers\x18\x02 \x03(\x0b\x32\x0f.gooseai.Answer\"\x8f\x04\n\x07Request\x12\x11\n\tengine_id\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12-\n\x0erequested_type\x18\x03 \x01(\x0e\x32\x15.gooseai.ArtifactType\x12\x1f\n\x06prompt\x18\x04 \x03(\x0b\x32\x0f.gooseai.Prompt\x12)\n\x05image\x18\x05 \x01(\x0b\x32\x18.gooseai.ImageParametersH\x00\x12\x33\n\nclassifier\x18\x07 \x01(\x0b\x32\x1d.gooseai.ClassifierParametersH\x00\x12)\n\x05\x61sset\x18\x08 \x01(\x0b\x32\x18.gooseai.AssetParametersH\x00\x12\x35\n\x0binterpolate\x18\x0b \x01(\x0b\x32\x1e.gooseai.InterpolateParametersH\x00\x12\x31\n\ttransform\x18\x0c \x01(\x0b\x32\x1c.gooseai.TransformParametersH\x00\x12\x38\n\x0b\x63onditioner\x18\x06 \x01(\x0b\x32\x1e.gooseai.ConditionerParametersH\x01\x88\x01\x01\x12-\n\x06\x65xtras\x18\xff\x0f \x01(\x0b\x32\x17.google.protobuf.StructH\x02\x88\x01\x01\x42\x08\n\x06paramsB\x0e\n\x0c_conditionerB\t\n\x07_extrasJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"w\n\x08OnStatus\x12%\n\x06reason\x18\x01 \x03(\x0e\x32\x15.gooseai.FinishReason\x12\x13\n\x06target\x18\x02 \x01(\tH\x00\x88\x01\x01\x12$\n\x06\x61\x63tion\x18\x03 \x03(\x0e\x32\x14.gooseai.StageActionB\t\n\x07_target\"\\\n\x05Stage\x12\n\n\x02id\x18\x01 \x01(\t\x12!\n\x07request\x18\x02 \x01(\x0b\x32\x10.gooseai.Request\x12$\n\ton_status\x18\x03 \x03(\x0b\x32\x11.gooseai.OnStatus\"A\n\x0c\x43hainRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\t\x12\x1d\n\x05stage\x18\x02 \x03(\x0b\x32\x0e.gooseai.Stage*E\n\x0c\x46inishReason\x12\x08\n\x04NULL\x10\x00\x12\n\n\x06LENGTH\x10\x01\x12\x08\n\x04STOP\x10\x02\x12\t\n\x05\x45RROR\x10\x03\x12\n\n\x06\x46ILTER\x10\x04*\xf8\x01\n\x0c\x41rtifactType\x12\x11\n\rARTIFACT_NONE\x10\x00\x12\x12\n\x0e\x41RTIFACT_IMAGE\x10\x01\x12\x12\n\x0e\x41RTIFACT_VIDEO\x10\x02\x12\x11\n\rARTIFACT_TEXT\x10\x03\x12\x13\n\x0f\x41RTIFACT_TOKENS\x10\x04\x12\x16\n\x12\x41RTIFACT_EMBEDDING\x10\x05\x12\x1c\n\x18\x41RTIFACT_CLASSIFICATIONS\x10\x06\x12\x11\n\rARTIFACT_MASK\x10\x07\x12\x13\n\x0f\x41RTIFACT_LATENT\x10\x08\x12\x13\n\x0f\x41RTIFACT_TENSOR\x10\t\x12\x12\n\x0e\x41RTIFACT_DEPTH\x10\n*g\n\x0eMaskedAreaInit\x12\x19\n\x15MASKED_AREA_INIT_ZERO\x10\x00\x12\x1b\n\x17MASKED_AREA_INIT_RANDOM\x10\x01\x12\x1d\n\x19MASKED_AREA_INIT_ORIGINAL\x10\x02*5\n\x0cWeightMethod\x12\x10\n\x0cTEXT_ENCODER\x10\x00\x12\x13\n\x0f\x43ROSS_ATTENTION\x10\x01*\x98\x02\n\x10\x44iffusionSampler\x12\x10\n\x0cSAMPLER_DDIM\x10\x00\x12\x10\n\x0cSAMPLER_DDPM\x10\x01\x12\x13\n\x0fSAMPLER_K_EULER\x10\x02\x12\x1d\n\x19SAMPLER_K_EULER_ANCESTRAL\x10\x03\x12\x12\n\x0eSAMPLER_K_HEUN\x10\x04\x12\x13\n\x0fSAMPLER_K_DPM_2\x10\x05\x12\x1d\n\x19SAMPLER_K_DPM_2_ANCESTRAL\x10\x06\x12\x11\n\rSAMPLER_K_LMS\x10\x07\x12 \n\x1cSAMPLER_K_DPMPP_2S_ANCESTRAL\x10\x08\x12\x16\n\x12SAMPLER_K_DPMPP_2M\x10\t\x12\x17\n\x13SAMPLER_K_DPMPP_SDE\x10\n*F\n\x08Upscaler\x12\x10\n\x0cUPSCALER_RGB\x10\x00\x12\x13\n\x0fUPSCALER_GFPGAN\x10\x01\x12\x13\n\x0fUPSCALER_ESRGAN\x10\x02*\xd8\x01\n\x0eGuidancePreset\x12\x18\n\x14GUIDANCE_PRESET_NONE\x10\x00\x12\x1a\n\x16GUIDANCE_PRESET_SIMPLE\x10\x01\x12\x1d\n\x19GUIDANCE_PRESET_FAST_BLUE\x10\x02\x12\x1e\n\x1aGUIDANCE_PRESET_FAST_GREEN\x10\x03\x12\x18\n\x14GUIDANCE_PRESET_SLOW\x10\x04\x12\x1a\n\x16GUIDANCE_PRESET_SLOWER\x10\x05\x12\x1b\n\x17GUIDANCE_PRESET_SLOWEST\x10\x06*\x91\x01\n\x11ModelArchitecture\x12\x1b\n\x17MODEL_ARCHITECTURE_NONE\x10\x00\x12\x1f\n\x1bMODEL_ARCHITECTURE_CLIP_VIT\x10\x01\x12\"\n\x1eMODEL_ARCHITECTURE_CLIP_RESNET\x10\x02\x12\x1a\n\x16MODEL_ARCHITECTURE_LDM\x10\x03*\xa2\x01\n\x06\x41\x63tion\x12\x16\n\x12\x41\x43TION_PASSTHROUGH\x10\x00\x12\x1f\n\x1b\x41\x43TION_REGENERATE_DUPLICATE\x10\x01\x12\x15\n\x11\x41\x43TION_REGENERATE\x10\x02\x12\x1e\n\x1a\x41\x43TION_OBFUSCATE_DUPLICATE\x10\x03\x12\x14\n\x10\x41\x43TION_OBFUSCATE\x10\x04\x12\x12\n\x0e\x41\x43TION_DISCARD\x10\x05*D\n\x0e\x43lassifierMode\x12\x17\n\x13\x43LSFR_MODE_ZEROSHOT\x10\x00\x12\x19\n\x15\x43LSFR_MODE_MULTICLASS\x10\x01*\x8c\x01\n\x0fInterpolateMode\x12\x16\n\x12INTERPOLATE_LINEAR\x10\x00\x12\x14\n\x10INTERPOLATE_RIFE\x10\x01\x12\x1a\n\x16INTERPOLATE_VAE_LINEAR\x10\x02\x12\x19\n\x15INTERPOLATE_VAE_SLERP\x10\x03\x12\x14\n\x10INTERPOLATE_FILM\x10\x04*l\n\nBorderMode\x12\x12\n\x0e\x42ORDER_REFLECT\x10\x00\x12\x14\n\x10\x42ORDER_REPLICATE\x10\x01\x12\x0f\n\x0b\x42ORDER_WRAP\x10\x02\x12\x0f\n\x0b\x42ORDER_ZERO\x10\x03\x12\x12\n\x0e\x42ORDER_PREFILL\x10\x04*O\n\x0e\x43olorMatchMode\x12\x13\n\x0f\x43OLOR_MATCH_HSV\x10\x00\x12\x13\n\x0f\x43OLOR_MATCH_LAB\x10\x01\x12\x13\n\x0f\x43OLOR_MATCH_RGB\x10\x02*=\n\nCameraType\x12\x16\n\x12\x43\x41MERA_PERSPECTIVE\x10\x00\x12\x17\n\x13\x43\x41MERA_ORTHOGRAPHIC\x10\x01*4\n\nRenderMode\x12\x0f\n\x0bRENDER_MESH\x10\x00\x12\x15\n\x11RENDER_POINTCLOUD\x10\x01*=\n\x0b\x41ssetAction\x12\r\n\tASSET_PUT\x10\x00\x12\r\n\tASSET_GET\x10\x01\x12\x10\n\x0c\x41SSET_DELETE\x10\x02*\x81\x01\n\x08\x41ssetUse\x12\x17\n\x13\x41SSET_USE_UNDEFINED\x10\x00\x12\x13\n\x0f\x41SSET_USE_INPUT\x10\x01\x12\x14\n\x10\x41SSET_USE_OUTPUT\x10\x02\x12\x1a\n\x16\x41SSET_USE_INTERMEDIATE\x10\x03\x12\x15\n\x11\x41SSET_USE_PROJECT\x10\x04*W\n\x0bStageAction\x12\x15\n\x11STAGE_ACTION_PASS\x10\x00\x12\x18\n\x14STAGE_ACTION_DISCARD\x10\x01\x12\x17\n\x13STAGE_ACTION_RETURN\x10\x02\x32\x83\x01\n\x11GenerationService\x12\x31\n\x08Generate\x12\x10.gooseai.Request\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x12;\n\rChainGenerate\x12\x15.gooseai.ChainRequest\x1a\x0f.gooseai.Answer\"\x00\x30\x01\x42;Z9github.com/stability-ai/api-interfaces/gooseai/generationb\x06proto3')
 
 _FINISHREASON = DESCRIPTOR.enum_types_by_name['FinishReason']
 FinishReason = enum_type_wrapper.EnumTypeWrapper(_FINISHREASON)
 _ARTIFACTTYPE = DESCRIPTOR.enum_types_by_name['ArtifactType']
 ArtifactType = enum_type_wrapper.EnumTypeWrapper(_ARTIFACTTYPE)
 _MASKEDAREAINIT = DESCRIPTOR.enum_types_by_name['MaskedAreaInit']
 MaskedAreaInit = enum_type_wrapper.EnumTypeWrapper(_MASKEDAREAINIT)
@@ -34,14 +35,24 @@
 GuidancePreset = enum_type_wrapper.EnumTypeWrapper(_GUIDANCEPRESET)
 _MODELARCHITECTURE = DESCRIPTOR.enum_types_by_name['ModelArchitecture']
 ModelArchitecture = enum_type_wrapper.EnumTypeWrapper(_MODELARCHITECTURE)
 _ACTION = DESCRIPTOR.enum_types_by_name['Action']
 Action = enum_type_wrapper.EnumTypeWrapper(_ACTION)
 _CLASSIFIERMODE = DESCRIPTOR.enum_types_by_name['ClassifierMode']
 ClassifierMode = enum_type_wrapper.EnumTypeWrapper(_CLASSIFIERMODE)
+_INTERPOLATEMODE = DESCRIPTOR.enum_types_by_name['InterpolateMode']
+InterpolateMode = enum_type_wrapper.EnumTypeWrapper(_INTERPOLATEMODE)
+_BORDERMODE = DESCRIPTOR.enum_types_by_name['BorderMode']
+BorderMode = enum_type_wrapper.EnumTypeWrapper(_BORDERMODE)
+_COLORMATCHMODE = DESCRIPTOR.enum_types_by_name['ColorMatchMode']
+ColorMatchMode = enum_type_wrapper.EnumTypeWrapper(_COLORMATCHMODE)
+_CAMERATYPE = DESCRIPTOR.enum_types_by_name['CameraType']
+CameraType = enum_type_wrapper.EnumTypeWrapper(_CAMERATYPE)
+_RENDERMODE = DESCRIPTOR.enum_types_by_name['RenderMode']
+RenderMode = enum_type_wrapper.EnumTypeWrapper(_RENDERMODE)
 _ASSETACTION = DESCRIPTOR.enum_types_by_name['AssetAction']
 AssetAction = enum_type_wrapper.EnumTypeWrapper(_ASSETACTION)
 _ASSETUSE = DESCRIPTOR.enum_types_by_name['AssetUse']
 AssetUse = enum_type_wrapper.EnumTypeWrapper(_ASSETUSE)
 _STAGEACTION = DESCRIPTOR.enum_types_by_name['StageAction']
 StageAction = enum_type_wrapper.EnumTypeWrapper(_STAGEACTION)
 NULL = 0
@@ -55,14 +66,15 @@
 ARTIFACT_TEXT = 3
 ARTIFACT_TOKENS = 4
 ARTIFACT_EMBEDDING = 5
 ARTIFACT_CLASSIFICATIONS = 6
 ARTIFACT_MASK = 7
 ARTIFACT_LATENT = 8
 ARTIFACT_TENSOR = 9
+ARTIFACT_DEPTH = 10
 MASKED_AREA_INIT_ZERO = 0
 MASKED_AREA_INIT_RANDOM = 1
 MASKED_AREA_INIT_ORIGINAL = 2
 TEXT_ENCODER = 0
 CROSS_ATTENTION = 1
 SAMPLER_DDIM = 0
 SAMPLER_DDPM = 1
@@ -70,14 +82,15 @@
 SAMPLER_K_EULER_ANCESTRAL = 3
 SAMPLER_K_HEUN = 4
 SAMPLER_K_DPM_2 = 5
 SAMPLER_K_DPM_2_ANCESTRAL = 6
 SAMPLER_K_LMS = 7
 SAMPLER_K_DPMPP_2S_ANCESTRAL = 8
 SAMPLER_K_DPMPP_2M = 9
+SAMPLER_K_DPMPP_SDE = 10
 UPSCALER_RGB = 0
 UPSCALER_GFPGAN = 1
 UPSCALER_ESRGAN = 2
 GUIDANCE_PRESET_NONE = 0
 GUIDANCE_PRESET_SIMPLE = 1
 GUIDANCE_PRESET_FAST_BLUE = 2
 GUIDANCE_PRESET_FAST_GREEN = 3
@@ -92,14 +105,31 @@
 ACTION_REGENERATE_DUPLICATE = 1
 ACTION_REGENERATE = 2
 ACTION_OBFUSCATE_DUPLICATE = 3
 ACTION_OBFUSCATE = 4
 ACTION_DISCARD = 5
 CLSFR_MODE_ZEROSHOT = 0
 CLSFR_MODE_MULTICLASS = 1
+INTERPOLATE_LINEAR = 0
+INTERPOLATE_RIFE = 1
+INTERPOLATE_VAE_LINEAR = 2
+INTERPOLATE_VAE_SLERP = 3
+INTERPOLATE_FILM = 4
+BORDER_REFLECT = 0
+BORDER_REPLICATE = 1
+BORDER_WRAP = 2
+BORDER_ZERO = 3
+BORDER_PREFILL = 4
+COLOR_MATCH_HSV = 0
+COLOR_MATCH_LAB = 1
+COLOR_MATCH_RGB = 2
+CAMERA_PERSPECTIVE = 0
+CAMERA_ORTHOGRAPHIC = 1
+RENDER_MESH = 0
+RENDER_POINTCLOUD = 1
 ASSET_PUT = 0
 ASSET_GET = 1
 ASSET_DELETE = 2
 ASSET_USE_UNDEFINED = 0
 ASSET_USE_INPUT = 1
 ASSET_USE_OUTPUT = 2
 ASSET_USE_INTERMEDIATE = 3
@@ -124,17 +154,26 @@
 _GUIDANCEINSTANCEPARAMETERS = DESCRIPTOR.message_types_by_name['GuidanceInstanceParameters']
 _GUIDANCEPARAMETERS = DESCRIPTOR.message_types_by_name['GuidanceParameters']
 _TRANSFORMTYPE = DESCRIPTOR.message_types_by_name['TransformType']
 _IMAGEPARAMETERS = DESCRIPTOR.message_types_by_name['ImageParameters']
 _CLASSIFIERCONCEPT = DESCRIPTOR.message_types_by_name['ClassifierConcept']
 _CLASSIFIERCATEGORY = DESCRIPTOR.message_types_by_name['ClassifierCategory']
 _CLASSIFIERPARAMETERS = DESCRIPTOR.message_types_by_name['ClassifierParameters']
+_INTERPOLATEPARAMETERS = DESCRIPTOR.message_types_by_name['InterpolateParameters']
+_TRANSFORMCOLORADJUST = DESCRIPTOR.message_types_by_name['TransformColorAdjust']
+_TRANSFORMDEPTHCALC = DESCRIPTOR.message_types_by_name['TransformDepthCalc']
+_TRANSFORMMATRIX = DESCRIPTOR.message_types_by_name['TransformMatrix']
+_TRANSFORMRESAMPLE = DESCRIPTOR.message_types_by_name['TransformResample']
+_CAMERAPARAMETERS = DESCRIPTOR.message_types_by_name['CameraParameters']
+_TRANSFORMCAMERAPOSE = DESCRIPTOR.message_types_by_name['TransformCameraPose']
+_TRANSFORMPARAMETERS = DESCRIPTOR.message_types_by_name['TransformParameters']
 _ASSETPARAMETERS = DESCRIPTOR.message_types_by_name['AssetParameters']
 _ANSWERMETA = DESCRIPTOR.message_types_by_name['AnswerMeta']
 _ANSWER = DESCRIPTOR.message_types_by_name['Answer']
+_ANSWERBATCH = DESCRIPTOR.message_types_by_name['AnswerBatch']
 _REQUEST = DESCRIPTOR.message_types_by_name['Request']
 _ONSTATUS = DESCRIPTOR.message_types_by_name['OnStatus']
 _STAGE = DESCRIPTOR.message_types_by_name['Stage']
 _CHAINREQUEST = DESCRIPTOR.message_types_by_name['ChainRequest']
 Token = _reflection.GeneratedProtocolMessageType('Token', (_message.Message,), {
   'DESCRIPTOR' : _TOKEN,
   '__module__' : 'generation_pb2'
@@ -264,14 +303,70 @@
 ClassifierParameters = _reflection.GeneratedProtocolMessageType('ClassifierParameters', (_message.Message,), {
   'DESCRIPTOR' : _CLASSIFIERPARAMETERS,
   '__module__' : 'generation_pb2'
   # @@protoc_insertion_point(class_scope:gooseai.ClassifierParameters)
   })
 _sym_db.RegisterMessage(ClassifierParameters)
 
+InterpolateParameters = _reflection.GeneratedProtocolMessageType('InterpolateParameters', (_message.Message,), {
+  'DESCRIPTOR' : _INTERPOLATEPARAMETERS,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.InterpolateParameters)
+  })
+_sym_db.RegisterMessage(InterpolateParameters)
+
+TransformColorAdjust = _reflection.GeneratedProtocolMessageType('TransformColorAdjust', (_message.Message,), {
+  'DESCRIPTOR' : _TRANSFORMCOLORADJUST,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.TransformColorAdjust)
+  })
+_sym_db.RegisterMessage(TransformColorAdjust)
+
+TransformDepthCalc = _reflection.GeneratedProtocolMessageType('TransformDepthCalc', (_message.Message,), {
+  'DESCRIPTOR' : _TRANSFORMDEPTHCALC,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.TransformDepthCalc)
+  })
+_sym_db.RegisterMessage(TransformDepthCalc)
+
+TransformMatrix = _reflection.GeneratedProtocolMessageType('TransformMatrix', (_message.Message,), {
+  'DESCRIPTOR' : _TRANSFORMMATRIX,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.TransformMatrix)
+  })
+_sym_db.RegisterMessage(TransformMatrix)
+
+TransformResample = _reflection.GeneratedProtocolMessageType('TransformResample', (_message.Message,), {
+  'DESCRIPTOR' : _TRANSFORMRESAMPLE,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.TransformResample)
+  })
+_sym_db.RegisterMessage(TransformResample)
+
+CameraParameters = _reflection.GeneratedProtocolMessageType('CameraParameters', (_message.Message,), {
+  'DESCRIPTOR' : _CAMERAPARAMETERS,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.CameraParameters)
+  })
+_sym_db.RegisterMessage(CameraParameters)
+
+TransformCameraPose = _reflection.GeneratedProtocolMessageType('TransformCameraPose', (_message.Message,), {
+  'DESCRIPTOR' : _TRANSFORMCAMERAPOSE,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.TransformCameraPose)
+  })
+_sym_db.RegisterMessage(TransformCameraPose)
+
+TransformParameters = _reflection.GeneratedProtocolMessageType('TransformParameters', (_message.Message,), {
+  'DESCRIPTOR' : _TRANSFORMPARAMETERS,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.TransformParameters)
+  })
+_sym_db.RegisterMessage(TransformParameters)
+
 AssetParameters = _reflection.GeneratedProtocolMessageType('AssetParameters', (_message.Message,), {
   'DESCRIPTOR' : _ASSETPARAMETERS,
   '__module__' : 'generation_pb2'
   # @@protoc_insertion_point(class_scope:gooseai.AssetParameters)
   })
 _sym_db.RegisterMessage(AssetParameters)
 
@@ -285,14 +380,21 @@
 Answer = _reflection.GeneratedProtocolMessageType('Answer', (_message.Message,), {
   'DESCRIPTOR' : _ANSWER,
   '__module__' : 'generation_pb2'
   # @@protoc_insertion_point(class_scope:gooseai.Answer)
   })
 _sym_db.RegisterMessage(Answer)
 
+AnswerBatch = _reflection.GeneratedProtocolMessageType('AnswerBatch', (_message.Message,), {
+  'DESCRIPTOR' : _ANSWERBATCH,
+  '__module__' : 'generation_pb2'
+  # @@protoc_insertion_point(class_scope:gooseai.AnswerBatch)
+  })
+_sym_db.RegisterMessage(AnswerBatch)
+
 Request = _reflection.GeneratedProtocolMessageType('Request', (_message.Message,), {
   'DESCRIPTOR' : _REQUEST,
   '__module__' : 'generation_pb2'
   # @@protoc_insertion_point(class_scope:gooseai.Request)
   })
 _sym_db.RegisterMessage(Request)
 
@@ -317,89 +419,119 @@
   })
 _sym_db.RegisterMessage(ChainRequest)
 
 _GENERATIONSERVICE = DESCRIPTOR.services_by_name['GenerationService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\r./;generation'
-  _FINISHREASON._serialized_start=4542
-  _FINISHREASON._serialized_end=4611
-  _ARTIFACTTYPE._serialized_start=4614
-  _ARTIFACTTYPE._serialized_end=4842
-  _MASKEDAREAINIT._serialized_start=4844
-  _MASKEDAREAINIT._serialized_end=4947
-  _WEIGHTMETHOD._serialized_start=4949
-  _WEIGHTMETHOD._serialized_end=5002
-  _DIFFUSIONSAMPLER._serialized_start=5005
-  _DIFFUSIONSAMPLER._serialized_end=5260
-  _UPSCALER._serialized_start=5262
-  _UPSCALER._serialized_end=5332
-  _GUIDANCEPRESET._serialized_start=5335
-  _GUIDANCEPRESET._serialized_end=5551
-  _MODELARCHITECTURE._serialized_start=5554
-  _MODELARCHITECTURE._serialized_end=5699
-  _ACTION._serialized_start=5702
-  _ACTION._serialized_end=5864
-  _CLASSIFIERMODE._serialized_start=5866
-  _CLASSIFIERMODE._serialized_end=5934
-  _ASSETACTION._serialized_start=5936
-  _ASSETACTION._serialized_end=5997
-  _ASSETUSE._serialized_start=6000
-  _ASSETUSE._serialized_end=6129
-  _STAGEACTION._serialized_start=6131
-  _STAGEACTION._serialized_end=6218
-  _TOKEN._serialized_start=44
-  _TOKEN._serialized_end=91
-  _TOKENS._serialized_start=93
-  _TOKENS._serialized_end=177
-  _ARTIFACT._serialized_start=180
-  _ARTIFACT._serialized_end=551
-  _PROMPTPARAMETERS._serialized_start=553
-  _PROMPTPARAMETERS._serialized_end=631
-  _PROMPT._serialized_start=634
-  _PROMPT._serialized_end=809
-  _SAMPLERPARAMETERS._serialized_start=812
-  _SAMPLERPARAMETERS._serialized_end=1103
-  _CONDITIONERPARAMETERS._serialized_start=1106
-  _CONDITIONERPARAMETERS._serialized_end=1245
-  _SCHEDULEPARAMETERS._serialized_start=1247
-  _SCHEDULEPARAMETERS._serialized_end=1353
-  _STEPPARAMETER._serialized_start=1356
-  _STEPPARAMETER._serialized_end=1584
-  _MODEL._serialized_start=1587
-  _MODEL._serialized_end=1738
-  _CUTOUTPARAMETERS._serialized_start=1741
-  _CUTOUTPARAMETERS._serialized_end=1929
-  _GUIDANCESCHEDULEPARAMETERS._serialized_start=1931
-  _GUIDANCESCHEDULEPARAMETERS._serialized_end=1992
-  _GUIDANCEINSTANCEPARAMETERS._serialized_start=1995
-  _GUIDANCEINSTANCEPARAMETERS._serialized_end=2274
-  _GUIDANCEPARAMETERS._serialized_start=2276
-  _GUIDANCEPARAMETERS._serialized_end=2402
-  _TRANSFORMTYPE._serialized_start=2404
-  _TRANSFORMTYPE._serialized_end=2514
-  _IMAGEPARAMETERS._serialized_start=2517
-  _IMAGEPARAMETERS._serialized_end=2857
-  _CLASSIFIERCONCEPT._serialized_start=2859
-  _CLASSIFIERCONCEPT._serialized_end=2933
-  _CLASSIFIERCATEGORY._serialized_start=2936
-  _CLASSIFIERCATEGORY._serialized_end=3180
-  _CLASSIFIERPARAMETERS._serialized_start=3183
-  _CLASSIFIERPARAMETERS._serialized_end=3367
-  _ASSETPARAMETERS._serialized_start=3369
-  _ASSETPARAMETERS._serialized_end=3476
-  _ANSWERMETA._serialized_start=3479
-  _ANSWERMETA._serialized_end=3627
-  _ANSWER._serialized_start=3630
-  _ANSWER._serialized_end=3799
-  _REQUEST._serialized_start=3802
-  _REQUEST._serialized_end=4258
-  _ONSTATUS._serialized_start=4260
-  _ONSTATUS._serialized_end=4379
-  _STAGE._serialized_start=4381
-  _STAGE._serialized_end=4473
-  _CHAINREQUEST._serialized_start=4475
-  _CHAINREQUEST._serialized_end=4540
-  _GENERATIONSERVICE._serialized_start=6221
-  _GENERATIONSERVICE._serialized_end=6352
+  DESCRIPTOR._serialized_options = b'Z9github.com/stability-ai/api-interfaces/gooseai/generation'
+  _TRANSFORMMATRIX.fields_by_name['data']._options = None
+  _TRANSFORMMATRIX.fields_by_name['data']._serialized_options = b'\020\001'
+  _FINISHREASON._serialized_start=6454
+  _FINISHREASON._serialized_end=6523
+  _ARTIFACTTYPE._serialized_start=6526
+  _ARTIFACTTYPE._serialized_end=6774
+  _MASKEDAREAINIT._serialized_start=6776
+  _MASKEDAREAINIT._serialized_end=6879
+  _WEIGHTMETHOD._serialized_start=6881
+  _WEIGHTMETHOD._serialized_end=6934
+  _DIFFUSIONSAMPLER._serialized_start=6937
+  _DIFFUSIONSAMPLER._serialized_end=7217
+  _UPSCALER._serialized_start=7219
+  _UPSCALER._serialized_end=7289
+  _GUIDANCEPRESET._serialized_start=7292
+  _GUIDANCEPRESET._serialized_end=7508
+  _MODELARCHITECTURE._serialized_start=7511
+  _MODELARCHITECTURE._serialized_end=7656
+  _ACTION._serialized_start=7659
+  _ACTION._serialized_end=7821
+  _CLASSIFIERMODE._serialized_start=7823
+  _CLASSIFIERMODE._serialized_end=7891
+  _INTERPOLATEMODE._serialized_start=7894
+  _INTERPOLATEMODE._serialized_end=8034
+  _BORDERMODE._serialized_start=8036
+  _BORDERMODE._serialized_end=8144
+  _COLORMATCHMODE._serialized_start=8146
+  _COLORMATCHMODE._serialized_end=8225
+  _CAMERATYPE._serialized_start=8227
+  _CAMERATYPE._serialized_end=8288
+  _RENDERMODE._serialized_start=8290
+  _RENDERMODE._serialized_end=8342
+  _ASSETACTION._serialized_start=8344
+  _ASSETACTION._serialized_end=8405
+  _ASSETUSE._serialized_start=8408
+  _ASSETUSE._serialized_end=8537
+  _STAGEACTION._serialized_start=8539
+  _STAGEACTION._serialized_end=8626
+  _TOKEN._serialized_start=74
+  _TOKEN._serialized_end=121
+  _TOKENS._serialized_start=123
+  _TOKENS._serialized_end=207
+  _ARTIFACT._serialized_start=210
+  _ARTIFACT._serialized_end=581
+  _PROMPTPARAMETERS._serialized_start=583
+  _PROMPTPARAMETERS._serialized_end=661
+  _PROMPT._serialized_start=664
+  _PROMPT._serialized_end=839
+  _SAMPLERPARAMETERS._serialized_start=842
+  _SAMPLERPARAMETERS._serialized_end=1185
+  _CONDITIONERPARAMETERS._serialized_start=1188
+  _CONDITIONERPARAMETERS._serialized_end=1327
+  _SCHEDULEPARAMETERS._serialized_start=1329
+  _SCHEDULEPARAMETERS._serialized_end=1435
+  _STEPPARAMETER._serialized_start=1438
+  _STEPPARAMETER._serialized_end=1666
+  _MODEL._serialized_start=1669
+  _MODEL._serialized_end=1820
+  _CUTOUTPARAMETERS._serialized_start=1823
+  _CUTOUTPARAMETERS._serialized_end=2011
+  _GUIDANCESCHEDULEPARAMETERS._serialized_start=2013
+  _GUIDANCESCHEDULEPARAMETERS._serialized_end=2074
+  _GUIDANCEINSTANCEPARAMETERS._serialized_start=2077
+  _GUIDANCEINSTANCEPARAMETERS._serialized_end=2356
+  _GUIDANCEPARAMETERS._serialized_start=2358
+  _GUIDANCEPARAMETERS._serialized_end=2484
+  _TRANSFORMTYPE._serialized_start=2486
+  _TRANSFORMTYPE._serialized_end=2596
+  _IMAGEPARAMETERS._serialized_start=2599
+  _IMAGEPARAMETERS._serialized_end=3044
+  _CLASSIFIERCONCEPT._serialized_start=3046
+  _CLASSIFIERCONCEPT._serialized_end=3120
+  _CLASSIFIERCATEGORY._serialized_start=3123
+  _CLASSIFIERCATEGORY._serialized_end=3367
+  _CLASSIFIERPARAMETERS._serialized_start=3370
+  _CLASSIFIERPARAMETERS._serialized_end=3554
+  _INTERPOLATEPARAMETERS._serialized_start=3556
+  _INTERPOLATEPARAMETERS._serialized_end=3649
+  _TRANSFORMCOLORADJUST._serialized_start=3652
+  _TRANSFORMCOLORADJUST._serialized_end=4064
+  _TRANSFORMDEPTHCALC._serialized_start=4067
+  _TRANSFORMDEPTHCALC._serialized_end=4207
+  _TRANSFORMMATRIX._serialized_start=4209
+  _TRANSFORMMATRIX._serialized_end=4244
+  _TRANSFORMRESAMPLE._serialized_start=4247
+  _TRANSFORMRESAMPLE._serialized_end=4509
+  _CAMERAPARAMETERS._serialized_start=4511
+  _CAMERAPARAMETERS._serialized_end=4636
+  _TRANSFORMCAMERAPOSE._serialized_start=4639
+  _TRANSFORMCAMERAPOSE._serialized_end=4897
+  _TRANSFORMPARAMETERS._serialized_start=4900
+  _TRANSFORMPARAMETERS._serialized_end=5141
+  _ASSETPARAMETERS._serialized_start=5143
+  _ASSETPARAMETERS._serialized_end=5250
+  _ANSWERMETA._serialized_start=5253
+  _ANSWERMETA._serialized_end=5401
+  _ANSWER._serialized_start=5404
+  _ANSWER._serialized_end=5573
+  _ANSWERBATCH._serialized_start=5575
+  _ANSWERBATCH._serialized_end=5640
+  _REQUEST._serialized_start=5643
+  _REQUEST._serialized_end=6170
+  _ONSTATUS._serialized_start=6172
+  _ONSTATUS._serialized_end=6291
+  _STAGE._serialized_start=6293
+  _STAGE._serialized_end=6385
+  _CHAINREQUEST._serialized_start=6387
+  _CHAINREQUEST._serialized_end=6452
+  _GENERATIONSERVICE._serialized_start=8629
+  _GENERATIONSERVICE._serialized_end=8760
 # @@protoc_insertion_point(module_scope)
```

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/generation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/generation/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/gooseai/project/project_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,14 +38,24 @@
                 response_deserializer=project__pb2.Project.FromString,
                 )
         self.Delete = channel.unary_unary(
                 '/gooseai.ProjectService/Delete',
                 request_serializer=project__pb2.DeleteProjectRequest.SerializeToString,
                 response_deserializer=project__pb2.Project.FromString,
                 )
+        self.QueryAssets = channel.unary_unary(
+                '/gooseai.ProjectService/QueryAssets',
+                request_serializer=project__pb2.QueryAssetsRequest.SerializeToString,
+                response_deserializer=project__pb2.QueryAssetsResponse.FromString,
+                )
+        self.DeleteAssets = channel.unary_unary(
+                '/gooseai.ProjectService/DeleteAssets',
+                request_serializer=project__pb2.DeleteAssetsRequest.SerializeToString,
+                response_deserializer=project__pb2.DeleteAssetsResponse.FromString,
+                )
 
 
 class ProjectServiceServicer(object):
     """
     gRPC services
 
     """
@@ -81,14 +91,28 @@
     def Delete(self, request, context):
         """Delete a project
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def QueryAssets(self, request, context):
+        """Query the assets of a project, with additional filtering
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteAssets(self, request, context):
+        """Delete one or more assets of a project
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_ProjectServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Create': grpc.unary_unary_rpc_method_handler(
                     servicer.Create,
                     request_deserializer=project__pb2.CreateProjectRequest.FromString,
                     response_serializer=project__pb2.Project.SerializeToString,
@@ -109,14 +133,24 @@
                     response_serializer=project__pb2.Project.SerializeToString,
             ),
             'Delete': grpc.unary_unary_rpc_method_handler(
                     servicer.Delete,
                     request_deserializer=project__pb2.DeleteProjectRequest.FromString,
                     response_serializer=project__pb2.Project.SerializeToString,
             ),
+            'QueryAssets': grpc.unary_unary_rpc_method_handler(
+                    servicer.QueryAssets,
+                    request_deserializer=project__pb2.QueryAssetsRequest.FromString,
+                    response_serializer=project__pb2.QueryAssetsResponse.SerializeToString,
+            ),
+            'DeleteAssets': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteAssets,
+                    request_deserializer=project__pb2.DeleteAssetsRequest.FromString,
+                    response_serializer=project__pb2.DeleteAssetsResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'gooseai.ProjectService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -206,7 +240,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/gooseai.ProjectService/Delete',
             project__pb2.DeleteProjectRequest.SerializeToString,
             project__pb2.Project.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def QueryAssets(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/gooseai.ProjectService/QueryAssets',
+            project__pb2.QueryAssetsRequest.SerializeToString,
+            project__pb2.QueryAssetsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteAssets(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/gooseai.ProjectService/DeleteAssets',
+            project__pb2.DeleteAssetsRequest.SerializeToString,
+            project__pb2.DeleteAssetsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/tensors/tensors_pb2.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py` & `stability-sdk-0.5.0/src/stability_sdk/interfaces/src/tensorizer/test_tensorizer.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/src/stability_sdk/utils.py` & `stability-sdk-0.5.0/src/stability_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/src/stability_sdk.egg-info/PKG-INFO` & `stability-sdk-0.5.0/src/stability_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: stability-sdk
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python SDK for interacting with stability.ai APIs
 Home-page: https://beta.dreamstudio.ai/
 Download-URL: https://github.com/Stability-AI/stability-sdk/
-Author: Wes Brown
-Author-email: wesbrown18@gmail.com
-Maintainer: David Marx
-Maintainer-email: david@stability.ai
+Author: Stability AI
+Author-email: support@stability.ai
+Maintainer: Stability AI
+Maintainer-email: support@stability.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Education
@@ -31,26 +31,27 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # stability-sdk
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/stability-ai/stability-sdk/blob/main/nbs/demo_colab.ipynb)
 
-Client implementations that interact with the Stability Generator API
+Client implementations that interact with the Stability API. 
 
-# Installation
+## Getting an API key
 
-Install the PyPI package via:
+Follow the [instructions](https://platform.stability.ai/docs/getting-started/authentication) on [Platform](https://platform.stability.ai) to obtain an API key.
 
-`pip install stability-sdk`
+## PyPI Package Installation
+
+Install the [PyPI](https://pypi.org/project/stability-sdk/) package via:
 
-# Getting an API key
-You can manage API keys in your dreamstudio account [here](https://beta.dreamstudio.ai/membership?tab=apiKeys)
+`pip install stability-sdk`
 
-# Python client
+## Python Client
 
 `client.py` is both a command line client and an API class that wraps the gRPC based API. To try the client:
 
 - Use Python venv: `python3 -m venv pyenv`
 - Set up in venv dependencies: `pyenv/bin/pip3 install -e .`
 - `pyenv/bin/activate` to use the venv.
 - Set the `STABILITY_HOST` environment variable. This is by default set to the production endpoint `grpc.stability.ai:443`.
@@ -63,15 +64,15 @@
 It will generate and put PNGs in your current directory.
 
 To upscale:
 `python3 -m stability_sdk upscale -i "/path/to/image.png"`
 
 ## SDK Usage
 
-See usage demo notebooks in ./nbs
+Be sure to check out [Platform](https://platform.stability.ai) for comprehensive documentation on how to interact with our API.
 
 ## Command line usage
 
 ```
 usage: python -m stability_sdk generate [-h] [--height HEIGHT] [--width WIDTH] [--start_schedule START_SCHEDULE]
                  [--end_schedule END_SCHEDULE] [--cfg_scale CFG_SCALE] [--sampler SAMPLER]
                  [--steps STEPS] [--seed SEED] [--prefix PREFIX] [--engine ENGINE]
@@ -141,26 +142,21 @@
   --engine ENGINE, -e ENGINE
                         engine to use for upscale
 ```
 
 
 ## Connecting to the API using languages other than Python
 
-The `src` subdirectory contains pre-compiled gRPC stubs for the following languages:
-
-- [Javascript/Typescript](https://github.com/Stability-AI/stability-sdk/tree/main/src/js)
-
-If a language you would like to connect to the API with is not listed above, you can use the following
+If a language you would like to connect to the API with is not currently documented on [Platform](https://platform.stability.ai) you can use the following
 protobuf definition to compile stubs for your language:
 
 - [protobuf spec](https://github.com/Stability-AI/api-interfaces/blob/main/src/proto/)
 
 ## Community-contributed clients
 
 * Typescript client: https://github.com/jakiestfu/stability-ts
 * Guide to building for Ruby: https://github.com/kmcphillips/stability-sdk/blob/main/src/ruby/README.md
 
-## DreamStudio API TOS
-
-Unless otherwise specified, usage of the dreamstudio API falls under the same usage terms as the dreamstudio web interface: 
+## Stability API TOS
 
-* https://beta.dreamstudio.ai/terms-of-service
+Usage of the Stability API falls under the [STABILITY AI API Terms of Service.
+](https://platform.stability.ai/docs/terms-of-service)
```

### Comparing `stability-sdk-0.4.0/src/stability_sdk.egg-info/SOURCES.txt` & `stability-sdk-0.5.0/src/stability_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/tests/test_client.py` & `stability-sdk-0.5.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `stability-sdk-0.4.0/tests/test_utils.py` & `stability-sdk-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

