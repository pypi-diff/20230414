# Comparing `tmp/pepper_cli-0.1.0.tar.gz` & `tmp/pepper_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepper_cli-0.1.0.tar", max compression
+gzip compressed data, was "pepper_cli-0.1.1.tar", max compression
```

## Comparing `pepper_cli-0.1.0.tar` & `pepper_cli-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1137 2023-04-14 02:59:53.956400 pepper_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     4367 2023-04-14 02:59:53.956400 pepper_cli-0.1.0/README.md
--rw-r--r--   0        0        0    15466 2023-04-14 02:59:53.956400 pepper_cli-0.1.0/pepper_cli.py
--rw-r--r--   0        0        0      763 2023-04-14 02:59:53.956400 pepper_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4963 1970-01-01 00:00:00.000000 pepper_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-04-14 03:09:12.769659 pepper_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4367 2023-04-14 03:09:12.769659 pepper_cli-0.1.1/README.md
+-rw-r--r--   0        0        0    15389 2023-04-14 03:09:12.769659 pepper_cli-0.1.1/pepper_cli.py
+-rw-r--r--   0        0        0      763 2023-04-14 03:09:12.769659 pepper_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4963 1970-01-01 00:00:00.000000 pepper_cli-0.1.1/PKG-INFO
```

### Comparing `pepper_cli-0.1.0/LICENSE` & `pepper_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pepper_cli-0.1.0/README.md` & `pepper_cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pepper_cli-0.1.0/pepper_cli.py` & `pepper_cli-0.1.1/pepper_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 import webbrowser
 import multiprocessing
 from textwrap import TextWrapper
 from urllib.request import urlopen, HTTPError
 from http.client import HTTPResponse
 from html.parser import HTMLParser
 
-__version__ = "0.1.0"
-RAW_PEP_URL_BASE = "https://raw.githubusercontent.com/python/peps/main/pep-"
+__version__ = "0.1.1"
 PEP_URL_BASE = "https://peps.python.org/pep-"
 PEP_0_URL = "https://peps.python.org/pep-0000"
 
 try:
     WEBVIEW = __import__("webview")
 except ModuleNotFoundError:
     WEBVIEW = None
```

### Comparing `pepper_cli-0.1.0/pyproject.toml` & `pepper_cli-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pepper-cli"
-version = "0.1.0"
+version = "0.1.1"
 description = "Get information about any PEP (Python Enhancement Proposal)"
 authors = ["Noah Tanner <50159154+kevinshome@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pepper_cli-0.1.0/PKG-INFO` & `pepper_cli-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepper-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Get information about any PEP (Python Enhancement Proposal)
 License: MIT
 Author: Noah Tanner
 Author-email: 50159154+kevinshome@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

