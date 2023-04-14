# Comparing `tmp/psychoevals-0.1.tar.gz` & `tmp/psychoevals-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoevals-0.1.tar", last modified: Fri Apr 14 21:36:02 2023, max compression
+gzip compressed data, was "psychoevals-0.2.tar", last modified: Fri Apr 14 21:44:43 2023, max compression
```

## Comparing `psychoevals-0.1.tar` & `psychoevals-0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:36:02.887040 psychoevals-0.1/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 21:36:02.887040 psychoevals-0.1/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6066 2023-04-14 21:19:33.000000 psychoevals-0.1/README.md
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:36:02.887040 psychoevals-0.1/psychoevals/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.1/psychoevals/__init__.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:36:02.887040 psychoevals-0.1/psychoevals/agents/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       50 2023-04-13 22:53:06.000000 psychoevals-0.1/psychoevals/agents/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      202 2023-04-12 23:17:23.000000 psychoevals-0.1/psychoevals/agents/base_eval_agent.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.1/psychoevals/cognitive_state.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      442 2023-04-13 22:56:20.000000 psychoevals-0.1/psychoevals/evaluation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1763 2023-04-13 23:33:32.000000 psychoevals-0.1/psychoevals/moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.1/psychoevals/qna_result.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     4127 2023-04-13 23:33:58.000000 psychoevals-0.1/psychoevals/security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3929 2023-04-13 23:32:44.000000 psychoevals-0.1/psychoevals/utils.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:36:02.887040 psychoevals-0.1/psychoevals.egg-info/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 21:36:02.000000 psychoevals-0.1/psychoevals.egg-info/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      550 2023-04-14 21:36:02.000000 psychoevals-0.1/psychoevals.egg-info/SOURCES.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-14 21:36:02.000000 psychoevals-0.1/psychoevals.egg-info/dependency_links.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       29 2023-04-14 21:36:02.000000 psychoevals-0.1/psychoevals.egg-info/requires.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-14 21:36:02.000000 psychoevals-0.1/psychoevals.egg-info/top_level.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-14 21:36:02.887040 psychoevals-0.1/setup.cfg
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      520 2023-04-14 20:18:51.000000 psychoevals-0.1/setup.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:36:02.887040 psychoevals-0.1/tests/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.1/tests/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3039 2023-04-14 20:33:13.000000 psychoevals-0.1/tests/test_mbti.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1852 2023-04-14 20:16:12.000000 psychoevals-0.1/tests/test_moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1424 2023-04-14 20:16:27.000000 psychoevals-0.1/tests/test_security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      893 2023-04-14 20:16:18.000000 psychoevals-0.1/tests/test_troll_agent.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:44:43.107036 psychoevals-0.2/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 21:44:43.107036 psychoevals-0.2/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6066 2023-04-14 21:19:33.000000 psychoevals-0.2/README.md
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:44:43.107036 psychoevals-0.2/psychoevals/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.2/psychoevals/__init__.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:44:43.107036 psychoevals-0.2/psychoevals/agents/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       50 2023-04-13 22:53:06.000000 psychoevals-0.2/psychoevals/agents/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      202 2023-04-12 23:17:23.000000 psychoevals-0.2/psychoevals/agents/base_eval_agent.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.2/psychoevals/cognitive_state.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      442 2023-04-13 22:56:20.000000 psychoevals-0.2/psychoevals/evaluation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1763 2023-04-13 23:33:32.000000 psychoevals-0.2/psychoevals/moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.2/psychoevals/qna_result.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     4127 2023-04-13 23:33:58.000000 psychoevals-0.2/psychoevals/security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3929 2023-04-13 23:32:44.000000 psychoevals-0.2/psychoevals/utils.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:44:43.107036 psychoevals-0.2/psychoevals.egg-info/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 21:44:43.000000 psychoevals-0.2/psychoevals.egg-info/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      550 2023-04-14 21:44:43.000000 psychoevals-0.2/psychoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-14 21:44:43.000000 psychoevals-0.2/psychoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-14 21:44:43.000000 psychoevals-0.2/psychoevals.egg-info/requires.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-14 21:44:43.000000 psychoevals-0.2/psychoevals.egg-info/top_level.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-14 21:44:43.107036 psychoevals-0.2/setup.cfg
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-14 21:43:30.000000 psychoevals-0.2/setup.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:44:43.107036 psychoevals-0.2/tests/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.2/tests/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3039 2023-04-14 20:33:13.000000 psychoevals-0.2/tests/test_mbti.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1852 2023-04-14 20:16:12.000000 psychoevals-0.2/tests/test_moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1424 2023-04-14 20:16:27.000000 psychoevals-0.2/tests/test_security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      893 2023-04-14 20:16:18.000000 psychoevals-0.2/tests/test_troll_agent.py
```

### Comparing `psychoevals-0.1/README.md` & `psychoevals-0.2/README.md`

 * *Files identical despite different names*

### Comparing `psychoevals-0.1/psychoevals/moderation.py` & `psychoevals-0.2/psychoevals/moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.1/psychoevals/security.py` & `psychoevals-0.2/psychoevals/security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.1/psychoevals/utils.py` & `psychoevals-0.2/psychoevals/utils.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.1/psychoevals.egg-info/SOURCES.txt` & `psychoevals-0.2/psychoevals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psychoevals-0.1/setup.py` & `psychoevals-0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='psychoevals',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         "openai>=0.27.0",
         "pandas>=1.3.0",
+        "tenacity>=8.0.0",
+        "python-dotenv>=0.15.0"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
     ],
```

### Comparing `psychoevals-0.1/tests/test_mbti.py` & `psychoevals-0.2/tests/test_mbti.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.1/tests/test_moderation.py` & `psychoevals-0.2/tests/test_moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.1/tests/test_security.py` & `psychoevals-0.2/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.1/tests/test_troll_agent.py` & `psychoevals-0.2/tests/test_troll_agent.py`

 * *Files identical despite different names*

