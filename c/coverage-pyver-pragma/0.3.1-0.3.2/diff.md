# Comparing `tmp/coverage_pyver_pragma-0.3.1.tar.gz` & `tmp/coverage_pyver_pragma-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage_pyver_pragma-0.3.1.tar", last modified: Tue Feb  8 22:03:32 2022, max compression
+gzip compressed data, was "coverage_pyver_pragma-0.3.2.tar", last modified: Fri Apr 14 14:46:35 2023, max compression
```

## Comparing `coverage_pyver_pragma-0.3.1.tar` & `coverage_pyver_pragma-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-02-08 22:03:31.855249 coverage_pyver_pragma-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-02-08 22:03:31.863248 coverage_pyver_pragma-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4582 2022-02-08 22:03:31.863248 coverage_pyver_pragma-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     7465 2022-02-08 22:03:31.999248 coverage_pyver_pragma-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5893 2022-02-08 22:03:31.863248 coverage_pyver_pragma-0.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10107 2022-02-08 22:02:37.775375 coverage_pyver_pragma-0.3.1/coverage_pyver_pragma/grammar.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-08 22:02:37.775375 coverage_pyver_pragma-0.3.1/coverage_pyver_pragma/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3185 2022-02-08 22:02:37.775375 coverage_pyver_pragma-0.3.1/coverage_pyver_pragma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7518 2023-04-14 14:46:35.075218 coverage_pyver_pragma-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4612 2023-04-14 14:46:35.075218 coverage_pyver_pragma-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-14 14:46:35.067218 coverage_pyver_pragma-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5895 2023-04-14 14:46:35.075218 coverage_pyver_pragma-0.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-14 14:46:35.075218 coverage_pyver_pragma-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3256 2023-04-14 14:46:05.682897 coverage_pyver_pragma-0.3.2/coverage_pyver_pragma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 14:46:05.682897 coverage_pyver_pragma-0.3.2/coverage_pyver_pragma/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    10384 2023-04-14 14:46:05.682897 coverage_pyver_pragma-0.3.2/coverage_pyver_pragma/grammar.py
```

### Comparing `coverage_pyver_pragma-0.3.1/LICENSE` & `coverage_pyver_pragma-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coverage_pyver_pragma-0.3.1/pyproject.toml` & `coverage_pyver_pragma-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "coverage_pyver_pragma"
-version = "0.3.1"
+version = "0.3.2"
 description = "Plugin for Coverage.py to selectively ignore branches depending on the Python version."
 readme = "README.rst"
 keywords = [ "coverage",]
 dynamic = []
 dependencies = [ "coverage>=5.5", "domdf-python-tools>=2.8.0", "packaging>=20.9", "pyparsing>=2.4.7",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
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
     "Topic :: Utilities",
@@ -37,24 +38,24 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/python-coincidence/coverage_pyver_pragma"
 "Issue Tracker" = "https://github.com/python-coincidence/coverage_pyver_pragma/issues"
 "Source Code" = "https://github.com/python-coincidence/coverage_pyver_pragma"
-Documentation = "https://coverage_pyver_pragma.readthedocs.io/en/latest"
+Documentation = "https://coverage-pyver-pragma.readthedocs.io/en/latest"
 
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 
 [tool.mkrecipe]
 extras = "all"
 conda-channels = [ "conda-forge", "domdfcoding",]
@@ -69,31 +70,31 @@
 package_root = "coverage_pyver_pragma"
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
-    "sphinx_toolbox_experimental.autosummary_widths",
-    "sphinx_toolbox_experimental.needspace",
+    "sphinx_toolbox.more_autosummary.column_widths",
+    "sphinx_favicon",
 ]
 sphinxemoji_style = "twemoji"
 gitstamp_fmt = "%d %b %Y"
 templates_path = [ "_templates",]
 html_static_path = [ "_static",]
 source_suffix = ".rst"
 master_doc = "index"
```

### Comparing `coverage_pyver_pragma-0.3.1/PKG-INFO` & `coverage_pyver_pragma-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: coverage-pyver-pragma
-Version: 0.3.1
+Version: 0.3.2
 Summary: Plugin for Coverage.py to selectively ignore branches depending on the Python version.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: coverage
 Home-page: https://github.com/python-coincidence/coverage_pyver_pragma
 Project-URL: Issue Tracker, https://github.com/python-coincidence/coverage_pyver_pragma/issues
 Project-URL: Source Code, https://github.com/python-coincidence/coverage_pyver_pragma
