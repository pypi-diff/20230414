# Comparing `tmp/chat-spiral-0.0.1.tar.gz` & `tmp/chat-spiral-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-spiral-0.0.1.tar", last modified: Fri Apr 14 04:02:20 2023, max compression
+gzip compressed data, was "chat-spiral-0.0.2.tar", last modified: Fri Apr 14 04:49:08 2023, max compression
```

## Comparing `chat-spiral-0.0.1.tar` & `chat-spiral-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 04:02:20.228743 chat-spiral-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 chat-spiral-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    12494 2023-04-14 04:02:20.224754 chat-spiral-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    11971 2023-04-13 05:58:40.000000 chat-spiral-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 04:02:20.223757 chat-spiral-0.0.1/chat_spiral.egg-info/
--rw-rw-rw-   0        0        0    12494 2023-04-14 04:02:19.000000 chat-spiral-0.0.1/chat_spiral.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-04-14 04:02:20.000000 chat-spiral-0.0.1/chat_spiral.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 04:02:19.000000 chat-spiral-0.0.1/chat_spiral.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 04:02:19.000000 chat-spiral-0.0.1/chat_spiral.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 04:02:19.000000 chat-spiral-0.0.1/chat_spiral.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 04:02:20.228743 chat-spiral-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-04-14 04:02:11.000000 chat-spiral-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 04:49:08.865207 chat-spiral-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 chat-spiral-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    12671 2023-04-14 04:49:08.860174 chat-spiral-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12148 2023-04-14 04:47:21.000000 chat-spiral-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 04:49:08.841356 chat-spiral-0.0.2/chat_spiral.egg-info/
+-rw-rw-rw-   0        0        0    12671 2023-04-14 04:49:08.000000 chat-spiral-0.0.2/chat_spiral.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-04-14 04:49:08.000000 chat-spiral-0.0.2/chat_spiral.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 04:49:08.000000 chat-spiral-0.0.2/chat_spiral.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 04:49:08.000000 chat-spiral-0.0.2/chat_spiral.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 04:49:08.000000 chat-spiral-0.0.2/chat_spiral.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 04:49:08.865207 chat-spiral-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-04-14 04:48:27.000000 chat-spiral-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 04:49:08.857181 chat-spiral-0.0.2/spiral/
+-rw-rw-rw-   0        0        0        0 2023-04-14 04:22:39.000000 chat-spiral-0.0.2/spiral/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-04-14 04:47:37.000000 chat-spiral-0.0.2/spiral/chat_history.py
+-rw-rw-rw-   0        0        0     1330 2023-04-14 04:47:37.000000 chat-spiral-0.0.2/spiral/chat_llm.py
+-rw-rw-rw-   0        0        0    50794 2023-04-14 04:47:37.000000 chat-spiral-0.0.2/spiral/flow.py
+-rw-rw-rw-   0        0        0     4276 2023-04-14 04:47:37.000000 chat-spiral-0.0.2/spiral/memory.py
+-rw-rw-rw-   0        0        0    14376 2023-04-11 23:37:20.000000 chat-spiral-0.0.2/spiral/message.py
+-rw-rw-rw-   0        0        0     2202 2023-04-14 04:44:27.000000 chat-spiral-0.0.2/spiral/tools.py
```

### Comparing `chat-spiral-0.0.1/LICENSE` & `chat-spiral-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.1/PKG-INFO` & `chat-spiral-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-spiral
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/spiral
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,35 +38,36 @@
 
 
 Installation
 ------------
 
 To use this project, you will need to install the required dependencies:
 
-1.  Install Python 3.8 or higher.
+1.  Install Python 3.9 or higher.
 2.  Install the `openai` package: `pip install openai`.
 3.  Install the `regex` package: `pip install regex`.
