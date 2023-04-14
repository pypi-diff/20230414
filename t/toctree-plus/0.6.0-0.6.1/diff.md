# Comparing `tmp/toctree_plus-0.6.0.tar.gz` & `tmp/toctree_plus-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toctree_plus-0.6.0.tar", last modified: Fri Mar 25 13:13:06 2022, max compression
+gzip compressed data, was "toctree_plus-0.6.1.tar", last modified: Fri Apr 14 14:56:58 2023, max compression
```

## Comparing `toctree_plus-0.6.0.tar` & `toctree_plus-0.6.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-03-25 13:13:05.993412 toctree_plus-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-03-25 13:13:06.009412 toctree_plus-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-03-25 13:13:06.009412 toctree_plus-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     8394 2022-03-25 13:13:06.089412 toctree_plus-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-03-25 13:13:06.009412 toctree_plus-0.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-25 13:12:20.057438 toctree_plus-0.6.0/sphinxcontrib/toctree_plus/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     9153 2022-03-25 13:12:20.057438 toctree_plus-0.6.0/sphinxcontrib/toctree_plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8396 2023-04-14 14:56:58.993141 toctree_plus-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-04-14 14:56:58.989141 toctree_plus-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-04-14 14:56:58.985141 toctree_plus-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6732 2023-04-14 14:56:58.993141 toctree_plus-0.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-14 14:56:58.993141 toctree_plus-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9153 2023-04-14 14:56:30.740730 toctree_plus-0.6.1/sphinxcontrib/toctree_plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 14:56:30.740730 toctree_plus-0.6.1/sphinxcontrib/toctree_plus/py.typed
```

### Comparing `toctree_plus-0.6.0/LICENSE` & `toctree_plus-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toctree_plus-0.6.0/pyproject.toml` & `toctree_plus-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "toctree_plus"
-version = "0.6.0"
+version = "0.6.1"
 description = "Enhanced Sphinx TocTree which shows classes, functions etc. as if they were sections."
 readme = "README.rst"
 keywords = [ "documentation", "sphinx", "sphinx-extension",]
 dynamic = []
 dependencies = [ "docutils==0.16", "jinja2<3.1", "sphinx<3.6.0,>=3.0.3",]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -40,15 +40,15 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/sphinx-toolbox/toctree_plus"
 "Issue Tracker" = "https://github.com/sphinx-toolbox/toctree_plus/issues"
 "Source Code" = "https://github.com/sphinx-toolbox/toctree_plus"
-Documentation = "https://toctree_plus.readthedocs.io/en/latest"
+Documentation = "https://toctree-plus.readthedocs.io/en/latest"
 
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "Topic :: Documentation",
@@ -76,25 +76,25 @@
 package_root = "sphinxcontrib/toctree_plus"
 extensions = [
     "sphinx_toolbox",
     "sphinx_toolbox.more_autodoc",
     "sphinx_toolbox.more_autosummary",
     "sphinx_toolbox.documentation_summary",
     "sphinx_toolbox.tweaks.param_dash",
+    "sphinxcontrib.toctree_plus",
     "sphinx_toolbox.tweaks.latex_layout",
     "sphinx_toolbox.tweaks.latex_toc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinxcontrib.extras_require",
     "sphinx.ext.todo",
     "sphinxemoji.sphinxemoji",
     "notfound.extension",
     "sphinx_copybutton",
     "sphinxcontrib.default_values",
-    "sphinxcontrib.toctree_plus",
     "sphinx_debuginfo",
     "sphinx_licenseinfo",
     "seed_intersphinx_mapping",
     "html_section",
     "sphinx.ext.autosummary",
     "sphinx_toolbox_experimental.autosummary_widths",
 ]
