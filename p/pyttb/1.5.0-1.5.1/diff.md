# Comparing `tmp/pyttb-1.5.0.tar.gz` & `tmp/pyttb-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttb-1.5.0.tar", last modified: Sun Mar 19 18:38:40 2023, max compression
+gzip compressed data, was "pyttb-1.5.1.tar", last modified: Fri Apr 14 21:56:23 2023, max compression
```

## Comparing `pyttb-1.5.0.tar` & `pyttb-1.5.1.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:38:40.545967 pyttb-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-19 18:38:20.000000 pyttb-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-19 18:38:40.545967 pyttb-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-19 18:38:20.000000 pyttb-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:38:40.541967 pyttb-1.5.0/pyttb/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/cp_als.py
--rw-r--r--   0 runner    (1001) docker     (123)    58614 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/cp_apr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/hosvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/import_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/khatrirao.py
--rw-r--r--   0 runner    (1001) docker     (123)    75671 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/ktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/pyttb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/sptenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    85192 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/sptensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/sptensor3.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/sumtensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/symktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/symtensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/tenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    57563 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17952 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/ttensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-03-19 18:38:20.000000 pyttb-1.5.0/pyttb/tucker_als.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:38:40.541967 pyttb-1.5.0/pyttb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-19 18:38:40.000000 pyttb-1.5.0/pyttb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-19 18:38:40.000000 pyttb-1.5.0/pyttb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 18:38:40.000000 pyttb-1.5.0/pyttb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-19 18:38:40.000000 pyttb-1.5.0/pyttb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-19 18:38:40.000000 pyttb-1.5.0/pyttb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 18:38:40.545967 pyttb-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-19 18:38:20.000000 pyttb-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 18:38:40.545967 pyttb-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_cp_als.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_cp_apr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_hosvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_import_export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_khatrirao.py
--rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_ktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_pyttb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    64544 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_sptensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_tenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    55950 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_ttensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-03-19 18:38:20.000000 pyttb-1.5.0/tests/test_tucker_als.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:23.045105 pyttb-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-14 21:56:00.000000 pyttb-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 21:56:23.045105 pyttb-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-14 21:56:00.000000 pyttb-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:23.041105 pyttb-1.5.1/pyttb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/cp_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58614 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/cp_apr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/hosvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/khatrirao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75671 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/ktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/pyttb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/sptenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90402 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/sptensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/sptensor3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/sumtensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/symktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/symtensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/tenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57312 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17952 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/ttensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/tucker_als.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:23.041105 pyttb-1.5.1/pyttb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 21:56:23.000000 pyttb-1.5.1/pyttb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-14 21:56:23.000000 pyttb-1.5.1/pyttb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:56:23.000000 pyttb-1.5.1/pyttb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 21:56:23.000000 pyttb-1.5.1/pyttb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 21:56:23.000000 pyttb-1.5.1/pyttb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:56:23.045105 pyttb-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:23.045105 pyttb-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_cp_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_cp_apr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_hosvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_import_export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_khatrirao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_ktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16303 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_pyttb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66581 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_sptensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_tenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55950 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_ttensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_tucker_als.py
```

### Comparing `pyttb-1.5.0/LICENSE` & `pyttb-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/PKG-INFO` & `pyttb-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyttb
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python Tensor Toolbox
-Home-page: 
-Author: Daniel M. Dunlavy
+Author: Nick Johnson
 Author-email: "Daniel M. Dunlavy" <dmdunla@sandia.gov>
 License: BSD 2-Clause License
 Project-URL: homepage, https://github.com/sandialabs/pyttb
 Project-URL: coverage, https://coveralls.io/github/sandialabs/pyttb
 Project-URL: documentation, https://pyttb.readthedocs.io
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: testing
+Provides-Extra: dev
+Provides-Extra: doc
 License-File: LICENSE
 
 ```
 Copyright 2022 National Technology & Engineering Solutions of Sandia,
 LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 U.S. Government retains certain rights in this software.
 ```
```

### Comparing `pyttb-1.5.0/README.md` & `pyttb-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyproject.toml` & `pyttb-1.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 name = "pyttb"
-version = "1.5.0"
+dynamic = ["version"]
 description = "Python Tensor Toolbox"
 authors = [
   {name="Daniel M. Dunlavy", email="dmdunla@sandia.gov"},
+  {name="Nick Johnson"},
 ]
 license = { text="BSD 2-Clause License" }
 readme = "README.md"
 requires-python = ">=3.8"
 
 dependencies = [
     "numpy",
@@ -22,14 +23,33 @@
 ]
 
 [project.urls]
 homepage = "https://github.com/sandialabs/pyttb"
 coverage = "https://coveralls.io/github/sandialabs/pyttb"
 documentation = "https://pyttb.readthedocs.io"
 
+[project.optional-dependencies]
+dev = [
+    "black",
+    "isort",
+    "pylint",
+    "mypy",
+    "pytest",
+    "pytest-cov",
+]
+doc = [
+    "sphinx_rtd_theme",
+]
+
+[tool.setuptools]
+packages = ["pyttb"]
+
+[tool.setuptools.dynamic]
+version = {attr = "pyttb.__version__"}
+
 [build-system]
 requires = ["setuptools>=61.0", "numpy", "numpy_groupies", "scipy", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.isort]
 profile = "black"
```

### Comparing `pyttb-1.5.0/pyttb/__init__.py` & `pyttb-1.5.1/pyttb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
 
-__version__ = "1.3.8"
+__version__ = "1.5.1"
 
 import warnings
 
 from pyttb.cp_als import cp_als
 from pyttb.cp_apr import *
 from pyttb.export_data import export_data
 from pyttb.hosvd import hosvd
```

### Comparing `pyttb-1.5.0/pyttb/cp_als.py` & `pyttb-1.5.1/pyttb/cp_als.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb/cp_apr.py` & `pyttb-1.5.1/pyttb/cp_apr.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb/export_data.py` & `pyttb-1.5.1/pyttb/export_data.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb/hosvd.py` & `pyttb-1.5.1/pyttb/hosvd.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb/import_data.py` & `pyttb-1.5.1/pyttb/import_data.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb/khatrirao.py` & `pyttb-1.5.1/pyttb/khatrirao.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb/ktensor.py` & `pyttb-1.5.1/pyttb/ktensor.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb/pyttb_utils.py` & `pyttb-1.5.1/pyttb/pyttb_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
-
+"""PYTTB shared utilities across tensor types"""
 from inspect import signature
 from typing import Optional, Tuple, overload
 
 import numpy as np
-import scipy.sparse as sparse
 
 import pyttb as ttb
 
 
 def tt_to_dense_matrix(tensorInstance, mode, transpose=False):
     """
-    Helper function to unwrap tensor into dense matrix, should replace the core need for tenmat
+    Helper function to unwrap tensor into dense matrix, should replace the core need
+    for tenmat
 
     Parameters
     ----------
     tensorInstance: :class:`pyttb.tensor` or :class:`pyttb.tensor`
         Ktensor->matrix is supported but the inverse is not
     mode: int
         Mode around which to unwrap tensor
@@ -42,15 +42,16 @@
     if transpose:
         matrix = np.transpose(matrix)
     return matrix
 
 
 def tt_from_dense_matrix(matrix, shape, mode, idx):
     """
-    Helper function to wrap dense matrix into tensor. Inverse of :class:`pyttb.tt_to_dense_matrix`
+    Helper function to wrap dense matrix into tensor.
+    Inverse of :class:`pyttb.tt_to_dense_matrix`
 
     Parameters
     ----------
     matrix: :class:`numpy.ndarray`
     mode: int
         Mode around which tensor was unwrapped
     idx: int
@@ -66,71 +67,14 @@
     tensorInstance = tensorInstance.reshape(shape)
     tensorInstance = tensorInstance.permute(
         np.concatenate((np.arange(1, mode + 1), [0], np.arange(mode + 1, len(shape))))
     )
     return tensorInstance
 
 
-def tt_to_sparse_matrix(sptensorInstance, mode, transpose=False):
-    """
-    Helper function to unwrap sptensor into sparse matrix, should replace the core need for sptenmat
-
-    Parameters
-    ----------
-    sptensorInstance: :class:`pyttb.sptensor`
-    mode: int
-        Mode around which to unwrap tensor
-    transpose: bool
-        Whether or not to tranpose unwrapped tensor
-
-    Returns
-    -------
-    spmatrix: :class:`Scipy.sparse.coo_matrix`
-    """
-    old = np.setdiff1d(np.arange(sptensorInstance.ndims), mode).astype(int)
-    spmatrix = sptensorInstance.reshape(
-        (np.prod(np.array(sptensorInstance.shape)[old]),), old
-    ).spmatrix()
-    if transpose:
-        return spmatrix.transpose()
-    else:
-        return spmatrix
-
-
-def tt_from_sparse_matrix(spmatrix, shape, mode, idx):
-    """
-    Helper function to wrap sparse matrix into sptensor. Inverse of :class:`pyttb.tt_to_sparse_matrix`
-
-    Parameters
-    ----------
-    spmatrix: :class:`Scipy.sparse.coo_matrix`
-    mode: int
-        Mode around which tensor was unwrapped
-    idx: int
-        in {0,1}, idx of mode in spmatrix, s.b. 0 for tranpose=True
-
-    Returns
-    -------
-    sptensorInstance: :class:`pyttb.sptensor`
-    """
-    siz = np.array(shape)
-    old = np.setdiff1d(np.arange(len(shape)), mode).astype(int)
-    sptensorInstance = ttb.sptensor.from_tensor_type(sparse.coo_matrix(spmatrix))
-
-    # This expands the compressed dimension back to full size
-    sptensorInstance = sptensorInstance.reshape(siz[old], idx)
-    # This puts the modes in the right order, reshape places modified modes after the unchanged ones
-    sptensorInstance = sptensorInstance.reshape(
-        shape,
-        np.concatenate((np.arange(1, mode + 1), [0], np.arange(mode + 1, len(shape)))),
-    )
-
-    return sptensorInstance
-
-
 def tt_union_rows(MatrixA, MatrixB):
     """
     Helper function to reproduce functionality of MATLABS intersect(a,b,'rows')
 
     Parameters
     ----------
     MatrixA: :class:`numpy.ndarray`
@@ -202,43 +146,44 @@
         if not np.all(np.isin(-dims, np.arange(0, N + 1))):
             assert False, "Invalid magnitude for negative dims selection"
         dims = np.setdiff1d(np.arange(1, N + 1), -dims) - 1
 
     # Save dimensions of dims
     P = len(dims)
 
-    # Reorder dims from smallest to largest
-    # (this matters in particular for the vector multiplicand case, where the order affects the result)
+    # Reorder dims from smallest to largest (this matters in particular for the vector
+    # multiplicand case, where the order affects the result)
     sidx = np.argsort(dims)
     sdims = dims[sidx]
     vidx = None
 
     if M is not None:
         # Can't have more multiplicands than dimensions
         if M > N:
             assert False, "Cannot have more multiplicands than dimensions"
 
-        # Check that the number of multiplicands must either be full dimensional or equal to the specified dimensions
-        # (M==N) or M(==P) respectively
-        if M != N and M != P:
+        # Check that the number of multiplicands must either be full dimensional or
+        # equal to the specified dimensions (M==N) or M(==P) respectively
+        if M not in (N, P):
             assert False, "Invalid number of multiplicands"
 
         # Check sizes to determine how to index multiplicands
         if P == M:
-            # Case 1: Number of items in dims and number of multiplicands are equal; therfore, index in order of sdims
+            # Case 1: Number of items in dims and number of multiplicands are equal;
+            # therfore, index in order of sdims
             vidx = sidx
         else:
-            # Case 2: Number of multiplicands is equal to the number of dimensions of tensor;
-            # therefore, index multiplicands by dimensions in dims argument.
+            # Case 2: Number of multiplicands is equal to the number of dimensions of
+            # tensor; therefore, index multiplicands by dimensions in dims argument.
             vidx = sdims
 
     return sdims, vidx
 
 
-def tt_tenfun(function_handle, *inputs):
+def tt_tenfun(function_handle, *inputs):  # pylint:disable=too-many-branches
     """
     Apply a function to each element in a tensor
 
     Parameters
     ----------
     function_handle: callable
     inputs: tensor type, or np.array
@@ -252,57 +197,58 @@
 
     if len(inputs) == 0:
         assert False, "Must provide element(s) to perform operation on"
 
     assert callable(function_handle), "function_handle must be callable"
 
     # Convert inputs to tensors if they aren't already
-    for i in range(0, len(inputs)):
-        if isinstance(inputs[i], ttb.tensor) or isinstance(inputs[i], (float, int)):
+    for i, an_input in enumerate(inputs):
+        if isinstance(an_input, (ttb.tensor, float, int)):
             continue
-        elif isinstance(inputs[i], np.ndarray):
-            inputs[i] = ttb.tensor.from_data(inputs[i])
+        if isinstance(an_input, np.ndarray):
+            inputs[i] = ttb.tensor.from_data(an_input)
         elif isinstance(
-            inputs[i],
+            an_input,
             (
                 ttb.ktensor,
                 ttb.ttensor,
                 ttb.sptensor,
                 ttb.sumtensor,
                 ttb.symtensor,
                 ttb.symktensor,
             ),
         ):
-            inputs[i] = ttb.tensor.from_tensor_type(inputs[i])
+            inputs[i] = ttb.tensor.from_tensor_type(an_input)
         else:
             assert False, "Invalid input to ten fun"
 