+4.  Install the `spiral` package: `git clone https://github.com/Tiger767/spiral.git` and then `pip install .` inside the repo.
 4.  Make sure OPENAI_API_KEY is set as an environment variable with your OpenAI API key.
 
 Usage
 -----
 
 Here is a quick example to demonstrate how to use the project:
 
 ```python
-from message import (
+from spiral.message import (
     Role,
     InputMessage,
     OutputMessage,
     InputJSONMessage,
     OutputJSONMessage,
 )
-from chat_llm import ChatLLM
-from chat_history import ChatHistory
-from flow import ChatFlow
+from spiral.chat_llm import ChatLLM
+from spiral.chat_history import ChatHistory
+from spiral.flow import ChatFlow
 
 
 # Create input and output messages
 chat_flow = ChatFlow.from_dicts([
     {Role.SYSTEM: 'All your outputs follow the format: The capital of country is capital country.'},
     {Role.USER: 'What is the capital of {country1}?'},
     {Role.ASSISTANT: 'The capital of {country1} is {capital1}.', 'type': 'output'},  # optionally specify the type of message for USER/ASSISTANT
@@ -127,17 +128,17 @@
 Paris is the capital of France, while Madrid is the capital of Spain.
 Assistant: Yes, that statement is true. Paris is the capital of France, while Madrid is the capital of Spain.
 ```
 
 Here is an example using a *spiral* and some of the more advanced features:
 
 ```python
-from message import Role
-from chat_llm import ChatLLM
-from flow import ChatFlow, ConditonalChatFlow, FuncChatFlow, NoHistory, ChatSpiral
+from spiral.message import Role
+from spiral.chat_llm import ChatLLM
+from spiral.flow import ChatFlow, ConditonalChatFlow, FuncChatFlow, NoHistory, ChatSpiral
 
 decision_flow = ChatFlow.from_dicts([
     {Role.USER: 'Options:\n\n'
                 '1. Keep asking and answering questions.\n\n'
                 '2. Choose this when you have provided 2 prompts in the total conversation history.\n\n'
                 'Only respond by typing the number of the option you choose. Say nothing else other than `1` or `2`.'},
     {Role.ASSISTANT: '{decision}'}
```

### Comparing `chat-spiral-0.0.1/README.md` & `chat-spiral-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,35 +24,36 @@
 
 
 Installation
 ------------
 
 To use this project, you will need to install the required dependencies:
 
-1.  Install Python 3.8 or higher.
+1.  Install Python 3.9 or higher.
 2.  Install the `openai` package: `pip install openai`.
 3.  Install the `regex` package: `pip install regex`.
+4.  Install the `spiral` package: `git clone https://github.com/Tiger767/spiral.git` and then `pip install .` inside the repo.
 4.  Make sure OPENAI_API_KEY is set as an environment variable with your OpenAI API key.
 
 Usage
 -----
 
 Here is a quick example to demonstrate how to use the project:
 
 ```python
-from message import (
+from spiral.message import (
     Role,
     InputMessage,
     OutputMessage,
     InputJSONMessage,
     OutputJSONMessage,
 )
-from chat_llm import ChatLLM
-from chat_history import ChatHistory
-from flow import ChatFlow
+from spiral.chat_llm import ChatLLM
+from spiral.chat_history import ChatHistory
+from spiral.flow import ChatFlow
 
 
 # Create input and output messages
 chat_flow = ChatFlow.from_dicts([
     {Role.SYSTEM: 'All your outputs follow the format: The capital of country is capital country.'},
     {Role.USER: 'What is the capital of {country1}?'},
     {Role.ASSISTANT: 'The capital of {country1} is {capital1}.', 'type': 'output'},  # optionally specify the type of message for USER/ASSISTANT
@@ -113,17 +114,17 @@
 Paris is the capital of France, while Madrid is the capital of Spain.
 Assistant: Yes, that statement is true. Paris is the capital of France, while Madrid is the capital of Spain.
 ```
 
 Here is an example using a *spiral* and some of the more advanced features:
 
 ```python
-from message import Role
-from chat_llm import ChatLLM
-from flow import ChatFlow, ConditonalChatFlow, FuncChatFlow, NoHistory, ChatSpiral
+from spiral.message import Role
+from spiral.chat_llm import ChatLLM
+from spiral.flow import ChatFlow, ConditonalChatFlow, FuncChatFlow, NoHistory, ChatSpiral
 
 decision_flow = ChatFlow.from_dicts([
     {Role.USER: 'Options:\n\n'
                 '1. Keep asking and answering questions.\n\n'
                 '2. Choose this when you have provided 2 prompts in the total conversation history.\n\n'
                 'Only respond by typing the number of the option you choose. Say nothing else other than `1` or `2`.'},
     {Role.ASSISTANT: '{decision}'}
```

