# Comparing `tmp/basaran-0.14.1.tar.gz` & `tmp/basaran-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basaran-0.14.1.tar", last modified: Fri Apr  7 16:44:42 2023, max compression
+gzip compressed data, was "basaran-0.15.0.tar", last modified: Fri Apr 14 17:59:49 2023, max compression
```

## Comparing `basaran-0.14.1.tar` & `basaran-0.15.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:44:42.376244 basaran-0.14.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-07 16:42:20.000000 basaran-0.14.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-07 16:42:20.000000 basaran-0.14.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-07 16:44:42.376244 basaran-0.14.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-07 16:42:20.000000 basaran-0.14.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:44:42.372244 basaran-0.14.1/basaran/
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-07 16:42:20.000000 basaran-0.14.1/basaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-04-07 16:42:20.000000 basaran-0.14.1/basaran/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-07 16:42:20.000000 basaran-0.14.1/basaran/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-07 16:42:20.000000 basaran-0.14.1/basaran/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:44:42.376244 basaran-0.14.1/basaran/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-07 16:42:20.000000 basaran-0.14.1/basaran/static/playground.css
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-07 16:42:20.000000 basaran-0.14.1/basaran/static/playground.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-07 16:42:20.000000 basaran-0.14.1/basaran/static/presets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:44:42.376244 basaran-0.14.1/basaran/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-07 16:42:20.000000 basaran-0.14.1/basaran/templates/playground.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-07 16:42:20.000000 basaran-0.14.1/basaran/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:44:42.372244 basaran-0.14.1/basaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-07 16:44:42.000000 basaran-0.14.1/basaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 16:44:42.000000 basaran-0.14.1/basaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 16:44:42.000000 basaran-0.14.1/basaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-07 16:44:42.000000 basaran-0.14.1/basaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-07 16:44:42.000000 basaran-0.14.1/basaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 16:44:42.376244 basaran-0.14.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-07 16:42:20.000000 basaran-0.14.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 16:44:42.376244 basaran-0.14.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-07 16:42:20.000000 basaran-0.14.1/tests/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-07 16:42:20.000000 basaran-0.14.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-07 16:42:20.000000 basaran-0.14.1/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.607919 basaran-0.15.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-14 17:57:06.000000 basaran-0.15.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 17:57:06.000000 basaran-0.15.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 17:59:49.607919 basaran-0.15.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-14 17:57:06.000000 basaran-0.15.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.603919 basaran-0.15.0/basaran/
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.603919 basaran-0.15.0/basaran/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/static/playground.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/static/playground.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/static/presets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.603919 basaran-0.15.0/basaran/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/templates/playground.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 17:57:06.000000 basaran-0.15.0/basaran/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.603919 basaran-0.15.0/basaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 17:59:49.000000 basaran-0.15.0/basaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-14 17:59:49.000000 basaran-0.15.0/basaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:59:49.000000 basaran-0.15.0/basaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 17:59:49.000000 basaran-0.15.0/basaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 17:59:49.000000 basaran-0.15.0/basaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:59:49.607919 basaran-0.15.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-14 17:57:06.000000 basaran-0.15.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:59:49.607919 basaran-0.15.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 17:57:06.000000 basaran-0.15.0/tests/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-14 17:57:06.000000 basaran-0.15.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-14 17:57:06.000000 basaran-0.15.0/tests/test_tokenizer.py
```

### Comparing `basaran-0.14.1/LICENSE` & `basaran-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/PKG-INFO` & `basaran-0.15.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.14.1
+Version: 0.15.0
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.14.1/README.md` & `basaran-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/basaran/__init__.py` & `basaran-0.15.0/basaran/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 MODEL_LOAD_IN_8BIT = is_true(os.getenv("MODEL_LOAD_IN_8BIT", ""))
 MODEL_LOCAL_FILES_ONLY = is_true(os.getenv("MODEL_LOCAL_FILES_ONLY", ""))
 MODEL_TRUST_REMOTE_CODE = is_true(os.getenv("MODEL_TRUST_REMOTE_CODE", ""))
 MODEL_HALF_PRECISION = is_true(os.getenv("MODEL_HALF_PRECISION", ""))
 
 # Server-related arguments:
 # https://docs.pylonsproject.org/projects/waitress/en/stable/arguments.html