-    # It's ok if there are two input and one is a scalar; otherwise all inputs have to be the same size
+    # It's ok if there are two input and one is a scalar; otherwise all inputs have to
+    # be the same size
     if (
         (len(inputs) == 2)
         and isinstance(inputs[0], (float, int))
         and isinstance(inputs[1], ttb.tensor)
     ):
         sz = inputs[1].shape
     elif (
         (len(inputs) == 2)
         and isinstance(inputs[1], (float, int))
         and isinstance(inputs[0], ttb.tensor)
     ):
         sz = inputs[0].shape
     else:
-        for i in range(0, len(inputs)):
-            if isinstance(inputs[i], (float, int)):
-                assert False, "Argument {} is a scalar but expected a tensor".format(i)
+        for i, an_input in enumerate(inputs):
+            if isinstance(an_input, (float, int)):
+                assert False, f"Argument {i} is a scalar but expected a tensor"
             elif i == 0:
-                sz = inputs[i].shape
-            elif sz != inputs[i].shape:
+                sz = an_input.shape
+            elif sz != an_input.shape:
                 assert (
                     False
-                ), "Tensor {} is not the same size as the first tensor input".format(i)
+                ), f"Tensor {i} is not the same size as the first tensor input"
 
     # Number of inputs for function handle
     nfunin = len(signature(function_handle).parameters)
 
     # Case I: Binary function
     if len(inputs) == 2 and nfunin == 2:
         X = inputs[0]
@@ -318,16 +264,16 @@
 
     # Case II: Expects input to be matrix and applies operation on each columns
     if len(inputs) == 1:
         X = inputs[0].data
         X = np.reshape(X, (1, -1))
     else:
         X = np.zeros((len(inputs), np.prod(sz)))
-        for i in range(0, len(inputs)):
-            X[i, :] = np.reshape(inputs[i].data, (np.prod(sz)))
+        for i, an_input in enumerate(inputs):
+            X[i, :] = np.reshape(an_input.data, (np.prod(sz)))
     data = function_handle(X)
     data = np.reshape(data, sz)
     Z = ttb.tensor.from_data(data)
     return Z
 
 
 def tt_setdiff_rows(MatrixA, MatrixB):
@@ -391,47 +337,47 @@
         MatrixBUnique = idxB = np.array([], dtype=int)
     location = tt_ismember_rows(
         MatrixBUnique[np.argsort(idxB)], MatrixAUnique[np.argsort(idxA)]
     )
     return location[np.where(location >= 0)]
 
 
-def tt_irenumber(t, shape, number_range):
+def tt_irenumber(t, shape, number_range):  # pylint: disable=unused-argument
     """
     RENUMBER indices for sptensor subsasgn
 
     Parameters
     ----------
     t: :class:`pyttb.sptensor`
     shape: tuple(int)
     range: tuple, len(range) = modes in tensor. Is key from __setitem__
 
     Returns
     -------
     newsubs: :class:`numpy.ndarray`
     """
-    # TODO shape is unused. Should it be used? I don't particularly understand what this is meant to be doing
+    # TODO shape is unused. Should it be used? I don't particularly understand what
+    #  this is meant to be doing
     nz = t.nnz
     if nz == 0:
         newsubs = np.array([])
         return newsubs
-    else:
-        newsubs = t.subs.astype(int)
-        for i in range(0, len(number_range)):
-            r = number_range[i]
-            if isinstance(r, slice):
-                newsubs[:, i] = (newsubs[:, i])[r]
-            elif isinstance(r, int):
-                # This appears to be inserting new keys as rows to our subs here
-                newsubs = np.insert(newsubs, obj=i, values=r, axis=1)
-            else:
-                if isinstance(r, list):
-                    r = np.array(r)
-                newsubs[:, i] = r[newsubs[:, i]]
-        return newsubs
+
+    newsubs = t.subs.astype(int)
+    for i, r in enumerate(number_range):
+        if isinstance(r, slice):
+            newsubs[:, i] = (newsubs[:, i])[r]
+        elif isinstance(r, int):
+            # This appears to be inserting new keys as rows to our subs here
+            newsubs = np.insert(newsubs, obj=i, values=r, axis=1)
+        else:
+            if isinstance(r, list):
+                r = np.array(r)
+            newsubs[:, i] = r[newsubs[:, i]]
+    return newsubs
 
 
 def tt_assignment_type(x, subs, rhs):
     """
     TT_ASSIGNMENT_TYPE What type of subsagn is this?
 
     Parameters
@@ -440,21 +386,20 @@
     subs:
     rhs:
 
     Returns
     -------
     objectType
     """
-    if type(x) == type(rhs):
+    if type(x) is type(rhs):
         return "subtensor"
     # If subscripts is a tuple that contains an nparray
-    elif isinstance(subs, tuple) and len(subs) >= 2:
+    if isinstance(subs, tuple) and len(subs) >= 2:
         return "subtensor"
-    else:
-        return "subscripts"
+    return "subscripts"
 
 
 def tt_renumber(subs, shape, number_range):
     """
     RENUMBER indices for sptensor subsref
 
     [NEWSUBS,NEWSZ] = RENUMBER(SUBS,SZ,RANGE) takes a set of
@@ -472,16 +417,16 @@
     Returns
     -------
     newsubs: :class:`numpy.ndarray`
     newshape: tuple
     """
     newshape = np.array(shape)
     newsubs = subs
-    for i in range(0, len(shape)):
-        if not (number_range[i] == slice(None, None, None)):
+    for i in range(0, len(shape)):  # pylint: disable=consider-using-enumerate
+        if not number_range[i] == slice(None, None, None):
             if subs.size == 0:
                 if not isinstance(number_range[i], slice):
                     if isinstance(number_range[i], (int, float)):
                         newshape[i] = number_range[i]
                     else:
                         newshape[i] = len(number_range[i])
                 else:
@@ -525,20 +470,22 @@
         idx_map[number_range[i]] = int(i)
 
     # Do the mapping
     newidx = idx_map[idx]
     return newidx, newshape
 
 
+# TODO make more efficient, decide if we want to support the multiple response
+#  matlab does
+# pylint: disable=line-too-long
+# https://stackoverflow.com/questions/22699756/python-version-of-ismember-with-rows-and-index
+# For thoughts on how to speed this up
 def tt_ismember_rows(search, source):
     """
     Find location of search rows in source array
-    https://stackoverflow.com/questions/22699756/python-version-of-ismember-with-rows-and-index
-    For thoughts on how to speed this up
-    #TODO make more efficient, decide if we want to support the multiple response matlab does
 
     Parameters
     ----------
     search: :class:`numpy.ndarray`
     source: :class:`numpy.ndarray`
 
     Returns
@@ -547,18 +494,18 @@
     search.size==results.size,
     if search[0,:] == source[3,:], then results[0] = 3
     if exists i such that search[i,:] != source[j,:] for any j, then results[i] = -1
 
     Examples
     --------
     >>> a = np.array([[4, 6], [1, 9], [2, 6]])
-    >>> b = np.array([[1, 7],[1, 8],[2, 6],[2, 1],[2, 4],[4, 6],[4, 7],[5, 9],[5, 2],[5, 1]])
+    >>> b = np.array([[2, 6],[2, 1],[2, 4],[4, 6],[4, 7],[5, 9],[5, 2],[5, 1]])
     >>> results = tt_ismember_rows(a,b)
     >>> print(results)
-    [ 5 -1  2]
+    [ 3 -1  0]
 
     """
     results = np.ones(shape=search.shape[0]) * -1
     if search.size == 0:
         return results.astype(int)
     if source.size == 0:
         return results.astype(int)
@@ -581,38 +528,40 @@
     """
     if idx.size == 0:
         return np.empty(shape=(0, len(shape)), dtype=int)
 
     return np.array(np.unravel_index(idx, shape, order="F")).transpose()
 
 
-def tt_subsubsref(obj, s):
+def tt_subsubsref(obj, s):  # pylint: disable=unused-argument
     """
     Helper function for tensor toolbox subsref.
 
     Parameters
     ----------
     obj: Tensor Data Structure
     s: Reference into tensor
 
     Returns
     -------
     Still uncertain to this functionality
     """
-    # TODO figure out when subsref yields key of length>1 for now ignore this logic and just return
+    # TODO figure out when subsref yields key of length>1 for now ignore this logic and
+    #  just return
     # if len(s) == 1:
     #    return obj
     # else:
     #   return obj[s[1:]]
     return obj
 
 
 def tt_intvec2str(v):
     """
-    Print integer vector to a string with brackets. Numpy should already handle this so it is a placeholder stub
+    Print integer vector to a string with brackets. Numpy should already handle this so
+    it is a placeholder stub
 
     Parameters
     ----------
     v: :class:`numpy.ndarray` integer vector
     Returns
     -------
     str: formatted string to print
@@ -770,18 +719,15 @@
     v: :class:`numpy.ndarray`
     vector input
 
     Returns
     -------
     bool
     """
-    if v.ndim == 2 and v.shape[0] == 1 and v.shape[1] >= 1:
-        return True
-    else:
-        return False
+    return v.ndim == 2 and v.shape[0] == 1 and v.shape[1] >= 1
 
 
 def isvector(a):
     """
     ISVECTOR Checks if vector is a row vector.
 
     ISVECTOR(A) returns True if A is a vector; otherwise returns False.
@@ -790,29 +736,27 @@
     ----------
     a: :class:`numpy.ndarray`
 
     Returns
     -------
     bool
     """
-    if a.ndim == 1 or (a.ndim == 2 and (a.shape[0] == 1 or a.shape[1] == 1)):
-        return True
-    else:
-        return False
+    return a.ndim == 1 or (a.ndim == 2 and (a.shape[0] == 1 or a.shape[1] == 1))
 
 
-# TODO: this is a challenge, since it may need to apply to either Python built in types or numpy types
+# TODO: this is a challenge, since it may need to apply to either Python built in types
+#  or numpy types
 def islogical(a):
     """
     ISLOGICAL Checks if vector is a logical vector.
 
     ISLOGICAL(A) returns True if A is a logical array; otherwise returns False.
 
     Parameters
     ----------
     a: :class:`numpy.ndarray`
 
     Returns
     -------
     bool
     """
-    return type(a) == bool
+    return isinstance(a, bool)
```

### Comparing `pyttb-1.5.0/pyttb/sptensor.py` & `pyttb-1.5.1/pyttb/sptensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,98 @@
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
+"""Sparse Tensor Implementation"""
+from __future__ import annotations
 
 import warnings
+from collections.abc import Sequence
+from typing import Any, Callable, List, Optional, Tuple, Union, cast, overload
 
 import numpy as np
-import scipy.sparse as sparse
 import scipy.sparse.linalg
 from numpy_groupies import aggregate as accumarray
+from scipy import sparse
 
 import pyttb as ttb
+from pyttb.pyttb_utils import (
+    tt_assignment_type,
+    tt_dimscheck,
+    tt_ind2sub,
+    tt_intvec2str,
+    tt_sizecheck,
+    tt_sub2ind,
+    tt_subscheck,
+    tt_subsubsref,
+    tt_valscheck,
+)
+
+
+def tt_to_sparse_matrix(
+    sptensorInstance: sptensor, mode: int, transpose: bool = False
+) -> sparse.coo_matrix:
+    """
+    Helper function to unwrap sptensor into sparse matrix, should replace the core need
+    for sptenmat
 
-from .pyttb_utils import *
+    Parameters
+    ----------
+    sptensorInstance: sparse tensor to unwrap
+    mode: Mode around which to unwrap tensor
+    transpose: Whether or not to tranpose unwrapped tensor
+
+    Returns
+    -------
+    spmatrix: unwrapped tensor
+    """
+    old = np.setdiff1d(np.arange(sptensorInstance.ndims), mode).astype(int)
+    spmatrix = sptensorInstance.reshape(
+        (np.prod(np.array(sptensorInstance.shape)[old]),), old
+    ).spmatrix()
+    if transpose:
+        return spmatrix.transpose()
+    return spmatrix
 
 
-class sptensor(object):
+def tt_from_sparse_matrix(
+    spmatrix: sparse.coo_matrix, shape: Any, mode: int, idx: int
+) -> sptensor:
+    """
+    Helper function to wrap sparse matrix into sptensor.
+    Inverse of :class:`pyttb.tt_to_sparse_matrix`
+
+    Parameters
+    ----------
+    spmatrix: :class:`Scipy.sparse.coo_matrix`
+    mode: int
+        Mode around which tensor was unwrapped
+    idx: int
+        in {0,1}, idx of mode in spmatrix, s.b. 0 for tranpose=True
+
+    Returns
+    -------
+    sptensorInstance: :class:`pyttb.sptensor`
+    """
+    siz = np.array(shape)
+    old = np.setdiff1d(np.arange(len(shape)), mode).astype(int)
+    sptensorInstance = ttb.sptensor.from_tensor_type(sparse.coo_matrix(spmatrix))
+
+    # This expands the compressed dimension back to full size
+    sptensorInstance = sptensorInstance.reshape(siz[old], idx)
+    # This puts the modes in the right order, reshape places modified modes after the
+    # unchanged ones
+    sptensorInstance = sptensorInstance.reshape(
+        shape,
+        np.concatenate([np.arange(1, mode + 1), [0], np.arange(mode + 1, len(shape))]),
+    )
+
+    return sptensorInstance
+
+
+class sptensor:
     """
     SPTENSOR Class for sparse tensors.
     """
 
     def __init__(self):
         """
         Create an empty sparse tensor
@@ -37,27 +111,25 @@
         # if tt_sizecheck(source):
         #    self.subs = np.array([])
         #    self.vals = np.array([])
         #    self.size = source
         #    return
 
     @classmethod