```

### Comparing `toctree_plus-0.6.0/PKG-INFO` & `toctree_plus-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: toctree-plus
-Version: 0.6.0
+Version: 0.6.1
 Summary: Enhanced Sphinx TocTree which shows classes, functions etc. as if they were sections.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: BSD-3-Clause
 Keywords: documentation,sphinx,sphinx-extension
 Home-page: https://github.com/sphinx-toolbox/toctree_plus
 Project-URL: Issue Tracker, https://github.com/sphinx-toolbox/toctree_plus/issues
 Project-URL: Source Code, https://github.com/sphinx-toolbox/toctree_plus
-Project-URL: Documentation, https://toctree_plus.readthedocs.io/en/latest
+Project-URL: Documentation, https://toctree-plus.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -64,16 +64,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/toctree_plus/latest?logo=read-the-docs
-	:target: https://toctree_plus.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/toctree-plus/latest?logo=read-the-docs
+	:target: https://toctree-plus.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/sphinx-toolbox/toctree_plus/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/sphinx-toolbox/toctree_plus/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/sphinx-toolbox/toctree_plus/workflows/Linux/badge.svg
@@ -92,16 +92,16 @@
 	:target: https://github.com/sphinx-toolbox/toctree_plus/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/sphinx-toolbox/toctree_plus/workflows/mypy/badge.svg
 	:target: https://github.com/sphinx-toolbox/toctree_plus/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/toctree_plus/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/toctree_plus/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/toctree_plus/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/toctree_plus/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/sphinx-toolbox/toctree_plus/master?logo=coveralls
 	:target: https://coveralls.io/github/sphinx-toolbox/toctree_plus?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/sphinx-toolbox/toctree_plus?logo=codefactor
@@ -135,23 +135,23 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/toctree_plus
 	:target: https://github.com/sphinx-toolbox/toctree_plus/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/toctree_plus
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/toctree_plus/v0.6.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/toctree_plus/v0.6.1
 	:target: https://github.com/sphinx-toolbox/toctree_plus/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/toctree_plus
 	:target: https://github.com/sphinx-toolbox/toctree_plus/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/toctree_plus
 	:target: https://pypi.org/project/toctree_plus/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `toctree_plus-0.6.0/README.rst` & `toctree_plus-0.6.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/toctree_plus/latest?logo=read-the-docs
-	:target: https://toctree_plus.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/toctree-plus/latest?logo=read-the-docs
+	:target: https://toctree-plus.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/sphinx-toolbox/toctree_plus/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/sphinx-toolbox/toctree_plus/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/sphinx-toolbox/toctree_plus/workflows/Linux/badge.svg
@@ -53,16 +53,16 @@
 	:target: https://github.com/sphinx-toolbox/toctree_plus/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/sphinx-toolbox/toctree_plus/workflows/mypy/badge.svg
 	:target: https://github.com/sphinx-toolbox/toctree_plus/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/toctree_plus/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/toctree_plus/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/toctree_plus/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/toctree_plus/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/sphinx-toolbox/toctree_plus/master?logo=coveralls
 	:target: https://coveralls.io/github/sphinx-toolbox/toctree_plus?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/sphinx-toolbox/toctree_plus?logo=codefactor
@@ -96,23 +96,23 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/toctree_plus
 	:target: https://github.com/sphinx-toolbox/toctree_plus/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/toctree_plus
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/toctree_plus/v0.6.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/toctree_plus/v0.6.1
 	:target: https://github.com/sphinx-toolbox/toctree_plus/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/toctree_plus
 	:target: https://github.com/sphinx-toolbox/toctree_plus/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/toctree_plus
 	:target: https://pypi.org/project/toctree_plus/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `toctree_plus-0.6.0/sphinxcontrib/toctree_plus/__init__.py` & `toctree_plus-0.6.1/sphinxcontrib/toctree_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 from sphinx.transforms import SphinxContentsFilter
 from sphinx.util import logging, texescape
 from sphinx.writers.latex import LaTeXTranslator
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2021 Dominic Davis-Foster"
 __license__: str = "BSD"
-__version__: str = "0.6.0"
+__version__: str = "0.6.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["TocTreePlusCollector", "setup"]
 
 N = TypeVar('N')
 
 logger = logging.getLogger(__name__)
```

