# Comparing `tmp/extras_require-0.4.3.tar.gz` & `tmp/extras_require-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extras_require-0.4.3.tar", last modified: Sun May  8 15:52:18 2022, max compression
+gzip compressed data, was "extras_require-0.5.0.tar", last modified: Fri Apr 14 11:59:04 2023, max compression
```

## Comparing `extras_require-0.4.3.tar` & `extras_require-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0 runner    (1001) docker     (121)    10206 2022-05-08 15:52:18.524216 extras_require-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5301 2022-05-08 15:52:18.524216 extras_require-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     8300 2022-05-08 15:52:18.524216 extras_require-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-05-08 15:52:18.516216 extras_require-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-05-08 15:52:18.524216 extras_require-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7410 2022-05-08 15:51:45.011781 extras_require-0.4.3/sphinxcontrib/extras_require/directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-05-08 15:51:45.011781 extras_require-0.4.3/sphinxcontrib/extras_require/purger.py
--rw-r--r--   0 runner    (1001) docker     (121)     9327 2022-05-08 15:51:45.011781 extras_require-0.4.3/sphinxcontrib/extras_require/sources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-05-08 15:51:45.011781 extras_require-0.4.3/sphinxcontrib/extras_require/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-08 15:51:45.011781 extras_require-0.4.3/sphinxcontrib/extras_require/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    10259 2023-04-14 11:59:04.794059 extras_require-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-04-14 11:59:04.790059 extras_require-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-04-14 11:59:04.782059 extras_require-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     8302 2023-04-14 11:59:04.790059 extras_require-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-14 11:59:04.790059 extras_require-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2844 2023-04-14 11:58:36.674097 extras_require-0.5.0/sphinxcontrib/extras_require/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 11:58:36.674097 extras_require-0.5.0/sphinxcontrib/extras_require/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     9426 2023-04-14 11:58:36.674097 extras_require-0.5.0/sphinxcontrib/extras_require/sources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7410 2023-04-14 11:58:36.674097 extras_require-0.5.0/sphinxcontrib/extras_require/directive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-04-14 11:58:36.674097 extras_require-0.5.0/sphinxcontrib/extras_require/purger.py
```

### Comparing `extras_require-0.4.3/PKG-INFO` & `extras_require-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: extras-require
-Version: 0.4.3
+Version: 0.5.0
 Summary: Display a warning at the top of module documentation that it has additional requirements.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: BSD-3-Clause
 Keywords: documentation,requirements,sphinx,sphinx-extension
 Home-page: https://github.com/sphinx-toolbox/extras_require
 Project-URL: Issue Tracker, https://github.com/sphinx-toolbox/extras_require/issues
 Project-URL: Source Code, https://github.com/sphinx-toolbox/extras_require
-Project-URL: Documentation, https://extras_require.readthedocs.io/en/latest
+Project-URL: Documentation, https://extras-require.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,28 +20,29 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: docutils>=0.16
 Requires-Dist: domdf-python-tools>=0.7.1
 Requires-Dist: packaging>=20.4
 Requires-Dist: setuptools>=49.2.0
 Requires-Dist: shippinglabel>=0.10.0
-Requires-Dist: sphinx>=3.1.0
+Requires-Dist: sphinx>=3.3.0
 Requires-Dist: sphinx-prompt>=1.1.0
 Requires-Dist: sphinx-toolbox>=2.13.0
 Description-Content-Type: text/x-rst
 
 
 ================
 extras_require
@@ -70,16 +71,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/extras_require/latest?logo=read-the-docs
-	:target: https://extras_require.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/extras-require/latest?logo=read-the-docs
+	:target: https://extras-require.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/sphinx-toolbox/extras_require/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/sphinx-toolbox/extras_require/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/sphinx-toolbox/extras_require/workflows/Linux/badge.svg
@@ -98,16 +99,16 @@
 	:target: https://github.com/sphinx-toolbox/extras_require/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/sphinx-toolbox/extras_require/workflows/mypy/badge.svg
 	:target: https://github.com/sphinx-toolbox/extras_require/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/extras_require/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/extras_require/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/extras_require/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/extras_require/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/sphinx-toolbox/extras_require/master?logo=coveralls
 	:target: https://coveralls.io/github/sphinx-toolbox/extras_require?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/sphinx-toolbox/extras_require?logo=codefactor
@@ -141,23 +142,23 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/extras_require
 	:target: https://github.com/sphinx-toolbox/extras_require/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/extras_require
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/extras_require/v0.4.3
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/extras_require/v0.5.0
 	:target: https://github.com/sphinx-toolbox/extras_require/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/extras_require
 	:target: https://github.com/sphinx-toolbox/extras_require/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/extras_require
 	:target: https://pypi.org/project/extras_require/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `extras_require-0.4.3/pyproject.toml` & `extras_require-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "extras_require"
