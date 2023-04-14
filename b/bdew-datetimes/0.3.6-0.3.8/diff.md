# Comparing `tmp/bdew_datetimes-0.3.6.tar.gz` & `tmp/bdew_datetimes-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdew_datetimes-0.3.6.tar", last modified: Sun Apr  9 13:46:47 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `bdew_datetimes-0.3.6.tar` & `bdew_datetimes-0.3.8.tar`

### file list

```diff
@@ -1,38 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.492800 bdew_datetimes-0.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.488800 bdew_datetimes-0.3.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.488800 bdew_datetimes-0.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/workflows/linters.yml
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-09 13:46:47.492800 bdew_datetimes-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-09 13:46:47.492800 bdew_datetimes-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.488800 bdew_datetimes-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.488800 bdew_datetimes-0.3.6/src/bdew_datetimes/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/src/bdew_datetimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/src/bdew_datetimes/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/src/bdew_datetimes/german_strom_and_gas_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/src/bdew_datetimes/periods.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/src/bdew_datetimes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.492800 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-09 13:46:47.000000 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-09 13:46:47.000000 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:46:47.000000 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-09 13:46:47.000000 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 13:46:47.000000 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.492800 bdew_datetimes-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tests/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tests/test_german_strom_and_gas_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tests/test_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tox.ini
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/README.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/requirements.in
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/requirements.txt
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/tox.ini
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/workflows/black.yml
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/workflows/linters.yml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/workflows/release.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/_bdew_datetimes_version.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/bdew_datetimes/__init__.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/bdew_datetimes/calendar.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/bdew_datetimes/german_strom_and_gas_tag.py
+-rw-r--r--   0        0        0     8447 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/bdew_datetimes/periods.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/src/bdew_datetimes/py.typed
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6613 2020-02-02 00:00:00.000000 bdew_datetimes-0.3.8/PKG-INFO
```

### Comparing `bdew_datetimes-0.3.6/.github/dependabot.yml` & `bdew_datetimes-0.3.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.6/.github/workflows/linters.yml` & `bdew_datetimes-0.3.8/.github/workflows/linters.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.6/.github/workflows/packaging_test.yml` & `bdew_datetimes-0.3.8/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.6/.github/workflows/release.yml` & `bdew_datetimes-0.3.8/.github/workflows/release.yml`

 * *Files 3% similar despite different names*

```diff
@@ -43,18 +43,18 @@
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install setuptools setuptools-scm wheel twine
+          pip install build twine
       - name: Build a binary wheel and a source tarball
         run: |
-          python setup.py sdist bdist_wheel
+          python -m build
       - name: Publish distribution 📦 to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.TEST_PYPI_API_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
       - name: Publish distribution 📦 to PyPI
         if: startsWith(github.ref, 'refs/tags/v') # the tag name has to be v1.2.3 (with 1.2.3 being the semver)
```

### Comparing `bdew_datetimes-0.3.6/.github/workflows/unittests.yml` & `bdew_datetimes-0.3.8/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.6/.gitignore` & `bdew_datetimes-0.3.8/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -53,7 +53,9 @@
 # Dask
 dask-worker-space/
 
 # Editors
 .idea/
 .vscode/
 *.code-workspace
+
+src/_bdew_datetimes_version.py
```

### Comparing `bdew_datetimes-0.3.6/LICENSE` & `bdew_datetimes-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.6/PKG-INFO` & `bdew_datetimes-0.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: bdew_datetimes
-Version: 0.3.6
-Summary: Generate and work with holidays of the BDEW-Calendar for power and gas in Germany.
-Home-page: UNKNOWN
+Version: 0.3.8
+Summary: Generate and work with holidays of the BDEW-Calendar for power and gas in Germany
+Project-URL: Changelog, https://github.com/mj0nez/bdew-datetimes/releases
+Project-URL: Homepage, https://github.com/mj0nez/bdew-datetimes/
+Author: Konstantin Klein
+Author-email: Marcel Johannesmann <mj0nez@fn.de>
 License: MIT
-Platform: any
+License-File: LICENSE
+Keywords: bdew,edi@energy
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Office/Business :: Scheduling
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Localization
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+Requires-Dist: holidays>=0.16
+Requires-Dist: python-dateutil
+Requires-Dist: pytz>=2022.7.1
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # bdew_datetimes
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mj0nez/bdew-datetimes/packaging_test.yml?style=plastic)![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bdew-datetimes?style=plastic)![PyPI - License](https://img.shields.io/pypi/l/bdew-datetimes?style=plastic)![PyPI](https://img.shields.io/pypi/v/bdew-datetimes?style=plastic)
 
 A collection of utils to work with datetimes and holidays in the German energy
 market and is based on the [python-holiday](https://github.com/dr-prodigy/python-holidays) package.
 
 The implementation considers the publications of the **BDEW** (Bundesverband der Energie- und Wasserwirtschaft e. V.) and **EDI@Energy**, which provide boundaries and guidance for the data exchange on the german energy market. 
 
 ### Current highlights:
@@ -137,9 +140,7 @@
 
 Shifting holidays to the next weekday if they fall on a weekend is currently not considered.  
 
 
 ## License
 
 This library is licensed under the *MIT* license, see the [LICENSE file](LICENSE).
-
-
```

### Comparing `bdew_datetimes-0.3.6/README.md` & `bdew_datetimes-0.3.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # bdew_datetimes
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mj0nez/bdew-datetimes/packaging_test.yml?style=plastic)![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bdew-datetimes?style=plastic)![PyPI - License](https://img.shields.io/pypi/l/bdew-datetimes?style=plastic)![PyPI](https://img.shields.io/pypi/v/bdew-datetimes?style=plastic)
 
 A collection of utils to work with datetimes and holidays in the German energy
 market and is based on the [python-holiday](https://github.com/dr-prodigy/python-holidays) package.
 
 The implementation considers the publications of the **BDEW** (Bundesverband der Energie- und Wasserwirtschaft e. V.) and **EDI@Energy**, which provide boundaries and guidance for the data exchange on the german energy market. 
 
 ### Current highlights:
```

### Comparing `bdew_datetimes-0.3.6/requirements.txt` & `bdew_datetimes-0.3.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.6/src/bdew_datetimes/calendar.py` & `bdew_datetimes-0.3.8/src/bdew_datetimes/calendar.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.6/src/bdew_datetimes/german_strom_and_gas_tag.py` & `bdew_datetimes-0.3.8/src/bdew_datetimes/german_strom_and_gas_tag.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.6/src/bdew_datetimes/periods.py` & `bdew_datetimes-0.3.8/src/bdew_datetimes/periods.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.6/tox.ini` & `bdew_datetimes-0.3.8/tox.ini`

 * *Files identical despite different names*

