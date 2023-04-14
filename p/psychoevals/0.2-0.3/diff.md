# Comparing `tmp/psychoevals-0.2.tar.gz` & `tmp/psychoevals-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoevals-0.2.tar", last modified: Fri Apr 14 21:44:43 2023, max compression
+gzip compressed data, was "psychoevals-0.3.tar", last modified: Fri Apr 14 21:55:52 2023, max compression
```

## Comparing `psychoevals-0.2.tar` & `psychoevals-0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:44:43.107036 psychoevals-0.2/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 21:44:43.107036 psychoevals-0.2/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6066 2023-04-14 21:19:33.000000 psychoevals-0.2/README.md
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:44:43.107036 psychoevals-0.2/psychoevals/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.2/psychoevals/__init__.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:44:43.107036 psychoevals-0.2/psychoevals/agents/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       50 2023-04-13 22:53:06.000000 psychoevals-0.2/psychoevals/agents/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      202 2023-04-12 23:17:23.000000 psychoevals-0.2/psychoevals/agents/base_eval_agent.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.2/psychoevals/cognitive_state.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      442 2023-04-13 22:56:20.000000 psychoevals-0.2/psychoevals/evaluation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1763 2023-04-13 23:33:32.000000 psychoevals-0.2/psychoevals/moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.2/psychoevals/qna_result.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     4127 2023-04-13 23:33:58.000000 psychoevals-0.2/psychoevals/security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3929 2023-04-13 23:32:44.000000 psychoevals-0.2/psychoevals/utils.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:44:43.107036 psychoevals-0.2/psychoevals.egg-info/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 21:44:43.000000 psychoevals-0.2/psychoevals.egg-info/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      550 2023-04-14 21:44:43.000000 psychoevals-0.2/psychoevals.egg-info/SOURCES.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-14 21:44:43.000000 psychoevals-0.2/psychoevals.egg-info/dependency_links.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-14 21:44:43.000000 psychoevals-0.2/psychoevals.egg-info/requires.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-14 21:44:43.000000 psychoevals-0.2/psychoevals.egg-info/top_level.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-14 21:44:43.107036 psychoevals-0.2/setup.cfg
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-14 21:43:30.000000 psychoevals-0.2/setup.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:44:43.107036 psychoevals-0.2/tests/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.2/tests/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3039 2023-04-14 20:33:13.000000 psychoevals-0.2/tests/test_mbti.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1852 2023-04-14 20:16:12.000000 psychoevals-0.2/tests/test_moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1424 2023-04-14 20:16:27.000000 psychoevals-0.2/tests/test_security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      893 2023-04-14 20:16:18.000000 psychoevals-0.2/tests/test_troll_agent.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:55:52.007039 psychoevals-0.3/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 21:55:52.007039 psychoevals-0.3/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6066 2023-04-14 21:19:33.000000 psychoevals-0.3/README.md
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:55:51.997039 psychoevals-0.3/psychoevals/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.3/psychoevals/__init__.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:55:51.997039 psychoevals-0.3/psychoevals/agents/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       50 2023-04-13 22:53:06.000000 psychoevals-0.3/psychoevals/agents/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      202 2023-04-12 23:17:23.000000 psychoevals-0.3/psychoevals/agents/base_eval_agent.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.3/psychoevals/cognitive_state.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      442 2023-04-13 22:56:20.000000 psychoevals-0.3/psychoevals/evaluation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1716 2023-04-14 21:54:45.000000 psychoevals-0.3/psychoevals/moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.3/psychoevals/qna_result.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     4127 2023-04-13 23:33:58.000000 psychoevals-0.3/psychoevals/security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3882 2023-04-14 21:54:37.000000 psychoevals-0.3/psychoevals/utils.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:55:51.997039 psychoevals-0.3/psychoevals.egg-info/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 21:55:51.000000 psychoevals-0.3/psychoevals.egg-info/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      550 2023-04-14 21:55:51.000000 psychoevals-0.3/psychoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-14 21:55:51.000000 psychoevals-0.3/psychoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-14 21:55:51.000000 psychoevals-0.3/psychoevals.egg-info/requires.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-14 21:55:51.000000 psychoevals-0.3/psychoevals.egg-info/top_level.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-14 21:55:52.007039 psychoevals-0.3/setup.cfg
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-14 21:55:39.000000 psychoevals-0.3/setup.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:55:52.007039 psychoevals-0.3/tests/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.3/tests/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3039 2023-04-14 20:33:13.000000 psychoevals-0.3/tests/test_mbti.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1852 2023-04-14 20:16:12.000000 psychoevals-0.3/tests/test_moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1424 2023-04-14 20:16:27.000000 psychoevals-0.3/tests/test_security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      893 2023-04-14 20:16:18.000000 psychoevals-0.3/tests/test_troll_agent.py
```

### Comparing `psychoevals-0.2/README.md` & `psychoevals-0.3/README.md`

 * *Files identical despite different names*

### Comparing `psychoevals-0.2/psychoevals/moderation.py` & `psychoevals-0.3/psychoevals/moderation.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from functools import wraps
 from logging import getLogger
 logging = getLogger(__name__)
 import os 
 import openai
 from dotenv import load_dotenv, find_dotenv
 dotenv_path = find_dotenv()
+
 if dotenv_path:
     load_dotenv(dotenv_path)
-else:
-    raise Exception("No .env file found")
 
 openai.api_key = os.environ["OPENAI_API_KEY"] 
 
 @retry(wait=wait_random(min=1, max=2), stop=stop_after_attempt(2))
 def get_moderation_result(text_sequence):
     result = openai.Moderation.create(
         input=text_sequence,
```

### Comparing `psychoevals-0.2/psychoevals/security.py` & `psychoevals-0.3/psychoevals/security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.2/psychoevals/utils.py` & `psychoevals-0.3/psychoevals/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from logging import getLogger
 logging = getLogger(__name__)
 import os 
 import openai
 import json 
 from dotenv import load_dotenv, find_dotenv
 dotenv_path = find_dotenv()
+
 if dotenv_path:
     load_dotenv(dotenv_path)
-else:
-    raise Exception("No .env file found")
 
 openai.api_key = os.environ["OPENAI_API_KEY"]
 
 @retry(wait=wait_random(min=1, max=2), stop=stop_after_attempt(2))
 def get_moderation_result(text_sequence):
     result = openai.Moderation.create(
         input=text_sequence,
```

### Comparing `psychoevals-0.2/psychoevals.egg-info/SOURCES.txt` & `psychoevals-0.3/psychoevals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psychoevals-0.2/setup.py` & `psychoevals-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='psychoevals',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         "openai>=0.27.0",
         "pandas>=1.3.0",
         "tenacity>=8.0.0",
         "python-dotenv>=0.15.0"
     ],
```

### Comparing `psychoevals-0.2/tests/test_mbti.py` & `psychoevals-0.3/tests/test_mbti.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.2/tests/test_moderation.py` & `psychoevals-0.3/tests/test_moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.2/tests/test_security.py` & `psychoevals-0.3/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.2/tests/test_troll_agent.py` & `psychoevals-0.3/tests/test_troll_agent.py`

 * *Files identical despite different names*

