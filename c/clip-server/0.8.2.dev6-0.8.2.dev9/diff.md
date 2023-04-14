# Comparing `tmp/clip-server-0.8.2.dev6.tar.gz` & `tmp/clip-server-0.8.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clip-server-0.8.2.dev6.tar", last modified: Tue Nov 29 06:53:26 2022, max compression
+gzip compressed data, was "clip-server-0.8.2.dev9.tar", last modified: Wed Dec  7 07:23:08 2022, max compression
```

## Comparing `clip-server-0.8.2.dev6.tar` & `clip-server-0.8.2.dev9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:53:26.427405 clip-server-0.8.2.dev6/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    31434 2022-11-29 06:53:26.427405 clip-server-0.8.2.dev6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:53:26.423404 clip-server-0.8.2.dev6/clip_server/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2022-11-29 06:53:22.000000 clip-server-0.8.2.dev6/clip_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      605 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:53:26.423404 clip-server-0.8.2.dev6/clip_server/executors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6846 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/executors/clip_onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)     5671 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/executors/clip_tensorrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     6648 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/executors/clip_torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3693 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/executors/helper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:53:26.427405 clip-server-0.8.2.dev6/clip_server/model/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/clip.py
--rw-r--r--   0 runner    (1001) docker     (122)     1634 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/clip_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    12134 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/clip_onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/clip_trt.py
--rw-r--r--   0 runner    (1001) docker     (122)     3549 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (122)     2592 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/mclip_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    19706 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1992 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/openclip_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     8295 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/pretrained_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     4958 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/simple_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (122)    11395 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/model/trt_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      227 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/onnx-flow.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:53:26.427405 clip-server-0.8.2.dev6/clip_server/resources/
--rw-r--r--   0 runner    (1001) docker     (122)  1356917 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/resources/bpe_simple_vocab_16e6.txt.gz
--rw-r--r--   0 runner    (1001) docker     (122)      231 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/tensorrt-flow.yml
--rw-r--r--   0 runner    (1001) docker     (122)      228 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/clip_server/torch-flow.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:53:26.423404 clip-server-0.8.2.dev6/clip_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    31434 2022-11-29 06:53:26.000000 clip-server-0.8.2.dev6/clip_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2022-11-29 06:53:26.000000 clip-server-0.8.2.dev6/clip_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:53:26.000000 clip-server-0.8.2.dev6/clip_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:53:26.000000 clip-server-0.8.2.dev6/clip_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      246 2022-11-29 06:53:26.000000 clip-server-0.8.2.dev6/clip_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-29 06:53:26.000000 clip-server-0.8.2.dev6/clip_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 06:53:26.427405 clip-server-0.8.2.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3410 2022-11-29 06:53:14.000000 clip-server-0.8.2.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:23:08.604458 clip-server-0.8.2.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25311 2022-12-07 07:23:08.604458 clip-server-0.8.2.dev9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:23:08.600458 clip-server-0.8.2.dev9/clip_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-07 07:23:05.000000 clip-server-0.8.2.dev9/clip_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:23:08.600458 clip-server-0.8.2.dev9/clip_server/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/executors/clip_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/executors/clip_tensorrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9114 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/executors/clip_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/executors/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:23:08.604458 clip-server-0.8.2.dev9/clip_server/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/clip_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/clip_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/clip_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/mclip_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19757 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/openclip_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/pretrained_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/simple_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/model/trt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/onnx-flow.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:23:08.604458 clip-server-0.8.2.dev9/clip_server/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)  1356917 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/resources/bpe_simple_vocab_16e6.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/tensorrt-flow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/clip_server/torch-flow.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 07:23:08.600458 clip-server-0.8.2.dev9/clip_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25311 2022-12-07 07:23:08.000000 clip-server-0.8.2.dev9/clip_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-12-07 07:23:08.000000 clip-server-0.8.2.dev9/clip_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 07:23:08.000000 clip-server-0.8.2.dev9/clip_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 07:23:08.000000 clip-server-0.8.2.dev9/clip_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-07 07:23:08.000000 clip-server-0.8.2.dev9/clip_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-07 07:23:08.000000 clip-server-0.8.2.dev9/clip_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-07 07:23:08.604458 clip-server-0.8.2.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2022-12-07 07:23:01.000000 clip-server-0.8.2.dev9/setup.py
```

### Comparing `clip-server-0.8.2.dev6/PKG-INFO` & `clip-server-0.8.2.dev9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,784 +1,19 @@
 Metadata-Version: 2.1
 Name: clip-server
-Version: 0.8.2.dev6
+Version: 0.8.2.dev9
 Summary: Embed images and sentences into fixed-length vectors via CLIP
 Home-page: https://github.com/jina-ai/clip-as-service
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/clip-as-service/tags
 Project-URL: Documentation, https://clip-as-service.jina.ai
 Project-URL: Source, https://github.com/jina-ai/clip-as-service/
 Project-URL: Tracker, https://github.com/jina-ai/clip-as-service/issues
