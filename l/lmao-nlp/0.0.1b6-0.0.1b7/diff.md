# Comparing `tmp/lmao-nlp-0.0.1b6.tar.gz` & `tmp/lmao-nlp-0.0.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmao-nlp-0.0.1b6.tar", last modified: Fri Apr 14 14:51:41 2023, max compression
+gzip compressed data, was "lmao-nlp-0.0.1b7.tar", last modified: Fri Apr 14 20:03:00 2023, max compression
```

## Comparing `lmao-nlp-0.0.1b6.tar` & `lmao-nlp-0.0.1b7.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.987842 lmao-nlp-0.0.1b6/
--rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b6/LICENSE
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-14 14:51:41.987695 lmao-nlp-0.0.1b6/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2824 2023-04-14 14:48:14.000000 lmao-nlp-0.0.1b6/README.md
--rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b6/pyproject.toml
--rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 14:51:41.987886 lmao-nlp-0.0.1b6/setup.cfg
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1437 2023-04-14 14:51:39.000000 lmao-nlp-0.0.1b6/setup.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.982658 lmao-nlp-0.0.1b6/src/
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.983920 lmao-nlp-0.0.1b6/src/lmao/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      201 2023-04-14 14:51:39.000000 lmao-nlp-0.0.1b6/src/lmao/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.984399 lmao-nlp-0.0.1b6/src/lmao/adapters/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       73 2023-04-14 13:50:37.000000 lmao-nlp-0.0.1b6/src/lmao/adapters/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1101 2023-04-14 14:25:11.000000 lmao-nlp-0.0.1b6/src/lmao/adapters/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1573 2023-04-14 14:29:05.000000 lmao-nlp-0.0.1b6/src/lmao/adapters/chatbot.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     3950 2023-04-14 14:30:29.000000 lmao-nlp-0.0.1b6/src/lmao/adapters/classification.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2445 2023-04-14 14:51:09.000000 lmao-nlp-0.0.1b6/src/lmao/factory.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.984660 lmao-nlp-0.0.1b6/src/lmao/lm/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-13 20:14:27.000000 lmao-nlp-0.0.1b6/src/lmao/lm/__init__.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.985180 lmao-nlp-0.0.1b6/src/lmao/lm/clients/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       67 2023-04-11 21:11:07.000000 lmao-nlp-0.0.1b6/src/lmao/lm/clients/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2101 2023-04-13 18:36:40.000000 lmao-nlp-0.0.1b6/src/lmao/lm/clients/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     5157 2023-04-13 18:52:54.000000 lmao-nlp-0.0.1b6/src/lmao/lm/clients/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2626 2023-04-13 20:15:49.000000 lmao-nlp-0.0.1b6/src/lmao/lm/clients/openai.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.985521 lmao-nlp-0.0.1b6/src/lmao/lm/prompts/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      105 2023-04-08 18:47:45.000000 lmao-nlp-0.0.1b6/src/lmao/lm/prompts/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1070 2023-04-09 17:21:49.000000 lmao-nlp-0.0.1b6/src/lmao/lm/prompts/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1607 2023-04-09 15:19:32.000000 lmao-nlp-0.0.1b6/src/lmao/lm/prompts/classification.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.986209 lmao-nlp-0.0.1b6/src/lmao/lm/schemas/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-11 21:04:00.000000 lmao-nlp-0.0.1b6/src/lmao/lm/schemas/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1145 2023-04-11 22:13:08.000000 lmao-nlp-0.0.1b6/src/lmao/lm/schemas/anthropic.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-09 15:35:32.000000 lmao-nlp-0.0.1b6/src/lmao/lm/schemas/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     2718 2023-04-11 20:57:46.000000 lmao-nlp-0.0.1b6/src/lmao/lm/schemas/openai.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b6/src/lmao/lm/utils.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.986453 lmao-nlp-0.0.1b6/src/lmao/orchestrators/
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b6/src/lmao/orchestrators/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b6/src/lmao/orchestrators/base.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.986944 lmao-nlp-0.0.1b6/src/lmao/tasks/
--rw-r--r--   0 johnnygreco   (501) staff       (20)       73 2023-04-14 13:51:20.000000 lmao-nlp-0.0.1b6/src/lmao/tasks/__init__.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      701 2023-04-14 14:35:35.000000 lmao-nlp-0.0.1b6/src/lmao/tasks/base.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)      786 2023-04-14 14:26:22.000000 lmao-nlp-0.0.1b6/src/lmao/tasks/chatbot.py
--rw-r--r--   0 johnnygreco   (501) staff       (20)     1447 2023-04-14 14:36:05.000000 lmao-nlp-0.0.1b6/src/lmao/tasks/classification.py
-drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:51:41.987526 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/
--rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-14 14:51:41.000000 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/PKG-INFO
--rw-r--r--   0 johnnygreco   (501) staff       (20)      946 2023-04-14 14:51:41.000000 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-14 14:51:41.000000 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-14 14:51:41.000000 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/requires.txt
--rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-14 14:51:41.000000 lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.531409 lmao-nlp-0.0.1b7/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)    11357 2023-04-02 19:11:18.000000 lmao-nlp-0.0.1b7/LICENSE
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-14 20:03:00.531253 lmao-nlp-0.0.1b7/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     4116 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/README.md
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      764 2023-04-02 17:52:45.000000 lmao-nlp-0.0.1b7/pyproject.toml
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 20:03:00.531461 lmao-nlp-0.0.1b7/setup.cfg
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1275 2023-04-14 20:02:57.000000 lmao-nlp-0.0.1b7/setup.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.526239 lmao-nlp-0.0.1b7/src/
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.527133 lmao-nlp-0.0.1b7/src/lmao/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      203 2023-04-14 20:02:57.000000 lmao-nlp-0.0.1b7/src/lmao/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.527754 lmao-nlp-0.0.1b7/src/lmao/adapters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/adapters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1100 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/adapters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1573 2023-04-14 14:29:05.000000 lmao-nlp-0.0.1b7/src/lmao/adapters/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     3939 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/adapters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1533 2023-04-14 19:44:53.000000 lmao-nlp-0.0.1b7/src/lmao/adapters/fermi.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2673 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/factory.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.527975 lmao-nlp-0.0.1b7/src/lmao/lm/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       38 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/lm/__init__.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.528494 lmao-nlp-0.0.1b7/src/lmao/lm/clients/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       67 2023-04-11 21:11:07.000000 lmao-nlp-0.0.1b7/src/lmao/lm/clients/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2101 2023-04-13 18:36:40.000000 lmao-nlp-0.0.1b7/src/lmao/lm/clients/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     5157 2023-04-13 18:52:54.000000 lmao-nlp-0.0.1b7/src/lmao/lm/clients/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2626 2023-04-13 20:15:49.000000 lmao-nlp-0.0.1b7/src/lmao/lm/clients/openai.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.528959 lmao-nlp-0.0.1b7/src/lmao/lm/schemas/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       47 2023-04-11 21:04:00.000000 lmao-nlp-0.0.1b7/src/lmao/lm/schemas/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1145 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/lm/schemas/anthropic.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      420 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/lm/schemas/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     2718 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/lm/schemas/openai.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1974 2023-04-13 20:12:50.000000 lmao-nlp-0.0.1b7/src/lmao/lm/utils.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.529188 lmao-nlp-0.0.1b7/src/lmao/orchestrators/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:08.000000 lmao-nlp-0.0.1b7/src/lmao/orchestrators/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        0 2023-04-14 14:32:03.000000 lmao-nlp-0.0.1b7/src/lmao/orchestrators/base.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.529660 lmao-nlp-0.0.1b7/src/lmao/prompters/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       71 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b7/src/lmao/prompters/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      496 2023-04-14 19:07:04.000000 lmao-nlp-0.0.1b7/src/lmao/prompters/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1852 2023-04-14 19:31:31.000000 lmao-nlp-0.0.1b7/src/lmao/prompters/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      756 2023-04-14 19:45:56.000000 lmao-nlp-0.0.1b7/src/lmao/prompters/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.530480 lmao-nlp-0.0.1b7/src/lmao/tasks/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)       94 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/tasks/__init__.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      836 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/tasks/base.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      786 2023-04-14 19:04:53.000000 lmao-nlp-0.0.1b7/src/lmao/tasks/chatbot.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1234 2023-04-14 20:02:16.000000 lmao-nlp-0.0.1b7/src/lmao/tasks/classification.py
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      601 2023-04-14 19:41:35.000000 lmao-nlp-0.0.1b7/src/lmao/tasks/fermi.py
+drwxr-xr-x   0 johnnygreco   (501) staff       (20)        0 2023-04-14 20:03:00.531089 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      700 2023-04-14 20:03:00.000000 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 johnnygreco   (501) staff       (20)     1022 2023-04-14 20:03:00.000000 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        1 2023-04-14 20:03:00.000000 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)      288 2023-04-14 20:03:00.000000 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/requires.txt
+-rw-r--r--   0 johnnygreco   (501) staff       (20)        5 2023-04-14 20:03:00.000000 lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/top_level.txt
```

### Comparing `lmao-nlp-0.0.1b6/LICENSE` & `lmao-nlp-0.0.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b6/PKG-INFO` & `lmao-nlp-0.0.1b7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b6
+Version: 0.0.1b7
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b6/pyproject.toml` & `lmao-nlp-0.0.1b7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b6/src/lmao/adapters/base.py` & `lmao-nlp-0.0.1b7/src/lmao/adapters/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 
 from lmao.lm.clients.base import BaseClient, ChatHistory, ClientResponse
