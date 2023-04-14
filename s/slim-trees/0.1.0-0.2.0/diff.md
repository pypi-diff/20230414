# Comparing `tmp/slim-trees-0.1.0.tar.gz` & `tmp/slim-trees-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slim-trees-0.1.0.tar", last modified: Tue Mar 28 21:47:50 2023, max compression
+gzip compressed data, was "slim-trees-0.2.0.tar", last modified: Fri Apr 14 10:59:07 2023, max compression
```

## Comparing `slim-trees-0.1.0.tar` & `slim-trees-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:47:50.141819 slim-trees-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-28 21:47:41.000000 slim-trees-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-28 21:47:41.000000 slim-trees-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-28 21:47:50.141819 slim-trees-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-28 21:47:41.000000 slim-trees-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-28 21:47:41.000000 slim-trees-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-28 21:47:50.141819 slim-trees-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:47:50.141819 slim-trees-0.1.0/slim_trees/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-28 21:47:41.000000 slim-trees-0.1.0/slim_trees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-28 21:47:41.000000 slim-trees-0.1.0/slim_trees/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-03-28 21:47:41.000000 slim-trees-0.1.0/slim_trees/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-03-28 21:47:41.000000 slim-trees-0.1.0/slim_trees/lgbm_booster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-03-28 21:47:41.000000 slim-trees-0.1.0/slim_trees/pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-03-28 21:47:41.000000 slim-trees-0.1.0/slim_trees/sklearn_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-28 21:47:41.000000 slim-trees-0.1.0/slim_trees/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 21:47:50.141819 slim-trees-0.1.0/slim_trees.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-28 21:47:50.000000 slim-trees-0.1.0/slim_trees.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-28 21:47:50.000000 slim-trees-0.1.0/slim_trees.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 21:47:50.000000 slim-trees-0.1.0/slim_trees.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-28 21:47:50.000000 slim-trees-0.1.0/slim_trees.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-28 21:47:50.000000 slim-trees-0.1.0/slim_trees.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:59:07.655280 slim-trees-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-14 10:58:54.000000 slim-trees-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 10:58:54.000000 slim-trees-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-14 10:59:07.655280 slim-trees-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-14 10:58:54.000000 slim-trees-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-14 10:58:54.000000 slim-trees-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-14 10:59:07.655280 slim-trees-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:59:07.651280 slim-trees-0.2.0/slim_trees/
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/lgbm_booster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/sklearn_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-14 10:58:54.000000 slim-trees-0.2.0/slim_trees/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:59:07.655280 slim-trees-0.2.0/slim_trees.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-14 10:59:07.000000 slim-trees-0.2.0/slim_trees.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-14 10:59:07.000000 slim-trees-0.2.0/slim_trees.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:59:07.000000 slim-trees-0.2.0/slim_trees.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 10:59:07.000000 slim-trees-0.2.0/slim_trees.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 10:59:07.000000 slim-trees-0.2.0/slim_trees.egg-info/top_level.txt
```

### Comparing `slim-trees-0.1.0/LICENSE` & `slim-trees-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slim-trees-0.1.0/pyproject.toml` & `slim-trees-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 [tool.mypy]
 python_version = "3.8"
 ignore_missing_imports = true
 no_implicit_optional = true
 check_untyped_defs = true
 
 [tool.tbump.version]
-current = "0.1.0"
+current = "0.2.0"
 regex = '''
   (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:\.(?P<extra>.+))?
 '''
 
 [[tool.tbump.field]]
 name = "extra"
 default = ""
```

### Comparing `slim-trees-0.1.0/setup.cfg` & `slim-trees-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `slim-trees-0.1.0/slim_trees/compression_utils.py` & `slim-trees-0.2.0/slim_trees/compression_utils.py`

 * *Files identical despite different names*

### Comparing `slim-trees-0.1.0/slim_trees/lgbm_booster.py` & `slim-trees-0.2.0/slim_trees/lgbm_booster.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 try:
     from lightgbm.basic import Booster
 except ImportError:
     print("LightGBM does not seem to be installed.")
     sys.exit(os.EX_CONFIG)
 
 
-def dump_lgbm(model: Any, file: BinaryIO):
+def dump(model: Any, file: BinaryIO):
     p = pickle.Pickler(file)
     p.dispatch_table = copyreg.dispatch_table.copy()
     p.dispatch_table[Booster] = _booster_pickle
     p.dump(model)
 
 
 def _booster_pickle(booster: Booster):
```

### Comparing `slim-trees-0.1.0/slim_trees/pickling.py` & `slim-trees-0.2.0/slim_trees/pickling.py`

 * *Files identical despite different names*

### Comparing `slim-trees-0.1.0/slim_trees/sklearn_tree.py` & `slim-trees-0.2.0/slim_trees/sklearn_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import copyreg
 import pickle
 from typing import Any, BinaryIO
 
 import numpy as np
 
 
-def dump_sklearn(model: Any, file: BinaryIO):
+def dump(model: Any, file: BinaryIO):
     p = pickle.Pickler(file)
     p.dispatch_table = copyreg.dispatch_table.copy()
     p.dispatch_table[Tree] = _tree_pickle
     p.dump(model)
 
 
 def _tree_pickle(tree):
```

