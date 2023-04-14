# Comparing `tmp/basaran-0.15.0.tar.gz` & `tmp/basaran-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basaran-0.15.0.tar", last modified: Fri Apr 14 17:59:49 2023, max compression
+gzip compressed data, was "basaran-0.15.1.tar", last modified: Fri Apr 14 18:25:58 2023, max compression
```

## Comparing `basaran-0.15.0.tar` & `basaran-0.15.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.607919 basaran-0.15.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-14 17:57:06.000000 basaran-0.15.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 17:57:06.000000 basaran-0.15.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 17:59:49.607919 basaran-0.15.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-14 17:57:06.000000 basaran-0.15.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.603919 basaran-0.15.0/basaran/
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.603919 basaran-0.15.0/basaran/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/static/playground.css
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/static/playground.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/static/presets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.603919 basaran-0.15.0/basaran/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/templates/playground.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.603919 basaran-0.15.0/basaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 17:59:49.000000 basaran-0.15.0/basaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-14 17:59:49.000000 basaran-0.15.0/basaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:59:49.000000 basaran-0.15.0/basaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 17:59:49.000000 basaran-0.15.0/basaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 17:59:49.000000 basaran-0.15.0/basaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:59:49.607919 basaran-0.15.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-14 17:57:06.000000 basaran-0.15.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.607919 basaran-0.15.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 17:57:06.000000 basaran-0.15.0/tests/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-14 17:57:06.000000 basaran-0.15.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-14 17:57:06.000000 basaran-0.15.0/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:25:58.819098 basaran-0.15.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-14 18:23:16.000000 basaran-0.15.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 18:23:16.000000 basaran-0.15.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 18:25:58.819098 basaran-0.15.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-14 18:23:16.000000 basaran-0.15.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:25:58.815098 basaran-0.15.1/basaran/
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-14 18:23:16.000000 basaran-0.15.1/basaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-04-14 18:23:16.000000 basaran-0.15.1/basaran/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 18:23:16.000000 basaran-0.15.1/basaran/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-14 18:23:16.000000 basaran-0.15.1/basaran/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:25:58.815098 basaran-0.15.1/basaran/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-14 18:23:16.000000 basaran-0.15.1/basaran/static/playground.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-14 18:23:16.000000 basaran-0.15.1/basaran/static/playground.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-14 18:23:16.000000 basaran-0.15.1/basaran/static/presets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:25:58.815098 basaran-0.15.1/basaran/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-14 18:23:16.000000 basaran-0.15.1/basaran/templates/playground.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 18:23:16.000000 basaran-0.15.1/basaran/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:25:58.815098 basaran-0.15.1/basaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 18:25:58.000000 basaran-0.15.1/basaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-14 18:25:58.000000 basaran-0.15.1/basaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:25:58.000000 basaran-0.15.1/basaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 18:25:58.000000 basaran-0.15.1/basaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 18:25:58.000000 basaran-0.15.1/basaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:25:58.819098 basaran-0.15.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-14 18:23:16.000000 basaran-0.15.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:25:58.815098 basaran-0.15.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 18:23:16.000000 basaran-0.15.1/tests/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-14 18:23:16.000000 basaran-0.15.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-14 18:23:16.000000 basaran-0.15.1/tests/test_tokenizer.py
```

### Comparing `basaran-0.15.0/LICENSE` & `basaran-0.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/PKG-INFO` & `basaran-0.15.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.15.0
+Version: 0.15.1
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.15.0/README.md` & `basaran-0.15.1/README.md`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/basaran/__init__.py` & `basaran-0.15.1/basaran/__init__.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/basaran/__main__.py` & `basaran-0.15.1/basaran/__main__.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/basaran/choice.py` & `basaran-0.15.1/basaran/choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/basaran/model.py` & `basaran-0.15.1/basaran/model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/basaran/static/playground.css` & `basaran-0.15.1/basaran/static/playground.css`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/basaran/static/playground.js` & `basaran-0.15.1/basaran/static/playground.js`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/basaran/static/presets.json` & `basaran-0.15.1/basaran/static/presets.json`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/basaran/templates/playground.html` & `basaran-0.15.1/basaran/templates/playground.html`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/basaran/tokenizer.py` & `basaran-0.15.1/basaran/tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/basaran.egg-info/PKG-INFO` & `basaran-0.15.1/basaran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.15.0
+Version: 0.15.1
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.15.0/setup.py` & `basaran-0.15.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Script for building and distributing Python packages.
 """
 from setuptools import find_packages, setup
 
-VERSION = "0.15.0"
+VERSION = "0.15.1"
 
 setup(
     name="basaran",
     version=VERSION,
     description="Open-source alternative to the OpenAI text completion API",
     long_description="Basaran is an open-source alternative to the OpenAI "
     "text completion API. It provides a compatible streaming API for your "
```

### Comparing `basaran-0.15.0/tests/test_choice.py` & `basaran-0.15.1/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/tests/test_model.py` & `basaran-0.15.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.15.0/tests/test_tokenizer.py` & `basaran-0.15.1/tests/test_tokenizer.py`

 * *Files identical despite different names*

