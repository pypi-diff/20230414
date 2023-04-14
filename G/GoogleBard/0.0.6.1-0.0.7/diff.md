# Comparing `tmp/GoogleBard-0.0.6.1.tar.gz` & `tmp/GoogleBard-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleBard-0.0.6.1.tar", last modified: Thu Mar 30 01:22:44 2023, max compression
+gzip compressed data, was "GoogleBard-0.0.7.tar", last modified: Fri Apr 14 12:23:00 2023, max compression
```

## Comparing `GoogleBard-0.0.6.1.tar` & `GoogleBard-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:22:44.971226 GoogleBard-0.0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 01:22:19.000000 GoogleBard-0.0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-30 01:22:44.971226 GoogleBard-0.0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-30 01:22:19.000000 GoogleBard-0.0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 01:22:44.971226 GoogleBard-0.0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-30 01:22:19.000000 GoogleBard-0.0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:22:44.971226 GoogleBard-0.0.6.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-03-30 01:22:19.000000 GoogleBard-0.0.6.1/src/Bard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:22:44.971226 GoogleBard-0.0.6.1/src/GoogleBard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-30 01:22:44.000000 GoogleBard-0.0.6.1/src/GoogleBard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-30 01:22:44.000000 GoogleBard-0.0.6.1/src/GoogleBard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 01:22:44.000000 GoogleBard-0.0.6.1/src/GoogleBard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-30 01:22:44.000000 GoogleBard-0.0.6.1/src/GoogleBard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-30 01:22:44.000000 GoogleBard-0.0.6.1/src/GoogleBard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:23:00.916013 GoogleBard-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 12:22:38.000000 GoogleBard-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-14 12:23:00.916013 GoogleBard-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-14 12:22:38.000000 GoogleBard-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:23:00.916013 GoogleBard-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 12:22:38.000000 GoogleBard-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:23:00.916013 GoogleBard-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-14 12:22:38.000000 GoogleBard-0.0.7/src/Bard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:23:00.916013 GoogleBard-0.0.7/src/GoogleBard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-14 12:23:00.000000 GoogleBard-0.0.7/src/GoogleBard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 12:23:00.000000 GoogleBard-0.0.7/src/GoogleBard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:23:00.000000 GoogleBard-0.0.7/src/GoogleBard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 12:23:00.000000 GoogleBard-0.0.7/src/GoogleBard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 12:23:00.000000 GoogleBard-0.0.7/src/GoogleBard.egg-info/top_level.txt
```

### Comparing `GoogleBard-0.0.6.1/LICENSE` & `GoogleBard-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleBard-0.0.6.1/PKG-INFO` & `GoogleBard-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 0.0.6.1
+Version: 0.0.7
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
-License: GNU General Public License v2.0
+License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,11 +40,20 @@
 
 options:
   -h, --help         show this help message and exit
   --session SESSION  __Secure-1PSID cookie.
 ```
 
 ## [Developer Documentation](https://github.com/acheong08/Bard/blob/main/DOCUMENTATION.md)
+```python
+from os import environ
+from Bard import Chatbot
 
+token = environ.get("BARD_TOKEN")
+
+chatbot = Chatbot(token)
+
+chatbot.ask("Hello, how are you?")
+```
 
 Credits:
 - [discordtehe](https://github.com/discordtehe) - Derivative of his original reverse engineering
```

### Comparing `GoogleBard-0.0.6.1/setup.py` & `GoogleBard-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="GoogleBard",
-    version="0.0.6.1",
-    license="GNU General Public License v2.0",
+    version="0.0.7",
+    license="MIT License",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineering of Google's Bard chatbot",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/Bard",
     project_urls={"Bug Report": "https://github.com/acheong08/Bard/issues/new"},
```

### Comparing `GoogleBard-0.0.6.1/src/Bard.py` & `GoogleBard-0.0.7/src/Bard.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Reverse engineering of Google Bard
 """
 import argparse
 import json
 import random
 import re
 import string
+import os
+import sys
 
 import requests
 from prompt_toolkit import prompt
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
@@ -146,27 +148,38 @@
         """
         Bard - A command-line interface to Google's Bard (https://bard.google.com/)
         Repo: github.com/acheong08/Bard
 
         Enter `alt+enter` or `esc+enter` to send a message.
         """,
     )
+    console = Console()
+    if os.getenv("BARD_QUICK"):
+        session = os.getenv("BARD_SESSION")
+        if not session:
+            print("BARD_SESSION environment variable not set.")
+            sys.exit(1)
+        chatbot = Chatbot(session)
+        # Join arguments into a single string
+        MESSAGE = " ".join(sys.argv[1:])
+        console.print(Markdown(chatbot.ask(MESSAGE)["content"]))
+        sys.exit(0)
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--session",
         help="__Secure-1PSID cookie.",
         type=str,
         required=True,
     )
     args = parser.parse_args()
 
     chatbot = Chatbot(args.session)
     prompt_session = __create_session()
     completions = __create_completer(["!exit", "!reset"])
-    console = Console()
+
     try:
         while True:
             console.print("You:")
             user_prompt = __get_input(session=prompt_session, completer=completions)
             console.print()
             if user_prompt == "!exit":
                 break
```

### Comparing `GoogleBard-0.0.6.1/src/GoogleBard.egg-info/PKG-INFO` & `GoogleBard-0.0.7/src/GoogleBard.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: GoogleBard
-Version: 0.0.6.1
+Version: 0.0.7
 Summary: Reverse engineering of Google's Bard chatbot
 Home-page: https://github.com/acheong08/Bard
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
-License: GNU General Public License v2.0
+License: MIT License
 Project-URL: Bug Report, https://github.com/acheong08/Bard/issues/new
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,11 +40,20 @@
 
 options:
   -h, --help         show this help message and exit
   --session SESSION  __Secure-1PSID cookie.
 ```
 
 ## [Developer Documentation](https://github.com/acheong08/Bard/blob/main/DOCUMENTATION.md)
+```python
+from os import environ
+from Bard import Chatbot
 
+token = environ.get("BARD_TOKEN")
+
+chatbot = Chatbot(token)
+
+chatbot.ask("Hello, how are you?")
+```
 
 Credits:
 - [discordtehe](https://github.com/discordtehe) - Derivative of his original reverse engineering
```

