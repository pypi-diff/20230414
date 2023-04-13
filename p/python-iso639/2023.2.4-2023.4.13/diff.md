# Comparing `tmp/python-iso639-2023.2.4.tar.gz` & `tmp/python-iso639-2023.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-iso639-2023.2.4.tar", last modified: Sat Feb  4 19:19:56 2023, max compression
+gzip compressed data, was "python-iso639-2023.4.13.tar", last modified: Thu Apr 13 23:11:57 2023, max compression
```

## Comparing `python-iso639-2023.2.4.tar` & `python-iso639-2023.4.13.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-02-04 19:19:56.712617 python-iso639-2023.2.4/
--rw-r--r--   0 jacksonlee   (501) staff       (20)    10759 2022-08-28 17:23:57.000000 python-iso639-2023.2.4/LICENSE.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)    13261 2023-02-04 19:19:56.712453 python-iso639-2023.2.4/PKG-INFO
--rw-r--r--   0 jacksonlee   (501) staff       (20)    11919 2023-02-04 19:16:58.000000 python-iso639-2023.2.4/README.md
--rw-r--r--   0 jacksonlee   (501) staff       (20)     1777 2023-02-04 19:16:58.000000 python-iso639-2023.2.4/pyproject.toml
--rw-r--r--   0 jacksonlee   (501) staff       (20)       38 2023-02-04 19:19:56.712649 python-iso639-2023.2.4/setup.cfg
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-02-04 19:19:56.709064 python-iso639-2023.2.4/src/
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-02-04 19:19:56.710433 python-iso639-2023.2.4/src/iso639/
--rw-r--r--   0 jacksonlee   (501) staff       (20)      525 2023-02-04 19:16:58.000000 python-iso639-2023.2.4/src/iso639/__init__.py
--rw-r--r--   0 jacksonlee   (501) staff       (20)     7693 2022-11-27 16:41:42.000000 python-iso639-2023.2.4/src/iso639/language.py
--rw-r--r--   0 jacksonlee   (501) staff       (20)   540672 2023-02-04 19:16:58.000000 python-iso639-2023.2.4/src/iso639/languages.db
-drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-02-04 19:19:56.712269 python-iso639-2023.2.4/src/python_iso639.egg-info/
--rw-r--r--   0 jacksonlee   (501) staff       (20)    13261 2023-02-04 19:19:56.000000 python-iso639-2023.2.4/src/python_iso639.egg-info/PKG-INFO
--rw-r--r--   0 jacksonlee   (501) staff       (20)      350 2023-02-04 19:19:56.000000 python-iso639-2023.2.4/src/python_iso639.egg-info/SOURCES.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2023-02-04 19:19:56.000000 python-iso639-2023.2.4/src/python_iso639.egg-info/dependency_links.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2022-08-28 17:28:05.000000 python-iso639-2023.2.4/src/python_iso639.egg-info/not-zip-safe
--rw-r--r--   0 jacksonlee   (501) staff       (20)       76 2023-02-04 19:19:56.000000 python-iso639-2023.2.4/src/python_iso639.egg-info/requires.txt
--rw-r--r--   0 jacksonlee   (501) staff       (20)        7 2023-02-04 19:19:56.000000 python-iso639-2023.2.4/src/python_iso639.egg-info/top_level.txt
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-04-13 23:11:57.942475 python-iso639-2023.4.13/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    10759 2022-08-28 17:23:57.000000 python-iso639-2023.4.13/LICENSE.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    13262 2023-04-13 23:11:57.942257 python-iso639-2023.4.13/PKG-INFO
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    11919 2023-02-04 19:16:58.000000 python-iso639-2023.4.13/README.md
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     1778 2023-04-13 23:10:38.000000 python-iso639-2023.4.13/pyproject.toml
+-rw-r--r--   0 jacksonlee   (501) staff       (20)       38 2023-04-13 23:11:57.942509 python-iso639-2023.4.13/setup.cfg
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-04-13 23:11:57.938351 python-iso639-2023.4.13/src/
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-04-13 23:11:57.939445 python-iso639-2023.4.13/src/iso639/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)      525 2023-02-04 19:16:58.000000 python-iso639-2023.4.13/src/iso639/__init__.py
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     7722 2023-04-13 23:04:34.000000 python-iso639-2023.4.13/src/iso639/language.py
+-rw-r--r--   0 jacksonlee   (501) staff       (20)   540672 2023-02-04 19:16:58.000000 python-iso639-2023.4.13/src/iso639/languages.db
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-04-13 23:11:57.941526 python-iso639-2023.4.13/src/python_iso639.egg-info/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)    13262 2023-04-13 23:11:57.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/PKG-INFO
+-rw-r--r--   0 jacksonlee   (501) staff       (20)      402 2023-04-13 23:11:57.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/SOURCES.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2023-04-13 23:11:57.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/dependency_links.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)        1 2022-08-28 17:28:05.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/not-zip-safe
+-rw-r--r--   0 jacksonlee   (501) staff       (20)       76 2023-04-13 23:11:57.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/requires.txt
+-rw-r--r--   0 jacksonlee   (501) staff       (20)        7 2023-04-13 23:11:57.000000 python-iso639-2023.4.13/src/python_iso639.egg-info/top_level.txt
+drwxr-xr-x   0 jacksonlee   (501) staff       (20)        0 2023-04-13 23:11:57.941910 python-iso639-2023.4.13/tests/
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     2435 2023-02-04 19:16:58.000000 python-iso639-2023.4.13/tests/test_language.py
+-rw-r--r--   0 jacksonlee   (501) staff       (20)     1295 2022-08-28 17:23:57.000000 python-iso639-2023.4.13/tests/test_version_number.py
```

### Comparing `python-iso639-2023.2.4/LICENSE.txt` & `python-iso639-2023.4.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-iso639-2023.2.4/PKG-INFO` & `python-iso639-2023.4.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iso639
-Version: 2023.2.4
+Version: 2023.4.13
 Summary: Look-up utilities for ISO 639 language codes and names
 Author-email: "Jackson L. Lee" <jacksonlunlee@gmail.com>
 License: Apache 2.0
 Project-URL: source, https://github.com/jacksonllee/iso639
 Project-URL: tracker, https://github.com/jacksonllee/iso639/issues
 Keywords: ISO 639,language codes,languages,linguistics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-iso639-2023.2.4/README.md` & `python-iso639-2023.4.13/README.md`

 * *Files identical despite different names*

### Comparing `python-iso639-2023.2.4/pyproject.toml` & `python-iso639-2023.4.13/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.3.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-iso639"
-version = "2023.2.4"
+version = "2023.4.13"
 description = "Look-up utilities for ISO 639 language codes and names"
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { text = "Apache 2.0" }
 authors = [ { name = "Jackson L. Lee", email = "jacksonlunlee@gmail.com" } ]
 keywords = ["ISO 639", "language codes", "languages", "linguistics"]
 classifiers = [
```

### Comparing `python-iso639-2023.2.4/src/iso639/__init__.py` & `python-iso639-2023.4.13/src/iso639/__init__.py`

 * *Files identical despite different names*

### Comparing `python-iso639-2023.2.4/src/iso639/language.py` & `python-iso639-2023.4.13/src/iso639/language.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dataclasses import dataclass
 
 from typing import Iterable, List, Optional, Tuple
 
 
 _DB = sqlite3.connect(
     os.path.join(os.path.dirname(os.path.realpath(__file__)), "languages.db"),
+    check_same_thread=False,
 )
 
 
 class LanguageNotFoundError(Exception):
     pass
```

### Comparing `python-iso639-2023.2.4/src/iso639/languages.db` & `python-iso639-2023.4.13/src/iso639/languages.db`

 * *Files identical despite different names*

### Comparing `python-iso639-2023.2.4/src/python_iso639.egg-info/PKG-INFO` & `python-iso639-2023.4.13/src/python_iso639.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-iso639
-Version: 2023.2.4
+Version: 2023.4.13
 Summary: Look-up utilities for ISO 639 language codes and names
 Author-email: "Jackson L. Lee" <jacksonlunlee@gmail.com>
 License: Apache 2.0
 Project-URL: source, https://github.com/jacksonllee/iso639
 Project-URL: tracker, https://github.com/jacksonllee/iso639/issues
 Keywords: ISO 639,language codes,languages,linguistics
 Classifier: Development Status :: 5 - Production/Stable
```

