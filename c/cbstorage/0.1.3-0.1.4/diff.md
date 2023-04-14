# Comparing `tmp/cbstorage-0.1.3.tar.gz` & `tmp/cbstorage-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbstorage-0.1.3.tar", max compression
+gzip compressed data, was "cbstorage-0.1.4.tar", max compression
```

## Comparing `cbstorage-0.1.3.tar` & `cbstorage-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       22 2023-04-14 13:09:33.104854 cbstorage-0.1.3/cbstorage/__init__.py
--rw-r--r--   0        0        0     7498 2023-04-14 13:20:46.801175 cbstorage-0.1.3/cbstorage/storage.py
--rw-r--r--   0        0        0      340 2023-04-14 13:37:58.096001 cbstorage-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      592 2023-04-14 13:37:59.207590 cbstorage-0.1.3/setup.py
--rw-r--r--   0        0        0      439 2023-04-14 13:37:59.207707 cbstorage-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-14 13:09:33.104854 cbstorage-0.1.4/cbstorage/__init__.py
+-rw-r--r--   0        0        0     7498 2023-04-14 13:20:46.801175 cbstorage-0.1.4/cbstorage/storage.py
+-rw-r--r--   0        0        0      649 2023-04-14 13:44:41.001051 cbstorage-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      901 2023-04-14 13:44:41.921778 cbstorage-0.1.4/setup.py
+-rw-r--r--   0        0        0      748 2023-04-14 13:44:41.921910 cbstorage-0.1.4/PKG-INFO
```

### Comparing `cbstorage-0.1.3/cbstorage/storage.py` & `cbstorage-0.1.4/cbstorage/storage.py`

 * *Files identical despite different names*

