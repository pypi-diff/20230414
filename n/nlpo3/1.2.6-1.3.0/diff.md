# Comparing `tmp/nlpo3-1.2.6.tar.gz` & `tmp/nlpo3-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpo3-1.2.6.tar", last modified: Thu Dec  1 09:52:19 2022, max compression
+gzip compressed data, was "nlpo3-1.3.0.tar", last modified: Fri Apr 14 11:50:33 2023, max compression
```

## Comparing `nlpo3-1.2.6.tar` & `nlpo3-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 09:52:19.944696 nlpo3-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (122)      462 2022-12-01 09:52:06.000000 nlpo3-1.2.6/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-12-01 09:52:06.000000 nlpo3-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       85 2022-12-01 09:52:06.000000 nlpo3-1.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4211 2022-12-01 09:52:19.944696 nlpo3-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3062 2022-12-01 09:52:06.000000 nlpo3-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 09:52:19.944696 nlpo3-1.2.6/nlpo3/
--rw-r--r--   0 runner    (1001) docker     (122)     1861 2022-12-01 09:52:06.000000 nlpo3-1.2.6/nlpo3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 09:52:19.944696 nlpo3-1.2.6/nlpo3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4211 2022-12-01 09:52:19.000000 nlpo3-1.2.6/nlpo3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      247 2022-12-01 09:52:19.000000 nlpo3-1.2.6/nlpo3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 09:52:19.000000 nlpo3-1.2.6/nlpo3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 09:52:19.000000 nlpo3-1.2.6/nlpo3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-01 09:52:19.000000 nlpo3-1.2.6/nlpo3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1491 2022-12-01 09:52:06.000000 nlpo3-1.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2022-12-01 09:52:19.956696 nlpo3-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      370 2022-12-01 09:52:06.000000 nlpo3-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 09:52:19.944696 nlpo3-1.2.6/src/
--rw-r--r--   0 runner    (1001) docker     (122)     3613 2022-12-01 09:52:06.000000 nlpo3-1.2.6/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:50:33.487734 nlpo3-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 11:50:19.000000 nlpo3-1.3.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 11:50:19.000000 nlpo3-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 11:50:19.000000 nlpo3-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-14 11:50:33.487734 nlpo3-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-14 11:50:19.000000 nlpo3-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:50:33.487734 nlpo3-1.3.0/nlpo3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 11:50:19.000000 nlpo3-1.3.0/nlpo3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:50:33.487734 nlpo3-1.3.0/nlpo3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-14 11:50:33.000000 nlpo3-1.3.0/nlpo3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 11:50:33.000000 nlpo3-1.3.0/nlpo3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:50:33.000000 nlpo3-1.3.0/nlpo3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:50:33.000000 nlpo3-1.3.0/nlpo3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 11:50:33.000000 nlpo3-1.3.0/nlpo3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-14 11:50:19.000000 nlpo3-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-14 11:50:33.487734 nlpo3-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-14 11:50:19.000000 nlpo3-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:50:33.487734 nlpo3-1.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-14 11:50:19.000000 nlpo3-1.3.0/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:50:33.487734 nlpo3-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-04-14 11:50:19.000000 nlpo3-1.3.0/tests/test_tokenize.py
```

### Comparing `nlpo3-1.2.6/LICENSE` & `nlpo3-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlpo3-1.2.6/PKG-INFO` & `nlpo3-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpo3
-Version: 1.2.6
+Version: 1.3.0
 Summary: Python binding for nlpO3 Thai language processing library in Rust
 Home-page: https://github.com/PyThaiNLP/nlpo3/
 Author: Thanathip Suntorntip, Arthit Suriyawongkul, Wannaphong Phatthiyaphaibun
 Author-email: wannaphong@yahoo.com
 License: Apache-2.0
 Project-URL: homepage, https://github.com/PyThaiNLP/nlpo3/
 Project-URL: repository, https://github.com/PyThaiNLP/nlpo3/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlpo3 Version: 1.2.6 Summary: Python binding for
+Metadata-Version: 2.1 Name: nlpo3 Version: 1.3.0 Summary: Python binding for
 nlpO3 Thai language processing library in Rust Home-page: https://github.com/
 PyThaiNLP/nlpo3/ Author: Thanathip Suntorntip, Arthit Suriyawongkul, Wannaphong
 Phatthiyaphaibun Author-email: wannaphong@yahoo.com License: Apache-2.0
 Project-URL: homepage, https://github.com/PyThaiNLP/nlpo3/ Project-URL:
 repository, https://github.com/PyThaiNLP/nlpo3/ Keywords:
 thai,tokenizer,nlp,word-segmentation,pythainlp Classifier: Development Status
 :: 5 - Production/Stable Classifier: Programming Language :: Python :: 3 ::
```

### Comparing `nlpo3-1.2.6/README.md` & `nlpo3-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nlpo3-1.2.6/nlpo3/__init__.py` & `nlpo3-1.3.0/nlpo3/__init__.py`

 * *Files identical despite different names*

### Comparing `nlpo3-1.2.6/nlpo3.egg-info/PKG-INFO` & `nlpo3-1.3.0/nlpo3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpo3
-Version: 1.2.6
+Version: 1.3.0
 Summary: Python binding for nlpO3 Thai language processing library in Rust
 Home-page: https://github.com/PyThaiNLP/nlpo3/
 Author: Thanathip Suntorntip, Arthit Suriyawongkul, Wannaphong Phatthiyaphaibun
 Author-email: wannaphong@yahoo.com
 License: Apache-2.0
 Project-URL: homepage, https://github.com/PyThaiNLP/nlpo3/
 Project-URL: repository, https://github.com/PyThaiNLP/nlpo3/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlpo3 Version: 1.2.6 Summary: Python binding for
+Metadata-Version: 2.1 Name: nlpo3 Version: 1.3.0 Summary: Python binding for
 nlpO3 Thai language processing library in Rust Home-page: https://github.com/
 PyThaiNLP/nlpo3/ Author: Thanathip Suntorntip, Arthit Suriyawongkul, Wannaphong
 Phatthiyaphaibun Author-email: wannaphong@yahoo.com License: Apache-2.0
 Project-URL: homepage, https://github.com/PyThaiNLP/nlpo3/ Project-URL:
 repository, https://github.com/PyThaiNLP/nlpo3/ Keywords:
 thai,tokenizer,nlp,word-segmentation,pythainlp Classifier: Development Status
 :: 5 - Production/Stable Classifier: Programming Language :: Python :: 3 ::
```

### Comparing `nlpo3-1.2.6/pyproject.toml` & `nlpo3-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-rust", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nlpo3"
-version = "1.2.6"
+version = "1.3.0"
 description = "Python binding for nlpO3 Thai language processing library in Rust"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {text = "Apache-2.0"}
 keywords = ["thai", "tokenizer", "nlp", "word-segmentation", "pythainlp"]
 authors = [
   { name = "Thanathip Suntorntip" },
```

### Comparing `nlpo3-1.2.6/setup.cfg` & `nlpo3-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlpo3-1.2.6/src/lib.rs` & `nlpo3-1.3.0/src/lib.rs`

 * *Files identical despite different names*

