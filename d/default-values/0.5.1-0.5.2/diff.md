# Comparing `tmp/default_values-0.5.1.tar.gz` & `tmp/default_values-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "default_values-0.5.1.tar", last modified: Fri Apr  1 06:18:33 2022, max compression
+gzip compressed data, was "default_values-0.5.2.tar", last modified: Fri Apr 14 12:27:14 2023, max compression
```

## Comparing `default_values-0.5.1.tar` & `default_values-0.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-04-01 06:18:32.947298 default_values-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-04-01 06:18:32.955298 default_values-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4926 2022-04-01 06:18:32.955298 default_values-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     7490 2022-04-01 06:18:33.003298 default_values-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5853 2022-04-01 06:18:32.955298 default_values-0.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-04-01 06:17:54.871221 default_values-0.5.1/sphinxcontrib/default_values/demo.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 06:17:54.871221 default_values-0.5.1/sphinxcontrib/default_values/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    10171 2022-04-01 06:17:54.871221 default_values-0.5.1/sphinxcontrib/default_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7492 2023-04-14 12:27:14.699399 default_values-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4926 2023-04-14 12:27:14.699399 default_values-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-04-14 12:27:14.691399 default_values-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-04-14 12:27:14.699399 default_values-0.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-14 12:27:14.699399 default_values-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-04-14 12:26:43.915115 default_values-0.5.2/sphinxcontrib/default_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-04-14 12:26:43.915115 default_values-0.5.2/sphinxcontrib/default_values/demo.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 12:26:43.915115 default_values-0.5.2/sphinxcontrib/default_values/py.typed
```

### Comparing `default_values-0.5.1/LICENSE` & `default_values-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `default_values-0.5.1/pyproject.toml` & `default_values-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "default_values"
-version = "0.5.1"
+version = "0.5.2"
 description = "Sphinx extension to show default values in documentation."
 readme = "README.rst"
 keywords = [ "documentation", "sphinx",]
 dynamic = []
 dependencies = [ "docutils==0.16", "sphinx<3.6.0,>=3.2.0", "sphinx-jinja2-compat>=0.1.0",]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -40,15 +40,15 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/sphinx-toolbox/default_values"
 "Issue Tracker" = "https://github.com/sphinx-toolbox/default_values/issues"
 "Source Code" = "https://github.com/sphinx-toolbox/default_values"
-Documentation = "https://default_values.readthedocs.io/en/latest"
+Documentation = "https://default-values.readthedocs.io/en/latest"
 
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "Topic :: Documentation",
@@ -76,25 +76,25 @@
 package_root = "sphinxcontrib/default_values"
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
     "sphinx_toolbox_experimental.rst_field",
     "sphinx_toolbox_experimental.html_section",
     "sphinx_toolbox_experimental.autosummary_widths",
@@ -145,15 +145,15 @@
     "__new__",
     "__getnewargs__",
     "__abstractmethods__",
     "__hash__",
 ]
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
```

### Comparing `default_values-0.5.1/PKG-INFO` & `default_values-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: default-values
-Version: 0.5.1
+Version: 0.5.2
 Summary: Sphinx extension to show default values in documentation.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: documentation,sphinx
 Home-page: https://github.com/sphinx-toolbox/default_values
 Project-URL: Issue Tracker, https://github.com/sphinx-toolbox/default_values/issues
 Project-URL: Source Code, https://github.com/sphinx-toolbox/default_values
-Project-URL: Documentation, https://default_values.readthedocs.io/en/latest
+Project-URL: Documentation, https://default-values.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -81,16 +81,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/default_values/latest?logo=read-the-docs
-	:target: https://default_values.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/default-values/latest?logo=read-the-docs
+	:target: https://default-values.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/sphinx-toolbox/default_values/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/sphinx-toolbox/default_values/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/sphinx-toolbox/default_values/workflows/Linux/badge.svg
@@ -109,16 +109,16 @@
 	:target: https://github.com/sphinx-toolbox/default_values/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/sphinx-toolbox/default_values/workflows/mypy/badge.svg
 	:target: https://github.com/sphinx-toolbox/default_values/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/default_values/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/default_values/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/default_values/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/default_values/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/sphinx-toolbox/default_values/master?logo=coveralls
 	:target: https://coveralls.io/github/sphinx-toolbox/default_values?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/sphinx-toolbox/default_values?logo=codefactor
