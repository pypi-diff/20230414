# Comparing `tmp/parsenv-0.1.2.tar.gz` & `tmp/parsenv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsenv-0.1.2.tar", last modified: Fri Apr 14 14:55:08 2023, max compression
+gzip compressed data, was "parsenv-0.1.3.tar", last modified: Fri Apr 14 15:00:54 2023, max compression
```

## Comparing `parsenv-0.1.2.tar` & `parsenv-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      108 2023-04-14 13:58:02.332781 parsenv-0.1.2/env/__init__.py
--rw-r--r--   0        0        0      997 2023-04-14 14:41:02.857950 parsenv-0.1.2/env/core.py
--rw-r--r--   0        0        0      522 2023-04-14 13:58:02.297520 parsenv-0.1.2/env/main.py
--rw-r--r--   0        0        0      190 2023-04-14 13:58:02.313738 parsenv-0.1.2/env/parsers.py
--rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.1.2/env/py.typed
--rw-r--r--   0        0        0      449 2023-04-14 14:55:03.935900 parsenv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      604 2023-04-14 14:54:11.775560 parsenv-0.1.2/README.md
--rw-r--r--   0        0        0      576 2023-04-14 14:41:44.254568 parsenv-0.1.2/tests/__main__.py
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 parsenv-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      108 2023-04-14 13:58:02.332781 parsenv-0.1.3/env/__init__.py
+-rw-r--r--   0        0        0      997 2023-04-14 14:41:02.857950 parsenv-0.1.3/env/core.py
+-rw-r--r--   0        0        0      522 2023-04-14 13:58:02.297520 parsenv-0.1.3/env/main.py
+-rw-r--r--   0        0        0      190 2023-04-14 13:58:02.313738 parsenv-0.1.3/env/parsers.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:19:51.037073 parsenv-0.1.3/env/py.typed
+-rw-r--r--   0        0        0      449 2023-04-14 15:00:50.420182 parsenv-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      665 2023-04-14 15:00:50.440285 parsenv-0.1.3/README.md
+-rw-r--r--   0        0        0      576 2023-04-14 14:41:44.254568 parsenv-0.1.3/tests/__main__.py
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 parsenv-0.1.3/PKG-INFO
```

### Comparing `parsenv-0.1.2/env/core.py` & `parsenv-0.1.3/env/core.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.1.2/env/main.py` & `parsenv-0.1.3/env/main.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.1.2/README.md` & `parsenv-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Env parser
 
+Use `pip install parsenv`
+
+## Example
+
 ```py
 import env
 
 assert env.get("TOKEN") == "abc123"
 assert env.get("X", False) is False
 assert env.get_int("PORT") == 123
 assert env.get_strs("KEYS", []) == ["word1", "F402", "12"]
@@ -15,11 +19,11 @@
 except KeyError as e:
     assert str(e) == "Environment variable `X` not set"
 
 try:
     env.get_ints("BAD_NUMS")
 except ValueError as e:
     assert (
-        str(e) == "Can't parse environment variable `BAD_NUMS`: "
-        "invalid literal for int() with base 10: 'a'"
+            str(e) == "Can't parse environment variable `BAD_NUMS`: "
+                      "invalid literal for int() with base 10: 'a'"
     )
 ```
```

### Comparing `parsenv-0.1.2/tests/__main__.py` & `parsenv-0.1.3/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `parsenv-0.1.2/PKG-INFO` & `parsenv-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: parsenv
-Version: 0.1.2
+Version: 0.1.3
 License: MIT
 Author-email: levch <levchenko.d.a1998@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Env parser
 
+Use `pip install parsenv`
+
+## Example
+
 ```py
 import env
 
 assert env.get("TOKEN") == "abc123"
 assert env.get("X", False) is False
 assert env.get_int("PORT") == 123
 assert env.get_strs("KEYS", []) == ["word1", "F402", "12"]
@@ -23,12 +27,12 @@
 except KeyError as e:
     assert str(e) == "Environment variable `X` not set"
 
 try:
     env.get_ints("BAD_NUMS")
 except ValueError as e:
     assert (
-        str(e) == "Can't parse environment variable `BAD_NUMS`: "
-        "invalid literal for int() with base 10: 'a'"
+            str(e) == "Can't parse environment variable `BAD_NUMS`: "
+                      "invalid literal for int() with base 10: 'a'"
     )
 ```
```