### Comparing `chat-spiral-0.0.1/chat_spiral.egg-info/PKG-INFO` & `chat-spiral-0.0.2/chat_spiral.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-spiral
-Version: 0.0.1
+Version: 0.0.2
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/spiral
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,35 +38,36 @@
 
 
 Installation
 ------------
 
 To use this project, you will need to install the required dependencies:
 
-1.  Install Python 3.8 or higher.
+1.  Install Python 3.9 or higher.
 2.  Install the `openai` package: `pip install openai`.
 3.  Install the `regex` package: `pip install regex`.
+4.  Install the `spiral` package: `git clone https://github.com/Tiger767/spiral.git` and then `pip install .` inside the repo.
 4.  Make sure OPENAI_API_KEY is set as an environment variable with your OpenAI API key.
 
 Usage
 -----
 
 Here is a quick example to demonstrate how to use the project:
 
 ```python
-from message import (
+from spiral.message import (
     Role,
     InputMessage,
     OutputMessage,
     InputJSONMessage,
     OutputJSONMessage,
 )
-from chat_llm import ChatLLM
-from chat_history import ChatHistory
-from flow import ChatFlow
+from spiral.chat_llm import ChatLLM
+from spiral.chat_history import ChatHistory
+from spiral.flow import ChatFlow
 
 
 # Create input and output messages
 chat_flow = ChatFlow.from_dicts([
     {Role.SYSTEM: 'All your outputs follow the format: The capital of country is capital country.'},
     {Role.USER: 'What is the capital of {country1}?'},
     {Role.ASSISTANT: 'The capital of {country1} is {capital1}.', 'type': 'output'},  # optionally specify the type of message for USER/ASSISTANT
@@ -127,17 +128,17 @@
 Paris is the capital of France, while Madrid is the capital of Spain.
 Assistant: Yes, that statement is true. Paris is the capital of France, while Madrid is the capital of Spain.
 ```
 
 Here is an example using a *spiral* and some of the more advanced features:
 
 ```python
-from message import Role
-from chat_llm import ChatLLM
-from flow import ChatFlow, ConditonalChatFlow, FuncChatFlow, NoHistory, ChatSpiral
+from spiral.message import Role
+from spiral.chat_llm import ChatLLM
+from spiral.flow import ChatFlow, ConditonalChatFlow, FuncChatFlow, NoHistory, ChatSpiral
 
 decision_flow = ChatFlow.from_dicts([
     {Role.USER: 'Options:\n\n'
                 '1. Keep asking and answering questions.\n\n'
                 '2. Choose this when you have provided 2 prompts in the total conversation history.\n\n'
                 'Only respond by typing the number of the option you choose. Say nothing else other than `1` or `2`.'},
     {Role.ASSISTANT: '{decision}'}
```

### Comparing `chat-spiral-0.0.1/setup.py` & `chat-spiral-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chat-spiral",
-    version="0.0.1",
+    version="0.0.2",
     author="Travis Hammond",
     description="A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tiger767/spiral",
     packages=setuptools.find_packages(),
     install_requires=[
```

