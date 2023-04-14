# Comparing `tmp/chatarena-0.1.8.tar.gz` & `tmp/chatarena-0.1.8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatarena-0.1.8.tar", last modified: Thu Apr 13 16:45:14 2023, max compression
+gzip compressed data, was "chatarena-0.1.8.dev0.tar", last modified: Fri Apr 14 21:18:39 2023, max compression
```

## Comparing `chatarena-0.1.8.tar` & `chatarena-0.1.8.dev0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-13 16:45:14.663982 chatarena-0.1.8/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    11404 2023-04-03 15:56:48.000000 chatarena-0.1.8/LICENSE
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    12250 2023-04-13 16:45:14.663591 chatarena-0.1.8/PKG-INFO
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    11657 2023-04-12 19:45:36.000000 chatarena-0.1.8/README.md
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-13 16:45:14.654802 chatarena-0.1.8/chatarena/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        0 2023-04-03 15:56:48.000000 chatarena-0.1.8/chatarena/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4899 2023-04-12 22:43:42.000000 chatarena-0.1.8/chatarena/agent.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     6681 2023-04-06 00:43:37.000000 chatarena-0.1.8/chatarena/arena.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-13 16:45:14.660732 chatarena-0.1.8/chatarena/backends/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      749 2023-04-12 22:35:18.000000 chatarena-0.1.8/chatarena/backends/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3859 2023-04-12 23:12:18.000000 chatarena-0.1.8/chatarena/backends/anthropic.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     1337 2023-04-12 22:43:42.000000 chatarena-0.1.8/chatarena/backends/base.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4088 2023-04-12 22:43:42.000000 chatarena-0.1.8/chatarena/backends/cohere.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3613 2023-04-12 22:42:35.000000 chatarena-0.1.8/chatarena/backends/hf_transformers.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      669 2023-04-04 12:55:00.000000 chatarena-0.1.8/chatarena/backends/human.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     3646 2023-04-12 22:43:42.000000 chatarena-0.1.8/chatarena/backends/openai.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4839 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/config.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4671 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/database.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-13 16:45:14.663104 chatarena-0.1.8/chatarena/environments/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      700 2023-04-06 00:43:37.000000 chatarena-0.1.8/chatarena/environments/__init__.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2647 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/environments/base.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    11463 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/environments/chameleon.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     6153 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/environments/conversation.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     4757 2023-04-05 14:34:27.000000 chatarena-0.1.8/chatarena/environments/pettingzoo_chess.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)     2794 2023-04-12 22:12:06.000000 chatarena-0.1.8/chatarena/message.py
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      827 2023-04-03 15:56:48.000000 chatarena-0.1.8/chatarena/utils.py
-drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-13 16:45:14.656742 chatarena-0.1.8/chatarena.egg-info/
--rw-r--r--   0 yuxiangwu   (501) staff       (20)    12250 2023-04-13 16:45:14.000000 chatarena-0.1.8/chatarena.egg-info/PKG-INFO
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      745 2023-04-13 16:45:14.000000 chatarena-0.1.8/chatarena.egg-info/SOURCES.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)        1 2023-04-13 16:45:14.000000 chatarena-0.1.8/chatarena.egg-info/dependency_links.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      111 2023-04-13 16:45:14.000000 chatarena-0.1.8/chatarena.egg-info/requires.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)       10 2023-04-13 16:45:14.000000 chatarena-0.1.8/chatarena.egg-info/top_level.txt
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      603 2023-04-13 12:35:26.000000 chatarena-0.1.8/pyproject.toml
--rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2023-04-13 16:45:14.664063 chatarena-0.1.8/setup.cfg
--rw-r--r--   0 yuxiangwu   (501) staff       (20)      866 2023-04-13 12:35:26.000000 chatarena-0.1.8/setup.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-14 21:18:39.783217 chatarena-0.1.8.dev0/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    11404 2023-04-03 15:56:48.000000 chatarena-0.1.8.dev0/LICENSE
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    12435 2023-04-14 21:18:39.782875 chatarena-0.1.8.dev0/PKG-INFO
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    11837 2023-04-14 21:15:02.000000 chatarena-0.1.8.dev0/README.md
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-14 21:18:39.774672 chatarena-0.1.8.dev0/chatarena/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)        0 2023-04-03 15:56:48.000000 chatarena-0.1.8.dev0/chatarena/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4899 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/agent.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     6690 2023-04-14 21:14:59.000000 chatarena-0.1.8.dev0/chatarena/arena.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-14 21:18:39.779924 chatarena-0.1.8.dev0/chatarena/backends/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      749 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/backends/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3869 2023-04-14 21:14:59.000000 chatarena-0.1.8.dev0/chatarena/backends/anthropic.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     1337 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/backends/base.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4088 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/backends/cohere.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3613 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/backends/hf_transformers.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      669 2023-04-04 12:55:00.000000 chatarena-0.1.8.dev0/chatarena/backends/human.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     3656 2023-04-14 21:14:59.000000 chatarena-0.1.8.dev0/chatarena/backends/openai.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4839 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/config.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4671 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/database.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-14 21:18:39.782457 chatarena-0.1.8.dev0/chatarena/environments/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      700 2023-04-06 00:43:37.000000 chatarena-0.1.8.dev0/chatarena/environments/__init__.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2647 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/environments/base.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    11463 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/environments/chameleon.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     6153 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/environments/conversation.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     4757 2023-04-05 14:34:27.000000 chatarena-0.1.8.dev0/chatarena/environments/pettingzoo_chess.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)     2794 2023-04-13 17:13:03.000000 chatarena-0.1.8.dev0/chatarena/message.py
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      827 2023-04-03 15:56:48.000000 chatarena-0.1.8.dev0/chatarena/utils.py
+drwxr-xr-x   0 yuxiangwu   (501) staff       (20)        0 2023-04-14 21:18:39.776788 chatarena-0.1.8.dev0/chatarena.egg-info/
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)    12435 2023-04-14 21:18:39.000000 chatarena-0.1.8.dev0/chatarena.egg-info/PKG-INFO
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      745 2023-04-14 21:18:39.000000 chatarena-0.1.8.dev0/chatarena.egg-info/SOURCES.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)        1 2023-04-14 21:18:39.000000 chatarena-0.1.8.dev0/chatarena.egg-info/dependency_links.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      111 2023-04-14 21:18:39.000000 chatarena-0.1.8.dev0/chatarena.egg-info/requires.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)       10 2023-04-14 21:18:39.000000 chatarena-0.1.8.dev0/chatarena.egg-info/top_level.txt
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      608 2023-04-14 21:17:28.000000 chatarena-0.1.8.dev0/pyproject.toml
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)       38 2023-04-14 21:18:39.783301 chatarena-0.1.8.dev0/setup.cfg
+-rw-r--r--   0 yuxiangwu   (501) staff       (20)      871 2023-04-14 21:18:19.000000 chatarena-0.1.8.dev0/setup.py
```

### Comparing `chatarena-0.1.8/LICENSE` & `chatarena-0.1.8.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/PKG-INFO` & `chatarena-0.1.8.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: chatarena
-Version: 0.1.8
+Version: 0.1.8.dev0
 Summary: Multi-Agent Language Game Environments for LLMs
 Home-page: https://github.com/chatarena/chatarena
 Author: Yuxiang Wu
 Author-email: Yuxiang Wu <yuxiang.cs@gmail.com>
 Project-URL: Homepage, https://github.com/chatarena/chatarena
 Project-URL: Bug Tracker, https://github.com/chatarena/chatarena/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<!--