-from lmao.lm.prompts.base import Prompter
+from lmao.prompters.base import Prompter
 
 __all__ = ["BaseAdapter", "BaseChatbotAdapter", "BaseTaskAdapter"]
 
 
 class BaseAdapter(ABC):
     def __init__(self, client: BaseClient, endpoint_method_name: str):
         self.client = client
```

### Comparing `lmao-nlp-0.0.1b6/src/lmao/adapters/chatbot.py` & `lmao-nlp-0.0.1b7/src/lmao/adapters/chatbot.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b6/src/lmao/adapters/classification.py` & `lmao-nlp-0.0.1b7/src/lmao/adapters/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional
 
 from lmao.adapters.base import BaseTaskAdapter
 from lmao.lm.clients.anthropic import AnthropicClient
 from lmao.lm.clients.base import BaseClient, ClientResponse
 from lmao.lm.clients.openai import OpenAIClient
-from lmao.lm.prompts.classification import ClassificationPrompter, SentimentAnalysisPrompter
+from lmao.prompters.classification import ClassificationPrompter, SentimentAnalysisPrompter
 
 __all__ = [
     "AnthropicSentimentAnalysisAdapter",
     "AnthropicTextClassificationAdapter",
     "OpenAISentimentAnalysisAdapter",
     "OpenAITextClassificationAdapter",
     "SentimentAnalysisAdapter",
@@ -18,15 +18,15 @@
 
 class TextClassificationAdapter(BaseTaskAdapter):
     def __init__(
         self, client: BaseClient, endpoint_method_name: str, categories: List[str], lowercase: bool = True, **kwargs
     ):
         self.lowercase = lowercase
         self.categories = [c.lower() for c in categories] if lowercase else categories
-        prompter = kwargs.pop("prompter", None) or ClassificationPrompter(categories=self.categories, **kwargs)
+        prompter = kwargs.pop("prompter", None) or ClassificationPrompter(categories=self.categories)
         super().__init__(client=client, endpoint_method_name=endpoint_method_name, prompter=prompter)
 
 
 class SentimentAnalysisAdapter(TextClassificationAdapter):
     def __init__(self, client: BaseClient, endpoint_method_name: str, include_neutral: bool = True, **kwargs):
         super().__init__(
             client=client,
```

### Comparing `lmao-nlp-0.0.1b6/src/lmao/factory.py` & `lmao-nlp-0.0.1b7/src/lmao/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 class ObjectMapping(NamedTuple):
     name_to_client: dict = {"anthropic": clients.AnthropicClient, "openai": clients.OpenAIClient}
     name_to_history: dict = {"anthropic": clients.AnthropicChatHistory, "openai": clients.OpenAIChatHistory}
     name_to_task: dict = {
         "sentiment_analysis": tasks.TextClassification,
         "text_classification": tasks.TextClassification,
+        "fermi_problem": tasks.FermiProblem,
         "chatbot": tasks.Chatbot,
     }
     task_to_adapter: dict = {
         "chatbot": {
             "anthropic": adapters.AnthropicChatbotAdapter,
             "openai": adapters.OpenAIChatbotAdapter,
         },
@@ -24,14 +25,18 @@
             "anthropic": adapters.AnthropicSentimentAnalysisAdapter,
             "openai": adapters.OpenAISentimentAnalysisAdapter,
         },
         "text_classification": {
             "anthropic": adapters.AnthropicTextClassificationAdapter,
             "openai": adapters.OpenAITextClassificationAdapter,
         },
+        "fermi_problem": {
+            "anthropic": adapters.AnthropicFermiProblemAdapter,
+            "openai": adapters.OpenAIFermiProblemAdapter,
+        },
     }
 
 
 _m = ObjectMapping()
 
 
 def _validate_task_input(task: str, client_name: str):
@@ -52,12 +57,12 @@
     client_name: str, chat_history: bool = False, **kwargs
 ) -> Union[clients.BaseClient, Tuple[clients.BaseClient, clients.ChatHistory]]:
     max_length = kwargs.pop("max_length", 5)
     Client, History = _m.name_to_client[client_name], _m.name_to_history[client_name]
     return (Client(**kwargs), History(max_length=max_length)) if chat_history else Client(**kwargs)
 
 
