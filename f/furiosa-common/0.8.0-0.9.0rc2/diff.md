# Comparing `tmp/furiosa-common-0.8.0.tar.gz` & `tmp/furiosa-common-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-common-0.8.0.tar", last modified: Sat Nov  5 00:13:42 2022, max compression
+gzip compressed data, was "furiosa-common-0.9.0rc2.tar", last modified: Fri Apr 14 20:48:21 2023, max compression
```

## Comparing `furiosa-common-0.8.0.tar` & `furiosa-common-0.9.0rc2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      353 2022-11-05 00:10:11.982210 furiosa-common-0.8.0/Makefile
--rw-r--r--   0        0        0      144 2022-11-05 00:10:11.982210 furiosa-common-0.8.0/README.md
--rw-r--r--   0        0        0      142 2022-11-05 00:10:11.982210 furiosa-common-0.8.0/furiosa/common/__init__.py
--rw-r--r--   0        0        0      523 2022-11-05 00:10:11.982210 furiosa-common-0.8.0/furiosa/common/error.py
--rw-r--r--   0        0        0       14 2022-11-05 00:11:10.950306 furiosa-common-0.8.0/furiosa/common/git_version.txt
--rw-r--r--   0        0        0     3184 2022-11-05 00:10:11.982210 furiosa-common-0.8.0/furiosa/common/native.py
--rw-r--r--   0        0        0     1552 2022-11-05 00:10:11.982210 furiosa-common-0.8.0/furiosa/common/thread.py
--rw-r--r--   0        0        0     1110 2022-11-05 00:10:11.982210 furiosa-common-0.8.0/furiosa/common/utils.py
--rw-r--r--   0        0        0     2295 2022-11-05 00:10:11.982210 furiosa-common-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1224 1970-01-01 00:00:00.000000 furiosa-common-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-04-14 20:42:32.537317 furiosa-common-0.9.0rc2/Makefile
+-rw-r--r--   0        0        0      144 2023-04-14 20:42:32.537317 furiosa-common-0.9.0rc2/README.md
+-rw-r--r--   0        0        0      142 2023-04-14 20:42:32.537317 furiosa-common-0.9.0rc2/furiosa/common/__init__.py
+-rw-r--r--   0        0        0      523 2023-04-14 20:42:32.537317 furiosa-common-0.9.0rc2/furiosa/common/error.py
+-rw-r--r--   0        0        0       17 2023-04-14 20:43:38.072716 furiosa-common-0.9.0rc2/furiosa/common/git_version.txt
+-rw-r--r--   0        0        0     3184 2023-04-14 20:42:32.537317 furiosa-common-0.9.0rc2/furiosa/common/native.py
+-rw-r--r--   0        0        0     1552 2023-04-14 20:42:32.537317 furiosa-common-0.9.0rc2/furiosa/common/thread.py
+-rw-r--r--   0        0        0     1110 2023-04-14 20:42:32.537317 furiosa-common-0.9.0rc2/furiosa/common/utils.py
+-rw-r--r--   0        0        0     2301 2023-04-14 20:42:32.537317 furiosa-common-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 furiosa-common-0.9.0rc2/PKG-INFO
```

### Comparing `furiosa-common-0.8.0/furiosa/common/error.py` & `furiosa-common-0.9.0rc2/furiosa/common/error.py`

 * *Files identical despite different names*

### Comparing `furiosa-common-0.8.0/furiosa/common/native.py` & `furiosa-common-0.9.0rc2/furiosa/common/native.py`

 * *Files identical despite different names*

### Comparing `furiosa-common-0.8.0/furiosa/common/thread.py` & `furiosa-common-0.9.0rc2/furiosa/common/thread.py`

 * *Files identical despite different names*

### Comparing `furiosa-common-0.8.0/furiosa/common/utils.py` & `furiosa-common-0.9.0rc2/furiosa/common/utils.py`

 * *Files identical despite different names*

### Comparing `furiosa-common-0.8.0/pyproject.toml` & `furiosa-common-0.9.0rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-common"
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
+requires-python = "~=3.8"
 dependencies = ["packaging"]
 
 [project.optional-dependencies]
 test = []
 
 [project.urls]
 Home = "https://furiosa.ai"
@@ -38,15 +38,15 @@
 
 [tool.flit.module]
 name = "furiosa.common"
 
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

### Comparing `furiosa-common-0.8.0/PKG-INFO` & `furiosa-common-0.9.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: furiosa-common
-Version: 0.8.0
+Version: 0.9.0rc2
 Summary: Furiosa SDK common utilities
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
 Requires-Dist: packaging
 Project-URL: Bug Tracker, https://github.com/furiosa-ai/furiosa-sdk/issues
 Project-URL: Documentation, https://furiosa-ai.github.io/docs
 Project-URL: Home, https://furiosa.ai
 Project-URL: Source Code, https://github.com/furiosa-ai/furiosa-sdk
```

