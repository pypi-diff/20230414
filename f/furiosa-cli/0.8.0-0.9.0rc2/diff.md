# Comparing `tmp/furiosa-cli-0.8.0.tar.gz` & `tmp/furiosa-cli-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-cli-0.8.0.tar", last modified: Sat Nov  5 00:13:47 2022, max compression
+gzip compressed data, was "furiosa-cli-0.9.0rc2.tar", last modified: Fri Apr 14 20:48:27 2023, max compression
```

## Comparing `furiosa-cli-0.8.0.tar` & `furiosa-cli-0.9.0rc2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      353 2022-11-05 00:10:11.982210 furiosa-cli-0.8.0/Makefile
--rw-r--r--   0        0        0      166 2022-11-05 00:10:11.982210 furiosa-cli-0.8.0/README.md
--rw-r--r--   0        0        0       64 2022-11-05 00:10:11.982210 furiosa-cli-0.8.0/furiosa/cli/__init__.py
--rw-r--r--   0        0        0       14 2022-11-05 00:11:15.534314 furiosa-cli-0.8.0/furiosa/cli/git_version.txt
--rw-r--r--   0        0        0     2733 2022-11-05 00:10:11.982210 furiosa-cli-0.8.0/furiosa/cli/main.py
--rw-r--r--   0        0        0      450 2022-11-05 00:10:11.982210 furiosa-cli-0.8.0/furiosa/cli/utils.py
--rw-r--r--   0        0        0     2320 2022-11-05 00:10:11.982210 furiosa-cli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 furiosa-cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/Makefile
+-rw-r--r--   0        0        0      166 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/README.md
+-rw-r--r--   0        0        0       64 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/furiosa/cli/__init__.py
+-rw-r--r--   0        0        0       17 2023-04-14 20:43:41.616683 furiosa-cli-0.9.0rc2/furiosa/cli/git_version.txt
+-rw-r--r--   0        0        0     2733 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/furiosa/cli/main.py
+-rw-r--r--   0        0        0      450 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/furiosa/cli/utils.py
+-rw-r--r--   0        0        0     2326 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 furiosa-cli-0.9.0rc2/PKG-INFO
```

### Comparing `furiosa-cli-0.8.0/furiosa/cli/main.py` & `furiosa-cli-0.9.0rc2/furiosa/cli/main.py`

 * *Files identical despite different names*

### Comparing `furiosa-cli-0.8.0/pyproject.toml` & `furiosa-cli-0.9.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-cli"
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
-dependencies = ["furiosa-common == 0.8.*"]
+requires-python = "~=3.8"
+dependencies = ["furiosa-common == 0.9.*"]
 
 [project.scripts]
 furiosa = "furiosa.cli.main:main"
 
 [project.optional-dependencies]
 test = []
 
@@ -41,15 +41,15 @@
 
 [tool.flit.module]
 name = "furiosa.cli"
 
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

### Comparing `furiosa-cli-0.8.0/PKG-INFO` & `furiosa-cli-0.9.0rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: furiosa-cli
-Version: 0.8.0
+Version: 0.9.0rc2
 Summary: FuriosaAI CLI
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
-Requires-Dist: furiosa-common == 0.8.*
+Requires-Dist: furiosa-common == 0.9.*
 Project-URL: Bug Tracker, https://github.com/furiosa-ai/furiosa-sdk/issues
 Project-URL: Documentation, https://furiosa-ai.github.io/docs
 Project-URL: Home, https://furiosa.ai
 Project-URL: Source Code, https://github.com/furiosa-ai/furiosa-sdk
 Provides-Extra: test
 
 # Package `furiosa.cli`
```