-version = "0.4.3"
+version = "0.5.0"
 description = "Display a warning at the top of module documentation that it has additional requirements."
 readme = "README.rst"
 keywords = [ "documentation", "requirements", "sphinx", "sphinx-extension",]
 dynamic = []
 dependencies = [
     "docutils>=0.16",
     "domdf-python-tools>=0.7.1",
     "packaging>=20.4",
     "setuptools>=49.2.0",
     "shippinglabel>=0.10.0",
-    "sphinx>=3.1.0",
+    "sphinx>=3.3.0",
     "sphinx-prompt>=1.1.0",
     "sphinx-toolbox>=2.13.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Documentation",
@@ -50,29 +51,29 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/sphinx-toolbox/extras_require"
 "Issue Tracker" = "https://github.com/sphinx-toolbox/extras_require/issues"
 "Source Code" = "https://github.com/sphinx-toolbox/extras_require"
-Documentation = "https://extras_require.readthedocs.io/en/latest"
+Documentation = "https://extras-require.readthedocs.io/en/latest"
 
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Software Development :: Documentation",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "BSD-3-Clause"
 package = "sphinxcontrib"
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
@@ -92,25 +93,25 @@
 package_root = "sphinxcontrib/extras_require"
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
     "sphinx_toolbox_experimental.needspace",
     "sphinx_toolbox_experimental.succinct_seealso",
     "sphinx_toolbox_experimental.autosummary_widths",
```

### Comparing `extras_require-0.4.3/README.rst` & `extras_require-0.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/extras_require/latest?logo=read-the-docs
-	:target: https://extras_require.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/extras-require/latest?logo=read-the-docs
+	:target: https://extras-require.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/sphinx-toolbox/extras_require/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/sphinx-toolbox/extras_require/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/sphinx-toolbox/extras_require/workflows/Linux/badge.svg
@@ -53,16 +53,16 @@
 	:target: https://github.com/sphinx-toolbox/extras_require/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/sphinx-toolbox/extras_require/workflows/mypy/badge.svg
 	:target: https://github.com/sphinx-toolbox/extras_require/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/extras_require/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/extras_require/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/extras_require/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/extras_require/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/sphinx-toolbox/extras_require/master?logo=coveralls
 	:target: https://coveralls.io/github/sphinx-toolbox/extras_require?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/sphinx-toolbox/extras_require?logo=codefactor
@@ -96,23 +96,23 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/extras_require
 	:target: https://github.com/sphinx-toolbox/extras_require/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/extras_require
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/extras_require/v0.4.3
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/extras_require/v0.5.0
 	:target: https://github.com/sphinx-toolbox/extras_require/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/extras_require
 	:target: https://github.com/sphinx-toolbox/extras_require/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/extras_require
 	:target: https://pypi.org/project/extras_require/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `extras_require-0.4.3/LICENSE` & `extras_require-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extras_require-0.4.3/sphinxcontrib/extras_require/directive.py` & `extras_require-0.5.0/sphinxcontrib/extras_require/directive.py`

 * *Files identical despite different names*

### Comparing `extras_require-0.4.3/sphinxcontrib/extras_require/purger.py` & `extras_require-0.5.0/sphinxcontrib/extras_require/purger.py`

 * *Files identical despite different names*

### Comparing `extras_require-0.4.3/sphinxcontrib/extras_require/sources.py` & `extras_require-0.5.0/sphinxcontrib/extras_require/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,17 @@
 				spec.loader.exec_module(__pkginfo__)
 				requirements = __pkginfo__.extras_require[extra]
 				return requirements
 				# TODO: handle extra not found
 
 	except ValueError:
 		pass
+	except SyntaxError as e:
+		if e.msg != "source code string cannot contain null bytes":
+			raise e
 
 	raise ImportError("Could not import __pkginfo__.py")
 
 
 requirements_from___pkginfo__ = requirements_from_pkginfo
```

### Comparing `extras_require-0.4.3/sphinxcontrib/extras_require/__init__.py` & `extras_require-0.5.0/sphinxcontrib/extras_require/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from sphinxcontrib.extras_require.directive import ExtrasRequireDirective
 from sphinxcontrib.extras_require.purger import extras_require_purger
 from sphinxcontrib.extras_require.sources import sources  # noqa: F401
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "BSD"
-__version__: str = "0.4.3"
+__version__: str = "0.5.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["extras_require_purger", "setup"]
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
 	"""
```

