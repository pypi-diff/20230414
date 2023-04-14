# Comparing `tmp/parsenv-0.1.1.tar.gz` & `tmp/parsenv-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsenv-0.1.1.tar", last modified: Fri Apr 14 14:51:48 2023, max compression
+gzip compressed data, was "parsenv-0.1.2.tar", last modified: Fri Apr 14 14:55:08 2023, max compression
```

## Comparing `parsenv-0.1.1.tar` & `parsenv-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      108 2023-04-14 13:58:02.332781 parsenv-0.1.1/env/__init__.py
--rw-r--r--   0        0        0      997 2023-04-14 14:41:02.857950 parsenv-0.1.1/env/core.py
--rw-r--r--   0        0        0      522 2023-04-14 13:58:02.297520 parsenv-0.1.1/env/main.py
--rw-r--r--   0        0        0      190 2023-04-14 13:58:02.313738 parsenv-0.1.1/env/parsers.py
--rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.1.1/env/py.typed
--rw-r--r--   0        0        0      449 2023-04-14 14:51:44.778654 parsenv-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      601 2023-04-14 14:51:38.676003 parsenv-0.1.1/README.md
--rw-r--r--   0        0        0      576 2023-04-14 14:41:44.254568 parsenv-0.1.1/tests/__main__.py
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 parsenv-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2023-04-14 13:58:02.332781 parsenv-0.1.2/env/__init__.py
+-rw-r--r--   0        0        0      997 2023-04-14 14:41:02.857950 parsenv-0.1.2/env/core.py
+-rw-r--r--   0        0        0      522 2023-04-14 13:58:02.297520 parsenv-0.1.2/env/main.py
+-rw-r--r--   0        0        0      190 2023-04-14 13:58:02.313738 parsenv-0.1.2/env/parsers.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.1.2/env/py.typed
+-rw-r--r--   0        0        0      449 2023-04-14 14:55:03.935900 parsenv-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-04-14 14:54:11.775560 parsenv-0.1.2/README.md
+-rw-r--r--   0        0        0      576 2023-04-14 14:41:44.254568 parsenv-0.1.2/tests/__main__.py
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 parsenv-0.1.2/PKG-INFO
```

### Comparing `parsenv-0.1.1/env/core.py` & `parsenv-0.1.2/env/core.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.1.1/env/main.py` & `parsenv-0.1.2/env/main.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.1.1/README.md` & `parsenv-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# parsenv
+# Env parser
 
 ```py
 import env
 
 assert env.get("TOKEN") == "abc123"
 assert env.get("X", False) is False
 assert env.get_int("PORT") == 123
```

### Comparing `parsenv-0.1.1/tests/__main__.py` & `parsenv-0.1.2/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.1.1/PKG-INFO` & `parsenv-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: parsenv
-Version: 0.1.1
+Version: 0.1.2
 License: MIT
 Author-email: levch <levchenko.d.a1998@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# parsenv
+# Env parser
 
 ```py
 import env
 
 assert env.get("TOKEN") == "abc123"
 assert env.get("X", False) is False
 assert env.get_int("PORT") == 123
```