+  Title: Chat Arena
+  Description: Chat Arena (or ChatArena) is a language game environment for Large Language Models (LLMs) like GPT-3, GPT-4, ChatGPT, etc.
+  Author: Yuxiang Wu
+  -->
+
 <h1 align="center"> 🏟 <span style="color:orange">ChatArena</span> </h1>
 
 <h3 align="center">
     <p>Multi-Agent Language Game Environments for LLMs</p>
 </h3>
 
 
@@ -25,22 +31,22 @@
 [![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/)
 [![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![twitter](https://img.shields.io/twitter/follow/_chatarena?style=social&label=Follow%20ChatArena)](https://twitter.com/_chatarena)
 [![slack](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
 
 ---
 
-ChatArena is a Python library designed to facilitate communication and collaboration between multiple large language
-models (LLMs).
+ChatArena is a Python library designed to facilitate communication and collaboration between multiple Large Language
+Models (LLMs).
 It provides the following features:
 
-- **Language Game Environments**: it provides a framework for creating multi-agent language game environments, and a set
+- **Language Game Environments**: it provides a framework for creating multi-agent language game environments and a set
   of general-purposed language-driven environments.
-- **Infrastructure for Multi-LLM Interaction**: it allows you to quickly create multiple LLM-powered player agents, and
-  enables seamlessly communication between them.
+- **Infrastructure for Multi-LLM Interaction**: it allows you to quickly create multiple LLM-powered player agents and
+  enables seamless communication between them.
 - **User-friendly Interfaces**: it provides both Web browser UI and command line interface (CLI) to develop (prompt
   engineer) your LLM players to succeed in the environment.
 
 ![ChatArena Architecture](docs/images/chatarena_architecture.png)
 
 ## Getting Started
 
@@ -60,17 +66,15 @@
 ```bash
 pip install chatarena
 ```
 
 or install from source:
 
 ```bash
-git clone https://github.com/chatarena/chatarena
-cd chatarena
-pip install .
+pip install git+https://github.com/chatarena/chatarena
 ```
 
 To use GPT-3 as an LLM agent, set your OpenAI API key:
 
 ```bash
 export OPENAI_API_KEY="your_api_key_here"
 ```
@@ -81,15 +85,15 @@
 To launch the demo on your local machine, you first need to git clone the repository and install it from source
 (see above instruction). Then run the following command in the root directory of the repository:
 
 ```shell
 gradio app.py
 ```
 
-This will launch a demo server for ChatArena and you can access it in your browser.
+This will launch a demo server for ChatArena, and you can access it from your browser.
 
 [//]: # (The interface looks like this:)
 
 [//]: # (![webui screenshot]&#40;docs/images/webui.png&#41;)
 
 Check out this video to learn how to use Web
 UI: [![Webui demo video](https://img.shields.io/badge/WebUI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
@@ -102,15 +106,15 @@
   its name, its backend, and its role description.
     - **Backend**: a backend is a class that actually processes queries and generates responses in a conversation. A
       backend can be a human, a remote or local LLM, or any program you create.
 - **Environment**: an environment is a class that defines the rules of a game and the game state transition.
     - **Moderator**: a moderator is a special type of player that can control the game environment. It allows you to
       define game environments using an LLM.
 - **Arena**: an arena is a utility class that contains the game environment and the players. It enables you to easily
-  run the game and save the game history, as well as interacting with the game via Web UI or CLI.
+  run the game and save the game history, and interact with the game via the Web UI or CLI.
 
 ### Step 1: Define Multiple Players with LLM Backend
 
 ```python
 from chatarena.agent import Player
 from chatarena.backends import OpenAIChat
 
@@ -123,15 +127,15 @@
                  global_prompt=environment_description)
 # A "Student" player
 player2 = Player(name="Student", backend=OpenAIChat(),
                  role_desc="You are a student who is interested in ...",
                  global_prompt=environment_description)
 # A "Teaching Assistant" player
 player3 = Player(name="Teaching assistant", backend=OpenAIChat(),
-                 role_desc="You are a teaching assistant of module ...",
+                 role_desc="You are a teaching assistant of the module ...",
                  global_prompt=environment_description)
 ```
 
 ### Step 2: Create a Language Game Environment
 
 You can also create a language model-driven environment and add it to the ChatArena:
 
@@ -139,15 +143,15 @@
 from chatarena.environments.conversation import Conversation
 
 env = Conversation(player_names=[p.name for p in [player1, player2, player3]])
 ```
 
 ### Step 3: Run the Language Game using Arena
 
-Arena is a utility class to help you run language games.
+`Arena` is a utility class to help you run language games:
 
 ```python
 from chatarena.arena import Arena
 
 arena = Arena(players=[player1, player2, player3],
               environment=env, global_prompt=environment_description)
 # Run the game for 10 steps
@@ -155,36 +159,36 @@
 
 # Alternatively, you can run your own main loop
 for _ in range(10):
     arena.step()
     # Your code goes here ...
 ```
 
-You can easily save your game play history to file
+You can easily save your gameplay history to file:
 
 ```python
 arena.save_history(path=...)
 ```
 
-and save your game config to file
+and save your game config to file:
 
 ```python
 arena.save_config(path=...)
 ```
 
 ### Other Utilities
 
-Load Arena from config file (here we use `examples/nlp-classroom-3players.json` in this repository as an example)
+Load `Arena` from a config file -- here we use `examples/nlp-classroom-3players.json` in this repository as an example:
 
 ```python
 arena = Arena.from_config("examples/nlp-classroom-3players.json")
 arena.run(num_steps=10)
 ```
 
-Run the game in an interactive CLI interface
+Run the game in an interactive CLI interface:
 
 ```python
 arena.launch_cli()
 ```
 
 Check out this video to learn how to use
 CLI: [![cli demo video](https://img.shields.io/badge/CLI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816989884)
@@ -192,15 +196,15 @@
 ## Advanced Usage
 
 ### `ModeratedConversation`: a LLM-driven Environment
 
 We support a more advanced environment called `ModeratedConversation` that allows you to **control the game dynamics
 using an LLM**.
 The moderator is a special player that controls the game state transition and determines when the game ends.
-For example, you can define a moderator that track the board status of a board game, and end the game when a player
+For example, you can define a moderator that tracks the board status of a board game and ends the game when a player
 wins.
 You can try out our Tic-tac-toe and Rock-paper-scissors games to get a sense of how it works:
 
 ```python
 # Tic-tac-toe example
 Arena.from_config("examples/tic-tac-toe.json").launch_cli()
 
@@ -215,15 +219,15 @@
 1. Define the class by inheriting from a base class and setting `type_name`, then add the class
    to [`ALL_ENVIRONMENTS`](chatarena/environments/__init__.py#L17)
 2. Initialize the class by defining `__init__` method (its arguments will define the corresponding config) and
    initializing class attributes
 3. Implement game mechanics in methods `step`
 4. Handle game states and rewards by implementing methods such as `reset`, `get_observation`, `is_terminal`,
    and `get_rewards`
-5. Develop role description prompts (and global prompt if necessary) for players using CLI or Web UI and save them to a
+5. Develop role description prompts (and a global prompt if necessary) for players using CLI or Web UI and save them to a
    config file.
 
 We provide [a detailed tutorial](docs/tutorials/create_your_environment.md) to demonstrate how to define a custom
 environment,
 using the [`Chameleon` environment](chatarena/environments/chameleon.py) as example.
 
 If you want to port an existing library's environment to ChatArena, check
```

### Comparing `chatarena-0.1.8/README.md` & `chatarena-0.1.8.dev0/chatarena.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: chatarena
+Version: 0.1.8.dev0
+Summary: Multi-Agent Language Game Environments for LLMs
+Home-page: https://github.com/chatarena/chatarena
+Author: Yuxiang Wu
+Author-email: Yuxiang Wu <yuxiang.cs@gmail.com>
+Project-URL: Homepage, https://github.com/chatarena/chatarena
+Project-URL: Bug Tracker, https://github.com/chatarena/chatarena/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<!--
+  Title: Chat Arena
+  Description: Chat Arena (or ChatArena) is a language game environment for Large Language Models (LLMs) like GPT-3, GPT-4, ChatGPT, etc.
+  Author: Yuxiang Wu
+  -->
+
 <h1 align="center"> 🏟 <span style="color:orange">ChatArena</span> </h1>
 
 <h3 align="center">
     <p>Multi-Agent Language Game Environments for LLMs</p>
 </h3>
 
 
@@ -9,22 +31,22 @@
 [![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/)
 [![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![twitter](https://img.shields.io/twitter/follow/_chatarena?style=social&label=Follow%20ChatArena)](https://twitter.com/_chatarena)
 [![slack](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
 
 ---
 
-ChatArena is a Python library designed to facilitate communication and collaboration between multiple large language
-models (LLMs).
+ChatArena is a Python library designed to facilitate communication and collaboration between multiple Large Language
+Models (LLMs).
 It provides the following features:
 
-- **Language Game Environments**: it provides a framework for creating multi-agent language game environments, and a set
+- **Language Game Environments**: it provides a framework for creating multi-agent language game environments and a set
   of general-purposed language-driven environments.
-- **Infrastructure for Multi-LLM Interaction**: it allows you to quickly create multiple LLM-powered player agents, and
-  enables seamlessly communication between them.
+- **Infrastructure for Multi-LLM Interaction**: it allows you to quickly create multiple LLM-powered player agents and
+  enables seamless communication between them.
 - **User-friendly Interfaces**: it provides both Web browser UI and command line interface (CLI) to develop (prompt
   engineer) your LLM players to succeed in the environment.
 
 ![ChatArena Architecture](docs/images/chatarena_architecture.png)
 
 ## Getting Started
 
@@ -44,17 +66,15 @@
 ```bash
 pip install chatarena
 ```
 
 or install from source:
 
 ```bash
-git clone https://github.com/chatarena/chatarena
-cd chatarena
-pip install .
+pip install git+https://github.com/chatarena/chatarena
 ```
 
 To use GPT-3 as an LLM agent, set your OpenAI API key:
 
 ```bash
 export OPENAI_API_KEY="your_api_key_here"
 ```
@@ -65,15 +85,15 @@
 To launch the demo on your local machine, you first need to git clone the repository and install it from source
 (see above instruction). Then run the following command in the root directory of the repository:
 
 ```shell
 gradio app.py
 ```
 
-This will launch a demo server for ChatArena and you can access it in your browser.
+This will launch a demo server for ChatArena, and you can access it from your browser.
 
 [//]: # (The interface looks like this:)
 
 [//]: # (![webui screenshot]&#40;docs/images/webui.png&#41;)
 
 Check out this video to learn how to use Web
 UI: [![Webui demo video](https://img.shields.io/badge/WebUI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
@@ -86,15 +106,15 @@
   its name, its backend, and its role description.
     - **Backend**: a backend is a class that actually processes queries and generates responses in a conversation. A
       backend can be a human, a remote or local LLM, or any program you create.
 - **Environment**: an environment is a class that defines the rules of a game and the game state transition.
     - **Moderator**: a moderator is a special type of player that can control the game environment. It allows you to
       define game environments using an LLM.
 - **Arena**: an arena is a utility class that contains the game environment and the players. It enables you to easily
-  run the game and save the game history, as well as interacting with the game via Web UI or CLI.
+  run the game and save the game history, and interact with the game via the Web UI or CLI.
 
 ### Step 1: Define Multiple Players with LLM Backend
 
 ```python
 from chatarena.agent import Player
 from chatarena.backends import OpenAIChat
 
@@ -107,15 +127,15 @@
                  global_prompt=environment_description)
 # A "Student" player
 player2 = Player(name="Student", backend=OpenAIChat(),
                  role_desc="You are a student who is interested in ...",
                  global_prompt=environment_description)
 # A "Teaching Assistant" player
 player3 = Player(name="Teaching assistant", backend=OpenAIChat(),
-                 role_desc="You are a teaching assistant of module ...",
+                 role_desc="You are a teaching assistant of the module ...",
                  global_prompt=environment_description)
 ```
 
 ### Step 2: Create a Language Game Environment
 
 You can also create a language model-driven environment and add it to the ChatArena:
 
@@ -123,15 +143,15 @@
 from chatarena.environments.conversation import Conversation
 
 env = Conversation(player_names=[p.name for p in [player1, player2, player3]])
 ```
 
 ### Step 3: Run the Language Game using Arena
 
-Arena is a utility class to help you run language games.
+`Arena` is a utility class to help you run language games:
 
 ```python
 from chatarena.arena import Arena
 
 arena = Arena(players=[player1, player2, player3],
               environment=env, global_prompt=environment_description)
 # Run the game for 10 steps
@@ -139,36 +159,36 @@
 
 # Alternatively, you can run your own main loop
 for _ in range(10):
     arena.step()
     # Your code goes here ...
 ```
 
-You can easily save your game play history to file
+You can easily save your gameplay history to file:
 
 ```python
 arena.save_history(path=...)
 ```
 
-and save your game config to file
+and save your game config to file:
 
 ```python
 arena.save_config(path=...)
 ```
 
 ### Other Utilities
 
-Load Arena from config file (here we use `examples/nlp-classroom-3players.json` in this repository as an example)
+Load `Arena` from a config file -- here we use `examples/nlp-classroom-3players.json` in this repository as an example:
 
 ```python
 arena = Arena.from_config("examples/nlp-classroom-3players.json")
 arena.run(num_steps=10)
 ```
 
-Run the game in an interactive CLI interface
+Run the game in an interactive CLI interface:
 
 ```python
 arena.launch_cli()
 ```
 
 Check out this video to learn how to use
 CLI: [![cli demo video](https://img.shields.io/badge/CLI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816989884)
@@ -176,15 +196,15 @@
 ## Advanced Usage
 
 ### `ModeratedConversation`: a LLM-driven Environment
 
 We support a more advanced environment called `ModeratedConversation` that allows you to **control the game dynamics
 using an LLM**.
 The moderator is a special player that controls the game state transition and determines when the game ends.
-For example, you can define a moderator that track the board status of a board game, and end the game when a player
+For example, you can define a moderator that tracks the board status of a board game and ends the game when a player
 wins.
 You can try out our Tic-tac-toe and Rock-paper-scissors games to get a sense of how it works:
 
 ```python
 # Tic-tac-toe example
 Arena.from_config("examples/tic-tac-toe.json").launch_cli()
 
@@ -199,15 +219,15 @@
 1. Define the class by inheriting from a base class and setting `type_name`, then add the class
    to [`ALL_ENVIRONMENTS`](chatarena/environments/__init__.py#L17)
 2. Initialize the class by defining `__init__` method (its arguments will define the corresponding config) and
    initializing class attributes
 3. Implement game mechanics in methods `step`
 4. Handle game states and rewards by implementing methods such as `reset`, `get_observation`, `is_terminal`,
    and `get_rewards`
-5. Develop role description prompts (and global prompt if necessary) for players using CLI or Web UI and save them to a
+5. Develop role description prompts (and a global prompt if necessary) for players using CLI or Web UI and save them to a
    config file.
 
 We provide [a detailed tutorial](docs/tutorials/create_your_environment.md) to demonstrate how to define a custom
 environment,
 using the [`Chameleon` environment](chatarena/environments/chameleon.py) as example.
 
 If you want to port an existing library's environment to ChatArena, check
```

### Comparing `chatarena-0.1.8/chatarena/agent.py` & `chatarena-0.1.8.dev0/chatarena/agent.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/arena.py` & `chatarena-0.1.8.dev0/chatarena/arena.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             global_prompt=self.global_prompt
         )
 
     def launch_cli(self, max_steps: int = None, interactive: bool = True):
         """
         launch the command line interface
         """
-        from .ui.cli import ArenaCLI
+        from chatarena.ui.cli import ArenaCLI
         cli = ArenaCLI(self)
         cli.launch(max_steps=max_steps, interactive=interactive)
 
     def save_config(self, path: str):
         """
         save the config to a file
         """
```

### Comparing `chatarena-0.1.8/chatarena/backends/__init__.py` & `chatarena-0.1.8.dev0/chatarena/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/backends/anthropic.py` & `chatarena-0.1.8.dev0/chatarena/backends/anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,10 +91,10 @@
         assert prev_is_human  # The last message should be from the human
         # Add the AI prompt for Claude to generate the response
         prompt = f"{prompt}{anthropic.AI_PROMPT}"
 
         response = self._get_response(prompt, *args, **kwargs)
 
         # Remove the agent name if the response starts with it
-        response = re.sub(rf"^\s*\[{agent_name}]", "", response)
+        response = re.sub(rf"^\s*\[{agent_name}]:?", "", response).strip()
 
         return response
```

### Comparing `chatarena-0.1.8/chatarena/backends/base.py` & `chatarena-0.1.8.dev0/chatarena/backends/base.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/backends/cohere.py` & `chatarena-0.1.8.dev0/chatarena/backends/cohere.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/backends/hf_transformers.py` & `chatarena-0.1.8.dev0/chatarena/backends/hf_transformers.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/backends/human.py` & `chatarena-0.1.8.dev0/chatarena/backends/human.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/backends/openai.py` & `chatarena-0.1.8.dev0/chatarena/backends/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,10 +87,10 @@
             request_prompt = [{"role": "user", "content": request_msg.content}]
         else:
             request_prompt = []
 
         response = self._get_response([system_prompt] + conversations + request_prompt, *args, **kwargs)
 
         # Remove the agent name if the response starts with it
-        response = re.sub(rf"^\s*\[{agent_name}]", "", response)
+        response = re.sub(rf"^\s*\[{agent_name}]:?", "", response).strip()
 
         return response
```

### Comparing `chatarena-0.1.8/chatarena/config.py` & `chatarena-0.1.8.dev0/chatarena/config.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/database.py` & `chatarena-0.1.8.dev0/chatarena/database.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/environments/__init__.py` & `chatarena-0.1.8.dev0/chatarena/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/environments/base.py` & `chatarena-0.1.8.dev0/chatarena/environments/base.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/environments/chameleon.py` & `chatarena-0.1.8.dev0/chatarena/environments/chameleon.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/environments/conversation.py` & `chatarena-0.1.8.dev0/chatarena/environments/conversation.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/environments/pettingzoo_chess.py` & `chatarena-0.1.8.dev0/chatarena/environments/pettingzoo_chess.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/message.py` & `chatarena-0.1.8.dev0/chatarena/message.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena/utils.py` & `chatarena-0.1.8.dev0/chatarena/utils.py`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/chatarena.egg-info/PKG-INFO` & `chatarena-0.1.8.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-Metadata-Version: 2.1
-Name: chatarena
-Version: 0.1.8
-Summary: Multi-Agent Language Game Environments for LLMs
-Home-page: https://github.com/chatarena/chatarena
-Author: Yuxiang Wu
-Author-email: Yuxiang Wu <yuxiang.cs@gmail.com>
-Project-URL: Homepage, https://github.com/chatarena/chatarena
-Project-URL: Bug Tracker, https://github.com/chatarena/chatarena/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<!--
+  Title: Chat Arena
+  Description: Chat Arena (or ChatArena) is a language game environment for Large Language Models (LLMs) like GPT-3, GPT-4, ChatGPT, etc.
+  Author: Yuxiang Wu
+  -->
 
 <h1 align="center"> 🏟 <span style="color:orange">ChatArena</span> </h1>
 
 <h3 align="center">
     <p>Multi-Agent Language Game Environments for LLMs</p>
 </h3>
 
@@ -25,22 +15,22 @@
 [![PyPI](https://img.shields.io/pypi/v/chatarena)](https://pypi.org/project/chatarena/)
 [![Python 3.9+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![twitter](https://img.shields.io/twitter/follow/_chatarena?style=social&label=Follow%20ChatArena)](https://twitter.com/_chatarena)
 [![slack](https://img.shields.io/badge/Slack-join-blueviolet?logo=slack&amp)](https://join.slack.com/t/chatarena/shared_invite/zt-1t5fpbiep-CbKucEHdJ5YeDLEpKWxDOg)
 
 ---
 
-ChatArena is a Python library designed to facilitate communication and collaboration between multiple large language
-models (LLMs).
+ChatArena is a Python library designed to facilitate communication and collaboration between multiple Large Language
+Models (LLMs).
 It provides the following features:
 
-- **Language Game Environments**: it provides a framework for creating multi-agent language game environments, and a set
+- **Language Game Environments**: it provides a framework for creating multi-agent language game environments and a set
   of general-purposed language-driven environments.
-- **Infrastructure for Multi-LLM Interaction**: it allows you to quickly create multiple LLM-powered player agents, and
-  enables seamlessly communication between them.
+- **Infrastructure for Multi-LLM Interaction**: it allows you to quickly create multiple LLM-powered player agents and
+  enables seamless communication between them.
 - **User-friendly Interfaces**: it provides both Web browser UI and command line interface (CLI) to develop (prompt
   engineer) your LLM players to succeed in the environment.
 
 ![ChatArena Architecture](docs/images/chatarena_architecture.png)
 
 ## Getting Started
 
@@ -60,17 +50,15 @@
 ```bash
 pip install chatarena
 ```
 
 or install from source:
 
 ```bash
-git clone https://github.com/chatarena/chatarena
-cd chatarena
-pip install .
+pip install git+https://github.com/chatarena/chatarena
 ```
 
 To use GPT-3 as an LLM agent, set your OpenAI API key:
 
 ```bash
 export OPENAI_API_KEY="your_api_key_here"
 ```
@@ -81,15 +69,15 @@
 To launch the demo on your local machine, you first need to git clone the repository and install it from source
 (see above instruction). Then run the following command in the root directory of the repository:
 
 ```shell
 gradio app.py
 ```
 
-This will launch a demo server for ChatArena and you can access it in your browser.
+This will launch a demo server for ChatArena, and you can access it from your browser.
 
 [//]: # (The interface looks like this:)
 
 [//]: # (![webui screenshot]&#40;docs/images/webui.png&#41;)
 
 Check out this video to learn how to use Web
 UI: [![Webui demo video](https://img.shields.io/badge/WebUI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816979419)
@@ -102,15 +90,15 @@
   its name, its backend, and its role description.
     - **Backend**: a backend is a class that actually processes queries and generates responses in a conversation. A
       backend can be a human, a remote or local LLM, or any program you create.
 - **Environment**: an environment is a class that defines the rules of a game and the game state transition.
     - **Moderator**: a moderator is a special type of player that can control the game environment. It allows you to
       define game environments using an LLM.
 - **Arena**: an arena is a utility class that contains the game environment and the players. It enables you to easily
-  run the game and save the game history, as well as interacting with the game via Web UI or CLI.
+  run the game and save the game history, and interact with the game via the Web UI or CLI.
 
 ### Step 1: Define Multiple Players with LLM Backend
 
 ```python
 from chatarena.agent import Player
 from chatarena.backends import OpenAIChat
 
@@ -123,15 +111,15 @@
                  global_prompt=environment_description)
 # A "Student" player
 player2 = Player(name="Student", backend=OpenAIChat(),
                  role_desc="You are a student who is interested in ...",
                  global_prompt=environment_description)
 # A "Teaching Assistant" player
 player3 = Player(name="Teaching assistant", backend=OpenAIChat(),
-                 role_desc="You are a teaching assistant of module ...",
+                 role_desc="You are a teaching assistant of the module ...",
                  global_prompt=environment_description)
 ```
 
 ### Step 2: Create a Language Game Environment
 
 You can also create a language model-driven environment and add it to the ChatArena:
 
@@ -139,15 +127,15 @@
 from chatarena.environments.conversation import Conversation
 
 env = Conversation(player_names=[p.name for p in [player1, player2, player3]])
 ```
 
 ### Step 3: Run the Language Game using Arena
 
-Arena is a utility class to help you run language games.
+`Arena` is a utility class to help you run language games:
 
 ```python
 from chatarena.arena import Arena
 
 arena = Arena(players=[player1, player2, player3],
               environment=env, global_prompt=environment_description)
 # Run the game for 10 steps
@@ -155,36 +143,36 @@
 
 # Alternatively, you can run your own main loop
 for _ in range(10):
     arena.step()
     # Your code goes here ...
 ```
 
-You can easily save your game play history to file
+You can easily save your gameplay history to file:
 
 ```python
 arena.save_history(path=...)
 ```
 
-and save your game config to file
+and save your game config to file:
 
 ```python
 arena.save_config(path=...)
 ```
 
 ### Other Utilities
 
-Load Arena from config file (here we use `examples/nlp-classroom-3players.json` in this repository as an example)
+Load `Arena` from a config file -- here we use `examples/nlp-classroom-3players.json` in this repository as an example:
 
 ```python
 arena = Arena.from_config("examples/nlp-classroom-3players.json")
 arena.run(num_steps=10)
 ```
 
-Run the game in an interactive CLI interface
+Run the game in an interactive CLI interface:
 
 ```python
 arena.launch_cli()
 ```
 
 Check out this video to learn how to use
 CLI: [![cli demo video](https://img.shields.io/badge/CLI%20Demo%20Video-Vimeo-blue?logo=vimeo)](https://vimeo.com/816989884)
@@ -192,15 +180,15 @@
 ## Advanced Usage
 
 ### `ModeratedConversation`: a LLM-driven Environment
 
 We support a more advanced environment called `ModeratedConversation` that allows you to **control the game dynamics
 using an LLM**.
 The moderator is a special player that controls the game state transition and determines when the game ends.
-For example, you can define a moderator that track the board status of a board game, and end the game when a player
+For example, you can define a moderator that tracks the board status of a board game and ends the game when a player
 wins.
 You can try out our Tic-tac-toe and Rock-paper-scissors games to get a sense of how it works:
 
 ```python
 # Tic-tac-toe example
 Arena.from_config("examples/tic-tac-toe.json").launch_cli()
 
@@ -215,15 +203,15 @@
 1. Define the class by inheriting from a base class and setting `type_name`, then add the class
    to [`ALL_ENVIRONMENTS`](chatarena/environments/__init__.py#L17)
 2. Initialize the class by defining `__init__` method (its arguments will define the corresponding config) and
    initializing class attributes
 3. Implement game mechanics in methods `step`
 4. Handle game states and rewards by implementing methods such as `reset`, `get_observation`, `is_terminal`,
    and `get_rewards`
-5. Develop role description prompts (and global prompt if necessary) for players using CLI or Web UI and save them to a
+5. Develop role description prompts (and a global prompt if necessary) for players using CLI or Web UI and save them to a
    config file.
 
 We provide [a detailed tutorial](docs/tutorials/create_your_environment.md) to demonstrate how to define a custom
 environment,
 using the [`Chameleon` environment](chatarena/environments/chameleon.py) as example.
 
 If you want to port an existing library's environment to ChatArena, check
```

### Comparing `chatarena-0.1.8/chatarena.egg-info/SOURCES.txt` & `chatarena-0.1.8.dev0/chatarena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatarena-0.1.8/pyproject.toml` & `chatarena-0.1.8.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatarena"
-version = "0.1.8"
+version = "0.1.8.dev0"
 authors = [
     { name = "Yuxiang Wu", email = "yuxiang.cs@gmail.com" },
 ]
 description = "Multi-Agent Language Game Environments for LLMs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chatarena-0.1.8/setup.py` & `chatarena-0.1.8.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 requirements = _deps
 
 setup(
     name="chatarena",
-    version="0.1.8",
+    version="0.1.8.dev0",
     author="Yuxiang Wu",
     author_email="yuxiang.cs@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/chatarena/chatarena",
     packages=find_packages(),
```

