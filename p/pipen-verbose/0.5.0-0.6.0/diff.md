# Comparing `tmp/pipen_verbose-0.5.0.tar.gz` & `tmp/pipen_verbose-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_verbose-0.5.0.tar", max compression
+gzip compressed data, was "pipen_verbose-0.6.0.tar", max compression
```

## Comparing `pipen_verbose-0.5.0.tar` & `pipen_verbose-0.6.0.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rwxr-xr-x   0        0        0     5398 2023-03-29 21:56:08.268808 pipen_verbose-0.5.0/README.md
--rwxr-xr-x   0        0        0     6266 2023-03-29 21:56:08.268808 pipen_verbose-0.5.0/pipen_verbose.py
--rwxr-xr-x   0        0        0     1084 2023-03-29 21:56:08.268808 pipen_verbose-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6093 1970-01-01 00:00:00.000000 pipen_verbose-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0     5398 2023-04-14 07:09:46.761085 pipen_verbose-0.6.0/README.md
+-rwxr-xr-x   0        0        0     6266 2023-04-14 07:09:46.761085 pipen_verbose-0.6.0/pipen_verbose.py
+-rwxr-xr-x   0        0        0     1130 2023-04-14 07:09:46.761085 pipen_verbose-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 pipen_verbose-0.6.0/setup.py
+-rw-r--r--   0        0        0     6090 1970-01-01 00:00:00.000000 pipen_verbose-0.6.0/PKG-INFO
```

### Comparing `pipen_verbose-0.5.0/README.md` & `pipen_verbose-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pipen_verbose-0.5.0/pipen_verbose.py` & `pipen_verbose-0.6.0/pipen_verbose.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pipen import plugin
 from pipen.utils import get_logger, brief_list
 
 if TYPE_CHECKING:  # pragma: no cover
     from pipen import Proc
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 logger = get_logger("verbose", "info")
 
 VERBOSAL_CONFIGS = {
     # name: getter
     "scheduler": lambda proc: proc.scheduler.name,
     "lang": None,
```

### Comparing `pipen_verbose-0.5.0/pyproject.toml` & `pipen_verbose-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [tool.poetry]
 name = "pipen-verbose"
-version = "0.5.0"
+version = "0.6.0"
 description = "Add verbosal information in logs for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-verbose"
 repository = "https://github.com/pwwang/pipen-verbose"
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen = "^0.7"
+python = "^3.8"
+pipen = "^0.9"
+
+[tool.poetry.build]
+generate-setup-file = true
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
 
 [build-system]
 requires = ["poetry>=0.12"]
```

### Comparing `pipen_verbose-0.5.0/PKG-INFO` & `pipen_verbose-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pipen-verbose
-Version: 0.5.0
+Version: 0.6.0
 Summary: Add verbosal information in logs for pipen.
 Home-page: https://github.com/pwwang/pipen-verbose
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pipen (>=0.7,<0.8)
+Requires-Dist: pipen (>=0.9,<0.10)
 Project-URL: Repository, https://github.com/pwwang/pipen-verbose
 Description-Content-Type: text/markdown
 
 # pipen-verbose
 
 Add verbosal information in logs for [pipen][1].
```

