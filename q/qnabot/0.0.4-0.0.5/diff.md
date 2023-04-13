# Comparing `tmp/qnabot-0.0.4.tar.gz` & `tmp/qnabot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnabot-0.0.4.tar", last modified: Thu Apr 13 23:26:54 2023, max compression
+gzip compressed data, was "qnabot-0.0.5.tar", last modified: Thu Apr 13 23:57:45 2023, max compression
```

## Comparing `qnabot-0.0.4.tar` & `qnabot-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:26:54.496979 qnabot-0.0.4/
--rw-r--r--   0 momegas    (501) staff       (20)     3236 2023-04-13 23:26:54.496856 qnabot-0.0.4/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)     2876 2023-04-13 23:16:27.000000 qnabot-0.0.4/README.md
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:26:54.495770 qnabot-0.0.4/qnabot/
--rw-r--r--   0 momegas    (501) staff       (20)     3070 2023-04-13 23:17:12.000000 qnabot-0.0.4/qnabot/QnABot.py
--rw-r--r--   0 momegas    (501) staff       (20)       27 2023-04-11 20:11:06.000000 qnabot-0.0.4/qnabot/__init__.py
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:26:54.496665 qnabot-0.0.4/qnabot/tests/
--rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-12 18:37:58.000000 qnabot-0.0.4/qnabot/tests/__init__.py
--rw-r--r--   0 momegas    (501) staff       (20)     1484 2023-04-13 23:17:41.000000 qnabot-0.0.4/qnabot/tests/test_QnABot.py
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:26:54.496455 qnabot-0.0.4/qnabot.egg-info/
--rw-r--r--   0 momegas    (501) staff       (20)     3236 2023-04-13 23:26:54.000000 qnabot-0.0.4/qnabot.egg-info/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)      256 2023-04-13 23:26:54.000000 qnabot-0.0.4/qnabot.egg-info/SOURCES.txt
--rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-13 23:26:54.000000 qnabot-0.0.4/qnabot.egg-info/dependency_links.txt
--rw-r--r--   0 momegas    (501) staff       (20)       50 2023-04-13 23:26:54.000000 qnabot-0.0.4/qnabot.egg-info/requires.txt
--rw-r--r--   0 momegas    (501) staff       (20)        7 2023-04-13 23:26:54.000000 qnabot-0.0.4/qnabot.egg-info/top_level.txt
--rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-13 23:26:54.497027 qnabot-0.0.4/setup.cfg
--rw-r--r--   0 momegas    (501) staff       (20)      739 2023-04-13 23:26:49.000000 qnabot-0.0.4/setup.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:57:45.015192 qnabot-0.0.5/
+-rw-r--r--   0 momegas    (501) staff       (20)     3521 2023-04-13 23:57:45.015065 qnabot-0.0.5/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)     3161 2023-04-13 23:55:55.000000 qnabot-0.0.5/README.md
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:57:45.013900 qnabot-0.0.5/qnabot/
+-rw-r--r--   0 momegas    (501) staff       (20)     2997 2023-04-13 23:33:14.000000 qnabot-0.0.5/qnabot/QnABot.py
+-rw-r--r--   0 momegas    (501) staff       (20)       55 2023-04-13 23:53:43.000000 qnabot-0.0.5/qnabot/__init__.py
+-rw-r--r--   0 momegas    (501) staff       (20)      267 2023-04-13 23:52:46.000000 qnabot-0.0.5/qnabot/api.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:57:45.014810 qnabot-0.0.5/qnabot/tests/
+-rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-12 18:37:58.000000 qnabot-0.0.5/qnabot/tests/__init__.py
+-rw-r--r--   0 momegas    (501) staff       (20)     1484 2023-04-13 23:17:41.000000 qnabot-0.0.5/qnabot/tests/test_QnABot.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-13 23:57:45.014618 qnabot-0.0.5/qnabot.egg-info/
+-rw-r--r--   0 momegas    (501) staff       (20)     3521 2023-04-13 23:57:44.000000 qnabot-0.0.5/qnabot.egg-info/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)      270 2023-04-13 23:57:44.000000 qnabot-0.0.5/qnabot.egg-info/SOURCES.txt
+-rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-13 23:57:44.000000 qnabot-0.0.5/qnabot.egg-info/dependency_links.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       50 2023-04-13 23:57:44.000000 qnabot-0.0.5/qnabot.egg-info/requires.txt
+-rw-r--r--   0 momegas    (501) staff       (20)        7 2023-04-13 23:57:44.000000 qnabot-0.0.5/qnabot.egg-info/top_level.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-13 23:57:45.015232 qnabot-0.0.5/setup.cfg
+-rw-r--r--   0 momegas    (501) staff       (20)      739 2023-04-13 23:57:19.000000 qnabot-0.0.5/setup.py
```

### Comparing `qnabot-0.0.4/PKG-INFO` & `qnabot-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnabot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create a question answering over docs bot with one line of code.
 Home-page: https://github.com/momegas/qnabot
 Author: Megaklis Vasilakis
 Author-email: megaklis.vasilakis@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -35,23 +35,31 @@
 # Save the index to save costs (GPT is used to create the index)
 bot.save_index("index.pickle")
 
 # Load the index from a previous run
 bot = QnABot(directory="./mydata", index="index.pickle")
 ```
 
+You can also create a FastAPI app that will expose the bot as an API. You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
+
+```python
+from qnabot import QnABot, create_app
+
+app = create_app(QnABot("./examples/files"))
+```
+
 ### Features
 
 - [x] Create a question answering bot over your documents with one line of code using GPT
 - [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
 - [x] Local data source (directory of documents) or S3 data source
 - [x] FAISS for storing vectors / index
+- [x] Expose bot over API using FastAPI
 - [ ] Support for other vector databases (e.g. Weaviate, Pinecone)
 - [ ] Customise prompt
-- [ ] Expose API
 - [ ] Support for LLaMA model
 - [ ] Support for Anthropic models
 - [ ] CLI / UI
 
 ### Here's how it works
 
 Large language models (LLMs) are powerful, but they can't answer questions about documents they haven't seen. If you want to use an LLM to answer questions about documents it was not trained on, you have to give it information about those documents. To solve this, we use "retrieval augmented generation."
```