-    def from_data(cls, subs, vals, shape):
+    def from_data(
+        cls, subs: np.ndarray, vals: np.ndarray, shape: Tuple[int, ...]
+    ) -> sptensor:
         """
         Construct an sptensor from fully defined SUB, VAL and SIZE matrices.
 
         Parameters
         ----------
-        subs: :class:`numpy.ndarray`
-        vals: :class:`numpy.ndarray`
-        shape: tuple
-
-        Returns
-        -------
-        :class:`pyttb.sptensor`
+        subs: location of non-zero entries
+        vals: values for non-zero entries
+        shape: shape of sparse tensor
 
         Examples
         --------
         Import required modules:
 
         >>> import pyttb as ttb
         >>> import numpy as np
@@ -73,27 +145,27 @@
         sptensorInstance = cls()
         sptensorInstance.subs = subs
         sptensorInstance.vals = vals
         sptensorInstance.shape = shape
         return sptensorInstance
 
     @classmethod
-    def from_tensor_type(cls, source):
+    def from_tensor_type(
+        cls, source: Union[sptensor, ttb.tensor, sparse.coo_matrix]
+    ) -> sptensor:
         """
-        Contruct an :class:`pyttb.sptensor` from :class:`pyttb.sptensor`,
-        :class:`pyttb.tensor`, :class:`pyttb.sptenmat`, :class:`pyttb.sptensor3`
+        Contruct an :class:`pyttb.sptensor` from compatible tensor types
 
         Parameters
         ----------
-        source: :class:`pyttb.sptensor`, :class:`pyttb.tensor`, :class:`pyttb.sptenmat`,\
-            or :class:`pyttb.sptensor3`
+        source: Source tensor to create sptensor from
 
         Returns
         -------
-        :class:`pyttb.sptensor`
+        Generated Sparse Tensor
         """
         # Copy Constructor
         if isinstance(source, sptensor):
             return cls().from_data(source.subs.copy(), source.vals.copy(), source.shape)
 
         # Convert SPTENMAT
         if isinstance(source, ttb.sptenmat):  # pragma: no cover
@@ -117,39 +189,48 @@
 
         # Convert MDA
         # TODO what is an MDA?
 
         assert False, "Invalid Tensor Type To initialize Sptensor"
 
     @classmethod
-    def from_function(cls, function_handle, shape, nonzeros):
+    def from_function(
+        cls,
+        function_handle: Callable[[Tuple[float, float]], np.ndarray],
+        shape: Tuple[int, ...],
+        nonzeros: float,
+    ) -> sptensor:
         """
-        Creates a sparse tensor of the specified shape with NZ nonzeros created from the specified function handle
+        Creates a sparse tensor of the specified shape with NZ nonzeros created from
+        the specified function handle
 
         Parameters
         ----------
-        function_handle: function that accepts 2 arguments and generates :class:`numpy.ndarray` of length nonzeros
+        function_handle: function that accepts 2 arguments and generates
+            :class:`numpy.ndarray` of length nonzeros
         shape: tuple
         nonzeros: int or float
 
         Returns
         -------
-        :class:`pyttb.sptensor`
+        Generated Sparse Tensor
         """
         # Random Tensor
         assert callable(function_handle), "function_handle must be callable"
 
         if (nonzeros < 0) or (nonzeros >= np.prod(shape)):
-            assert (
-                False
-            ), "Requested number of non-zeros must be positive and less than the total size"
+            assert False, (
+                "Requested number of non-zeros must be positive "
+                "and less than the total size"
+            )
         elif nonzeros < 1:
             nonzeros = int(np.ceil(np.prod(shape) * nonzeros))
         else:
             nonzeros = int(np.floor(nonzeros))
+        nonzeros = int(nonzeros)
 
         # Keep iterating until we find enough unique non-zeros or we give up
         subs = np.array([])
         cnt = 0
         while (len(subs) < nonzeros) and (cnt < 10):
             subs = (
                 np.random.uniform(size=[nonzeros, len(shape)]).dot(np.diag(shape))
@@ -161,28 +242,36 @@
         subs = subs[0:nonzeros, :]
         vals = function_handle((nonzeros, 1))
 
         # Store everything
         return cls().from_data(subs, vals, shape)
 
     @classmethod
-    def from_aggregator(cls, subs, vals, shape=None, function_handle="sum"):
+    def from_aggregator(
+        cls,
+        subs: np.ndarray,
+        vals: np.ndarray,
+        shape: Optional[Tuple[int, ...]] = None,
+        function_handle: Union[str, Callable[[Any], Union[float, np.ndarray]]] = "sum",
+    ) -> sptensor:
         """
-        Construct an sptensor from fully defined SUB, VAL and shape matrices, after an aggregation is applied
+        Construct an sptensor from fully defined SUB, VAL and shape matrices,
+        after an aggregation is applied
 
         Parameters
         ----------
-        subs: :class:`numpy.ndarray`
-        vals: :class:`numpy.ndarray`
-        shape: tuple
-        function_handle: callable
+        subs: location of non-zero entries
+        vals: values for non-zero entries
+        shape: shape of sparse tensor
+        function_handle: Aggregation function, or name of supported
+            aggregation function from numpy_groupies
 
         Returns
         -------
-        :class:`pyttb.sptensor`
+        Generated Sparse Tensor
 
         Examples
         --------
         >>> subs = np.array([[1, 2], [1, 3]])
         >>> vals = np.array([[6], [7]])
         >>> shape = np.array([4, 4])
         >>> K0 = ttb.sptensor.from_aggregator(subs,vals)
@@ -203,16 +292,16 @@
             shape = tuple(np.max(subs, axis=0) + 1)
 
         # Check for wrong input
         if subs.size > 0 and subs.shape[1] > len(shape):
             assert False, "More subscripts than specified by shape"
 
         # Check for subscripts out of range
-        for j in range(len(shape)):
-            if subs.size > 0 and np.max(subs[:, j]) > shape[j]:
+        for j, dim in enumerate(shape):
+            if subs.size > 0 and np.max(subs[:, j]) > dim:
                 assert False, "Subscript exceeds sptensor shape"
 
         if subs.size == 0:
             newsubs = np.array([])
             newvals = np.array([])
         else:
             # Identify only the unique indices
@@ -231,20 +320,21 @@
         if newvals.size > 0:
             newvals = newvals[:, None]
 
         # Store everything
         return cls().from_data(newsubs, newvals, shape)
 
     # TODO decide if property
-    def allsubs(self):
+    def allsubs(self) -> np.ndarray:
         """
         Generate all possible subscripts for sparse tensor
+
         Returns
         -------
-        s: :class:`numpy.ndarray` all possible subscripts for sptensor
+        s: All possible subscripts for sptensor
         """
 
         # Generate all possible indices
 
         # Preallocate (discover any memory issues here!)
         s = np.zeros(shape=(np.prod(self.shape), self.ndims))
 
@@ -257,76 +347,92 @@
         for n in range(0, self.ndims):
             i = o.copy()
             i[n] = np.expand_dims(np.arange(0, self.shape[n]), axis=1)
             s[:, n] = np.squeeze(ttb.khatrirao(i))
 
         return s.astype(int)
 
-    def collapse(self, dims=None, fun="sum"):
+    def collapse(
+        self,
+        dims: Optional[np.ndarray] = None,
+        fun: Callable[[np.ndarray], Union[float, np.ndarray]] = np.sum,
+    ) -> Union[float, np.ndarray, sptensor]:
         """
         Collapse sparse tensor along specified dimensions.
 
         Parameters
         ----------
-        dims:
-        fun: callable
+        dims: Dimensions to collapse
+        fun: Method used to collapse dimensions
 
         Returns
         -------
+        Collapsed value
 
+        Example
+        -------
+        >>> subs = np.array([[1, 2], [1, 3]])
+        >>> vals = np.array([[1], [1]])
+        >>> shape = np.array([4, 4])
+        >>> X = ttb.sptensor.from_data(subs, vals, shape)
+        >>> X.collapse()
+        2
+        >>> X.collapse(np.arange(X.ndims), sum)
+        2
         """
         if dims is None:
             dims = np.arange(0, self.ndims)
 
         dims, _ = tt_dimscheck(dims, self.ndims)
         remdims = np.setdiff1d(np.arange(0, self.ndims), dims)
 
         # Check for the case where we accumulate over *all* dimensions
         if remdims.size == 0:
-            if fun == "sum":
-                return sum(self.vals.transpose()[0])
-            else:
-                return fun(self.vals.transpose()[0])
+            return fun(self.vals.transpose()[0])
 
         # Calculate the size of the result
         newsize = np.array(self.shape)[remdims]
 
         # Check for the case where the result is just a dense vector
         if remdims.size == 1:
             if self.subs.size > 0:
                 return accumarray(
                     self.subs[:, remdims].transpose()[0],
                     self.vals.transpose()[0],
                     size=newsize[0],
                     func=fun,
                 )
-            else:
-                return np.zeros((newsize[0], 1))
+            return np.zeros((newsize[0], 1))
 
         # Create Result
         if self.subs.size > 0:
             return ttb.sptensor.from_aggregator(
                 self.subs[:, remdims], self.vals, tuple(newsize), fun
             )
-        else:
-            return ttb.sptensor.from_data(np.array([]), np.array([]), tuple(newsize))
+        return ttb.sptensor.from_data(np.array([]), np.array([]), tuple(newsize))
 
-    def contract(self, i, j):
+    def contract(self, i: int, j: int) -> Union[np.ndarray, sptensor, ttb.tensor]:
         """
         Contract tensor along two dimensions (array trace).
 
         Parameters
         ----------
-        i: int
-        j: int
+        i: First dimension
+        j: Second dimension
 
         Returns
         -------
+        Contracted sptensor, converted to tensor if sufficiently dense
 
-
+        Example
+        -------
+        >>> X = ttb.tensor.from_data(np.ones((2,2)))
+        >>> Y = sptensor.from_tensor_type(X)
+        >>> Y.contract(0, 1)
+        2.0
         """
         if self.shape[i] != self.shape[j]:
             assert False, "Must contract along equally sized dimensions"
 
         if i == j:
             assert False, "Must contract along two different dimensions"
 
@@ -354,78 +460,71 @@
                 self.subs[indx, :][:, remdims], self.vals[indx], newsize
             )
 
         # Check if result should be dense
         if y.nnz > 0.5 * np.prod(y.shape):
             # Final result is a dense tensor
             return ttb.tensor.from_tensor_type(y)
-        else:
-            return y
+        return y
 
-    def double(self):
+    def double(self) -> np.ndarray:
         """
         Convert sptensor to dense multidimensional array
-
-        Returns
-        -------
-        :class:`numpy.ndarray`
         """
         a = np.zeros(self.shape)
         if self.nnz > 0:
             a[tuple(self.subs.transpose())] = self.vals.transpose()[0]
         return a
 
-    def elemfun(self, function):
+    def elemfun(self, function_handle: Callable[[np.ndarray], np.ndarray]) -> sptensor:
         """
         Manipulate the non-zero elements of a sparse tensor
 
         Parameters
         ----------
-        function: callable
+        function_handle: Function that updates all values.
 
         Returns
         -------
-        :class:`Tensortoolbox.sptensor`
+        Updated sptensor
+
+        Example
+        -------
+        >>> X = ttb.tensor.from_data(np.ones((2,2)))
+        >>> Y = sptensor.from_tensor_type(X)
+        >>> Z = Y.elemfun(lambda values: values*2)
+        >>> Z.isequal(Y*2)
+        True
         """
 
-        vals = function(self.vals)
+        vals = function_handle(self.vals)
         idx = np.where(vals > 0)[0]
         if idx.size == 0:
             return ttb.sptensor.from_data(np.array([]), np.array([]), self.shape)
-        else:
-            return ttb.sptensor.from_data(self.subs[idx, :], vals[idx], self.shape)
+        return ttb.sptensor.from_data(self.subs[idx, :], vals[idx], self.shape)
 
-    def end(self, k=None):
+    def end(self, k: Optional[int] = None) -> int:
         """
         Last index of indexing expression for sparse tensor
 
         Parameters
         ----------
         k: int Dimension for subscript indexing
-
-        Returns
-        -------
-        int:
         """
         if k is not None:
             return self.shape[k] - 1
-        else:
-            return np.prod(self.shape) - 1
+        return np.prod(self.shape) - 1
 
-    def extract(self, searchsubs):
+    def extract(self, searchsubs: np.ndarray) -> np.ndarray:
         """
         Extract value for a sptensor.
 
         Parameters
         ----------
-        searchsubs: :class:`numpy.ndarray` subscripts to find in sptensor
-
-        Returns
-        -------
-        :class:`numpy.ndarray`
+        searchsubs: subscripts to find in sptensor
 
         See Also
         --------
         :meth:`__getitem__`
         """
 
         # Check range of requested subscripts
@@ -451,30 +550,28 @@
         # Find which indices already exist and their locations
         loc = ttb.tt_ismember_rows(searchsubs, self.subs)
         # Fill in the non-zero elements in the answer
         nzsubs = np.where(loc >= 0)
         a[nzsubs] = self.vals[loc[nzsubs]]
         return a
 
-    def find(self):
+    def find(self) -> Tuple[np.ndarray, np.ndarray]:
         """
         FIND Find subscripts of nonzero elements in a sparse tensor.
 
         Returns
         -------
-        subs: :class:`numpy.ndarray`
-        vals: :class:`numpy.ndarray`
+        subs: Subscripts of nonzero elements
+        vals: Values at corresponding subscripts
         """
         return self.subs, self.vals
 
-    def full(self):
+    def full(self) -> ttb.tensor:
         """
         FULL Convert a sparse tensor to a (dense) tensor.
-
-        :return: tensor
         """
         # Handle the completely empty (no shape) case
         if len(self.shape) == 0:
             return ttb.tensor()
 
         # Create a dense zero tensor B that is the same shape as A
         B = ttb.tensor.from_data(np.zeros(shape=self.shape), self.shape)
