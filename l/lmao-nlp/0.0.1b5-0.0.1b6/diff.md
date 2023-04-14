# Comparing `tmp/lmao-nlp-0.0.1b5.tar.gz` & `tmp/lmao-nlp-0.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmao-nlp-0.0.1b5.tar", last modified: Thu Apr 13 01:57:31 2023, max compression
+gzip compressed data, was "lmao-nlp-0.0.1b6.tar", last modified: Fri Apr 14 14:51:41 2023, max compression
```

## Comparing `lmao-nlp-0.0.1b5.tar` & `lmao-nlp-0.0.1b6.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.182344 lmao-nlp-0.0.1b5/
--rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b5/LICENSE
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-13 01:57:31.182181 lmao-nlp-0.0.1b5/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1853 2023-04-13 01:54:40.000000 lmao-nlp-0.0.1b5/README.md
--rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b5/pyproject.toml
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-13 01:57:31.182384 lmao-nlp-0.0.1b5/setup.cfg
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1437 2023-04-13 01:57:28.000000 lmao-nlp-0.0.1b5/setup.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.177026 lmao-nlp-0.0.1b5/src/
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.178029 lmao-nlp-0.0.1b5/src/lmao/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      232 2023-04-13 01:57:28.000000 lmao-nlp-0.0.1b5/src/lmao/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.178323 lmao-nlp-0.0.1b5/src/lmao/adapters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      151 2023-04-12 16:05:36.000000 lmao-nlp-0.0.1b5/src/lmao/adapters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      722 2023-04-12 16:15:07.000000 lmao-nlp-0.0.1b5/src/lmao/adapters/chatbot.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.178696 lmao-nlp-0.0.1b5/src/lmao/adapters/tasks/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       50 2023-04-12 14:54:23.000000 lmao-nlp-0.0.1b5/src/lmao/adapters/tasks/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      878 2023-04-12 02:01:57.000000 lmao-nlp-0.0.1b5/src/lmao/adapters/tasks/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2119 2023-04-13 01:32:11.000000 lmao-nlp-0.0.1b5/src/lmao/adapters/tasks/classification.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.178981 lmao-nlp-0.0.1b5/src/lmao/lm/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-08 21:16:32.000000 lmao-nlp-0.0.1b5/src/lmao/lm/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.179505 lmao-nlp-0.0.1b5/src/lmao/lm/clients/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       67 2023-04-11 21:11:07.000000 lmao-nlp-0.0.1b5/src/lmao/lm/clients/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2081 2023-04-12 02:42:12.000000 lmao-nlp-0.0.1b5/src/lmao/lm/clients/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     5003 2023-04-13 01:30:54.000000 lmao-nlp-0.0.1b5/src/lmao/lm/clients/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2820 2023-04-13 01:37:43.000000 lmao-nlp-0.0.1b5/src/lmao/lm/clients/openai.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.179921 lmao-nlp-0.0.1b5/src/lmao/lm/prompts/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      105 2023-04-08 18:47:45.000000 lmao-nlp-0.0.1b5/src/lmao/lm/prompts/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1070 2023-04-09 17:21:49.000000 lmao-nlp-0.0.1b5/src/lmao/lm/prompts/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1607 2023-04-09 15:19:32.000000 lmao-nlp-0.0.1b5/src/lmao/lm/prompts/classification.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.180595 lmao-nlp-0.0.1b5/src/lmao/lm/schemas/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-11 21:04:00.000000 lmao-nlp-0.0.1b5/src/lmao/lm/schemas/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1145 2023-04-11 22:13:08.000000 lmao-nlp-0.0.1b5/src/lmao/lm/schemas/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-09 15:35:32.000000 lmao-nlp-0.0.1b5/src/lmao/lm/schemas/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2718 2023-04-11 20:57:46.000000 lmao-nlp-0.0.1b5/src/lmao/lm/schemas/openai.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1976 2023-04-09 03:26:12.000000 lmao-nlp-0.0.1b5/src/lmao/lm/utils.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2858 2023-04-12 16:08:12.000000 lmao-nlp-0.0.1b5/src/lmao/loader.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.181141 lmao-nlp-0.0.1b5/src/lmao/orchestrators/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       93 2023-04-09 15:33:39.000000 lmao-nlp-0.0.1b5/src/lmao/orchestrators/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      177 2023-04-09 15:23:07.000000 lmao-nlp-0.0.1b5/src/lmao/orchestrators/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1175 2023-04-12 02:01:57.000000 lmao-nlp-0.0.1b5/src/lmao/orchestrators/classification.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-13 01:57:31.182006 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-13 01:57:31.000000 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)      925 2023-04-13 01:57:31.000000 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-13 01:57:31.000000 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-13 01:57:31.000000 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/requires.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-13 01:57:31.000000 lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.987842 lmao-nlp-0.0.1b6/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b6/LICENSE
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-14 14:51:41.987695 lmao-nlp-0.0.1b6/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2824 2023-04-14 14:48:14.000000 lmao-nlp-0.0.1b6/README.md
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b6/pyproject.toml
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 14:51:41.987886 lmao-nlp-0.0.1b6/setup.cfg
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1437 2023-04-14 14:51:39.000000 lmao-nlp-0.0.1b6/setup.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.982658 lmao-nlp-0.0.1b6/src/
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.983920 lmao-nlp-0.0.1b6/src/lmao/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      201 2023-04-14 14:51:39.000000 lmao-nlp-0.0.1b6/src/lmao/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.984399 lmao-nlp-0.0.1b6/src/lmao/adapters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       73 2023-04-14 13:50:37.000000 lmao-nlp-0.0.1b6/src/lmao/adapters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1101 2023-04-14 14:25:11.000000 lmao-nlp-0.0.1b6/src/lmao/adapters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1573 2023-04-14 14:29:05.000000 lmao-nlp-0.0.1b6/src/lmao/adapters/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     3950 2023-04-14 14:30:29.000000 lmao-nlp-0.0.1b6/src/lmao/adapters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2445 2023-04-14 14:51:09.000000 lmao-nlp-0.0.1b6/src/lmao/factory.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.984660 lmao-nlp-0.0.1b6/src/lmao/lm/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-13 20:14:27.000000 lmao-nlp-0.0.1b6/src/lmao/lm/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.985180 lmao-nlp-0.0.1b6/src/lmao/lm/clients/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       67 2023-04-11 21:11:07.000000 lmao-nlp-0.0.1b6/src/lmao/lm/clients/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2101 2023-04-13 18:36:40.000000 lmao-nlp-0.0.1b6/src/lmao/lm/clients/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     5157 2023-04-13 18:52:54.000000 lmao-nlp-0.0.1b6/src/lmao/lm/clients/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2626 2023-04-13 20:15:49.000000 lmao-nlp-0.0.1b6/src/lmao/lm/clients/openai.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.985521 lmao-nlp-0.0.1b6/src/lmao/lm/prompts/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      105 2023-04-08 18:47:45.000000 lmao-nlp-0.0.1b6/src/lmao/lm/prompts/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1070 2023-04-09 17:21:49.000000 lmao-nlp-0.0.1b6/src/lmao/lm/prompts/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1607 2023-04-09 15:19:32.000000 lmao-nlp-0.0.1b6/src/lmao/lm/prompts/classification.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.986209 lmao-nlp-0.0.1b6/src/lmao/lm/schemas/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-11 21:04:00.000000 lmao-nlp-0.0.1b6/src/lmao/lm/schemas/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1145 2023-04-11 22:13:08.000000 lmao-nlp-0.0.1b6/src/lmao/lm/schemas/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-09 15:35:32.000000 lmao-nlp-0.0.1b6/src/lmao/lm/schemas/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2718 2023-04-11 20:57:46.000000 lmao-nlp-0.0.1b6/src/lmao/lm/schemas/openai.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b6/src/lmao/lm/utils.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.986453 lmao-nlp-0.0.1b6/src/lmao/orchestrators/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b6/src/lmao/orchestrators/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b6/src/lmao/orchestrators/base.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.986944 lmao-nlp-0.0.1b6/src/lmao/tasks/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       73 2023-04-14 13:51:20.000000 lmao-nlp-0.0.1b6/src/lmao/tasks/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      701 2023-04-14 14:35:35.000000 lmao-nlp-0.0.1b6/src/lmao/tasks/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      786 2023-04-14 14:26:22.000000 lmao-nlp-0.0.1b6/src/lmao/tasks/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1447 2023-04-14 14:36:05.000000 lmao-nlp-0.0.1b6/src/lmao/tasks/classification.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.987526 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-14 14:51:41.000000 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      946 2023-04-14 14:51:41.000000 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-14 14:51:41.000000 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-14 14:51:41.000000 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/requires.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-14 14:51:41.000000 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/top_level.txt
```

### Comparing `lmao-nlp-0.0.1b5/LICENSE` & `lmao-nlp-0.0.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b5/PKG-INFO` & `lmao-nlp-0.0.1b6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b5
+Version: 0.0.1b6
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b5/pyproject.toml` & `lmao-nlp-0.0.1b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b5/setup.py` & `lmao-nlp-0.0.1b6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.0.1-beta.5"
+__version__ = "0.0.1-beta.6"
 
 with open("requirements.txt", "r") as f:
     install_requires = [line.replace("==", ">=") for line in f.read().splitlines() if line != "" if line[0] != "#"]
 
 extras_require = {}
 
 with open("requirements-dev.txt", "r") as f:
```

### Comparing `lmao-nlp-0.0.1b5/src/lmao/adapters/chatbot.py` & `lmao-nlp-0.0.1b6/src/lmao/adapters/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,31 @@
-from lmao.lm.clients import BaseClient, ChatHistory
-from lmao.lm.clients.base import SUCCESS_STATUS_CODE
+from abc import ABC, abstractmethod
 
-__all__ = ["Chatbot"]
+from lmao.lm.clients.base import BaseClient, ChatHistory, ClientResponse
+from lmao.lm.prompts.base import Prompter
 
+__all__ = ["BaseAdapter", "BaseChatbotAdapter", "BaseTaskAdapter"]
 
-class Chatbot:
-    def __init__(self, lm_client: BaseClient, chat_history: ChatHistory, client_method_name: str):
-        self.lm_client = lm_client
-        self.history = chat_history
-        self.client_method_name = client_method_name
-
-    def chat(self, message: str, **kwargs) -> str:
-        self.history.add_human_message(message)
-        response = getattr(self.lm_client, self.client_method_name)(self.history.to_request_format(), **kwargs)
-        if response.status_code == SUCCESS_STATUS_CODE:
-            self.history.add_assistant_message(response.text)
+
+class BaseAdapter(ABC):
+    def __init__(self, client: BaseClient, endpoint_method_name: str):
+        self.client = client
+        self.endpoint_method_name = endpoint_method_name
+
+    def postprocess_response(self, response: ClientResponse) -> ClientResponse:
         return response