-def create_task(task: str, client_name: str, **kwargs) -> Union[tasks.BaseTask, tasks.Chatbot]:
+def create_task(task: str, client_name: str, **kwargs) -> Union[tasks.ModelProtocol, tasks.QAProtocol, tasks.Chatbot]:
     task, client_name = _validate_task_input(task, client_name)
     Task = _m.name_to_task[task]
     client_adapter = _m.task_to_adapter[task][client_name](**kwargs)
     return Task(client_adapter) if task != "chatbot" else create_chatbot(client_name, **kwargs)
```

### Comparing `lmao-nlp-0.0.1b6/src/lmao/lm/clients/anthropic.py` & `lmao-nlp-0.0.1b7/src/lmao/lm/clients/anthropic.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b6/src/lmao/lm/clients/base.py` & `lmao-nlp-0.0.1b7/src/lmao/lm/clients/base.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b6/src/lmao/lm/clients/openai.py` & `lmao-nlp-0.0.1b7/src/lmao/lm/clients/openai.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b6/src/lmao/lm/prompts/classification.py` & `lmao-nlp-0.0.1b7/src/lmao/prompters/classification.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-from typing import List, Optional
+from typing import List
 
-from .base import Prompter
+from lmao.prompters.base import Prompter, build_prompt_template
 
 __all__ = ["ClassificationPrompter"]
 
 
 class ClassificationPrompter(Prompter):
     task = "classification"
 
