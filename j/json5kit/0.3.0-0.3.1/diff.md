# Comparing `tmp/json5kit-0.3.0.tar.gz` & `tmp/json5kit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json5kit-0.3.0.tar", last modified: Thu Apr 13 21:51:33 2023, max compression
+gzip compressed data, was "json5kit-0.3.1.tar", last modified: Fri Apr 14 13:24:47 2023, max compression
```

## Comparing `json5kit-0.3.0.tar` & `json5kit-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-13 21:51:33.727327 json5kit-0.3.0/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2023-04-13 16:58:14.000000 json5kit-0.3.0/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-13 21:51:33.727432 json5kit-0.3.0/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1415 2023-04-13 21:46:23.000000 json5kit-0.3.0/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1170 2023-04-13 21:51:33.727888 json5kit-0.3.0/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       38 2023-04-13 16:58:14.000000 json5kit-0.3.0/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-13 21:51:33.725056 json5kit-0.3.0/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-13 21:51:33.726347 json5kit-0.3.0/src/json5kit/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)    11763 2023-04-13 21:33:38.000000 json5kit-0.3.0/src/json5kit/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     7225 2023-04-13 21:43:51.000000 json5kit-0.3.0/src/json5kit/nodes.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3629 2023-04-13 21:44:53.000000 json5kit-0.3.0/src/json5kit/visitor.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-13 21:51:33.727173 json5kit-0.3.0/src/json5kit.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-13 21:51:33.000000 json5kit-0.3.0/src/json5kit.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      286 2023-04-13 21:51:33.000000 json5kit-0.3.0/src/json5kit.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2023-04-13 21:51:33.000000 json5kit-0.3.0/src/json5kit.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       29 2023-04-13 21:51:33.000000 json5kit-0.3.0/src/json5kit.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2023-04-13 21:51:33.000000 json5kit-0.3.0/src/json5kit.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-14 13:24:47.501735 json5kit-0.3.1/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2023-04-13 16:58:14.000000 json5kit-0.3.1/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-14 13:24:47.501847 json5kit-0.3.1/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1415 2023-04-13 21:46:23.000000 json5kit-0.3.1/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1213 2023-04-14 13:24:47.502330 json5kit-0.3.1/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       38 2023-04-13 16:58:14.000000 json5kit-0.3.1/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-14 13:24:47.497236 json5kit-0.3.1/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-14 13:24:47.500376 json5kit-0.3.1/src/json5kit/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)    11877 2023-04-14 13:21:37.000000 json5kit-0.3.1/src/json5kit/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     7345 2023-04-14 13:19:22.000000 json5kit-0.3.1/src/json5kit/nodes.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3629 2023-04-13 21:44:53.000000 json5kit-0.3.1/src/json5kit/visitor.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-14 13:24:47.501567 json5kit-0.3.1/src/json5kit.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-14 13:24:47.000000 json5kit-0.3.1/src/json5kit.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      286 2023-04-14 13:24:47.000000 json5kit-0.3.1/src/json5kit.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2023-04-14 13:24:47.000000 json5kit-0.3.1/src/json5kit.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       77 2023-04-14 13:24:47.000000 json5kit-0.3.1/src/json5kit.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2023-04-14 13:24:47.000000 json5kit-0.3.1/src/json5kit.egg-info/top_level.txt
```

### Comparing `json5kit-0.3.0/LICENSE` & `json5kit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `json5kit-0.3.0/PKG-INFO` & `json5kit-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json5kit
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Roundtrip parser and CST for JSON, JSONC and JSON5.
 Home-page: https://github.com/tusharsadhwani/json5kit
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `json5kit-0.3.0/README.md` & `json5kit-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `json5kit-0.3.0/setup.cfg` & `json5kit-0.3.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = json5kit
-version = 0.3.0
+version = 0.3.1
 description = A Roundtrip parser and CST for JSON, JSONC and JSON5.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/json5kit
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
@@ -30,14 +30,15 @@
 where = ./src
 
 [options.extras_require]
 dev = 
 	black
 	mypy
 	pytest-cov
+	typing_extensions; python_version < "3.8"
 
 [tool:pytest]
 addopts = --cov --cov-report=term-missing
 
 [coverage:report]
 exclude_lines = 
 	\#\s*pragma: no cover\b
```

### Comparing `json5kit-0.3.0/src/json5kit/__init__.py` & `json5kit-0.3.1/src/json5kit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 """json5kit - A Parser and CST for JSON5."""
 from __future__ import annotations
 import string
+import sys
+
+from typing import Sequence, cast
+
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
 
-from typing import Literal, Sequence, cast
 
 from json5kit.nodes import (
     Json5Array,
     Json5Boolean,
     Json5Comma,
     Json5Comment,
     Json5File,
```

### Comparing `json5kit-0.3.0/src/json5kit/nodes.py` & `json5kit-0.3.1/src/json5kit/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from __future__ import annotations
+import sys
 
-from typing import Protocol, Self, runtime_checkable
+if sys.version_info >= (3, 8):
+    from typing import Protocol, Self, runtime_checkable
+else:
+    from typing_extensions import Protocol, Self, runtime_checkable
 
 
 @runtime_checkable
 class Json5Node(Protocol):
     """Sets the expectation from a JSON5 node: be able to convert back to source."""
 
     trailing_trivia_nodes: list[Json5Trivia]
```

### Comparing `json5kit-0.3.0/src/json5kit/visitor.py` & `json5kit-0.3.1/src/json5kit/visitor.py`

 * *Files identical despite different names*

### Comparing `json5kit-0.3.0/src/json5kit.egg-info/PKG-INFO` & `json5kit-0.3.1/src/json5kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json5kit
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Roundtrip parser and CST for JSON, JSONC and JSON5.
 Home-page: https://github.com/tusharsadhwani/json5kit
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