-Project-URL: Documentation, https://coverage_pyver_pragma.readthedocs.io/en/latest
+Project-URL: Documentation, https://coverage-pyver-pragma.readthedocs.io/en/latest
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
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
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: coverage>=5.5
 Requires-Dist: domdf-python-tools>=2.8.0
@@ -63,16 +64,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/coverage_pyver_pragma/latest?logo=read-the-docs
-	:target: https://coverage_pyver_pragma.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/coverage-pyver-pragma/latest?logo=read-the-docs
+	:target: https://coverage-pyver-pragma.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/python-coincidence/coverage_pyver_pragma/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/python-coincidence/coverage_pyver_pragma/workflows/Linux/badge.svg
@@ -91,16 +92,16 @@
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/python-coincidence/coverage_pyver_pragma/workflows/mypy/badge.svg
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/python-coincidence/coverage_pyver_pragma/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/python-coincidence/coverage_pyver_pragma/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/python-coincidence/coverage_pyver_pragma/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/python-coincidence/coverage_pyver_pragma/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/python-coincidence/coverage_pyver_pragma/master?logo=coveralls
 	:target: https://coveralls.io/github/python-coincidence/coverage_pyver_pragma?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/python-coincidence/coverage_pyver_pragma?logo=codefactor
@@ -134,23 +135,23 @@
 .. |license| image:: https://img.shields.io/github/license/python-coincidence/coverage_pyver_pragma
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/python-coincidence/coverage_pyver_pragma
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/python-coincidence/coverage_pyver_pragma/v0.3.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-coincidence/coverage_pyver_pragma/v0.3.2
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/python-coincidence/coverage_pyver_pragma
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/coverage_pyver_pragma
 	:target: https://pypi.org/project/coverage_pyver_pragma/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `coverage_pyver_pragma-0.3.1/README.rst` & `coverage_pyver_pragma-0.3.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/coverage_pyver_pragma/latest?logo=read-the-docs
-	:target: https://coverage_pyver_pragma.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/coverage-pyver-pragma/latest?logo=read-the-docs
+	:target: https://coverage-pyver-pragma.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/python-coincidence/coverage_pyver_pragma/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/python-coincidence/coverage_pyver_pragma/workflows/Linux/badge.svg
@@ -54,16 +54,16 @@
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/python-coincidence/coverage_pyver_pragma/workflows/mypy/badge.svg
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/python-coincidence/coverage_pyver_pragma/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/python-coincidence/coverage_pyver_pragma/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/python-coincidence/coverage_pyver_pragma/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/python-coincidence/coverage_pyver_pragma/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/python-coincidence/coverage_pyver_pragma/master?logo=coveralls
 	:target: https://coveralls.io/github/python-coincidence/coverage_pyver_pragma?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/python-coincidence/coverage_pyver_pragma?logo=codefactor
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/python-coincidence/coverage_pyver_pragma
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/python-coincidence/coverage_pyver_pragma
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/python-coincidence/coverage_pyver_pragma/v0.3.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/python-coincidence/coverage_pyver_pragma/v0.3.2
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/python-coincidence/coverage_pyver_pragma
 	:target: https://github.com/python-coincidence/coverage_pyver_pragma/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/coverage_pyver_pragma
 	:target: https://pypi.org/project/coverage_pyver_pragma/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `coverage_pyver_pragma-0.3.1/coverage_pyver_pragma/grammar.py` & `coverage_pyver_pragma-0.3.2/coverage_pyver_pragma/grammar.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,18 @@
 
 	\clearpage
 
 API Reference
 ----------------
 
 .. automodulesumm:: coverage_pyver_pragma.grammar
