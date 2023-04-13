# Comparing `tmp/minichain-0.2.2.tar.gz` & `tmp/minichain-0.2.3.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minichain-0.2.2.tar", last modified: Thu Apr 13 22:46:28 2023, max compression
+gzip compressed data, was "minichain-0.2.3.linux-x86_64.tar", last modified: Thu Apr 13 22:54:27 2023, max compression
```

## Comparing `minichain-0.2.2.tar` & `minichain-0.2.3.linux-x86_64.tar`

### file list

```diff
@@ -1,27 +1,43 @@
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:46:28.020312 minichain-0.2.2/
--rw-rw-r--   0 srush     (1000) srush     (1000)     1067 2023-02-11 23:11:49.000000 minichain-0.2.2/LICENSE
--rw-rw-r--   0 srush     (1000) srush     (1000)     9685 2023-04-13 22:46:28.020312 minichain-0.2.2/PKG-INFO
--rw-rw-r--   0 srush     (1000) srush     (1000)     8799 2023-03-23 19:57:44.000000 minichain-0.2.2/README.md
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:46:28.016312 minichain-0.2.2/minichain/
--rw-rw-r--   0 srush     (1000) srush     (1000)      292 2023-04-13 21:57:58.000000 minichain-0.2.2/minichain/__init__.py
--rw-rw-r--   0 srush     (1000) srush     (1000)    10351 2023-04-13 22:01:03.000000 minichain-0.2.2/minichain/backend.py
--rw-rw-r--   0 srush     (1000) srush     (1000)     9095 2023-04-13 22:29:14.000000 minichain-0.2.2/minichain/base.py
--rw-rw-r--   0 srush     (1000) srush     (1000)    10430 2023-04-13 22:06:15.000000 minichain-0.2.2/minichain/gradio.py
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:46:28.016312 minichain-0.2.2/minichain/prompts/
--rw-rw-r--   0 srush     (1000) srush     (1000)        1 2023-03-18 14:29:59.000000 minichain-0.2.2/minichain/prompts/__init__.py
--rw-rw-r--   0 srush     (1000) srush     (1000)      510 2023-03-18 15:59:30.000000 minichain-0.2.2/minichain/prompts/search.py
--rw-rw-r--   0 srush     (1000) srush     (1000)     1370 2023-03-18 15:58:48.000000 minichain-0.2.2/minichain/prompts/template.py
--rw-rw-r--   0 srush     (1000) srush     (1000)     1469 2023-03-18 15:57:47.000000 minichain-0.2.2/minichain/prompts/typed.py
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:46:28.020312 minichain-0.2.2/minichain/templates/
--rw-rw-r--   0 srush     (1000) srush     (1000)        5 2023-02-12 11:12:06.000000 minichain-0.2.2/minichain/templates/anthropic_hhh.tpl
--rw-rw-r--   0 srush     (1000) srush     (1000)      578 2023-02-24 21:33:28.000000 minichain-0.2.2/minichain/templates/prompt.html.tpl
--rw-rw-r--   0 srush     (1000) srush     (1000)       46 2023-02-12 11:15:28.000000 minichain-0.2.2/minichain/templates/self_instruct.tpl
--rw-rw-r--   0 srush     (1000) srush     (1000)      975 2023-03-23 19:57:44.000000 minichain-0.2.2/minichain/templates/type_prompt.pmpt.tpl
-drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:46:28.016312 minichain-0.2.2/minichain.egg-info/
--rw-rw-r--   0 srush     (1000) srush     (1000)     9685 2023-04-13 22:46:28.000000 minichain-0.2.2/minichain.egg-info/PKG-INFO
--rw-rw-r--   0 srush     (1000) srush     (1000)      549 2023-04-13 22:46:28.000000 minichain-0.2.2/minichain.egg-info/SOURCES.txt
--rw-rw-r--   0 srush     (1000) srush     (1000)        1 2023-04-13 22:46:28.000000 minichain-0.2.2/minichain.egg-info/dependency_links.txt
--rw-rw-r--   0 srush     (1000) srush     (1000)      121 2023-04-13 22:46:28.000000 minichain-0.2.2/minichain.egg-info/requires.txt
--rw-rw-r--   0 srush     (1000) srush     (1000)       10 2023-04-13 22:46:28.000000 minichain-0.2.2/minichain.egg-info/top_level.txt
--rw-rw-r--   0 srush     (1000) srush     (1000)      597 2023-04-13 22:46:28.020312 minichain-0.2.2/setup.cfg
--rw-rw-r--   0 srush     (1000) srush     (1000)     1675 2023-04-13 22:07:02.000000 minichain-0.2.2/setup.py
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/MiniChain/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/MiniChain/venv/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/MiniChain/venv/lib/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.192691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.180691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/
+-rw-rw-r--   0 srush     (1000) srush     (1000)      292 2023-04-13 21:57:58.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__init__.py
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.188691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/
+-rw-rw-r--   0 srush     (1000) srush     (1000)      566 2023-04-13 22:54:27.180691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)    12396 2023-04-13 22:54:27.180691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/backend.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     8840 2023-04-13 22:54:27.188691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/base.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     9157 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/gradio.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     3239 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/__pycache__/prompts.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)    10351 2023-04-13 22:01:03.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/backend.py
+-rw-rw-r--   0 srush     (1000) srush     (1000)     9095 2023-04-13 22:29:14.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/base.py
+-rw-rw-r--   0 srush     (1000) srush     (1000)    10430 2023-04-13 22:06:15.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/gradio.py
+-rw-rw-r--   0 srush     (1000) srush     (1000)      701 2023-02-12 12:11:05.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/lang.py
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/
+-rw-rw-r--   0 srush     (1000) srush     (1000)        1 2023-03-18 14:29:59.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__init__.py
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/
+-rw-rw-r--   0 srush     (1000) srush     (1000)      187 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)      998 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/search.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     1662 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/template.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)     2573 2023-04-13 22:54:27.184691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/__pycache__/typed.cpython-310.pyc
+-rw-rw-r--   0 srush     (1000) srush     (1000)      510 2023-03-18 15:59:30.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/search.py
+-rw-rw-r--   0 srush     (1000) srush     (1000)     1370 2023-03-18 15:58:48.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/template.py
+-rw-rw-r--   0 srush     (1000) srush     (1000)     1469 2023-03-18 15:57:47.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/typed.py
+-rw-rw-r--   0 srush     (1000) srush     (1000)     2458 2023-02-27 19:02:03.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts.py
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.176691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/
+-rw-rw-r--   0 srush     (1000) srush     (1000)        5 2023-02-12 11:12:06.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/anthropic_hhh.tpl
+-rw-rw-r--   0 srush     (1000) srush     (1000)      578 2023-02-24 21:33:28.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/prompt.html.tpl
+-rw-rw-r--   0 srush     (1000) srush     (1000)       46 2023-02-12 11:15:28.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/self_instruct.tpl
+-rw-rw-r--   0 srush     (1000) srush     (1000)      975 2023-03-23 19:57:44.000000 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/type_prompt.pmpt.tpl
+drwxrwxr-x   0 srush     (1000) srush     (1000)        0 2023-04-13 22:54:27.192691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/
+-rw-rw-r--   0 srush     (1000) srush     (1000)     9685 2023-04-13 22:54:27.168691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/PKG-INFO
+-rw-rw-r--   0 srush     (1000) srush     (1000)      549 2023-04-13 22:54:27.172691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/SOURCES.txt
+-rw-rw-r--   0 srush     (1000) srush     (1000)        1 2023-04-13 22:54:27.168691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/dependency_links.txt
+-rw-rw-r--   0 srush     (1000) srush     (1000)      113 2023-04-13 22:54:27.168691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/requires.txt
+-rw-rw-r--   0 srush     (1000) srush     (1000)       10 2023-04-13 22:54:27.168691 ./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/top_level.txt
```

### Comparing `minichain-0.2.2/PKG-INFO` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minichain
-Version: 0.2.2
+Version: 0.2.3
 Summary: A tiny library for large language models
 Home-page: https://github.com/srush/minichain
 Author: Sasha Rush
 Author-email: srush.research@gmail.com
 License: MIT
 Project-URL: Documentation, https://srush.github.io/minichain
 Project-URL: Source Code, https://github.com/srush/minichain
```

### Comparing `minichain-0.2.2/minichain/backend.py` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/backend.py`

 * *Files identical despite different names*

### Comparing `minichain-0.2.2/minichain/base.py` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/base.py`

 * *Files identical despite different names*

### Comparing `minichain-0.2.2/minichain/gradio.py` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/gradio.py`

 * *Files identical despite different names*

### Comparing `minichain-0.2.2/minichain/prompts/template.py` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/template.py`

 * *Files identical despite different names*

### Comparing `minichain-0.2.2/minichain/prompts/typed.py` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/prompts/typed.py`

 * *Files identical despite different names*

### Comparing `minichain-0.2.2/minichain/templates/prompt.html.tpl` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/prompt.html.tpl`

 * *Files identical despite different names*

### Comparing `minichain-0.2.2/minichain/templates/type_prompt.pmpt.tpl` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain/templates/type_prompt.pmpt.tpl`

 * *Files identical despite different names*

### Comparing `minichain-0.2.2/minichain.egg-info/SOURCES.txt` & `./home/srush/Projects/MiniChain/venv/lib/python3.10/site-packages/minichain-0.2.3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