+    template = build_prompt_template(
+        intro=(
+            "Classify the input text into one of the following {num_categories} categories: [{categories}]. "
+            "Respond with the answer only, without punctuation."
+        ),
+        close="Input: {input_text}\nCategory:",
+    )
+
     def __init__(
         self,
         categories: List[str],
-        examples: Optional[List[str]] = None,
-        template: Optional[str] = None,
     ):
         self.categories = categories
-        self.examples = examples or []
-        super().__init__(template=template)
-
-    @staticmethod
-    def create_example(input_text: str, category: str) -> str:
-        return f"Input: {input_text}\nCategory: {category}\n\n"
+        self._examples: List[str] = []
 
     def add_example(self, input_text: str, category: str):
         if category not in self.categories:
             raise ValueError(f"Category {category} is not in the list of categories.")
-        self.examples.append(self.create_example(input_text, category))
+        self._examples.append(f"Input: {input_text}\nCategory: {category}\n\n")
 
     def create_prompt(self, input_text: str) -> str:
         return self.template.format(
             num_categories=len(self.categories),
             categories=", ".join(self.categories),
             input_text=input_text,
-            examples="".join(self.examples) if self.examples else "",
+            examples="".join(self._examples) if self._examples else "",
         )
 
 
 class SentimentAnalysisPrompter(ClassificationPrompter):
     task = "sentiment_analysis"
 