+
+.. autovariable:: GRAMMAR
+	:no-value:
+
 """  # noqa: D400
 #
 #  Copyright © 2021 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
@@ -135,15 +139,15 @@
 import platform
 import sys
 
 # 3rd party
 import packaging.specifiers
 from domdf_python_tools.doctools import prettify_docstrings
 from domdf_python_tools.stringlist import DelimitedList
-from pyparsing import (  # type: ignore
+from pyparsing import (
 		CaselessKeyword,
 		CaselessLiteral,
 		Combine,
 		Group,
 		Literal,
 		OneOrMore,
 		Optional,
@@ -152,34 +156,36 @@
 		Word,
 		infixNotation,
 		nums,
 		oneOf,
 		opAssoc
 		)
 
-__all__ = [
+__all__ = (
 		"ImplementationTag",
 		"LogicalAND",
 		"LogicalNOT",
 		"LogicalOR",
 		"LogicalOp",
 		"PlatformTag",
 		"VersionTag",
 		"VERSION_TAG",
 		"PLATFORM_TAG",
 		"IMPLEMENTATION_TAG",
 		"GRAMMAR",
-		]
+		)
 
 # This ensures coverage.py records the correct coverage for these modules
 # when they are under test
 
+# pylint: disable=loop-global-usage,dotted-import-in-loop
 for module in [m for m in sys.modules if m.startswith("domdf_python_tools")]:  # pragma: no cover (macOS)
 	if module in sys.modules:
 		del sys.modules[module]
+# pylint: enable=loop-global-usage,dotted-import-in-loop
 
 PYTHON_VERSION = os.environ.get("COV_PYTHON_VERSION", '.'.join(platform.python_version_tuple()[:2]))
 PLATFORM = os.environ.get("COV_PLATFORM", platform.system()).casefold()
 PYTHON_IMPLEMENTATION = os.environ.get("COV_PYTHON_IMPLEMENTATION", platform.python_implementation()).casefold()
 
 
 @prettify_docstrings
@@ -241,22 +247,24 @@
 	.. parsed-literal::
 
 		Windows
 		Linux
 		Darwin  # macOS
 		Java
 
+	.. latex:clearpage::
+
 	If the current platform cannot be determined all strings are treated as :py:obj:`True`.
 
 	:param tokens:
 	"""
 
 	__slots__ = ()
 
-	def __new__(cls, tokens: ParseResults):  # noqa: D102
+	def __new__(cls, tokens: ParseResults) -> "PlatformTag":  # noqa: D102
 		return super().__new__(cls, str(tokens["platform"]))
 
 	def __repr__(self) -> str:  # pragma: no cover
 		return f"<{self.__class__.__name__}({str(self)!r})>"
 
 	def __bool__(self) -> bool:
 		if not PLATFORM:  # pragma: no cover
@@ -285,15 +293,15 @@
 	:param tokens:
 
 	.. latex:vspace:: -10px
 	"""
 
 	__slots__ = ()
 
-	def __new__(cls, tokens: ParseResults):  # noqa: D102
+	def __new__(cls, tokens: ParseResults) -> "ImplementationTag":  # noqa: D102
 		return super().__new__(cls, str(tokens["implementation"]))
 
 	def __repr__(self) -> str:  # pragma: no cover
 		return f"<{self.__class__.__name__}({str(self)!r})>"
 
 	def __bool__(self) -> bool:
 		return PYTHON_IMPLEMENTATION == self.casefold()
@@ -306,15 +314,15 @@
 
 	:param tokens:
 	"""
 
 	def __init__(self, tokens: ParseResults):
 		self.tokens = DelimitedList(tokens[0])
 
-	def __format__(self, format_spec):
+	def __format__(self, format_spec: str) -> str:
 		return self.tokens.__format__(format_spec)
 
 	def __getitem__(self, item):
 		return self.tokens[item]
 
 	def __str__(self) -> str:
 		return f"[{self:, }]"
@@ -327,39 +335,39 @@
 class LogicalAND(LogicalOp):
 	"""
 	Represents the ``AND`` logical operator.
 
 	:param tokens:
 	"""
 
-	def __bool__(self):
+	def __bool__(self) -> bool:
 		return bool(self[0]) and bool(self[2])
 
 
 @prettify_docstrings
 class LogicalOR(LogicalOp):
 	"""
 	Represents the ``OR`` logical operator.
 
 	:param tokens:
 	"""
 
