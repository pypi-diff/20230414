# Comparing `tmp/libmultilabel-0.1.9.tar.gz` & `tmp/libmultilabel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/LibMultiLabel/LibMultiLabel/dist/.tmp-7rhbj1hd/libmultilabel-0.1.9.tar", last modified: Fri Feb 17 12:57:46 2023, max compression
+gzip compressed data, was "/home/runner/work/LibMultiLabel/LibMultiLabel/dist/.tmp-mea1opt5/libmultilabel-0.2.0.tar", last modified: Fri Apr 14 13:27:40 2023, max compression
```

## Comparing `libmultilabel-0.1.9.tar` & `libmultilabel-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/libmultilabel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/libmultilabel/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18768 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/linear/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/linear/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/linear/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/linear/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/libmultilabel/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16948 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/libmultilabel/nn/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/networks/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/networks/bert_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/networks/caml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/networks/kim_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/networks/labelwise_attention_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/networks/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/networks/xml_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/libmultilabel/nn/nn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/libmultilabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/libmultilabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/libmultilabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/libmultilabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/libmultilabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/libmultilabel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-17 12:57:33.000000 libmultilabel-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-17 12:57:46.000000 libmultilabel-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22422 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/bert_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/caml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/kim_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/labelwise_attention_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/xml_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/nn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/setup.cfg
```

### Comparing `libmultilabel-0.1.9/LICENSE` & `libmultilabel-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/PKG-INFO` & `libmultilabel-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.1.9
+Version: 0.2.0
 Summary: A library for multi-label text classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
```

### Comparing `libmultilabel-0.1.9/README.md` & `libmultilabel-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/libmultilabel/common_utils.py` & `libmultilabel-0.2.0/libmultilabel/common_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/libmultilabel/linear/linear.py` & `libmultilabel-0.2.0/libmultilabel/linear/linear.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,102 @@
+from __future__ import annotations
+
 import logging
 import os
 
 import numpy as np
 import scipy.sparse as sparse
 from liblinear.liblinearutil import train
 from tqdm import tqdm
 
 __all__ = ['train_1vsrest',
            'train_thresholding',
            'train_cost_sensitive',
            'train_cost_sensitive_micro',
            'train_binary_and_multiclass',
-           'predict_values']
+           'predict_values',
+           'get_topk_labels']
 
 
-def train_1vsrest(y: sparse.csr_matrix, x: sparse.csr_matrix, options: str):
+class FlatModel:
+    def __init__(self, name: str,
+                 weights: np.matrix,
+                 bias: float,
+                 thresholds: float | np.ndarray,
+                 ):
+        self.name = name
+        self.weights = weights
+        self.bias = bias
+        self.thresholds = thresholds
+
+    def predict_values(self, x: sparse.csr_matrix) -> np.ndarray:
+        """Calculates the decision values associated with x.
+
+        Args:
+            x (sparse.csr_matrix): A matrix with dimension number of instances * number of features.
+
+        Returns:
+            np.ndarray: A matrix with dimension number of instances * number of classes.
+        """
+        bias = self.bias
+        bias_col = np.full((x.shape[0], 1 if bias > 0 else 0), bias)
+        num_feature = self.weights.shape[0]
+        num_feature -= 1 if bias > 0 else 0
+        if x.shape[1] < num_feature:
+            x = sparse.hstack([
+                x,
+                np.zeros((x.shape[0], num_feature - x.shape[1])),
+                bias_col,
+            ], 'csr')
+        else:
+            x = sparse.hstack([
+                x[:, :num_feature],
+                bias_col,
+            ], 'csr')
+
+        return (x * self.weights).A + self.thresholds
+
+
+def train_1vsrest(y: sparse.csr_matrix,
+                  x: sparse.csr_matrix,
+                  options: str = '',
+                  verbose: bool = True
+                  ) -> FlatModel:
     """Trains a linear model for multiabel data using a one-vs-rest strategy.
 
     Args:
         y (sparse.csr_matrix): A 0/1 matrix with dimensions number of instances * number of classes.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
-        options (str): The option string passed to liblinear.
+        options (str, optional): The option string passed to liblinear. Defaults to ''.
+        verbose (bool, optional): Output extra progress information. Defaults to True.
 
     Returns:
         A model which can be used in predict_values.
     """
     # Follows the MATLAB implementation at https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/multilabel/
-    x, options, bias = prepare_options(x, options)
+    x, options, bias = _prepare_options(x, options)
 
     y = y.tocsc()
     num_class = y.shape[1]
     num_feature = x.shape[1]
     weights = np.zeros((num_feature, num_class), order='F')
 
-    logging.info(f'Training one-vs-rest model on {num_class} labels')
-    for i in tqdm(range(num_class)):
+    if verbose:
+        logging.info(f'Training one-vs-rest model on {num_class} labels')
+    for i in tqdm(range(num_class), disable=not verbose):
         yi = y[:, i].toarray().reshape(-1)
-        weights[:, i] = do_train(2*yi - 1, x, options).ravel()
+        weights[:, i] = _do_train(2*yi - 1, x, options).ravel()
 
-    return {'weights': np.asmatrix(weights), '-B': bias, 'threshold': 0}
+    return FlatModel(name='1vsrest',
+                     weights=np.asmatrix(weights),
+                     bias=bias,
+                     thresholds=0)
 
 
-def prepare_options(x: sparse.csr_matrix, options: str) -> 'tuple[sparse.csr_matrix, str, float]':
+def _prepare_options(x: sparse.csr_matrix, options: str) -> tuple[sparse.csr_matrix, str, float]:
     """Prepare options and x for multi-label training. Called in the first line of
     any training function.
 
     Args:
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
 
@@ -61,14 +112,17 @@
     options_split = options.split()
     if '-s' in options_split:
         i = options_split.index('-s')
         solver_type = int(options_split[i+1])
         if solver_type < 0 or solver_type > 7:
             raise ValueError(
                 "Invalid LIBLINEAR solver type. Only classification solvers are allowed.")
+    else:
+        # workaround for liblinear warning about unspecified solver
+        options_split.extend(['-s', '2'])
 
     bias = -1.
     if '-B' in options_split:
         i = options_split.index('-B')
         bias = float(options_split[i+1])
         options_split = options_split[:i] + options_split[i+2:]
         x = sparse.hstack([
@@ -80,52 +134,61 @@
     if not '-m' in options:
         options_split.append(f'-m {int(os.cpu_count() / 2)}')
 
     options = ' '.join(options_split)
     return x, options, bias
 
 
-def train_thresholding(y: sparse.csr_matrix, x: sparse.csr_matrix, options: str):
+def train_thresholding(y: sparse.csr_matrix,
+                       x: sparse.csr_matrix,
+                       options: str = '',
+                       verbose: bool = True
+                       ) -> FlatModel:
     """Trains a linear model for multilabel data using a one-vs-rest strategy
-    and cross-validation to pick an optimal decision threshold for Macro-F1.
+    and cross-validation to pick optimal decision thresholds for Macro-F1.
     Outperforms train_1vsrest in most aspects at the cost of higher
     time complexity.
     See user guide for more details.
 
     Args:
         y (sparse.csr_matrix): A 0/1 matrix with dimensions number of instances * number of classes.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
-        options (str): The option string passed to liblinear.
+        options (str, optional): The option string passed to liblinear. Defaults to ''.
+        verbose (bool, optional): Output extra progress information. Defaults to True.
 
     Returns:
         A model which can be used in predict_values.
     """
     # Follows the MATLAB implementation at https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/multilabel/
-    x, options, bias = prepare_options(x, options)
+    x, options, bias = _prepare_options(x, options)
 
     y = y.tocsc()
     num_class = y.shape[1]
     num_feature = x.shape[1]
     weights = np.zeros((num_feature, num_class), order='F')
     thresholds = np.zeros(num_class)
 
-    logging.info(f'Training thresholding model on {num_class} labels')
-    for i in tqdm(range(num_class)):
+    if verbose:
+        logging.info(f'Training thresholding model on {num_class} labels')
+    for i in tqdm(range(num_class), disable=not verbose):
         yi = y[:, i].toarray().reshape(-1)
-        w, t = thresholding_one_label(2*yi - 1, x, options)
+        w, t = _thresholding_one_label(2*yi - 1, x, options)
         weights[:, i] = w.ravel()
         thresholds[i] = t
 
-    return {'weights': np.asmatrix(weights), '-B': bias, 'threshold': thresholds}
+    return FlatModel(name='thresholding',
+                     weights=np.asmatrix(weights),
+                     bias=bias,
+                     thresholds=thresholds)
 
 
-def thresholding_one_label(y: np.ndarray,
-                           x: sparse.csr_matrix,
-                           options: str
-                           ) -> 'tuple[np.ndarray, float]':
+def _thresholding_one_label(y: np.ndarray,
+                            x: sparse.csr_matrix,
+                            options: str
+                            ) -> tuple[np.ndarray, float]:
     """Outer cross-validation for thresholding on a single label.
 
     Args:
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
 
