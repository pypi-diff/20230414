# Comparing `tmp/watchful-3.1.0.tar.gz` & `tmp/watchful-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchful-3.1.0.tar", last modified: Fri Apr 14 21:00:13 2023, max compression
+gzip compressed data, was "watchful-3.5.0.tar", last modified: Thu Apr  6 12:17:55 2023, max compression
```

## Comparing `watchful-3.1.0.tar` & `watchful-3.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 21:00:13.520734 watchful-3.1.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-14 20:56:42.000000 watchful-3.1.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2023-04-14 20:56:42.000000 watchful-3.1.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-14 21:00:13.520734 watchful-3.1.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6405 2023-04-14 20:56:42.000000 watchful-3.1.0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2064 2023-04-14 20:56:42.000000 watchful-3.1.0/README_PYPI.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-04-14 20:56:42.000000 watchful-3.1.0/README_PY_ENV.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 21:00:13.516734 watchful-3.1.0/examples/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   325333 2023-04-14 20:56:42.000000 watchful-3.1.0/examples/api_intro.ipynb
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1892 2023-04-14 20:56:42.000000 watchful-3.1.0/examples/requirements_api_intro.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      998 2023-04-14 20:56:42.000000 watchful-3.1.0/pylama.ini
--rw-r--r--   0 circleci  (3434) circleci  (3434)      375 2023-04-14 20:56:42.000000 watchful-3.1.0/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      983 2023-04-14 21:00:13.520734 watchful-3.1.0/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 21:00:13.512734 watchful-3.1.0/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 21:00:13.516734 watchful-3.1.0/src/watchful/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-04-14 20:56:42.000000 watchful-3.1.0/src/watchful/VERSION
--rw-r--r--   0 circleci  (3434) circleci  (3434)      575 2023-04-14 20:56:42.000000 watchful-3.1.0/src/watchful/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39513 2023-04-14 20:56:42.000000 watchful-3.1.0/src/watchful/attributes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    48367 2023-04-14 20:56:42.000000 watchful-3.1.0/src/watchful/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15767 2023-04-14 20:56:42.000000 watchful-3.1.0/src/watchful/enrich.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6356 2023-04-14 20:56:42.000000 watchful-3.1.0/src/watchful/enricher.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 21:00:13.520734 watchful-3.1.0/src/watchful.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-14 21:00:13.000000 watchful-3.1.0/src/watchful.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-04-14 21:00:13.000000 watchful-3.1.0/src/watchful.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-14 21:00:13.000000 watchful-3.1.0/src/watchful.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-04-14 21:00:13.000000 watchful-3.1.0/src/watchful.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-14 21:00:13.000000 watchful-3.1.0/src/watchful.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 21:00:13.520734 watchful-3.1.0/tests/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      388 2023-04-14 20:56:42.000000 watchful-3.1.0/tests/test_0000_import_sdk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2691 2023-04-14 20:56:42.000000 watchful-3.1.0/tests/test_0001_sdk_version_and_default_conn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-04-14 20:56:42.000000 watchful-3.1.0/tests/test_0002_encoding.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-06 12:14:03.000000 watchful-3.5.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2023-04-06 12:14:03.000000 watchful-3.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-06 12:17:55.945730 watchful-3.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6405 2023-04-06 12:14:03.000000 watchful-3.5.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2064 2023-04-06 12:14:03.000000 watchful-3.5.0/README_PYPI.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1554 2023-04-06 12:14:03.000000 watchful-3.5.0/README_PY_ENV.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/examples/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   325333 2023-04-06 12:14:03.000000 watchful-3.5.0/examples/api_intro.ipynb
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1900 2023-04-06 12:14:03.000000 watchful-3.5.0/examples/requirements_api_intro.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      998 2023-04-06 12:14:03.000000 watchful-3.5.0/pylama.ini
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      375 2023-04-06 12:14:03.000000 watchful-3.5.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      983 2023-04-06 12:17:55.949730 watchful-3.5.0/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.941730 watchful-3.5.0/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/src/watchful/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/VERSION
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      575 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39332 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/attributes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    48367 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15767 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/enrich.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6356 2023-04-06 12:14:03.000000 watchful-3.5.0/src/watchful/enricher.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/src/watchful.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-06 12:17:55.000000 watchful-3.5.0/src/watchful.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 12:17:55.945730 watchful-3.5.0/tests/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      388 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0000_import_sdk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2691 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0001_sdk_version_and_default_conn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-04-06 12:14:03.000000 watchful-3.5.0/tests/test_0002_encoding.py
```

### Comparing `watchful-3.1.0/LICENSE` & `watchful-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/PKG-INFO` & `watchful-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchful
-Version: 3.1.0
+Version: 3.5.0
 Summary: Watchful API for Interacting with Watchful Environment
 Home-page: https://github.com/Watchfulio/watchful-py
 Author: Watchful, Inc.
 Author-email: engineering@watchful.io
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/Watchfulio/watchful-py/issues
 Keywords: watchful