@@ -152,23 +152,23 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/default_values
 	:target: https://github.com/sphinx-toolbox/default_values/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/default_values
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/default_values/v0.5.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/default_values/v0.5.2
 	:target: https://github.com/sphinx-toolbox/default_values/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/default_values
 	:target: https://github.com/sphinx-toolbox/default_values/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/default_values
 	:target: https://pypi.org/project/default_values/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `default_values-0.5.1/README.rst` & `default_values-0.5.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/default_values/latest?logo=read-the-docs
-	:target: https://default_values.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/default-values/latest?logo=read-the-docs
+	:target: https://default-values.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/sphinx-toolbox/default_values/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/sphinx-toolbox/default_values/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/sphinx-toolbox/default_values/workflows/Linux/badge.svg
@@ -70,16 +70,16 @@
 	:target: https://github.com/sphinx-toolbox/default_values/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/sphinx-toolbox/default_values/workflows/mypy/badge.svg
 	:target: https://github.com/sphinx-toolbox/default_values/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/default_values/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/sphinx-toolbox/default_values/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/default_values/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/sphinx-toolbox/default_values/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/sphinx-toolbox/default_values/master?logo=coveralls
 	:target: https://coveralls.io/github/sphinx-toolbox/default_values?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/sphinx-toolbox/default_values?logo=codefactor
@@ -113,23 +113,23 @@
 .. |license| image:: https://img.shields.io/github/license/sphinx-toolbox/default_values
 	:target: https://github.com/sphinx-toolbox/default_values/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/sphinx-toolbox/default_values
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/default_values/v0.5.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/sphinx-toolbox/default_values/v0.5.2
 	:target: https://github.com/sphinx-toolbox/default_values/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/sphinx-toolbox/default_values
 	:target: https://github.com/sphinx-toolbox/default_values/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/default_values
 	:target: https://pypi.org/project/default_values/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `default_values-0.5.1/sphinxcontrib/default_values/demo.py` & `default_values-0.5.2/sphinxcontrib/default_values/demo.py`

 * *Files identical despite different names*

### Comparing `default_values-0.5.1/sphinxcontrib/default_values/__init__.py` & `default_values-0.5.2/sphinxcontrib/default_values/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 	# attrs is used in a way that it is only required in situations
 	# where it is available to import, so its fine to do this.
 	pass
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT"
-__version__: str = "0.5.1"
+__version__: str = "0.5.2"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = [
 		"process_docstring",
 		"process_default_format",
 		"setup",
 		"get_class_defaults",
@@ -70,22 +70,22 @@
 		"format_default_value",
 		]
 
 default_regex: Pattern = re.compile("^:(?i:default) ")
 """
 Regular expression to match default values declared in docstrings.
 
-.. versionchanged:: 0.5.1  Change to be case insensitive.
+.. versionchanged:: 0.5.2  Change to be case insensitive.
 """
 
 no_default_regex: Pattern = re.compile("^:(?i:no[-_]default) ")
 """
 Regular expression to match fields in docstrings to suppress default values.
 
-.. versionchanged:: 0.5.1  Change to be case insensitive.
+.. versionchanged:: 0.5.2  Change to be case insensitive.
 """
 
 # ref: sphinx.domains.python.PyObject.doc_field_types
 _fields = '|'.join([
 		"param",
 		"parameter",
 		"arg",
@@ -108,15 +108,15 @@
 	return string
 
 
 def format_default_value(value: Any) -> Optional[str]:
 	"""
 	Format the value as a string.
 
-	.. versionadded:: 0.5.1
+	.. versionadded:: 0.5.2
 
 	:param value:
 	"""
 
 	if value is not inspect.Signature.empty and value is not Ellipsis:
 
 		if isinstance(value, ModuleType):
```

