# Comparing `tmp/furiosa-litmus-0.8.0.tar.gz` & `tmp/furiosa-litmus-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-litmus-0.8.0.tar", last modified: Sat Nov  5 00:14:21 2022, max compression
+gzip compressed data, was "furiosa-litmus-0.9.0rc2.tar", last modified: Fri Apr 14 20:49:14 2023, max compression
```

## Comparing `furiosa-litmus-0.8.0.tar` & `furiosa-litmus-0.9.0rc2.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0      354 2022-11-05 00:10:11.982210 furiosa-litmus-0.8.0/Makefile
--rw-r--r--   0        0        0      224 2022-11-05 00:10:11.982210 furiosa-litmus-0.8.0/README.md
--rw-r--r--   0        0        0     3095 2022-11-05 00:10:11.982210 furiosa-litmus-0.8.0/furiosa/litmus/__init__.py
--rw-r--r--   0        0        0       14 2022-11-05 00:12:09.306405 furiosa-litmus-0.8.0/furiosa/litmus/git_version.txt
--rw-r--r--   0        0        0     2371 2022-11-05 00:10:11.982210 furiosa-litmus-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 furiosa-litmus-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/Makefile
+-rw-r--r--   0        0        0      224 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/README.md
+-rw-r--r--   0        0        0     7304 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/furiosa/litmus/__init__.py
+-rw-r--r--   0        0        0       17 2023-04-14 20:44:26.712272 furiosa-litmus-0.9.0rc2/furiosa/litmus/git_version.txt
+-rw-r--r--   0        0        0     2418 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0      878 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/tests/test_litmus.py
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 furiosa-litmus-0.9.0rc2/PKG-INFO
```

### Comparing `furiosa-litmus-0.8.0/pyproject.toml` & `furiosa-litmus-0.9.0rc2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,38 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-litmus"
-version = "0.8.0"
+version = "0.9.0.rc2"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dynamic = ["description"]
-requires-python = "~=3.7"
-dependencies = ["furiosa-runtime == 0.8.*", "furiosa-quantizer == 0.8.*"]
+requires-python = "~=3.8"
+dependencies = [
+    "furiosa-runtime == 0.9.*",
+    "furiosa-tools == 0.9.*", 
+    "furiosa-quantizer == 0.9.*"
+]
 
 [project.optional-dependencies]
 test = []
 
 [project.urls]
 Home = "https://furiosa.ai"
 Documentation = "https://furiosa-ai.github.io/docs"
@@ -41,15 +45,15 @@
 
 [project.scripts]
 furiosa-litmus = "furiosa.litmus:main"
 
 [tool.black]
 skip-string-normalization = true
 line-length = 100
-target-version = ["py37", "py38", "py39"]
+target-version = ["py38", "py39", "py310"]
 extend-exclude = "/generated/"
 
 [tool.isort]
 force_sort_within_sections = true
 known_first_party = ["furiosa"]
 line_length = 100
 profile = "black"
```

### Comparing `furiosa-litmus-0.8.0/PKG-INFO` & `furiosa-litmus-0.9.0rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: furiosa-litmus
-Version: 0.8.0
+Version: 0.9.0rc2
 Summary: Furiosa Litmus, which readily checks whether a given model can be compiled with Furiosa SDK
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Dist: furiosa-runtime == 0.8.*
-Requires-Dist: furiosa-quantizer == 0.8.*
+Requires-Dist: furiosa-runtime == 0.9.*
+Requires-Dist: furiosa-tools == 0.9.*
+Requires-Dist: furiosa-quantizer == 0.9.*
 Project-URL: Bug Tracker, https://github.com/furiosa-ai/furiosa-sdk/issues
 Project-URL: Documentation, https://furiosa-ai.github.io/docs
 Project-URL: Home, https://furiosa.ai
 Project-URL: Source Code, https://github.com/furiosa-ai/furiosa-sdk
 Provides-Extra: test
 
 # Package `furiosa.litmus`
```

