# Comparing `tmp/cbstorage-0.1.0.tar.gz` & `tmp/cbstorage-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbstorage-0.1.0.tar", max compression
+gzip compressed data, was "cbstorage-0.1.2.tar", max compression
```

## Comparing `cbstorage-0.1.0.tar` & `cbstorage-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       22 2023-04-14 13:09:33.104854 cbstorage-0.1.0/cbstorage/__init__.py
--rw-r--r--   0        0        0     7498 2023-04-14 13:20:46.801175 cbstorage-0.1.0/cbstorage/storage.py
--rw-r--r--   0        0        0      305 2023-04-14 13:20:24.684610 cbstorage-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      502 2023-04-14 13:21:01.339212 cbstorage-0.1.0/setup.py
--rw-r--r--   0        0        0      249 2023-04-14 13:21:01.339333 cbstorage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-14 13:09:33.104854 cbstorage-0.1.2/cbstorage/__init__.py
+-rw-r--r--   0        0        0     7498 2023-04-14 13:20:46.801175 cbstorage-0.1.2/cbstorage/storage.py
+-rw-r--r--   0        0        0      320 2023-04-14 13:31:50.382581 cbstorage-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-04-14 13:31:52.689584 cbstorage-0.1.2/setup.py
+-rw-r--r--   0        0        0      398 2023-04-14 13:31:52.689701 cbstorage-0.1.2/PKG-INFO
```

### Comparing `cbstorage-0.1.0/cbstorage/storage.py` & `cbstorage-0.1.2/cbstorage/storage.py`

 * *Files identical despite different names*