@@ -485,26 +582,23 @@
         # Extract the linear indices of entries in A
         idx = tt_sub2ind(self.shape, self.subs)
 
         # Copy the values of A into B using linear indices
         B[idx.astype(int)] = self.vals.transpose()[0]
         return B
 
-    def innerprod(self, other):
+    def innerprod(
+        self, other: Union[sptensor, ttb.tensor, ttb.ktensor, ttb.ttensor]
+    ) -> float:
         """
         Efficient inner product with a sparse tensor
 
         Parameters
         ----------
-        other: :class:`pyttb.tensor`, :class:`pyttb.sptensor`, :class:`pyttb.ktensor`,
-        :class:`pyttb.ttensor`
-
-        Returns
-        -------
-        float
+        other: Other tensor to take innerproduct with
         """
         # If all entries are zero innerproduct must be 0
         if self.nnz == 0:
             return 0
 
         if isinstance(other, ttb.sptensor):
             if self.shape != other.shape:
@@ -517,150 +611,170 @@
                 [subsSelf, valsSelf] = self.find()
                 valsOther = other.extract(subsSelf)
             else:
                 [subsOther, valsOther] = other.find()
                 valsSelf = self.extract(subsOther)
             return valsOther.transpose().dot(valsSelf)
 
-        elif isinstance(other, ttb.tensor):
+        if isinstance(other, ttb.tensor):
             if self.shape != other.shape:
                 assert False, "Sptensor and tensor must be same shape for innerproduct"
             [subsSelf, valsSelf] = self.find()
             valsOther = other[subsSelf, "extract"]
             return valsOther.transpose().dot(valsSelf)
 
-        elif isinstance(other, (ttb.ktensor, ttb.ttensor)):  # pragma: no cover
+        if isinstance(other, (ttb.ktensor, ttb.ttensor)):  # pragma: no cover
             # Reverse arguments to call ktensor/ttensor implementation
             return other.innerprod(self)
 
-        else:
-            assert False, "Inner product between sptensor and that class not supported"
+        assert False, f"Inner product between sptensor and {type(other)} not supported"
 
-    def isequal(self, other):
+    def isequal(self, other: Union[sptensor, ttb.tensor]) -> bool:
         """
         Exact equality for sptensors
 
         Parameters
         ----------
-        other: :class:`pyttb.tensor`, :class:`pyttb.sptensor`
-
-        Returns
-        -------
-        bool: True if sptensors are identical, false otherwise
+        other: Other tensor to compare against
         """
         if self.shape != other.shape:
             return False
-        elif isinstance(other, ttb.sptensor):
+        if isinstance(other, ttb.sptensor):
             return (self - other).nnz == 0
-        elif isinstance(other, ttb.tensor):
+        if isinstance(other, ttb.tensor):
             return other.isequal(self)
-        else:
-            return False
+        return False
 
-    def logical_and(self, B):
+    def logical_and(self, B: Union[float, sptensor, ttb.tensor]) -> sptensor:
         """
         Logical and with self and another object
 
-        :param B: Scalar, tensor, or sptensor
-        :return: Indicator tensor
+        Parameters
+        ----------
+        B: Other value to compare with
+
+        Returns
+        ----------
+        Indicator tensor
         """
         # Case 1: One argument is a scalar
         if isinstance(B, (int, float)):
             if B == 0:
                 C = sptensor.from_data(np.array([]), np.array([]), self.shape)
             else:
                 newvals = self.vals == B
                 C = sptensor.from_data(self.subs, newvals, self.shape)
             return C
         # Case 2: Argument is a tensor of some sort
         if isinstance(B, sptensor):
             # Check that the shapes match
-            if not (self.shape == B.shape):
+            if not self.shape == B.shape:
                 assert False, "Must be tensors of the same shape"
 
-            def isLength2(x):
+            def is_length_2(x):
                 return len(x) == 2
 
             C = sptensor.from_aggregator(
                 np.vstack((self.subs, B.subs)),
                 np.vstack((self.vals, B.vals)),
                 self.shape,
-                isLength2,
+                is_length_2,
             )
 
             return C
 
         if isinstance(B, ttb.tensor):
             BB = sptensor.from_data(
                 self.subs, B[self.subs, "extract"][:, None], self.shape
             )
             C = self.logical_and(BB)
             return C
 
         # Otherwise
         assert False, "The arguments must be two sptensors or an sptensor and a scalar."
 
-    def logical_not(self):
+    def logical_not(self) -> sptensor:
         """
         Logical NOT for sptensors
 
         Returns
         -------
-        :class:`pyttb.sptensor` Sparse tensor with all zero-values marked from original sparse tensor
+        Sparse tensor with all zero-values marked from original
+        sparse tensor
         """
         allsubs = self.allsubs()
         subsIdx = ttb.tt_setdiff_rows(allsubs, self.subs)
         subs = allsubs[subsIdx]
         trueVector = np.ones(shape=(subs.shape[0], 1), dtype=bool)
         return sptensor.from_data(subs, trueVector, self.shape)
 
-    def logical_or(self, B):
+    @overload
+    def logical_or(self, B: Union[float, ttb.tensor]) -> ttb.tensor:
+        ...  # pragma: no cover see coveragepy/issues/970
+
+    @overload
+    def logical_or(self, B: sptensor) -> sptensor:
+        ...  # pragma: no cover see coveragepy/issues/970
+
+    def logical_or(
+        self, B: Union[float, ttb.tensor, sptensor]
+    ) -> Union[ttb.tensor, sptensor]:
         """
-        Logical OR for sptensors
+        Logical OR for sptensor and another value
 
         Returns
         -------
-        :class:'pyttb.sptensor` or :class:'pyttb.tensor` sptensor.logical_or(<int,float,tensor>) yields
-        tensor, sptensor.logical_or(sptensor) yields sptensor.
+        Indicator tensor
         """
         # Case 1: Argument is a scalar or tensor
-        if isinstance(B, (float, int)) or isinstance(B, ttb.tensor):
+        if isinstance(B, (float, int, ttb.tensor)):
             return self.full().logical_or(B)
 
         # Case 2: Argument is an sptensor
         if self.shape != B.shape:
             assert False, "Logical Or requires tensors of the same size"
 
         if isinstance(B, ttb.sptensor):
 
-            def isLengthGE1(x):
+            def is_length_ge_1(x):
                 return len(x) >= 1
 
             return sptensor.from_aggregator(
                 np.vstack((self.subs, B.subs)),
                 np.ones((self.subs.shape[0] + B.subs.shape[0], 1)),
                 self.shape,
-                isLengthGE1,
+                is_length_ge_1,
             )
 
         assert False, "Sptensor Logical Or argument must be scalar or sptensor"
 
-    def logical_xor(self, other):
+    @overload
+    def logical_xor(self, other: Union[float, ttb.tensor]) -> ttb.tensor:
+        ...  # pragma: no cover see coveragepy/issues/970
+
+    @overload
+    def logical_xor(self, other: sptensor) -> sptensor:
+        ...  # pragma: no cover see coveragepy/issues/970
+
+    def logical_xor(
+        self, other: Union[float, ttb.tensor, sptensor]
+    ) -> Union[ttb.tensor, sptensor]:
         """
         Logical XOR for sptensors
 
         Parameters
         ----------
+        other: Other value to xor against
 
         Returns
         -------
-
+        Indicator tensor
         """
         # Case 1: Argument is a scalar or dense tensor
-        if isinstance(other, (float, int)) or isinstance(other, ttb.tensor):
+        if isinstance(other, (float, int, ttb.tensor)):
             return self.full().logical_xor(other)
 
         # Case 2: Argument is an sptensor
         if isinstance(other, ttb.sptensor):
             # Check shape consistency
             if self.shape != other.shape:
                 assert False, "Logical XOR requires tensors of the same size"
@@ -671,25 +785,25 @@
             subs = np.vstack((self.subs, other.subs))
             return ttb.sptensor.from_aggregator(
                 subs, np.ones((len(subs), 1)), self.shape, length1
             )
 
         assert False, "The argument must be an sptensor, tensor or scalar"
 
-    def mask(self, W):
+    def mask(self, W: sptensor) -> np.ndarray:
         """
         Extract values as specified by a mask tensor
 
         Parameters
         ----------
-        W: :class:`pyttb.sptensor`
+        W: Mask tensor
 
         Returns
         -------
-        :class:`Numpy.ndarray`
+        Extracted values
         """
         # Error check
         if len(W.shape) != len(self.shape) or np.any(
             np.array(W.shape) > np.array(self.shape)
         ):
             assert False, "Mask cannot be bigger than the data tensor"
 
@@ -701,26 +815,26 @@
 
         # Assemble return array
         nvals = wsubs.shape[0]
         vals = np.zeros((nvals, 1))
         vals[idx] = self.vals[idx]
         return vals
 
-    def mttkrp(self, U, n):
+    def mttkrp(self, U: Union[ttb.ktensor, List[np.ndarray]], n: int) -> np.ndarray:
         """
         Matricized tensor times Khatri-Rao product for sparse tensor.
 
         Parameters
         ----------
-        U: array of matrices or ktensor
-        n: multiplies by all modes except n
+        U: Matrices to create the Khatri-Rao product
+        n: Mode to matricize sptensor in
 
         Returns
         -------
-        :class:`numpy.ndarray`
+        Matrix product
 
         Examples
         --------
         >>> matrix = np.ones((4, 4))
         >>> subs = np.array([[1, 1, 1], [1, 1, 3], [2, 2, 2], [3, 3, 3]])
         >>> vals = np.array([[0.5], [1.5], [2.5], [3.5]])
         >>> shape = (4, 4, 4)
@@ -769,106 +883,91 @@
                     Z.append(np.array([]))
             # Perform ttv multiplication
             V[:, r] = self.ttv(Z, -(n + 1)).double()
 
         return V
 
     @property
-    def ndims(self):
+    def ndims(self) -> int:
         """
         NDIMS Number of dimensions of a sparse tensor.
-
-        Returns
-        -------
-        int
-            Number of dimensions of Sptensor
         """
         return len(self.shape)
 
     @property
-    def nnz(self):
+    def nnz(self) -> int:
         """
         Number of nonzeros in sparse tensor
-
-        Returns
-        -------
-        nnz: int
         """
         if self.subs.size == 0:
             return 0
-        else:
-            return self.subs.shape[0]
+        return self.subs.shape[0]
 
-    def norm(self):
+    def norm(self) -> np.floating:
         """
-        Compute the norm of a sparse tensor.
-        Returns
-        -------
-        norm: float, Frobenius norm of Tensor
+        Compute the Frobenius norm of a sparse tensor.
         """
         return np.linalg.norm(self.vals)
 
-    def nvecs(self, n, r, flipsign=True):
+    def nvecs(self, n: int, r: int, flipsign: bool = True) -> np.ndarray:
         """
         Compute the leading mode-n vectors for a sparse tensor.
 
         Parameters
         ----------
-        n: mode for tensor matricization
-        r: number of eigenvalues
-        flipsign: Make each column's largest element positive if true
-
-        Returns
-        -------
-
+        n: Mode to unfold
+        r: Number of eigenvectors to compute
+        flipsign: Make each eigenvector's largest element positive
         """
         old = np.setdiff1d(np.arange(self.ndims), n).astype(int)
-        tnt = (
-            self.reshape((np.prod(np.array(self.shape)[old]), 1), old)
+        # tnt calculation is a workaround for missing sptenmat
+        mutatable_sptensor = (
+            sptensor.from_tensor_type(self)
+            .reshape((np.prod(np.array(self.shape)[old]), 1), old)
             .squeeze()
-            .spmatrix()
-            .transpose()
         )
+        if isinstance(mutatable_sptensor, (int, float, np.generic)):
+            raise ValueError(
+                "Cannot call nvecs on sptensor with only singleton dimensions"
+            )
+        tnt = mutatable_sptensor.spmatrix().transpose()
         y = tnt.transpose().dot(tnt)
         if r < y.shape[0] - 1:
             _, v = scipy.sparse.linalg.eigs(y, r)
         else:
             warnings.warn(
-                "Greater than or equal to sptensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
+                "Greater than or equal to sptensor.shape[n] - 1 eigenvectors requires"
+                " cast to dense to solve"
             )
             w, v = scipy.linalg.eig(y.toarray())
             v = v[(-np.abs(w)).argsort()]
             v = v[:, :r]
 
         if flipsign:
             idx = np.argmax(np.abs(v), axis=0)
             for i in range(v.shape[1]):
                 if v[idx[i], i] < 0:  # pragma: no cover
                     v[:, i] *= -1
         return v
 
-    def ones(self):
+    def ones(self) -> sptensor:
         """
         Replace nonzero elements of sparse tensor with ones
         """
         oneVals = self.vals.copy()
         oneVals.fill(1)
         return ttb.sptensor.from_data(self.subs, oneVals, self.shape)
 
-    def permute(self, order):
+    def permute(self, order: np.ndarray) -> sptensor:
         """
         Rearrange the dimensions of a sparse tensor
 
         Parameters
         ----------
-        order: :class:`Numpy.ndarray`
-
-        Returns
-        -------
-        :class:`pyttb.sptensor`
+        order: Updated order of dimensions
         """
         # Error check
         if self.ndims != order.size or np.any(
             np.sort(order) != np.arange(0, self.ndims)
         ):
             assert False, "Invalid permutation order"
 
@@ -877,15 +976,19 @@
             return ttb.sptensor.from_data(
                 self.subs[:, order], self.vals, tuple(np.array(self.shape)[order])
             )
         return ttb.sptensor.from_data(
             self.subs, self.vals, tuple(np.array(self.shape)[order])
         )
 
-    def reshape(self, new_shape, old_modes=None):
+    def reshape(
+        self,
+        new_shape: Tuple[int, ...],
+        old_modes: Optional[Union[np.ndarray, int]] = None,
+    ) -> sptensor:
         """
         Reshape specified modes of sparse tensor
 
         Parameters
         ----------
         new_shape: tuple
         old_modes: :class:`Numpy.ndarray`