```

### Comparing `watchful-3.1.0/README.md` & `watchful-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/README_PYPI.md` & `watchful-3.5.0/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/README_PY_ENV.md` & `watchful-3.5.0/README_PY_ENV.md`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/examples/api_intro.ipynb` & `watchful-3.5.0/examples/api_intro.ipynb`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/examples/requirements_api_intro.txt` & `watchful-3.5.0/examples/requirements_api_intro.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 executing==1.2.0
 filelock==3.8.0
 flair==0.11.3
 fonttools==4.38.0
 ftfy==6.1.1
 future==0.18.3
 gdown==4.5.3
-gensim==4.3.1
+gensim==4.3.0
 huggingface-hub==0.13.3
 hyperopt==0.2.7
 idna==3.4
 importlib-metadata==6.1.0
 ipykernel==5.3.4
 ipython==8.10.0
 ipython-genutils==0.2.0
@@ -80,15 +80,15 @@
 scikit-learn==1.1.3
 scipy==1.9.3
 segtok==1.5.11
 sentencepiece==0.1.97
 setuptools==67.5.1
 six==1.16.0
 smart-open==6.3.0
-soupsieve==2.4
+soupsieve==2.3.2.post1
 spacy==3.4.3
 spacy-legacy==3.0.10
 spacy-loggers==1.0.3
 spacytextblob==4.0.0
 sqlitedict==2.1.0
 srsly==2.4.6
 stack-data==0.6.2
@@ -104,11 +104,11 @@
 transformers==4.26.1
 typer==0.7.0
 typing_extensions==4.4.0
 urllib3==1.26.13
 wasabi==0.10.1
 watchful==1.2.0
 wcwidth==0.2.5
-wheel==0.40.0
+wheel==0.38.1
 Wikipedia-API==0.5.4
 wrapt==1.14.1
 zipp==3.15.0
```

### Comparing `watchful-3.1.0/pylama.ini` & `watchful-3.5.0/pylama.ini`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/setup.cfg` & `watchful-3.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/src/watchful/__init__.py` & `watchful-3.5.0/src/watchful/__init__.py`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/src/watchful/attributes.py` & `watchful-3.5.0/src/watchful/attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 ################################################################################
 
 
 import csv
 import io
 import json
+import numbers
 import os
 import pprint
 import re
 from heapq import merge
 from multiprocessing import Pool
 from typing import Callable, Dict, List, Optional, Tuple
 import psutil
@@ -267,25 +268,22 @@
             # Gather and create new mappings at the same time. Duh :)
             for attr, vals in attr_vals.items():
                 if attr not in attrs:
                     attrs[attr] = len(attrs) + 1
                     values[attr] = {}
                     new_attrs.append(attr)
                 for val in vals:
-                    if isinstance(val, (int, float, bool)):
+                    if isinstance(val, numbers.Number):
                         val = str(val)
-                    elif val is None:
-                        pass
-                    elif val == "" or not isinstance(val, str):
-                        raise ValueError(
-                            "Attribute value needs to be either a non-empty "
-                            f"string, int, float, bool or None; got {val} "
-                            "instead."
+                    elif val and not isinstance(val, str):
+                        raise Exception(
+                            "Attribute value must be a string, "
+                            "None or a number. Was: " + val
                         )
-                    if val and val not in values[attr]:
+                    if val and not val in values[attr]:
                         values[attr][val] = len(values[attr]) + 1
                         if attr not in new_values:
                             new_values[attr] = []
                         new_values[attr].append(val)
 
             # Create the vector for the current cell.
             span_val = []
@@ -295,17 +293,15 @@
                 assert len(span) == len(
                     vals
                 ), "Must be the same amount of spans as attribute values."
                 # Not base64 the attributes to save space since there aren't
                 # that many of them.
                 span_val.append(attrs[attr])
                 span_val.append(
-                    base64str(
-                        [values[attr][str(val)] if val else 0 for val in vals]
-                    )
+                    base64str([values[attr][val] if val else 0 for val in vals])
                 )
 
             cell.append(base64str(contig_spans(span)))
             cell.append(span_val)
 
         # Output the lines (attributes, values and the cell value itself).
         if new_attrs:
```

### Comparing `watchful-3.1.0/src/watchful/client.py` & `watchful-3.5.0/src/watchful/client.py`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/src/watchful/enrich.py` & `watchful-3.5.0/src/watchful/enrich.py`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/src/watchful/enricher.py` & `watchful-3.5.0/src/watchful/enricher.py`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/src/watchful.egg-info/PKG-INFO` & `watchful-3.5.0/src/watchful.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchful
-Version: 3.1.0
+Version: 3.5.0
 Summary: Watchful API for Interacting with Watchful Environment
 Home-page: https://github.com/Watchfulio/watchful-py
 Author: Watchful, Inc.
 Author-email: engineering@watchful.io
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/Watchfulio/watchful-py/issues
 Keywords: watchful
```

### Comparing `watchful-3.1.0/src/watchful.egg-info/SOURCES.txt` & `watchful-3.5.0/src/watchful.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/tests/test_0001_sdk_version_and_default_conn.py` & `watchful-3.5.0/tests/test_0001_sdk_version_and_default_conn.py`

 * *Files identical despite different names*

### Comparing `watchful-3.1.0/tests/test_0002_encoding.py` & `watchful-3.5.0/tests/test_0002_encoding.py`

 * *Files identical despite different names*

