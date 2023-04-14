# Comparing `tmp/pycodeless-0.1.0.tar.gz` & `tmp/pycodeless-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycodeless-0.1.0.tar", max compression
+gzip compressed data, was "pycodeless-0.2.0.tar", max compression
```

## Comparing `pycodeless-0.1.0.tar` & `pycodeless-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.1.0/LICENSE
--rw-r--r--   0        0        0       64 2023-04-13 15:57:26.646535 pycodeless-0.1.0/pycodeless/__init__.py
--rw-r--r--   0        0        0      111 2023-04-13 15:57:18.930678 pycodeless-0.1.0/pycodeless/_api.py
--rw-r--r--   0        0        0      392 2023-04-13 15:55:34.783540 pycodeless-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       79 2023-04-13 15:47:38.373419 pycodeless-0.1.0/README.md
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 pycodeless-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-13 15:47:38.372155 pycodeless-0.2.0/LICENSE
+-rw-r--r--   0        0        0       62 2023-04-13 19:57:45.936649 pycodeless-0.2.0/pycodeless/__init__.py
+-rw-r--r--   0        0        0      665 2023-04-13 22:50:33.299322 pycodeless-0.2.0/pycodeless/_api.py
+-rw-r--r--   0        0        0     5142 2023-04-14 11:57:05.819090 pycodeless-0.2.0/pycodeless/_generate.py
+-rw-r--r--   0        0        0      920 2023-04-13 17:21:52.520835 pycodeless-0.2.0/pycodeless/_llm.py
+-rw-r--r--   0        0        0      436 2023-04-13 22:40:30.195789 pycodeless-0.2.0/pycodeless/_load.py
+-rw-r--r--   0        0        0      970 2023-04-14 10:54:07.150342 pycodeless-0.2.0/pycodeless/_openai_llm.py
+-rw-r--r--   0        0        0     4491 2023-04-14 11:38:36.064128 pycodeless-0.2.0/pycodeless/_parse.py
+-rw-r--r--   0        0        0      392 2023-04-14 12:49:31.166866 pycodeless-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-04-13 15:47:38.373419 pycodeless-0.2.0/README.md
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 pycodeless-0.2.0/PKG-INFO
```

### Comparing `pycodeless-0.1.0/LICENSE` & `pycodeless-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycodeless-0.1.0/PKG-INFO` & `pycodeless-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycodeless
-Version: 0.1.0
+Version: 0.2.0
 Summary: Build Python code using natural language as a universal interface
 License: MIT
 Author: hacksparr0w
 Author-email: hacksparr0w@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