@@ -910,115 +1013,106 @@
 
         if self.subs.size == 0:
             return ttb.sptensor.from_data(
                 np.array([]),
                 np.array([]),
                 tuple(np.concatenate((keep_shape, new_shape))),
             )
+        if np.isscalar(old_shape):
+            old_shape = (old_shape,)
+            inds = ttb.tt_sub2ind(old_shape, self.subs[:, old_modes][:, None])
         else:
-            if np.isscalar(old_shape):
-                old_shape = (old_shape,)
-                inds = ttb.tt_sub2ind(old_shape, self.subs[:, old_modes][:, None])
-            else:
-                inds = ttb.tt_sub2ind(old_shape, self.subs[:, old_modes])
-            new_subs = ttb.tt_ind2sub(new_shape, inds)
-            return ttb.sptensor.from_data(
-                np.concatenate((self.subs[:, keep_modes], new_subs), axis=1),
-                self.vals,
-                tuple(np.concatenate((keep_shape, new_shape))),
-            )
+            inds = ttb.tt_sub2ind(old_shape, self.subs[:, old_modes])
+        new_subs = ttb.tt_ind2sub(new_shape, inds)
+        return ttb.sptensor.from_data(
+            np.concatenate((self.subs[:, keep_modes], new_subs), axis=1),
+            self.vals,
+            tuple(np.concatenate((keep_shape, new_shape))),
+        )
 
-    def scale(self, factor, dims):
+    def scale(self, factor: np.ndarray, dims: Union[float, np.ndarray]) -> sptensor:
         """
         Scale along specified dimensions for sparse tensors
 
         Parameters
         ----------
         factor: :class:`numpy.ndarray`
         dims: int or :class:`numpy.ndarray`
 
         Returns
         -------
         :class:`pyttb.sptensor`
         """
         if isinstance(dims, (float, int)):
             dims = np.array([dims])
-        dims = ttb.tt_dimscheck(dims, self.ndims)
+        dims, _ = ttb.tt_dimscheck(dims, self.ndims)
 
         if isinstance(factor, ttb.tensor):
             shapeArray = np.array(self.shape)
             if np.any(factor.shape != shapeArray[dims]):
                 assert False, "Size mismatch in scale"
             return ttb.sptensor.from_data(
                 self.subs,
-                self.vals * factor[self.subs[:, dims[0]], "extract"][:, None],
+                self.vals * factor[self.subs[:, dims], "extract"][:, None],
                 self.shape,
             )
-        elif isinstance(factor, ttb.sptensor):
+        if isinstance(factor, ttb.sptensor):
             shapeArray = np.array(self.shape)
             if np.any(factor.shape != shapeArray[dims]):
                 assert False, "Size mismatch in scale"
             return ttb.sptensor.from_data(
-                self.subs, self.vals * factor.extract(self.subs[:, dims[0]]), self.shape
+                self.subs, self.vals * factor.extract(self.subs[:, dims]), self.shape
             )
-        elif isinstance(factor, np.ndarray):
+        if isinstance(factor, np.ndarray):
             shapeArray = np.array(self.shape)
             if factor.shape[0] != shapeArray[dims]:
                 assert False, "Size mismatch in scale"
             return ttb.sptensor.from_data(
                 self.subs,
-                self.vals * factor[self.subs[:, dims[0]].transpose()[0]],
+                self.vals * factor[self.subs[:, dims].transpose()[0]],
                 self.shape,
             )
-        else:
-            assert False, "Invalid scaling factor"
+        assert False, "Invalid scaling factor"
 
-    def spmatrix(self):
+    def spmatrix(self) -> sparse.coo_matrix:
         """
-        Converts a two-way sparse tensor to a sparse matrix in scipy.sparse.coo_matrix format
-
-        Returns
-        -------
-        :class:`scipy.sparse.coo_matrix`
+        Converts a two-way sparse tensor to a sparse matrix in
+        scipy.sparse.coo_matrix format
         """
         if self.ndims != 2:
             assert False, "Sparse tensor must be two dimensional"
 
         if self.subs.size == 0:
             return sparse.coo_matrix(self.shape)
-        else:
-            return sparse.coo_matrix(
-                (self.vals.transpose()[0], self.subs.transpose()), self.shape
-            )
+        return sparse.coo_matrix(
+            (self.vals.transpose()[0], self.subs.transpose()), self.shape
+        )
 
-    def squeeze(self):
+    def squeeze(self) -> Union[sptensor, float]:
         """
         Remove singleton dimensions from a sparse tensor
 
         Returns
         -------
         :class:`pyttb.sptensor` or float if sptensor is only singleton dimensions
         """
         shapeArray = np.array(self.shape)
 
         # No singleton dimensions
         if np.all(shapeArray > 1):
             return ttb.sptensor.from_tensor_type(self)
-        else:
-            idx = np.where(shapeArray > 1)[0]
-            if idx.size == 0:
-                return self.vals[0].copy()
-            else:
-                siz = tuple(shapeArray[idx])
-                if self.vals.size == 0:
-                    return ttb.sptensor.from_data(np.array([]), np.array([]), siz)
-                else:
-                    return ttb.sptensor.from_data(self.subs[:, idx], self.vals, siz)
+        idx = np.where(shapeArray > 1)[0]
+        if idx.size == 0:
+            return self.vals[0].copy()
+        siz = tuple(shapeArray[idx])
+        if self.vals.size == 0:
+            return ttb.sptensor.from_data(np.array([]), np.array([]), siz)
+        return ttb.sptensor.from_data(self.subs[:, idx], self.vals, siz)
 
-    def subdims(self, region):
+    def subdims(self, region: Sequence[Union[int, np.ndarray, slice]]) -> np.ndarray:
         """
         SUBDIMS Compute the locations of subscripts within a subdimension.
 
         Parameters
         ----------
         region: :class:`numpy.ndarray` or tuple denoting indexing
             Subset of total sptensor shape in which to find non-zero values
@@ -1045,63 +1139,71 @@
         """
         if len(region) != self.ndims:
             assert False, "Number of subdimensions must equal number of dimensions"
 
         # Error check that range is valid
         # TODO I think only accepting numeric arrays fixes this
 
-        # TODO we use this empty check a lot, do we want a boolean we store in the class for this?
+        # TODO we use this empty check a lot, do we want a boolean we store in the
+        #  class for this?
         if self.subs.size == 0:
             loc = np.array([])
             return loc
 
         # Compute the indices of the subscripts that are within the
         # specified range. We start with all indices in loc and
         # pare it down to a final list.
 
         loc = np.arange(0, len(self.subs))
 
         for i in range(0, self.ndims):
-            if not isinstance(region[i], slice):
-                # Find subscripts that match in dimension i
-                tf = np.isin(self.subs[loc, i], region[i])
-
-                # Pare down the list of indices
-                loc = loc[tf]
-            else:
+            # TODO: Consider cleaner typing coercion
+            # Find subscripts that match in dimension i
+            if isinstance(region[i], (int, np.generic)):
+                tf = np.isin(self.subs[loc, i], cast(int, region[i]))
+            elif isinstance(region[i], (np.ndarray, list)):
+                tf = np.isin(self.subs[loc, i], cast(np.ndarray, region[i]))
+            elif isinstance(region[i], slice):
                 sliceRegion = range(0, self.shape[i])[region[i]]
-
                 tf = np.isin(self.subs[loc, i], sliceRegion)
+            else:
+                raise ValueError(
+                    f"Unexpected type in region sequence. "
+                    f"At index: {i} got {region[i]} with type {type(region[i])}"
+                )
+
+            # Pare down the list of indices
+            loc = loc[tf]
 
-                # Pare down the list of indices
-                loc = loc[tf]
         return loc
 
-    def ttv(self, vector, dims=None):
+    # pylint: disable=too-many-branches, too-many-locals
+    def ttv(
+        self,
+        vector: Union[np.ndarray, List[np.ndarray]],
+        dims: Optional[Union[int, np.ndarray]] = None,
+    ) -> Union[sptensor, ttb.tensor]:
         """
         Sparse tensor times vector
 
         Parameters
         ----------
-        vector
-        dims
-
-        Returns
-        -------
-
+        vector: Vector(s) to multiply against
+        dims: Dimensions to multiply with vector(s)
         """
 
         if dims is None:
             dims = np.array([])
         elif isinstance(dims, (float, int)):
             dims = np.array([dims])
 
-        # Check that vector is a list of vectors, if not place single vector as element in list
+        # Check that vector is a list of vectors,
+        # if not place single vector as element in list
         if len(vector) > 0 and isinstance(vector[0], (int, float, np.int_, np.float_)):
-            return self.ttv([vector], dims)
+            return self.ttv(np.array([vector]), dims)
 
         # Get sorted dims and index for multiplicands
         dims, vidx = ttb.tt_dimscheck(dims, self.ndims, len(vector))
         remdims = np.setdiff1d(np.arange(0, self.ndims), dims).astype(int)
 
         # Check that each multiplicand is the right size.
         for i in range(dims.size):
@@ -1110,16 +1212,16 @@
 
         # Multiply each value by the appropriate elements of the appropriate vector
         newvals = self.vals.copy()
         subs = self.subs.copy()
         if subs.size == 0:  # No non-zeros in tensor
             newsubs = np.array([], dtype=int)
         else:
-            for n in range(len(dims)):
-                idx = subs[:, dims[n]]  # extract indices for dimension n
+            for n, dims_n in enumerate(dims):
+                idx = subs[:, dims_n]  # extract indices for dimension n
                 w = vector[vidx[n]]  # extract the nth vector
                 bigw = w[idx][:, None]  # stretch out the vector
                 newvals = newvals * bigw
             newsubs = subs[:, remdims].astype(int)
 
         # Case 0: If all dimensions were used, then just return the sum
         if remdims.size == 0:
@@ -1135,26 +1237,26 @@
             c = accumarray(
                 newsubs.transpose()[0], newvals.transpose()[0], size=newsiz[0]
             )
             if np.count_nonzero(c) <= 0.5 * newsiz:
                 return ttb.sptensor.from_aggregator(
                     np.arange(0, newsiz)[:, None], c, tuple(newsiz)
                 )
-            else:
-                return ttb.tensor.from_data(c, tuple(newsiz))
+            return ttb.tensor.from_data(c, tuple(newsiz))
 
         # Case 2: Result is a multiway array
         c = ttb.sptensor.from_aggregator(newsubs, newvals, tuple(newsiz))
 
         # Convert to a dense tensor if more than 50% of the result is nonzero.
         if c.nnz > 0.5 * np.prod(newsiz):
             c = ttb.tensor.from_tensor_type(c)
 
         return c
 
+    # pylint: disable=too-many-branches
     def __getitem__(self, item):
         """
         Subscripted reference for a sparse tensor.
 
         We can extract elements or subtensors from a sparse tensor in the
         following ways.
 
@@ -1181,21 +1283,24 @@
         Returns
         -------
 
         :class:`numpy.ndarray` or :class:`pyttb.sptensor`
 
         Examples
         --------
-        >>> X = sptensor.from_data(np.array([[3,3,3],[1,1,0],[1,2,1]]),np.array([3,5,1]),(4,4,4))
+        >>> subs = np.array([[3,3,3],[1,1,0],[1,2,1]])
+        >>> vals = np.array([3,5,1])
+        >>> shape = (4,4,4)
+        >>> X = sptensor.from_data(subs,vals,shape)
         >>> _ = X[0,1,0] #<-- returns zero
         >>> _ = X[3,3,3] #<-- returns 3
         >>> _ = X[2:3,:,:] #<-- returns 1 x 4 x 4 sptensor
         """
-        # This does not work like MATLAB TTB; you must call sptensor.extract to get this functionality
-        # X([1:6]','extract') %<-- extracts a vector of 6 elements
+        # This does not work like MATLAB TTB; you must call sptensor.extract to get
+        # this functionality: X([1:6]','extract') %<-- extracts a vector of 6 elements
 
         # TODO IndexError for value outside of indices
         # TODO Key error if item not in container
         # *** CASE 1: Rectangular Subtensor ***
         if isinstance(item, tuple) and len(item) == self.ndims:
             # Extract the subdimensions to be extracted from self
             region = item
@@ -1212,20 +1317,20 @@
 
             # Determine the subscripts
             newsiz = []  # (future) new size
             kpdims = []  # dimensions to keep
             rmdims = []  # dimensions to remove
 
             # Determine the new size and what dimensions to keep
-            for i in range(0, len(region)):
-                if isinstance(region[i], slice):
+            for i, a_region in enumerate(region):
+                if isinstance(a_region, slice):
                     newsiz.append(self.shape[i])
                     kpdims.append(i)
-                elif not isinstance(region[i], (int, float)):
-                    newsiz.append(np.prod(region[i]))
+                elif not isinstance(a_region, (int, float)):
+                    newsiz.append(np.prod(a_region))
                     kpdims.append(i)
                 else:
                     rmdims.append(i)
 
             newsiz = np.array(newsiz, dtype=int)
             kpdims = np.array(kpdims, dtype=int)
             rmdims = np.array(rmdims, dtype=int)
@@ -1278,14 +1383,15 @@
             srchsubs = tt_ind2sub(self.shape, idx)
 
         a = self.extract(srchsubs)
         a = tt_subsubsref(a, item)
 
         return a
 