@@ -144,37 +207,37 @@
 
     for fold in range(nr_fold):
         mask = np.zeros_like(perm, dtype='?')
         mask[np.arange(int(fold*l/nr_fold), int((fold+1)*l/nr_fold))] = 1
         val_idx = perm[mask]
         train_idx = perm[mask != True]
 
-        scutfbr_w, scutfbr_b_list = scutfbr(
+        scutfbr_w, scutfbr_b_list = _scutfbr(
             y[train_idx], x[train_idx], fbr_list, options)
         wTx = (x[val_idx] * scutfbr_w).A1
 
         for i in range(fbr_list.size):
-            F = fmeasure(y[val_idx], 2*(wTx > -scutfbr_b_list[i]) - 1)
+            F = _fmeasure(y[val_idx], 2*(wTx > -scutfbr_b_list[i]) - 1)
             f_list[i] += F
 
     best_fbr = fbr_list[::-1][np.argmax(f_list[::-1])]  # last largest
     if np.max(f_list) == 0:
         best_fbr = np.min(fbr_list)
 
     # final model
-    w, b_list = scutfbr(y, x, np.array([best_fbr]), options)
+    w, b_list = _scutfbr(y, x, np.array([best_fbr]), options)
 
     return w, b_list[0]
 
 
-def scutfbr(y: np.ndarray,
-            x: sparse.csr_matrix,
-            fbr_list: 'list[float]',
-            options: str
-            ) -> 'tuple[np.matrix, np.ndarray]':
+def _scutfbr(y: np.ndarray,
+             x: sparse.csr_matrix,
+             fbr_list: list[float],
+             options: str
+             ) -> tuple[np.matrix, np.ndarray]:
     """Inner cross-validation for SCutfbr heuristic.
 
     Args:
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         fbr_list (list[float]): list of fbr values.
         options (str): The option string passed to liblinear.
@@ -193,18 +256,18 @@
 
     for fold in range(nr_fold):
         mask = np.zeros_like(perm, dtype='?')
         mask[np.arange(int(fold*l/nr_fold), int((fold+1)*l/nr_fold))] = 1
         val_idx = perm[mask]
         train_idx = perm[mask != True]
 
-        w = do_train(y[train_idx], x[train_idx], options)
+        w = _do_train(y[train_idx], x[train_idx], options)
         wTx = (x[val_idx] * w).A1
         scut_b = 0.
-        start_F = fmeasure(y[val_idx], 2*(wTx > -scut_b) - 1)
+        start_F = _fmeasure(y[val_idx], 2*(wTx > -scut_b) - 1)
 
         # stableness to match the MATLAB implementation
         sorted_wTx_index = np.argsort(wTx, kind='stable')
         sorted_wTx = wTx[sorted_wTx_index]
 
         tp = np.sum(y[val_idx] == 1)
         fp = val_idx.size - tp
@@ -234,27 +297,30 @@
             if cut == -1:  # i.e. all 1 in scut
                 scut_b = np.nextafter(-sorted_wTx[0], np.inf)  # predict all 1
             elif cut == val_idx.size - 1:
                 scut_b = np.nextafter(-sorted_wTx[-1], np.inf)
             else:
                 scut_b = -(sorted_wTx[cut] + sorted_wTx[cut + 1]) / 2
 
-        F = fmeasure(y_val, 2*(wTx > -scut_b) - 1)
+        F = _fmeasure(y_val, 2*(wTx > -scut_b) - 1)
 
         for i in range(fbr_list.size):
             if F > fbr_list[i]:
                 b_list[i] += scut_b
             else:
                 b_list[i] -= np.max(wTx)
 
     b_list = b_list / nr_fold
-    return do_train(y, x, options), b_list
+    return _do_train(y, x, options), b_list
 
 
-def do_train(y: np.ndarray, x: sparse.csr_matrix, options: str) -> np.matrix:
+def _do_train(y: np.ndarray,
+              x: sparse.csr_matrix,
+              options: str
+              ) -> np.matrix:
     """Wrapper around liblinear.liblinearutil.train.
     Forcibly suppresses all IO regardless of options.
 
     Args:
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
@@ -294,15 +360,15 @@
 
     def __exit__(self, type, value, traceback):
         os.dup2(self.stderr, 2)
         os.close(self.devnull)
         os.close(self.stderr)
 
 
-def fmeasure(y_true: np.ndarray, y_pred: np.ndarray) -> float:
+def _fmeasure(y_true: np.ndarray, y_pred: np.ndarray) -> float:
     """Calculate F1 score.
 
     Args:
         y_true (np.ndarray): array of +1/-1.
         y_pred (np.ndarray): array of +1/-1.
 
     Returns:
@@ -314,52 +380,61 @@
 
     F = 0
     if tp != 0 or fp != 0 or fn != 0:
         F = 2*tp / (2*tp + fp + fn)
     return F
 
 
-def train_cost_sensitive(y: sparse.csr_matrix, x: sparse.csr_matrix, options: str):
+def train_cost_sensitive(y: sparse.csr_matrix,
+                         x: sparse.csr_matrix,
+                         options: str = '',
+                         verbose: bool = True
+                         ) -> FlatModel:
     """Trains a linear model for multilabel data using a one-vs-rest strategy
     and cross-validation to pick an optimal asymmetric misclassification cost
     for Macro-F1.
     Outperforms train_1vsrest in most aspects at the cost of higher
     time complexity.
     See user guide for more details.
 
     Args:
         y (sparse.csr_matrix): A 0/1 matrix with dimensions number of instances * number of classes.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
-        options (str): The option string passed to liblinear.
+        options (str, optional): The option string passed to liblinear. Defaults to ''.
+        verbose (bool, optional): Output extra progress information. Defaults to True.
 
     Returns:
         A model which can be used in predict_values.
     """
     # Follows the MATLAB implementation at https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/multilabel/
-    x, options, bias = prepare_options(x, options)
+    x, options, bias = _prepare_options(x, options)
 
     y = y.tocsc()
     num_class = y.shape[1]
     num_feature = x.shape[1]
     weights = np.zeros((num_feature, num_class), order='F')
 
-    logging.info(
-        f'Training cost-sensitive model for Macro-F1 on {num_class} labels')
-    for i in tqdm(range(num_class)):
+    if verbose:
+        logging.info(
+            f'Training cost-sensitive model for Macro-F1 on {num_class} labels')
+    for i in tqdm(range(num_class), disable=not verbose):
         yi = y[:, i].toarray().reshape(-1)
-        w = cost_sensitive_one_label(2*yi - 1, x, options)
+        w = _cost_sensitive_one_label(2*yi - 1, x, options)
         weights[:, i] = w.ravel()
 
-    return {'weights': np.asmatrix(weights), '-B': bias, 'threshold': 0}
+    return FlatModel(name='cost_sensitive',
+                     weights=np.asmatrix(weights),
+                     bias=bias,
+                     thresholds=0)
 
 
-def cost_sensitive_one_label(y: np.ndarray,
-                             x: sparse.csr_matrix,
-                             options: str
-                             ) -> np.ndarray:
+def _cost_sensitive_one_label(y: np.ndarray,
+                              x: sparse.csr_matrix,
+                              options: str
+                              ) -> np.ndarray:
     """Loop over parameter space for cost-sensitive on a single label.
 
     Args:
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
 
@@ -371,29 +446,29 @@
     perm = np.random.permutation(l)
 
     param_space = [1, 1.33, 1.8, 2.5, 3.67, 6, 13]
 
     bestScore = -np.Inf
     for a in param_space:
         cv_options = f'{options} -w1 {a}'
-        pred = cross_validate(y, x, cv_options, perm)
-        score = fmeasure(y, pred)
+        pred = _cross_validate(y, x, cv_options, perm)
+        score = _fmeasure(y, pred)
         if bestScore < score:
             bestScore = score
             bestA = a
 
     final_options = f'{options} -w1 {bestA}'
-    return do_train(y, x, final_options)
+    return _do_train(y, x, final_options)
 
 
-def cross_validate(y: np.ndarray,
-                   x: sparse.csr_matrix,
-                   options: str,
-                   perm: np.ndarray
-                   ) -> np.ndarray:
+def _cross_validate(y: np.ndarray,
+                    x: sparse.csr_matrix,
+                    options: str,
+                    perm: np.ndarray
+                    ) -> np.ndarray:
     """Cross-validation for cost-sensitive.
 
     Args:
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
 
@@ -405,89 +480,103 @@
     pred = np.zeros_like(y)
     for fold in range(nr_fold):
         mask = np.zeros_like(perm, dtype='?')
         mask[np.arange(int(fold*l/nr_fold), int((fold+1)*l/nr_fold))] = 1
         val_idx = perm[mask]
         train_idx = perm[mask != True]
 
-        w = do_train(y[train_idx], x[train_idx], options)
+        w = _do_train(y[train_idx], x[train_idx], options)
         pred[val_idx] = (x[val_idx] * w).A1 > 0
 
     return 2*pred - 1
 
 
-def train_cost_sensitive_micro(y: sparse.csr_matrix, x: sparse.csr_matrix, options: str):
+def train_cost_sensitive_micro(y: sparse.csr_matrix,
+                               x: sparse.csr_matrix,
+                               options: str = '',
+                               verbose: bool = True
+                               ) -> FlatModel:
     """Trains a linear model for multilabel data using a one-vs-rest strategy
     and cross-validation to pick an optimal asymmetric misclassification cost
     for Micro-F1.
     Outperforms train_1vsrest in most aspects at the cost of higher
     time complexity.
     See user guide for more details.
 
     Args:
         y (sparse.csr_matrix): A 0/1 matrix with dimensions number of instances * number of classes.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
-        options (str): The option string passed to liblinear.
+        options (str, optional): The option string passed to liblinear. Defaults to ''.
+        verbose (bool, optional): Output extra progress information. Defaults to True.
 
     Returns:
         A model which can be used in predict_values.
     """
     # Follows the MATLAB implementation at https://www.csie.ntu.edu.tw/~cjlin/libsvmtools/multilabel/
-    x, options, bias = prepare_options(x, options)
+    x, options, bias = _prepare_options(x, options)
 
     y = y.tocsc()
     num_class = y.shape[1]
     num_feature = x.shape[1]
     weights = np.zeros((num_feature, num_class), order='F')
 
     l = y.shape[0]
     perm = np.random.permutation(l)
     param_space = [1, 1.33, 1.8, 2.5, 3.67, 6, 13]
     bestScore = -np.Inf
 
-    logging.info(
-        f'Training cost-sensitive model for Micro-F1 on {num_class} labels')
+    if verbose:
+        logging.info(
+            f'Training cost-sensitive model for Micro-F1 on {num_class} labels')
     for a in param_space:
         tp = fn = fp = 0
-        for i in tqdm(range(num_class)):
+        for i in tqdm(range(num_class), disable=not verbose):
             yi = y[:, i].toarray().reshape(-1)
             yi = 2*yi - 1
 
             cv_options = f'{options} -w1 {a}'
-            pred = cross_validate(yi, x, cv_options, perm)
+            pred = _cross_validate(yi, x, cv_options, perm)
             tp = tp + np.sum(np.logical_and(yi == 1, pred == 1))
             fn = fn + np.sum(np.logical_and(yi == 1, pred == -1))
             fp = fp + np.sum(np.logical_and(yi == -1, pred == 1))
 
         score = 2*tp / (2*tp + fn + fp)
         if bestScore < score:
             bestScore = score
             bestA = a
 
     final_options = f'{options} -w1 {bestA}'
     for i in range(num_class):
         yi = y[:, i].toarray().reshape(-1)
-        w = do_train(2*yi - 1, x, final_options)
+        w = _do_train(2*yi - 1, x, final_options)
         weights[:, i] = w.ravel()
 
-    return {'weights': np.asmatrix(weights), '-B': bias, 'threshold': 0}
+    return FlatModel(name='cost_sensitive_micro',
+                     weights=np.asmatrix(weights),
+                     bias=bias,
+                     thresholds=0)
 
 
-def train_binary_and_multiclass(y: sparse.csr_matrix, x: sparse.csr_matrix, options: str):
+def train_binary_and_multiclass(y: sparse.csr_matrix,
+                                x: sparse.csr_matrix,
+                                options: str = '',
+                                verbose: bool = True
+                                ) -> FlatModel:
     """Trains a linear model for binary and multi-class data.
 
     Args:
         y (sparse.csr_matrix): A 0/1 matrix with dimensions number of instances * number of classes.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
-        options (str): The option string passed to liblinear.
+        options (str, optional): The option string passed to liblinear. Defaults to ''.
+        verbose (bool, optional): Output extra progress information. Defaults to True.
 
     Returns:
         A model which can be used in predict_values.
     """
-    x, options, bias = prepare_options(x, options)
+    x, options, bias = _prepare_options(x, options)
     num_instances, num_labels = y.shape
     nonzero_instance_ids, nonzero_label_ids = y.nonzero()
     assert len(set(nonzero_instance_ids)) == num_instances, """
         Invalid dataset. Only multi-class dataset is allowed."""
     y = np.squeeze(nonzero_label_ids)
 
     with silent_stderr():
@@ -504,39 +593,44 @@
         weights[:, train_labels[1]] = -w[:, 0]
     else:
         # Map label to the original index
         w = np.ctypeslib.as_array(model.w, (x.shape[1], len(train_labels)))
         weights[:, train_labels] = w
 
     # For labels not appeared in training, assign thresholds to -inf so they won't be predicted.
-    threshold = np.full(num_labels, -np.inf)
-    threshold[train_labels] = 0
-    return {'weights': np.asmatrix(weights), '-B': bias, 'threshold': threshold}
+    thresholds = np.full(num_labels, -np.inf)
+    thresholds[train_labels] = 0
+    return FlatModel(name='binary_and_multiclass',
+                     weights=np.asmatrix(weights),
+                     bias=bias,
+                     thresholds=thresholds)
 
 
 def predict_values(model, x: sparse.csr_matrix) -> np.ndarray:
     """Calculates the decision values associated with x.
 
     Args:
         model: A model returned from a training function.
         x (sparse.csr_matrix): A matrix with dimension number of instances * number of features.
 
     Returns:
         np.ndarray: A matrix with dimension number of instances * number of classes.
     """
-    bias = model['-B']
-    bias_col = np.full((x.shape[0], 1 if bias > 0 else 0), bias)
-    num_feature = model['weights'].shape[0]
-    num_feature -= 1 if bias > 0 else 0
-    if x.shape[1] < num_feature:
-        x = sparse.hstack([
-            x,
-            np.zeros((x.shape[0], num_feature - x.shape[1])),
-            bias_col,
-        ], 'csr')
-    else:
-        x = sparse.hstack([
-            x[:, :num_feature],
-            bias_col,
-        ], 'csr')
+    return model.predict_values(x)
+
+
+def get_topk_labels(label_mapping: np.ndarray,
+                    preds: np.ndarray,
+                    top_k: int = 5
+                    ) -> list[list[str]]:
+    """Get top k predictions from decision values.
 
-    return (x * model['weights']).A + model['threshold']
+    Args:
+        label_mapping (np.ndarray): A ndarray of class labels that maps each index (from 0 to ``num_class-1``) to its label.
+        preds (np.ndarray): A matrix of decision values with dimension number of instances * number of classes.
+        top_k (int): Determine how many classes per instance should be predicted.
+
+    Returns:
+        list of lists which contain top k labels.
+    """
+    top_k_ind = np.argpartition(preds, -top_k)[:, :-top_k-1:-1]
+    return label_mapping[top_k_ind].tolist()
```

### Comparing `libmultilabel-0.1.9/libmultilabel/linear/metrics.py` & `libmultilabel-0.2.0/libmultilabel/linear/metrics.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,85 @@
+from __future__ import annotations
+
 import re
 
 import numpy as np
 
-__all__ = ['RPrecision',
-           'Precision',
-           'F1',
-           'MetricCollection',
-           'get_metrics',
-           'tabulate_metrics']
+__all__ = ['get_metrics',
+           'compute_metrics',
+           'tabulate_metrics',
+           'MetricCollection']
 
 
 class RPrecision:
-    def __init__(self, top_k: int) -> None:
+    def __init__(self, top_k: int):
         self.top_k = top_k
         self.score = 0
         self.num_sample = 0
 
-    def update(self, preds: np.ndarray, target: np.ndarray) -> None:
+    def update(self, preds: np.ndarray, target: np.ndarray):
         assert preds.shape == target.shape  # (batch_size, num_classes)
         top_k_ind = np.argpartition(preds, -self.top_k)[:, -self.top_k:]
         num_relevant = np.take_along_axis(
             target, top_k_ind, axis=-1).sum(axis=-1)  # (batch_size, top_k)
         self.score += np.nan_to_num(
             num_relevant / np.minimum(self.top_k, target.sum(axis=-1)),
             posinf=0.
         ).sum()
         self.num_sample += preds.shape[0]
 
     def compute(self) -> float:
         return self.score / self.num_sample
 
+    def reset(self):
+        self.score = 0
+        self.num_sample = 0
+
 
 class Precision:
-    def __init__(self, num_classes: int, average: str, top_k: int) -> None:
+    def __init__(self, num_classes: int, average: str, top_k: int):
+        if average != 'samples':
+            raise ValueError('unsupported average')
+
         self.top_k = top_k
         self.score = 0
         self.num_sample = 0
 
-    def update(self, preds: np.ndarray, target: np.ndarray) -> None:
+    def update(self, preds: np.ndarray, target: np.ndarray):
         assert preds.shape == target.shape  # (batch_size, num_classes)
         top_k_ind = np.argpartition(preds, -self.top_k)[:, -self.top_k:]
         num_relevant = np.take_along_axis(target, top_k_ind, -1).sum()
         self.score += num_relevant / self.top_k
         self.num_sample += preds.shape[0]
 
     def compute(self) -> float:
         return self.score / self.num_sample
 
+    def reset(self):
+        self.score = 0
+        self.num_sample = 0
+
 
 class F1:
-    def __init__(self, num_classes: int, metric_threshold: float, average: str, multiclass=False) -> None:
+    def __init__(self, num_classes: int, average: str, multiclass=False):
         self.num_classes = num_classes
-        self.metric_threshold = metric_threshold
         if average not in {'macro', 'micro', 'another-macro'}:
             raise ValueError('unsupported average')
         self.average = average
         self.multiclass = multiclass
         self.tp = self.fp = self.fn = 0
 
-    def update(self, preds: np.ndarray, target: np.ndarray) -> None:
+    def update(self, preds: np.ndarray, target: np.ndarray):
         assert preds.shape == target.shape  # (batch_size, num_classes)
         if self.multiclass:
             max_idx = np.argmax(preds, axis=1).reshape(-1, 1)
             preds = np.zeros(preds.shape)
             np.put_along_axis(preds, max_idx, 1, axis=1)
         else:
-            preds = preds > self.metric_threshold
+            preds = preds > 0
         self.tp += np.logical_and(target == 1, preds == 1).sum(axis=0)
         self.fn += np.logical_and(target == 1, preds == 0).sum(axis=0)
         self.fp += np.logical_and(target == 0, preds == 1).sum(axis=0)
 
     def compute(self) -> float:
         prev_settings = np.seterr('ignore')
 
@@ -86,38 +96,66 @@
                 self.tp / (self.tp + self.fn)) / self.num_classes
             score = np.nan_to_num(
                 2 * macro_prec * macro_recall / (macro_prec + macro_recall))
 
         np.seterr(**prev_settings)
         return score
 
+    def reset(self):
+        self.tp = self.fp = self.fn = 0
+
 
 class MetricCollection(dict):
-    def __init__(self, metrics) -> None:
+    """A collection of metrics created by get_metrics.
+    MetricCollection computes metric values in two steps. First, batches of
+    decision values and labels are added with update(). After all instances have been
+    added, compute() computes the metric values from the accumulated batches.
+    """
+
+    def __init__(self, metrics):
         self.metrics = metrics
 
-    def update(self, preds: np.ndarray, target: np.ndarray) -> None:
+    def update(self, preds: np.ndarray, target: np.ndarray):
+        """Adds a batch of decision values and labels.
+
+        Args:
+            preds (np.ndarray): A matrix of decision values with dimensions number of instances * number of classes.
+            target (np.ndarray): A 0/1 matrix of labels with dimensions number of instances * number of classes.
+        """
         assert preds.shape == target.shape  # (batch_size, num_classes)
         for metric in self.metrics.values():
             metric.update(preds, target)
 
-    def compute(self) -> "dict[str, float]":
+    def compute(self) -> dict[str, float]:
+        """Computes the metrics from the accumulated batches of decision values and labels.
+
+        Returns:
+            dict[str, float]: A dictionary of metric values.
+        """
         ret = {}
         for name, metric in self.metrics.items():
             ret[name] = metric.compute()
         return ret
 
+    def reset(self):
+        """Clears the accumulated batches of decision values and labels.
+        """
+        for metric in self.metrics.values():
+            metric.reset()
+
 
-def get_metrics(metric_threshold: float, monitor_metrics: list, num_classes: int, multiclass=False):
+def get_metrics(monitor_metrics: list[str],
+                num_classes: int,
+                multiclass: bool = False
+                ) -> MetricCollection:
     """Get a collection of metrics by their names.
+    See MetricCollection for more details.
 
     Args:
-        metric_threshold (float): The decision value threshold over which a
-        label is predicted as positive.
-        monitor_metrics (list): A list of strings naming the metrics.
+        monitor_metrics (list[str]): A list of metric names.
         num_classes (int): The number of classes.
         multiclass (bool, optional): Enable multiclass mode. Defaults to False.
 
     Returns:
         MetricCollection: A metric collection of the list of metrics.
     """
     if monitor_metrics is None:
@@ -126,23 +164,58 @@
     for metric in monitor_metrics:
         if re.match('P@\d+', metric):
             metrics[metric] = Precision(
                 num_classes, average='samples', top_k=int(metric[2:]))
         elif re.match('RP@\d+', metric):
             metrics[metric] = RPrecision(top_k=int(metric[3:]))
         elif metric in {'Another-Macro-F1', 'Macro-F1', 'Micro-F1'}:
-            metrics[metric] = F1(num_classes, metric_threshold,
+            metrics[metric] = F1(num_classes,
                                  average=metric[:-3].lower(),
                                  multiclass=multiclass)
         else:
-            raise ValueError(f'Invalid metric: {metric}')
+            raise ValueError(f'invalid metric: {metric}')
 
     return MetricCollection(metrics)
 
 
-def tabulate_metrics(metric_dict, split):
+def compute_metrics(preds: np.ndarray,
+                    target: np.ndarray,
+                    monitor_metrics: list[str],
+                    multiclass: bool = False
+                    ) -> dict[str, float]:
+    """Compute metrics with decision values and labels.
+    See get_metrics and MetricCollection if decision values and labels are too
+    large to hold in memory.
+
+
+    Args:
+        preds (np.ndarray): A matrix of decision values with dimensions number of instances * number of classes.
+        target (np.ndarray): A 0/1 matrix of labels with dimensions number of instances * number of classes.
+        monitor_metrics (list[str]): A list of metric names.
+        multiclass (bool, optional): Enable multiclass mode. Defaults to False.
+
+    Returns:
+        dict[str, float]: A dictionary of metric values.
+    """
+    assert preds.shape == target.shape
+
+    metric = get_metrics(monitor_metrics, preds.shape[1], multiclass)
+    metric.update(preds, target)
+    return metric.compute()
+
+
+def tabulate_metrics(metric_dict: dict[str, float], split: str) -> str:
+    """Convert a dictionary of metric values into a pretty formatted string for printing.
+
+    Args:
+        metric_dict (dict[str, float]): A dictionary of metric values.
+        split (str): Name of the data split.
+
+    Returns:
+        str: Pretty formatted string.
+    """
     msg = f'====== {split} dataset evaluation result =======\n'
     header = '|'.join([f'{k:^18}' for k in metric_dict.keys()])
-    values = '|'.join([f'{x * 100:^18.4f}' if isinstance(x, (np.floating,
+    values = '|'.join([f'{x:^18.4f}' if isinstance(x, (np.floating,
                       float)) else f'{x:^18}' for x in metric_dict.values()])
     msg += f"|{header}|\n|{'-----------------:|' * len(metric_dict)}\n|{values}|\n"
     return msg
```

### Comparing `libmultilabel-0.1.9/libmultilabel/linear/preprocessor.py` & `libmultilabel-0.2.0/libmultilabel/linear/preprocessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import pandas as pd
 import scipy
 import scipy.sparse as sparse
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.preprocessing import MultiLabelBinarizer
 
-__all__ = ['Preprocessor']
+__all__ = ['Preprocessor', 'read_libmultilabel_format', 'read_libsvm_format']
 
 
 class Preprocessor:
     """Preprocessor is used to load and preprocess input data in LibSVM and LibMultiLabel formats.
     The same Preprocessor has to be used for both training and testing data;
     see save_pipeline and load_pipeline.
     """
@@ -29,79 +29,77 @@
             data_format (str): The data format used. 'svm' for LibSVM format, 'txt' for LibMultiLabel format in file and 'dataframe' for LibMultiLabel format in dataframe .
         """
         if not data_format in {'txt', 'svm', 'dataframe'}:
             raise ValueError(f'unsupported data format {data_format}')
 
         self.data_format = data_format
 
-    def load_data(self, training_data: Union[str, pd.DataFrame] = None,
-                  test_data: Union[str, pd.DataFrame] = None,
+    def load_data(self, training_data: str | pd.DataFrame = None,
+                  test_data: str | pd.DataFrame = None,
                   eval: bool = False,
                   label_file: str = None,
                   include_test_labels: bool = False,
-                  remove_no_label_data: bool = False) -> 'dict[str, dict]':
+                  remove_no_label_data: bool = False
+                  ) -> dict[str, dict[str, sparse.csr_matrix]]:
         """Loads and preprocesses data.
 
         Args:
-            training_data (Union[str, pd.DataFrame]): Training data file or dataframe in LibMultiLabel format. Ignored if eval is True. Defaults to None.
-            test_data (Union[str, pd.DataFrame]): Test data file or dataframe in LibMultiLabel format. Ignored if test_data doesn't exist. Defaults to None.
-            eval (bool): If True, ignores training data and uses previously loaded state to preprocess test data.
-            label_file (str, optional): Path to a file holding all labels.
+            training_data (str | pd.DataFrame, optional): Training data file or dataframe in LibMultiLabel format. Ignored if eval is True. Defaults to None.
+            test_data (str | pd.DataFrame, optional): Test data file or dataframe in LibMultiLabel format. Ignored if test_data doesn't exist. Defaults to None.
+            eval (bool, optional): If True, ignores training data and uses previously loaded state to preprocess test data. Defaults to False.
+            label_file (str, optional): Path to a file holding all labels. Defaults to None.
             include_test_labels (bool, optional): Whether to include labels in the test dataset. Defaults to False.
-            remove_no_label_data (bool, optional): Whether to remove training instances that have no labels.
+            remove_no_label_data (bool, optional): Whether to remove training instances that have no labels. Defaults to False.
 
         Returns:
-            dict[str, dict]: The training and test data, with keys 'train' and 'test' respectively. The data
-            has keys 'x' for input features and 'y' for labels.
+            dict[str, dict[str, sparse.csr_matrix]]: The training and test data, with keys 'train' and 'test' respectively.
+            The data has keys 'x' for input features and 'y' for labels.
         """
         if label_file is not None:
             logging.info(f'Load labels from {label_file}.')
             with open(label_file, 'r') as fp:
                 self.classes = sorted([s.strip() for s in fp.readlines()])
         else:
             if test_data is None and include_test_labels:
                 raise ValueError(
                     f'Specified the inclusion of test labels but test file does not exist')
             self.classes = None
             self.include_test_labels = include_test_labels
 
-        if self.data_format == 'txt' or 'dataframe':
-            data = self._load_libmultilabel(training_data, test_data, eval)
+        if self.data_format in {'txt', 'dataframe'}:
+            data = self._load_text(training_data, test_data, eval)
         elif self.data_format == 'svm':
             data = self._load_svm(training_data, test_data, eval)
 
         if 'train' in data:
             num_labels = data['train']['y'].getnnz(axis=1)
             num_no_label_data = np.count_nonzero(num_labels == 0)
             if num_no_label_data > 0:
                 if remove_no_label_data:
                     logging.info(
-                        f'Remove {num_no_label_data} instances that have no labels from {training_data}.',
+                        f'Remove {num_no_label_data} instances that have no labels from data.',
                         extra={'collect': True})
                     data['train']['x'] = data['train']['x'][num_labels > 0]
                     data['train']['y'] = data['train']['y'][num_labels > 0]
                 else:
                     logging.info(
-                        f'Keep {num_no_label_data} instances that have no labels from {training_data}.',
+                        f'Keep {num_no_label_data} instances that have no labels from data.',
                         extra={'collect': True})
 
         return data
 
-    def _load_libmultilabel(self, training_data, test_data, eval) -> 'dict[str, dict]':
+    def _load_text(self, training_data: str | pd.Dataframe,
+                   test_data: str | pd.Dataframe,
+                   eval: bool
+                   ) -> dict[str, dict[str, sparse.csr_matrix]]:
         datasets = defaultdict(dict)
         if test_data is not None:
-            if self.data_format == 'txt':
-                test_data = pd.read_csv(test_data, sep='\t', header=None,
-                                        error_bad_lines=False, warn_bad_lines=True, quoting=csv.QUOTE_NONE).fillna('')
             test = read_libmultilabel_format(test_data)
 
         if not eval:
-            if self.data_format == 'txt':
-                training_data = pd.read_csv(training_data, sep='\t', header=None,
-                                            error_bad_lines=False, warn_bad_lines=True, quoting=csv.QUOTE_NONE).fillna('')
             train = read_libmultilabel_format(training_data)
             self._generate_tfidf(train['text'])
 
             if self.classes or not self.include_test_labels:
                 self._generate_label_mapping(train['label'], self.classes)
             else:
                 self._generate_label_mapping(train['label'] + test['label'])
@@ -112,15 +110,18 @@
         if test_data is not None:
             datasets['test']['x'] = self.vectorizer.transform(test['text'])
             datasets['test']['y'] = self.binarizer.transform(
                 test['label']).astype('d')
 
         return dict(datasets)
 
-    def _load_svm(self, training_data, test_data, eval) -> 'dict[str, dict]':
+    def _load_svm(self, training_data: str,
+                  test_data: str,
+                  eval: bool
+                  ) -> dict[str, dict[str, sparse.csr_matrix]]:
         datasets = defaultdict(dict)
         if test_data is not None:
             ty, tx = read_libsvm_format(test_data)
 
         if not eval:
             y, x = read_libsvm_format(training_data)
             if self.classes or not self.include_test_labels:
@@ -131,37 +132,51 @@
             datasets['train']['y'] = self.binarizer.transform(y).astype('d')
 
         if test_data is not None:
             datasets['test']['x'] = tx
             datasets['test']['y'] = self.binarizer.transform(ty).astype('d')
         return dict(datasets)
 
-    def _generate_tfidf(self, texts):
+    def _generate_tfidf(self, texts: list[str]):
         self.vectorizer = TfidfVectorizer()
         self.vectorizer.fit(texts)
 
-    def _generate_label_mapping(self, labels, classes=None):
+    def _generate_label_mapping(self, labels: list[list[str]], classes: list[str] = None):
         self.binarizer = MultiLabelBinarizer(
             sparse_output=True, classes=classes)
         self.binarizer.fit(labels)
+        self.label_mapping = self.binarizer.classes_
 
 
-def read_libmultilabel_format(data: pd.DataFrame) -> 'dict[str,list[str]]':
+def read_libmultilabel_format(data: str | pd.Dataframe) -> dict[str,list[str]]:
+    """Read multi-label text data from file or pandas dataframe.
+
+    Args:
+        data ('str | pd.Dataframe'): A file path to data in `LibMultiLabel format <https://www.csie.ntu.edu.tw/~cjlin/libmultilabel/cli/ov_data_format.html#libmultilabel-format>`_
+            or a pandas dataframe contains index (optional), label, and text.
+    Returns:
+        dict[str,list[str]]: A dictionary with a list of index (optional), label, and text.
+    """
+    assert isinstance(data, str) or isinstance(data, pd.DataFrame), "Data must be from a file or pandas dataframe."
+    if isinstance(data, str):
+        data = pd.read_csv(data, sep='\t', header=None,
+                           on_bad_lines='warn', quoting=csv.QUOTE_NONE).fillna('')
     data = data.astype(str)
     if data.shape[1] == 2:
         data.columns = ['label', 'text']
         data = data.reset_index()
     elif data.shape[1] == 3:
         data.columns = ['index', 'label', 'text']
     else:
         raise ValueError(f'Expected 2 or 3 columns, got {data.shape[1]}.')
     data['label'] = data['label'].map(lambda s: s.split())
     return data.to_dict('list')
 
-def read_libsvm_format(file_path: str) -> 'tuple[list[list[int]], sparse.csr_matrix]':
+
+def read_libsvm_format(file_path: str) -> tuple[list[list[int]], sparse.csr_matrix]:
     """Read multi-label LIBSVM-format data.
 
     Args:
         file_path (str): Path to file.
 
     Returns:
         tuple[list[list[int]], sparse.csr_matrix]: A tuple of labels and features.
```

### Comparing `libmultilabel-0.1.9/libmultilabel/linear/utils.py` & `libmultilabel-0.2.0/libmultilabel/linear/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,108 @@
+from __future__ import annotations
+
 import os
+import pathlib
 import pickle
 import re
-from pathlib import Path
+from typing import Any
 
+import numpy as np
 import scipy.sparse as sparse
 import sklearn.base
 import sklearn.model_selection
 import sklearn.pipeline
 import sklearn.utils
 
 import libmultilabel.linear as linear
 
 from .preprocessor import Preprocessor
 
-__all__ = ['save_pipeline', 'load_pipeline', 'MultiLabelEstimator', 'GridSearchCV']
+__all__ = ['save_pipeline', 'load_pipeline',
+           'MultiLabelEstimator', 'GridSearchCV']
 
 
 LINEAR_TECHNIQUES = {
     '1vsrest': linear.train_1vsrest,
     'thresholding': linear.train_thresholding,
     'cost_sensitive': linear.train_cost_sensitive,
     'cost_sensitive_micro': linear.train_cost_sensitive_micro,
-    'binary_and_multiclass': linear.train_binary_and_multiclass
+    'binary_and_multiclass': linear.train_binary_and_multiclass,
+    'tree': linear.train_tree,
 }
 
 
 def save_pipeline(checkpoint_dir: str, preprocessor: Preprocessor, model):
     """Saves preprocessor and model to checkpoint_dir/linear_pipline.pickle.
 
     Args:
         checkpoint_dir (str): The directory to save to.
         preprocessor (Preprocessor): A Preprocessor.
         model: A model returned from one of the training functions.
     """
-    Path(checkpoint_dir).mkdir(parents=True, exist_ok=True)
+    pathlib.Path(checkpoint_dir).mkdir(parents=True, exist_ok=True)
     checkpoint_path = os.path.join(checkpoint_dir, 'linear_pipeline.pickle')
 
     with open(checkpoint_path, 'wb') as f:
         pickle.dump({
             'preprocessor': preprocessor,
             'model': model,
         }, f)
 
 
-def load_pipeline(checkpoint_path: str) -> tuple:
+def load_pipeline(checkpoint_path: str) -> tuple[Preprocessor, Any]:
     """Loads preprocessor and model from checkpoint_path.
 
     Args:
         checkpoint_path (str): The path to a previously saved pipeline.
 
     Returns:
-        tuple: A tuple of the preprocessor and model.
+        tuple[Preprocessor, Any]: A tuple of the preprocessor and model.
     """
     with open(checkpoint_path, 'rb') as f:
         pipeline = pickle.load(f)
     return (pipeline['preprocessor'], pipeline['model'])
 
 
 class MultiLabelEstimator(sklearn.base.BaseEstimator):
     """Customized sklearn estimator for the multi-label classifier.
 
     Args:
-        options (str, optional): The option string passed to liblinear. Defaults to '-s 2'.
+        options (str, optional): The option string passed to liblinear. Defaults to ''.
         linear_technique (str, optional): Multi-label technique defined in `utils.LINEAR_TECHNIQUES`.
             Defaults to '1vsrest'.
-        metric_threshold (int, optional): The decision value threshold over which a label
-            is predicted as positive. Defaults to 0.
         scoring_metric (str, optional): The scoring metric. Defaults to 'P@1'.
     """
 
-    def __init__(self, options='-s 2', linear_technique='1vsrest', metric_threshold=0, scoring_metric='P@1'):
+    def __init__(self, options: str = '',
+                 linear_technique: str = '1vsrest',
+                 scoring_metric: str = 'P@1'
+                 ):
         super().__init__()
         self.options = options
         self.linear_technique = linear_technique
-        self.metric_threshold = metric_threshold
         self.scoring_metric = scoring_metric
         self._is_fitted = False
 
     def fit(self, X: sparse.csr_matrix, y: sparse.csr_matrix):
         X, y = sklearn.utils.validation.check_X_y(
             X, y, accept_sparse=True, multi_output=True)
         self._is_fitted = True
         self.model = LINEAR_TECHNIQUES[self.linear_technique](
             y, X, self.options)
         return self
 
-    def predict(self, X: sparse.csr_matrix):
+    def predict(self, X: sparse.csr_matrix) -> np.ndarray:
         sklearn.utils.validation.check_is_fitted(
             self, attributes=['_is_fitted'])
         preds = linear.predict_values(self.model, X)
         return preds
 
-    def score(self, X: sparse.csr_matrix, y: sparse.csr_matrix):
+    def score(self, X: sparse.csr_matrix, y: sparse.csr_matrix) -> float:
         metrics = linear.get_metrics(
-            self.metric_threshold,
             [self.scoring_metric],
             y.shape[1],
         )
         preds = self.predict(X)
         metrics.update(preds, y.toarray())
         metric_dict = metrics.compute()
         return metric_dict[self.scoring_metric]
```

### Comparing `libmultilabel-0.1.9/libmultilabel/logging.py` & `libmultilabel-0.2.0/libmultilabel/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import transformers.utils.logging as transformer_logging
 
 LOG_FORMAT = '%(asctime)s %(levelname)s:%(message)s'
 
 
 class ListHandler(logging.Handler):
     """Collect logged messages to a list of strings that can be obtained later.
     The `logging` module does not provide this function, so we implement one.
@@ -44,16 +43,20 @@
     global stream_handler
 
     if stream_handler:
         return stream_handler
     else:
         logging.getLogger().setLevel(logging.NOTSET) # use handlers to control levels
 
-        transformer_logging.disable_default_handler()
-        transformer_logging.enable_propagation()
+        try:
+            import transformers.utils.logging as transformer_logging
+            transformer_logging.disable_default_handler()
+            transformer_logging.enable_propagation()
+        except ImportError:
+            pass
 
         lightning_logger = logging.getLogger('pytorch_lightning')
         lightning_logger.handlers.clear()
         lightning_logger.propagate = True
 
         stream_handler = logging.StreamHandler()
         stream_handler.setLevel(level)
```

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/data_utils.py` & `libmultilabel-0.2.0/libmultilabel/nn/data_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,43 +7,67 @@
 import torch
 import transformers
 from nltk.tokenize import RegexpTokenizer
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import MultiLabelBinarizer
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import Dataset
-from torchtext.vocab import build_vocab_from_iterator, pretrained_aliases
+from torchtext.vocab import build_vocab_from_iterator, pretrained_aliases, Vocab
 from tqdm import tqdm
 
 transformers.logging.set_verbosity_error()
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
 UNK = '<unk>'
 PAD = '<pad>'
 
 
 class TextDataset(Dataset):
-    """Class for text dataset"""
+    """Class for text dataset.
 
-    def __init__(self, data, word_dict, classes, max_seq_length, tokenizer=None, add_special_tokens=True):
+    Args:
+        data (list[dict]): List of instances with index, label, and text.
+        classes (list): List of labels.
+        max_seq_length (int, optional): The maximum number of tokens of a sample.
+        add_special_tokens (bool, optional): Whether to add the special tokens. Defaults to True.
+        tokenizer (transformers.PreTrainedTokenizerBase, optional): HuggingFace's tokenizer of
+            the transformer-based pretrained language model. Defaults to None.
+        word_dict (torchtext.vocab.Vocab, optional): A vocab object for word tokenizer to
+            map tokens to indices. Defaults to None.
+    """
+    def __init__(
+        self,
+        data,
+        classes,
+        max_seq_length,
+        add_special_tokens=True,
+        *,
+        tokenizer=None,
+        word_dict=None,
+    ):
         self.data = data
-        self.word_dict = word_dict
         self.classes = classes
         self.max_seq_length = max_seq_length
-        self.num_classes = len(self.classes)
-        self.label_binarizer = MultiLabelBinarizer().fit([classes])
+        self.word_dict = word_dict
         self.tokenizer = tokenizer
         self.add_special_tokens = add_special_tokens
 
+        self.num_classes = len(self.classes)
+        self.label_binarizer = MultiLabelBinarizer().fit([classes])
+
+        if not isinstance(self.word_dict, Vocab) ^ isinstance(
+            self.tokenizer, transformers.PreTrainedTokenizerBase):
+            raise ValueError(
+                'Please specify exactly one of word_dict or tokenizer')
+
     def __len__(self):
         return len(self.data)
 
     def __getitem__(self, index):
         data = self.data[index]
-
         if self.tokenizer is not None:  # transformers tokenizer
             if self.add_special_tokens:  # tentatively hard code
                 input_ids = self.tokenizer.encode(data['text'],
                                                   padding='max_length',
                                                   max_length=self.max_seq_length,
                                                   truncation=True)
             else:
@@ -79,43 +103,52 @@
         'label': torch.stack(label_list),
         'length': torch.IntTensor(length_list)
     }
 
 
 def get_dataset_loader(
     data,
-    word_dict,
     classes,
     device,
     max_seq_length=500,
     batch_size=1,
     shuffle=False,
     data_workers=4,
+    add_special_tokens=True,
+    *,
     tokenizer=None,
-    add_special_tokens=True
+    word_dict=None,
 ):
     """Create a pytorch DataLoader.
 
     Args:
-        data (list): List of training instances with index, label, and tokenized text.
-        word_dict (torchtext.vocab.Vocab): A vocab object which maps tokens to indices.
+        data (list[dict]): List of training instances with index, label, and tokenized text.
         classes (list): List of labels.
         device (torch.device): One of cuda or cpu.
         max_seq_length (int, optional): The maximum number of tokens of a sample. Defaults to 500.
         batch_size (int, optional): Size of training batches. Defaults to 1.
         shuffle (bool, optional): Whether to shuffle training data before each epoch. Defaults to False.
         data_workers (int, optional): Use multi-cpu core for data pre-processing. Defaults to 4.
-        tokenizer (optional): Tokenizer of the transformer-based language model. Defaults to None.
         add_special_tokens (bool, optional): Whether to add the special tokens. Defaults to True.
+        tokenizer (transformers.PreTrainedTokenizerBase, optional): HuggingFace's tokenizer of
+            the transformer-based pretrained language model. Defaults to None.
+        word_dict (torchtext.vocab.Vocab, optional): A vocab object for word tokenizer to
+            map tokens to indices. Defaults to None.
 
     Returns:
         torch.utils.data.DataLoader: A pytorch DataLoader.
     """
-    dataset = TextDataset(data, word_dict, classes, max_seq_length, tokenizer=tokenizer,
-                          add_special_tokens=add_special_tokens)
+    dataset = TextDataset(
+        data,
+        classes,
+        max_seq_length,
+        word_dict=word_dict,
+        tokenizer=tokenizer,
+        add_special_tokens=add_special_tokens
+    )
     dataset_loader = torch.utils.data.DataLoader(
         dataset,
         batch_size=batch_size,
         shuffle=shuffle,
         num_workers=data_workers,
         collate_fn=generate_batch,
         pin_memory='cuda' in device.type,
@@ -131,14 +164,19 @@
         is_test (bool, optional): Whether the data is for test or not. Defaults to False.
         remove_no_label_data (bool, optional): Whether to remove training/validation instances that have no labels.
             This is effective only when is_test=False. Defaults to False.
 
     Returns:
         pandas.DataFrame: Data composed of index, label, and tokenized text.
     """
+    assert isinstance(data, str) or isinstance(data, pd.DataFrame), "Data must be from a file or pandas dataframe."
+    if isinstance(data, str):
+        logging.info(f'Load data from {data}.')
+        data = pd.read_csv(data, sep='\t', header=None,
+                           on_bad_lines='warn', quoting=csv.QUOTE_NONE).fillna('')
     data = data.astype(str)
     if data.shape[1] == 2:
         data.columns = ['label', 'text']
         data = data.reset_index()
     elif data.shape[1] == 3:
         data.columns = ['index', 'label', 'text']
     else:
@@ -149,20 +187,20 @@
         data['text'] = data['text'].map(tokenize)
     data = data.to_dict('records')
     if not is_test:
         num_no_label_data = sum(1 for d in data if len(d['label']) == 0)
         if num_no_label_data > 0:
             if remove_no_label_data:
                 logging.info(
-                    f'Remove {num_no_label_data} instances that have no labels from {path}.',
+                    f'Remove {num_no_label_data} instances that have no labels from data.',
                     extra={'collect': True})
                 data = [d for d in data if len(d['label']) > 0]
             else:
                 logging.info(
-                    f'Keep {num_no_label_data} instances that have no labels from {path}.',
+                    f'Keep {num_no_label_data} instances that have no labels from data.',
                     extra={'collect': True})
     return data
 
 
 def load_datasets(
     training_data=None,
     test_data=None,
@@ -193,39 +231,27 @@
     if isinstance(training_data, str) or isinstance(test_data, str):
         assert training_data or test_data, "At least one of `training_data` and `test_data` must be specified."
     elif isinstance(training_data, pd.DataFrame) or isinstance(test_data, pd.DataFrame):
         assert not training_data.empty or not test_data.empty, "At least one of `training_data` and `test_data` must be specified."
 
     datasets = {}
     if training_data is not None:
-        if isinstance(training_data, str):
-            logging.info(f'Load data from {training_data}.')
-            training_data = pd.read_csv(training_data, sep='\t', header=None,
-                                        error_bad_lines=False, warn_bad_lines=True, quoting=csv.QUOTE_NONE).fillna('')
-        datasets['train'] = _load_raw_data(training_data, tokenize_text=tokenize_text,
-                                           remove_no_label_data=remove_no_label_data)
+        datasets['train'] = _load_raw_data(
+            training_data, tokenize_text=tokenize_text, remove_no_label_data=remove_no_label_data)
 
     if val_data is not None:
-        if isinstance(val_data, str):
-            logging.info(f'Load data from {val_data}.')
-            val_data = pd.read_csv(val_data, sep='\t', header=None,
-                                   error_bad_lines=False, warn_bad_lines=True, quoting=csv.QUOTE_NONE).fillna('')
-        datasets['val'] = _load_raw_data(val_data, tokenize_text=tokenize_text,
-                                           remove_no_label_data=remove_no_label_data)   
+        datasets['val'] = _load_raw_data(
+            val_data, tokenize_text=tokenize_text, remove_no_label_data=remove_no_label_data)
     elif val_size > 0:
         datasets['train'], datasets['val'] = train_test_split(
             datasets['train'], test_size=val_size, random_state=42)
 
     if test_data is not None:
-        if isinstance(test_data, str):
-            logging.info(f'Load data from {test_data}.')
-            test_data = pd.read_csv(test_data, sep='\t', header=None,
-                                    error_bad_lines=False, warn_bad_lines=True, quoting=csv.QUOTE_NONE).fillna('')
-        datasets['test'] = _load_raw_data(test_data, is_test=True, tokenize_text=tokenize_text,
-                                          remove_no_label_data=remove_no_label_data)
+        datasets['test'] = _load_raw_data(
+            test_data, is_test=True, tokenize_text=tokenize_text, remove_no_label_data=remove_no_label_data)
 
     if merge_train_val:
         datasets['train'] = datasets['train'] + datasets['val']
         for i in range(len(datasets['train'])):
             datasets['train'][i]['index'] = i
         del datasets['val']
         gc.collect()
```

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/metrics.py` & `libmultilabel-0.2.0/libmultilabel/nn/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 
 import numpy as np
 import torch
 import torchmetrics.classification
 from torchmetrics import Metric, MetricCollection, Precision, Recall
 from torchmetrics.functional.retrieval.ndcg import retrieval_normalized_dcg
@@ -118,15 +120,15 @@
 
 
 class MacroF1(Metric):
     """The macro-f1 score computes the average f1 scores of all labels in the dataset.
 
     Args:
         num_classes (int): Total number of classes.
-        metric_threshold (float): Threshold to monitor for metrics.
+        metric_threshold (float): The decision value threshold over which a label is predicted as positive.
         another_macro_f1 (bool, optional): Whether to compute the 'Another-Macro-F1' score.
             The 'Another-Macro-F1' is the f1 value of macro-precision and macro-recall.
             This variant of macro-f1 is less preferred but is used in some works.
             Please refer to Opitz et al. 2019 [https://arxiv.org/pdf/1911.03347.pdf].
             Defaults to False.
     """
     # If the metric state of one batch is independent of the state of other batches,
@@ -179,15 +181,15 @@
 
 
 def get_metrics(metric_threshold, monitor_metrics, num_classes, top_k=None):
     """Map monitor metrics to the corresponding classes defined in `torchmetrics.Metric`
     (https://torchmetrics.readthedocs.io/en/latest/references/modules.html).
 
     Args:
-        metric_threshold (float): Threshold to monitor for metrics.
+        metric_threshold (float): The decision value threshold over which a label is predicted as positive.
         monitor_metrics (list): Metrics to monitor while validating.
         num_classes (int): Total number of classes.
 
     Raises:
         ValueError: The metric is invalid if:
             (1) It is not one of 'P@k', 'R@k', 'RP@k', 'nDCG@k', 'Micro-Precision',
                 'Micro-Recall', 'Micro-F1', 'Macro-F1', 'Another-Macro-F1', or a
@@ -249,14 +251,23 @@
                 f'Invalid metric: {metric}. Make sure the metric is in the right format: Macro/Micro-Precision/Recall/F1 (ex. Micro-F1)')
 
     # If compute_groups is set to True (default), incorrect results may be calculated.
     # Please refer to https://github.com/Lightning-AI/metrics/issues/746 for more details.
     return MetricCollection(metrics, compute_groups=False)
 
 
-def tabulate_metrics(metric_dict, split):
+def tabulate_metrics(metric_dict: dict[str, float], split: str) -> str:
+    """Convert a dictionary of metric values into a pretty formatted string for printing.
+
+    Args:
+        metric_dict (dict[str, float]): A dictionary of metric values.
+        split (str): Name of the data split.
+
+    Returns:
+        str: Pretty formatted string.
+    """
     msg = f'====== {split} dataset evaluation result =======\n'
     header = '|'.join([f'{k:^18}' for k in metric_dict.keys()])
-    values = '|'.join([f'{x * 100:^18.4f}' if isinstance(x, (np.floating,
+    values = '|'.join([f'{x:^18.4f}' if isinstance(x, (np.floating,
                       float)) else f'{x:^18}' for x in metric_dict.values()])
     msg += f"|{header}|\n|{'-----------------:|' * len(metric_dict)}\n|{values}|\n"
     return msg
```

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/model.py` & `libmultilabel-0.2.0/libmultilabel/nn/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     Args:
         num_classes (int): Total number of classes.
         learning_rate (float, optional): Learning rate for optimizer. Defaults to 0.0001.
         optimizer (str, optional): Optimizer name (i.e., sgd, adam, or adamw). Defaults to 'adam'.
         momentum (float, optional): Momentum factor for SGD only. Defaults to 0.9.
         weight_decay (int, optional): Weight decay factor. Defaults to 0.
-        metric_threshold (float, optional): Threshold to monitor for metrics. Defaults to 0.5.
+        metric_threshold (float, optional): The decision value threshold over which a label is predicted as positive. Defaults to 0.5.
         monitor_metrics (list, optional): Metrics to monitor while validating. Defaults to None.
         log_path (str): Path to a directory holding the log files and models.
         multiclass (bool, optional): Enable multiclass mode. Defaults to False.
         silent (bool, optional): Enable silent mode. Defaults to False.
         save_k_predictions (int, optional): Save top k predictions on test set. Defaults to 0.
     """
```

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/networks/__init__.py` & `libmultilabel-0.2.0/libmultilabel/nn/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/networks/bert.py` & `libmultilabel-0.2.0/libmultilabel/nn/networks/bert.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/networks/bert_attention.py` & `libmultilabel-0.2.0/libmultilabel/nn/networks/bert_attention.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/networks/caml.py` & `libmultilabel-0.2.0/libmultilabel/nn/networks/caml.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/networks/kim_cnn.py` & `libmultilabel-0.2.0/libmultilabel/nn/networks/kim_cnn.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/networks/labelwise_attention_networks.py` & `libmultilabel-0.2.0/libmultilabel/nn/networks/labelwise_attention_networks.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/networks/modules.py` & `libmultilabel-0.2.0/libmultilabel/nn/networks/modules.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/networks/xml_cnn.py` & `libmultilabel-0.2.0/libmultilabel/nn/networks/xml_cnn.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.1.9/libmultilabel/nn/nn_utils.py` & `libmultilabel-0.2.0/libmultilabel/nn/nn_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     logging.info(f'Using device: {device}')
     return device
 
 
 def init_model(model_name,
                network_config,
                classes,
-               word_dict,
-               embed_vecs,
+               word_dict=None,
+               embed_vecs=None,
                init_weight=None,
                log_path=None,
                learning_rate=0.0001,
                optimizer='adam',
                momentum=0.9,
                weight_decay=0,
                metric_threshold=0.5,
@@ -53,41 +53,46 @@
                save_k_predictions=0):
     """Initialize a `Model` class for initializing and training a neural network.
 
     Args:
         model_name (str): Model to be used such as KimCNN.
         network_config (dict): Configuration for defining the network.
         classes (list): List of class names.
-        word_dict (torchtext.vocab.Vocab): A vocab object which maps tokens to indices.
-        embed_vecs (torch.Tensor): The pre-trained word vectors of shape (vocab_size, embed_dim).
+        word_dict (torchtext.vocab.Vocab, optional): A vocab object for word tokenizer to
+            map tokens to indices. Defaults to None.
+        embed_vecs (torch.Tensor, optional): The pre-trained word vectors of shape
+            (vocab_size, embed_dim). Defaults to None.
         init_weight (str): Weight initialization method from `torch.nn.init`.
             For example, the `init_weight` of `torch.nn.init.kaiming_uniform_`
             is `kaiming_uniform`. Defaults to None.
         log_path (str): Path to a directory holding the log files and models.
         learning_rate (float, optional): Learning rate for optimizer. Defaults to 0.0001.
         optimizer (str, optional): Optimizer name (i.e., sgd, adam, or adamw). Defaults to 'adam'.
         momentum (float, optional): Momentum factor for SGD only. Defaults to 0.9.
         weight_decay (int, optional): Weight decay factor. Defaults to 0.
-        metric_threshold (float, optional): Threshold to monitor for metrics. Defaults to 0.5.
+        metric_threshold (float, optional): The decision value threshold over which a label is predicted as positive. Defaults to 0.5.
         monitor_metrics (list, optional): Metrics to monitor while validating. Defaults to None.
         multiclass (bool, optional): Enable multiclass mode. Defaults to False.
         silent (bool, optional): Enable silent mode. Defaults to False.
         loss_function (str, optional): Loss function name (i.e., binary_cross_entropy_with_logits,
             cross_entropy). Defaults to 'binary_cross_entropy_with_logits'.
         save_k_predictions (int, optional): Save top k predictions on test set. Defaults to 0.
 
     Returns:
         Model: A class that implements `MultiLabelModel` for initializing and training a neural network.
     """
 
-    network = getattr(networks, model_name)(
-        embed_vecs=embed_vecs,
-        num_classes=len(classes),
-        **dict(network_config)
-    )
+    try:
+        network = getattr(networks, model_name)(
+            embed_vecs=embed_vecs,
+            num_classes=len(classes),
+            **dict(network_config)
+        )
+    except:
+        raise AttributeError(f'Failed to initialize {model_name}.')
 
     if init_weight is not None:
         init_weight = networks.get_init_weight_func(
             init_weight=init_weight)
         network.apply(init_weight)
 
     model = Model(
@@ -160,15 +165,16 @@
                                       mode='min' if val_metric == 'Loss' else 'max')]
     if search_params:
         from ray.tune.integration.pytorch_lightning import TuneReportCallback
         callbacks += [TuneReportCallback(
             {f'val_{val_metric}': val_metric}, on="validation_end")]
 
     trainer = pl.Trainer(logger=False, num_sanity_val_steps=0,
-                         gpus=0 if use_cpu else 1,
+                         accelerator='cpu' if use_cpu else 'gpu',
+                         devices=None if use_cpu else 1,
                          enable_progress_bar=False if silent else True,
                          max_epochs=epochs,
                          callbacks=callbacks,
                          limit_train_batches=limit_train_batches,
                          limit_val_batches=limit_val_batches,
                          limit_test_batches=limit_test_batches,
                          deterministic='warn')
```

### Comparing `libmultilabel-0.1.9/libmultilabel.egg-info/PKG-INFO` & `libmultilabel-0.2.0/libmultilabel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.1.9
+Version: 0.2.0
 Summary: A library for multi-label text classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
```

### Comparing `libmultilabel-0.1.9/libmultilabel.egg-info/SOURCES.txt` & `libmultilabel-0.2.0/libmultilabel.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 libmultilabel.egg-info/dependency_links.txt
 libmultilabel.egg-info/requires.txt
 libmultilabel.egg-info/top_level.txt
 libmultilabel/linear/__init__.py
 libmultilabel/linear/linear.py
 libmultilabel/linear/metrics.py
 libmultilabel/linear/preprocessor.py
+libmultilabel/linear/tree.py
 libmultilabel/linear/utils.py
 libmultilabel/nn/__init__.py
 libmultilabel/nn/data_utils.py
 libmultilabel/nn/metrics.py
 libmultilabel/nn/model.py
 libmultilabel/nn/nn_utils.py
 libmultilabel/nn/networks/__init__.py
```

### Comparing `libmultilabel-0.1.9/setup.cfg` & `libmultilabel-0.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libmultilabel
-version = 0.1.9
+version = 0.2.0
 author = LibMultiLabel Team
 license = MIT License
 license_file = LICENSE
 description = A library for multi-label text classification
 long_description = See documentation here: https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 url = https://github.com/ASUS-AICS/LibMultiLabel
 project_urls = 
@@ -22,15 +22,15 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 
 [options]
 packages = find:
 install_requires = 
 	nltk
-	pandas
+	pandas>1.3.0
 	PyYAML
 	scikit-learn
 	torch>=1.13.1
 	torchmetrics==0.10.3
 	torchtext>=0.13.0
 	pytorch-lightning==1.7.7
 	tqdm
```

