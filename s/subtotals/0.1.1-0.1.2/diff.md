# Comparing `tmp/subtotals-0.1.1.tar.gz` & `tmp/subtotals-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtotals-0.1.1.tar", last modified: Fri Apr 14 08:46:31 2023, max compression
+gzip compressed data, was "subtotals-0.1.2.tar", last modified: Fri Apr 14 08:49:54 2023, max compression
```

## Comparing `subtotals-0.1.1.tar` & `subtotals-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1799 2023-04-14 05:33:33.568111 subtotals-0.1.1/.gitignore
--rw-r--r--   0        0        0     1095 2023-04-14 04:59:05.593133 subtotals-0.1.1/LICENSE
--rw-r--r--   0        0        0     3145 2023-04-14 08:42:18.356440 subtotals-0.1.1/README.md
--rw-r--r--   0        0        0      432 2023-04-14 08:44:32.237632 subtotals-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1262 2023-04-14 08:46:28.282545 subtotals-0.1.1/subtotals.py
--rw-r--r--   0        0        0      900 2023-04-14 06:25:04.702421 subtotals-0.1.1/tests/sales.csv
--rw-r--r--   0        0        0     1239 2023-04-14 06:07:38.385392 subtotals-0.1.1/tests/test_subtotals.py
--rw-r--r--   0        0        0     3465 1970-01-01 00:00:00.000000 subtotals-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-04-14 05:33:33.568111 subtotals-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1095 2023-04-14 04:59:05.593133 subtotals-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3199 2023-04-14 08:49:01.777411 subtotals-0.1.2/README.md
+-rw-r--r--   0        0        0      432 2023-04-14 08:44:32.237632 subtotals-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1270 2023-04-14 08:49:21.281215 subtotals-0.1.2/subtotals.py
+-rw-r--r--   0        0        0      900 2023-04-14 06:25:04.702421 subtotals-0.1.2/tests/sales.csv
+-rw-r--r--   0        0        0     1239 2023-04-14 06:07:38.385392 subtotals-0.1.2/tests/test_subtotals.py
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 subtotals-0.1.2/PKG-INFO
```

### Comparing `subtotals-0.1.1/.gitignore` & `subtotals-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `subtotals-0.1.1/LICENSE` & `subtotals-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `subtotals-0.1.1/README.md` & `subtotals-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 python3 -m pip install subtotals
 ```
 
 subtotals requires Python 3 or above.
 
 ## Usage
 
-If you have a [sales.csv](tests/sales) like this:
+If you have a [sales.csv](https://github.com/gramener/subtotals/blob/master/tests/sales.csv) like this:
 
 ```text
 country    city              product   sales   growth
 India      Hyderabad         Biscuit   866.1   -0.270
 India      Hyderabad         Cake       26.4   -0.242
 India      Hyderabad         Cream      38.3   -0.291
 India      Hyderabad         Eggs      513.7   -0.113
```

### Comparing `subtotals-0.1.1/subtotals.py` & `subtotals-0.1.2/subtotals.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-'''Generate subtotals for Pandas DataFrames.'''
+'''Generate groupby subtotals for Pandas DataFrames.'''
 
 import pandas as pd
 from typing import Union, List, Dict, Callable
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 
 def groupby(
     data: pd.DataFrame,
     by: List[str],
     agg: Union[Callable, str, List[Union[str, Callable]], Dict[str, Union[str, Callable]]],
     margins_name: str = 'Total',
```

### Comparing `subtotals-0.1.1/tests/sales.csv` & `subtotals-0.1.2/tests/sales.csv`

 * *Files identical despite different names*

### Comparing `subtotals-0.1.1/tests/test_subtotals.py` & `subtotals-0.1.2/tests/test_subtotals.py`

 * *Files identical despite different names*

### Comparing `subtotals-0.1.1/PKG-INFO` & `subtotals-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: subtotals
-Version: 0.1.1
-Summary: Generate subtotals for Pandas DataFrames.
+Version: 0.1.2
+Summary: Generate groupby subtotals for Pandas DataFrames.
 Author-email: S Anand <root.node@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pandas
 Project-URL: Home, https://github.com/gramener/subtotals
 
 <!-- markdownlint-disable first-line-h1 -->
@@ -18,15 +18,15 @@
 python3 -m pip install subtotals
 ```
 
 subtotals requires Python 3 or above.
 
 ## Usage
 
-If you have a [sales.csv](tests/sales) like this:
+If you have a [sales.csv](https://github.com/gramener/subtotals/blob/master/tests/sales.csv) like this:
 
 ```text
 country    city              product   sales   growth
 India      Hyderabad         Biscuit   866.1   -0.270
 India      Hyderabad         Cake       26.4   -0.242
 India      Hyderabad         Cream      38.3   -0.291
 India      Hyderabad         Eggs      513.7   -0.113
```