+    # pylint:disable=too-many-statements, too-many-branches, too-many-locals
     def __setitem__(self, key, value):
         """
         Subscripted assignment for sparse tensor.
 
         We can assign elements to a sptensor in three ways.
 
         Case 1: X(R1,R2,...,RN) = Y, in which case we replace the
@@ -1333,45 +1439,46 @@
         ):
             return
 
         # Determine if we are doing a substenor or list of subscripts
         objectType = tt_assignment_type(self, key, value)
 
         # Case 1: Replace a sub-tensor
-        if objectType == "subtensor":
+        if objectType == "subtensor":  # pylint:disable=too-many-nested-blocks
             # Case I(a): RHS is another sparse tensor
             if isinstance(value, ttb.sptensor):
-                # First, Resize the tensor and check the size match with the tensor that's being inserted.
+                # First, Resize the tensor and check the size match with the tensor
+                # that's being inserted.
                 m = 0
                 newsz = []
-                for n in range(0, len(key)):
-                    if isinstance(key[n], slice):
+                for n, key_n in enumerate(key):
+                    if isinstance(key_n, slice):
                         if self.ndims <= n:
-                            if key[n].stop is None:
+                            if key_n.stop is None:
                                 newsz.append(value.shape[m])
                             else:
-                                newsz.append(key[n].stop)
+                                newsz.append(key_n.stop)
                         else:
-                            if key[n].stop is None:
+                            if key_n.stop is None:
                                 newsz.append(max([self.shape[n], value.shape[m]]))
                             else:
-                                newsz.append(max([self.shape[n], key[n].stop]))
+                                newsz.append(max([self.shape[n], key_n.stop]))
                         m = m + 1
-                    elif isinstance(key[n], (float, int)):
+                    elif isinstance(key_n, (float, int)):
                         if self.ndims <= n:
-                            newsz.append(key[n] + 1)
+                            newsz.append(key_n + 1)
                         else:
-                            newsz.append(max([self.shape[n], key[n] + 1]))
+                            newsz.append(max([self.shape[n], key_n + 1]))
                     else:
-                        if len(key[n]) != value.shape[m]:
+                        if len(key_n) != value.shape[m]:
                             assert False, "RHS does not match range size"
                         if self.ndims <= n:
-                            newsz.append(max(key[n]) + 1)
+                            newsz.append(max(key_n) + 1)
                         else:
-                            newsz.append(max([self.shape[n], max(key[n]) + 1]))
+                            newsz.append(max([self.shape[n], max(key_n) + 1]))
                 self.shape = tuple(newsz)
 
                 # Expand subs array if there are new modes, i.e., if the order
                 # has increased.
                 if self.subs.size > 0 and (len(self.shape) > self.subs.shape[1]):
                     self.subs = np.append(
                         self.subs,
@@ -1422,26 +1529,27 @@
                 else:
                     newsz.append(max([self.shape[n], key[n] + 1]))
 
             # Determine size of new modes, if any
             for n in range(self.ndims, len(key)):
                 if isinstance(key[n], slice):
                     if key[n].stop is None:
-                        assert (
-                            False
-                        ), "Must have well defined slice when expanding sptensor shape with setitem"
+                        assert False, (
+                            "Must have well defined slice when expanding sptensor "
+                            "shape with setitem"
+                        )
                     else:
                         newsz.append(key[n].stop)
                 elif isinstance(key[n], np.ndarray):
                     newsz.append(max(key[n]) + 1)
                 else:
                     newsz.append(key[n] + 1)
             self.shape = tuple(newsz)
 
-            # Expand subs array if there are new modes, i.e.m if the order has increasesd
+            # Expand subs array if there are new modes, i.e. if the order has increased
             if self.subs.size > 0 and len(self.shape) > self.subs.shape[1]:
                 self.subs = np.append(
                     self.subs,
                     np.zeros(
                         shape=(self.subs.shape[0], len(self.shape) - self.subs.shape[1])
                     ),
                     axis=1,
@@ -1543,23 +1651,26 @@
 
             # Copy rhs to newvals
             newvals = value
 
             if isinstance(newvals, (float, int)):
                 newvals = np.expand_dims([newvals], axis=1)
 
-            # Error check the rhs is a column vector. We don't bother to handle any other type with sparse tensors
+            # Error check the rhs is a column vector. We don't bother to handle any
+            # other type with sparse tensors
             tt_valscheck(newvals, nargout=False)
 
-            # Determine number of nonzeros being inserted. (This is determined by number of subscripts)
+            # Determine number of nonzeros being inserted.
+            # (This is determined by number of subscripts)
             newnnz = newsubs.shape[0]
 
             # Error check on size of newvals
             if newvals.size == 1:
-                # Special case where newvals is a single element to be assigned to multiple LHS. Fix to correct size
+                # Special case where newvals is a single element to be assigned
+                # to multiple LHS. Fix to correct size
                 newvals = newvals * np.ones((newnnz, 1))
 
             elif newvals.shape[0] != newnnz:
                 # Sizes don't match
                 assert False, "Number of subscripts and number of values do not match!"
 
             # Remove duplicates and print warning if any duplicates were removed
@@ -1581,15 +1692,16 @@
             #
             # Note that we are ignoring any new zero elements, because
             # those obviously do not need to be added. Also, it's
             # important to process Group A before Group B because the
             # processing of Group B may change the locations of the
             # remaining elements.
 
-            # TF+1 for logical consideration because 0 is valid index and -1 is our null flag
+            # TF+1 for logical consideration because 0 is valid index
+            # and -1 is our null flag
             idxa = np.logical_and(tf + 1, newvals)[0]
             idxb = np.logical_and(tf + 1, np.logical_not(newvals))[0]
             idxc = np.logical_and(np.logical_not(tf + 1), newvals)[0]
 
             # Process Group A: Changing values
             if np.sum(idxa) > 0:
                 self.vals[tf[idxa]] = newvals[idxa]
@@ -1602,17 +1714,17 @@
             # Process Group C: Adding new, nonzero values
             if np.sum(idxc) > 0:
                 self.subs = np.vstack((self.subs, newsubs[idxc, :]))
                 self.vals = np.vstack((self.vals, newvals[idxc]))
 
             # Resize the tensor
             newshape = []
-            for n in range(0, len(self.shape)):
+            for n, dim in enumerate(self.shape):
                 smax = max(newsubs[:, n] + 1)
-                newshape.append(max(self.shape[n], smax))
+                newshape.append(max(dim, smax))
             self.shape = tuple(newshape)
 
             return
 
     def __eq__(self, other):
         """
         Equal comparator for sptensors
@@ -1625,21 +1737,20 @@
         -------
         :class:`pyttb.sptensor`
         """
         # Case 1: other is a scalar
         if isinstance(other, (float, int)):
             if other == 0:
                 return self.logical_not()
-            else:
-                idx = self.vals == other
-                return sptensor.from_data(
-                    self.subs[idx.transpose()[0]],
-                    True * np.ones((self.subs.shape[0], 1)).astype(bool),
-                    self.shape,
-                )
+            idx = self.vals == other
+            return sptensor.from_data(
+                self.subs[idx.transpose()[0]],
+                True * np.ones((self.subs.shape[0], 1)).astype(bool),
+                self.shape,
+            )
 
         # Case 2: other is a tensor type
         # Check sizes
         if self.shape != other.shape:
             assert False, "Size mismatch in sptensor equality"
 
         # Case 2a: other is a sparse tensor
@@ -1650,15 +1761,16 @@
             # zzerosubs = np.isin(xzerosubs, otherzerosubs)
             zzerosubsIdx = ttb.tt_intersect_rows(
                 self.allsubs()[xzerosubs], other.allsubs()[otherzerosubs]
             )
             zzerosubs = self.allsubs()[xzerosubs][zzerosubsIdx]
 
             # Find where their nonzeros intersect
-            # TODO consider if intersect rows should return 3 args so we don't have to call it twice
+            # TODO consider if intersect rows should return 3 args so we don't have to
+            #  call it twice
             nzsubsIdx = ttb.tt_intersect_rows(self.subs, other.subs)
             nzsubs = self.subs[nzsubsIdx]
             iother = ttb.tt_intersect_rows(other.subs, self.subs)
             znzsubs = nzsubs[
                 (self.vals[nzsubsIdx] == other.vals[iother]).transpose()[0], :
             ]
 
@@ -1670,15 +1782,15 @@
                 ],
                 self.shape,
             )
 
         # Case 2b: other is a dense tensor
         if isinstance(other, ttb.tensor):
             # Find where their zeros interact
-            otherzerosubs, otherzerosubsflag = (other == 0).find()
+            otherzerosubs, _ = (other == 0).find()
             zzerosubs = otherzerosubs[
                 (self.extract(otherzerosubs) == 0).transpose()[0], :
             ]
 
             # Find where their nonzeros intersect
             othervals = other[self.subs, "extract"]
             znzsubs = self.subs[(othervals[:, None] == self.vals).transpose()[0], :]
@@ -1705,23 +1817,22 @@
         """
         # Case 1: One argument is a scalar
         if isinstance(other, (float, int)):
             if other == 0:
                 return ttb.sptensor.from_data(
                     self.subs, True * np.ones((self.subs.shape[0], 1)), self.shape
                 )
-            else:
-                subs1 = self.subs[self.vals.transpose()[0] != other, :]
-                subs2Idx = ttb.tt_setdiff_rows(self.allsubs(), self.subs)
-                subs2 = self.allsubs()[subs2Idx, :]
-                return ttb.sptensor.from_data(
-                    np.vstack((subs1, subs2)),
-                    True * np.ones((self.subs.shape[0], 1)).astype(bool),
-                    self.shape,
-                )
+            subs1 = self.subs[self.vals.transpose()[0] != other, :]
+            subs2Idx = ttb.tt_setdiff_rows(self.allsubs(), self.subs)
+            subs2 = self.allsubs()[subs2Idx, :]
+            return ttb.sptensor.from_data(
+                np.vstack((subs1, subs2)),
+                True * np.ones((self.subs.shape[0], 1)).astype(bool),
+                self.shape,
+            )
 
         # Case 2: Both x and y are tensors or some sort
         # Check that the sizes match
         if self.shape != other.shape:
             assert False, "Size mismatch"
         # Case 2a: Two sparse tensors
         if isinstance(other, ttb.sptensor):
@@ -1789,15 +1900,15 @@
         :class:`pyttb.sptensor`
         """
         # Case 1: One argument is a scalar
         # Emulating the sparse matrix case here, which creates and returns
         # a dense result, even if the scalar is zero.
 
         # Case 1: Second argument is a scalar or a dense tensor
-        if isinstance(other, (float, int)) or isinstance(other, ttb.tensor):
+        if isinstance(other, (float, int, ttb.tensor)):
             return self.full() - other
 
         # Case 2: Both are sparse tensors
         if not isinstance(other, ttb.sptensor) or self.shape != other.shape:
             assert False, "Must be two sparse tensors of the same shape"
 
         return ttb.sptensor.from_aggregator(
@@ -1871,33 +1982,33 @@
             idxSelf = ttb.tt_intersect_rows(self.subs, other.subs)
             idxOther = ttb.tt_intersect_rows(other.subs, self.subs)
             return ttb.sptensor.from_data(
                 self.subs[idxSelf],
                 self.vals[idxSelf] * other.vals[idxOther],
                 self.shape,
             )
-        elif isinstance(other, ttb.tensor):
+        if isinstance(other, ttb.tensor):
             csubs = self.subs
             cvals = self.vals * other[csubs, "extract"][:, None]
             return ttb.sptensor.from_data(csubs, cvals, self.shape)
-        elif isinstance(other, ttb.ktensor):
+        if isinstance(other, ttb.ktensor):
             csubs = self.subs
             cvals = np.zeros(self.vals.shape)
             R = other.weights.size
             N = self.ndims
             for r in range(R):
                 tvals = other.weights[r] * self.vals
                 for n in range(N):
-                    # Note other[n][:, r] extracts 1-D instead of column vector, which necessitates [:, None]
+                    # Note other[n][:, r] extracts 1-D instead of column vector,
+                    # which necessitates [:, None]
                     v = other[n][:, r][:, None]
                     tvals = tvals * v[csubs[:, n]]
                 cvals += tvals
             return ttb.sptensor.from_data(csubs, cvals, self.shape)
-        else:
-            assert False, "Sptensor cannot be multiplied by that type of object"
+        assert False, "Sptensor cannot be multiplied by that type of object"
 
     def __rmul__(self, other):
         """
         Element wise right multiplication (*) for sptensors
 
         Parameters
         ----------
@@ -1905,30 +2016,31 @@
 
         Returns
         -------
         :class:`pyttb.sptensor`
         """
         if isinstance(other, (float, int, np.number)):
             return self.__mul__(other)
-        else:
-            assert False, "This object cannot be multiplied by sptensor"
+        assert False, "This object cannot be multiplied by sptensor"
 
+    # pylint:disable=too-many-branches
     def __le__(self, other):
         """
         Less than or equal (<=) for sptensor
 
         Parameters
         ----------
         other: :class:`pyttb.sptensor`, :class:`pyttb.tensor`, float, int
 
         Returns
         -------
         :class:`pyttb.sptensor`
         """
-        # TODO le,lt,ge,gt have a lot of code duplication, look at generalizing them for future maintainabilty
+        # TODO le,lt,ge,gt have a lot of code duplication, look at generalizing them
+        #  for future maintainabilty
         # Case 1: One argument is a scalar
         if isinstance(other, (float, int)):
             subs1 = self.subs[(self.vals <= other).transpose()[0], :]
             if other >= 0:
                 subs2 = self.allsubs()[
                     ttb.tt_setdiff_rows(self.allsubs(), self.subs), :
                 ]
@@ -2006,14 +2118,15 @@
             return ttb.sptensor.from_data(
                 subs, True * np.ones((len(subs), 1)), self.shape
             )
 
         # Otherwise
         assert False, "Cannot compare sptensor with that type"
 
+    # pylint:disable=too-many-branches
     def __lt__(self, other):
         """
         Less than (<) for sptensor
 
         Parameters
         ----------
         other: :class:`pyttb.sptensor`, :class:`pyttb.tensor`, float, int