-SERVER_THREADS = int(os.getenv("SERVER_THREADS", "8"))
+SERVER_THREADS = int(os.getenv("SERVER_THREADS", "32"))
 SERVER_IDENTITY = os.getenv("SERVER_IDENTITY", "basaran")
 SERVER_CONNECTION_LIMIT = int(os.getenv("SERVER_CONNECTION_LIMIT", "512"))
 SERVER_CHANNEL_TIMEOUT = int(os.getenv("SERVER_CHANNEL_TIMEOUT", "300"))
 SERVER_MODEL_NAME = os.getenv("SERVER_MODEL_NAME", "") or MODEL
 SERVER_NO_PLAYGROUND = is_true(os.getenv("SERVER_NO_PLAYGROUND", ""))
 
 # Completion-related arguments:
```

### Comparing `basaran-0.14.1/basaran/__main__.py` & `basaran-0.15.0/basaran/__main__.py`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/basaran/choice.py` & `basaran-0.15.0/basaran/choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/basaran/model.py` & `basaran-0.15.0/basaran/model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/basaran/static/playground.css` & `basaran-0.15.0/basaran/static/playground.css`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/basaran/static/playground.js` & `basaran-0.15.0/basaran/static/playground.js`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/basaran/static/presets.json` & `basaran-0.15.0/basaran/static/presets.json`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/basaran/templates/playground.html` & `basaran-0.15.0/basaran/templates/playground.html`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/basaran/tokenizer.py` & `basaran-0.15.0/basaran/tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/basaran.egg-info/PKG-INFO` & `basaran-0.15.0/basaran.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.14.1
+Version: 0.15.0
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.14.1/setup.py` & `basaran-0.15.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Script for building and distributing Python packages.
 """
 from setuptools import find_packages, setup
 
-VERSION = "0.14.1"
+VERSION = "0.15.0"
 
 setup(
     name="basaran",
     version=VERSION,
     description="Open-source alternative to the OpenAI text completion API",
     long_description="Basaran is an open-source alternative to the OpenAI "
     "text completion API. It provides a compatible streaming API for your "
     "Hugging Face Transformers-based text generation models.",
     author="Hyperonym",
     author_email="prompt@hyperonym.org",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.8.0",
-    install_requires=["flask", "torch", "transformers", "waitress"],
+    install_requires=["flask", "jinja2", "torch", "transformers", "waitress"],
     keywords=["api", "huggingface", "nlp", "openai", "transformer"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
```

### Comparing `basaran-0.14.1/tests/test_choice.py` & `basaran-0.15.0/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.14.1/tests/test_model.py` & `basaran-0.15.0/tests/test_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -77,7 +77,21 @@
         model = load_model("./tests/data/tiny-random-t5")
         self.assert_stochastic(model)
 
     def test_deterministic(self):
         """Test completion using deterministic decoding."""
         model = load_model("./tests/data/tiny-random-t5")
         self.assert_deterministic(model)
+
+
+class TestLlamaModel(TestModel):
+    """Test text generation using LLaMA models."""
+
+    def test_stochastic(self):
+        """Test completion using stochastic decoding."""
+        model = load_model("./tests/data/tiny-random-llama")
+        self.assert_stochastic(model)
+
+    def test_deterministic(self):
+        """Test completion using deterministic decoding."""
+        model = load_model("./tests/data/tiny-random-llama")
+        self.assert_deterministic(model)
```

### Comparing `basaran-0.14.1/tests/test_tokenizer.py` & `basaran-0.15.0/tests/test_tokenizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,7 +40,25 @@
 
         actual = ""
         for token in tokens:
             actual += detokenizer.decode(token)
 
         assert actual == expected
         assert detokenizer.end == len(expected)
+
+    def test_llama_tokenizer(self):
+        """Test with LLaMA tokenizer."""
+        tokenizer = AutoTokenizer.from_pretrained(
+            pretrained_model_name_or_path="./tests/data/tiny-random-llama",
+            local_files_only=True,
+        )
+        detokenizer = StreamTokenizer(tokenizer)
+
+        expected = "hello world ABC \n 你好"
+        tokens = tokenizer.encode(expected)
+
+        actual = ""
+        for token in tokens:
+            actual += detokenizer.decode(token)
+
+        assert actual == expected
+        assert detokenizer.end == len(expected)
```