+    template = build_prompt_template(
+        intro=(
+            "Classify the sentiment of the input text into one of the following "
+            "{num_categories} categories: [{categories}]. Respond with the answer only, without punctuation."
+        ),
+        close="Input: {input_text}\nSentiment:",
+    )
+
     def __init__(
         self,
-        examples: Optional[List[str]] = None,
-        template: Optional[str] = None,
         include_neutral: bool = True,
     ):
-        super().__init__(
-            categories=["positive", "negative"] + (["neutral"] if include_neutral else []),
-            examples=examples,
-            template=template,
-        )
+        super().__init__(categories=["positive", "negative"] + (["neutral"] if include_neutral else []))
+        self.include_neutral = include_neutral
```

### Comparing `lmao-nlp-0.0.1b6/src/lmao/lm/schemas/anthropic.py` & `lmao-nlp-0.0.1b7/src/lmao/lm/schemas/anthropic.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """API Reference: https://console.anthropic.com/docs/api/reference"""
 
     class Config:
         extra = Extra.forbid
 
     prompt: str = Field(default="Human: Hello, Friend\n\nAssistant:", description="The prompt to complete.")
     model: str = Field(default="claude-v1.3", description="Must be of the form `claude-[model_version]`.")
-    max_tokens_to_sample: int = API_DEFAULTS.generate_max_tokens
+    max_tokens_to_sample: int = API_DEFAULTS.complete_max_tokens
     stop_sequences: Optional[List[str]] = None
     stream: bool = False
     temperature: float = Field(default=1, ge=0.0, le=1.0)
     top_k: int = -1
     top_p: float = -1
 
     @validator("model", pre=True, always=True)
```

### Comparing `lmao-nlp-0.0.1b6/src/lmao/lm/schemas/openai.py` & `lmao-nlp-0.0.1b7/src/lmao/lm/schemas/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     class Config:
         extra = Extra.forbid
 
     model: str = Field(default="text-davinci-003", description="Must be of the form `text-davinci-[model_version]`.")
     prompt: Optional[str] = Field(default=None)
     suffix: Optional[str] = Field(default=None)
-    max_tokens: int = Field(default=API_DEFAULTS.generate_max_tokens, le=4096)
+    max_tokens: int = Field(default=API_DEFAULTS.complete_max_tokens, le=4096)
     temperature: float = Field(default=0.7, ge=0.0, le=2.0)
     top_p: float = Field(default=1.0, ge=0.0, le=1.0)
     n: int = Field(default=1)
     stream: bool = Field(default=False)
     logprobs: Optional[int] = Field(default=None)
     echo: bool = Field(default=False)
     stop: Optional[Union[str, List[str]]] = Field(default=None)
```

### Comparing `lmao-nlp-0.0.1b6/src/lmao/lm/utils.py` & `lmao-nlp-0.0.1b7/src/lmao/lm/utils.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b6/src/lmao/tasks/base.py` & `lmao-nlp-0.0.1b7/src/lmao/tasks/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import NamedTuple
+from typing import NamedTuple, Protocol, runtime_checkable
 
 from lmao.adapters.base import BaseAdapter
 from lmao.lm.clients.base import ClientResponse
 
-__all__ = ["adapter_errors", "BaseTask"]
+__all__ = ["task_errors", "ModelProtocol", "QAProtocol", "TaskResponse"]
 
 
 class TaskErrors(NamedTuple):
     CLIENT_ERROR: str
     PREDICTION_ERROR: str
 
 
+task_errors = TaskErrors(CLIENT_ERROR="CLIENT ERROR", PREDICTION_ERROR="PREDICTION ERROR")
+
+
 @dataclass
 class TaskResponse:
     prediction: str
     client_response: ClientResponse
     success: bool
 
 
-class BaseTask(ABC):
-    def __init__(self, adapter: BaseAdapter):
-        self.adapter = adapter
+@runtime_checkable
+class ModelProtocol(Protocol):
+    adapter: BaseAdapter
+
+    def predict(self, text: str, **kwargs) -> TaskResponse:
+        ...
 
-    @abstractmethod
-    def predict(self, text: str) -> TaskResponse:
-        pass
 
+@runtime_checkable
+class QAProtocol(Protocol):
+    adapter: BaseAdapter
 