-Description: <p align="center">
-        <br>
-        <br>
-        <br>
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/docs/_static/logo-light.svg?raw=true" alt="CLIP-as-service logo: The data structure for unstructured data" width="200px">
-        <br>
-        <br>
-        <br>
-        <b>Embed images and sentences into fixed-length vectors with CLIP</b>
-        </p>
-        
-        <p align=center>
-        <a href="https://pypi.org/project/clip_server/"><img alt="PyPI" src="https://img.shields.io/pypi/v/clip_server?label=Release&style=flat-square"></a>
-        <a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-3.1k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
-        <a href="https://codecov.io/gh/jina-ai/clip-as-service"><img alt="Codecov branch" src="https://img.shields.io/codecov/c/github/jina-ai/clip-as-service/main?logo=Codecov&logoColor=white&style=flat-square"></a>
-        <a href="https://colab.research.google.com/github/jina-ai/clip-as-service/blob/main/docs/hosting/cas-on-colab.ipynb"><img src="https://img.shields.io/badge/Host-on%20Google%20Colab%20(GPU/TPU)-brightgreen?style=flat-square&logo=googlecolab&&logoColor=white" alt="Host on Google Colab with GPU/TPU support"></a>
-        </p>
-        
-        <!-- start elevator-pitch -->
-        
-        CLIP-as-service is a low-latency high-scalability service for embedding images and text. It can be easily integrated as a microservice into neural search solutions.
-        
-        ⚡ **Fast**: Serve CLIP models with TensorRT, ONNX runtime and PyTorch w/o JIT with 800QPS<sup>[*]</sup>. Non-blocking duplex streaming on requests and responses, designed for large data and long-running tasks. 
-        
-        🫐 **Elastic**: Horizontally scale up and down multiple CLIP models on single GPU, with automatic load balancing.
-        
-        🐥 **Easy-to-use**: No learning curve, minimalist design on client and server. Intuitive and consistent API for image and sentence embedding. 
-        
-        👒 **Modern**: Async client support. Easily switch between gRPC, HTTP, WebSocket protocols with TLS and compression.
-        
-        🍱 **Integration**: Smooth integration with neural search ecosystem including [Jina](https://github.com/jina-ai/jina) and [DocArray](https://github.com/jina-ai/docarray). Build cross-modal and multi-modal solutions in no time. 
-        
-        <sup>[*] with default config (single replica, PyTorch no JIT) on GeForce RTX 3090. </sup>
-        
-        <!-- end elevator-pitch -->
-        
-        ## Try it!
-        
-        An always-online server `api.clip.jina.ai` loaded with `ViT-L-14-336::openai` is there for you to play & test.
-        Before you start, make sure you have obtained an access token from our [console website](https://console.clip.jina.ai/get_started), 
-        or via CLI as described in [this guide](https://docs.jina.ai/jina-ai-cloud/login/#create-a-new-pat).
-        
-        ```bash 
-        jina auth token create <name of PAT> -e <expiration days>
-        ```
-        
-        Then, you need to configure the access token in the parameter `credential` of the client in python or set it in the HTTP request header `Authorization` as `<your access token>`.
-        
-        ⚠️ Our demo server `demo-cas.jina.ai` is sunset and no longer available after **15th of Sept 2022**. 
-        
-        
-        ### Text & image embedding
-        
-        <table>
-        <tr>
-        <td> via HTTPS 🔐 </td>
-        <td> via gRPC 🔐⚡⚡ </td>
-        </tr>
-        <tr>
-        <td>
-        
-        ```bash
-        curl \
-        -X POST https://api.clip.jina.ai:8443/post \
-        -H 'Content-Type: application/json' \
-        -H 'Authorization: <your access token>' \
-        -d '{"data":[{"text": "First do it"}, 
-            {"text": "then do it right"}, 
-            {"text": "then do it better"}, 
-            {"uri": "https://picsum.photos/200"}], 
-            "execEndpoint":"/"}'
-        ```
-        
-        </td>
-        <td>
-        
-        ```python
-        # pip install clip-client
-        from clip_client import Client
-        
-        c = Client(
-            'grpcs://api.clip.jina.ai:2096', credential={'Authorization': '<your access token>'}
-        )
-        
-        r = c.encode(
-            [
-                'First do it',
-                'then do it right',
-                'then do it better',
-                'https://picsum.photos/200',
-            ]
-        )
-        print(r)
-        ```
-        </td>
-        </tr>
-        </table>
-        
-        ### Visual reasoning
-        
-        There are four basic visual reasoning skills: object recognition, object counting, color recognition, and spatial relation understanding. Let's try some:
-        
-        > You need to install [`jq` (a JSON processor)](https://stedolan.github.io/jq/) to prettify the results.
-        
-        <table>
-        <tr>
-        <td> Image </td>
-        <td> via HTTPS 🔐 </td>
-        </tr>
-        <tr>
-        <td>
-        <img src="https://picsum.photos/id/1/300/300">
-        </td>
-        <td>
-        
-        ```bash
-        curl \
-        -X POST https://api.clip.jina.ai:8443/post \
-        -H 'Content-Type: application/json' \
-        -H 'Authorization: <your access token>' \
-        -d '{"data":[{"uri": "https://picsum.photos/id/1/300/300",
-        "matches": [{"text": "there is a woman in the photo"},
-                    {"text": "there is a man in the photo"}]}],
-                    "execEndpoint":"/rank"}' \
-        | jq ".data[].matches[] | (.text, .scores.clip_score.value)"
-        ```
-        
-        gives:
-        
-        ```
-        "there is a woman in the photo"
-        0.626907229423523
-        "there is a man in the photo"
-        0.37309277057647705
-        ```
-        
-        </td>
-        </tr>
-        <tr>
-        <td>
-        <img src="https://picsum.photos/id/133/300/300">
-        </td>
-        <td>
-        
-        ```bash
-        curl \
-        -X POST https://api.clip.jina.ai:8443/post \
-        -H 'Content-Type: application/json' \
-        -H 'Authorization: <your access token>' \
-        -d '{"data":[{"uri": "https://picsum.photos/id/133/300/300",
-        "matches": [
-        {"text": "the blue car is on the left, the red car is on the right"},
-        {"text": "the blue car is on the right, the red car is on the left"},
-        {"text": "the blue car is on top of the red car"},
-        {"text": "the blue car is below the red car"}]}],
-        "execEndpoint":"/rank"}' \
-        | jq ".data[].matches[] | (.text, .scores.clip_score.value)"
-        ```
-        
-        gives:
-        ```
-        "the blue car is on the left, the red car is on the right"
-        0.5232442617416382
-        "the blue car is on the right, the red car is on the left"
-        0.32878655195236206
-        "the blue car is below the red car"
-        0.11064132302999496
-        "the blue car is on top of the red car"
-        0.03732786327600479
-        ```
-        
-        </td>
-        </tr>
-        
-        
-        <tr>
-        <td>
-        <img src="https://picsum.photos/id/102/300/300">
-        </td>
-        <td>
-        
-        ```bash
-        curl \
-        -X POST https://api.clip.jina.ai:8443/post \
-        -H 'Content-Type: application/json' \
-        -H 'Authorization: <your access token>' \
-        -d '{"data":[{"uri": "https://picsum.photos/id/102/300/300",
-        "matches": [{"text": "this is a photo of one berry"},
-                    {"text": "this is a photo of two berries"},
-                    {"text": "this is a photo of three berries"},
-                    {"text": "this is a photo of four berries"},
-                    {"text": "this is a photo of five berries"},
-                    {"text": "this is a photo of six berries"}]}],
-                    "execEndpoint":"/rank"}' \
-        | jq ".data[].matches[] | (.text, .scores.clip_score.value)"
-        ```
-        
-        gives:
-        ```
-        "this is a photo of three berries"
-        0.48507222533226013
-        "this is a photo of four berries"
-        0.2377079576253891
-        "this is a photo of one berry"
-        0.11304923892021179
-        "this is a photo of five berries"
-        0.0731358453631401
-        "this is a photo of two berries"
-        0.05045759305357933
-        "this is a photo of six berries"
-        0.04057715833187103
-        ```
-        
-        </td>
-        </tr>
-        
-        
-        </table>
-        
-        
-        ## [Documentation](https://clip-as-service.jina.ai)
-        
-        ## Install
-        
-        CLIP-as-service consists of two Python packages `clip-server` and `clip-client` that can be installed _independently_. Both require Python 3.7+. 
-        
-        ### Install server
-        
-        <table>
-        <tr>
-        <td> Pytorch Runtime ⚡ </td>
-        <td> ONNX Runtime ⚡⚡</td>
-        <td> TensorRT Runtime ⚡⚡⚡ </td>
-        </tr>
-        <tr>
-        <td>
-        
-        ```bash
-        pip install clip-server
-        ```
-        
-        </td>
-        <td>
-        
-        ```bash
-        pip install "clip-server[onnx]"
-        ```
-        
-        </td>
-        <td>
-        
-        ```bash
-        pip install nvidia-pyindex 
-        pip install "clip-server[tensorrt]"
-        ```
-        </td>
-        </tr>
-        </table>
-        
-        You can also [host the server on Google Colab](https://clip-as-service.jina.ai/hosting/colab/), leveraging its free GPU/TPU.
-        
-        ### Install client
-        
-        ```bash
-        pip install clip-client
-        ```
-        
-        ### Quick check
-        
-        You can run a simple connectivity check after install.
-        
-        
-        <table>
-        <tr>
-        <th> C/S </th> 
-        <th> Command </th> 
-        <th> Expect output </th>
-        </tr>
-        <tr>
-        <td>
-        Server
-        </td>
-        <td> 
-        
-        ```bash
-        python -m clip_server
-        ```
-             
-        </td>
-        <td>
-        
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/server-output.svg?raw=true" alt="Expected server output" width="300px">
-        
-        </td>
-        </tr>
-        <tr>
-        <td>
-        Client
-        </td>
-        <td> 
-        
-        ```python
-        from clip_client import Client
-        
-        c = Client('grpc://0.0.0.0:23456')
-        c.profile()
-        ```
-             
-        </td>
-        <td>
-        
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/pyclient-output.svg?raw=true" alt="Expected clip-client output" width="300px">
-        
-        </td>
-        </tr>
-        </table>
-        
-        
-        You can change `0.0.0.0` to the intranet or public IP address to test the connectivity over private and public network. 
-        
-        
-        ## Get Started
-        
-        ### Basic usage
-        
-        1. Start the server: `python -m clip_server`. Remember its address and port.
-        2. Create a client:
-           ```python
-            from clip_client import Client
-           
-            c = Client('grpc://0.0.0.0:51000')
-            ```
-        3. To get sentence embedding:
-            ```python    
-            r = c.encode(['First do it', 'then do it right', 'then do it better'])
-            
-            print(r.shape)  # [3, 512] 
-            ```
-        4. To get image embedding:
-            ```python    
-            r = c.encode(['apple.png',  # local image 
-                          'https://clip-as-service.jina.ai/_static/favicon.png',  # remote image
-                          'data:image/gif;base64,R0lGODlhEAAQAMQAAORHHOVSKudfOulrSOp3WOyDZu6QdvCchPGolfO0o/XBs/fNwfjZ0frl3/zy7////wAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACH5BAkAABAALAAAAAAQABAAAAVVICSOZGlCQAosJ6mu7fiyZeKqNKToQGDsM8hBADgUXoGAiqhSvp5QAnQKGIgUhwFUYLCVDFCrKUE1lBavAViFIDlTImbKC5Gm2hB0SlBCBMQiB0UjIQA7'])  # in image URI
-            
-            print(r.shape)  # [3, 512]
-            ```
-        
-        More comprehensive server and client user guides can be found in the [docs](https://clip-as-service.jina.ai/).
-        
-        ### Text-to-image cross-modal search in 10 lines
-        
-        Let's build a text-to-image search using CLIP-as-service. Namely, a user can input a sentence and the program returns matching images. We'll use the [Totally Looks Like](https://sites.google.com/view/totally-looks-like-dataset) dataset and [DocArray](https://github.com/jina-ai/docarray) package. Note that DocArray is included within `clip-client` as an upstream dependency, so you don't need to install it separately.
-        
-        #### Load images
-        
-        First we load images. You can simply pull them from Jina Cloud:
-        
-        ```python
-        from docarray import DocumentArray
-        
-        da = DocumentArray.pull('ttl-original', show_progress=True, local_cache=True)
-        ```
-        
-        <details>
-        <summary>or download TTL dataset, unzip, load manually</summary>
-        
-        Alternatively, you can go to [Totally Looks Like](https://sites.google.com/view/totally-looks-like-dataset) official website, unzip and load images:
-        
-        ```python
-        from docarray import DocumentArray
-        
-        da = DocumentArray.from_files(['left/*.jpg', 'right/*.jpg'])
-        ```
-        
-        </details>
-        
-        The dataset contains 12,032 images, so it may take a while to pull. Once done, you can visualize it and get the first taste of those images:
-        
-        ```python
-        da.plot_image_sprites()
-        ```
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/ttl-image-sprites.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="50%">
-        </p>
-        
-        #### Encode images
-        
-        Start the server with `python -m clip_server`. Let's say it's at `0.0.0.0:51000` with `GRPC` protocol (you will get this information after running the server).
-        
-        Create a Python client script:
-        
-        ```python
-        from clip_client import Client
-        
-        c = Client(server='grpc://0.0.0.0:51000')
-        
-        da = c.encode(da, show_progress=True)
-        ```
-        
-        Depending on your GPU and client-server network, it may take a while to embed 12K images. In my case, it took about two minutes.
-        
-        <details>
-        <summary>Download the pre-encoded dataset</summary>
-        
-        If you're impatient or don't have a GPU, waiting can be Hell. In this case, you can simply pull our pre-encoded image dataset:
-        
-        ```python
-        from docarray import DocumentArray
-        
-        da = DocumentArray.pull('ttl-embedding', show_progress=True, local_cache=True)
-        ```
-        
-        </details>
-        
-        #### Search via sentence 
-        
-        Let's build a simple prompt to allow a user to type sentence:
-        
-        ```python
-        while True:
-            vec = c.encode([input('sentence> ')])
-            r = da.find(query=vec, limit=9)
-            r[0].plot_image_sprites()
-        ```
-        
-        #### Showcase
-        
-        Now you can input arbitrary English sentences and view the top-9 matching images. Search is fast and instinctive. Let's have some fun:
-        
-        <table>
-        <tr>
-        <th> "a happy potato" </th> 
-        <th> "a super evil AI" </th> 
-        <th> "a guy enjoying his burger" </th>
-        </tr>
-        <tr>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-happy-potato.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-super-evil-AI.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-guy-enjoying-his-burger.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        </tr>
-        </table>
-        
-        
-        <table>
-        <tr>
-        <th> "professor cat is very serious" </th> 
-        <th> "an ego engineer lives with parent" </th> 
-        <th> "there will be no tomorrow so lets eat unhealthy" </th>
-        </tr>
-        <tr>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/professor-cat-is-very-serious.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/an-ego-engineer-lives-with-parent.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/there-will-be-no-tomorrow-so-lets-eat-unhealthy.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        </tr>
-        </table>
-        
-        Let's save the embedding result for our next example: 
-        
-        ```python
-        da.save_binary('ttl-image')
-        ```
-        
-        ### Image-to-text cross-modal search in 10 Lines
-        
-        We can also switch the input and output of the last program to achieve image-to-text search. Precisely, given a query image find the sentence that best describes the image.
-        
-        Let's use all sentences from the book "Pride and Prejudice". 
-        
-        ```python
-        from docarray import Document, DocumentArray
-        
-        d = Document(uri='https://www.gutenberg.org/files/1342/1342-0.txt').load_uri_to_text()
-        da = DocumentArray(
-            Document(text=s.strip()) for s in d.text.replace('\r\n', '').split('.') if s.strip()
-        )
-        ```
-        
-        Let's look at what we got:
-        
-        ```python
-        da.summary()
-        ```
-        
-        ```text
-                    Documents Summary            
-                                                 
-          Length                 6403            
-          Homogenous Documents   True            
-          Common Attributes      ('id', 'text')  
-                                                 
-                             Attributes Summary                     
-                                                                    
-          Attribute   Data type   #Unique values   Has empty value  
-         ────────────────────────────────────────────────────────── 
-          id          ('str',)    6403             False            
-          text        ('str',)    6030             False            
-        ```
-        
-        #### Encode sentences
-        
-        Now encode these 6,403 sentences, it may take 10 seconds or less depending on your GPU and network: 
-        
-        ```python
-        from clip_client import Client
-        
-        c = Client('grpc://0.0.0.0:51000')
-        
-        r = c.encode(da, show_progress=True)
-        ```
-        
-        <details>
-        <summary>Download the pre-encoded dataset</summary>
-        
-        Again, for people who are impatient or don't have a GPU, we have prepared a pre-encoded text dataset:
-        
-        ```python
-        from docarray import DocumentArray
-        
-        da = DocumentArray.pull('ttl-textual', show_progress=True, local_cache=True)
-        ```
-        
-        </details>
-        
-        #### Search via image
-        
-        Let's load our previously stored image embedding, randomly sample 10 image Documents, then find top-1 nearest neighbour of each.
-        
-        ```python
-        from docarray import DocumentArray
-        
-        img_da = DocumentArray.load_binary('ttl-image')
-        
-        for d in img_da.sample(10):
-            print(da.find(d.embedding, limit=1)[0].text)
-        ```
-        
-        #### Showcase
-        
-        Fun time! Note, unlike the previous example, here the input is an image and the sentence is the output. All sentences come from the book "Pride and Prejudice". 
-        
-        <table>
-        <tr>
-        <td>
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Besides,-there-was-truth-in-his-looks.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Gardiner-smiled.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/what’s-his-name.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/By-tea-time,-however,-the-dose-had-been-enough,-and-Mr.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/You-do-not-look-well.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        </tr>
-        <tr>
-        <td>Besides, there was truth in his looks</td>
-        <td>Gardiner smiled</td>
-        <td>what’s his name</td>
-        <td>By tea time, however, the dose had been enough, and Mr</td>
-        <td>You do not look well</td>
-        </tr>
-        </table>
-        
-        <table>
-        <tr>
-        <td>
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/“A-gamester!”-she-cried.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/If-you-mention-my-name-at-the-Bell,-you-will-be-attended-to.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Never-mind-Miss-Lizzy’s-hair.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Elizabeth-will-soon-be-the-wife-of-Mr.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/I-saw-them-the-night-before-last.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        </tr>
-        <tr>
-        <td>“A gamester!” she cried</td>
-        <td>If you mention my name at the Bell, you will be attended to</td>
-        <td>Never mind Miss Lizzy’s hair</td>
-        <td>Elizabeth will soon be the wife of Mr</td>
-        <td>I saw them the night before last</td>
-        </tr>
-        </table>
-        
-        
-        
-        ### Rank image-text matches via CLIP model
-        
-        From `0.3.0` CLIP-as-service adds a new `/rank` endpoint that re-ranks cross-modal matches according to their joint likelihood in CLIP model. For example, given an image Document with some predefined sentence matches as below:
-        
-        ```python
-        from clip_client import Client
-        from docarray import Document
-        
-        c = Client(server='grpc://0.0.0.0:51000')
-        r = c.rank(
-            [
-                Document(
-                    uri='.github/README-img/rerank.png',
-                    matches=[
-                        Document(text=f'a photo of a {p}')
-                        for p in (
-                            'control room',
-                            'lecture room',
-                            'conference room',
-                            'podium indoor',
-                            'television studio',
-                        )
-                    ],
-                )
-            ]
-        )
-        
-        print(r['@m', ['text', 'scores__clip_score__value']])
-        ```
-        
-        ```text
-        [['a photo of a television studio', 'a photo of a conference room', 'a photo of a lecture room', 'a photo of a control room', 'a photo of a podium indoor'], 
-        [0.9920725226402283, 0.006038925610482693, 0.0009973491542041302, 0.00078492151806131, 0.00010626466246321797]]
-        ```
-        
-        One can see now `a photo of a television studio` is ranked to the top with `clip_score` score at `0.992`. In practice, one can use this endpoint to re-rank the matching result from another search system, for improving the cross-modal search quality.
-        
-        <table>
-        <tr>
-        <td>
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/rerank.png?raw=true" alt="Rerank endpoint image input" height="150px">
-        </td>
-        <td>
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/rerank-chart.svg?raw=true" alt="Rerank endpoint output">
-        </td>
-        </tr>
-        </table>
-        
-        ### Rank text-image matches via CLIP model
-        
-        In the [DALL·E Flow](https://github.com/jina-ai/dalle-flow) project, CLIP is called for ranking the generated results from DALL·E. [It has an Executor wrapped on top of `clip-client`](https://github.com/jina-ai/dalle-flow/blob/main/executors/rerank/executor.py), which calls `.arank()` - the async version of `.rank()`:
-        
-        ```python
-        from clip_client import Client
-        from jina import Executor, requests, DocumentArray
-        
-        
-        class ReRank(Executor):
-            def __init__(self, clip_server: str, **kwargs):
-                super().__init__(**kwargs)
-                self._client = Client(server=clip_server)
-        
-            @requests(on='/')
-            async def rerank(self, docs: DocumentArray, **kwargs):
-                return await self._client.arank(docs)
-        ```
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/client-dalle.png?raw=true" alt="CLIP-as-service used in DALLE Flow" width="300px">
-        </p>
-        
-        Intrigued? That's only scratching the surface of what CLIP-as-service is capable of. [Read our docs to learn more](https://clip-as-service.jina.ai).
-        
-        <!-- start support-pitch -->
-        ## Support
-        
-        - Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
-        - Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina's new features.
-            - **When?** The second Tuesday of every month
-            - **Where?**
-              Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
-              and [live stream on YouTube](https://youtube.com/c/jina-ai)
-        - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
-        
-        ## Join Us
-        
-        CLIP-as-service is backed by [Jina AI](https://jina.ai) and licensed under [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI engineers, solution engineers to build the next neural search ecosystem in open-source.
-        
-        <!-- end support-pitch -->
-        
 Keywords: jina openai clip deep-learning cross-modal multi-modal neural-search
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
@@ -801,7 +36,774 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: flash-attn
 Provides-Extra: onnx
 Provides-Extra: search
 Provides-Extra: tensorrt
 Provides-Extra: transformers
+
+<p align="center">
+<br>
+<br>
+<br>
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/docs/_static/logo-light.svg?raw=true" alt="CLIP-as-service logo: The data structure for unstructured data" width="200px">
+<br>
+<br>
+<br>
+<b>Embed images and sentences into fixed-length vectors with CLIP</b>
+</p>
+
+<p align=center>
+<a href="https://pypi.org/project/clip_server/"><img alt="PyPI" src="https://img.shields.io/pypi/v/clip_server?label=Release&style=flat-square"></a>
+<a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-3.1k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
+<a href="https://codecov.io/gh/jina-ai/clip-as-service"><img alt="Codecov branch" src="https://img.shields.io/codecov/c/github/jina-ai/clip-as-service/main?logo=Codecov&logoColor=white&style=flat-square"></a>
+<a href="https://colab.research.google.com/github/jina-ai/clip-as-service/blob/main/docs/hosting/cas-on-colab.ipynb"><img src="https://img.shields.io/badge/Host-on%20Google%20Colab%20(GPU/TPU)-brightgreen?style=flat-square&logo=googlecolab&&logoColor=white" alt="Host on Google Colab with GPU/TPU support"></a>
+</p>
+
+<!-- start elevator-pitch -->
+
+CLIP-as-service is a low-latency high-scalability service for embedding images and text. It can be easily integrated as a microservice into neural search solutions.
+
+⚡ **Fast**: Serve CLIP models with TensorRT, ONNX runtime and PyTorch w/o JIT with 800QPS<sup>[*]</sup>. Non-blocking duplex streaming on requests and responses, designed for large data and long-running tasks. 
+
+🫐 **Elastic**: Horizontally scale up and down multiple CLIP models on single GPU, with automatic load balancing.
+
+🐥 **Easy-to-use**: No learning curve, minimalist design on client and server. Intuitive and consistent API for image and sentence embedding. 
+
+👒 **Modern**: Async client support. Easily switch between gRPC, HTTP, WebSocket protocols with TLS and compression.
+
+🍱 **Integration**: Smooth integration with neural search ecosystem including [Jina](https://github.com/jina-ai/jina) and [DocArray](https://github.com/jina-ai/docarray). Build cross-modal and multi-modal solutions in no time. 
+
+<sup>[*] with default config (single replica, PyTorch no JIT) on GeForce RTX 3090. </sup>
+
+<!-- end elevator-pitch -->
+
+## Try it!
+
+An always-online server `api.clip.jina.ai` loaded with `ViT-L-14-336::openai` is there for you to play & test.
+Before you start, make sure you have obtained an access token from our [console website](https://console.clip.jina.ai/get_started), 
+or via CLI as described in [this guide](https://docs.jina.ai/jina-ai-cloud/login/#create-a-new-pat).
+
+```bash 
+jina auth token create <name of PAT> -e <expiration days>
+```
+
+Then, you need to configure the access token in the parameter `credential` of the client in python or set it in the HTTP request header `Authorization` as `<your access token>`.
+
+⚠️ Our demo server `demo-cas.jina.ai` is sunset and no longer available after **15th of Sept 2022**. 
+
+
+### Text & image embedding
+
+<table>
+<tr>
+<td> via HTTPS 🔐 </td>
+<td> via gRPC 🔐⚡⚡ </td>
+</tr>
+<tr>
+<td>
+
+```bash
+curl \
+-X POST https://api.clip.jina.ai:8443/post \
+-H 'Content-Type: application/json' \
+-H 'Authorization: <your access token>' \
+-d '{"data":[{"text": "First do it"}, 
+    {"text": "then do it right"}, 
+    {"text": "then do it better"}, 
+    {"uri": "https://picsum.photos/200"}], 
+    "execEndpoint":"/"}'
+```
+
+</td>
+<td>
+
+```python
+# pip install clip-client
+from clip_client import Client
+
+c = Client(
+    'grpcs://api.clip.jina.ai:2096', credential={'Authorization': '<your access token>'}
+)
+
+r = c.encode(
+    [
+        'First do it',
+        'then do it right',
+        'then do it better',
+        'https://picsum.photos/200',
+    ]
+)
+print(r)
+```
+</td>
+</tr>
+</table>
+
+### Visual reasoning
+
+There are four basic visual reasoning skills: object recognition, object counting, color recognition, and spatial relation understanding. Let's try some:
+
+> You need to install [`jq` (a JSON processor)](https://stedolan.github.io/jq/) to prettify the results.
+
+<table>
+<tr>
+<td> Image </td>
+<td> via HTTPS 🔐 </td>
+</tr>
+<tr>
+<td>
+<img src="https://picsum.photos/id/1/300/300">
+</td>
+<td>
+
+```bash
+curl \
+-X POST https://api.clip.jina.ai:8443/post \
+-H 'Content-Type: application/json' \
+-H 'Authorization: <your access token>' \
+-d '{"data":[{"uri": "https://picsum.photos/id/1/300/300",
+"matches": [{"text": "there is a woman in the photo"},
+            {"text": "there is a man in the photo"}]}],
+            "execEndpoint":"/rank"}' \
+| jq ".data[].matches[] | (.text, .scores.clip_score.value)"
+```
+
+gives:
+
+```
+"there is a woman in the photo"
+0.626907229423523
+"there is a man in the photo"
+0.37309277057647705
+```
+
+</td>
+</tr>
+<tr>
+<td>
+<img src="https://picsum.photos/id/133/300/300">
+</td>
+<td>
+
+```bash
+curl \
+-X POST https://api.clip.jina.ai:8443/post \
+-H 'Content-Type: application/json' \
+-H 'Authorization: <your access token>' \
+-d '{"data":[{"uri": "https://picsum.photos/id/133/300/300",
+"matches": [
+{"text": "the blue car is on the left, the red car is on the right"},
+{"text": "the blue car is on the right, the red car is on the left"},
+{"text": "the blue car is on top of the red car"},
+{"text": "the blue car is below the red car"}]}],
+"execEndpoint":"/rank"}' \
+| jq ".data[].matches[] | (.text, .scores.clip_score.value)"
+```
+
+gives:
+```
+"the blue car is on the left, the red car is on the right"
+0.5232442617416382
+"the blue car is on the right, the red car is on the left"
+0.32878655195236206
+"the blue car is below the red car"
+0.11064132302999496
+"the blue car is on top of the red car"
+0.03732786327600479
+```
+
+</td>
+</tr>
+
+
+<tr>
+<td>
+<img src="https://picsum.photos/id/102/300/300">
+</td>
+<td>
+
+```bash
+curl \
+-X POST https://api.clip.jina.ai:8443/post \
+-H 'Content-Type: application/json' \
+-H 'Authorization: <your access token>' \
+-d '{"data":[{"uri": "https://picsum.photos/id/102/300/300",
+"matches": [{"text": "this is a photo of one berry"},
+            {"text": "this is a photo of two berries"},
+            {"text": "this is a photo of three berries"},
+            {"text": "this is a photo of four berries"},
+            {"text": "this is a photo of five berries"},
+            {"text": "this is a photo of six berries"}]}],
+            "execEndpoint":"/rank"}' \
+| jq ".data[].matches[] | (.text, .scores.clip_score.value)"
+```
+
+gives:
+```
+"this is a photo of three berries"
+0.48507222533226013
+"this is a photo of four berries"
+0.2377079576253891
+"this is a photo of one berry"
+0.11304923892021179
+"this is a photo of five berries"
+0.0731358453631401
+"this is a photo of two berries"
+0.05045759305357933
+"this is a photo of six berries"
+0.04057715833187103
+```
+
+</td>
+</tr>
+
+
+</table>
+
+
+## [Documentation](https://clip-as-service.jina.ai)
+
+## Install
+
+CLIP-as-service consists of two Python packages `clip-server` and `clip-client` that can be installed _independently_. Both require Python 3.7+. 
+
+### Install server
+
+<table>
+<tr>
+<td> Pytorch Runtime ⚡ </td>
+<td> ONNX Runtime ⚡⚡</td>
+<td> TensorRT Runtime ⚡⚡⚡ </td>
+</tr>
+<tr>
+<td>
+
+```bash
+pip install clip-server
+```
+
+</td>
+<td>
+
+```bash
+pip install "clip-server[onnx]"
+```
+
+</td>
+<td>
+
+```bash
+pip install nvidia-pyindex 
+pip install "clip-server[tensorrt]"
+```
+</td>
+</tr>
+</table>
+
+You can also [host the server on Google Colab](https://clip-as-service.jina.ai/hosting/colab/), leveraging its free GPU/TPU.
+
+### Install client
+
+```bash
+pip install clip-client
+```
+
+### Quick check
+
+You can run a simple connectivity check after install.
+
+
+<table>
+<tr>
+<th> C/S </th> 
+<th> Command </th> 
+<th> Expect output </th>
+</tr>
+<tr>
+<td>
+Server
+</td>
+<td> 
+
+```bash
+python -m clip_server
+```
+     
+</td>
+<td>
+
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/server-output.svg?raw=true" alt="Expected server output" width="300px">
+
+</td>
+</tr>
+<tr>
+<td>
+Client
+</td>
+<td> 
+
+```python
+from clip_client import Client
+
+c = Client('grpc://0.0.0.0:23456')
+c.profile()
+```
+     
+</td>
+<td>
+
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/pyclient-output.svg?raw=true" alt="Expected clip-client output" width="300px">
+
+</td>
+</tr>
+</table>
+
+
+You can change `0.0.0.0` to the intranet or public IP address to test the connectivity over private and public network. 
+
+
+## Get Started
+
+### Basic usage
+
+1. Start the server: `python -m clip_server`. Remember its address and port.
+2. Create a client:
+   ```python
+    from clip_client import Client
+   
+    c = Client('grpc://0.0.0.0:51000')
+    ```
+3. To get sentence embedding:
+    ```python    
+    r = c.encode(['First do it', 'then do it right', 'then do it better'])
+    
+    print(r.shape)  # [3, 512] 
+    ```
+4. To get image embedding:
+    ```python    
+    r = c.encode(['apple.png',  # local image 
+                  'https://clip-as-service.jina.ai/_static/favicon.png',  # remote image
+                  'data:image/gif;base64,R0lGODlhEAAQAMQAAORHHOVSKudfOulrSOp3WOyDZu6QdvCchPGolfO0o/XBs/fNwfjZ0frl3/zy7////wAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACH5BAkAABAALAAAAAAQABAAAAVVICSOZGlCQAosJ6mu7fiyZeKqNKToQGDsM8hBADgUXoGAiqhSvp5QAnQKGIgUhwFUYLCVDFCrKUE1lBavAViFIDlTImbKC5Gm2hB0SlBCBMQiB0UjIQA7'])  # in image URI
+    
+    print(r.shape)  # [3, 512]
+    ```
+
+More comprehensive server and client user guides can be found in the [docs](https://clip-as-service.jina.ai/).
+
+### Text-to-image cross-modal search in 10 lines
+
+Let's build a text-to-image search using CLIP-as-service. Namely, a user can input a sentence and the program returns matching images. We'll use the [Totally Looks Like](https://sites.google.com/view/totally-looks-like-dataset) dataset and [DocArray](https://github.com/jina-ai/docarray) package. Note that DocArray is included within `clip-client` as an upstream dependency, so you don't need to install it separately.
+
+#### Load images
+
+First we load images. You can simply pull them from Jina Cloud:
+
+```python
+from docarray import DocumentArray
+
+da = DocumentArray.pull('ttl-original', show_progress=True, local_cache=True)
+```
+
+<details>
+<summary>or download TTL dataset, unzip, load manually</summary>
+
+Alternatively, you can go to [Totally Looks Like](https://sites.google.com/view/totally-looks-like-dataset) official website, unzip and load images:
+
+```python
+from docarray import DocumentArray
+
+da = DocumentArray.from_files(['left/*.jpg', 'right/*.jpg'])
+```
+
+</details>
+
+The dataset contains 12,032 images, so it may take a while to pull. Once done, you can visualize it and get the first taste of those images:
+
+```python
+da.plot_image_sprites()
+```
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/ttl-image-sprites.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="50%">
+</p>
+
+#### Encode images
+
+Start the server with `python -m clip_server`. Let's say it's at `0.0.0.0:51000` with `GRPC` protocol (you will get this information after running the server).
+
+Create a Python client script:
+
+```python
+from clip_client import Client
+
+c = Client(server='grpc://0.0.0.0:51000')
+
+da = c.encode(da, show_progress=True)
+```
+
+Depending on your GPU and client-server network, it may take a while to embed 12K images. In my case, it took about two minutes.
+
+<details>
+<summary>Download the pre-encoded dataset</summary>
+
+If you're impatient or don't have a GPU, waiting can be Hell. In this case, you can simply pull our pre-encoded image dataset:
+
+```python
+from docarray import DocumentArray
+
+da = DocumentArray.pull('ttl-embedding', show_progress=True, local_cache=True)
+```
+
+</details>
+
+#### Search via sentence 
+
+Let's build a simple prompt to allow a user to type sentence:
+
+```python
+while True:
+    vec = c.encode([input('sentence> ')])
+    r = da.find(query=vec, limit=9)
+    r[0].plot_image_sprites()
+```
+
+#### Showcase
+
+Now you can input arbitrary English sentences and view the top-9 matching images. Search is fast and instinctive. Let's have some fun:
+
+<table>
+<tr>
+<th> "a happy potato" </th> 
+<th> "a super evil AI" </th> 
+<th> "a guy enjoying his burger" </th>
+</tr>
+<tr>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-happy-potato.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-super-evil-AI.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-guy-enjoying-his-burger.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+</tr>
+</table>
+
+
+<table>
+<tr>
+<th> "professor cat is very serious" </th> 
+<th> "an ego engineer lives with parent" </th> 
+<th> "there will be no tomorrow so lets eat unhealthy" </th>
+</tr>
+<tr>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/professor-cat-is-very-serious.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/an-ego-engineer-lives-with-parent.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/there-will-be-no-tomorrow-so-lets-eat-unhealthy.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+</tr>
+</table>
+
+Let's save the embedding result for our next example: 
+
+```python
+da.save_binary('ttl-image')
+```
+
+### Image-to-text cross-modal search in 10 Lines
+
+We can also switch the input and output of the last program to achieve image-to-text search. Precisely, given a query image find the sentence that best describes the image.
+
+Let's use all sentences from the book "Pride and Prejudice". 
+
+```python
+from docarray import Document, DocumentArray
+
+d = Document(uri='https://www.gutenberg.org/files/1342/1342-0.txt').load_uri_to_text()
+da = DocumentArray(
+    Document(text=s.strip()) for s in d.text.replace('\r\n', '').split('.') if s.strip()
+)
+```
+
+Let's look at what we got:
+
+```python
+da.summary()
+```
+
+```text
+            Documents Summary            
+                                         
+  Length                 6403            
+  Homogenous Documents   True            
+  Common Attributes      ('id', 'text')  
+                                         
+                     Attributes Summary                     
+                                                            
+  Attribute   Data type   #Unique values   Has empty value  
+ ────────────────────────────────────────────────────────── 
+  id          ('str',)    6403             False            
+  text        ('str',)    6030             False            
+```
+
+#### Encode sentences
+
+Now encode these 6,403 sentences, it may take 10 seconds or less depending on your GPU and network: 
+
+```python
+from clip_client import Client
+
+c = Client('grpc://0.0.0.0:51000')
+
+r = c.encode(da, show_progress=True)
+```
+
+<details>
+<summary>Download the pre-encoded dataset</summary>
+
+Again, for people who are impatient or don't have a GPU, we have prepared a pre-encoded text dataset:
+
+```python
+from docarray import DocumentArray
+
+da = DocumentArray.pull('ttl-textual', show_progress=True, local_cache=True)
+```
+
+</details>
+
+#### Search via image
+
+Let's load our previously stored image embedding, randomly sample 10 image Documents, then find top-1 nearest neighbour of each.
+
+```python
+from docarray import DocumentArray
+
+img_da = DocumentArray.load_binary('ttl-image')
+
+for d in img_da.sample(10):
+    print(da.find(d.embedding, limit=1)[0].text)
+```
+
+#### Showcase
+
+Fun time! Note, unlike the previous example, here the input is an image and the sentence is the output. All sentences come from the book "Pride and Prejudice". 
+
+<table>
+<tr>
+<td>
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Besides,-there-was-truth-in-his-looks.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Gardiner-smiled.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/what’s-his-name.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/By-tea-time,-however,-the-dose-had-been-enough,-and-Mr.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/You-do-not-look-well.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+</tr>
+<tr>
+<td>Besides, there was truth in his looks</td>
+<td>Gardiner smiled</td>
+<td>what’s his name</td>
+<td>By tea time, however, the dose had been enough, and Mr</td>
+<td>You do not look well</td>
+</tr>
+</table>
+
+<table>
+<tr>
+<td>
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/“A-gamester!”-she-cried.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/If-you-mention-my-name-at-the-Bell,-you-will-be-attended-to.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Never-mind-Miss-Lizzy’s-hair.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Elizabeth-will-soon-be-the-wife-of-Mr.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/I-saw-them-the-night-before-last.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+</tr>
+<tr>
+<td>“A gamester!” she cried</td>
+<td>If you mention my name at the Bell, you will be attended to</td>
+<td>Never mind Miss Lizzy’s hair</td>
+<td>Elizabeth will soon be the wife of Mr</td>
+<td>I saw them the night before last</td>
+</tr>
+</table>
+
+
+
+### Rank image-text matches via CLIP model
+
+From `0.3.0` CLIP-as-service adds a new `/rank` endpoint that re-ranks cross-modal matches according to their joint likelihood in CLIP model. For example, given an image Document with some predefined sentence matches as below:
+
+```python
+from clip_client import Client
+from docarray import Document
+
+c = Client(server='grpc://0.0.0.0:51000')
+r = c.rank(
+    [
+        Document(
+            uri='.github/README-img/rerank.png',
+            matches=[
+                Document(text=f'a photo of a {p}')
+                for p in (
+                    'control room',
+                    'lecture room',
+                    'conference room',
+                    'podium indoor',
+                    'television studio',
+                )
+            ],
+        )
+    ]
+)
+
+print(r['@m', ['text', 'scores__clip_score__value']])
+```
+
+```text
+[['a photo of a television studio', 'a photo of a conference room', 'a photo of a lecture room', 'a photo of a control room', 'a photo of a podium indoor'], 
+[0.9920725226402283, 0.006038925610482693, 0.0009973491542041302, 0.00078492151806131, 0.00010626466246321797]]
+```
+
+One can see now `a photo of a television studio` is ranked to the top with `clip_score` score at `0.992`. In practice, one can use this endpoint to re-rank the matching result from another search system, for improving the cross-modal search quality.
+
+<table>
+<tr>
+<td>
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/rerank.png?raw=true" alt="Rerank endpoint image input" height="150px">
+</td>
+<td>
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/rerank-chart.svg?raw=true" alt="Rerank endpoint output">
+</td>
+</tr>
+</table>
+
+### Rank text-image matches via CLIP model
+
+In the [DALL·E Flow](https://github.com/jina-ai/dalle-flow) project, CLIP is called for ranking the generated results from DALL·E. [It has an Executor wrapped on top of `clip-client`](https://github.com/jina-ai/dalle-flow/blob/main/executors/rerank/executor.py), which calls `.arank()` - the async version of `.rank()`:
+
+```python
+from clip_client import Client
+from jina import Executor, requests, DocumentArray
+
+
+class ReRank(Executor):
+    def __init__(self, clip_server: str, **kwargs):
+        super().__init__(**kwargs)
+        self._client = Client(server=clip_server)
+
+    @requests(on='/')
+    async def rerank(self, docs: DocumentArray, **kwargs):
+        return await self._client.arank(docs)
+```
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/client-dalle.png?raw=true" alt="CLIP-as-service used in DALLE Flow" width="300px">
+</p>
+
+Intrigued? That's only scratching the surface of what CLIP-as-service is capable of. [Read our docs to learn more](https://clip-as-service.jina.ai).
+
+<!-- start support-pitch -->
+## Support
+
+- Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
+- Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina's new features.
+    - **When?** The second Tuesday of every month
+    - **Where?**
+      Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
+      and [live stream on YouTube](https://youtube.com/c/jina-ai)
+- Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
+
+## Join Us
+
+CLIP-as-service is backed by [Jina AI](https://jina.ai) and licensed under [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI engineers, solution engineers to build the next neural search ecosystem in open-source.
+
+<!-- end support-pitch -->
+
+
```

#### html2text {}

```diff
@@ -1,14 +1,33 @@
-Metadata-Version: 2.1 Name: clip-server Version: 0.8.2.dev6 Summary: Embed
+Metadata-Version: 2.1 Name: clip-server Version: 0.8.2.dev9 Summary: Embed
 images and sentences into fixed-length vectors via CLIP Home-page: https://
 github.com/jina-ai/clip-as-service Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/clip-as-service/
 tags Project-URL: Documentation, https://clip-as-service.jina.ai Project-URL:
 Source, https://github.com/jina-ai/clip-as-service/ Project-URL: Tracker,
-https://github.com/jina-ai/clip-as-service/issues Description:
+https://github.com/jina-ai/clip-as-service/issues Keywords: jina openai clip
+deep-learning cross-modal multi-modal neural-search Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Education Classifier:
+Intended Audience :: Science/Research Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Unix Shell Classifier:
+Environment :: Console Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Classifier: Topic ::
+Database :: Database Engines/Servers Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Internet :: WWW/
+HTTP :: Indexing/Search Classifier: Topic :: Scientific/Engineering :: Image
+Recognition Classifier: Topic :: Multimedia :: Video Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Description-Content-Type: text/markdown Provides-
+Extra: flash-attn Provides-Extra: onnx Provides-Extra: search Provides-Extra:
+tensorrt Provides-Extra: transformers
 
 
 
        [CLIP-as-service logo: The data structure for unstructured data]
 
 
         Embed images and sentences into fixed-length vectors with CLIP
@@ -272,27 +291,8 @@
 [.ical](https://calendar.google.com/calendar/ical/
 c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics)) and
 [live stream on YouTube](https://youtube.com/c/jina-ai) - Subscribe to the
 latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 ## Join Us CLIP-as-service is backed by [Jina AI](https://jina.ai) and licensed
 under [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai)
 AI engineers, solution engineers to build the next neural search ecosystem in
-open-source.  Keywords: jina openai clip deep-learning cross-modal multi-modal
-neural-search Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Education Classifier: Intended Audience :: Science/
-Research Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Unix Shell Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: OS Independent Classifier: Topic :: Database :: Database
-Engines/Servers Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Scientific/Engineering :: Image Recognition Classifier:
-Topic :: Multimedia :: Video Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
-Software Development Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown Provides-Extra: flash-attn Provides-
-Extra: onnx Provides-Extra: search Provides-Extra: tensorrt Provides-Extra:
-transformers
+open-source.
```

### Comparing `clip-server-0.8.2.dev6/clip_server/__main__.py` & `clip-server-0.8.2.dev9/clip_server/__main__.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/executors/clip_onnx.py` & `clip-server-0.8.2.dev9/clip_server/executors/clip_tensorrt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,170 +1,188 @@
-import os
 import warnings
-from multiprocessing.pool import ThreadPool
-from typing import Optional, Dict
 from functools import partial
+from multiprocessing.pool import ThreadPool
+from typing import Dict, Optional
 
-import onnxruntime as ort
+import numpy as np
 from clip_server.executors.helper import (
-    split_img_txt_da,
     preproc_image,
     preproc_text,
     set_rank,
+    split_img_txt_da,
 )
 from clip_server.model import clip
-from clip_server.model.clip_onnx import CLIPOnnxModel
+from clip_server.model.clip_trt import CLIPTensorRTModel
 from clip_server.model.tokenization import Tokenizer
-from jina import Executor, requests, DocumentArray
+from jina import DocumentArray, Executor, requests
+from opentelemetry.trace import NoOpTracer, Span
 
 
 class CLIPEncoder(Executor):
     def __init__(
         self,
         name: str = 'ViT-B-32::openai',
-        device: Optional[str] = None,
+        device: str = 'cuda',
         num_worker_preprocess: int = 4,
         minibatch_size: int = 32,
         access_paths: str = '@r',
-        model_path: Optional[str] = None,
         **kwargs,
     ):
         """
         :param name: The name of the model to be used. Default 'ViT-B-32::openai'. A list of available models can be
             found at https://clip-as-service.jina.ai/user-guides/server/#model-support
-        :param device: 'cpu' or 'cuda'. Default is None, which auto-detects the device.
+        :param device: 'cpu' or 'cuda'. Default is 'cuda' since TensorRT is only supported on CUDA.
         :param num_worker_preprocess: The number of CPU workers to preprocess images and texts. Default is 4.
         :param minibatch_size: The size of the minibatch for preprocessing and encoding. Default is 32. Reduce this
             number if you encounter OOM errors.
         :param access_paths: The access paths to traverse on the input documents to get the images and texts to be
             processed. Visit https://docarray.jina.ai/fundamentals/documentarray/access-elements for more details.
-        :param model_path: The path to the model to be used. If not specified, the model will be downloaded or loaded
-            from the local cache. Visit https://clip-as-service.jina.ai/user-guides/server/#use-custom-model-for-onnx
-            to learn how to finetune custom models.
         """
         super().__init__(**kwargs)
 
+        self._num_worker_preprocess = num_worker_preprocess
+        self._pool = ThreadPool(processes=num_worker_preprocess)
+
         self._minibatch_size = minibatch_size
         self._access_paths = access_paths
         if 'traversal_paths' in kwargs:
             warnings.warn(
                 f'`traversal_paths` is deprecated. Use `access_paths` instead.'
             )
             self._access_paths = kwargs['traversal_paths']
 
-        self._pool = ThreadPool(processes=num_worker_preprocess)
-
-        self._model = CLIPOnnxModel(name, model_path)
-        self._tokenizer = Tokenizer(name)
-
-        self._image_transform = clip._transform_ndarray(self._model.image_size)
+        self._device = device
 
         import torch
 
-        if not device:
-            self._device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        else:
-            self._device = device
-
-        # define the priority order for the execution providers
-        providers = ['CPUExecutionProvider']
-
-        # prefer CUDA Execution Provider over CPU Execution Provider
-        if self._device.startswith('cuda'):
-            providers.insert(0, 'CUDAExecutionProvider')
-
-        sess_options = ort.SessionOptions()
-
-        # Enables all available optimizations including layout optimizations
-        sess_options.graph_optimization_level = (
-            ort.GraphOptimizationLevel.ORT_ENABLE_ALL
+        assert self._device.startswith('cuda'), (
+            f'can not perform inference on {self._device}'
+            f' with Nvidia TensorRT as backend'
         )
 
-        if not self._device.startswith('cuda') and (
-            'OMP_NUM_THREADS' not in os.environ
-            and hasattr(self.runtime_args, 'replicas')
-        ):
-            replicas = getattr(self.runtime_args, 'replicas', 1)
-            num_threads = max(1, torch.get_num_threads() * 2 // replicas)
-            if num_threads < 2:
-                warnings.warn(
-                    f'Too many replicas ({replicas}) vs too few threads {num_threads} may result in '
-                    f'sub-optimal performance.'
-                )
+        assert (
+            torch.cuda.is_available()
+        ), "CUDA/GPU is not available on Pytorch. Please check your CUDA installation"
 
-            # Run the operators in the graph in parallel (not support the CUDA Execution Provider)
-            sess_options.execution_mode = ort.ExecutionMode.ORT_PARALLEL
+        self._model = CLIPTensorRTModel(name)
 
-            # The number of threads used to parallelize the execution of the graph (across nodes)
-            sess_options.inter_op_num_threads = 1
-            sess_options.intra_op_num_threads = max(num_threads, 1)
+        self._model.start_engines()
 
-        self._model.start_sessions(sess_options=sess_options, providers=providers)
+        self._tokenizer = Tokenizer(name)
+        self._image_transform = clip._transform_ndarray(self._model.image_size)
+
+        if not self.tracer:
+            self.tracer = NoOpTracer()
 
     def _preproc_images(self, docs: 'DocumentArray', drop_image_content: bool):
         with self.monitor(
             name='preprocess_images_seconds',
             documentation='images preprocess time in seconds',
         ):
-            return preproc_image(
-                docs,
-                preprocess_fn=self._image_transform,
-                return_np=True,
-                drop_image_content=drop_image_content,
-            )
+            with self.tracer.start_as_current_span('preprocess_images'):
+                return preproc_image(
+                    docs,
+                    preprocess_fn=self._image_transform,
+                    device=self._device,
+                    return_np=False,
+                    drop_image_content=drop_image_content,
+                )
 
     def _preproc_texts(self, docs: 'DocumentArray'):
         with self.monitor(
             name='preprocess_texts_seconds',
             documentation='texts preprocess time in seconds',
         ):
-            return preproc_text(docs, tokenizer=self._tokenizer, return_np=True)
+            with self.tracer.start_as_current_span('preprocess_images'):
+                return preproc_text(
+                    docs,
+                    tokenizer=self._tokenizer,
+                    device=self._device,
+                    return_np=False,
+                )
 
     @requests(on='/rank')
     async def rank(self, docs: 'DocumentArray', parameters: Dict, **kwargs):
         _drop_image_content = parameters.get('drop_image_content', False)
         await self.encode(docs['@r,m'], drop_image_content=_drop_image_content)
 
         set_rank(docs)
 
     @requests
-    async def encode(self, docs: 'DocumentArray', parameters: Dict = {}, **kwargs):
-        access_paths = parameters.get('access_paths', self._access_paths)
-        if 'traversal_paths' in parameters:
-            warnings.warn(
-                f'`traversal_paths` is deprecated. Use `access_paths` instead.'
-            )
-            access_paths = parameters['traversal_paths']
-        _drop_image_content = parameters.get('drop_image_content', False)
+    async def encode(
+        self,
+        docs: 'DocumentArray',
+        tracing_context=None,
+        parameters: Dict = {},
+        **kwargs,
+    ):
+        with self.tracer.start_as_current_span(
+            'encode', context=tracing_context
+        ) as span:
+            span.set_attribute('device', self._device)
+            span.set_attribute('runtime', 'tensorrt')
+            access_paths = parameters.get('access_paths', self._access_paths)
+            if 'traversal_paths' in parameters:
+                warnings.warn(
+                    f'`traversal_paths` is deprecated. Use `access_paths` instead.'
+                )
+                access_paths = parameters['traversal_paths']
+            _drop_image_content = parameters.get('drop_image_content', False)
 
-        _img_da = DocumentArray()
-        _txt_da = DocumentArray()
-        for d in docs[access_paths]:
-            split_img_txt_da(d, _img_da, _txt_da)
-
-        # for image
-        if _img_da:
-            for minibatch, batch_data in _img_da.map_batch(
-                partial(self._preproc_images, drop_image_content=_drop_image_content),
-                batch_size=self._minibatch_size,
-                pool=self._pool,
-            ):
-                with self.monitor(
-                    name='encode_images_seconds',
-                    documentation='images encode time in seconds',
-                ):
-                    minibatch.embeddings = self._model.encode_image(batch_data)
-
-        # for text
-        if _txt_da:
-            for minibatch, batch_data in _txt_da.map_batch(
-                self._preproc_texts,
-                batch_size=self._minibatch_size,
-                pool=self._pool,
-            ):
-                with self.monitor(
-                    name='encode_texts_seconds',
-                    documentation='texts encode time in seconds',
-                ):
-                    minibatch.embeddings = self._model.encode_text(batch_data)
+            _img_da = DocumentArray()
+            _txt_da = DocumentArray()
+            for d in docs[access_paths]:
+                split_img_txt_da(d, _img_da, _txt_da)
+
+            with self.tracer.start_as_current_span('inference') as inference_span:
+                inference_span.set_attribute('drop_image_content', _drop_image_content)
+                inference_span.set_attribute('minibatch_size', self._minibatch_size)
+                inference_span.set_attribute('has_img_da', True if _img_da else False)
+                inference_span.set_attribute('has_txt_da', True if _txt_da else False)
+                # for image
+                if _img_da:
+                    with self.tracer.start_as_current_span(
+                        'img_minibatch_encoding'
+                    ) as img_encode_span:
+                        for minibatch, batch_data in _img_da.map_batch(
+                            partial(
+                                self._preproc_images,
+                                drop_image_content=_drop_image_content,
+                            ),
+                            batch_size=self._minibatch_size,
+                            pool=self._pool,
+                        ):
+                            with self.monitor(
+                                name='encode_images_seconds',
+                                documentation='images encode time in seconds',
+                            ):
+                                minibatch.embeddings = (
+                                    self._model.encode_image(batch_data)
+                                    .detach()
+                                    .cpu()
+                                    .numpy()
+                                    .astype(np.float32)
+                                )
+
+                # for text
+                if _txt_da:
+                    with self.tracer.start_as_current_span(
+                        'txt_minibatch_encoding'
+                    ) as txt_encode_span:
+                        for minibatch, batch_data in _txt_da.map_batch(
+                            self._preproc_texts,
+                            batch_size=self._minibatch_size,
+                            pool=self._pool,
+                        ):
+                            with self.monitor(
+                                name='encode_texts_seconds',
+                                documentation='texts encode time in seconds',
+                            ):
+                                minibatch.embeddings = (
+                                    self._model.encode_text(batch_data)
+                                    .detach()
+                                    .cpu()
+                                    .numpy()
+                                    .astype(np.float32)
+                                )
 
         return docs
```

### Comparing `clip-server-0.8.2.dev6/clip_server/executors/clip_tensorrt.py` & `clip-server-0.8.2.dev9/clip_server/executors/clip_onnx.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,153 +1,206 @@
+import os
 import warnings
-from multiprocessing.pool import ThreadPool
-from typing import Optional, Dict
 from functools import partial
+from multiprocessing.pool import ThreadPool
+from typing import Dict, Optional
 
-import numpy as np
+import onnxruntime as ort
 from clip_server.executors.helper import (
-    split_img_txt_da,
     preproc_image,
     preproc_text,
     set_rank,
+    split_img_txt_da,
 )
 from clip_server.model import clip
+from clip_server.model.clip_onnx import CLIPOnnxModel
 from clip_server.model.tokenization import Tokenizer
-from clip_server.model.clip_trt import CLIPTensorRTModel
-from jina import Executor, requests, DocumentArray
+from jina import DocumentArray, Executor, requests
+from opentelemetry.trace import NoOpTracer, Span
 
 
 class CLIPEncoder(Executor):
     def __init__(
         self,
         name: str = 'ViT-B-32::openai',
-        device: str = 'cuda',
+        device: Optional[str] = None,
         num_worker_preprocess: int = 4,
         minibatch_size: int = 32,
         access_paths: str = '@r',
+        model_path: Optional[str] = None,
         **kwargs,
     ):
         """
         :param name: The name of the model to be used. Default 'ViT-B-32::openai'. A list of available models can be
             found at https://clip-as-service.jina.ai/user-guides/server/#model-support
-        :param device: 'cpu' or 'cuda'. Default is 'cuda' since TensorRT is only supported on CUDA.
+        :param device: 'cpu' or 'cuda'. Default is None, which auto-detects the device.
         :param num_worker_preprocess: The number of CPU workers to preprocess images and texts. Default is 4.
         :param minibatch_size: The size of the minibatch for preprocessing and encoding. Default is 32. Reduce this
             number if you encounter OOM errors.
         :param access_paths: The access paths to traverse on the input documents to get the images and texts to be
             processed. Visit https://docarray.jina.ai/fundamentals/documentarray/access-elements for more details.
+        :param model_path: The path to the model to be used. If not specified, the model will be downloaded or loaded
+            from the local cache. Visit https://clip-as-service.jina.ai/user-guides/server/#use-custom-model-for-onnx
+            to learn how to finetune custom models.
         """
         super().__init__(**kwargs)
 
-        self._pool = ThreadPool(processes=num_worker_preprocess)
-
         self._minibatch_size = minibatch_size
         self._access_paths = access_paths
         if 'traversal_paths' in kwargs:
             warnings.warn(
                 f'`traversal_paths` is deprecated. Use `access_paths` instead.'
             )
             self._access_paths = kwargs['traversal_paths']
 
-        self._device = device
+        self._num_worker_preprocess = num_worker_preprocess
+        self._pool = ThreadPool(processes=num_worker_preprocess)
+
+        self._model = CLIPOnnxModel(name, model_path)
+        self._tokenizer = Tokenizer(name)
+
+        self._image_transform = clip._transform_ndarray(self._model.image_size)
 
         import torch
 
-        assert self._device.startswith('cuda'), (
-            f'can not perform inference on {self._device}'
-            f' with Nvidia TensorRT as backend'
+        if not device:
+            self._device = 'cuda' if torch.cuda.is_available() else 'cpu'
+        else:
+            self._device = device
+
+        # define the priority order for the execution providers
+        providers = ['CPUExecutionProvider']
+
+        # prefer CUDA Execution Provider over CPU Execution Provider
+        if self._device.startswith('cuda'):
+            providers.insert(0, 'CUDAExecutionProvider')
+
+        sess_options = ort.SessionOptions()
+
+        # Enables all available optimizations including layout optimizations
+        sess_options.graph_optimization_level = (
+            ort.GraphOptimizationLevel.ORT_ENABLE_ALL
         )
 
-        assert (
-            torch.cuda.is_available()
-        ), "CUDA/GPU is not available on Pytorch. Please check your CUDA installation"
+        if not self._device.startswith('cuda') and (
+            'OMP_NUM_THREADS' not in os.environ
+            and hasattr(self.runtime_args, 'replicas')
+        ):
+            replicas = getattr(self.runtime_args, 'replicas', 1)
+            num_threads = max(1, torch.get_num_threads() * 2 // replicas)
+            if num_threads < 2:
+                warnings.warn(
+                    f'Too many replicas ({replicas}) vs too few threads {num_threads} may result in '
+                    f'sub-optimal performance.'
+                )
+
+            # Run the operators in the graph in parallel (not support the CUDA Execution Provider)
+            sess_options.execution_mode = ort.ExecutionMode.ORT_PARALLEL
+
+            # The number of threads used to parallelize the execution of the graph (across nodes)
+            sess_options.inter_op_num_threads = 1
+            sess_options.intra_op_num_threads = max(num_threads, 1)
 
-        self._model = CLIPTensorRTModel(name)
+        self._model.start_sessions(sess_options=sess_options, providers=providers)
 
-        self._model.start_engines()
-
-        self._tokenizer = Tokenizer(name)
-        self._image_transform = clip._transform_ndarray(self._model.image_size)
+        if not self.tracer:
+            self.tracer = NoOpTracer()
 
     def _preproc_images(self, docs: 'DocumentArray', drop_image_content: bool):
         with self.monitor(
             name='preprocess_images_seconds',
             documentation='images preprocess time in seconds',
         ):
-            return preproc_image(
-                docs,
-                preprocess_fn=self._image_transform,
-                device=self._device,
-                return_np=False,
-                drop_image_content=drop_image_content,
-            )
+            with self.tracer.start_as_current_span('preprocess_images'):
+                return preproc_image(
+                    docs,
+                    preprocess_fn=self._image_transform,
+                    return_np=True,
+                    drop_image_content=drop_image_content,
+                )
 
     def _preproc_texts(self, docs: 'DocumentArray'):
         with self.monitor(
             name='preprocess_texts_seconds',
             documentation='texts preprocess time in seconds',
         ):
-            return preproc_text(
-                docs, tokenizer=self._tokenizer, device=self._device, return_np=False
-            )
+            with self.tracer.start_as_current_span('preprocess_images'):
+                return preproc_text(docs, tokenizer=self._tokenizer, return_np=True)
 
     @requests(on='/rank')
     async def rank(self, docs: 'DocumentArray', parameters: Dict, **kwargs):
         _drop_image_content = parameters.get('drop_image_content', False)
         await self.encode(docs['@r,m'], drop_image_content=_drop_image_content)
 
         set_rank(docs)
 
     @requests
-    async def encode(self, docs: 'DocumentArray', parameters: Dict = {}, **kwargs):
-        access_paths = parameters.get('access_paths', self._access_paths)
-        if 'traversal_paths' in parameters:
-            warnings.warn(
-                f'`traversal_paths` is deprecated. Use `access_paths` instead.'
-            )
-            access_paths = parameters['traversal_paths']
-        _drop_image_content = parameters.get('drop_image_content', False)
-
-        _img_da = DocumentArray()
-        _txt_da = DocumentArray()
-        for d in docs[access_paths]:
-            split_img_txt_da(d, _img_da, _txt_da)
-
-        # for image
-        if _img_da:
-            for minibatch, batch_data in _img_da.map_batch(
-                partial(self._preproc_images, drop_image_content=_drop_image_content),
-                batch_size=self._minibatch_size,
-                pool=self._pool,
-            ):
-                with self.monitor(
-                    name='encode_images_seconds',
-                    documentation='images encode time in seconds',
-                ):
-                    minibatch.embeddings = (
-                        self._model.encode_image(batch_data)
-                        .detach()
-                        .cpu()
-                        .numpy()
-                        .astype(np.float32)
-                    )
-
-        # for text
-        if _txt_da:
-            for minibatch, batch_data in _txt_da.map_batch(
-                self._preproc_texts,
-                batch_size=self._minibatch_size,
-                pool=self._pool,
-            ):
-                with self.monitor(
-                    name='encode_texts_seconds',
-                    documentation='texts encode time in seconds',
-                ):
-                    minibatch.embeddings = (
-                        self._model.encode_text(batch_data)
-                        .detach()
-                        .cpu()
-                        .numpy()
-                        .astype(np.float32)
-                    )
+    async def encode(
+        self,
+        docs: 'DocumentArray',
+        tracing_context=None,
+        parameters: Dict = {},
+        **kwargs,
+    ):
+        with self.tracer.start_as_current_span(
+            'encode', context=tracing_context
+        ) as span:
+            span.set_attribute('device', self._device)
+            span.set_attribute('runtime', 'onnx')
+            access_paths = parameters.get('access_paths', self._access_paths)
+            if 'traversal_paths' in parameters:
+                warnings.warn(
+                    f'`traversal_paths` is deprecated. Use `access_paths` instead.'
+                )
+                access_paths = parameters['traversal_paths']
+            _drop_image_content = parameters.get('drop_image_content', False)
+
+            _img_da = DocumentArray()
+            _txt_da = DocumentArray()
+            for d in docs[access_paths]:
+                split_img_txt_da(d, _img_da, _txt_da)
+
+            with self.tracer.start_as_current_span('inference') as inference_span:
+                inference_span.set_attribute('drop_image_content', _drop_image_content)
+                inference_span.set_attribute('minibatch_size', self._minibatch_size)
+                inference_span.set_attribute('has_img_da', True if _img_da else False)
+                inference_span.set_attribute('has_txt_da', True if _txt_da else False)
+                # for image
+                if _img_da:
+                    with self.tracer.start_as_current_span(
+                        'img_minibatch_encoding'
+                    ) as img_encode_span:
+                        for minibatch, batch_data in _img_da.map_batch(
+                            partial(
+                                self._preproc_images,
+                                drop_image_content=_drop_image_content,
+                            ),
+                            batch_size=self._minibatch_size,
+                            pool=self._pool,
+                        ):
+                            with self.monitor(
+                                name='encode_images_seconds',
+                                documentation='images encode time in seconds',
+                            ):
+                                minibatch.embeddings = self._model.encode_image(
+                                    batch_data
+                                )
+
+                # for text
+                if _txt_da:
+                    with self.tracer.start_as_current_span(
+                        'txt_minibatch_encoding'
+                    ) as txt_encode_span:
+                        for minibatch, batch_data in _txt_da.map_batch(
+                            self._preproc_texts,
+                            batch_size=self._minibatch_size,
+                            pool=self._pool,
+                        ):
+                            with self.monitor(
+                                name='encode_texts_seconds',
+                                documentation='texts encode time in seconds',
+                            ):
+                                minibatch.embeddings = self._model.encode_text(
+                                    batch_data
+                                )
 
         return docs
```

### Comparing `clip-server-0.8.2.dev6/clip_server/executors/helper.py` & `clip-server-0.8.2.dev9/clip_server/executors/helper.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/helper.py` & `clip-server-0.8.2.dev9/clip_server/helper.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/clip.py` & `clip-server-0.8.2.dev9/clip_server/model/clip.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/clip_model.py` & `clip-server-0.8.2.dev9/clip_server/model/clip_model.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/clip_onnx.py` & `clip-server-0.8.2.dev9/clip_server/model/clip_onnx.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/clip_trt.py` & `clip-server-0.8.2.dev9/clip_server/model/clip_trt.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/flash_attention.py` & `clip-server-0.8.2.dev9/clip_server/model/flash_attention.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/mclip_model.py` & `clip-server-0.8.2.dev9/clip_server/model/mclip_model.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/model.py` & `clip-server-0.8.2.dev9/clip_server/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,17 @@
             )
         except KeyError:
             sd = {k[7:]: v for k, v in state_dict["state_dict"].items()}
             model = build_model_from_openai_state_dict(sd, dtype=dtype)
 
         # model from OpenAI state dict is in manually cast fp16 mode, must be converted for AMP/fp32/bf16 use
         model = model.to(device)
-        if dtype == torch.float32 or dtype.startswith('amp'):
+        if dtype == torch.float32 or (
+            isinstance(dtype, str) and dtype.startswith('amp')
+        ):
             model.float()
         elif dtype == torch.bfloat16:
             convert_weights_to_lp(model, dtype=torch.bfloat16)
 
         return model
 
     # patch the device names
```

### Comparing `clip-server-0.8.2.dev6/clip_server/model/openclip_model.py` & `clip-server-0.8.2.dev9/clip_server/model/openclip_model.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/pretrained_models.py` & `clip-server-0.8.2.dev9/clip_server/model/pretrained_models.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/simple_tokenizer.py` & `clip-server-0.8.2.dev9/clip_server/model/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/tokenization.py` & `clip-server-0.8.2.dev9/clip_server/model/tokenization.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/model/trt_utils.py` & `clip-server-0.8.2.dev9/clip_server/model/trt_utils.py`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server/resources/bpe_simple_vocab_16e6.txt.gz` & `clip-server-0.8.2.dev9/clip_server/resources/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/clip_server.egg-info/PKG-INFO` & `clip-server-0.8.2.dev9/clip_server.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,784 +1,19 @@
 Metadata-Version: 2.1
 Name: clip-server
-Version: 0.8.2.dev6
+Version: 0.8.2.dev9
 Summary: Embed images and sentences into fixed-length vectors via CLIP
 Home-page: https://github.com/jina-ai/clip-as-service
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/clip-as-service/tags
 Project-URL: Documentation, https://clip-as-service.jina.ai
 Project-URL: Source, https://github.com/jina-ai/clip-as-service/
 Project-URL: Tracker, https://github.com/jina-ai/clip-as-service/issues
-Description: <p align="center">
-        <br>
-        <br>
-        <br>
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/docs/_static/logo-light.svg?raw=true" alt="CLIP-as-service logo: The data structure for unstructured data" width="200px">
-        <br>
-        <br>
-        <br>
-        <b>Embed images and sentences into fixed-length vectors with CLIP</b>
-        </p>
-        
-        <p align=center>
-        <a href="https://pypi.org/project/clip_server/"><img alt="PyPI" src="https://img.shields.io/pypi/v/clip_server?label=Release&style=flat-square"></a>
-        <a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-3.1k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
-        <a href="https://codecov.io/gh/jina-ai/clip-as-service"><img alt="Codecov branch" src="https://img.shields.io/codecov/c/github/jina-ai/clip-as-service/main?logo=Codecov&logoColor=white&style=flat-square"></a>
-        <a href="https://colab.research.google.com/github/jina-ai/clip-as-service/blob/main/docs/hosting/cas-on-colab.ipynb"><img src="https://img.shields.io/badge/Host-on%20Google%20Colab%20(GPU/TPU)-brightgreen?style=flat-square&logo=googlecolab&&logoColor=white" alt="Host on Google Colab with GPU/TPU support"></a>
-        </p>
-        
-        <!-- start elevator-pitch -->
-        
-        CLIP-as-service is a low-latency high-scalability service for embedding images and text. It can be easily integrated as a microservice into neural search solutions.
-        
-        ⚡ **Fast**: Serve CLIP models with TensorRT, ONNX runtime and PyTorch w/o JIT with 800QPS<sup>[*]</sup>. Non-blocking duplex streaming on requests and responses, designed for large data and long-running tasks. 
-        
-        🫐 **Elastic**: Horizontally scale up and down multiple CLIP models on single GPU, with automatic load balancing.
-        
-        🐥 **Easy-to-use**: No learning curve, minimalist design on client and server. Intuitive and consistent API for image and sentence embedding. 
-        
-        👒 **Modern**: Async client support. Easily switch between gRPC, HTTP, WebSocket protocols with TLS and compression.
-        
-        🍱 **Integration**: Smooth integration with neural search ecosystem including [Jina](https://github.com/jina-ai/jina) and [DocArray](https://github.com/jina-ai/docarray). Build cross-modal and multi-modal solutions in no time. 
-        
-        <sup>[*] with default config (single replica, PyTorch no JIT) on GeForce RTX 3090. </sup>
-        
-        <!-- end elevator-pitch -->
-        
-        ## Try it!
-        
-        An always-online server `api.clip.jina.ai` loaded with `ViT-L-14-336::openai` is there for you to play & test.
-        Before you start, make sure you have obtained an access token from our [console website](https://console.clip.jina.ai/get_started), 
-        or via CLI as described in [this guide](https://docs.jina.ai/jina-ai-cloud/login/#create-a-new-pat).
-        
-        ```bash 
-        jina auth token create <name of PAT> -e <expiration days>
-        ```
-        
-        Then, you need to configure the access token in the parameter `credential` of the client in python or set it in the HTTP request header `Authorization` as `<your access token>`.
-        
-        ⚠️ Our demo server `demo-cas.jina.ai` is sunset and no longer available after **15th of Sept 2022**. 
-        
-        
-        ### Text & image embedding
-        
-        <table>
-        <tr>
-        <td> via HTTPS 🔐 </td>
-        <td> via gRPC 🔐⚡⚡ </td>
-        </tr>
-        <tr>
-        <td>
-        
-        ```bash
-        curl \
-        -X POST https://api.clip.jina.ai:8443/post \
-        -H 'Content-Type: application/json' \
-        -H 'Authorization: <your access token>' \
-        -d '{"data":[{"text": "First do it"}, 
-            {"text": "then do it right"}, 
-            {"text": "then do it better"}, 
-            {"uri": "https://picsum.photos/200"}], 
-            "execEndpoint":"/"}'
-        ```
-        
-        </td>
-        <td>
-        
-        ```python
-        # pip install clip-client
-        from clip_client import Client
-        
-        c = Client(
-            'grpcs://api.clip.jina.ai:2096', credential={'Authorization': '<your access token>'}
-        )
-        
-        r = c.encode(
-            [
-                'First do it',
-                'then do it right',
-                'then do it better',
-                'https://picsum.photos/200',
-            ]
-        )
-        print(r)
-        ```
-        </td>
-        </tr>
-        </table>
-        
-        ### Visual reasoning
-        
-        There are four basic visual reasoning skills: object recognition, object counting, color recognition, and spatial relation understanding. Let's try some:
-        
-        > You need to install [`jq` (a JSON processor)](https://stedolan.github.io/jq/) to prettify the results.
-        
-        <table>
-        <tr>
-        <td> Image </td>
-        <td> via HTTPS 🔐 </td>
-        </tr>
-        <tr>
-        <td>
-        <img src="https://picsum.photos/id/1/300/300">
-        </td>
-        <td>
-        
-        ```bash
-        curl \
-        -X POST https://api.clip.jina.ai:8443/post \
-        -H 'Content-Type: application/json' \
-        -H 'Authorization: <your access token>' \
-        -d '{"data":[{"uri": "https://picsum.photos/id/1/300/300",
-        "matches": [{"text": "there is a woman in the photo"},
-                    {"text": "there is a man in the photo"}]}],
-                    "execEndpoint":"/rank"}' \
-        | jq ".data[].matches[] | (.text, .scores.clip_score.value)"
-        ```
-        
-        gives:
-        
-        ```
-        "there is a woman in the photo"
-        0.626907229423523
-        "there is a man in the photo"
-        0.37309277057647705
-        ```
-        
-        </td>
-        </tr>
-        <tr>
-        <td>
-        <img src="https://picsum.photos/id/133/300/300">
-        </td>
-        <td>
-        
-        ```bash
-        curl \
-        -X POST https://api.clip.jina.ai:8443/post \
-        -H 'Content-Type: application/json' \
-        -H 'Authorization: <your access token>' \
-        -d '{"data":[{"uri": "https://picsum.photos/id/133/300/300",
-        "matches": [
-        {"text": "the blue car is on the left, the red car is on the right"},
-        {"text": "the blue car is on the right, the red car is on the left"},
-        {"text": "the blue car is on top of the red car"},
-        {"text": "the blue car is below the red car"}]}],
-        "execEndpoint":"/rank"}' \
-        | jq ".data[].matches[] | (.text, .scores.clip_score.value)"
-        ```
-        
-        gives:
-        ```
-        "the blue car is on the left, the red car is on the right"
-        0.5232442617416382
-        "the blue car is on the right, the red car is on the left"
-        0.32878655195236206
-        "the blue car is below the red car"
-        0.11064132302999496
-        "the blue car is on top of the red car"
-        0.03732786327600479
-        ```
-        
-        </td>
-        </tr>
-        
-        
-        <tr>
-        <td>
-        <img src="https://picsum.photos/id/102/300/300">
-        </td>
-        <td>
-        
-        ```bash
-        curl \
-        -X POST https://api.clip.jina.ai:8443/post \
-        -H 'Content-Type: application/json' \
-        -H 'Authorization: <your access token>' \
-        -d '{"data":[{"uri": "https://picsum.photos/id/102/300/300",
-        "matches": [{"text": "this is a photo of one berry"},
-                    {"text": "this is a photo of two berries"},
-                    {"text": "this is a photo of three berries"},
-                    {"text": "this is a photo of four berries"},
-                    {"text": "this is a photo of five berries"},
-                    {"text": "this is a photo of six berries"}]}],
-                    "execEndpoint":"/rank"}' \
-        | jq ".data[].matches[] | (.text, .scores.clip_score.value)"
-        ```
-        
-        gives:
-        ```
-        "this is a photo of three berries"
-        0.48507222533226013
-        "this is a photo of four berries"
-        0.2377079576253891
-        "this is a photo of one berry"
-        0.11304923892021179
-        "this is a photo of five berries"
-        0.0731358453631401
-        "this is a photo of two berries"
-        0.05045759305357933
-        "this is a photo of six berries"
-        0.04057715833187103
-        ```
-        
-        </td>
-        </tr>
-        
-        
-        </table>
-        
-        
-        ## [Documentation](https://clip-as-service.jina.ai)
-        
-        ## Install
-        
-        CLIP-as-service consists of two Python packages `clip-server` and `clip-client` that can be installed _independently_. Both require Python 3.7+. 
-        
-        ### Install server
-        
-        <table>
-        <tr>
-        <td> Pytorch Runtime ⚡ </td>
-        <td> ONNX Runtime ⚡⚡</td>
-        <td> TensorRT Runtime ⚡⚡⚡ </td>
-        </tr>
-        <tr>
-        <td>
-        
-        ```bash
-        pip install clip-server
-        ```
-        
-        </td>
-        <td>
-        
-        ```bash
-        pip install "clip-server[onnx]"
-        ```
-        
-        </td>
-        <td>
-        
-        ```bash
-        pip install nvidia-pyindex 
-        pip install "clip-server[tensorrt]"
-        ```
-        </td>
-        </tr>
-        </table>
-        
-        You can also [host the server on Google Colab](https://clip-as-service.jina.ai/hosting/colab/), leveraging its free GPU/TPU.
-        
-        ### Install client
-        
-        ```bash
-        pip install clip-client
-        ```
-        
-        ### Quick check
-        
-        You can run a simple connectivity check after install.
-        
-        
-        <table>
-        <tr>
-        <th> C/S </th> 
-        <th> Command </th> 
-        <th> Expect output </th>
-        </tr>
-        <tr>
-        <td>
-        Server
-        </td>
-        <td> 
-        
-        ```bash
-        python -m clip_server
-        ```
-             
-        </td>
-        <td>
-        
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/server-output.svg?raw=true" alt="Expected server output" width="300px">
-        
-        </td>
-        </tr>
-        <tr>
-        <td>
-        Client
-        </td>
-        <td> 
-        
-        ```python
-        from clip_client import Client
-        
-        c = Client('grpc://0.0.0.0:23456')
-        c.profile()
-        ```
-             
-        </td>
-        <td>
-        
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/pyclient-output.svg?raw=true" alt="Expected clip-client output" width="300px">
-        
-        </td>
-        </tr>
-        </table>
-        
-        
-        You can change `0.0.0.0` to the intranet or public IP address to test the connectivity over private and public network. 
-        
-        
-        ## Get Started
-        
-        ### Basic usage
-        
-        1. Start the server: `python -m clip_server`. Remember its address and port.
-        2. Create a client:
-           ```python
-            from clip_client import Client
-           
-            c = Client('grpc://0.0.0.0:51000')
-            ```
-        3. To get sentence embedding:
-            ```python    
-            r = c.encode(['First do it', 'then do it right', 'then do it better'])
-            
-            print(r.shape)  # [3, 512] 
-            ```
-        4. To get image embedding:
-            ```python    
-            r = c.encode(['apple.png',  # local image 
-                          'https://clip-as-service.jina.ai/_static/favicon.png',  # remote image
-                          'data:image/gif;base64,R0lGODlhEAAQAMQAAORHHOVSKudfOulrSOp3WOyDZu6QdvCchPGolfO0o/XBs/fNwfjZ0frl3/zy7////wAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACH5BAkAABAALAAAAAAQABAAAAVVICSOZGlCQAosJ6mu7fiyZeKqNKToQGDsM8hBADgUXoGAiqhSvp5QAnQKGIgUhwFUYLCVDFCrKUE1lBavAViFIDlTImbKC5Gm2hB0SlBCBMQiB0UjIQA7'])  # in image URI
-            
-            print(r.shape)  # [3, 512]
-            ```
-        
-        More comprehensive server and client user guides can be found in the [docs](https://clip-as-service.jina.ai/).
-        
-        ### Text-to-image cross-modal search in 10 lines
-        
-        Let's build a text-to-image search using CLIP-as-service. Namely, a user can input a sentence and the program returns matching images. We'll use the [Totally Looks Like](https://sites.google.com/view/totally-looks-like-dataset) dataset and [DocArray](https://github.com/jina-ai/docarray) package. Note that DocArray is included within `clip-client` as an upstream dependency, so you don't need to install it separately.
-        
-        #### Load images
-        
-        First we load images. You can simply pull them from Jina Cloud:
-        
-        ```python
-        from docarray import DocumentArray
-        
-        da = DocumentArray.pull('ttl-original', show_progress=True, local_cache=True)
-        ```
-        
-        <details>
-        <summary>or download TTL dataset, unzip, load manually</summary>
-        
-        Alternatively, you can go to [Totally Looks Like](https://sites.google.com/view/totally-looks-like-dataset) official website, unzip and load images:
-        
-        ```python
-        from docarray import DocumentArray
-        
-        da = DocumentArray.from_files(['left/*.jpg', 'right/*.jpg'])
-        ```
-        
-        </details>
-        
-        The dataset contains 12,032 images, so it may take a while to pull. Once done, you can visualize it and get the first taste of those images:
-        
-        ```python
-        da.plot_image_sprites()
-        ```
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/ttl-image-sprites.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="50%">
-        </p>
-        
-        #### Encode images
-        
-        Start the server with `python -m clip_server`. Let's say it's at `0.0.0.0:51000` with `GRPC` protocol (you will get this information after running the server).
-        
-        Create a Python client script:
-        
-        ```python
-        from clip_client import Client
-        
-        c = Client(server='grpc://0.0.0.0:51000')
-        
-        da = c.encode(da, show_progress=True)
-        ```
-        
-        Depending on your GPU and client-server network, it may take a while to embed 12K images. In my case, it took about two minutes.
-        
-        <details>
-        <summary>Download the pre-encoded dataset</summary>
-        
-        If you're impatient or don't have a GPU, waiting can be Hell. In this case, you can simply pull our pre-encoded image dataset:
-        
-        ```python
-        from docarray import DocumentArray
-        
-        da = DocumentArray.pull('ttl-embedding', show_progress=True, local_cache=True)
-        ```
-        
-        </details>
-        
-        #### Search via sentence 
-        
-        Let's build a simple prompt to allow a user to type sentence:
-        
-        ```python
-        while True:
-            vec = c.encode([input('sentence> ')])
-            r = da.find(query=vec, limit=9)
-            r[0].plot_image_sprites()
-        ```
-        
-        #### Showcase
-        
-        Now you can input arbitrary English sentences and view the top-9 matching images. Search is fast and instinctive. Let's have some fun:
-        
-        <table>
-        <tr>
-        <th> "a happy potato" </th> 
-        <th> "a super evil AI" </th> 
-        <th> "a guy enjoying his burger" </th>
-        </tr>
-        <tr>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-happy-potato.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-super-evil-AI.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-guy-enjoying-his-burger.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        </tr>
-        </table>
-        
-        
-        <table>
-        <tr>
-        <th> "professor cat is very serious" </th> 
-        <th> "an ego engineer lives with parent" </th> 
-        <th> "there will be no tomorrow so lets eat unhealthy" </th>
-        </tr>
-        <tr>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/professor-cat-is-very-serious.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/an-ego-engineer-lives-with-parent.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/there-will-be-no-tomorrow-so-lets-eat-unhealthy.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
-        </p>
-        
-        </td>
-        </tr>
-        </table>
-        
-        Let's save the embedding result for our next example: 
-        
-        ```python
-        da.save_binary('ttl-image')
-        ```
-        
-        ### Image-to-text cross-modal search in 10 Lines
-        
-        We can also switch the input and output of the last program to achieve image-to-text search. Precisely, given a query image find the sentence that best describes the image.
-        
-        Let's use all sentences from the book "Pride and Prejudice". 
-        
-        ```python
-        from docarray import Document, DocumentArray
-        
-        d = Document(uri='https://www.gutenberg.org/files/1342/1342-0.txt').load_uri_to_text()
-        da = DocumentArray(
-            Document(text=s.strip()) for s in d.text.replace('\r\n', '').split('.') if s.strip()
-        )
-        ```
-        
-        Let's look at what we got:
-        
-        ```python
-        da.summary()
-        ```
-        
-        ```text
-                    Documents Summary            
-                                                 
-          Length                 6403            
-          Homogenous Documents   True            
-          Common Attributes      ('id', 'text')  
-                                                 
-                             Attributes Summary                     
-                                                                    
-          Attribute   Data type   #Unique values   Has empty value  
-         ────────────────────────────────────────────────────────── 
-          id          ('str',)    6403             False            
-          text        ('str',)    6030             False            
-        ```
-        
-        #### Encode sentences
-        
-        Now encode these 6,403 sentences, it may take 10 seconds or less depending on your GPU and network: 
-        
-        ```python
-        from clip_client import Client
-        
-        c = Client('grpc://0.0.0.0:51000')
-        
-        r = c.encode(da, show_progress=True)
-        ```
-        
-        <details>
-        <summary>Download the pre-encoded dataset</summary>
-        
-        Again, for people who are impatient or don't have a GPU, we have prepared a pre-encoded text dataset:
-        
-        ```python
-        from docarray import DocumentArray
-        
-        da = DocumentArray.pull('ttl-textual', show_progress=True, local_cache=True)
-        ```
-        
-        </details>
-        
-        #### Search via image
-        
-        Let's load our previously stored image embedding, randomly sample 10 image Documents, then find top-1 nearest neighbour of each.
-        
-        ```python
-        from docarray import DocumentArray
-        
-        img_da = DocumentArray.load_binary('ttl-image')
-        
-        for d in img_da.sample(10):
-            print(da.find(d.embedding, limit=1)[0].text)
-        ```
-        
-        #### Showcase
-        
-        Fun time! Note, unlike the previous example, here the input is an image and the sentence is the output. All sentences come from the book "Pride and Prejudice". 
-        
-        <table>
-        <tr>
-        <td>
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Besides,-there-was-truth-in-his-looks.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Gardiner-smiled.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/what’s-his-name.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/By-tea-time,-however,-the-dose-had-been-enough,-and-Mr.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/You-do-not-look-well.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        </tr>
-        <tr>
-        <td>Besides, there was truth in his looks</td>
-        <td>Gardiner smiled</td>
-        <td>what’s his name</td>
-        <td>By tea time, however, the dose had been enough, and Mr</td>
-        <td>You do not look well</td>
-        </tr>
-        </table>
-        
-        <table>
-        <tr>
-        <td>
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/“A-gamester!”-she-cried.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/If-you-mention-my-name-at-the-Bell,-you-will-be-attended-to.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Never-mind-Miss-Lizzy’s-hair.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Elizabeth-will-soon-be-the-wife-of-Mr.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        
-        <td>
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/I-saw-them-the-night-before-last.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
-        </p>
-        
-        </td>
-        </tr>
-        <tr>
-        <td>“A gamester!” she cried</td>
-        <td>If you mention my name at the Bell, you will be attended to</td>
-        <td>Never mind Miss Lizzy’s hair</td>
-        <td>Elizabeth will soon be the wife of Mr</td>
-        <td>I saw them the night before last</td>
-        </tr>
-        </table>
-        
-        
-        
-        ### Rank image-text matches via CLIP model
-        
-        From `0.3.0` CLIP-as-service adds a new `/rank` endpoint that re-ranks cross-modal matches according to their joint likelihood in CLIP model. For example, given an image Document with some predefined sentence matches as below:
-        
-        ```python
-        from clip_client import Client
-        from docarray import Document
-        
-        c = Client(server='grpc://0.0.0.0:51000')
-        r = c.rank(
-            [
-                Document(
-                    uri='.github/README-img/rerank.png',
-                    matches=[
-                        Document(text=f'a photo of a {p}')
-                        for p in (
-                            'control room',
-                            'lecture room',
-                            'conference room',
-                            'podium indoor',
-                            'television studio',
-                        )
-                    ],
-                )
-            ]
-        )
-        
-        print(r['@m', ['text', 'scores__clip_score__value']])
-        ```
-        
-        ```text
-        [['a photo of a television studio', 'a photo of a conference room', 'a photo of a lecture room', 'a photo of a control room', 'a photo of a podium indoor'], 
-        [0.9920725226402283, 0.006038925610482693, 0.0009973491542041302, 0.00078492151806131, 0.00010626466246321797]]
-        ```
-        
-        One can see now `a photo of a television studio` is ranked to the top with `clip_score` score at `0.992`. In practice, one can use this endpoint to re-rank the matching result from another search system, for improving the cross-modal search quality.
-        
-        <table>
-        <tr>
-        <td>
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/rerank.png?raw=true" alt="Rerank endpoint image input" height="150px">
-        </td>
-        <td>
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/rerank-chart.svg?raw=true" alt="Rerank endpoint output">
-        </td>
-        </tr>
-        </table>
-        
-        ### Rank text-image matches via CLIP model
-        
-        In the [DALL·E Flow](https://github.com/jina-ai/dalle-flow) project, CLIP is called for ranking the generated results from DALL·E. [It has an Executor wrapped on top of `clip-client`](https://github.com/jina-ai/dalle-flow/blob/main/executors/rerank/executor.py), which calls `.arank()` - the async version of `.rank()`:
-        
-        ```python
-        from clip_client import Client
-        from jina import Executor, requests, DocumentArray
-        
-        
-        class ReRank(Executor):
-            def __init__(self, clip_server: str, **kwargs):
-                super().__init__(**kwargs)
-                self._client = Client(server=clip_server)
-        
-            @requests(on='/')
-            async def rerank(self, docs: DocumentArray, **kwargs):
-                return await self._client.arank(docs)
-        ```
-        
-        <p align="center">
-        <img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/client-dalle.png?raw=true" alt="CLIP-as-service used in DALLE Flow" width="300px">
-        </p>
-        
-        Intrigued? That's only scratching the surface of what CLIP-as-service is capable of. [Read our docs to learn more](https://clip-as-service.jina.ai).
-        
-        <!-- start support-pitch -->
-        ## Support
-        
-        - Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
-        - Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina's new features.
-            - **When?** The second Tuesday of every month
-            - **Where?**
-              Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
-              and [live stream on YouTube](https://youtube.com/c/jina-ai)
-        - Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
-        
-        ## Join Us
-        
-        CLIP-as-service is backed by [Jina AI](https://jina.ai) and licensed under [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI engineers, solution engineers to build the next neural search ecosystem in open-source.
-        
-        <!-- end support-pitch -->
-        
 Keywords: jina openai clip deep-learning cross-modal multi-modal neural-search
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
@@ -801,7 +36,774 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: flash-attn
 Provides-Extra: onnx
 Provides-Extra: search
 Provides-Extra: tensorrt
 Provides-Extra: transformers
+
+<p align="center">
+<br>
+<br>
+<br>
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/docs/_static/logo-light.svg?raw=true" alt="CLIP-as-service logo: The data structure for unstructured data" width="200px">
+<br>
+<br>
+<br>
+<b>Embed images and sentences into fixed-length vectors with CLIP</b>
+</p>
+
+<p align=center>
+<a href="https://pypi.org/project/clip_server/"><img alt="PyPI" src="https://img.shields.io/pypi/v/clip_server?label=Release&style=flat-square"></a>
+<a href="https://slack.jina.ai"><img src="https://img.shields.io/badge/Slack-3.1k-blueviolet?logo=slack&amp;logoColor=white&style=flat-square"></a>
+<a href="https://codecov.io/gh/jina-ai/clip-as-service"><img alt="Codecov branch" src="https://img.shields.io/codecov/c/github/jina-ai/clip-as-service/main?logo=Codecov&logoColor=white&style=flat-square"></a>
+<a href="https://colab.research.google.com/github/jina-ai/clip-as-service/blob/main/docs/hosting/cas-on-colab.ipynb"><img src="https://img.shields.io/badge/Host-on%20Google%20Colab%20(GPU/TPU)-brightgreen?style=flat-square&logo=googlecolab&&logoColor=white" alt="Host on Google Colab with GPU/TPU support"></a>
+</p>
+
+<!-- start elevator-pitch -->
+
+CLIP-as-service is a low-latency high-scalability service for embedding images and text. It can be easily integrated as a microservice into neural search solutions.
+
+⚡ **Fast**: Serve CLIP models with TensorRT, ONNX runtime and PyTorch w/o JIT with 800QPS<sup>[*]</sup>. Non-blocking duplex streaming on requests and responses, designed for large data and long-running tasks. 
+
+🫐 **Elastic**: Horizontally scale up and down multiple CLIP models on single GPU, with automatic load balancing.
+
+🐥 **Easy-to-use**: No learning curve, minimalist design on client and server. Intuitive and consistent API for image and sentence embedding. 
+
+👒 **Modern**: Async client support. Easily switch between gRPC, HTTP, WebSocket protocols with TLS and compression.
+
+🍱 **Integration**: Smooth integration with neural search ecosystem including [Jina](https://github.com/jina-ai/jina) and [DocArray](https://github.com/jina-ai/docarray). Build cross-modal and multi-modal solutions in no time. 
+
+<sup>[*] with default config (single replica, PyTorch no JIT) on GeForce RTX 3090. </sup>
+
+<!-- end elevator-pitch -->
+
+## Try it!
+
+An always-online server `api.clip.jina.ai` loaded with `ViT-L-14-336::openai` is there for you to play & test.
+Before you start, make sure you have obtained an access token from our [console website](https://console.clip.jina.ai/get_started), 
+or via CLI as described in [this guide](https://docs.jina.ai/jina-ai-cloud/login/#create-a-new-pat).
+
+```bash 
+jina auth token create <name of PAT> -e <expiration days>
+```
+
+Then, you need to configure the access token in the parameter `credential` of the client in python or set it in the HTTP request header `Authorization` as `<your access token>`.
+
+⚠️ Our demo server `demo-cas.jina.ai` is sunset and no longer available after **15th of Sept 2022**. 
+
+
+### Text & image embedding
+
+<table>
+<tr>
+<td> via HTTPS 🔐 </td>
+<td> via gRPC 🔐⚡⚡ </td>
+</tr>
+<tr>
+<td>
+
+```bash
+curl \
+-X POST https://api.clip.jina.ai:8443/post \
+-H 'Content-Type: application/json' \
+-H 'Authorization: <your access token>' \
+-d '{"data":[{"text": "First do it"}, 
+    {"text": "then do it right"}, 
+    {"text": "then do it better"}, 
+    {"uri": "https://picsum.photos/200"}], 
+    "execEndpoint":"/"}'
+```
+
+</td>
+<td>
+
+```python
+# pip install clip-client
+from clip_client import Client
+
+c = Client(
+    'grpcs://api.clip.jina.ai:2096', credential={'Authorization': '<your access token>'}
+)
+
+r = c.encode(
+    [
+        'First do it',
+        'then do it right',
+        'then do it better',
+        'https://picsum.photos/200',
+    ]
+)
+print(r)
+```
+</td>
+</tr>
+</table>
+
+### Visual reasoning
+
+There are four basic visual reasoning skills: object recognition, object counting, color recognition, and spatial relation understanding. Let's try some:
+
+> You need to install [`jq` (a JSON processor)](https://stedolan.github.io/jq/) to prettify the results.
+
+<table>
+<tr>
+<td> Image </td>
+<td> via HTTPS 🔐 </td>
+</tr>
+<tr>
+<td>
+<img src="https://picsum.photos/id/1/300/300">
+</td>
+<td>
+
+```bash
+curl \
+-X POST https://api.clip.jina.ai:8443/post \
+-H 'Content-Type: application/json' \
+-H 'Authorization: <your access token>' \
+-d '{"data":[{"uri": "https://picsum.photos/id/1/300/300",
+"matches": [{"text": "there is a woman in the photo"},
+            {"text": "there is a man in the photo"}]}],
+            "execEndpoint":"/rank"}' \
+| jq ".data[].matches[] | (.text, .scores.clip_score.value)"
+```
+
+gives:
+
+```
+"there is a woman in the photo"
+0.626907229423523
+"there is a man in the photo"
+0.37309277057647705
+```
+
+</td>
+</tr>
+<tr>
+<td>
+<img src="https://picsum.photos/id/133/300/300">
+</td>
+<td>
+
+```bash
+curl \
+-X POST https://api.clip.jina.ai:8443/post \
+-H 'Content-Type: application/json' \
+-H 'Authorization: <your access token>' \
+-d '{"data":[{"uri": "https://picsum.photos/id/133/300/300",
+"matches": [
+{"text": "the blue car is on the left, the red car is on the right"},
+{"text": "the blue car is on the right, the red car is on the left"},
+{"text": "the blue car is on top of the red car"},
+{"text": "the blue car is below the red car"}]}],
+"execEndpoint":"/rank"}' \
+| jq ".data[].matches[] | (.text, .scores.clip_score.value)"
+```
+
+gives:
+```
+"the blue car is on the left, the red car is on the right"
+0.5232442617416382
+"the blue car is on the right, the red car is on the left"
+0.32878655195236206
+"the blue car is below the red car"
+0.11064132302999496
+"the blue car is on top of the red car"
+0.03732786327600479
+```
+
+</td>
+</tr>
+
+
+<tr>
+<td>
+<img src="https://picsum.photos/id/102/300/300">
+</td>
+<td>
+
+```bash
+curl \
+-X POST https://api.clip.jina.ai:8443/post \
+-H 'Content-Type: application/json' \
+-H 'Authorization: <your access token>' \
+-d '{"data":[{"uri": "https://picsum.photos/id/102/300/300",
+"matches": [{"text": "this is a photo of one berry"},
+            {"text": "this is a photo of two berries"},
+            {"text": "this is a photo of three berries"},
+            {"text": "this is a photo of four berries"},
+            {"text": "this is a photo of five berries"},
+            {"text": "this is a photo of six berries"}]}],
+            "execEndpoint":"/rank"}' \
+| jq ".data[].matches[] | (.text, .scores.clip_score.value)"
+```
+
+gives:
+```
+"this is a photo of three berries"
+0.48507222533226013
+"this is a photo of four berries"
+0.2377079576253891
+"this is a photo of one berry"
+0.11304923892021179
+"this is a photo of five berries"
+0.0731358453631401
+"this is a photo of two berries"
+0.05045759305357933
+"this is a photo of six berries"
+0.04057715833187103
+```
+
+</td>
+</tr>
+
+
+</table>
+
+
+## [Documentation](https://clip-as-service.jina.ai)
+
+## Install
+
+CLIP-as-service consists of two Python packages `clip-server` and `clip-client` that can be installed _independently_. Both require Python 3.7+. 
+
+### Install server
+
+<table>
+<tr>
+<td> Pytorch Runtime ⚡ </td>
+<td> ONNX Runtime ⚡⚡</td>
+<td> TensorRT Runtime ⚡⚡⚡ </td>
+</tr>
+<tr>
+<td>
+
+```bash
+pip install clip-server
+```
+
+</td>
+<td>
+
+```bash
+pip install "clip-server[onnx]"
+```
+
+</td>
+<td>
+
+```bash
+pip install nvidia-pyindex 
+pip install "clip-server[tensorrt]"
+```
+</td>
+</tr>
+</table>
+
+You can also [host the server on Google Colab](https://clip-as-service.jina.ai/hosting/colab/), leveraging its free GPU/TPU.
+
+### Install client
+
+```bash
+pip install clip-client
+```
+
+### Quick check
+
+You can run a simple connectivity check after install.
+
+
+<table>
+<tr>
+<th> C/S </th> 
+<th> Command </th> 
+<th> Expect output </th>
+</tr>
+<tr>
+<td>
+Server
+</td>
+<td> 
+
+```bash
+python -m clip_server
+```
+     
+</td>
+<td>
+
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/server-output.svg?raw=true" alt="Expected server output" width="300px">
+
+</td>
+</tr>
+<tr>
+<td>
+Client
+</td>
+<td> 
+
+```python
+from clip_client import Client
+
+c = Client('grpc://0.0.0.0:23456')
+c.profile()
+```
+     
+</td>
+<td>
+
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/pyclient-output.svg?raw=true" alt="Expected clip-client output" width="300px">
+
+</td>
+</tr>
+</table>
+
+
+You can change `0.0.0.0` to the intranet or public IP address to test the connectivity over private and public network. 
+
+
+## Get Started
+
+### Basic usage
+
+1. Start the server: `python -m clip_server`. Remember its address and port.
+2. Create a client:
+   ```python
+    from clip_client import Client
+   
+    c = Client('grpc://0.0.0.0:51000')
+    ```
+3. To get sentence embedding:
+    ```python    
+    r = c.encode(['First do it', 'then do it right', 'then do it better'])
+    
+    print(r.shape)  # [3, 512] 
+    ```
+4. To get image embedding:
+    ```python    
+    r = c.encode(['apple.png',  # local image 
+                  'https://clip-as-service.jina.ai/_static/favicon.png',  # remote image
+                  'data:image/gif;base64,R0lGODlhEAAQAMQAAORHHOVSKudfOulrSOp3WOyDZu6QdvCchPGolfO0o/XBs/fNwfjZ0frl3/zy7////wAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACH5BAkAABAALAAAAAAQABAAAAVVICSOZGlCQAosJ6mu7fiyZeKqNKToQGDsM8hBADgUXoGAiqhSvp5QAnQKGIgUhwFUYLCVDFCrKUE1lBavAViFIDlTImbKC5Gm2hB0SlBCBMQiB0UjIQA7'])  # in image URI
+    
+    print(r.shape)  # [3, 512]
+    ```
+
+More comprehensive server and client user guides can be found in the [docs](https://clip-as-service.jina.ai/).
+
+### Text-to-image cross-modal search in 10 lines
+
+Let's build a text-to-image search using CLIP-as-service. Namely, a user can input a sentence and the program returns matching images. We'll use the [Totally Looks Like](https://sites.google.com/view/totally-looks-like-dataset) dataset and [DocArray](https://github.com/jina-ai/docarray) package. Note that DocArray is included within `clip-client` as an upstream dependency, so you don't need to install it separately.
+
+#### Load images
+
+First we load images. You can simply pull them from Jina Cloud:
+
+```python
+from docarray import DocumentArray
+
+da = DocumentArray.pull('ttl-original', show_progress=True, local_cache=True)
+```
+
+<details>
+<summary>or download TTL dataset, unzip, load manually</summary>
+
+Alternatively, you can go to [Totally Looks Like](https://sites.google.com/view/totally-looks-like-dataset) official website, unzip and load images:
+
+```python
+from docarray import DocumentArray
+
+da = DocumentArray.from_files(['left/*.jpg', 'right/*.jpg'])
+```
+
+</details>
+
+The dataset contains 12,032 images, so it may take a while to pull. Once done, you can visualize it and get the first taste of those images:
+
+```python
+da.plot_image_sprites()
+```
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/ttl-image-sprites.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="50%">
+</p>
+
+#### Encode images
+
+Start the server with `python -m clip_server`. Let's say it's at `0.0.0.0:51000` with `GRPC` protocol (you will get this information after running the server).
+
+Create a Python client script:
+
+```python
+from clip_client import Client
+
+c = Client(server='grpc://0.0.0.0:51000')
+
+da = c.encode(da, show_progress=True)
+```
+
+Depending on your GPU and client-server network, it may take a while to embed 12K images. In my case, it took about two minutes.
+
+<details>
+<summary>Download the pre-encoded dataset</summary>
+
+If you're impatient or don't have a GPU, waiting can be Hell. In this case, you can simply pull our pre-encoded image dataset:
+
+```python
+from docarray import DocumentArray
+
+da = DocumentArray.pull('ttl-embedding', show_progress=True, local_cache=True)
+```
+
+</details>
+
+#### Search via sentence 
+
+Let's build a simple prompt to allow a user to type sentence:
+
+```python
+while True:
+    vec = c.encode([input('sentence> ')])
+    r = da.find(query=vec, limit=9)
+    r[0].plot_image_sprites()
+```
+
+#### Showcase
+
+Now you can input arbitrary English sentences and view the top-9 matching images. Search is fast and instinctive. Let's have some fun:
+
+<table>
+<tr>
+<th> "a happy potato" </th> 
+<th> "a super evil AI" </th> 
+<th> "a guy enjoying his burger" </th>
+</tr>
+<tr>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-happy-potato.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-super-evil-AI.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/a-guy-enjoying-his-burger.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+</tr>
+</table>
+
+
+<table>
+<tr>
+<th> "professor cat is very serious" </th> 
+<th> "an ego engineer lives with parent" </th> 
+<th> "there will be no tomorrow so lets eat unhealthy" </th>
+</tr>
+<tr>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/professor-cat-is-very-serious.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/an-ego-engineer-lives-with-parent.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/there-will-be-no-tomorrow-so-lets-eat-unhealthy.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" width="100%">
+</p>
+
+</td>
+</tr>
+</table>
+
+Let's save the embedding result for our next example: 
+
+```python
+da.save_binary('ttl-image')
+```
+
+### Image-to-text cross-modal search in 10 Lines
+
+We can also switch the input and output of the last program to achieve image-to-text search. Precisely, given a query image find the sentence that best describes the image.
+
+Let's use all sentences from the book "Pride and Prejudice". 
+
+```python
+from docarray import Document, DocumentArray
+
+d = Document(uri='https://www.gutenberg.org/files/1342/1342-0.txt').load_uri_to_text()
+da = DocumentArray(
+    Document(text=s.strip()) for s in d.text.replace('\r\n', '').split('.') if s.strip()
+)
+```
+
+Let's look at what we got:
+
+```python
+da.summary()
+```
+
+```text
+            Documents Summary            
+                                         
+  Length                 6403            
+  Homogenous Documents   True            
+  Common Attributes      ('id', 'text')  
+                                         
+                     Attributes Summary                     
+                                                            
+  Attribute   Data type   #Unique values   Has empty value  
+ ────────────────────────────────────────────────────────── 
+  id          ('str',)    6403             False            
+  text        ('str',)    6030             False            
+```
+
+#### Encode sentences
+
+Now encode these 6,403 sentences, it may take 10 seconds or less depending on your GPU and network: 
+
+```python
+from clip_client import Client
+
+c = Client('grpc://0.0.0.0:51000')
+
+r = c.encode(da, show_progress=True)
+```
+
+<details>
+<summary>Download the pre-encoded dataset</summary>
+
+Again, for people who are impatient or don't have a GPU, we have prepared a pre-encoded text dataset:
+
+```python
+from docarray import DocumentArray
+
+da = DocumentArray.pull('ttl-textual', show_progress=True, local_cache=True)
+```
+
+</details>
+
+#### Search via image
+
+Let's load our previously stored image embedding, randomly sample 10 image Documents, then find top-1 nearest neighbour of each.
+
+```python
+from docarray import DocumentArray
+
+img_da = DocumentArray.load_binary('ttl-image')
+
+for d in img_da.sample(10):
+    print(da.find(d.embedding, limit=1)[0].text)
+```
+
+#### Showcase
+
+Fun time! Note, unlike the previous example, here the input is an image and the sentence is the output. All sentences come from the book "Pride and Prejudice". 
+
+<table>
+<tr>
+<td>
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Besides,-there-was-truth-in-his-looks.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Gardiner-smiled.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/what’s-his-name.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/By-tea-time,-however,-the-dose-had-been-enough,-and-Mr.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/You-do-not-look-well.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+</tr>
+<tr>
+<td>Besides, there was truth in his looks</td>
+<td>Gardiner smiled</td>
+<td>what’s his name</td>
+<td>By tea time, however, the dose had been enough, and Mr</td>
+<td>You do not look well</td>
+</tr>
+</table>
+
+<table>
+<tr>
+<td>
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/“A-gamester!”-she-cried.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/If-you-mention-my-name-at-the-Bell,-you-will-be-attended-to.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Never-mind-Miss-Lizzy’s-hair.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/Elizabeth-will-soon-be-the-wife-of-Mr.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+
+<td>
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/I-saw-them-the-night-before-last.png?raw=true" alt="Visualization of the image sprite of Totally looks like dataset" height="100px">
+</p>
+
+</td>
+</tr>
+<tr>
+<td>“A gamester!” she cried</td>
+<td>If you mention my name at the Bell, you will be attended to</td>
+<td>Never mind Miss Lizzy’s hair</td>
+<td>Elizabeth will soon be the wife of Mr</td>
+<td>I saw them the night before last</td>
+</tr>
+</table>
+
+
+
+### Rank image-text matches via CLIP model
+
+From `0.3.0` CLIP-as-service adds a new `/rank` endpoint that re-ranks cross-modal matches according to their joint likelihood in CLIP model. For example, given an image Document with some predefined sentence matches as below:
+
+```python
+from clip_client import Client
+from docarray import Document
+
+c = Client(server='grpc://0.0.0.0:51000')
+r = c.rank(
+    [
+        Document(
+            uri='.github/README-img/rerank.png',
+            matches=[
+                Document(text=f'a photo of a {p}')
+                for p in (
+                    'control room',
+                    'lecture room',
+                    'conference room',
+                    'podium indoor',
+                    'television studio',
+                )
+            ],
+        )
+    ]
+)
+
+print(r['@m', ['text', 'scores__clip_score__value']])
+```
+
+```text
+[['a photo of a television studio', 'a photo of a conference room', 'a photo of a lecture room', 'a photo of a control room', 'a photo of a podium indoor'], 
+[0.9920725226402283, 0.006038925610482693, 0.0009973491542041302, 0.00078492151806131, 0.00010626466246321797]]
+```
+
+One can see now `a photo of a television studio` is ranked to the top with `clip_score` score at `0.992`. In practice, one can use this endpoint to re-rank the matching result from another search system, for improving the cross-modal search quality.
+
+<table>
+<tr>
+<td>
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/rerank.png?raw=true" alt="Rerank endpoint image input" height="150px">
+</td>
+<td>
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/rerank-chart.svg?raw=true" alt="Rerank endpoint output">
+</td>
+</tr>
+</table>
+
+### Rank text-image matches via CLIP model
+
+In the [DALL·E Flow](https://github.com/jina-ai/dalle-flow) project, CLIP is called for ranking the generated results from DALL·E. [It has an Executor wrapped on top of `clip-client`](https://github.com/jina-ai/dalle-flow/blob/main/executors/rerank/executor.py), which calls `.arank()` - the async version of `.rank()`:
+
+```python
+from clip_client import Client
+from jina import Executor, requests, DocumentArray
+
+
+class ReRank(Executor):
+    def __init__(self, clip_server: str, **kwargs):
+        super().__init__(**kwargs)
+        self._client = Client(server=clip_server)
+
+    @requests(on='/')
+    async def rerank(self, docs: DocumentArray, **kwargs):
+        return await self._client.arank(docs)
+```
+
+<p align="center">
+<img src="https://github.com/jina-ai/clip-as-service/blob/main/.github/README-img/client-dalle.png?raw=true" alt="CLIP-as-service used in DALLE Flow" width="300px">
+</p>
+
+Intrigued? That's only scratching the surface of what CLIP-as-service is capable of. [Read our docs to learn more](https://clip-as-service.jina.ai).
+
+<!-- start support-pitch -->
+## Support
+
+- Join our [Slack community](https://slack.jina.ai) and chat with other community members about ideas.
+- Join our [Engineering All Hands](https://youtube.com/playlist?list=PL3UBBWOUVhFYRUa_gpYYKBqEAkO4sxmne) meet-up to discuss your use case and learn Jina's new features.
+    - **When?** The second Tuesday of every month
+    - **Where?**
+      Zoom ([see our public events calendar](https://calendar.google.com/calendar/embed?src=c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com&ctz=Europe%2FBerlin)/[.ical](https://calendar.google.com/calendar/ical/c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics))
+      and [live stream on YouTube](https://youtube.com/c/jina-ai)
+- Subscribe to the latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
+
+## Join Us
+
+CLIP-as-service is backed by [Jina AI](https://jina.ai) and licensed under [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai) AI engineers, solution engineers to build the next neural search ecosystem in open-source.
+
+<!-- end support-pitch -->
+
+
```

#### html2text {}

```diff
@@ -1,14 +1,33 @@
-Metadata-Version: 2.1 Name: clip-server Version: 0.8.2.dev6 Summary: Embed
+Metadata-Version: 2.1 Name: clip-server Version: 0.8.2.dev9 Summary: Embed
 images and sentences into fixed-length vectors via CLIP Home-page: https://
 github.com/jina-ai/clip-as-service Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/clip-as-service/
 tags Project-URL: Documentation, https://clip-as-service.jina.ai Project-URL:
 Source, https://github.com/jina-ai/clip-as-service/ Project-URL: Tracker,
-https://github.com/jina-ai/clip-as-service/issues Description:
+https://github.com/jina-ai/clip-as-service/issues Keywords: jina openai clip
+deep-learning cross-modal multi-modal neural-search Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Education Classifier:
+Intended Audience :: Science/Research Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Unix Shell Classifier:
+Environment :: Console Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Classifier: Topic ::
+Database :: Database Engines/Servers Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Internet :: WWW/
+HTTP :: Indexing/Search Classifier: Topic :: Scientific/Engineering :: Image
+Recognition Classifier: Topic :: Multimedia :: Video Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Description-Content-Type: text/markdown Provides-
+Extra: flash-attn Provides-Extra: onnx Provides-Extra: search Provides-Extra:
+tensorrt Provides-Extra: transformers
 
 
 
        [CLIP-as-service logo: The data structure for unstructured data]
 
 
         Embed images and sentences into fixed-length vectors with CLIP
@@ -272,27 +291,8 @@
 [.ical](https://calendar.google.com/calendar/ical/
 c_1t5ogfp2d45v8fit981j08mcm4%40group.calendar.google.com/public/basic.ics)) and
 [live stream on YouTube](https://youtube.com/c/jina-ai) - Subscribe to the
 latest video tutorials on our [YouTube channel](https://youtube.com/c/jina-ai)
 ## Join Us CLIP-as-service is backed by [Jina AI](https://jina.ai) and licensed
 under [Apache-2.0](./LICENSE). [We are actively hiring](https://jobs.jina.ai)
 AI engineers, solution engineers to build the next neural search ecosystem in
-open-source.  Keywords: jina openai clip deep-learning cross-modal multi-modal
-neural-search Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Education Classifier: Intended Audience :: Science/
-Research Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Unix Shell Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: OS Independent Classifier: Topic :: Database :: Database
-Engines/Servers Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Scientific/Engineering :: Image Recognition Classifier:
-Topic :: Multimedia :: Video Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
-Software Development Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown Provides-Extra: flash-attn Provides-
-Extra: onnx Provides-Extra: search Provides-Extra: tensorrt Provides-Extra:
-transformers
+open-source.
```

### Comparing `clip-server-0.8.2.dev6/clip_server.egg-info/SOURCES.txt` & `clip-server-0.8.2.dev9/clip_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clip-server-0.8.2.dev6/setup.py` & `clip-server-0.8.2.dev9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 from os import path
 
-from setuptools import find_packages
-from setuptools import setup
+from setuptools import find_packages, setup
 
 if sys.version_info < (3, 7, 0):
     raise OSError(f'CLIP-as-service requires Python >=3.7, but yours is {sys.version}')
 
 try:
     pkg_name = 'clip-server'
     libinfo_py = path.join(
@@ -42,15 +41,15 @@
     zip_safe=False,
     setup_requires=['setuptools>=18.0', 'wheel'],
     install_requires=[
         'ftfy',
         'torch',
         'regex',
         'torchvision<=0.13.0' if sys.version_info <= (3, 7, 2) else 'torchvision',
-        'jina>=3.8.0',
+        'jina>=3.12.0',
         'prometheus-client',
         'open_clip_torch>=2.7.0',
     ],
     extras_require={
         'onnx': [
             'onnxruntime',
             'onnx',
```

