# Comparing `tmp/seed_intersphinx_mapping-1.2.0.tar.gz` & `tmp/seed_intersphinx_mapping-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seed_intersphinx_mapping-1.2.0.tar", last modified: Thu Jan 12 10:25:07 2023, max compression
+gzip compressed data, was "seed_intersphinx_mapping-1.2.1.tar", last modified: Fri Apr 14 18:11:29 2023, max compression
```

## Comparing `seed_intersphinx_mapping-1.2.0.tar` & `seed_intersphinx_mapping-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-01-12 10:25:07.089096 seed_intersphinx_mapping-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-01-12 10:25:07.097097 seed_intersphinx_mapping-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5175 2023-01-12 10:25:07.097097 seed_intersphinx_mapping-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     7809 2023-01-12 10:25:07.097097 seed_intersphinx_mapping-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-01-12 10:25:07.097097 seed_intersphinx_mapping-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-12 10:24:29.560112 seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-01-12 10:24:29.560112 seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-01-12 10:24:29.560112 seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-01-12 10:24:29.560112 seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2960 2023-01-12 10:24:29.560112 seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/requirements_parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-01-12 10:24:29.560112 seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/fallback_mapping.json
--rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-01-12 10:24:29.560112 seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-04-14 18:11:29.150884 seed_intersphinx_mapping-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5175 2023-04-14 18:11:29.150884 seed_intersphinx_mapping-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-14 18:11:29.142884 seed_intersphinx_mapping-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7809 2023-04-14 18:11:29.150884 seed_intersphinx_mapping-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-14 18:11:29.150884 seed_intersphinx_mapping-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2960 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/requirements_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/fallback_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-04-14 18:11:00.726475 seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/extension.py
```

### Comparing `seed_intersphinx_mapping-1.2.0/LICENSE` & `seed_intersphinx_mapping-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seed_intersphinx_mapping-1.2.0/pyproject.toml` & `seed_intersphinx_mapping-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "seed_intersphinx_mapping"
-version = "1.2.0"
+version = "1.2.1"
 description = "Populate the Sphinx 'intersphinx_mapping' dictionary from the project's requirements."
 readme = "README.rst"
 keywords = [ "documentation", "intersphinx", "sphinx",]
 dynamic = []
 dependencies = [
     "apeye>=1.0.1",
     "dist-meta>=0.1.2",
@@ -49,15 +49,15 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/sphinx-toolbox/seed_intersphinx_mapping"
 "Issue Tracker" = "https://github.com/sphinx-toolbox/seed_intersphinx_mapping/issues"
 "Source Code" = "https://github.com/sphinx-toolbox/seed_intersphinx_mapping"
-Documentation = "https://seed_intersphinx_mapping.readthedocs.io/en/latest"
+Documentation = "https://seed-intersphinx-mapping.readthedocs.io/en/latest"
 
 [tool.whey]
 base-classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "Topic :: Documentation",
```

### Comparing `seed_intersphinx_mapping-1.2.0/README.rst` & `seed_intersphinx_mapping-1.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/seed_intersphinx_mapping/latest?logo=read-the-docs
-	:target: https://seed_intersphinx_mapping.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/seed-intersphinx-mapping/latest?logo=read-the-docs
+	:target: https://seed-intersphinx-mapping.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/workflows/Linux/badge.svg
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/seed_intersphinx_mapping
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/seed_intersphinx_mapping
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/seed_intersphinx_mapping/v1.2.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/seed_intersphinx_mapping/v1.2.1
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/seed_intersphinx_mapping
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/commit/master
 	:alt: GitHub last commit
```

### Comparing `seed_intersphinx_mapping-1.2.0/PKG-INFO` & `seed_intersphinx_mapping-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: seed-intersphinx-mapping
-Version: 1.2.0
+Version: 1.2.1
 Summary: Populate the Sphinx 'intersphinx_mapping' dictionary from the project's requirements.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: documentation,intersphinx,sphinx
 Home-page: https://github.com/sphinx-toolbox/seed_intersphinx_mapping
 Project-URL: Issue Tracker, https://github.com/sphinx-toolbox/seed_intersphinx_mapping/issues
 Project-URL: Source Code, https://github.com/sphinx-toolbox/seed_intersphinx_mapping
-Project-URL: Documentation, https://seed_intersphinx_mapping.readthedocs.io/en/latest
+Project-URL: Documentation, https://seed-intersphinx-mapping.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -70,16 +70,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/seed_intersphinx_mapping/latest?logo=read-the-docs
-	:target: https://seed_intersphinx_mapping.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/seed-intersphinx-mapping/latest?logo=read-the-docs
+	:target: https://seed-intersphinx-mapping.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/workflows/Linux/badge.svg
@@ -141,15 +141,15 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/seed_intersphinx_mapping
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/seed_intersphinx_mapping
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/seed_intersphinx_mapping/v1.2.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/seed_intersphinx_mapping/v1.2.1
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/seed_intersphinx_mapping
 	:target: https://github.com/sphinx-toolbox/seed_intersphinx_mapping/commit/master
 	:alt: GitHub last commit
```

### Comparing `seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/cache.py` & `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/cache.py`

 * *Files identical despite different names*

### Comparing `seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/__main__.py` & `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/__main__.py`

 * *Files identical despite different names*

### Comparing `seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/__init__.py` & `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # this package
 from seed_intersphinx_mapping.cache import cache
 from seed_intersphinx_mapping.extension import setup
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "1.2.0"
+__version__: str = "1.2.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["get_sphinx_doc_url", "fallback_mapping", "seed_intersphinx_mapping"]
 
 _DOCUMENTATION_RE = re.compile(r"^[dD]oc(s|umentation)")
```

### Comparing `seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/requirements_parsers.py` & `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/requirements_parsers.py`

 * *Files identical despite different names*

### Comparing `seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/fallback_mapping.json` & `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/fallback_mapping.json`

 * *Files identical despite different names*

### Comparing `seed_intersphinx_mapping-1.2.0/seed_intersphinx_mapping/extension.py` & `seed_intersphinx_mapping-1.2.1/seed_intersphinx_mapping/extension.py`

 * *Files identical despite different names*

