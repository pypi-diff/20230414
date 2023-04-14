# Comparing `tmp/parsenv-0.1.0.tar.gz` & `tmp/parsenv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsenv-0.1.0.tar", last modified: Fri Apr 14 14:48:15 2023, max compression
+gzip compressed data, was "parsenv-0.1.1.tar", last modified: Fri Apr 14 14:51:48 2023, max compression
```

## Comparing `parsenv-0.1.0.tar` & `parsenv-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      108 2023-04-14 13:58:02.332781 parsenv-0.1.0/env/__init__.py
--rw-r--r--   0        0        0      997 2023-04-14 14:41:02.857950 parsenv-0.1.0/env/core.py
--rw-r--r--   0        0        0      522 2023-04-14 13:58:02.297520 parsenv-0.1.0/env/main.py
--rw-r--r--   0        0        0      190 2023-04-14 13:58:02.313738 parsenv-0.1.0/env/parsers.py
--rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.1.0/env/py.typed
--rw-r--r--   0        0        0      449 2023-04-14 14:09:56.694736 parsenv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       15 2023-04-14 13:18:26.416106 parsenv-0.1.0/README.md
--rw-r--r--   0        0        0      576 2023-04-14 14:41:44.254568 parsenv-0.1.0/tests/__main__.py
--rw-r--r--   0        0        0      192 1970-01-01 00:00:00.000000 parsenv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      108 2023-04-14 13:58:02.332781 parsenv-0.1.1/env/__init__.py
+-rw-r--r--   0        0        0      997 2023-04-14 14:41:02.857950 parsenv-0.1.1/env/core.py
+-rw-r--r--   0        0        0      522 2023-04-14 13:58:02.297520 parsenv-0.1.1/env/main.py
+-rw-r--r--   0        0        0      190 2023-04-14 13:58:02.313738 parsenv-0.1.1/env/parsers.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.1.1/env/py.typed
+-rw-r--r--   0        0        0      449 2023-04-14 14:51:44.778654 parsenv-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      601 2023-04-14 14:51:38.676003 parsenv-0.1.1/README.md
+-rw-r--r--   0        0        0      576 2023-04-14 14:41:44.254568 parsenv-0.1.1/tests/__main__.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 parsenv-0.1.1/PKG-INFO
```

### Comparing `parsenv-0.1.0/env/core.py` & `parsenv-0.1.1/env/core.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.1.0/env/main.py` & `parsenv-0.1.1/env/main.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.1.0/tests/__main__.py` & `parsenv-0.1.1/tests/__main__.py`

 * *Files identical despite different names*

