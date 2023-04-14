# Comparing `tmp/dask_histogram-2023.4.1.tar.gz` & `tmp/dask_histogram-2023.4.2.tar.gz`

## Comparing `dask_histogram-2023.4.1.tar` & `dask_histogram-2023.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/__init__.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/bins.py
--rw-r--r--   0        0        0    29278 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/boost.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/config.py
--rw-r--r--   0        0        0    39039 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/core.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/histogram.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/py.typed
--rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/routines.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/sizeof.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/typing.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/version.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/LICENSE
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/README.md
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/pyproject.toml
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/PKG-INFO
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/__init__.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/bins.py
+-rw-r--r--   0        0        0    29278 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/boost.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/config.py
+-rw-r--r--   0        0        0    39039 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/core.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/histogram.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/py.typed
+-rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/routines.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/sizeof.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/typing.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/version.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/LICENSE
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/README.md
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/PKG-INFO
```

### Comparing `dask_histogram-2023.4.1/src/dask_histogram/__init__.py` & `dask_histogram-2023.4.2/src/dask_histogram/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.1/src/dask_histogram/bins.py` & `dask_histogram-2023.4.2/src/dask_histogram/bins.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.1/src/dask_histogram/boost.py` & `dask_histogram-2023.4.2/src/dask_histogram/boost.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.1/src/dask_histogram/core.py` & `dask_histogram-2023.4.2/src/dask_histogram/core.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.1/src/dask_histogram/routines.py` & `dask_histogram-2023.4.2/src/dask_histogram/routines.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.1/src/dask_histogram/sizeof.py` & `dask_histogram-2023.4.2/src/dask_histogram/sizeof.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.1/.gitignore` & `dask_histogram-2023.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.1/LICENSE` & `dask_histogram-2023.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.1/README.md` & `dask_histogram-2023.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.1/pyproject.toml` & `dask_histogram-2023.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.1/PKG-INFO` & `dask_histogram-2023.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-histogram
-Version: 2023.4.1
+Version: 2023.4.2
 Summary: Histogramming with Dask.
 Project-URL: Homepage, https://github.com/dask-contrib/dask-histogram
 Project-URL: Documentation, https://dask-histogram.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-histogram/issues
 Author-email: Doug Davis <ddavis@ddavis.io>
 License: BSD-3-Clause
 License-File: LICENSE
```

