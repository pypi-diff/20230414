# Comparing `tmp/furiosa-litmus-0.9.0rc2.tar.gz` & `tmp/furiosa-litmus-0.9.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-litmus-0.9.0rc2.tar", last modified: Fri Apr 14 20:49:14 2023, max compression
+gzip compressed data, was "furiosa-litmus-0.9.0rc3.tar", last modified: Fri Apr 14 21:25:44 2023, max compression
```

## Comparing `furiosa-litmus-0.9.0rc2.tar` & `furiosa-litmus-0.9.0rc3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      353 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/Makefile
--rw-r--r--   0        0        0      224 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/README.md
--rw-r--r--   0        0        0     7304 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/furiosa/litmus/__init__.py
--rw-r--r--   0        0        0       17 2023-04-14 20:44:26.712272 furiosa-litmus-0.9.0rc2/furiosa/litmus/git_version.txt
--rw-r--r--   0        0        0     2418 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/tests/__init__.py
--rw-r--r--   0        0        0      878 2023-04-14 20:42:32.537317 furiosa-litmus-0.9.0rc2/tests/test_litmus.py
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 furiosa-litmus-0.9.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/Makefile
+-rw-r--r--   0        0        0      224 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/README.md
+-rw-r--r--   0        0        0     7304 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/furiosa/litmus/__init__.py
+-rw-r--r--   0        0        0       17 2023-04-14 21:22:15.679548 furiosa-litmus-0.9.0rc3/furiosa/litmus/git_version.txt
+-rw-r--r--   0        0        0     2418 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/tests/__init__.py
+-rw-r--r--   0        0        0      878 2023-04-14 21:20:22.712571 furiosa-litmus-0.9.0rc3/tests/test_litmus.py
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 furiosa-litmus-0.9.0rc3/PKG-INFO
```

### Comparing `furiosa-litmus-0.9.0rc2/furiosa/litmus/__init__.py` & `furiosa-litmus-0.9.0rc3/furiosa/litmus/__init__.py`

 * *Files identical despite different names*

### Comparing `furiosa-litmus-0.9.0rc2/pyproject.toml` & `furiosa-litmus-0.9.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-litmus"
-version = "0.9.0.rc2"
+version = "0.9.0.rc3"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
```

### Comparing `furiosa-litmus-0.9.0rc2/tests/test_litmus.py` & `furiosa-litmus-0.9.0rc3/tests/test_litmus.py`

 * *Files identical despite different names*

### Comparing `furiosa-litmus-0.9.0rc2/PKG-INFO` & `furiosa-litmus-0.9.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-litmus
-Version: 0.9.0rc2
+Version: 0.9.0rc3
 Summary: Furiosa Litmus, which readily checks whether a given model can be compiled with Furiosa SDK
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

