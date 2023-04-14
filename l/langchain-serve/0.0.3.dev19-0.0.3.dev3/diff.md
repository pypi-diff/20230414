# Comparing `tmp/langchain-serve-0.0.3.dev19.tar.gz` & `tmp/langchain-serve-0.0.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-serve-0.0.3.dev19.tar", last modified: Fri Apr 14 18:32:51 2023, max compression
+gzip compressed data, was "langchain-serve-0.0.3.dev3.tar", last modified: Fri Apr  7 06:22:00 2023, max compression
```

## Comparing `langchain-serve-0.0.3.dev19.tar` & `langchain-serve-0.0.3.dev3.tar`

### file list

```diff
@@ -1,56 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:51.188079 langchain-serve-0.0.3.dev19/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    27093 2023-04-14 18:32:51.184078 langchain-serve-0.0.3.dev19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25843 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:51.184078 langchain-serve-0.0.3.dev19/langchain_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27093 2023-04-14 18:32:51.000000 langchain-serve-0.0.3.dev19/langchain_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-14 18:32:51.000000 langchain-serve-0.0.3.dev19/langchain_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:32:51.000000 langchain-serve-0.0.3.dev19/langchain_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 18:32:51.000000 langchain-serve-0.0.3.dev19/langchain_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:32:51.000000 langchain-serve-0.0.3.dev19/langchain_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 18:32:51.000000 langchain-serve-0.0.3.dev19/langchain_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 18:32:51.000000 langchain-serve-0.0.3.dev19/langchain_serve.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:51.184078 langchain-serve-0.0.3.dev19/lcserve/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 18:32:50.000000 langchain-serve-0.0.3.dev19/lcserve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/agent-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:51.180078 langchain-serve-0.0.3.dev19/lcserve/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:51.184078 langchain-serve-0.0.3.dev19/lcserve/apps/babyagi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/apps/babyagi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/apps/babyagi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/apps/babyagi/babyagi.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/apps/babyagi/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:51.184078 langchain-serve-0.0.3.dev19/lcserve/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/agentexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:51.184078 langchain-serve-0.0.3.dev19/lcserve/backend/playground/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/playground/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/playground/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:51.184078 langchain-serve-0.0.3.dev19/lcserve/backend/playground/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/playground/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/playground/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/playground/utils/langchain_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/playground/utils/talk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/backend/playground/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/customgateway.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/customgateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/flow.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:51.180078 langchain-serve-0.0.3.dev19/lcserve/playground/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:32:51.184078 langchain-serve-0.0.3.dev19/lcserve/playground/babyagi/
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/playground/babyagi/playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/playground/babyagi/user_input.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/playgroundgateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/servinggateway.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/lcserve/servinggateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:32:51.188079 langchain-serve-0.0.3.dev19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-14 18:32:45.000000 langchain-serve-0.0.3.dev19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:22:00.763548 langchain-serve-0.0.3.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26707 2023-04-07 06:22:00.763548 langchain-serve-0.0.3.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:22:00.763548 langchain-serve-0.0.3.dev3/langchain_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26707 2023-04-07 06:22:00.000000 langchain-serve-0.0.3.dev3/langchain_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-07 06:22:00.000000 langchain-serve-0.0.3.dev3/langchain_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 06:22:00.000000 langchain-serve-0.0.3.dev3/langchain_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 06:22:00.000000 langchain-serve-0.0.3.dev3/langchain_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 06:22:00.000000 langchain-serve-0.0.3.dev3/langchain_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 06:22:00.000000 langchain-serve-0.0.3.dev3/langchain_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 06:22:00.000000 langchain-serve-0.0.3.dev3/langchain_serve.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:22:00.763548 langchain-serve-0.0.3.dev3/lcserve/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-07 06:22:00.000000 langchain-serve-0.0.3.dev3/lcserve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/agent-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:22:00.763548 langchain-serve-0.0.3.dev3/lcserve/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/agentexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21956 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:22:00.763548 langchain-serve-0.0.3.dev3/lcserve/backend/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/playground/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/playground/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 06:22:00.763548 langchain-serve-0.0.3.dev3/lcserve/backend/playground/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/playground/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/playground/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/playground/utils/langchain_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/playground/utils/talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/backend/playground/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/customgateway.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/customgateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/flow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/playgroundgateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/servinggateway.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/lcserve/servinggateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 06:22:00.763548 langchain-serve-0.0.3.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-07 06:21:57.000000 langchain-serve-0.0.3.dev3/setup.py
```

### Comparing `langchain-serve-0.0.3.dev19/LICENSE` & `langchain-serve-0.0.3.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.3.dev19/PKG-INFO` & `langchain-serve-0.0.3.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-serve
-Version: 0.0.3.dev19
+Version: 0.0.3.dev3
 Summary: Langchain Serve - serve your langchain apps on Jina AI Cloud.
 Home-page: https://github.com/jina-ai/langchain-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/langchain-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -30,32 +30,15 @@
 # LangChain Apps on Production with Jina 🚀
 
 [Jina](https://github.com/jina-ai/jina) is an open-source framework to build, deploy & manage machine learning applications at scale. [LangChain](https://python.langchain.com/en/latest/index.html) is another open-source framework for building applications powered by language models. 
 
 **langchain-serve** helps you deploy your LangChain apps on Jina AI Cloud in just a matter of seconds. You can now benefit from the scalability and serverless architecture of the cloud without sacrificing the ease and convenience of local development.
 
 
-## 🧠 Babyagi-as-a-service
-
-- Deploy `babyagi` on Jina AI Cloud with one command
-
-  ```bash
-  lc-serve deploy babyagi
-  ```
-
-- Integrate babyagi with external services using our Websocket API. Get a flavor of the integration on your CLI with 
-    
-  ```bash
-  lc-serve playground babyagi
-  ```
-
-![Babyagi-as-a-service Playground](.github/images/babyagi-playground.gif)
-
-
-#### 🎉 Custom Apps to production in 4 simple steps
+#### 🎉 To production in 4 simple steps
 
   1. Refactor your code to function(s) that should be served with `@serving` decorator.
   1. Create a `requirements.txt` file in your app directory to ensure all necessary dependencies are installed.
   1. Run `lc-serve deploy local app` to test your API locally.
   1. Run `lc-serve deploy jcloud app` to deploy on [Jina AI Cloud](https://jina.ai/product/cloud/).
```

### Comparing `langchain-serve-0.0.3.dev19/README.md` & `langchain-serve-0.0.3.dev3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,15 @@
 # LangChain Apps on Production with Jina 🚀
 
 [Jina](https://github.com/jina-ai/jina) is an open-source framework to build, deploy & manage machine learning applications at scale. [LangChain](https://python.langchain.com/en/latest/index.html) is another open-source framework for building applications powered by language models. 
 
 **langchain-serve** helps you deploy your LangChain apps on Jina AI Cloud in just a matter of seconds. You can now benefit from the scalability and serverless architecture of the cloud without sacrificing the ease and convenience of local development.
 
 
-## 🧠 Babyagi-as-a-service
-
-- Deploy `babyagi` on Jina AI Cloud with one command
-
-  ```bash
-  lc-serve deploy babyagi
-  ```
-
-- Integrate babyagi with external services using our Websocket API. Get a flavor of the integration on your CLI with 
-    
-  ```bash
-  lc-serve playground babyagi
-  ```
-
-![Babyagi-as-a-service Playground](.github/images/babyagi-playground.gif)
-
-
-#### 🎉 Custom Apps to production in 4 simple steps
+#### 🎉 To production in 4 simple steps
 
   1. Refactor your code to function(s) that should be served with `@serving` decorator.
   1. Create a `requirements.txt` file in your app directory to ensure all necessary dependencies are installed.
   1. Run `lc-serve deploy local app` to test your API locally.
   1. Run `lc-serve deploy jcloud app` to deploy on [Jina AI Cloud](https://jina.ai/product/cloud/).
```

### Comparing `langchain-serve-0.0.3.dev19/langchain_serve.egg-info/PKG-INFO` & `langchain-serve-0.0.3.dev3/langchain_serve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-serve
-Version: 0.0.3.dev19
+Version: 0.0.3.dev3
 Summary: Langchain Serve - serve your langchain apps on Jina AI Cloud.
 Home-page: https://github.com/jina-ai/langchain-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/langchain-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -30,32 +30,15 @@
 # LangChain Apps on Production with Jina 🚀
 
 [Jina](https://github.com/jina-ai/jina) is an open-source framework to build, deploy & manage machine learning applications at scale. [LangChain](https://python.langchain.com/en/latest/index.html) is another open-source framework for building applications powered by language models. 
 
 **langchain-serve** helps you deploy your LangChain apps on Jina AI Cloud in just a matter of seconds. You can now benefit from the scalability and serverless architecture of the cloud without sacrificing the ease and convenience of local development.
 
 
-## 🧠 Babyagi-as-a-service
-
-- Deploy `babyagi` on Jina AI Cloud with one command
-
-  ```bash
-  lc-serve deploy babyagi
-  ```
-
-- Integrate babyagi with external services using our Websocket API. Get a flavor of the integration on your CLI with 
-    
-  ```bash
-  lc-serve playground babyagi
-  ```
-
-![Babyagi-as-a-service Playground](.github/images/babyagi-playground.gif)
-
-
-#### 🎉 Custom Apps to production in 4 simple steps
+#### 🎉 To production in 4 simple steps
 
   1. Refactor your code to function(s) that should be served with `@serving` decorator.
   1. Create a `requirements.txt` file in your app directory to ensure all necessary dependencies are installed.
   1. Run `lc-serve deploy local app` to test your API locally.
   1. Run `lc-serve deploy jcloud app` to deploy on [Jina AI Cloud](https://jina.ai/product/cloud/).
```

### Comparing `langchain-serve-0.0.3.dev19/langchain_serve.egg-info/SOURCES.txt` & `langchain-serve-0.0.3.dev3/langchain_serve.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,26 +19,20 @@
 lcserve/customgateway_config.yml
 lcserve/flow.py
 lcserve/flow.yml
 lcserve/playgroundgateway_config.yml
 lcserve/requirements.txt
 lcserve/servinggateway.Dockerfile
 lcserve/servinggateway_config.yml
-lcserve/apps/babyagi/__init__.py
-lcserve/apps/babyagi/app.py
-lcserve/apps/babyagi/babyagi.py
-lcserve/apps/babyagi/requirements.txt
 lcserve/backend/__init__.py
 lcserve/backend/agentexecutor.py
 lcserve/backend/decorators.py
 lcserve/backend/gateway.py
 lcserve/backend/nginx.conf
 lcserve/backend/playground/__init__.py
 lcserve/backend/playground/app.py
 lcserve/backend/playground/config.toml
 lcserve/backend/playground/utils/__init__.py
 lcserve/backend/playground/utils/helper.py
 lcserve/backend/playground/utils/langchain_helper.py
 lcserve/backend/playground/utils/talk.py
-lcserve/backend/playground/utils/tools.py
-lcserve/playground/babyagi/playground.py
-lcserve/playground/babyagi/user_input.py
+lcserve/backend/playground/utils/tools.py
```

### Comparing `langchain-serve-0.0.3.dev19/lcserve/__main__.py` & `langchain-serve-0.0.3.dev3/lcserve/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,59 @@
-import os
-import sys
 from typing import List, Union
 
 import click
 from jcloud.constants import Phase
 from jina import Flow
 
 from .flow import (
     APP_NAME,
-    BABYAGI_APP_NAME,
     deploy_app_on_jcloud,
     get_app_status_on_jcloud,
     get_flow_dict,
     get_flow_yaml,
     list_apps_on_jcloud,
     push_app_to_hubble,
     remove_app_on_jcloud,
     syncify,
 )
 
 
 def serve_locally(module: Union[str, List[str]], port: int = 8080):
-    sys.path.append(os.getcwd())
     f_yaml = get_flow_yaml(module, jcloud=False, port=port)
     with Flow.load_config(f_yaml) as f:
         # TODO: add local description
         f.block()
 
 
 async def serve_on_jcloud(
     module: Union[str, List[str]],
     name: str = APP_NAME,
-    requirements: List[str] = None,
     app_id: str = None,
     verbose: bool = False,
 ):
     from .backend.playground.utils.helper import get_random_tag
 
     tag = get_random_tag()
-    gateway_id_wo_tag, is_websocket = push_app_to_hubble(
-        module,
-        requirements=requirements,
-        tag=tag,
-        verbose=verbose,
-    )
+    gateway_id_wo_tag, websocket = push_app_to_hubble(module, tag=tag, verbose=verbose)
     app_id, endpoint = await deploy_app_on_jcloud(
         flow_dict=get_flow_dict(
             module=module,
             jcloud=True,
             port=8080,
             name=name,
             app_id=app_id,
             gateway_id=gateway_id_wo_tag + ':' + tag,
-            websocket=is_websocket,
+            websocket=websocket,
         ),
         app_id=app_id,
         verbose=verbose,
     )
     await get_app_status_on_jcloud(app_id=app_id)
 
 
-async def serve_babyagi_on_jcloud(
-    name: str = BABYAGI_APP_NAME,
-    requirements: List[str] = None,
-    app_id: str = None,
-    verbose: bool = False,
-):
-    await serve_on_jcloud(
-        module='lcserve.apps.babyagi.app',
-        name=name,
-        requirements=requirements,
-        app_id=app_id,
-        verbose=verbose,
-    )
-
-
 @click.group()
 @click.help_option('-h', '--help')
 def serve():
     pass
 
 
 @serve.group(help='Deploy the app.')
@@ -132,52 +107,14 @@
 )
 @click.help_option('-h', '--help')
 @syncify
 async def jcloud(module, name, app_id, verbose):
     await serve_on_jcloud(module, name=name, app_id=app_id, verbose=verbose)
 
 
-@deploy.command(help='Deploy babyagi on JCloud.')
-@click.option(
-    '--name',
-    type=str,
-    default=BABYAGI_APP_NAME,
-    help='Name of the app.',
-    show_default=True,
-)
-@click.option(
-    '--requirements',
-    default=None,
-    help='List of requirements to be installed.',
-    multiple=True,
-)
-@click.option(
-    '--app-id',
-    type=str,
-    default=None,
-    help='AppID of the deployed agent to be updated.',
-    show_default=True,
-)
-@click.option(
-    '--verbose',
-    is_flag=True,
-    help='Verbose mode.',
-    show_default=True,
-)
-@click.help_option('-h', '--help')
-@syncify
-async def babyagi(name, requirements, app_id, verbose):
-    await serve_babyagi_on_jcloud(
-        name=name,
-        requirements=requirements,
-        app_id=app_id,
-        verbose=verbose,
-    )
-
-
 @serve.command(help='List all deployed apps.')
 @click.option(
     '--phase',
     type=str,
     default=','.join(
         [
             Phase.Serving,
@@ -215,23 +152,9 @@
 @click.argument('app-id')
 @click.help_option('-h', '--help')
 @syncify
 async def remove(app_id):
     await remove_app_on_jcloud(app_id)
 
 
-@serve.group(help='Play with predefined apps on JCloud.')
-@click.help_option('-h', '--help')
-def playground():
-    pass
-
-
-@playground.command(help='Play with babyagi on JCloud.')
-def babyagi():
-    sys.path.append(os.path.join(os.path.dirname(__file__), 'playground', 'babyagi'))
-    from .playground.babyagi.playground import play
-
-    play()
-
-
 if __name__ == "__main__":
     serve()
```

### Comparing `langchain-serve-0.0.3.dev19/lcserve/backend/agentexecutor.py` & `langchain-serve-0.0.3.dev3/lcserve/backend/agentexecutor.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.3.dev19/lcserve/backend/decorators.py` & `langchain-serve-0.0.3.dev3/lcserve/backend/decorators.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.3.dev19/lcserve/backend/gateway.py` & `langchain-serve-0.0.3.dev3/lcserve/backend/gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 import shutil
 import sys
 import time
 from enum import Enum
 from importlib import import_module
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable, Dict, List, Tuple, Type, Any
+from typing import TYPE_CHECKING, Callable, Dict, List, Tuple
 
+import uvicorn
 from docarray import Document, DocumentArray
 from jina import Gateway
-from jina.enums import ProtocolType as GatewayProtocolType
-from jina.serve.runtimes.gateway.composite import CompositeGateway
+from jina.enums import GatewayProtocolType
+from jina.serve.runtimes.gateway import CompositeGateway
 from jina.serve.runtimes.gateway.http.fastapi import FastAPIBaseGateway
 from pydantic import Field, ValidationError, create_model
 
 from .playground.utils.helper import (
     AGENT_OUTPUT,
     APPDIR,
     DEFAULT_KEY,
@@ -28,15 +29,15 @@
     Capturing,
     EnvironmentVarCtxtManager,
     parse_uses_with,
     run_cmd,
 )
 from .playground.utils.langchain_helper import (
     AsyncStreamingWebsocketCallbackHandler,
-    BuiltinsWrapper,
+    InputWrapper,
     StreamingWebsocketCallbackHandler,
 )
 
 if TYPE_CHECKING:
     from fastapi import FastAPI
 
 cur_dir = os.path.dirname(__file__)
@@ -358,70 +359,65 @@
         _name = func.__name__.title().replace('_', '')
 
         # check if _name is already registered
         if _name in [route.name for route in self.app.routes]:
             print(f'Route {_name} already registered. Skipping...')
             return
 
-        def _get_input_model_fields() -> Dict[str, Tuple[Type, Any]]:
-            _input_model_fields = {}
-            for _name, _param in inspect.signature(func).parameters.items():
-                if _param.kind == inspect.Parameter.VAR_KEYWORD:
-                    continue
-
-                if _param.annotation is inspect.Parameter.empty:
-                    raise ValueError(
-                        f'Annotation missing for parameter {_name} in function {func.__name__}. '
-                        'Please add type annotations to all parameters.'
-                    )
-
-                if _param.default is inspect.Parameter.empty:
-                    _input_model_fields[_name] = (_param.annotation, ...)
-                else:
-                    _input_model_fields[_name] = (_param.annotation, _param.default)
-
-            return _input_model_fields
+        _input_params = [
+            (name, parameter.annotation)
+            for name, parameter in inspect.signature(func).parameters.items()
+        ]
 
-        def _get_output_model_fields() -> Dict[str, Tuple[Type, Any]]:
-            def _get_result_type():
-                if 'return' in func.__annotations__:
-                    _return = func.__annotations__['return']
-                    if hasattr(
-                        _return, '__next__'
-                    ):  # if a Generator, return the first type
-                        return _return.__next__.__annotations__['return']
-                    elif _return is None:
-                        return str
-                    else:
-                        return _return
-                else:
+        _input_model_fields = {
+            name: (field_type, ...)
+            for name, field_type in _input_params
+            if name != 'kwargs'
+        }
+
+        _ws_recv_lock = asyncio.Lock()
+
+        def _get_result_type():
+            if 'return' in func.__annotations__:
+                _return = func.__annotations__['return']
+                if hasattr(
+                    _return, '__origin__'
+                ):  # if  a Generic, return the first type
+                    return _return.__args__[0]
+                elif hasattr(
+                    _return, '__next__'
+                ):  # if a Generator, return the first type
+                    return _return.__next__.__annotations__['return']
+                elif _return is None:
                     return str
+                else:
+                    return _return
+            else:
+                return str
 
-            _output_model_fields = {
-                'result': (_get_result_type(), ...),
-                'error': (str, ...),
-                'stdout': (str, Field(default='', alias='stdout')),
-            }
-
-            return _output_model_fields
+        _output_model_fields = {
+            'result': (_get_result_type(), ...),
+            'error': (str, ...),
+            'stdout': (str, Field(default='', alias='stdout')),
+        }
 
         class Config:
             arbitrary_types_allowed = True
 
         input_model = create_model(
             f'Input{_name}',
             __config__=Config,
-            **_get_input_model_fields(),
+            **_input_model_fields,
             **{'envs': (Dict[str, str], Field(default={}, alias='envs'))},
         )
 
         output_model = create_model(
             f'Output{_name}',
             __config__=Config,
-            **_get_output_model_fields(),
+            **_output_model_fields,
         )
 
         if route_type == RouteType.HTTP:
             self.logger.info(f'Registering HTTP route: {func.__name__}')
 
             @self.app.post(
                 path=f'/{func.__name__}',
@@ -454,116 +450,118 @@
 
         elif route_type == RouteType.WEBSOCKET:
             self.logger.info(f'Registering Websocket route: {func.__name__}')
             self._update_dry_run_with_ws()
 
             @self.app.websocket(path=f'/{func.__name__}', name=_name)
             async def _create_ws_route(websocket: WebSocket):
-                with BuiltinsWrapper(
-                    websocket=websocket, output_model=output_model, wrap_print=False
-                ):
-                    await websocket.accept()
-                    _ws_recv_lock = asyncio.Lock()
-                    try:
-                        while True:
-                            # if websocket is closed, break
-                            if websocket.client_state not in [
-                                WebSocketState.CONNECTED,
-                                WebSocketState.CONNECTING,
-                            ]:
-                                self.logger.info(
-                                    f'Client {websocket.client} already disconnected from `{func.__name__}`. Breaking...'
-                                )
-                                break
+                import builtins
 
-                            async with _ws_recv_lock:
-                                _data = await websocket.receive_json()
+                # replace input with a websocket input to support human-in-the-loop
+                builtins.input = InputWrapper(
+                    websocket=websocket, recv_lock=_ws_recv_lock
+                )
 
-                            try:
-                                _input_data = input_model(**_data)
-                            except ValidationError as e:
-                                self.logger.error(
-                                    f'Exception while converting data to input model: {e}'
-                                )
-                                _ws_serving_error = str(e)
-                                _data = output_model(
-                                    result='',
-                                    error=_ws_serving_error,
-                                )
-                                await websocket.send_text(_data.json())
-                                continue
+                await websocket.accept()
+                try:
+                    while True:
+                        # if websocket is closed, break
+                        if websocket.client_state not in [
+                            WebSocketState.CONNECTED,
+                            WebSocketState.CONNECTING,
+                        ]:
+                            self.logger.info(
+                                f'Client {websocket.client} already disconnected from `{func.__name__}`. Breaking...'
+                            )
+                            break
 
-                            _returned_data, _ws_serving_error = '', ''
-                            _envs = {}
-                            if hasattr(_input_data, 'envs'):
-                                _envs = _input_data.envs
-                                del _input_data.envs
-
-                            with EnvironmentVarCtxtManager(_envs):
-                                try:
-                                    _input_data_dict = dict(_input_data)
-                                    # If the function is a streaming response, we pass the callback handler,
-                                    # so that stream data can be sent back to the client.
-                                    if include_callback_handlers:
-                                        _input_data_dict.update(
-                                            {
-                                                'websocket': websocket,
-                                                'streaming_handler': StreamingWebsocketCallbackHandler(
-                                                    websocket=websocket,
-                                                    output_model=output_model,
-                                                ),
-                                                'async_streaming_handler': AsyncStreamingWebsocketCallbackHandler(
-                                                    websocket=websocket,
-                                                    output_model=output_model,
-                                                ),
-                                            }
-                                        )
+                        async with _ws_recv_lock:
+                            _data = await websocket.receive_json()
+
+                        try:
+                            _input_data = input_model(**_data)
+                        except ValidationError as e:
+                            self.logger.error(
+                                f'Exception while converting data to input model: {e}'
+                            )
+                            _ws_serving_error = str(e)
+                            _data = output_model(
+                                result='',
+                                error=_ws_serving_error,
+                            )
+                            await websocket.send_text(_data.json())
+                            continue
+
+                        _returned_data, _ws_serving_error = '', ''
+                        _envs = {}
+                        if hasattr(_input_data, 'envs'):
+                            _envs = _input_data.envs
+                            del _input_data.envs
 
-                                    _returned_data = func(**_input_data_dict)
-                                    if inspect.isgenerator(_returned_data):
-                                        # If the function is a generator, we iterate through the generator and send each item back to the client.
-                                        for _stream in _returned_data:
-                                            _data = output_model(
-                                                result=_stream,
-                                                error=_ws_serving_error,
-                                            )
-                                            await websocket.send_text(_data.json())
+                        with EnvironmentVarCtxtManager(_envs):
+                            try:
+                                _input_data_dict = dict(_input_data)
+                                # If the function is a streaming response, we pass the callback handler,
+                                # so that stream data can be sent back to the client.
+                                if include_callback_handlers:
+                                    _input_data_dict.update(
+                                        {
+                                            'streaming_handler': StreamingWebsocketCallbackHandler(
+                                                websocket=websocket,
+                                                output_model=output_model,
+                                            ),
+                                            'async_streaming_handler': AsyncStreamingWebsocketCallbackHandler(
+                                                websocket=websocket,
+                                                output_model=output_model,
+                                            ),
+                                        }
+                                    )
 
-                                    else:
-                                        # If the function is not a generator, we send the result back to the client.
+                                _returned_data = func(**_input_data_dict)
+                                if inspect.isgenerator(_returned_data):
+                                    # If the function is a generator, we iterate through the generator and send each item back to the client.
+                                    for _stream in _returned_data:
                                         _data = output_model(
-                                            result=_returned_data,
+                                            result=_stream,
                                             error=_ws_serving_error,
                                         )
                                         await websocket.send_text(_data.json())
 
-                                    # Once the generator is exhausted/ function call is completed, send a close message
-                                    self.logger.info(
-                                        f'Closing ws connection `{func.__name__}` for client: {websocket.client}'
-                                    )
-                                    await websocket.close()
-                                    break
-
-                                except WebSocketDisconnect as e:
-                                    self.logger.info(
-                                        f'Client {websocket.client} disconnected from `{func.__name__}` with code {e.code} and reason {e.reason}'
-                                    )
-                                    break
-
-                                except Exception as e:
-                                    self.logger.error(f'Got an exception: {e}')
-                                    _ws_serving_error = str(e)
-                                    # For other errors, we send the error back to the client.
+                                else:
+                                    # If the function is not a generator, we send the result back to the client.
                                     _data = output_model(
-                                        result='',
+                                        result=_returned_data,
                                         error=_ws_serving_error,
                                     )
                                     await websocket.send_text(_data.json())
 
-                                if _ws_serving_error != '':
-                                    print(f'Error: {_ws_serving_error}')
+                                # Once the generator is exhausted/ function call is completed, send a close message
+                                self.logger.info(
+                                    f'Closing ws connection `{func.__name__}` for client: {websocket.client}'
+                                )
+                                await websocket.close()
+                                break
 
-                    except WebSocketDisconnect as e:
-                        self.logger.info(
-                            f'Client {websocket.client} disconnected from `{func.__name__}` with code {e.code} and reason {e.reason}'
-                        )
-                        return
+                            except WebSocketDisconnect as e:
+                                self.logger.info(
+                                    f'Client {websocket.client} disconnected from `{func.__name__}` with code {e.code} and reason {e.reason}'
+                                )
+                                break
+
+                            except Exception as e:
+                                self.logger.error(f'Got an exception: {e}')
+                                _ws_serving_error = str(e)
+                                # For other errors, we send the error back to the client.
+                                _data = output_model(
+                                    result='',
+                                    error=_ws_serving_error,
+                                )
+                                await websocket.send_text(_data.json())
+
+                            if _ws_serving_error != '':
+                                print(f'Error: {_ws_serving_error}')
+
+                except WebSocketDisconnect as e:
+                    self.logger.info(
+                        f'Client {websocket.client} disconnected from `{func.__name__}` with code {e.code} and reason {e.reason}'
+                    )
+                    return
```

### Comparing `langchain-serve-0.0.3.dev19/lcserve/backend/nginx.conf` & `langchain-serve-0.0.3.dev3/lcserve/backend/nginx.conf`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.3.dev19/lcserve/backend/playground/app.py` & `langchain-serve-0.0.3.dev3/lcserve/backend/playground/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+import streamlit as st
 import os
 import sys
 
-import streamlit as st
-
 # get file dir and add it to sys.path
 cwd = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(cwd)
 
 from utils.talk import talk_to_agent  # doesn't work
-from utils.tools import ALL_AGENT_TYPES, ALL_TOOLS
+from utils.tools import ALL_TOOLS, ALL_AGENT_TYPES
 
 st.set_page_config(
     page_title='Langchain on Jina',
     page_icon='⚡',
     layout='wide',
     initial_sidebar_state='auto',
 )
```

### Comparing `langchain-serve-0.0.3.dev19/lcserve/backend/playground/utils/helper.py` & `langchain-serve-0.0.3.dev3/lcserve/backend/playground/utils/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,37 +7,29 @@
 from collections import defaultdict
 from io import StringIO
 from typing import Any, Dict, List, Union
 
 import nest_asyncio
 from pydantic import BaseModel
 
+
 CLS = 'cls'
 RESULT = 'result'
 LLM_TYPE = '_type'
 DEFAULT_FIELD = 'chain'
 DEFAULT_KEY = '__default__'
 AGENT_OUTPUT = '__agent_output__'
 SERVING = 'Serving'
 APPDIR = '/appdir'
 
 LANGCHAIN_API_PORT = os.environ.get('LANGCHAIN_API_PORT', 8080)
 LANGCHAIN_PLAYGROUND_PORT = os.environ.get('LANGCHAIN_PLAYGROUND_PORT', 8501)
 
 
-try:
-    nest_asyncio.apply()
-except RuntimeError:
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-
-    try:
-        nest_asyncio.apply()
-    except RuntimeError:
-        pass
+nest_asyncio.apply()
 
 
 def get_or_create_eventloop():
     try:
         return asyncio.get_event_loop()
     except RuntimeError as ex:
         if "There is no current event loop in thread" in str(ex):
```

### Comparing `langchain-serve-0.0.3.dev19/lcserve/backend/playground/utils/talk.py` & `langchain-serve-0.0.3.dev3/lcserve/backend/playground/utils/talk.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Tuple
-
 import requests
 
+
 LANGCHAIN_API_HOST = 'http://localhost:8080/run'
 
 
 def agent_params_from_input(
     selected_params: Dict[str, Dict[str, str]], agent_type: str
 ) -> Dict:
     tools = {'tool_names': []}
```

### Comparing `langchain-serve-0.0.3.dev19/lcserve/backend/playground/utils/tools.py` & `langchain-serve-0.0.3.dev3/lcserve/backend/playground/utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,13 @@
 
         l_tools.append(LangchainTool(name=name, api=k, args=args))
 
     return l_tools
 
 
 ALL_TOOLS = {t.name: {'api': t.api, 'args': t.args} for t in get_all_langchain_tools()}
-ALL_TOOL_NAMES = [t.name for t in get_all_langchain_tools()]
-
 # https://python.langchain.com/en/latest/modules/agents/agents.html
 ALL_AGENT_TYPES = {
     'MRKL': 'zero-shot-react-description',
     'ReAct': 'react-docstore',
     'Self-Ask-With-Search': 'self-ask-with-search',
 }
```

### Comparing `langchain-serve-0.0.3.dev19/lcserve/customgateway.Dockerfile` & `langchain-serve-0.0.3.dev3/lcserve/customgateway.Dockerfile`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.3.dev19/lcserve/flow.py` & `langchain-serve-0.0.3.dev3/lcserve/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from functools import wraps
 from http import HTTPStatus
 from importlib import import_module
 from shutil import copytree
 from tempfile import mkdtemp
-from typing import Dict, List, Optional, Tuple, Union, Sequence
+from typing import Dict, List, Optional, Tuple, Union
 
 import requests
 import yaml
 from docarray import Document, DocumentArray
 from jina import Flow
 
 APP_NAME = 'langchain'
-BABYAGI_APP_NAME = 'babyagi'
 ServingGatewayConfigFile = 'servinggateway_config.yml'
 JCloudConfigFile = 'jcloud_config.yml'
 
 
 def syncify(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
@@ -152,34 +151,26 @@
     for _, func in inspect.getmembers(app, inspect.isfunction):
         if hasattr(func, '__ws_serving__'):
             return True
 
     return False
 
 
-def _add_to_path():
-    sys.path.append(os.getcwd())
-    # get all directories in the apps folder and add them to the path
-    for app in os.listdir(os.path.join(os.path.dirname(__file__), 'apps')):
-        sys.path.append(os.path.join(os.path.dirname(__file__), 'apps', app))
-
-
 def push_app_to_hubble(
     mod: str,
     tag: str = 'latest',
-    requirements: Tuple[str] = None,
     verbose: Optional[bool] = False,
 ) -> Tuple[str, bool]:
     from hubble.executor.hubio import HubIO
     from hubble.executor.parsers import set_hub_push_parser
 
     from .backend.playground.utils.helper import get_random_name
 
     try:
-        _add_to_path()
+        sys.path.append(os.getcwd())
         app = import_module(mod)
         file = app.__file__
         if file.endswith('.py'):
             appdir = os.path.dirname(file)
         else:
             print(f'Unknown file type for module {mod}')
             sys.exit(1)
@@ -199,25 +190,14 @@
     copytree(appdir, tmpdir, dirs_exist_ok=True)
     # Copy lcserve to tmpdir
     copytree(
         os.path.dirname(__file__), os.path.join(tmpdir, 'lcserve'), dirs_exist_ok=True
     )
 
     name = get_random_name()
-
-    # Create the requirements.txt if requirements are given
-    if requirements is not None and isinstance(requirements, Sequence):
-        # Get existing requirements and add the new ones
-        if os.path.exists(os.path.join(tmpdir, 'requirements.txt')):
-            with open(os.path.join(tmpdir, 'requirements.txt'), 'r') as f:
-                requirements = set(requirements + tuple(f.read().splitlines()))
-
-        with open(os.path.join(tmpdir, 'requirements.txt'), 'w') as f:
-            f.write('\n'.join(requirements))
-
     # Create the Dockerfile
     with open(os.path.join(tmpdir, 'Dockerfile'), 'w') as f:
         dockerfile = [
             'FROM jinawolf/serving-gateway:latest',
             'COPY . /appdir/',
             'RUN if [ -e /appdir/requirements.txt ]; then pip install -r /appdir/requirements.txt; fi',
             'ENTRYPOINT [ "jina", "gateway", "--uses", "config.yml" ]',
```

### Comparing `langchain-serve-0.0.3.dev19/lcserve/flow.yml` & `langchain-serve-0.0.3.dev3/lcserve/flow.yml`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.3.dev19/setup.py` & `langchain-serve-0.0.3.dev3/setup.py`

 * *Files identical despite different names*

