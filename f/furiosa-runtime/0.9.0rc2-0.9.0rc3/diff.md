# Comparing `tmp/furiosa-runtime-0.9.0rc2.tar.gz` & `tmp/furiosa-runtime-0.9.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-runtime-0.9.0rc2.tar", last modified: Fri Apr 14 20:48:45 2023, max compression
+gzip compressed data, was "furiosa-runtime-0.9.0rc3.tar", last modified: Fri Apr 14 21:25:19 2023, max compression
```

## Comparing `furiosa-runtime-0.9.0rc2.tar` & `furiosa-runtime-0.9.0rc3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      340 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/Makefile
--rw-r--r--   0        0        0      193 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/README.md
--rw-r--r--   0        0        0      589 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/__init__.py
--rw-r--r--   0        0        0      104 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/_api/__init__.py
--rw-r--r--   0        0        0     8334 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/_api/v1.py
--rw-r--r--   0        0        0     1344 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/_util.py
--rw-r--r--   0        0        0     1924 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/compiler.py
--rw-r--r--   0        0        0      301 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/consts.py
--rw-r--r--   0        0        0     1696 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/envs.py
--rw-r--r--   0        0        0     7202 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/errors.py
--rw-r--r--   0        0        0       17 2023-04-14 20:43:57.992533 furiosa-runtime-0.9.0rc2/furiosa/runtime/git_version.txt
--rw-r--r--   0        0        0     4904 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/model.py
--rw-r--r--   0        0        0    11619 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/profiler.py
--rw-r--r--   0        0        0        0 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/py.typed
--rw-r--r--   0        0        0    19965 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/session.py
--rw-r--r--   0        0        0    10840 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/tensor.py
--rw-r--r--   0        0        0     2443 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/pyproject.toml
--rw-r--r--   0        0        0      115 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/__init__.py
--rw-r--r--   0        0        0     3296 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_async_session.py
--rw-r--r--   0        0        0     3029 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_base.py
--rw-r--r--   0        0        0      534 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_error.py
--rw-r--r--   0        0        0     1780 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_profiler.py
--rw-r--r--   0        0        0     7713 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_session.py
--rw-r--r--   0        0        0     5486 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_tensor.py
--rw-r--r--   0        0        0      559 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_version.py
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 furiosa-runtime-0.9.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/Makefile
+-rw-r--r--   0        0        0      193 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/README.md
+-rw-r--r--   0        0        0      589 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/__init__.py
+-rw-r--r--   0        0        0      104 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/_api/__init__.py
+-rw-r--r--   0        0        0     8334 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/_api/v1.py
+-rw-r--r--   0        0        0     1344 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/_util.py
+-rw-r--r--   0        0        0     1924 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/compiler.py
+-rw-r--r--   0        0        0      301 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/consts.py
+-rw-r--r--   0        0        0     1696 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/envs.py
+-rw-r--r--   0        0        0     7202 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/errors.py
+-rw-r--r--   0        0        0       17 2023-04-14 21:21:46.631810 furiosa-runtime-0.9.0rc3/furiosa/runtime/git_version.txt
+-rw-r--r--   0        0        0     4904 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/model.py
+-rw-r--r--   0        0        0    11619 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/profiler.py
+-rw-r--r--   0        0        0        0 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/py.typed
+-rw-r--r--   0        0        0    19965 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/session.py
+-rw-r--r--   0        0        0    10840 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/furiosa/runtime/tensor.py
+-rw-r--r--   0        0        0     2443 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/tests/__init__.py
+-rw-r--r--   0        0        0     3296 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/tests/test_async_session.py
+-rw-r--r--   0        0        0     3029 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/tests/test_base.py
+-rw-r--r--   0        0        0      534 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/tests/test_error.py
+-rw-r--r--   0        0        0     1780 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/tests/test_profiler.py
+-rw-r--r--   0        0        0     7713 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/tests/test_session.py
+-rw-r--r--   0        0        0     5486 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/tests/test_tensor.py
+-rw-r--r--   0        0        0      559 2023-04-14 21:20:22.940569 furiosa-runtime-0.9.0rc3/tests/test_version.py
+-rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 furiosa-runtime-0.9.0rc3/PKG-INFO
```

### Comparing `furiosa-runtime-0.9.0rc2/furiosa/runtime/__init__.py` & `furiosa-runtime-0.9.0rc3/furiosa/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/furiosa/runtime/_api/v1.py` & `furiosa-runtime-0.9.0rc3/furiosa/runtime/_api/v1.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/furiosa/runtime/_util.py` & `furiosa-runtime-0.9.0rc3/furiosa/runtime/_util.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/furiosa/runtime/compiler.py` & `furiosa-runtime-0.9.0rc3/furiosa/runtime/compiler.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/furiosa/runtime/envs.py` & `furiosa-runtime-0.9.0rc3/furiosa/runtime/envs.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/furiosa/runtime/errors.py` & `furiosa-runtime-0.9.0rc3/furiosa/runtime/errors.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/furiosa/runtime/model.py` & `furiosa-runtime-0.9.0rc3/furiosa/runtime/model.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/furiosa/runtime/profiler.py` & `furiosa-runtime-0.9.0rc3/furiosa/runtime/profiler.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/furiosa/runtime/session.py` & `furiosa-runtime-0.9.0rc3/furiosa/runtime/session.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/furiosa/runtime/tensor.py` & `furiosa-runtime-0.9.0rc3/furiosa/runtime/tensor.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/pyproject.toml` & `furiosa-runtime-0.9.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-runtime"
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

### Comparing `furiosa-runtime-0.9.0rc2/tests/test_async_session.py` & `furiosa-runtime-0.9.0rc3/tests/test_async_session.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/tests/test_base.py` & `furiosa-runtime-0.9.0rc3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/tests/test_error.py` & `furiosa-runtime-0.9.0rc3/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/tests/test_profiler.py` & `furiosa-runtime-0.9.0rc3/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/tests/test_session.py` & `furiosa-runtime-0.9.0rc3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/tests/test_tensor.py` & `furiosa-runtime-0.9.0rc3/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/tests/test_version.py` & `furiosa-runtime-0.9.0rc3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.9.0rc2/PKG-INFO` & `furiosa-runtime-0.9.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furiosa-runtime
-Version: 0.9.0rc2
+Version: 0.9.0rc3
 Summary: Provide high-level Python APIs to access Furiosa AI's NPUs and its eco-system
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