+
+    @abstractmethod
+    def to_endpoint_kwargs(self, request) -> dict:
+        pass
+
+
+class BaseChatbotAdapter(BaseAdapter):
+    def __init__(self, client: BaseClient, endpoint_method_name: str, chat_history: ChatHistory):
+        self.chat_history = chat_history
+        super().__init__(client=client, endpoint_method_name=endpoint_method_name)
+
+
+class BaseTaskAdapter(BaseAdapter):
+    def __init__(self, client: BaseClient, endpoint_method_name: str, prompter: Prompter):
+        self.prompter = prompter
+        super().__init__(client=client, endpoint_method_name=endpoint_method_name)
```

### Comparing `lmao-nlp-0.0.1b5/src/lmao/lm/clients/anthropic.py` & `lmao-nlp-0.0.1b6/src/lmao/lm/clients/anthropic.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 class AnthropicClient(BaseClient):
     base_url = "https://api.anthropic.com"
     api_env_name = "ANTHROPIC_API_KEY"
     api_header_format = "x-api-key"
 
     schema = Schema(complete=AnthropicCompleteSchema.schema()["properties"])
 
-    def __init__(self, api_key: Optional[str] = None):
-        super().__init__(api_key)
+    def __init__(self, api_key: Optional[str] = None, **kwargs):
+        super().__init__(api_key, **kwargs)
 
     def complete(self, prompt: str, **kwargs) -> ClientResponse:
         status_code, response = self._post_request(
             "v1/complete",
             AnthropicCompleteSchema(prompt=prompt, **kwargs).to_request_dict(),
         )
         return ClientResponse(
```

### Comparing `lmao-nlp-0.0.1b5/src/lmao/lm/clients/base.py` & `lmao-nlp-0.0.1b6/src/lmao/lm/clients/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 from abc import ABC, abstractmethod, abstractstaticmethod
 from collections import deque
+from dataclasses import dataclass
 from typing import Callable, Deque, List, NamedTuple, Optional, Tuple
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
 __all__ = ["ClientResponse", "BaseClient", "ChatHistory", "SUCCESS_STATUS_CODE"]
@@ -20,21 +21,22 @@
 API_HEADER_FORMAT_DICT = {
     "x-api-key": APIHeader(key="X-API-Key", value=lambda api_key: api_key),
     "basic authentication": APIHeader(key="Authorization", value=lambda api_key: f"Basic {api_key}"),
     "bearer authentication": APIHeader(key="Authorization", value=lambda api_key: f"Bearer {api_key}"),
 }
 
 
-class ClientResponse(NamedTuple):
+@dataclass
+class ClientResponse:
     text: Optional[str]
     raw_response: dict
     status_code: int
 
     def __repr__(self):
-        repr = "\n".join([f"{k}: {v}" for k, v in self._asdict().items()])
+        repr = "\n".join([f"{k}: {v}" for k, v in self.__dict__.items()])
         repr = re.sub(r"^", " " * 4, repr, 0, re.M)
         return f"{self.__class__.__name__}({{\n{repr}\n}})"
 
 
 class ChatHistory(ABC):
     human_role: str = "human"
     assistant_role: str = "assistant"
@@ -90,32 +92,33 @@
 class LM(ABC):
     @abstractmethod
     def complete(self, prompt: str, **kwargs) -> ClientResponse:
         pass
 
 
 class BaseClient(LM, ABC):
-    base_url: str = "none"
-    api_env_name: str = "none"
-    api_header_format: str = "none"
+    base_url: Optional[str] = None
+    api_env_name: Optional[str] = None
+    api_header_format: Optional[str] = None
 
     #  If the backoff_factor is 0.1, then sleep() will sleep for [0.0s, 0.2s, 0.4s, …] between retries.
     RETRY_BACKOFF_FACTOR: float = 0.1
     RETRY_STATUS_CODES: List[int] = [429, 500, 502, 503, 504]
 
-    def __init__(self, api_key: Optional[str] = None, max_retries: int = 5):
+    def __init__(self, api_key: Optional[str] = None, max_retries: int = 5, default_method_name: str = "complete"):
         self.max_retries = max_retries
-        self.__api_key = api_key or os.environ.get(self.api_env_name)
+        self.__api_key = api_key or os.environ.get(self.api_env_name or "")
         if self.__api_key is None:
             raise ValueError("You must provide an API key or set api_env_name to initialize an LM Client.")
-        if self.base_url == "none":
+        if self.base_url is None:
             raise ValueError("Client subclasses must define a base URL attribute.")
         if self.api_header_format not in API_HEADER_FORMAT_DICT:
             raise ValueError(f"Client subclasses must have api_header_format in {list(API_HEADER_FORMAT_DICT.keys())}")
         self._api_header = API_HEADER_FORMAT_DICT[self.api_header_format]
+        self.default_method_name = default_method_name
 
     def _post_request(self, api_path: str, request: dict, extra_headers: Optional[dict] = None) -> Tuple[int, dict]:
         with requests.Session() as session:
             retries = Retry(
                 total=self.max_retries,
                 backoff_factor=self.RETRY_BACKOFF_FACTOR,
                 status_forcelist=self.RETRY_STATUS_CODES,
```

### Comparing `lmao-nlp-0.0.1b5/src/lmao/lm/clients/openai.py` & `lmao-nlp-0.0.1b6/src/lmao/lm/clients/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, NamedTuple, Optional, Union
+from typing import Dict, List, NamedTuple, Optional
 
 from lmao.lm.clients.base import SUCCESS_STATUS_CODE, BaseClient, ChatHistory, ClientResponse
 from lmao.lm.schemas.openai import OpenAIChatSchema, OpenAICompleteSchema
 
 __all__ = ["OpenAIClient", "OpenAIChatHistory"]
 
 
@@ -37,29 +37,26 @@
 class OpenAIClient(BaseClient):
     base_url = "https://api.openai.com/v1"
     api_env_name = "OPENAI_API_KEY"
     api_header_format = "bearer authentication"
 
     schema = Schema(complete=OpenAICompleteSchema.schema()["properties"], chat=OpenAIChatSchema.schema()["properties"])
 
-    def __init__(self, api_key: Optional[str] = None):
-        super().__init__(api_key)
+    def __init__(self, api_key: Optional[str] = None, **kwargs):
+        super().__init__(api_key, **kwargs)
 
     def chat(
         self,
-        messages: Union[str, List[Dict[str, str]]],
+        messages: List[Dict[str, str]],
         system_message: str = DEFAULT_SYSTEM_MESSAGE,
         **kwargs,
     ) -> ClientResponse:
-        if isinstance(messages, str):
-            messages = [{"role": "system", "content": system_message}] + [{"role": "user", "content": messages}]
-        elif len(messages) > 0:
-            messages = [{"role": "system", "content": system_message}] + [
-                OpenAIChatHistory.check_message_format(m) for m in messages
-            ]
+        messages = [{"role": "system", "content": system_message}] + [
+            OpenAIChatHistory.check_message_format(m) for m in messages
+        ]
         status_code, response = self._post_request(
             "chat/completions", OpenAIChatSchema(messages=messages, **kwargs).to_request_dict()
         )
         return ClientResponse(
             text=response["choices"][0]["message"]["content"] if status_code == SUCCESS_STATUS_CODE else None,
             raw_response=response,
             status_code=status_code,
```

### Comparing `lmao-nlp-0.0.1b5/src/lmao/lm/prompts/base.py` & `lmao-nlp-0.0.1b6/src/lmao/lm/prompts/base.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b5/src/lmao/lm/prompts/classification.py` & `lmao-nlp-0.0.1b6/src/lmao/lm/prompts/classification.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b5/src/lmao/lm/schemas/anthropic.py` & `lmao-nlp-0.0.1b6/src/lmao/lm/schemas/anthropic.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b5/src/lmao/lm/schemas/openai.py` & `lmao-nlp-0.0.1b6/src/lmao/lm/schemas/openai.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b5/src/lmao/lm/utils.py` & `lmao-nlp-0.0.1b6/src/lmao/lm/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 num_tokens += len(encoding.encode(value))
                 if key == "name":  # if there's a name, the role is omitted
                     num_tokens += -1  # role is always required and always 1 token
         num_tokens += 2  # every reply is primed with <im_start>assistant
         return num_tokens
     else:
         raise NotImplementedError(
-            f"Not implemented for model {model}. See https://github.com/openai/openai-python/blob/main/chatml.md.,"
+            f"Not implemented for model {model}. See https://github.com/openai/openai-python/blob/main/chatml.md"
         )
 
 
 def chat_estimate_price(messages, model="gpt-3.5-turbo-0301"):
     """Returns the estimated price of a list of messages."""
     model_short = "gpt-3.5-turbo" if model.startswith("gpt-3.5-turbo") else model
     return chat_count_tokens(messages, model) * price_per_token[model_short]
```

### Comparing `lmao-nlp-0.0.1b5/src/lmao/loader.py` & `lmao-nlp-0.0.1b6/src/lmao/factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,63 @@
-import inspect
-from typing import Tuple, Union
+from typing import NamedTuple, Tuple, Union
 
 import lmao.adapters as adapters
-import lmao.orchestrators as orcs
-from lmao.lm.clients import (
-    AnthropicChatHistory,
-    AnthropicClient,
-    BaseClient,
-    ChatHistory,
-    OpenAIChatHistory,
-    OpenAIClient,
-)
+import lmao.lm.clients as clients
+import lmao.tasks as tasks
 
-__all__ = ["load_chatbot", "load_lm_client", "load_orchestrator", "load_task_adapter"]
+__all__ = ["create_chatbot", "create_client", "create_task"]
 
 
-default_chat_method = {"openai": "chat", "anthropic": "complete"}
+class ObjectMapping(NamedTuple):
+    name_to_client: dict = {"anthropic": clients.AnthropicClient, "openai": clients.OpenAIClient}
+    name_to_history: dict = {"anthropic": clients.AnthropicChatHistory, "openai": clients.OpenAIChatHistory}
+    name_to_task: dict = {
+        "sentiment_analysis": tasks.TextClassification,
+        "text_classification": tasks.TextClassification,
+        "chatbot": tasks.Chatbot,
+    }
+    task_to_adapter: dict = {
+        "chatbot": {
+            "anthropic": adapters.AnthropicChatbotAdapter,
+            "openai": adapters.OpenAIChatbotAdapter,
+        },
+        "sentiment_analysis": {
+            "anthropic": adapters.AnthropicSentimentAnalysisAdapter,
+            "openai": adapters.OpenAISentimentAnalysisAdapter,
+        },
+        "text_classification": {
+            "anthropic": adapters.AnthropicTextClassificationAdapter,
+            "openai": adapters.OpenAITextClassificationAdapter,
+        },
+    }
 
-name_to_client = {"anthropic": (AnthropicClient, AnthropicChatHistory), "openai": (OpenAIClient, OpenAIChatHistory)}
 
-task_to_adapter = {
-    "sentiment_analysis": adapters.SentimentAnalysisAdapter,
-}
+_m = ObjectMapping()
 
-task_to_orchestrator = {
-    "sentiment_analysis": orcs.SentimentAnalysisOrchestrator,
-}
 
-
-def _get_lm_kwargs(name: str, **kwargs):
-    return {k: kwargs.pop(k) for k in inspect.signature(name_to_client[name][0]).parameters.keys() if k in kwargs}
-
-
-def _validate_input(lm_client_name: str, task: str):
-    lm_client_name = lm_client_name.lower()
+def _validate_task_input(task: str, client_name: str):
+    client_name = client_name.lower()
     task = task.lower().replace(" ", "_")
-    if lm_client_name not in default_chat_method or lm_client_name not in name_to_client:
-        raise ValueError(f"LM provider {lm_client_name} not supported")
-    if task not in task_to_orchestrator:
+    if client_name not in _m.name_to_client:
+        raise ValueError(f"LM client {client_name} not supported")
+    if task not in _m.name_to_task:
         raise ValueError(f"Task {task} not supported")
-    return lm_client_name, task
+    return task, client_name
 
 
-def load_chatbot(lm_client_name: str, **kwargs) -> adapters.Chatbot:
-    max_length = kwargs.pop("max_length", 5)
-    Client, History = name_to_client[lm_client_name]
-    return adapters.Chatbot(
-        lm_client=Client(**kwargs),
-        chat_history=History(max_length=max_length),
-        client_method_name=kwargs.pop("client_method_name", default_chat_method[lm_client_name]),
-    )
+def create_chatbot(client_name: str, **kwargs) -> tasks.Chatbot:
+    return tasks.Chatbot(_m.task_to_adapter["chatbot"][client_name](**kwargs))
 
 
-def load_lm_client(
-    lm_client_name: str, chat_history: bool = False, **kwargs
-) -> Union[BaseClient, Tuple[BaseClient, ChatHistory]]:
+def create_client(
+    client_name: str, chat_history: bool = False, **kwargs
+) -> Union[clients.BaseClient, Tuple[clients.BaseClient, clients.ChatHistory]]:
     max_length = kwargs.pop("max_length", 5)
-    Client, History = name_to_client[lm_client_name]
+    Client, History = _m.name_to_client[client_name], _m.name_to_history[client_name]
     return (Client(**kwargs), History(max_length=max_length)) if chat_history else Client(**kwargs)
 
 
-def load_orchestrator(lm_client_name: str, task: str, **kwargs) -> orcs.BaseOrchestrator:
-    lm_client_name, task = _validate_input(lm_client_name, task)
-    return task_to_orchestrator[task](
-        lm_client=name_to_client[lm_client_name][0](**_get_lm_kwargs(lm_client_name, **kwargs)),
-        client_method_name=kwargs.pop("client_method_name", default_chat_method[lm_client_name]),
-        **kwargs,
-    )
-
-
-def load_task_adapter(lm_client_name: str, task: str, **kwargs) -> adapters.TaskAdapter:
-    lm_client_name, task = _validate_input(lm_client_name, task)
-    return task_to_adapter[task](
-        lm_client=name_to_client[lm_client_name][0](**_get_lm_kwargs(lm_client_name, **kwargs)),
-        client_method_name=kwargs.pop("client_method_name", default_chat_method[lm_client_name]),
-        **kwargs,
-    )
+def create_task(task: str, client_name: str, **kwargs) -> Union[tasks.BaseTask, tasks.Chatbot]:
+    task, client_name = _validate_task_input(task, client_name)
+    Task = _m.name_to_task[task]
+    client_adapter = _m.task_to_adapter[task][client_name](**kwargs)
+    return Task(client_adapter) if task != "chatbot" else create_chatbot(client_name, **kwargs)
```

### Comparing `lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/PKG-INFO` & `lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b5
+Version: 0.0.1b6
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b5/src/lmao_nlp.egg-info/SOURCES.txt` & `lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/lmao/__init__.py
-src/lmao/loader.py
+src/lmao/factory.py
 src/lmao/adapters/__init__.py
+src/lmao/adapters/base.py
 src/lmao/adapters/chatbot.py
-src/lmao/adapters/tasks/__init__.py
-src/lmao/adapters/tasks/base.py
-src/lmao/adapters/tasks/classification.py
+src/lmao/adapters/classification.py
 src/lmao/lm/__init__.py
 src/lmao/lm/utils.py
 src/lmao/lm/clients/__init__.py
 src/lmao/lm/clients/anthropic.py
 src/lmao/lm/clients/base.py
 src/lmao/lm/clients/openai.py
 src/lmao/lm/prompts/__init__.py
@@ -20,13 +19,16 @@
 src/lmao/lm/prompts/classification.py
 src/lmao/lm/schemas/__init__.py
 src/lmao/lm/schemas/anthropic.py
 src/lmao/lm/schemas/base.py
 src/lmao/lm/schemas/openai.py
 src/lmao/orchestrators/__init__.py
 src/lmao/orchestrators/base.py
-src/lmao/orchestrators/classification.py
+src/lmao/tasks/__init__.py
+src/lmao/tasks/base.py
+src/lmao/tasks/chatbot.py
+src/lmao/tasks/classification.py
 src/lmao_nlp.egg-info/PKG-INFO
 src/lmao_nlp.egg-info/SOURCES.txt
 src/lmao_nlp.egg-info/dependency_links.txt
 src/lmao_nlp.egg-info/requires.txt
 src/lmao_nlp.egg-info/top_level.txt
```