@@ -2207,14 +2320,15 @@
                 True * np.ones((len(subs1) + len(subs2), 1)),
                 self.shape,
             )
 
         # Otherwise
         assert False, "Cannot compare sptensor with that type"
 
+    # pylint:disable=too-many-statements, too-many-branches, too-many-locals
     def __truediv__(self, other):
         """
         Division for sparse tensors (sptensor/other).
 
         Parameters
         ----------
         other
@@ -2224,15 +2338,16 @@
 
         """
 
         # Divide by a scalar -> result is sparse
         if isinstance(other, (float, int)):
             # Inline mrdivide
             newsubs = self.subs
-            # We ignore the divide by zero errors because np.inf/np.nan is an appropriate representation
+            # We ignore the divide by zero errors because np.inf/np.nan is an
+            # appropriate representation
             with np.errstate(divide="ignore", invalid="ignore"):
                 newvals = self.vals / other
             if other == 0:
                 nansubsidx = ttb.tt_setdiff_rows(self.allsubs(), newsubs)
                 nansubs = self.allsubs()[nansubsidx]
                 newsubs = np.vstack((newsubs, nansubs))
                 newvals = np.vstack((newvals, np.nan * np.ones((nansubs.shape[0], 1))))
@@ -2293,19 +2408,19 @@
             morevals.fill(np.nan)
             if moresubs.size > 0:
                 newsubs = np.vstack((newsubs, SelfZeroSubs[moresubs, :]))
                 newvals = np.vstack((newvals, morevals))
 
             return ttb.sptensor.from_data(newsubs, newvals, self.shape)
 
-        elif isinstance(other, ttb.tensor):
+        if isinstance(other, ttb.tensor):
             csubs = self.subs
             cvals = self.vals / other[csubs, "extract"][:, None]
             return ttb.sptensor.from_data(csubs, cvals, self.shape)
-        elif isinstance(other, ttb.ktensor):
+        if isinstance(other, ttb.ktensor):
             # TODO consider removing epsilon and generating nans consistent with above
             epsilon = np.finfo(float).eps
             subs = self.subs
             vals = np.zeros(self.vals.shape)
             R = (other.weights).size
             N = self.ndims
             for r in range(R):
@@ -2313,16 +2428,15 @@
                 for n in range(N):
                     v = other[n][:, r][:, None]
                     tvals = tvals * v[subs[:, n]]
                 vals += tvals
             return ttb.sptensor.from_data(
                 self.subs, self.vals / np.maximum(epsilon, vals), self.shape
             )
-        else:
-            assert False, "Invalid arguments for sptensor division"
+        assert False, "Invalid arguments for sptensor division"
 
     def __rtruediv__(self, other):
         """
         Right Division for sparse tensors (other/sptensor).
 
         Parameters
         ----------
@@ -2331,16 +2445,15 @@
         Returns
         -------
 
         """
         # Scalar divided by a tensor -> result is dense
         if isinstance(other, (float, int)):
             return other / self.full()
-        else:
-            assert False, "Dividing that object by an sptensor is not supported"
+        assert False, "Dividing that object by an sptensor is not supported"
 
     def __repr__(self):  # pragma: no cover
         """
         String representation of a sparse tensor.
 
         Returns
         -------
@@ -2351,38 +2464,43 @@
         if nz == 0:
             s = "All-zero sparse tensor of shape "
             if self.ndims == 0:
                 s += str(self.shape)
                 return s
             s += (" x ").join([str(int(d)) for d in self.shape])
             return s
-        else:
-            s = "Sparse tensor of shape "
-            s += (" x ").join([str(int(d)) for d in self.shape])
-            s += " with {} nonzeros \n".format(nz)
+
+        s = "Sparse tensor of shape "
+        s += (" x ").join([str(int(d)) for d in self.shape])
+        s += f" with {nz} nonzeros \n"
 
         # Stop insane printouts
         if nz > 10000:
             r = input("Are you sure you want to print all nonzeros? (Y/N)")
             if r.upper() != "Y":
                 return s
-        for i, j in enumerate(range(0, self.subs.shape[0])):
+        for i in range(0, self.subs.shape[0]):
             s += "\t"
             s += "["
             idx = self.subs[i, :]
             s += str(idx.tolist())[1:]
             s += " = "
             s += str(self.vals[i][0])
             if i < self.subs.shape[0] - 1:
                 s += "\n"
         return s
 
     __str__ = __repr__
 
-    def ttm(self, matrices, dims=None, transpose=False):
+    def ttm(
+        self,
+        matrices: Union[np.ndarray, List[np.ndarray]],
+        dims: Optional[Union[float, np.ndarray]] = None,
+        transpose: bool = False,
+    ):
         """
         Sparse tensor times matrix.
 
         Parameters
         ----------
         matrices: A matrix or list of matrices
         dims: :class:`Numpy.ndarray`, int
@@ -2392,15 +2510,15 @@
         -------
 
         """
         if dims is None:
             dims = np.arange(self.ndims)
         elif isinstance(dims, list):
             dims = np.array(dims)
-        elif np.isscalar(dims) or isinstance(dims, list):
+        elif isinstance(dims, (float, int, np.generic)):
             dims = np.array([dims])
 
         # Handle list of matrices
         if isinstance(matrices, list):
             # Check dimensions are valid
             [dims, vidx] = tt_dimscheck(dims, self.ndims, len(matrices))
             # Calculate individual products
@@ -2416,37 +2534,37 @@
         # Flip matrices if transposed
         if transpose:
             matrices = matrices.transpose()
 
         # Ensure this is the terminal single dimension case
         if not (dims.size == 1 and np.isin(dims, np.arange(self.ndims))):
             assert False, "dims must contain values in [0,self.dims)"
-        dims = dims[0]
+        final_dim: int = dims[0]
 
         # Compute the product
 
         # Check that sizes match
-        if self.shape[dims] != matrices.shape[1]:
+        if self.shape[final_dim] != matrices.shape[1]:
             assert False, "Matrix shape doesn't match tensor shape"
 
         # Compute the new size
         siz = np.array(self.shape)
-        siz[dims] = matrices.shape[0]
+        siz[final_dim] = matrices.shape[0]
 
         # Compute self[mode]'
-        Xnt = ttb.tt_to_sparse_matrix(self, dims, True)
+        Xnt = tt_to_sparse_matrix(self, final_dim, True)
 
-        # Reshape puts the reshaped things after the unchanged modes, transpose then puts it in front
+        # Reshape puts the reshaped things after the unchanged modes, transpose then
+        # puts it in front
         idx = 0
 
         # Convert to sparse matrix and do multiplication; generally result is sparse
         Z = Xnt.dot(matrices.transpose())
 
         # Rearrange back into sparse tensor of correct shape
-        Ynt = ttb.tt_from_sparse_matrix(Z, siz, dims, idx)
+        Ynt = tt_from_sparse_matrix(Z, siz, final_dim, idx)
 
         if not isinstance(Z, np.ndarray) and Z.nnz <= 0.5 * np.prod(siz):
             return Ynt
-        else:
-            # TODO evaluate performance loss by casting into sptensor then tensor. I assume minimal since we are already
-            # using spare matrix representation
-            return ttb.tensor.from_tensor_type(Ynt)
+        # TODO evaluate performance loss by casting into sptensor then tensor.
+        #  I assume minimal since we are already using spare matrix representation
+        return ttb.tensor.from_tensor_type(Ynt)
```

### Comparing `pyttb-1.5.0/pyttb/sumtensor.py` & `pyttb-1.5.1/pyttb/sumtensor.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb/tenmat.py` & `pyttb-1.5.1/pyttb/tenmat.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb/tensor.py` & `pyttb-1.5.1/pyttb/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # U.S. Government retains certain rights in this software.
 """Dense Tensor Implementation"""
 from __future__ import annotations
 
 import warnings
 from itertools import permutations
 from math import factorial
-from typing import Any, Callable, List, Literal, Optional, Tuple, Union
+from typing import Any, Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import scipy.sparse.linalg
 from numpy_groupies import aggregate as accumarray
 
 import pyttb as ttb
 from pyttb.pyttb_utils import tt_dimscheck, tt_ind2sub
@@ -175,17 +175,15 @@
 
         # Create the tensor
         return cls.from_data(data, shape)
 
     def collapse(
         self,
         dims: Optional[np.ndarray] = None,
-        fun: Union[
-            Literal["sum"], Callable[[np.ndarray], Union[float, np.ndarray]]
-        ] = "sum",
+        fun: Callable[[np.ndarray], Union[float, np.ndarray]] = np.sum,
     ) -> Union[float, np.ndarray, tensor]:
         """
         Collapse tensor along specified dimensions.
 
         Parameters
         ----------
         dims: Dimensions to collapse
@@ -196,15 +194,15 @@
         Collapsed value
 
         Example
         -------
         >>> X = ttb.tensor.from_data(np.ones((2,2)))
         >>> X.collapse()
         4.0
-        >>> X.collapse(np.arange(X.ndims), lambda values: sum(values))
+        >>> X.collapse(np.arange(X.ndims), sum)
         4.0
         """
         if self.data.size == 0:
             return np.array([])
 
         if dims is None:
             dims = np.arange(0, self.ndims)
@@ -213,31 +211,26 @@
             return ttb.tensor.from_tensor_type(self)
 
         dims, _ = tt_dimscheck(dims, self.ndims)
         remdims = np.setdiff1d(np.arange(0, self.ndims), dims)
 
         # Check for the case where we accumulate over *all* dimensions
         if remdims.size == 0:
-            if fun == "sum":
-                return sum(self.data.flatten("F"))
             return fun(self.data.flatten("F"))
 
         ## Calculate the shape of the result
         newshape = tuple(np.array(self.shape)[remdims])
 
         ## Convert to a matrix where each row is going to be collapsed
         A = ttb.tenmat.from_data(self.data, remdims, dims).double()
 
         ## Apply the collapse function
         B = np.zeros((A.shape[0], 1))
         for i in range(0, A.shape[0]):
-            if fun == "sum":
-                B[i] = np.sum(A[i, :])
-            else:
-                B[i] = fun(A[i, :])
+            B[i] = fun(A[i, :])
 
         ## Form and return the final result
         return ttb.tensor.from_data(B, newshape)
 
     def contract(self, i: int, j: int) -> Union[np.ndarray, tensor]:
         """
         Contract tensor along two dimensions (array trace).
@@ -409,15 +402,15 @@
             y = np.reshape(other.data, (other.data.size,), order="F")
             return x.dot(y)
         if isinstance(other, (ttb.ktensor, ttb.sptensor, ttb.ttensor)):
             # Reverse arguments and call specializer code
             return other.innerprod(self)
         assert False, "Inner product between tensor and that class is not supported"
 
-    def isequal(self, other: Union[tensor, ttb.sptensor]) -> Union[bool, np.bool_]:
+    def isequal(self, other: Union[tensor, ttb.sptensor]) -> bool:
         """
         Exact equality for tensors
 
         Parameters
         ----------
         other: Tensor to compare against
 
@@ -425,17 +418,17 @@
         --------
         >>> X = ttb.tensor.from_data(np.ones((2,2)))
         >>> Y = ttb.tensor.from_data(np.zeros((2,2)))
         >>> X.isequal(Y)
         False
         """
         if isinstance(other, ttb.tensor):
-            return np.all(self.data == other.data)
+            return bool(np.all(self.data == other.data))
         if isinstance(other, ttb.sptensor):
