# Comparing `tmp/furiosa-cli-0.9.0rc2.tar.gz` & `tmp/furiosa-cli-0.9.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-cli-0.9.0rc2.tar", last modified: Fri Apr 14 20:48:27 2023, max compression
+gzip compressed data, was "furiosa-cli-0.9.0rc3.tar", last modified: Fri Apr 14 21:24:58 2023, max compression
```

## Comparing `furiosa-cli-0.9.0rc2.tar` & `furiosa-cli-0.9.0rc3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      353 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/Makefile
--rw-r--r--   0        0        0      166 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/README.md
--rw-r--r--   0        0        0       64 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/furiosa/cli/__init__.py
--rw-r--r--   0        0        0       17 2023-04-14 20:43:41.616683 furiosa-cli-0.9.0rc2/furiosa/cli/git_version.txt
--rw-r--r--   0        0        0     2733 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/furiosa/cli/main.py
--rw-r--r--   0        0        0      450 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/furiosa/cli/utils.py
--rw-r--r--   0        0        0     2326 2023-04-14 20:42:32.537317 furiosa-cli-0.9.0rc2/pyproject.toml
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 furiosa-cli-0.9.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-04-14 21:20:22.712571 furiosa-cli-0.9.0rc3/Makefile
+-rw-r--r--   0        0        0      166 2023-04-14 21:20:22.712571 furiosa-cli-0.9.0rc3/README.md
+-rw-r--r--   0        0        0       64 2023-04-14 21:20:22.712571 furiosa-cli-0.9.0rc3/furiosa/cli/__init__.py
+-rw-r--r--   0        0        0       17 2023-04-14 21:21:30.463956 furiosa-cli-0.9.0rc3/furiosa/cli/git_version.txt
+-rw-r--r--   0        0        0     2733 2023-04-14 21:20:22.712571 furiosa-cli-0.9.0rc3/furiosa/cli/main.py
+-rw-r--r--   0        0        0      450 2023-04-14 21:20:22.712571 furiosa-cli-0.9.0rc3/furiosa/cli/utils.py
+-rw-r--r--   0        0        0     2326 2023-04-14 21:20:22.712571 furiosa-cli-0.9.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 furiosa-cli-0.9.0rc3/PKG-INFO
```

### Comparing `furiosa-cli-0.9.0rc2/furiosa/cli/main.py` & `furiosa-cli-0.9.0rc3/furiosa/cli/main.py`

 * *Files identical despite different names*

### Comparing `furiosa-cli-0.9.0rc2/pyproject.toml` & `furiosa-cli-0.9.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-cli"
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

### Comparing `furiosa-cli-0.9.0rc2/PKG-INFO` & `furiosa-cli-0.9.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-cli
-Version: 0.9.0rc2
+Version: 0.9.0rc3
 Summary: FuriosaAI CLI
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

