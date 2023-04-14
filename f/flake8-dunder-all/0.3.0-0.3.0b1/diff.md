# Comparing `tmp/flake8_dunder_all-0.3.0.tar.gz` & `tmp/flake8_dunder_all-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_dunder_all-0.3.0.tar", last modified: Fri Apr 14 13:15:27 2023, max compression
+gzip compressed data, was "flake8_dunder_all-0.3.0b1.tar", last modified: Tue Apr 11 13:11:49 2023, max compression
```

## Comparing `flake8_dunder_all-0.3.0.tar` & `flake8_dunder_all-0.3.0b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0 runner    (1001) docker     (122)     8053 2023-04-14 13:15:27.110515 flake8_dunder_all-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-04-14 13:15:27.106516 flake8_dunder_all-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-04-14 13:15:27.098515 flake8_dunder_all-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-04-14 13:15:27.110515 flake8_dunder_all-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-14 13:15:27.106516 flake8_dunder_all-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8628 2023-04-14 13:14:48.134352 flake8_dunder_all-0.3.0/flake8_dunder_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 13:14:48.134352 flake8_dunder_all-0.3.0/flake8_dunder_all/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-04-14 13:14:48.134352 flake8_dunder_all-0.3.0/flake8_dunder_all/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3102 2023-04-14 13:14:48.134352 flake8_dunder_all-0.3.0/flake8_dunder_all/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8059 2023-04-11 13:11:49.717365 flake8_dunder_all-0.3.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4919 2023-04-11 13:11:49.713365 flake8_dunder_all-0.3.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-04-11 13:11:49.709365 flake8_dunder_all-0.3.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6456 2023-04-11 13:11:49.717365 flake8_dunder_all-0.3.0b1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-11 13:11:49.717365 flake8_dunder_all-0.3.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8630 2023-04-11 13:11:20.712577 flake8_dunder_all-0.3.0b1/flake8_dunder_all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 13:11:20.712577 flake8_dunder_all-0.3.0b1/flake8_dunder_all/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-04-11 13:11:20.712577 flake8_dunder_all-0.3.0b1/flake8_dunder_all/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3102 2023-04-11 13:11:20.712577 flake8_dunder_all-0.3.0b1/flake8_dunder_all/utils.py
```

### Comparing `flake8_dunder_all-0.3.0/PKG-INFO` & `flake8_dunder_all-0.3.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-dunder-all
-Version: 0.3.0
+Version: 0.3.0b1
 Summary: A Flake8 plugin and pre-commit hook which checks to ensure modules have defined '__all__'.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: flake8
 Home-page: https://github.com/python-formate/flake8-dunder-all
 Project-URL: Issue Tracker, https://github.com/python-formate/flake8-dunder-all/issues
 Project-URL: Source Code, https://github.com/python-formate/flake8-dunder-all
@@ -136,15 +136,15 @@
 .. |license| image:: https://img.shields.io/github/license/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/python-formate/flake8-dunder-all
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.3.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.3.0b1
 	:target: https://github.com/python-formate/flake8-dunder-all/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/commit/master
 	:alt: GitHub last commit
 
@@ -208,15 +208,15 @@
 
 .. code-block:: yaml
 
 	 - repo: https://gitlab.com/pycqa/flake8
 	   rev: 3.8.1
 	   hooks:
 	    - id: flake8
-	      additional_dependencies: [flake8-dunder-all==0.3.0]
+	      additional_dependencies: [flake8-dunder-all==0.3.0b1]
 
 ``ensure-dunder-all`` script
 
 There is also a script which will automatically add __all__ for files which don't have it.
 
 See `the documentation <https://flake8-dunder-all.readthedocs.io/en/latest/usage.html#ensure-dunder-all-script>`_
 for details.
```

### Comparing `flake8_dunder_all-0.3.0/pyproject.toml` & `flake8_dunder_all-0.3.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "flake8-dunder-all"
-version = "0.3.0"
+version = "0.3.0b1"
 description = "A Flake8 plugin and pre-commit hook which checks to ensure modules have defined '__all__'."
 readme = "README.rst"
 keywords = [ "flake8",]
 dynamic = []
 dependencies = [
     "astatine>=0.3.1",
     "click>=7.1.2",
```

### Comparing `flake8_dunder_all-0.3.0/LICENSE` & `flake8_dunder_all-0.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_dunder_all-0.3.0/README.rst` & `flake8_dunder_all-0.3.0b1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/python-formate/flake8-dunder-all
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.3.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-formate/flake8-dunder-all/v0.3.0b1
 	:target: https://github.com/python-formate/flake8-dunder-all/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/python-formate/flake8-dunder-all
 	:target: https://github.com/python-formate/flake8-dunder-all/commit/master
 	:alt: GitHub last commit
 
@@ -169,15 +169,15 @@
 
 .. code-block:: yaml
 
 	 - repo: https://gitlab.com/pycqa/flake8
 	   rev: 3.8.1
 	   hooks:
 	    - id: flake8
-	      additional_dependencies: [flake8-dunder-all==0.3.0]
+	      additional_dependencies: [flake8-dunder-all==0.3.0b1]
 
 ``ensure-dunder-all`` script
 
 There is also a script which will automatically add __all__ for files which don't have it.
 
 See `the documentation <https://flake8-dunder-all.readthedocs.io/en/latest/usage.html#ensure-dunder-all-script>`_
 for details.
```

### Comparing `flake8_dunder_all-0.3.0/flake8_dunder_all/__init__.py` & `flake8_dunder_all-0.3.0b1/flake8_dunder_all/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 # this package
 from flake8_dunder_all.utils import find_noqa, get_docstring_lineno, mark_text_ranges
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT"
-__version__: str = "0.3.0"
+__version__: str = "0.3.0b1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ("Visitor", "Plugin", "check_and_add_all", "DALL000")
 
 DALL000 = "DALL000 Module lacks __all__."
```

### Comparing `flake8_dunder_all-0.3.0/flake8_dunder_all/__main__.py` & `flake8_dunder_all-0.3.0b1/flake8_dunder_all/__main__.py`

 * *Files identical despite different names*

### Comparing `flake8_dunder_all-0.3.0/flake8_dunder_all/utils.py` & `flake8_dunder_all-0.3.0b1/flake8_dunder_all/utils.py`

 * *Files identical despite different names*