-            return np.all(self.data == other.full().data)
+            return bool(np.all(self.data == other.full().data))
         return False
 
     # TODO: We should probably always return details and let caller drop them
     # pylint: disable=too-many-branches, too-many-locals
     def issymmetric(
         self,
         grps: Optional[np.ndarray] = None,
```

### Comparing `pyttb-1.5.0/pyttb/ttensor.py` & `pyttb-1.5.1/pyttb/ttensor.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb/tucker_als.py` & `pyttb-1.5.1/pyttb/tucker_als.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/pyttb.egg-info/PKG-INFO` & `pyttb-1.5.1/pyttb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyttb
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python Tensor Toolbox
-Home-page: 
-Author: Daniel M. Dunlavy
+Author: Nick Johnson
 Author-email: "Daniel M. Dunlavy" <dmdunla@sandia.gov>
 License: BSD 2-Clause License
 Project-URL: homepage, https://github.com/sandialabs/pyttb
 Project-URL: coverage, https://coveralls.io/github/sandialabs/pyttb
 Project-URL: documentation, https://pyttb.readthedocs.io
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: testing
+Provides-Extra: dev
+Provides-Extra: doc
 License-File: LICENSE
 
 ```
 Copyright 2022 National Technology & Engineering Solutions of Sandia,
 LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 U.S. Government retains certain rights in this software.
 ```
```

### Comparing `pyttb-1.5.0/pyttb.egg-info/SOURCES.txt` & `pyttb-1.5.1/pyttb.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
-./pyttb/__init__.py
-./pyttb/cp_als.py
-./pyttb/cp_apr.py
-./pyttb/export_data.py
-./pyttb/hosvd.py
-./pyttb/import_data.py
-./pyttb/khatrirao.py
-./pyttb/ktensor.py
-./pyttb/pyttb_utils.py
-./pyttb/sptenmat.py
-./pyttb/sptensor.py
-./pyttb/sptensor3.py
-./pyttb/sumtensor.py
-./pyttb/symktensor.py
-./pyttb/symtensor.py
-./pyttb/tenmat.py
-./pyttb/tensor.py
-./pyttb/ttensor.py
-./pyttb/tucker_als.py
+pyttb/__init__.py
+pyttb/cp_als.py
+pyttb/cp_apr.py
+pyttb/export_data.py
+pyttb/hosvd.py
+pyttb/import_data.py
+pyttb/khatrirao.py
+pyttb/ktensor.py
+pyttb/pyttb_utils.py
+pyttb/sptenmat.py
+pyttb/sptensor.py
+pyttb/sptensor3.py
+pyttb/sumtensor.py
+pyttb/symktensor.py
+pyttb/symtensor.py
+pyttb/tenmat.py
+pyttb/tensor.py
+pyttb/ttensor.py
+pyttb/tucker_als.py
 pyttb.egg-info/PKG-INFO
 pyttb.egg-info/SOURCES.txt
 pyttb.egg-info/dependency_links.txt
 pyttb.egg-info/requires.txt
 pyttb.egg-info/top_level.txt
 tests/test_cp_als.py
 tests/test_cp_apr.py
```

### Comparing `pyttb-1.5.0/tests/test_cp_als.py` & `pyttb-1.5.1/tests/test_cp_als.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/tests/test_cp_apr.py` & `pyttb-1.5.1/tests/test_cp_apr.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/tests/test_hosvd.py` & `pyttb-1.5.1/tests/test_hosvd.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,11 +111,13 @@
     fm2 = np.array(
         [
             [-1.922305666539489e-01, 8.924016710972924e-01],
             [-5.140779746206554e-01, 2.627873081852611e-01],
             [-8.359253825873615e-01, -3.668270547267537e-01],
         ]
     )
-    assert np.allclose(M.core.data, core)
-    assert np.allclose(M.u[0], fm0)
-    assert np.allclose(M.u[1], fm1)
-    assert np.allclose(M.u[2], fm2)
+    expected = ttb.ttensor.from_data(ttb.tensor.from_data(core), [fm0, fm1, fm2])
+    assert np.allclose(M.double(), expected.double())
+    assert np.allclose(np.abs(M.core.data), np.abs(core))
+    assert np.allclose(np.abs(M.u[0]), np.abs(fm0))
+    assert np.allclose(np.abs(M.u[1]), np.abs(fm1))
+    assert np.allclose(np.abs(M.u[2]), np.abs(fm2))
```

### Comparing `pyttb-1.5.0/tests/test_import_export_data.py` & `pyttb-1.5.1/tests/test_import_export_data.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/tests/test_khatrirao.py` & `pyttb-1.5.1/tests/test_khatrirao.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/tests/test_ktensor.py` & `pyttb-1.5.1/tests/test_ktensor.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/tests/test_package.py` & `pyttb-1.5.1/tests/test_package.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,32 +9,39 @@
 
 @pytest.mark.packaging
 def test_formatting():
     """Confirm formatting of the project is consistent"""
 
     source_dir = os.path.dirname(ttb.__file__)
     root_dir = os.path.dirname(source_dir)
-    subprocess.run(f"isort {root_dir} --check --settings-path {root_dir}", check=True)
-    subprocess.run(f"black --check {root_dir}", check=True)
+    subprocess.run(
+        f"isort {root_dir} --check --settings-path {root_dir}", check=True, shell=True
+    )
+    subprocess.run(f"black --check {root_dir}", check=True, shell=True)
 
 
 @pytest.mark.packaging
 def test_linting():
     """Confirm linting of the project is enforce"""
 
     enforced_files = [
         os.path.join(os.path.dirname(ttb.__file__), f"{ttb.tensor.__name__}.py"),
+        os.path.join(os.path.dirname(ttb.__file__), f"{ttb.sptensor.__name__}.py"),
+        ttb.pyttb_utils.__file__,
     ]
     # TODO pylint fails to import pyttb in tests
     # add mypy check
     root_dir = os.path.dirname(os.path.dirname(__file__))
     toml_file = os.path.join(root_dir, "pyproject.toml")
-    for a_file in enforced_files:
-        subprocess.run(f"pylint {a_file} --rcfile {toml_file}", check=True)
+    subprocess.run(
+        f"pylint {' '.join(enforced_files)} --rcfile {toml_file} -j0",
+        check=True,
+        shell=True,
+    )
 
 
 @pytest.mark.packaging
 def test_typing():
     """Run type checker on package"""
     root_dir = os.path.dirname(os.path.dirname(__file__))
     toml_file = os.path.join(root_dir, "pyproject.toml")
-    subprocess.run(f"mypy -p pyttb  --config-file {toml_file}", check=True)
+    subprocess.run(f"mypy -p pyttb  --config-file {toml_file}", check=True, shell=True)
```

### Comparing `pyttb-1.5.0/tests/test_pyttb_utils.py` & `pyttb-1.5.1/tests/test_pyttb_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,50 +48,14 @@
         tensorCopy = ttb.tensor.from_tensor_type(tensorInstance)
         Xnt = ttb.tt_to_dense_matrix(tensorCopy, mode, False)
         Ynt = ttb.tt_from_dense_matrix(Xnt, tensorCopy.shape, mode, 1)
         assert tensorCopy.isequal(Ynt)
 
 
 @pytest.mark.indevelopment
-def test_sptensor_to_sparse_matrix():
-    subs = np.array([[1, 1, 1], [1, 1, 3], [2, 2, 2], [3, 3, 3]])
-    vals = np.array([[0.5], [1.5], [2.5], [3.5]])
-    shape = (4, 4, 4)
-    mode0 = sparse.coo_matrix(([0.5, 1.5, 2.5, 3.5], ([5, 13, 10, 15], [1, 1, 2, 3])))
-    mode1 = sparse.coo_matrix(([0.5, 1.5, 2.5, 3.5], ([5, 13, 10, 15], [1, 1, 2, 3])))
-    mode2 = sparse.coo_matrix(([0.5, 1.5, 2.5, 3.5], ([5, 5, 10, 15], [1, 3, 2, 3])))
-    Ynt = [mode0, mode1, mode2]
-    sptensorInstance = ttb.sptensor().from_data(subs, vals, shape)
-
-    for mode in range(sptensorInstance.ndims):
-        Xnt = ttb.tt_to_sparse_matrix(sptensorInstance, mode, True)
-        assert (Xnt != Ynt[mode]).nnz == 0
-        assert Xnt.shape == Ynt[mode].shape
-
-
-@pytest.mark.indevelopment
-def test_sptensor_from_sparse_matrix():
-    subs = np.array([[1, 1, 1], [1, 1, 3], [2, 2, 2], [3, 3, 3]])
-    vals = np.array([[0.5], [1.5], [2.5], [3.5]])
-    shape = (4, 4, 4)
-    sptensorInstance = ttb.sptensor().from_data(subs, vals, shape)
-    for mode in range(sptensorInstance.ndims):
-        sptensorCopy = ttb.sptensor.from_tensor_type(sptensorInstance)
-        Xnt = ttb.tt_to_sparse_matrix(sptensorCopy, mode, True)
-        Ynt = ttb.tt_from_sparse_matrix(Xnt, sptensorCopy.shape, mode, 0)
-        assert sptensorCopy.isequal(Ynt)
-
-    for mode in range(sptensorInstance.ndims):
-        sptensorCopy = ttb.sptensor.from_tensor_type(sptensorInstance)
-        Xnt = ttb.tt_to_sparse_matrix(sptensorCopy, mode, False)
-        Ynt = ttb.tt_from_sparse_matrix(Xnt, sptensorCopy.shape, mode, 1)
-        assert sptensorCopy.isequal(Ynt)
-
-
-@pytest.mark.indevelopment
 def test_tt_union_rows():
     a = np.array([[4, 6], [1, 9], [2, 6], [2, 6], [99, 0]])
     b = np.array([[1, 7], [1, 8], [2, 6]])
     assert (
         ttb.tt_union_rows(a, b)
         == np.array([[1, 7], [1, 8], [4, 6], [1, 9], [2, 6], [99, 0]])
     ).all()
```

### Comparing `pyttb-1.5.0/tests/test_sptensor.py` & `pyttb-1.5.1/tests/test_sptensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 
 import numpy as np
 import pytest
 import scipy.sparse as sparse
 
 import pyttb as ttb
+from pyttb.sptensor import tt_from_sparse_matrix, tt_to_sparse_matrix
 
 
 @pytest.fixture()
 def sample_sptensor():
     subs = np.array([[1, 1, 1], [1, 1, 3], [2, 2, 2], [3, 3, 3]])
     vals = np.array([[0.5], [1.5], [2.5], [3.5]])
     shape = (4, 4, 4)
@@ -226,14 +227,17 @@
         sptensorInstance.subdims((1, 1, slice(None, None, None))) == np.array([0, 1])
     ).all()
 
     with pytest.raises(AssertionError) as excinfo:
         sptensorInstance.subdims([[1], [1, 3]])
     assert "Number of subdimensions must equal number of dimensions" in str(excinfo)
 
+    with pytest.raises(ValueError):
+        sptensorInstance.subdims(("bad", "region", "types"))
+
 
 @pytest.mark.indevelopment
 def test_sptensor_ndims(sample_sptensor):
     (data, sptensorInstance) = sample_sptensor
 
     assert sptensorInstance.ndims == 3
 
@@ -1127,15 +1131,15 @@
     with pytest.raises(AssertionError) as excinfo:
         sptensorInstance.innerprod(ttb.tensor.from_data(np.array([1])))
     assert "Sptensor and tensor must be same shape for innerproduct" in str(excinfo)
 
     # Wrong type for innerprod
     with pytest.raises(AssertionError) as excinfo:
         sptensorInstance.innerprod(5)
-    assert "Inner product between sptensor and that class not supported" in str(excinfo)
+    assert f"Inner product between sptensor and {type(5)} not supported" in str(excinfo)
 
 
 @pytest.mark.indevelopment
 def test_sptensor_logical_xor(sample_sptensor):
     (data, sptensorInstance) = sample_sptensor
     nonZeroMatrix = np.zeros(data["shape"])
     nonZeroMatrix[tuple(data["subs"].transpose())] = 1
@@ -1628,14 +1632,21 @@
         ans[1, 2] = 1
         assert np.allclose((sptensorInstance.nvecs(1, 3)), ans)
     assert (
         "Greater than or equal to sptensor.shape[n] - 1 eigenvectors requires cast to dense to solve"
         in str(record[0].message)
     )
 
+    # Negative test, check for only singleton dims
+    with pytest.raises(ValueError):
+        single_val_sptensor = ttb.sptensor.from_data(
+            np.array([[0, 0]]), np.array([1]), shape=(1, 1)
+        )
+        single_val_sptensor.nvecs(0, 0)
+
 
 @pytest.mark.indevelopment
 def test_sptensor_ttm(sample_sptensor):
     (data, sptensorInstance) = sample_sptensor
     result = np.zeros((4, 4, 4))
     result[:, 1, 1] = 0.5
     result[:, 1, 3] = 1.5
@@ -1704,7 +1715,43 @@
 
     # Confirm reshape for non-square matrix
     assert sptensorInstance.ttm(sparse.coo_matrix(np.ones((1, 4))), dims=2).shape == (
         4,
         4,
         1,
     )
+
+
+@pytest.mark.indevelopment
+def test_sptensor_to_sparse_matrix():
+    subs = np.array([[1, 1, 1], [1, 1, 3], [2, 2, 2], [3, 3, 3]])
+    vals = np.array([[0.5], [1.5], [2.5], [3.5]])
+    shape = (4, 4, 4)
+    mode0 = sparse.coo_matrix(([0.5, 1.5, 2.5, 3.5], ([5, 13, 10, 15], [1, 1, 2, 3])))
+    mode1 = sparse.coo_matrix(([0.5, 1.5, 2.5, 3.5], ([5, 13, 10, 15], [1, 1, 2, 3])))
+    mode2 = sparse.coo_matrix(([0.5, 1.5, 2.5, 3.5], ([5, 5, 10, 15], [1, 3, 2, 3])))
+    Ynt = [mode0, mode1, mode2]
+    sptensorInstance = ttb.sptensor().from_data(subs, vals, shape)
+
+    for mode in range(sptensorInstance.ndims):
+        Xnt = tt_to_sparse_matrix(sptensorInstance, mode, True)
+        assert (Xnt != Ynt[mode]).nnz == 0
+        assert Xnt.shape == Ynt[mode].shape
+
+
+@pytest.mark.indevelopment
+def test_sptensor_from_sparse_matrix():
+    subs = np.array([[1, 1, 1], [1, 1, 3], [2, 2, 2], [3, 3, 3]])
+    vals = np.array([[0.5], [1.5], [2.5], [3.5]])
+    shape = (4, 4, 4)
+    sptensorInstance = ttb.sptensor().from_data(subs, vals, shape)
+    for mode in range(sptensorInstance.ndims):
+        sptensorCopy = ttb.sptensor.from_tensor_type(sptensorInstance)
+        Xnt = tt_to_sparse_matrix(sptensorCopy, mode, True)
+        Ynt = tt_from_sparse_matrix(Xnt, sptensorCopy.shape, mode, 0)
+        assert sptensorCopy.isequal(Ynt)
+
+    for mode in range(sptensorInstance.ndims):
+        sptensorCopy = ttb.sptensor.from_tensor_type(sptensorInstance)
+        Xnt = tt_to_sparse_matrix(sptensorCopy, mode, False)
+        Ynt = tt_from_sparse_matrix(Xnt, sptensorCopy.shape, mode, 1)
+        assert sptensorCopy.isequal(Ynt)
```

### Comparing `pyttb-1.5.0/tests/test_tenmat.py` & `pyttb-1.5.1/tests/test_tenmat.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/tests/test_tensor.py` & `pyttb-1.5.1/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/tests/test_ttensor.py` & `pyttb-1.5.1/tests/test_ttensor.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.0/tests/test_tucker_als.py` & `pyttb-1.5.1/tests/test_tucker_als.py`

 * *Files identical despite different names*