### Comparing `qnabot-0.0.4/README.md` & `qnabot-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,23 +23,31 @@
 # Save the index to save costs (GPT is used to create the index)
 bot.save_index("index.pickle")
 
 # Load the index from a previous run
 bot = QnABot(directory="./mydata", index="index.pickle")
 ```
 
+You can also create a FastAPI app that will expose the bot as an API. You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
+
+```python
+from qnabot import QnABot, create_app
+
+app = create_app(QnABot("./examples/files"))
+```
+
 ### Features
 
 - [x] Create a question answering bot over your documents with one line of code using GPT
 - [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
 - [x] Local data source (directory of documents) or S3 data source
 - [x] FAISS for storing vectors / index
+- [x] Expose bot over API using FastAPI
 - [ ] Support for other vector databases (e.g. Weaviate, Pinecone)
 - [ ] Customise prompt
-- [ ] Expose API
 - [ ] Support for LLaMA model
 - [ ] Support for Anthropic models
 - [ ] CLI / UI
 
 ### Here's how it works
 
 Large language models (LLMs) are powerful, but they can't answer questions about documents they haven't seen. If you want to use an LLM to answer questions about documents it was not trained on, you have to give it information about those documents. To solve this, we use "retrieval augmented generation."
```

### Comparing `qnabot-0.0.4/qnabot/QnABot.py` & `qnabot-0.0.5/qnabot/QnABot.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from langchain.chat_models import ChatOpenAI
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.document_loaders import DirectoryLoader, S3DirectoryLoader
 from langchain.chains.qa_with_sources import load_qa_with_sources_chain
 from langchain.vectorstores.faiss import FAISS
 import pickle
 import os
-from langchain.chains.combine_documents.stuff import StuffDocumentsChain
 
 
 class QnABot:
     def __init__(
         self,
         directory: str,
         index: str | None = None,
```

### Comparing `qnabot-0.0.4/qnabot/tests/test_QnABot.py` & `qnabot-0.0.5/qnabot/tests/test_QnABot.py`

 * *Files identical despite different names*

### Comparing `qnabot-0.0.4/qnabot.egg-info/PKG-INFO` & `qnabot-0.0.5/qnabot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnabot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create a question answering over docs bot with one line of code.
 Home-page: https://github.com/momegas/qnabot
 Author: Megaklis Vasilakis
 Author-email: megaklis.vasilakis@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -35,23 +35,31 @@
 # Save the index to save costs (GPT is used to create the index)
 bot.save_index("index.pickle")
 
 # Load the index from a previous run
 bot = QnABot(directory="./mydata", index="index.pickle")
 ```
 
+You can also create a FastAPI app that will expose the bot as an API. You should then be able to visit `http://localhost:8000/docs` to see the API documentation.
+
+```python
+from qnabot import QnABot, create_app
+
+app = create_app(QnABot("./examples/files"))
+```
+
 ### Features
 
 - [x] Create a question answering bot over your documents with one line of code using GPT
 - [x] Save / load index to reduce costs (Open AI embedings are used to create the index)
 - [x] Local data source (directory of documents) or S3 data source
 - [x] FAISS for storing vectors / index
+- [x] Expose bot over API using FastAPI
 - [ ] Support for other vector databases (e.g. Weaviate, Pinecone)
 - [ ] Customise prompt
-- [ ] Expose API
 - [ ] Support for LLaMA model
 - [ ] Support for Anthropic models
 - [ ] CLI / UI
 
 ### Here's how it works
 
 Large language models (LLMs) are powerful, but they can't answer questions about documents they haven't seen. If you want to use an LLM to answer questions about documents it was not trained on, you have to give it information about those documents. To solve this, we use "retrieval augmented generation."
```

### Comparing `qnabot-0.0.4/setup.py` & `qnabot-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 
 setup(
     name="qnabot",
     version=VERSION,
     packages=find_packages(),
     install_requires=[
         "langchain",
```