-	def __bool__(self):
+	def __bool__(self) -> bool:
 		return bool(self[0]) or bool(self[2])
 
 
 @prettify_docstrings
 class LogicalNOT(LogicalOp):
 	"""
 	Represents the ``NOT / !`` logical operator.
 
 	:param tokens:
 	"""
 
-	def __bool__(self):
+	def __bool__(self) -> bool:
 		return not bool(self[1])
 
 
 # Logical operators
 AND = CaselessKeyword("and")
 OR = CaselessKeyword("or")
 NOT = CaselessKeyword("not") | Literal('!')
@@ -370,15 +378,15 @@
 PLUS = Literal('+').setResultsName("plus")
 
 LESS_THAN_EQUAL = "<="
 LESS_THAN = '<'
 GREATER_THAN_EQUAL = ">="
 GREATER_THAN = '>'
 
-OPS = [LESS_THAN, LESS_THAN_EQUAL, GREATER_THAN, GREATER_THAN_EQUAL]
+OPS = [LESS_THAN, LESS_THAN_EQUAL, GREATER_THAN, GREATER_THAN_EQUAL]  # pylint: disable=use-tuple-over-list
 COMPARATOR = Optional(oneOf(' '.join(OPS))).setResultsName("comparator")
 
 VERSION = Combine(CaselessLiteral("py") + Word(nums)).setResultsName("version")
 VERSION_TAG = Group(COMPARATOR + VERSION + Optional(PLUS)).setResultsName("version")
 VERSION_TAG.setParseAction(VersionTag)
 
 # Platforms (Windows, !Linux)
```

### Comparing `coverage_pyver_pragma-0.3.1/coverage_pyver_pragma/__init__.py` & `coverage_pyver_pragma-0.3.2/coverage_pyver_pragma/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,31 +26,32 @@
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 # stdlib
 import functools
 import re
 from contextlib import suppress
+from typing import Set
 
 # 3rd party
-import coverage.python  # type: ignore
-import pyparsing  # type: ignore
-from coverage.config import DEFAULT_EXCLUDE  # type: ignore
-from coverage.misc import join_regex  # type: ignore
+import coverage.python  # type: ignore[import]
+import pyparsing
+from coverage.config import DEFAULT_EXCLUDE  # type: ignore[import]
+from coverage.misc import join_regex  # type: ignore[import]
 
 # this package
 from coverage_pyver_pragma.grammar import GRAMMAR
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020-2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.3.1"
+__version__: str = "0.3.2"
 __email__: str = "dominic@davis-foster.co.uk"
 
-__all__ = ["DSL_EXCLUDE", "evaluate_exclude"]
+__all__ = ("DSL_EXCLUDE", "evaluate_exclude")
 
 DSL_EXCLUDE = re.compile(r'.*#\s*(?:pragma|PRAGMA)[:\s]?\s*(?:no|NO)\s*(?:cover|COVER)\s*\((.*)\)')
 """
 Compiled regular expression to match comments in the ``# pragma: no cover (XXX)``,
 where ``XXX`` is an expression to be evaluated to determine whether the line
 should be excluded from coverage.
 
@@ -69,24 +70,25 @@
 	"""
 
 	return all(list(GRAMMAR.parseString(expression.lower(), parseAll=True)))
 
 
 class PythonParser(coverage.python.PythonParser):
 
-	def lines_matching(self, *regexes):
+	def lines_matching(self, *regexes) -> Set[int]:
 
 		combined = join_regex([*regexes, *DEFAULT_EXCLUDE])
 
 		regex_c = re.compile(combined)
 		matches = set()
+		exclude = DSL_EXCLUDE
 
 		for idx, ltext in enumerate(self.lines, start=1):
 
-			dsl_m = DSL_EXCLUDE.match(ltext)
+			dsl_m = exclude.match(ltext)
 
 			# Check if it matches the DSL regex:
 			if dsl_m:
 				exclude_source = dsl_m.group(1)
 
 				with suppress(pyparsing.ParseBaseException):
 					if evaluate_exclude(exclude_source):
@@ -96,9 +98,9 @@
 
 			if regex_c.search(ltext):
 				matches.add(idx)
 
 		return matches
 
 
-def coverage_init(*args, **kwargs):
+def coverage_init(*args, **kwargs) -> None:
 	coverage.python.PythonParser.lines_matching = PythonParser.lines_matching
```