-adapter_errors = TaskErrors(CLIENT_ERROR="CLIENT ERROR", PREDICTION_ERROR="PREDICTION ERROR")
+    def ask(self, question: str, **kwargs) -> TaskResponse:
+        ...
```

### Comparing `lmao-nlp-0.0.1b6/src/lmao/tasks/chatbot.py` & `lmao-nlp-0.0.1b7/src/lmao/tasks/chatbot.py`

 * *Files identical despite different names*

### Comparing `lmao-nlp-0.0.1b6/src/lmao/tasks/classification.py` & `lmao-nlp-0.0.1b7/src/lmao/tasks/classification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from lmao.adapters import TextClassificationAdapter
 from lmao.lm.clients.base import SUCCESS_STATUS_CODE
-from lmao.tasks.base import BaseTask, TaskResponse, adapter_errors
+from lmao.tasks.base import TaskResponse, task_errors
 
 __all__ = ["TextClassification"]
 
 
-class TextClassification(BaseTask):
+class TextClassification:
     def __init__(self, adapter: TextClassificationAdapter):
-        if not hasattr(adapter, "categories"):
-            raise AttributeError("TextClassificationAdapter must have a categories attribute")
-        super().__init__(adapter=adapter)
         self.categories = adapter.categories
         self.adapter: TextClassificationAdapter = adapter
 
     def predict(self, text: str, **kwargs) -> TaskResponse:
         success = True
         input_text = self.adapter.prompter.create_prompt(text)
         kwargs.update(self.adapter.to_endpoint_kwargs(input_text))
         response = getattr(self.adapter.client, self.adapter.endpoint_method_name)(**kwargs)
         if response.status_code == SUCCESS_STATUS_CODE:
             prediction = response.text.strip().lower() if self.adapter.lowercase else response.text.strip()
             prediction = prediction.replace(".", "")
             if prediction not in self.categories:
-                prediction = adapter_errors.PREDICTION_ERROR
+                prediction = task_errors.PREDICTION_ERROR
                 success = False
         else:
-            prediction = adapter_errors.CLIENT_ERROR
+            prediction = task_errors.CLIENT_ERROR
             success = False
         return TaskResponse(prediction=prediction, client_response=response, success=success)
```

### Comparing `lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/PKG-INFO` & `lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmao-nlp
-Version: 0.0.1b6
+Version: 0.0.1b7
 Summary: LMAO: Language Model Adapters and Orchestrators
 Home-page: https://github.com/johnnygreco/lmao
 Author: Johnny Greco
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `lmao-nlp-0.0.1b6/src/lmao_nlp.egg-info/SOURCES.txt` & `lmao-nlp-0.0.1b7/src/lmao_nlp.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 setup.py
 src/lmao/__init__.py
 src/lmao/factory.py
 src/lmao/adapters/__init__.py
 src/lmao/adapters/base.py
 src/lmao/adapters/chatbot.py
 src/lmao/adapters/classification.py
+src/lmao/adapters/fermi.py
 src/lmao/lm/__init__.py
 src/lmao/lm/utils.py
 src/lmao/lm/clients/__init__.py
 src/lmao/lm/clients/anthropic.py
 src/lmao/lm/clients/base.py
 src/lmao/lm/clients/openai.py
-src/lmao/lm/prompts/__init__.py
-src/lmao/lm/prompts/base.py
-src/lmao/lm/prompts/classification.py
 src/lmao/lm/schemas/__init__.py
 src/lmao/lm/schemas/anthropic.py
 src/lmao/lm/schemas/base.py
 src/lmao/lm/schemas/openai.py
 src/lmao/orchestrators/__init__.py
 src/lmao/orchestrators/base.py
+src/lmao/prompters/__init__.py
+src/lmao/prompters/base.py
+src/lmao/prompters/classification.py
+src/lmao/prompters/fermi.py
 src/lmao/tasks/__init__.py
 src/lmao/tasks/base.py
 src/lmao/tasks/chatbot.py
 src/lmao/tasks/classification.py
+src/lmao/tasks/fermi.py
 src/lmao_nlp.egg-info/PKG-INFO
 src/lmao_nlp.egg-info/SOURCES.txt
 src/lmao_nlp.egg-info/dependency_links.txt
 src/lmao_nlp.egg-info/requires.txt
 src/lmao_nlp.egg-info/top_level.txt
```

