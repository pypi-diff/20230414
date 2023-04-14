# Comparing `tmp/gurobi-machinelearning-1.1.0b0.tar.gz` & `tmp/gurobi-machinelearning-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gurobi-machinelearning-1.1.0b0.tar", last modified: Thu Jan 12 12:02:49 2023, max compression
+gzip compressed data, was "gurobi-machinelearning-1.1.1.tar", last modified: Fri Apr 14 07:36:15 2023, max compression
```

## Comparing `gurobi-machinelearning-1.1.0b0.tar` & `gurobi-machinelearning-1.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:02:49.351832 gurobi-machinelearning-1.1.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-01-12 12:02:49.351832 gurobi-machinelearning-1.1.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-12 12:02:49.351832 gurobi-machinelearning-1.1.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:02:49.343832 gurobi-machinelearning-1.1.0b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:02:49.347832 gurobi-machinelearning-1.1.0b0/src/gurobi_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-01-12 12:02:49.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-01-12 12:02:49.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 12:02:49.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-12 12:02:49.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-12 12:02:49.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_machinelearning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:02:49.347832 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-01-12 12:02:40.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/add_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:02:49.347832 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/keras/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:02:49.347832 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/_var_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/base_predictor_constr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/get_convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:02:49.347832 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/neuralnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/neuralnet/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/neuralnet/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/neuralnet/neural_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/submodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/register_user_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/registered_predictors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:02:49.351832 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/base_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/mlpregressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/pls_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/predictors_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/skgetter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 12:02:49.351832 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-01-12 12:02:38.000000 gurobi-machinelearning-1.1.0b0/src/gurobi_ml/torch/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.753751 gurobi-machinelearning-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.753751 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-14 07:36:15.000000 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-14 07:36:15.000000 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:36:15.000000 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 07:36:15.000000 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 07:36:15.000000 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-14 07:36:07.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/add_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/keras/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/_var_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/base_predictor_constr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/get_convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/neural_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/submodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/register_user_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/registered_predictors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/base_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/mlpregressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/pls_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/predictors_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/skgetter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/torch/sequential.py
```

### Comparing `gurobi-machinelearning-1.1.0b0/LICENSE` & `gurobi-machinelearning-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.0b0/PKG-INFO` & `gurobi-machinelearning-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.1.0b0
+Version: 1.1.1
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
@@ -42,15 +42,15 @@
 
 For questions related to using Gurobi Machine Learning please use [Gurobi's Forum](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects).
 
 For reporting bugs, issues and feature request please
 [open an issue](https://github.com/Gurobi/gurobi-machinelearning/issues).
 
 If you encounter issues with Gurobi or ``gurobipy`` please contact
-[Gurobi Support](https://support.gurobi.com/hc/en-us)
+[Gurobi Support](https://support.gurobi.com/hc/en-us).
 
 # Installation
 
 ## Dependencies
 
 `gurobi-machinelearning` requires the following:
 - Python >= 3.9
@@ -59,15 +59,15 @@
 - [`scipy`](https://pypi.org/project/scipy/) >= 1.9.3
 
 The current version supports the following ML packages:
 - [`torch`](https://pypi.org/project/torch/)
 - [`scikit-learn`](https://pypi.org/project/scikit-learn)
 - [`tensorflow`](https://pypi.org/project/tensorflow)
 
-Installing these package is only required if the predictor you want to insert uses them
+Installing these packages is only required if the predictor you want to insert uses them
 (i.e. to insert a Keras based predictor you need to have `tensorflow` installed).
 
 The up to date supported and tested versions of each package for the last release can be [found in the documentation](https://gurobi-machinelearning.readthedocs.io/en/1.1.x/firststeps-introduction.html#table-versions).
 
 ## Pip installation
 
 The easiest way to install `gurobi-machinelearning` is using `pip` in a virtual environment:
```

### Comparing `gurobi-machinelearning-1.1.0b0/README.md` & `gurobi-machinelearning-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 For questions related to using Gurobi Machine Learning please use [Gurobi's Forum](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects).
 
 For reporting bugs, issues and feature request please
 [open an issue](https://github.com/Gurobi/gurobi-machinelearning/issues).
 
 If you encounter issues with Gurobi or ``gurobipy`` please contact
-[Gurobi Support](https://support.gurobi.com/hc/en-us)
+[Gurobi Support](https://support.gurobi.com/hc/en-us).
 
 # Installation
 
 ## Dependencies
 
 `gurobi-machinelearning` requires the following:
 - Python >= 3.9
@@ -40,15 +40,15 @@
 - [`scipy`](https://pypi.org/project/scipy/) >= 1.9.3
 
 The current version supports the following ML packages:
 - [`torch`](https://pypi.org/project/torch/)
 - [`scikit-learn`](https://pypi.org/project/scikit-learn)
 - [`tensorflow`](https://pypi.org/project/tensorflow)
 
-Installing these package is only required if the predictor you want to insert uses them
+Installing these packages is only required if the predictor you want to insert uses them
 (i.e. to insert a Keras based predictor you need to have `tensorflow` installed).
 
 The up to date supported and tested versions of each package for the last release can be [found in the documentation](https://gurobi-machinelearning.readthedocs.io/en/1.1.x/firststeps-introduction.html#table-versions).
 
 ## Pip installation
 
 The easiest way to install `gurobi-machinelearning` is using `pip` in a virtual environment:
```

### Comparing `gurobi-machinelearning-1.1.0b0/pyproject.toml` & `gurobi-machinelearning-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gurobi-machinelearning"
-version = "1.1.0b0"
+version = "1.1.1"
 description = "package to insert ML models in Gurobi"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="Apache-2.0"}
 keywords = ["mathematical optimization", "gurobi", "scikit-learn", "pytorch", "tensorflow", "ml"]
 authors = [
   {name = "Gurobi Optimization LLC"}
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_machinelearning.egg-info/PKG-INFO` & `gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.1.0b0
+Version: 1.1.1
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
@@ -42,15 +42,15 @@
 
 For questions related to using Gurobi Machine Learning please use [Gurobi's Forum](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects).
 
 For reporting bugs, issues and feature request please
 [open an issue](https://github.com/Gurobi/gurobi-machinelearning/issues).
 
 If you encounter issues with Gurobi or ``gurobipy`` please contact
-[Gurobi Support](https://support.gurobi.com/hc/en-us)
+[Gurobi Support](https://support.gurobi.com/hc/en-us).
 
 # Installation
 
 ## Dependencies
 
 `gurobi-machinelearning` requires the following:
 - Python >= 3.9
@@ -59,15 +59,15 @@
 - [`scipy`](https://pypi.org/project/scipy/) >= 1.9.3
 
 The current version supports the following ML packages:
 - [`torch`](https://pypi.org/project/torch/)
 - [`scikit-learn`](https://pypi.org/project/scikit-learn)
 - [`tensorflow`](https://pypi.org/project/tensorflow)
 
-Installing these package is only required if the predictor you want to insert uses them
+Installing these packages is only required if the predictor you want to insert uses them
 (i.e. to insert a Keras based predictor you need to have `tensorflow` installed).
 
 The up to date supported and tested versions of each package for the last release can be [found in the documentation](https://gurobi-machinelearning.readthedocs.io/en/1.1.x/firststeps-introduction.html#table-versions).
 
 ## Pip installation
 
 The easiest way to install `gurobi-machinelearning` is using `pip` in a virtual environment:
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_machinelearning.egg-info/SOURCES.txt` & `gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/__init__.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/_version.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/_version.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" To get version and git hash of built package """
+"""To get version and git hash of built package."""
 from importlib import metadata
 
 try:
     __version__ = metadata.version("gurobi_machinelearning")
 except metadata.PackageNotFoundError:
     __version__ = "dev"
 
-GIT_HASH = "95bc6f9cf3a08bb996650b402be7548614e5adc3"
+GIT_HASH = "c845d69838e1554a657b0653400c0e710ca774ad"
 
 
 def get_versions():
-    """Get package version"""
+    """Get package version."""
     # Downloaded package with inserted git hash.
     if "Format" not in GIT_HASH:
         git_hash = f"-{GIT_HASH}"
     # No inserted git hash, the repo is probably cloned.
     else:
         git_hash = ""
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/add_predictor.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/add_predictor.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,34 +9,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Define generic function that can add any known trained predictor
-"""
+"""Define generic function that can add any known trained predictor."""
 
 from .exceptions import NotRegistered
 from .modeling.get_convertor import get_convertor
 from .registered_predictors import registered_predictors
 
 
 def add_predictor_constr(gp_model, predictor, input_vars, output_vars=None, **kwargs):
-    """Use `predictor` to predict the value of `output_vars` using `input_vars` in `gp_model`
+    """Formulate predictor in gp_model.
+
+    The formulation predicts the values of output_vars using input_vars according to
+    predictor.
 
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
             The gurobipy model where the predictor should be inserted.
     predictor:
         The predictor to insert.
-    input_vars: mvar_array_like
+    input_vars : mvar_array_like
         Decision variables used as input for predictor in gp_model.
-    output_vars: mvar_array_like, optional
+    output_vars : mvar_array_like, optional
         Decision variables used as output for predictor in gp_model.
 
     Returns
     -------
     AbstractPredictorConstr
         Object containing information about what was added to gp_model to insert the
         predictor in it
@@ -49,28 +51,31 @@
      * Pandas data frames containing columns of variables or constants
      * Lists of variables
      * Dictionaries of variables
 
     For internal use in the package they are cast into matrix variables.
 
     They should have dimensions that conforms with the input/output of the predictor.
-    We denote by `n_features` the dimension of the input of the predictor and by `n_output` the dimension of the output.
-
-    If they are matrix variables, `input_vars` and `output_vars` can be either of shape `(n_features)` and
-    `(n_outputs,)` respectively or `(k, n_features)` and `(k, n_outputs)` respectively (with `k >= 1`).
-    The latter form is especially useful if the predictor is used to associate different groups of
-    variables (e.g. a prediction is made for every time period in a planning horizon).
-
-    If they are pandas dataframe, `input_vars` should have the features as columns and `output_vars` the
-    outputs of predictors. Note that the input_vars dataframe may have *fixed* columns containing constant values
-    and *variable* columns containing gurobipy variables. A column should not mix constants and variables.
-
-    If they are lists or dictionaries, `input_vars` should have length `n_features` and `output_vars`
-    should have length `n_output`.
-    List and dictionaries can have bad performances in particular if the same predictor is used with different input/output many times.
+    We denote by `n_features` the dimension of the input of the predictor and by
+    `n_output` the dimension of the output.
 
+    If they are matrix variables, `input_vars` and `output_vars` can be either of
+    shape `(n_features)` and `(n_outputs,)` respectively or `(k, n_features)` and
+    `(k, n_outputs)` respectively (with `k >= 1`). The latter form is especially
+    useful if the predictor is used to associate different groups of variables
+    (e.g. a prediction is made for every time period in a planning horizon).
+
+    If they are pandas dataframe, `input_vars` should have the features as columns and
+    `output_vars` the outputs of predictors. Note that the input_vars dataframe may
+    have *fixed* columns containing constant values and *variable* columns containing
+    gurobipy variables. A column should not mix constants and variables.
+
+    If they are lists or dictionaries, `input_vars` should have length `n_features` and
+    `output_vars` should have length `n_output`.
+    List and dictionaries can have bad performances in particular if particular adding
+    many predictor constraints in a for loop is significantly slower.
     """
     convertors = registered_predictors()
     convertor = get_convertor(predictor, convertors)
     if convertor is None:
         raise NotRegistered(type(predictor).__name__)
     return convertor(gp_model, predictor, input_vars, output_vars, **kwargs)
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/exceptions.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,40 +9,40 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Exceptions for gurobi_ml """
+"""Exceptions for gurobi_ml."""
 
 
 class NotRegistered(Exception):
-    """Predictor is not supported by gurobi_ml"""
+    """Predictor is not supported by gurobi_ml."""
 
     def __init__(self, predictor):
         super().__init__(
             f"Object of type {predictor} is not registered/supported with gurobi_ml"
         )
 
 
 class NoModel(Exception):
-    """No model is known for some structure"""
+    """No model is known for some structure."""
 
     def __init__(self, predictor, reason):
         if not isinstance(predictor, str):
             predictor = type(predictor).__name__
         super().__init__(f"Can't do model for {predictor}: {reason}")
 
 
 class NoSolution(Exception):
-    """Gurobi doesn't have a solution"""
+    """Gurobi doesn't have a solution."""
 
     def __init__(self):
         super().__init__("No solution available")
 
 
 class ParameterError(Exception):
-    """Wrong parameter to a function"""
+    """Wrong parameter to a function."""
 
     def __init__(self, message):
         super().__init__(message)
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/keras/__init__.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/keras/keras.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/keras/keras.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,73 +9,70 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for formulating a Keras model into a :gurobipy:`model`
-"""
+"""Module for formulating a Keras model into a :gurobipy:`model`."""
 
 import numpy as np
 from tensorflow import keras
 
 from ..exceptions import NoModel, NoSolution
 from ..modeling.neuralnet import BaseNNConstr
 
 
 def add_keras_constr(gp_model, keras_model, input_vars, output_vars=None, **kwargs):
-    """Formulate keras_model into gp_model
+    """Formulate keras_model into gp_model.
 
     The formulation predicts the values of output_vars using input_vars according to keras_model.
     See our :ref:`Users Guide <Neural Networks>` for details on the mip formulation used.
 
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the predictor should be inserted.
-    keras_model: `keras.Model <https://keras.io/api/models/model/>`
+    keras_model : `keras.Model <https://keras.io/api/models/model/>`
         The keras model to insert as predictor.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for Keras model in gp_model.
-    output_vars: :gurobipy:`mvar` or :gurobipy:`var` array like, optional
+    output_vars : :gurobipy:`mvar` or :gurobipy:`var` array like, optional
         Decision variables used as output for Keras model in gp_model.
 
     Returns
     -------
     KerasNetworkConstr
         Object containing information about what was added to gp_model to formulate
         keras_model into it
 
+    Raises
+    ------
+    NoModel
+        If the translation for some of the Keras model structure
+        (layer or activation) is not implemented.
 
     Warning
     -------
 
       Only `Dense <https://keras.io/api/layers/core_layers/dense/>`_ (possibly
       with `relu` activation), and `ReLU <https://keras.io/api/layers/activation_layers/relu/>`_ with
       default settings are supported.
 
-    Raises
-    ------
-    NoModel
-        If the translation for some of the Keras model structure
-        (layer or activation) is not implemented.
-
     Note
     ----
     |VariablesDimensionsWarn|
     """
     return KerasNetworkConstr(gp_model, keras_model, input_vars, output_vars, **kwargs)
 
 
 class KerasNetworkConstr(BaseNNConstr):
-    """Class to model trained `keras.Model <https://keras.io/api/models/model/>` with gurobipy
+    """Class to model trained `keras.Model <https://keras.io/api/models/model/>` with gurobipy.
 
     |ClassShort|
-
     """
 
     def __init__(self, gp_model, predictor, input_vars, output_vars=None, **kwargs):
         assert predictor.built
         for step in predictor.layers:
             if isinstance(step, keras.layers.Dense):
                 config = step.get_config()
@@ -111,30 +108,31 @@
         for i, step in enumerate(network.layers):
             if i == num_layers - 1:
                 output = self._output
             if isinstance(step, keras.layers.InputLayer):
                 pass
             elif isinstance(step, keras.layers.ReLU):
                 layer = self.add_activation_layer(
-                    _input, self.act_dict["relu"], output, name="relu"
+                    _input, self.act_dict["relu"], output, name=f"relu{i}", **kwargs
                 )
                 _input = layer.output
             else:
                 config = step.get_config()
                 activation = config["activation"]
                 if activation == "linear":
                     activation = "identity"
                 weights, bias = step.get_weights()
                 layer = self.add_dense_layer(
                     _input,
                     weights,
                     bias,
                     self.act_dict[activation],
                     output,
-                    name="dense",
+                    name=f"dense{i}",
+                    **kwargs,
                 )
                 _input = layer.output
         if self._output is None:
             self._output = layer.output
 
     def get_error(self):
         if self._has_solution:
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/__init__.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/_var_utils.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/_var_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Utility functions for dealing with input and output variables of predictor constr objects"""
+"""Utility functions for dealing with input and output variables of predictor constr objects."""
 
 import gurobipy as gp
 import numpy as np
 
 from ..exceptions import ParameterError
 
 try:
@@ -36,71 +36,79 @@
     predictor:
         Class of the predictor
     """
     return type(predictor).__name__.lower()
 
 
 def _get_sol_values(values, columns=None, index=None):
-    """Get solution values
+    """Get solution values.
 
     This is complicated because of the column_transformer.
     In most cases we can just do values.X but if we have a column transformer with
-    some constants that can't be translated to Gurobi variables we need to fill in missing values"""
+    some constants that can't be translated to Gurobi variables we need to fill in missing values
+    """
     if HAS_PANDAS:
         if isinstance(values, pd.DataFrame):
-            return pd.DataFrame(
+            rval = pd.DataFrame(
                 data=_get_sol_values(values.to_numpy()),
                 index=values.index,
                 columns=values.columns,
             )
+            for col in rval.columns:
+                try:
+                    rval[col] = rval[col].astype(np.float64)
+                except ValueError:
+                    pass
+            return rval.convert_dtypes()
     if isinstance(values, np.ndarray):
         return np.array(
             [v.X if isinstance(v, gp.Var) else v for v in values.ravel()]
         ).reshape(values.shape)
     X = values.X
     if columns is not None and HAS_PANDAS:
         if isinstance(index, (pd.Index, pd.MultiIndex)):
             X = pd.DataFrame(data=X, columns=columns, index=index)
         else:
-            raise NotImplementedError("Input variables as pd.Series is not implemented")
             X = pd.Series(data=X, columns=columns, name=index)
+            raise NotImplementedError("Input variables as pd.Series is not implemented")
     return X
 
 
 def _dataframe_to_mvar(model, df):
-    """Convert a DataFrame to an mvar
+    """Convert a DataFrame to an mvar.
 
-    This just calls the array_to_mvar function"""
+    This just calls the array_to_mvar function
+    """
     if isinstance(df, pd.DataFrame):
         data = df.to_numpy()
         columns = df.columns
         index = df.index
     elif isinstance(df, pd.Series):
         raise NotImplementedError("Input variables as pd.Series is not implemented")
     return _array_to_mvar(model, data, columns, index)
 
 
 def _array_to_mvar(model, data, columns=None, index=None):
-    """Function to create an MVar from an ndarray
+    """Function to create an MVar from an ndarray.
 
     The array data may contain columns of Gurobi variables and constant values.
     In this function we create an array of same shape as data where constant
     values are replace by fixed variables. This is then converted to an MVar.
 
     If columns and index are passed, used them to give appropriate names to
     created variables.
 
     Parameters
     ----------
-    model: gp.Model
+    model : gp.Model
         The gurobipy model
-    data: ndarray
+    data : ndarray
         A numpy array whose columns are either columns of gp.Var or data that
         can be converted to a float
-    columns: optional
+    columns : optional
         Name of data columns
     index:
         Name of data rows
     """
 
     # If data only contains gp.Var's we can directly convert it to an MVar
     if all(map(lambda i: isinstance(i, gp.Var), data.ravel())):
@@ -147,15 +155,15 @@
         rval[:, j] = mvar[:, i].tolist()
     model.update()
     rval = gp.MVar.fromlist(rval)
     return rval
 
 
 def validate_output_vars(gp_vars):
-    """Put variables into appropriate form (matrix of variable) for the output of a predictor constraint
+    """Put variables into appropriate form (matrix of variable) for the output of a predictor constraint.
 
     Parameters
     ----------
     gpvars:
         Decision variables used.
 
     Returns
@@ -181,15 +189,15 @@
         return gp.MVar.fromlist(gp_vars)
     if isinstance(gp_vars, gp.Var):
         return gp.MVar.fromlist([gp_vars]).reshape(1, 1)
     raise ParameterError("Could not validate variables")
 
 
 def validate_input_vars(model, gp_vars):
-    """Put variables into appropriate form (matrix of variable) for the input of a predictor constraint
+    """Put variables into appropriate form (matrix of variable) for the input of a predictor constraint.
 
     Parameters
     ----------
     gpvars:
         Decision variables used.
 
     Returns
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/base_predictor_constr.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/base_predictor_constr.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,27 @@
 
 from ..exceptions import ParameterError
 from ._var_utils import _get_sol_values, validate_input_vars, validate_output_vars
 from .submodel import SubModel
 
 
 class AbstractPredictorConstr(ABC, SubModel):
-    """Base class to store sub-model added by :py:func:`gurobi_ml.add_predictor_constr`
+    """Base class to store sub-model added by :py:func:`gurobi_ml.add_predictor_constr`.
 
     This class is the base class to store everything that is added to
     a Gurobi model when a trained predictor is inserted into it. Depending on
     the type of the predictor, a class derived from it will be returned
     by :py:func:`gurobi_ml.add_predictor_constr`.
 
     Warning
     -------
 
     Users should usually never construct objects of this class or one of its derived
-    classes. They are returned by the :py:func:`gurobi_ml.add_predictor_constr` and other
-    functions.
-
+    classes. They are returned by the :py:func:`gurobi_ml.add_predictor_constr` and
+    other functions.
     """
 
     def __init__(self, gp_model, input_vars, output_vars=None, **kwargs):
         self._input = input_vars
         self._output = output_vars
         SubModel.__init__(self, gp_model, **kwargs)
 
@@ -79,156 +78,163 @@
                 + f"{output_vars.shape[0]} != {input_vars.shape[0]}"
             )
 
         self._input = input_vars
         self._output = output_vars
 
     def _build_submodel(self, gp_model, *args, **kwargs):
-        """Predict output from input using predictor or transformer"""
+        """Predict output from input using predictor or transformer."""
         self._input, columns, index = validate_input_vars(self._gp_model, self._input)
         self._input_index = index
         self._input_columns = columns
 
         if self._output is None:
-            self._create_output_vars(self._input)
+            self._output = self._create_output_vars(self._input)
         if self._output is not None:
             self._output = validate_output_vars(self._output)
             self._validate()
         self._mip_model(**kwargs)
         assert self._output is not None
         return self
 
+    def _print_container_steps(self, iterations_name, iterable, file):
+        header = f"{iterations_name:13} {'Output Shape':>14} {'Variables':>12} {'Constraints':^38}"
+        print("-" * len(header), file=file)
+        print(header, file=file)
+        print(f"{' '*41} {'Linear':>12} {'Quadratic':>12} {'General':>12}", file=file)
+        print("=" * len(header), file=file)
+        for step in iterable:
+            step.print_stats(abbrev=True, file=file)
+            print(file=file)
+        print("-" * len(header), file=file)
+
     def print_stats(self, abbrev=False, file=None):
-        """Print statistics on model additions stored by this class
+        """Print statistics on model additions stored by this class.
 
         This function prints detailed statistics on the variables
         and constraints that where added to the model.
 
         Usually derived classes reimplement this function to provide more
         details about the structure of the additions (type of ML model,
         layers if it's a neural network,...)
 
         Arguments
         ---------
 
         file: None, optional
             Text stream to which output should be redirected. By default sys.stdout.
-
         """
 
         if abbrev:
             print(
                 f"{self._name:13} {self.output.shape.__str__():>14} {len(self.vars):>12} "
                 + f"{len(self.constrs):>12} {len(self.qconstrs):>12} {len(self.genconstrs):>12}",
                 file=file,
             )
         else:
             super().print_stats(file)
             print(f"Input has shape {self.input.shape}", file=file)
             print(f"Output has shape {self.output.shape}", file=file)
 
     def _create_output_vars(self, input_vars, name="out"):
-        """May be defined in derived class to create the output variables of predictor"""
+        """May be defined in derived class to create the output variables of predictor."""
         try:
             n_outputs = self._output_shape
         except AttributeError:
             return
-        self._output = self._gp_model.addMVar(
+        output = self._gp_model.addMVar(
             (input_vars.shape[0], n_outputs), lb=-gp.GRB.INFINITY, name=name
         )
         self._gp_model.update()
+        return output
 
     @property
     def _has_solution(self):
-        """Returns true if we have a solution"""
+        """Returns true if we have a solution."""
         try:
             self.input_values
             return True
         except gp.GurobiError:
             pass
         return False
 
     @abstractmethod
     def get_error(self):
-        """Returns error in Gurobi's solution with respect to prediction from input
+        """Returns error in Gurobi's solution with respect to prediction from input.
 
         Returns
         -------
-        error: ndarray of same shape as :py:attr:`gurobi_ml.modeling.base_predictor_constr.AbstractPredictorConstr.output`
+        error : ndarray of same shape as :py:attr:`gurobi_ml.modeling.base_predictor_constr.AbstractPredictorConstr.output`
             Assuming that we have a solution for the input and output variables
             `x, y`. Returns the absolute value of the differences between `predictor.predict(x)` and
             `y`. Where predictor is the regression model represented by this object.
+
         Raises
         ------
         NoSolution
             If the Gurobi model has no solution (either was not optimized or is infeasible).
-
         """
         ...
 
     @abstractmethod
     def _mip_model(self, **kwargs):
-        """Makes MIP model for the predictor the sub-class implements"""
+        """Makes MIP model for the predictor the sub-class implements."""
         ...
 
     @staticmethod
     def _indexed_name(index, name):
         index = f"{index}".replace(" ", "")
         return f"{name}[{index}]"
 
     @property
     def output(self):
-        """Output variables of embedded predictor
+        """Output variables of embedded predictor.
 
         Returns
         -------
-        output: :gurobipy:`MVar`.
-
+        output : :gurobipy:`MVar`.
         """
         return self._output
 
     @property
     def input_values(self):
-        """Returns the values for the input variables if a solution is known
+        """Returns the values for the input variables if a solution is known.
 
         Returns
         -------
-        output_value: ndarray or pandas dataframe with values
+        output_value : ndarray or pandas dataframe with values
 
         Raises
         ------
         NoSolution
             If the Gurobi model has no solution (either was not optimized or is infeasible).
-
         """
 
         return _get_sol_values(self.input, self._input_columns, self._input_index)
 
     @property
     def output_values(self):
-        """Returns the values for the output variables if a solution is known
+        """Returns the values for the output variables if a solution is known.
 
         Returns
         -------
-        output_value: ndarray or pandas dataframe with values
+        output_value : ndarray or pandas dataframe with values
 
         Raises
         ------
         NoSolution
             If the Gurobi model has no solution (either was not optimized or is infeasible).
-
         """
         return _get_sol_values(self.output)
 
     @property
     def input(self):
-        """Returns the input variables of embedded predictor
+        """Returns the input variables of embedded predictor.
 
         Returns
         -------
-        output: :gurobipy:`MVar`.
-
+        output : :gurobipy:`MVar`.
         """
         return self._input
 
     def __str__(self):
         return self._name
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/get_convertor.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/get_convertor.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Utility function to find function that add a predictor in dictionnary """
+"""Utility function to find function that add a predictor in dictionnary."""
 
 
 def get_convertor(predictor, convertors):
-    """Return the convertor for a given predictor"""
+    """Return the convertor for a given predictor."""
     convertor = None
     try:
         convertor = convertors[type(predictor)]
     except KeyError:
         pass
     if convertor is None:
         for parent in type(predictor).mro():
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/neuralnet/__init__.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/neuralnet/activations.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/activations.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,76 +9,76 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-"""Internal module to make MIP modeling of activation functions"""
+"""Internal module to make MIP modeling of activation functions."""
 
 import numpy as np
 from gurobipy import GRB
 
 
 class Identity:
-    """Class to apply identity activation on a neural network layer
+    """Class to apply identity activation on a neural network layer.
 
     Parameters
     ----------
-    setbounds: Bool
+    setbounds : Bool
         Optional flag not to set bounds on the output variables.
 
     Attributes
     ----------
-    setbounds: Bool
+    setbounds : Bool
         Optional flag not to set bounds on the output variables.
     """
 
     def __init__(self):
         pass
 
     def mip_model(self, layer):
-        """MIP model for identity activation on a layer
+        """MIP model for identity activation on a layer.
 
         Parameters
         ----------
-        layer: AbstractNNLayer
+        layer : AbstractNNLayer
             Layer to which activation is applied.
         """
         output = layer.output
         layer.gp_model.addConstr(output == layer.input @ layer.coefs + layer.intercept)
 
 
 class ReLU:
-    """Class to apply the ReLU activation on a neural network layer
+    """Class to apply the ReLU activation on a neural network layer.
 
     Parameters
     ----------
-    setbounds: Bool
+    setbounds : Bool
         Optional flag not to set bounds on the output variables.
-    bigm: Float
+    bigm : Float
         Optional maximal value for bounds use in the formulation
 
     Attributes
     ----------
-    setbounds: Bool
+    setbounds : Bool
         Optional flag not to set bounds on the output variables.
-    bigm: Float
+    bigm : Float
         Optional maximal value for bounds use in the formulation
     """
 
     def __init__(self):
         pass
 
     def mip_model(self, layer):
-        """MIP model for ReLU activation on a layer
+        """MIP model for ReLU activation on a layer.
 
         Parameters
         ----------
-        layer: AbstractNNLayer
+        layer : AbstractNNLayer
             Layer to which activation is applied.
         """
         output = layer.output
         if hasattr(layer, "coefs"):
             if not hasattr(layer, "mixing"):
                 mixing = layer.gp_model.addMVar(
                     output.shape, lb=-GRB.INFINITY, vtype=GRB.CONTINUOUS, name="_mix"
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/neuralnet/layers.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/neural_net.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,135 +9,119 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-"""Bases classes for modeling neural network layers"""
+"""Bases classes for modeling neural network layers."""
 
-import gurobipy as gp
 
 from .._var_utils import _default_name
 from ..base_predictor_constr import AbstractPredictorConstr
+from .activations import Identity, ReLU
+from .layers import ActivationLayer, DenseLayer
 
 
-class AbstractNNLayer(AbstractPredictorConstr):
-    """Abstract class for NN layers"""
-
-    def __init__(
-        self,
-        gp_model,
-        output_vars,
-        input_vars,
-        activation_function,
-        **kwargs,
-    ):
-        self.activation = activation_function
-        AbstractPredictorConstr.__init__(
-            self, gp_model, input_vars, output_vars, **kwargs
-        )
-
-    def get_error(self):
-        assert False
-
-    def print_stats(self, file=None):
-        """Print statistics about submodel created
-
-        Parameters
-        ---------
-
-        file: None, optional
-          Text stream to which output should be redirected. By default sys.stdout.
-        """
-        print(
-            f"{self._name:12} {_default_name(self.activation):12} "
-            + f"{self.output.shape.__str__():>12} {len(self.vars):>10} "
-            + f"{len(self.constrs):>10} {len(self.qconstrs):>10} {len(self.genconstrs):>10}",
-            file=file,
-        )
+class BaseNNConstr(AbstractPredictorConstr):
+    """Base class for inserting a regressor based on neural-network/tensor into Gurobi."""
 
+    def __init__(self, gp_model, predictor, input_vars, output_vars, **kwargs):
+        self.predictor = predictor
+        self.act_dict = {
+            "relu": ReLU(),
+            "identity": Identity(),
+        }
+        try:
+            for activation, activation_model in kwargs["activation_models"].items():
+                self.act_dict[activation] = activation_model
+        except KeyError:
+            pass
+        self._layers = []
 
-class ActivationLayer(AbstractNNLayer):
-    """Class to build one activation layer of a neural network"""
-
-    def __init__(
-        self,
-        gp_model,
-        output_vars,
-        input_vars,
-        activation_function,
-        **kwargs,
-    ):
-        self.zvar = None
-        self._default_name = "activation"
+        self._default_name = _default_name(predictor)
         super().__init__(
-            gp_model,
-            output_vars,
-            input_vars,
-            activation_function,
+            gp_model=gp_model,
+            input_vars=input_vars,
+            output_vars=output_vars,
             **kwargs,
         )
 
-    def _create_output_vars(self, input_vars):
-        rval = self._gp_model.addMVar(input_vars.shape, lb=-gp.GRB.INFINITY, name="act")
-        self._gp_model.update()
-        self._output = rval
-
-    def _mip_model(self, **kwargs):
-        """Add the layer to model"""
-        model = self.gp_model
-        model.update()
-        if "activation" in kwargs:
-            activation = kwargs["activation"]
-        else:
-            activation = self.activation
+    def __iter__(self):
+        return self._layers.__iter__()
 
-        # Do the mip model for the activation in the layer
-        activation.mip_model(self)
-        self._gp_model.update()
-
-
-class DenseLayer(AbstractNNLayer):
-    """Class to build one layer of a neural network"""
-
-    def __init__(
+    def add_dense_layer(
         self,
-        gp_model,
-        output_vars,
         input_vars,
         layer_coefs,
         layer_intercept,
-        activation_function,
+        activation,
+        activation_vars=None,
         **kwargs,
     ):
-        self.coefs = layer_coefs
-        self.intercept = layer_intercept
-        self.zvar = None
-        self._default_name = "dense"
-        super().__init__(
-            gp_model,
-            output_vars,
+        """Add a dense layer to gurobipy model.
+
+        Parameters
+        ----------
+
+        input_vars : mvar_array_like
+            Decision variables used as input for predictor in model.
+        layer_coefs:
+            Coefficient for each node in a layer
+        layer_intercept:
+            Intercept bias
+        activation:
+            Activation function
+        activation_vars : None, optional
+            Output variables
+        """
+        layer = DenseLayer(
+            self._gp_model,
+            activation_vars,
             input_vars,
-            activation_function,
+            layer_coefs,
+            layer_intercept,
+            activation,
             **kwargs,
         )
+        self._layers.append(layer)
+        return layer
+
+    def add_activation_layer(
+        self, input_vars, activation, activation_vars=None, **kwargs
+    ):
+        """Add an activation layer to gurobipy model.
 
-    def _create_output_vars(self, input_vars):
-        rval = self._gp_model.addMVar(
-            (input_vars.shape[0], self.coefs.shape[1]), lb=-gp.GRB.INFINITY, name="act"
+        Parameters
+        ----------
+
+        input_vars : mvar_array_like
+            Decision variables used as input for predictor in gurobipy model.
+        activation:
+            Activation function
+        activation_vars : mvar_array_like, optional
+            Output variables
+        """
+        layer = ActivationLayer(
+            self._gp_model, activation_vars, input_vars, activation, **kwargs
         )
-        self._gp_model.update()
-        self._output = rval
+        self._layers.append(layer)
+        return layer
 
-    def _mip_model(self, **kwargs):
-        """Add the layer to model"""
-        model = self.gp_model
-        model.update()
-        if "activation" in kwargs:
-            activation = kwargs["activation"]
-        else:
-            activation = self.activation
+    def print_stats(self, abbrev=False, file=None):
+        """Print statistics about submodel created.
 
-        # Do the mip model for the activation in the layer
-        activation.mip_model(self)
-        self._gp_model.update()
+        Parameters
+        ----------
+
+        file : None, optional
+            Text stream to which output should be redirected. By default sys.stdout.
+        """
+        if not abbrev:
+            super().print_stats(abbrev, file)
+            print(file=file)
+
+            self._print_container_steps("Layer", self._layers, file=file)
+        else:
+            for layer in self:
+                layer.print_stats(abbrev=True, file=file)
+                print(file=file)
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/modeling/submodel.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/submodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-"""Building Sub-models with gurobipy"""
+"""Building Sub-models with gurobipy."""
+
+from time import time
 
 
 class SubModel:
     """Base class for building and representing a MIP formulation embedded in a gurobipy.Model.
 
     When instantiating this class, a (sub-)model is created in the provided
     gurobipy.Model.  The instance represents the sub-model that was created,
@@ -85,15 +87,14 @@
     gurobipy.Model.  In particular, you can instantiate SubModels from
     within the model construction method or function of a SubModel itself.
     In this case, the automatic name handling will '.'-separated generate
     names following your call hierarchy.
 
     Parameters
     ----------
-
     """
 
     def __init__(
         self,
         gp_model,
         *args,
         model_function=None,
@@ -113,14 +114,20 @@
         self._last_callback = None
         self._name = None
         self._model_function = model_function
 
         if not hasattr(self, "_default_name"):
             self._default_name = type(self).__name__
 
+        if "verbose" in kwargs:
+            self.verbose = kwargs["verbose"]
+            self._start_time = time()
+        else:
+            self.verbose = False
+
         before = self._open(gp_model)
         self._objects = self._build_submodel(gp_model, *args, **kwargs)
         if self._objects is None:
             self._objects = {}
         self._close(before, name)
 
     def _build_submodel(self, gp_model, *args, **kwargs):
@@ -128,48 +135,48 @@
 
         When using SubModel to wrap a modeling function in a SubModel, the default
         implementation of this method simply calls the modeling function.
         """
         return self._model_function(gp_model, *args, **kwargs)
 
     class _ModelingData:
-        """Class for recording modeling data in a gurobipy.Model object"""
+        """Class for recording modeling data in a gurobipy.Model object."""
 
         def __init__(self):
             self.name_handler = None
 
         def pop_name_handler(self):
             """Remove name handler and return it."""
             name_handler = self.name_handler
             self.name_handler = None
             return name_handler
 
         def push_name_handler(self, name_handler):
-            """install name handler"""
+            """Install name handler."""
             self.name_handler = name_handler
 
     class _modelstats:
-        """Helper class for recording gurobi model dimensions
+        """Helper class for recording gurobi model dimensions.
 
         Parameters
         ----------
-        gp_model: gp.Model <https://www.gurobi.com/documentation/9.5/refman/py_model.html>
+        gp_model : gp.Model <https://www.gurobi.com/documentation/9.5/refman/py_model.html>
             A gurobipy model
 
         Attributes
         ----------
-        numvars: int
+        numvars : int
             Number of variables in `gp_model`.
-        numconstrs: int
+        numconstrs : int
             Number of constraints in `gp_model`.
-        numsos: int
+        numsos : int
             Number of SOS constraints in `gp_model`
-        numqconstrs: int
+        numqconstrs : int
             Number of quadratic constraints in `gp_model`
-        numgenconstrs: int
+        numgenconstrs : int
             Number of general constraints in `gp_model`
         """
 
         def __init__(self, gp_model):
             gp_model.update()
             self.numvars = gp_model.numVars
             self.numconstrs = gp_model.numConstrs
@@ -244,15 +251,15 @@
 
     @property
     def sos(self):
         """Return the list of SOS constraints in the submodel."""
         return self._sos
 
     def _open(self, gp_model):
-        """Start registering modeling object that are added to the gurobipy.Model"""
+        """Start registering modeling object that are added to the gurobipy.Model."""
         self._gp_model = gp_model
         try:
             modeling_data = gp_model._modeling_data
         except AttributeError:
             modeling_data = SubModel._ModelingData()
         gp_model._modeling_data = modeling_data
 
@@ -261,15 +268,15 @@
     def _close(self, before, name):
         """Finalize addition of modeling objects to the gurobipy.Model object.
 
         Record all added modeling objects in SubModel and prefix their names.
         """
 
         class NameHandler:
-            """Handle automatic name generation in gp.Model"""
+            """Handle automatic name generation in gp.Model."""
 
             def __init__(self):
                 self.name = {}
 
             def get_name(self, sub: SubModel):
                 """Return a default name for specified submodel sub."""
                 name = sub.default_name
@@ -277,15 +284,15 @@
                     num = self.name[name]
                 except KeyError:
                     num = 1
                 self.name[name] = num + 1
                 return f"{name}{num}"
 
         def prefix_names(gp_model, objs, attr, name):
-            """Prefix all modeling object names with name"""
+            """Prefix all modeling object names with name."""
             if len(objs) == 0:
                 return
             object_names = gp_model.getAttr(attr, objs)
             new_names = [f"{name}.{obj_name}" for obj_name in object_names]
             gp_model.setAttr(attr, objs, new_names)
 
         # re-install name handler
@@ -299,35 +306,38 @@
             if name is None:
                 name_handler = self._gp_model._modeling_data.name_handler
                 if name_handler is None:
                     name_handler = NameHandler()
                     self._gp_model._modeling_data.push_name_handler(name_handler)
                 name = name_handler.get_name(self)
             self._name = name
+            if self.verbose:
+                gen_time = time() - self._start_time
+                print(f"Added {name} took {gen_time:.2f} seconds.")
             prefix_names(self._gp_model, self.vars, "VarName", name)
             prefix_names(self._gp_model, self.constrs, "ConstrName", name)
             prefix_names(self._gp_model, self.qconstrs, "QCName", name)
             prefix_names(self._gp_model, self.genconstrs, "GenConstrName", name)
             # SOS can't have a name! :-O
             # prefix_names(self._gp_model, self.sos, "SOSName", name)
 
     def print_stats(self, abbrev=False, file=None):
-        """Print statistics about submodel
+        """Print statistics about submodel.
 
         This functions prints detailed statistics on the variables
         and constraints that where added to the gp_model using this object.
 
         Usually derived class reimplement this function to provide more
         details about the structure of the additions (type of ML model,
         layers if it's a neural network,...)
 
         Parameters
-        ---------
+        ----------
 
-        file: None, optional
+        file : None, optional
             Text stream to which output should be redirected. By default sys.stdout.
         """
         if abbrev:
             return
         name = self._name
         print(f"Model for {name}:", file=file)
         print(f"{len(self.vars)} variables", file=file)
@@ -340,26 +350,27 @@
             print(f"{genconstr} general constraints", file=file)
         sosconstr = len(self.sos)
         if sosconstr > 0:
             print(f"{sosconstr} SOS constraints", file=file)
 
     @property
     def gp_model(self):
-        """Access gurobipy model the submodel is a part of"""
+        """Access gurobipy model the submodel is a part of."""
         return self._gp_model
 
     @property
     def default_name(self):
         """Access the default name base used for automatic name generation.
 
-        :meta private:"""
+        :meta private:
+        """
         return self._default_name
 
     def remove(self):
-        """Remove the submodel from the model"""
+        """Remove the submodel from the model."""
         if self._gp_model:
             self._gp_model.remove(self.vars)
             self._gp_model.remove(self.constrs)
             self._gp_model.remove(self.qconstrs)
             self._gp_model.remove(self.genconstrs)
             self._gp_model.remove(self.sos)
             if self._first_callback:
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/register_user_predictor.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/register_user_predictor.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 
-""" Module for user to register a predictor for the function add_predictor_constr"""
+"""Module for user to register a predictor for the function add_predictor_constr."""
 USER_PREDICTORS = {}
 
 
 def register_predictor_constr(predictor, predictor_constr):
-    """Register a new predictor that can be added using use_predictor_constr
+    """Register a new predictor that can be added using use_predictor_constr.
 
     Parameters
     ----------
     predictor:
         Class of the predictor
     predictor_constr:
-        Class implementing the MIP formulation of a trained object of
-        class predictor in a gurobi Model <https://www.gurobi.com/documentation/9.5/refman/py_model.html>
+        Class implementing the MIP formulation of a trained object of class predictor
+        in a gurobi :gurobipy:`Model`.
     """
     USER_PREDICTORS[predictor] = predictor_constr
 
 
 def user_predictors():
-    """Returns dictionary of user defined predictors"""
+    """Returns dictionary of user defined predictors."""
     return USER_PREDICTORS
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/registered_predictors.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/registered_predictors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Define generic function that can add any known trained predictor
-"""
+"""Define generic function that can add any known trained predictor."""
 import sys
 
 from .register_user_predictor import user_predictors
 
 
 def sklearn_convertors():
-    """Collect convertors for Scikit-learn objects"""
+    """Collect convertors for Scikit-learn objects."""
     if "sklearn" in sys.modules:
         from .sklearn import (  # pylint: disable=import-outside-toplevel
             add_pipeline_constr,
         )
         from .sklearn.predictors_list import (  # pylint: disable=import-outside-toplevel
             sklearn_predictors,
         )
@@ -38,28 +37,28 @@
                 "Pipeline": add_pipeline_constr,
             }
         )
     return {}
 
 
 def pytorch_convertors():
-    """Collect known PyTorch objects that can be formulated and the conversion class"""
+    """Collect known PyTorch objects that can be formulated and the conversion class."""
     if "torch" in sys.modules:
         import torch  # pylint: disable=import-outside-toplevel
 
         from .torch import (  # pylint: disable=import-outside-toplevel
             add_sequential_constr,
         )
 
         return {torch.nn.Sequential: add_sequential_constr}
     return {}
 
 
 def keras_convertors():
-    """Collect known Keras objects that can be embedded and the conversion class"""
+    """Collect known Keras objects that can be embedded and the conversion class."""
     if "tensorflow" in sys.modules:
         from keras.engine.functional import (  # pylint: disable=import-outside-toplevel
             Functional,
         )
         from keras.engine.training import (  # pylint: disable=import-outside-toplevel
             Model,
         )
@@ -72,14 +71,14 @@
             Functional: add_keras_constr,
             Model: add_keras_constr,
         }
     return {}
 
 
 def registered_predictors():
-    """Return the list of registered predictors"""
+    """Return the list of registered predictors."""
     convertors = {}
     convertors |= sklearn_convertors()
     convertors |= pytorch_convertors()
     convertors |= keras_convertors()
     convertors |= user_predictors()
     return convertors
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/__init__.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/base_regressions.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/base_regressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for inserting simple Scikit-Learn regression models into a gurobipy model
+"""Module for inserting simple Scikit-Learn regression models into a gurobipy model.
 
 All linear models should work:
    - :external+sklearn:py:class:`sklearn.linear_model.LinearRegression`
    - :external+sklearn:py:class:`sklearn.linear_model.Ridge`
    - :external+sklearn:py:class:`sklearn.linear_model.Lasso`
-
 """
 
 
 from ..modeling import AbstractPredictorConstr
 from .skgetter import SKgetter
 
 
@@ -47,14 +46,14 @@
             self,
             gp_model,
             input_vars,
             output_vars,
             **kwargs,
         )
 
-    def add_regression_constr(self):
-        """Add the prediction constraints to Gurobi"""
+    def add_regression_constr(self, output=None):
+        """Add the prediction constraints to Gurobi."""
+        if output is None:
+            output = self.output
         coefs = self.predictor.coef_.reshape(-1, 1)
         intercept = self.predictor.intercept_
-        self.gp_model.addConstr(
-            self.output == self.input @ coefs + intercept, name="linreg"
-        )
+        self.gp_model.addConstr(output == self.input @ coefs + intercept, name="linreg")
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/column_transformer.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/column_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,61 +9,60 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for formulating a column transformer in a :gurobipy:`gurobipy model <Model>`"""
+"""Module for formulating a column transformer in a :gurobipy:`gurobipy model <Model>`."""
 
 import gurobipy as gp
 
 from .preprocessing import sklearn_transformers
 from .skgetter import SKtransformer
 
 
 class ColumnTransformerConstr(SKtransformer):
-    """Class to model a fitted :external+sklearn:py:class:`sklearn.compose.ColumnTransformer` with gurobipy
+    """Class to model a fitted :external+sklearn:py:class:`sklearn.compose.ColumnTransformer` with gurobipy.
 
     Note
     ----
     This object differs from all the other object in the Gurobi Machine Learning package in
     that it may not be possible to write all of its input with Gurobi variables. Specifically
     some input may consist of categorical features to be encoded using the column transformer.
 
     Then such input cannot be directly represented in Gurobi but the result of the encoding may be represented.
     If the categorical features are fixed for the optimization model, we can use it so it is allowed by
     the ColumnTransormerConstr class.
 
     The rule we use to apply the ColumnTransformer to the input is that if the set of columns to which a preprocessing
     transformation is constant in the input we use directly the scikit learn preprocessing object. It at least one of the columns
     is made of gurobipy variables, we use the gurobi-ml object (if it exists).
-
     """
 
     def __init__(self, gp_model, column_transformer, input_vars, **kwargs):
         self._default_name = "col_trans"
         super().__init__(gp_model, column_transformer, input_vars, **kwargs)
 
     # For this class we need to reimplement submodel because we don't want
     # to transform input variables to Gurobi variable. We can't do it for categorical
     # The input should be unchanged.
     def _build_submodel(self, gp_model, *args, **kwargs):
-        """Predict output from input using predictor or transformer"""
+        """Predict output from input using predictor or transformer."""
         _input = self.input
         if hasattr(self._input, "columns"):
             self._input_columns = _input.columns
         if hasattr(self._input, "index"):
             self._input_index = _input.index
         self._mip_model(**kwargs)
         assert self._output is not None
         return self
 
     def _mip_model(self, **kwargs):
-        """Do the transformation on x"""
+        """Do the transformation on x."""
         column_transform = self.transformer
         _input = self._input
         transformers = {k.lower(): v for k, v in sklearn_transformers().items()}
         transformed = []
         for name, trans, cols in column_transform.transformers_:
             if trans == "passthrough":
                 transformed.append(_input.loc[:, cols])
@@ -80,26 +79,25 @@
                     transformed.append(trans_constr.output.tolist())
                 else:
                     transformed.append(trans.transform(_input.loc[:, cols]))
         self._output = column_transform._hstack(transformed)
 
 
 def add_column_transformer_constr(gp_model, column_transformer, input_vars, **kwargs):
-    """Formulate column_transformer in gurobipy model
+    """Formulate column_transformer in gurobipy model.
 
     Parameters
     ----------
     gp_model : :gurobipy:`model`
         The gurobipy model where polynomial features should be inserted.
     column_transformer : :external+sklearn:py:class:`sklearn.compose.ColumnTransformer`
         The column transformer to insert in gp_model.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for polynomial features in model.
 
     Returns
     -------
     sklearn.preprocessing.ColumnTransformerConstr
         Object containing information about what was added to gp_model to insert the
         polynomial_features in it.
-
     """
     return ColumnTransformerConstr(gp_model, column_transformer, input_vars, **kwargs)
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/decision_tree_regressor.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/decision_tree_regressor.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for formulating a :external+sklearn:py:class:`sklearn.tree.DecisionTreeRegressor`
+"""Module for formulating a
+:external+sklearn:py:class:`sklearn.tree.DecisionTreeRegressor`
 in a :gurobipy:`model`.
 """
 
 import numpy as np
 from gurobipy import GRB
 
 from ..modeling import AbstractPredictorConstr
@@ -30,68 +31,75 @@
     input_vars,
     output_vars=None,
     epsilon=0.0,
     scale=1.0,
     float_type=np.float32,
     **kwargs
 ):
-    """Formulate decision_tree_regressor into gp_model
+    """Formulate decision_tree_regressor into gp_model.
 
-    The formulation predicts the values of output_vars using input_vars according to decision_tree_regressor.
-    See our :ref:`User's Guide <Decision Tree Regression>` for details on the mip formulation used.
+    The formulation predicts the values of output_vars using input_vars
+    according to decision_tree_regressor. See our :ref:`User's Guide <Decision
+    Tree Regression>` for details on the mip formulation used.
 
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the predictor should be inserted.
-    decision_tree_regressor: :external+sklearn:py:class:`sklearn.tree.DecisionTreeRegressor`
+    decision_tree_regressor : :external+sklearn:py:class:`sklearn.tree.DecisionTreeRegressor`
         The decision tree regressor to insert as predictor.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for decision tree in model.
-    output_vars: :gurobipy:`mvar` or :gurobipy:`var` array like, optional
+    output_vars : :gurobipy:`mvar` or :gurobipy:`var` array like, optional
         Decision variables used as output for decision tree in model.
-    epsilon: float, optional
-        Small value used to impose strict inequalities for splitting nodes in MIP formulations.
-    scale: float, optional
+    epsilon : float, optional
+        Small value used to impose strict inequalities for splitting nodes in
+        MIP formulations.
+    scale : float, optional
         Value
-    float_type: type, optional
-        Float type for the thresholds defining the node splits in the MIP formulation
+    float_type : type, optional
+        Float type for the thresholds defining the node splits in the MIP
+        formulation
 
     Returns
     -------
     DecisionTreeRegressorConstr
-        Object containing information about what was added to gp_model to formulate decision_tree_regressor
-
+        Object containing information about what was added to gp_model to
+        formulate decision_tree_regressor
 
     Note
     ----
+
     |VariablesDimensionsWarn|
 
     Warning
     -------
-    Although decision trees with multiple outputs are tested they were never used in
-    a non-trivial optimization model. It should be used with care at this point.
+
+    Although decision trees with multiple outputs are tested they were never
+    used in a non-trivial optimization model. It should be used with care at
+    this point.
     """
     return DecisionTreeRegressorConstr(
         gp_model,
         decision_tree_regressor,
         input_vars,
         output_vars,
         epsilon,
         scale,
         float_type,
         **kwargs
     )
 
 
 class DecisionTreeRegressorConstr(SKgetter, AbstractPredictorConstr):
-    """Class to model trained :external+sklearn:py:class:`sklearn.tree.DecisionTreeRegressor` with gurobipy
+    """Class to model trained
+    :external+sklearn:py:class:`sklearn.tree.DecisionTreeRegressor` with
+    gurobipy.
 
     |ClassShort|
-
     """
 
     def __init__(
         self,
         gp_model,
         predictor,
         input_vars,
@@ -115,15 +123,14 @@
         model = self._gp_model
 
         _input = self._input
         output = self._output
         outdim = output.shape[1]
         nex = _input.shape[0]
         nodes = model.addMVar((nex, tree.capacity), vtype=GRB.BINARY, name="node")
-        self.nodevars = nodes
 
         # Collect leafs and non-leafs nodes
         notleafs = tree.children_left >= 0
         leafs = tree.children_left < 0
 
         # Connectivity constraint
         model.addConstr(
@@ -175,12 +182,9 @@
             value = tree.value[node, :, 0]
             model.addConstrs(
                 (rhs[k] == 1) >> (lhs[k][i] == value[i])
                 for k in range(nex)
                 for i in range(outdim)
             )
 
-        # We should attain 1 leaf
-        model.addConstr(nodes[:, leafs].sum(axis=1) == 1)
-
         output.LB = np.min(tree.value)
         output.UB = np.max(tree.value)
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/gradient_boosting_regressor.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,66 +9,71 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for formulating a :external+sklearn:py:class:`sklearn.ensemble.GradientBoostingRegressor`
+"""Module for formulating a
+:external+sklearn:py:class:`sklearn.ensemble.GradientBoostingRegressor`
 into a :gurobipy:`model`.
 """
 
 from gurobipy import GRB
 
 from ..modeling import AbstractPredictorConstr
 from .decision_tree_regressor import add_decision_tree_regressor_constr
 from .skgetter import SKgetter
 
 
 def add_gradient_boosting_regressor_constr(
     gp_model, gradient_boosting_regressor, input_vars, output_vars=None, **kwargs
 ):
-    """Formulate gradient_boosting_regressor into gp_model
+    """Formulate gradient_boosting_regressor into gp_model.
 
-    The formulation predicts the values of output_vars using input_vars according to gradient_boosting_regressor.
-    See our :ref:`User's Guide <Gradient Boosting Regression>` for details on the mip formulation used.
+    The formulation predicts the values of output_vars using input_vars
+    according to gradient_boosting_regressor. See our :ref:`User's Guide
+    <Gradient Boosting Regression>` for details on the mip formulation used.
 
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the predictor should be inserted.
-    gradient_boosting_regressor: :external+sklearn:py:class:`sklearn.ensemble.GradientBoostingRegressor`
+    gradient_boosting_regressor : :external+sklearn:py:class:`sklearn.ensemble.GradientBoostingRegressor`
         The gradient boosting regressor to insert as predictor.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for gradient boosting regressor in model.
-    output_vars: :gurobipy:`mvar` or :gurobipy:`var` array like, optional
+    output_vars : :gurobipy:`mvar` or :gurobipy:`var` array like, optional
         Decision variables used as output for gradient boosting regressor in model.
+
     Returns
     -------
     GradientBoostingRegressorConstr
-        Object containing information about what was added to gp_model to formulate gradient_boosting_regressor.
+        Object containing information about what was added to gp_model to formulate
+        gradient_boosting_regressor.
 
     Note
     ----
     |VariablesDimensionsWarn|
 
-    Also see :py:func:`gurobi_ml.sklearn.decision_tree_regressor.add_decision_tree_regressor`
+    Also see
+    :py:func:`gurobi_ml.sklearn.decision_tree_regressor.add_decision_tree_regressor`
     for specific parameters to model decision tree estimators.
-
     """
     return GradientBoostingRegressorConstr(
         gp_model, gradient_boosting_regressor, input_vars, output_vars, **kwargs
     )
 
 
 class GradientBoostingRegressorConstr(SKgetter, AbstractPredictorConstr):
-    """Class to model trained :external+sklearn:py:class:`sklearn.ensemble.GradientBoostingRegressor` with gurobipy
+    """Class to model trained
+    :external+sklearn:py:class:`sklearn.ensemble.GradientBoostingRegressor`
+    with gurobipy.
 
     |ClassShort|
-
     """
 
     def __init__(self, gp_model, predictor, input_vars, output_vars, **kwargs):
         self._output_shape = 1
         self.estimators_ = []
         self._default_name = "gbtree_reg"
         SKgetter.__init__(self, predictor, input_vars)
@@ -110,15 +115,15 @@
         self.estimators_ = estimators
 
         model.addConstr(
             output == predictor.learning_rate * treevars.sum(axis=1) + constant[0][0]
         )
 
     def print_stats(self, abbrev=False, file=None):
-        """Print statistics on model additions stored by this class
+        """Print statistics on model additions stored by this class.
 
         This function prints detailed statistics on the variables
         and constraints that where added to the model.
 
         Includes a summary of the estimators that it contains.
 
         Arguments
@@ -128,16 +133,8 @@
             Text stream to which output should be redirected. By default sys.stdout.
         """
         super().print_stats(abbrev=abbrev, file=file)
         if abbrev:
             return
         print(file=file)
 
-        header = f"{'Estimator':13} {'Output Shape':>14} {'Variables':>12} {'Constraints':^38}"
-        print("-" * len(header), file=file)
-        print(header, file=file)
-        print(f"{' '*41} {'Linear':>12} {'Quadratic':>12} {'General':>12}", file=file)
-        print("=" * len(header), file=file)
-        for estimator in self.estimators_:
-            estimator.print_stats(abbrev=True, file=file)
-            print(file=file)
-        print("-" * len(header), file=file)
+        self._print_container_steps("Estimator", self.estimators_, file=file)
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/linear_regression.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/linear_regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,73 +9,77 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for inserting ordinary Scikit-Learn regression models into a :gurobipy:`model`
+"""Module for inserting ordinary Scikit-Learn regression models into a
+:gurobipy:`model`.
 
 The following linear models are tested and should work:
    - :external+sklearn:py:class:`sklearn.linear_model.LinearRegression`
    - :external+sklearn:py:class:`sklearn.linear_model.Ridge`
    - :external+sklearn:py:class:`sklearn.linear_model.Lasso`
 """
 
 from .base_regressions import BaseSKlearnRegressionConstr
 
 
 def add_linear_regression_constr(
     gp_model, linear_regression, input_vars, output_vars=None, **kwargs
 ):
-    """Formulate linear_regression in gp_model
+    """Formulate linear_regression in gp_model.
 
-    The formulation predicts the values of output_vars using input_vars according to linear_regression.
-    See our :ref:`Users Guide <Linear Regression>` for details on the mip formulation used.
+    The formulation predicts the values of output_vars using input_vars according to
+    linear_regression. See our :ref:`Users Guide <Linear Regression>` for details on the
+    mip formulation used.
 
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the predictor should be inserted.
-    linear_regression: :external+sklearn:py:class:`sklearn.linear_model.LinearRegression`
+    linear_regression : :external+sklearn:py:class:`sklearn.linear_model.LinearRegression`
      The linear regression to insert. It can be of any of the following types:
          * :external+sklearn:py:class:`sklearn.linear_model.LinearRegression`
          * :external+sklearn:py:class:`sklearn.linear_model.Ridge`
          * :external+sklearn:py:class:`sklearn.linear_model.Lasso`
      input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
          Decision variables used as input for random forest in model.
      output_vars: :gurobipy:`mvar` or :gurobipy:`var` array like, optional
          Decision variables used as output for random forest in model.
 
     Returns
     -------
     LinearRegressionConstr
-        Object containing information about what was added to gp_model to formulate linear_regression.
+        Object containing information about what was added to gp_model to formulate
+        linear_regression.
 
     Note
     ----
     |VariablesDimensionsWarn|
     """
     return LinearRegressionConstr(
         gp_model, linear_regression, input_vars, output_vars, **kwargs
     )
 
 
 class LinearRegressionConstr(BaseSKlearnRegressionConstr):
-    """Class to model trained :external+sklearn:py:class:`sklearn.linear_model.LinearRegression` with gurobipy
-
-    |ClassShort|"""
+    """Class to model trained
+    :external+sklearn:py:class:`sklearn.linear_model.LinearRegression` with gurobipy
+    |ClassShort|.
+    """
 
     def __init__(self, gp_model, predictor, input_vars, output_vars=None, **kwargs):
         self._default_name = "lin_reg"
         BaseSKlearnRegressionConstr.__init__(
             self,
             gp_model,
             predictor,
             input_vars,
             output_vars,
             **kwargs,
         )
 
     def _mip_model(self, **kwargs):
-        """Add the prediction constraints to Gurobi"""
+        """Add the prediction constraints to Gurobi."""
         self.add_regression_constr()
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/logistic_regression.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/logistic_regression.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for formulating a :external+sklearn:py:class:`sklearn.linear_model.LogisticRegression` in a
-:gurobipy:`model`
+"""Module for formulating a
+:external+sklearn:py:class:`sklearn.linear_model.LogisticRegression` in a
+:gurobipy:`model`.
 """
 
 import gurobipy as gp
 import numpy as np
 
 from ..exceptions import NoModel, ParameterError
 from .base_regressions import BaseSKlearnRegressionConstr
@@ -30,70 +31,73 @@
     input_vars,
     output_vars=None,
     output_type="classification",
     epsilon=0.0,
     pwl_attributes=None,
     **kwargs,
 ):
-    """Formulate logistic_regression in gp_model
+    """Formulate logistic_regression in gp_model.
 
-    The formulation predicts the values of output_vars using input_vars according to logistic_regression.
+    The formulation predicts the values of output_vars using input_vars according to
+    logistic_regression.
 
     Note that the model uses a piecewise linear approximation of the logistic function.
-    The quality of the approximation can be controlled with the parameter pwl_attributes.
-    By default, it is parametrized so that the maximal error of the approximation is `1e-2`.
-    See our :ref:`Users Guide <Logistic Regression>` for details on the mip formulation used.
-
-
+    The quality of the approximation can be controlled with the parameter
+    pwl_attributes. By default, it is parametrized so that the maximal error of the
+    approximation is `1e-2`. See our :ref:`Users Guide <Logistic Regression>` for
+    details on the mip formulation used.
 
     Parameters
     ----------
 
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the predictor should be inserted.
-    logistic_regression: :external+sklearn:py:class:`sklearn.linear_model.LogisticRegression`
+    logistic_regression : :external+sklearn:py:class:`sklearn.linear_model.LogisticRegression`
         The logistic regression to insert.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for logistic regression in model.
-    output_vars: :gurobipy:`mvar` or :gurobipy:`var` array like, optional
+    output_vars : :gurobipy:`mvar` or :gurobipy:`var` array like, optional
         Decision variables used as output for logistic regression in model.
 
-    output_type: {'classification', 'probability_1'}, default='classification'
+    output_type : {'classification', 'probability_1'}, default='classification'
         If the option chosen is 'classification' the output is the class label
-        of either 0 or 1 given by the logistic regression.
-        If the option 'probability_1' is chosen the output is the probability of the class 1.
+        of either 0 or 1 given by the logistic regression. If the option
+        'probability_1' is chosen the output is the probability of the class 1.
 
-    epsilon: float, default=0.0
+    epsilon : float, default=0.0
         When the `output_type` is 'classification', this tolerance can be set
-        to enforce that class 1 is chosen when the result of the logistic function is greater or
-        equal to *0.5 + epsilon*.
+        to enforce that class 1 is chosen when the result of the logistic
+        function is greater or equal to *0.5 + epsilon*.
 
-        By default, with the value of *0.0*, if the result of the logistic function is
-        very close to *0.5* (up to Gurobi tolerances) in the solution of the optimization model,
-        the output of the regression can be either 0 or 1.
-        The optimization model doesn't make a distinction between the two values.
-
-        Setting *esilon* to a small value will remove this ambiguity on the output but may
-        also make the model infeasible if the problem is very constrained:
-        the open interval *(0.5, 0.5 + epsilon)* is excluded from the feasible set of the optimization
-        problem.
-
-    pwl_attributes: dict, optional
-        Dictionary for non-default attributes for Gurobi to build the piecewise linear
-        approximation of the logistic function.
-        The default values for those attributes set in the package can be obtained
-        with LogisticRegressionConstr.default_pwl_attributes().
-        The dictionary keys should be the `attributes for modeling piece wise linear functions
+        By default, with the value of *0.0*, if the result of the logistic
+        function is very close to *0.5* (up to Gurobi tolerances) in the
+        solution of the optimization model, the output of the regression can be
+        either 0 or 1. The optimization model doesn't make a distinction
+        between the two values.
+
+        Setting *esilon* to a small value will remove this ambiguity on the
+        output but may also make the model infeasible if the problem is very
+        constrained: the open interval *(0.5, 0.5 + epsilon)* is excluded from
+        the feasible set of the optimization problem.
+
+    pwl_attributes : dict, optional
+        Dictionary for non-default attributes for Gurobi to build the piecewise
+        linear approximation of the logistic function. The default values for
+        those attributes set in the package can be obtained with
+        LogisticRegressionConstr.default_pwl_attributes(). The dictionary keys
+        should be the `attributes for modeling piece wise linear functions
         <https://www.gurobi.com/documentation/9.1/refman/general_constraint_attribu.html>`_
-        and the values the corresponding value the users wants to pass to Gurobi.
+        and the values the corresponding value the users wants to pass to
+        Gurobi.
 
     Returns
     -------
     LogisticRegressionConstr
-        Object containing information about what was added to gp_model to formulate logistic_regression.
+        Object containing information about what was added to gp_model to formulate
+        logistic_regression.
 
     Raises
     ------
 
     NoModel
         If the logistic regression is not a binary label regression
 
@@ -113,17 +117,18 @@
         epsilon,
         pwl_attributes=pwl_attributes,
         **kwargs,
     )
 
 
 class LogisticRegressionConstr(BaseSKlearnRegressionConstr):
-    """Class to model trained :external+sklearn:py:class:`sklearn.linear_model.LogisticRegression` with gurobipy
-
-    |ClassShort|"""
+    """Class to model trained
+    :external+sklearn:py:class:`sklearn.linear_model.LogisticRegression` with gurobipy
+    |ClassShort|.
+    """
 
     def __init__(
         self,
         gp_model,
         predictor,
         input_vars,
         output_vars=None,
@@ -154,50 +159,54 @@
             output_vars,
             output_type,
             **kwargs,
         )
 
     @staticmethod
     def default_pwl_attributes():
-        """Default attributes for approximating the logistic function with Gurobi
+        """Default attributes for approximating the logistic function with Gurobi.
 
-        See `Gurobi's User Manual <https://www.gurobi.com/documentation/9.1/refman/general_constraint_attribu.html>`_
+        See `Gurobi's User Manual
+        <https://www.gurobi.com/documentation/9.1/refman/general_constraint_attribu.html>`_
         for the meaning of the attributes.
         """
         return {
             "FuncPieces": -1,
             "FuncPieceLength": 0.01,
             "FuncPieceError": 0.01,
             "FuncPieceRatio": -1.0,
         }
 
     def _mip_model(self, **kwargs):
-        """Add the prediction constraints to Gurobi"""
-        outputvars = self._output
-        self._create_output_vars(self._input, name="affine_trans")
-        affinevars = self._output
-        self.add_regression_constr()
+        """Add the prediction constraints to Gurobi."""
         if self.output_type == "classification":
             # For classification we need an extra binary variable
-            self._create_output_vars(self._input, name="log_result")
-            log_result = self._output
-            self.gp_model.addConstr(outputvars >= log_result - 0.5 + self.epsilon)
-            self.gp_model.addConstr(outputvars <= log_result + 0.5)
-            outputvars.VType = gp.GRB.BINARY
-            outputvars.LB = 0.0
-            outputvars.UB = 1.0
+            log_result = self._gp_model.addMVar(
+                self.output.shape, lb=-gp.GRB.INFINITY, name="log_result"
+            )
+            bin_output = self.gp_model.addMVar(
+                self.output.shape, vtype=gp.GRB.BINARY, name="bin_output"
+            )
+
+            self.gp_model.addConstr(bin_output >= log_result - 0.5 + self.epsilon)
+            self.gp_model.addConstr(bin_output <= log_result + 0.5)
+            self.gp_model.addConstr(bin_output == self.output)
         else:
-            log_result = outputvars
+            log_result = self.output
+
+        affinevars = self._gp_model.addMVar(
+            self.output.shape, lb=-gp.GRB.INFINITY, name="affine_trans"
+        )
+        self.add_regression_constr(output=affinevars)
 
-        self._output = outputvars
-        for index in np.ndindex(outputvars.shape):
-            gc = self.gp_model.addGenConstrLogistic(
+        for index in np.ndindex(self.output.shape):
+            self.gp_model.addGenConstrLogistic(
                 affinevars[index],
                 log_result[index],
                 name=self._indexed_name(index, "logistic"),
             )
         num_gc = self.gp_model.NumGenConstrs
         self.gp_model.update()
-        for gc in self.gp_model.getGenConstrs()[num_gc:]:
+        for gen_constr in self.gp_model.getGenConstrs()[num_gc:]:
             for attr, val in self.attributes.items():
-                gc.setAttr(attr, val)
+                gen_constr.setAttr(attr, val)
         self.gp_model.update()
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/mlpregressor.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/mlpregressor.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,66 +9,68 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for formulating a :external+sklearn:py:class:`sklearn.neural_network.MLPRegressor` in a
-:gurobipy:`model`
+"""Module for formulating a :external+sklearn:py:class:`sklearn.neural_network.MLPRegressor` in a
+:gurobipy:`model`.
 """
 from ..exceptions import NoModel
 from ..modeling.neuralnet import BaseNNConstr
 from .skgetter import SKgetter
 
 
 def add_mlp_regressor_constr(
     gp_model, mlp_regressor, input_vars, output_vars=None, **kwargs
 ):
-    """Formulate mlp_regressor in gp_model
+    """Formulate mlp_regressor in gp_model.
 
-    The formulation predicts the values of output_vars using input_vars according to mlp_regressor.
-    See our :ref:`Users Guide <Neural Networks>` for details on the mip formulation used.
+    The formulation predicts the values of output_vars using input_vars according to
+    mlp_regressor. See our :ref:`Users Guide <Neural Networks>` for details on the mip
+    formulation used.
 
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the predictor should be inserted.
-    mlpregressor: :external+sklearn:py:class:`sklearn.neural_network.MLPRegressor`
+    mlpregressor : :external+sklearn:py:class:`sklearn.neural_network.MLPRegressor`
         The multi-layer perceptron regressor to insert as predictor.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for regression in model.
-    output_vars: :gurobipy:`mvar` or :gurobipy:`var` array like, optional
+    output_vars : :gurobipy:`mvar` or :gurobipy:`var` array like, optional
         Decision variables used as output for regression in model.
 
     Returns
     -------
     MLPRegressorConstr
-        Object containing information about what was added to gp_model to formulate mlp_regressor.
+        Object containing information about what was added to gp_model to formulate
+        mlp_regressor.
 
     Raises
     ------
     NoModel
-        If the translation to Gurobi of the activation function for the network
-        is not implemented.
+        If the translation to Gurobi of the activation function for the network is not
+        implemented.
 
     Note
     ----
     |VariablesDimensionsWarn|
     """
     return MLPRegressorConstr(
         gp_model, mlp_regressor, input_vars, output_vars, **kwargs
     )
 
 
 class MLPRegressorConstr(SKgetter, BaseNNConstr):
-    """Class to model trained :external+sklearn:py:class:`sklearn.neural_network.MLPRegressor` with gurobipy
+    """Class to model trained
+    :external+sklearn:py:class:`sklearn.neural_network.MLPRegressor` with gurobipy.
 
     |ClassShort|
-
     """
 
     def __init__(
         self,
         gp_model,
         predictor,
         input_vars,
@@ -85,15 +87,15 @@
             output_vars,
             clean_predictor=clean_predictor,
             **kwargs,
         )
         assert predictor.out_activation_ in ("identity", "relu")
 
     def _mip_model(self, **kwargs):
-        """Add the prediction constraints to Gurobi"""
+        """Add the prediction constraints to Gurobi."""
         neural_net = self.predictor
         if neural_net.activation not in self.act_dict:
             print(self.act_dict)
             raise NoModel(
                 neural_net,
                 f"No implementation for activation function {neural_net.activation}",
             )
@@ -113,13 +115,14 @@
 
             layer = self.add_dense_layer(
                 input_vars,
                 layer_coefs,
                 layer_intercept,
                 activation,
                 output,
+                **kwargs,
             )
             input_vars = layer._output  # pylint: disable=W0212
             self._gp_model.update()
         assert (
             self._output is not None
         )  # Should never happen since sklearn object defines n_ouputs_
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/pipeline.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for formulating a :external+sklearn:py:class:`sklearn.pipeline.Pipeline`
+"""Module for formulating a :external+sklearn:py:class:`sklearn.pipeline.Pipeline`
 in a :gurobipy:`model`.
 """
 
 
 from ..exceptions import NoModel
 from ..modeling.base_predictor_constr import AbstractPredictorConstr
 from ..modeling.get_convertor import get_convertor
@@ -25,27 +25,28 @@
 from .column_transformer import add_column_transformer_constr
 from .predictors_list import sklearn_predictors
 from .preprocessing import sklearn_transformers
 from .skgetter import SKgetter
 
 
 def add_pipeline_constr(gp_model, pipeline, input_vars, output_vars=None, **kwargs):
-    """Formulate pipeline into gp_model
+    """Formulate pipeline into gp_model.
 
-    The formulation predicts the values of output_vars using input_vars according to pipeline.
+    The formulation predicts the values of output_vars using input_vars according to
+    pipeline.
 
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the predictor should be inserted.
-    pipeline: :external+sklearn:py:class:`sklearn.pipeline.Pipeline`
+    pipeline : :external+sklearn:py:class:`sklearn.pipeline.Pipeline`
         The pipeline to insert as predictor.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for regression in model.
-    output_vars: :gurobipy:`mvar` or :gurobipy:`var` array like, optional
+    output_vars : :gurobipy:`mvar` or :gurobipy:`var` array like, optional
         Decision variables used as output for regression in model.
 
     Returns
     -------
     PipelineConstr
         Object containing information about what was added to gp_model to embed the
         predictor into it
@@ -60,28 +61,29 @@
     ----
     |VariablesDimensionsWarn|
     """
     return PipelineConstr(gp_model, pipeline, input_vars, output_vars, **kwargs)
 
 
 class PipelineConstr(SKgetter, AbstractPredictorConstr):
-    """Class to model trained :external+sklearn:py:class:`sklearn.pipeline.Pipeline` with gurobipy
-
-    |ClassShort|"""
+    """Class to model trained :external+sklearn:py:class:`sklearn.pipeline.Pipeline`
+    with gurobipy
+    |ClassShort|.
+    """
 
     def __init__(self, gp_model, pipeline, input_vars, output_vars=None, **kwargs):
         self._steps = []
         self._default_name = "pipe"
         SKgetter.__init__(self, pipeline, input_vars, **kwargs)
         AbstractPredictorConstr.__init__(
             self, gp_model, input_vars, output_vars, validate_input=False, **kwargs
         )
 
     def _build_submodel(self, gp_model, *args, **kwargs):
-        """Predict output from input using predictor or transformer
+        """Predict output from input using predictor or transformer.
 
         Pipelines are different from other objects because they can't validate
         their input and output. They are just containers of other objects that will
         do it.
         """
         self._mip_model(**kwargs)
         assert self.output is not None
@@ -93,14 +95,15 @@
     def _mip_model(self, **kwargs):
         pipeline = self.predictor
         gp_model = self._gp_model
         input_vars = self._input
         output_vars = self._output
         steps = self._steps
         transformers = sklearn_transformers()
+        transformers |= user_predictors()
         transformers["ColumnTransformer"] = add_column_transformer_constr
         kwargs["validate_input"] = True
 
         for transformer in pipeline[:-1]:
             convertor = get_convertor(transformer, transformers)
             if convertor is None:
                 raise NoModel(
@@ -119,15 +122,15 @@
                 f"I don't know how to deal with that object: {predictor}",
             )
         steps.append(convertor(gp_model, predictor, input_vars, output_vars, **kwargs))
         if self._output is None:
             self._output = steps[-1].output
 
     def print_stats(self, file=None):
-        """Print statistics on model additions stored by this class
+        """Print statistics on model additions stored by this class.
 
         This function prints detailed statistics on the variables
         and constraints that where added to the model.
 
         The pipeline version includes a summary of the steps that it contains.
 
         Arguments
@@ -137,54 +140,44 @@
             Text stream to which output should be redirected. By default sys.stdout.
         """
         super().print_stats(file=file)
         print(file=file)
         print(f"Pipeline has {len(self._steps)} steps:", file=file)
         print(file=file)
 
-        header = (
-            f"{'Step':13} {'Output Shape':>14} {'Variables':>12} {'Constraints':^38}"
-        )
-        print("-" * len(header), file=file)
-        print(header, file=file)
-        print(f"{' '*41} {'Linear':>12} {'Quadratic':>12} {'General':>12}", file=file)
-        print("=" * len(header), file=file)
-        for step in self:
-            step.print_stats(abbrev=True, file=file)
-            print(file=file)
-        print("-" * len(header), file=file)
+        self._print_container_steps("Step", self._steps, file=file)
 
     @property
     def _has_solution(self):
         return self[-1]._has_solution
 
     @property
     def output(self):
-        """Returns output variables of pipeline, i.e. output of its last step"""
+        """Returns output variables of pipeline, i.e. output of its last step."""
         return self[-1].output
 
     @property
     def output_values(self):
-        """Returns output values of pipeline in solution, i.e. output of its last step"""
+        """Returns output values of pipeline in solution, i.e. output of its last step."""
         return self[-1].output_values
 
     @property
     def input(self):
-        """Returns input variables of pipeline, i.e. input of its first step"""
+        """Returns input variables of pipeline, i.e. input of its first step."""
         return self[0].input
 
     @property
     def input_values(self):
-        """Returns input values of pipeline in solution, i.e. input of its first step"""
+        """Returns input values of pipeline in solution, i.e. input of its first step."""
         return self[0].input_values
 
     def __getitem__(self, key):
-        """Get an item from the pipeline steps"""
+        """Get an item from the pipeline steps."""
         return self._steps[key]
 
     def __iter__(self):
-        """Iterate through pipeline steps"""
+        """Iterate through pipeline steps."""
         return self._steps.__iter__()
 
     def __len__(self):
-        """Get number of pipeline steps"""
+        """Get number of pipeline steps."""
         return self._steps.__len__()
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/pls_regression.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/pls_regression.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,61 +9,64 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for formulating simple Scikit-Learn PLS regression models in a gurobipy model
-"""
+"""Module for formulating simple Scikit-Learn PLS regression models in a gurobipy model."""
 
 import numpy as np
 
 from ..modeling import AbstractPredictorConstr
 from .skgetter import SKgetter
 
 
 def add_pls_regression_constr(
     gp_model, pls_regression, input_vars, output_vars=None, **kwargs
 ):
-    """Formulate pls_regression in gp_model
+    """Formulate pls_regression in gp_model.
 
-    The formulation predicts the values of output_vars using input_vars according to pls_regression.
+    The formulation predicts the values of output_vars using input_vars
+    according to pls_regression.
 
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the predictor should be inserted.
-    pls_regression: :external+sklearn:py:class:`sklearn.cross_decomposition.PLSRegression`
+    pls_regression : :external+sklearn:py:class:`sklearn.cross_decomposition.PLSRegression`
      The linear regression to insert. It can be of any of the following types:
          * :external+sklearn:py:class:`sklearn.cross_decomposition.PLSRegression`
          * :external+sklearn:py:class:`sklearn.cross_decomposition.PLSCanonical`
      input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
          Decision variables used as input for random forest in model.
      output_vars: :gurobipy:`mvar` or :gurobipy:`var` array like, optional
          Decision variables used as output for random forest in model.
 
     Returns
     -------
     PLSRegressionConstr
-        Object containing information about what was added to gp_model to formulate pls_regression.
+        Object containing information about what was added to gp_model to
+        formulate pls_regression.
 
     Note
     ----
     |VariablesDimensionsWarn|
     """
     return PLSRegressionConstr(
         gp_model, pls_regression, input_vars, output_vars, **kwargs
     )
 
 
 class PLSRegressionConstr(SKgetter, AbstractPredictorConstr):
-    """Class to model trained :external+sklearn:py:class:`sklearn.cross_decomposition.PLSRegression` with gurobipy
-
-    |ClassShort|"""
+    """Class to model trained
+    :external+sklearn:py:class:`sklearn.cross_decomposition.PLSRegression` with
+    gurobipy
+    |ClassShort|.
+    """
 
     def __init__(
         self,
         gp_model,
         predictor,
         input_vars,
         output_vars=None,
@@ -77,23 +80,23 @@
             gp_model,
             input_vars,
             output_vars,
             **kwargs,
         )
 
     def add_regression_constr(self):
-        """Add the prediction constraints to Gurobi"""
+        """Add the prediction constraints to Gurobi."""
         x_mean = self.predictor._x_mean
         x_std = self.predictor._x_std
         coefs = self.predictor._coef_.T
         intercept = self.predictor.intercept_
         self.gp_model.addConstr(
             self.output
             == self.input @ (coefs / x_std[:, np.newaxis])
             - x_mean / x_std @ coefs
             + intercept,
             name="plsreg",
         )
 
     def _mip_model(self, **kwargs):
-        """Add the prediction constraints to Gurobi"""
+        """Add the prediction constraints to Gurobi."""
         self.add_regression_constr()
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/predictors_list.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/predictors_list.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/preprocessing.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,114 +9,117 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Implementation for using sklearn preprocessing object in a
-Guobi model"""
+"""Implementation for using sklearn preprocessing object in a
+Guobi model.
+"""
 
 import gurobipy as gp
 
 from ..exceptions import NoModel
 from .skgetter import SKtransformer
 
 
 def add_polynomial_features_constr(gp_model, polynomial_features, input_vars, **kwargs):
-    """Formulate polynomial_features into gp_model
+    """Formulate polynomial_features into gp_model.
 
     Note that this function creates the output variables from
     the input variables.
 
-    Warning
-    -------
-    Only polynomial features of degree 2 are supported.
-
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where polynomial features should be inserted.
-    polynomial_features: :external+sklearn:py:class:`sklearn.preprocessing.PolynomialFeatures`
+    polynomial_features : :external+sklearn:py:class:`sklearn.preprocessing.PolynomialFeatures`
         The polynomial features to insert in gp_model.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for polynomial features in model.
 
     Returns
     -------
     sklearn.preprocessing.PolynomialFeaturesConstr
         Object containing information about what was added to gp_model to insert the
         polynomial_features in it
 
+    Warning
+    -------
+    Only polynomial features of degree 2 are supported.
     """
     return PolynomialFeaturesConstr(gp_model, polynomial_features, input_vars, **kwargs)
 
 
 def add_standard_scaler_constr(gp_model, standard_scaler, input_vars, **kwargs):
-    """Formulate standard_scaler into gp_model
+    """Formulate standard_scaler into gp_model.
 
     Note that this function creates the output variables from
     the input variables.
 
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the standard scaler should be inserted.
-    standard_scaler: :external+sklearn:py:class:`sklearn.preprocessing.StandardScaler`
+    standard_scaler : :external+sklearn:py:class:`sklearn.preprocessing.StandardScaler`
         The standard scaler to insert as predictor.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for standard scaler in model.
 
     Returns
     -------
     sklearn.preprocessing.StandardScalerConstr
         Object containing information about what was added to gp_model to insert the
         standard_scaler in it
-
     """
     return StandardScalerConstr(gp_model, standard_scaler, input_vars, **kwargs)
 
 
 class StandardScalerConstr(SKtransformer):
-    """Class to model a fitted :external+sklearn:py:class:`sklearn.preprocessing.StandardScaler` with gurobipy
+    """Class to model a fitted
+    :external+sklearn:py:class:`sklearn.preprocessing.StandardScaler` with
+    gurobipy.
 
     Stores the changes to :gurobipy:`model` when embedding an instance into it.
-
     """
 
     def __init__(self, gp_model, scaler, input_vars, **kwargs):
         self._default_name = "std_scaler"
         self._output_shape = scaler.n_features_in_
         super().__init__(gp_model, scaler, input_vars, **kwargs)
 
     def _mip_model(self, **kwargs):
-        """Do the transformation on x"""
+        """Do the transformation on x."""
         _input = self._input
         output = self._output
 
         scale = self.transformer.scale_
         mean = self.transformer.mean_
 
         self._gp_model.addConstr(_input - output * scale == mean, name="s")
         return self
 
 
 class PolynomialFeaturesConstr(SKtransformer):
-    """Class to model trained :external+sklearn:py:class:`sklearn.preprocessing.PolynomialFeatures` with gurobipy"""
+    """Class to model trained
+    :external+sklearn:py:class:`sklearn.preprocessing.PolynomialFeatures` with
+    gurobipy.
+    """
 
     def __init__(self, gp_model, polynomial_features, input_vars, **kwargs):
         if polynomial_features.degree > 2:
             raise NoModel(
                 polynomial_features, "Can only handle polynomials of degree < 2"
             )
         self._default_name = "poly_feat"
         super().__init__(gp_model, polynomial_features, input_vars, **kwargs)
 
     def _mip_model(self, **kwargs):
-        """Do the transformation on x"""
+        """Do the transformation on x."""
         _input = self._input
         output = self._output
 
         n_examples, n_feat = _input.shape
         powers = self.transformer.powers_
         assert powers.shape[0] == self.transformer.n_output_features_
         assert powers.shape[1] == n_feat
@@ -133,11 +136,12 @@
                         q_expr *= feat.item()
                 self.gp_model.addConstr(
                     output[k, i] == q_expr, name=f"polyfeat[{k},{i}]"
                 )
 
 
 def sklearn_transformers():
+    """Return dictionary of Scikit Learn preprocessing objects."""
     return {
         "StandardScaler": add_standard_scaler_constr,
         "PolynomialFeatures": add_polynomial_features_constr,
     }
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/random_forest_regressor.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/random_forest_regressor.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,66 +9,71 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for formulating a :external+sklearn:py:class:`sklearn.ensemble.RandomForestRegressor`
+"""Module for formulating a
+:external+sklearn:py:class:`sklearn.ensemble.RandomForestRegressor`
 into a :gurobipy:`model`.
 """
 
 from gurobipy import GRB
 
 from ..modeling import AbstractPredictorConstr
 from .decision_tree_regressor import add_decision_tree_regressor_constr
 from .skgetter import SKgetter
 
 
 def add_random_forest_regressor_constr(
     gp_model, random_forest_regressor, input_vars, output_vars=None, **kwargs
 ):
-    """Formulate random_forest_regressor in gp_model
+    """Formulate random_forest_regressor in gp_model.
 
-    The formulation predicts the values of output_vars using input_vars according to random_forest_regressor.
-    See our :ref:`User's Guide <Random Forest Regression>` for details on the mip formulation used.
+    The formulation predicts the values of output_vars using input_vars according to
+    random_forest_regressor. See our :ref:`User's Guide <Random Forest Regression>` for
+    details on the mip formulation used.
 
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the predictor should be inserted.
-    random_forest_regressor: :external+sklearn:py:class:`sklearn.ensemble.RandomForestRegressor`
+    random_forest_regressor : :external+sklearn:py:class:`sklearn.ensemble.RandomForestRegressor`
         The random forest regressor to insert as predictor.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for random forest in model.
-    output_vars: :gurobipy:`mvar` or :gurobipy:`var` array like, optional
+    output_vars : :gurobipy:`mvar` or :gurobipy:`var` array like, optional
         Decision variables used as output for random forest in model.
 
     Returns
     -------
     RandomForestRegressorConstr
-       Object containing information about what was added to gp_model to formulate random_forest_regressor.
+       Object containing information about what was added to gp_model to formulate
+       random_forest_regressor.
 
     Note
     ----
     |VariablesDimensionsWarn|
 
-    Also see :py:func:`gurobi_ml.sklearn.decision_tree_regressor.add_decision_tree_regressor`
+    Also see
+    :py:func:`gurobi_ml.sklearn.decision_tree_regressor.add_decision_tree_regressor`
     for specific parameters to model decision tree estimators.
-
     """
     return RandomForestRegressorConstr(
         gp_model, random_forest_regressor, input_vars, output_vars, **kwargs
     )
 
 
 class RandomForestRegressorConstr(SKgetter, AbstractPredictorConstr):
-    """Class to model trained :external+sklearn:py:class:`sklearn.ensemble.RandomForestRegressor` with gurobipy
-
-    |ClassShort|"""
+    """Class to model trained
+    :external+sklearn:py:class:`sklearn.ensemble.RandomForestRegressor` with
+    gurobipy
+    |ClassShort|.
+    """
 
     def __init__(self, gp_model, predictor, input_vars, output_vars, **kwargs):
         self.estimators_ = []
         self._default_name = "rand_forest_reg"
         SKgetter.__init__(self, predictor, input_vars)
         AbstractPredictorConstr.__init__(
             self, gp_model, input_vars, output_vars, **kwargs
@@ -102,34 +107,26 @@
                 )
             )
         self.estimators_ = estimators
 
         model.addConstr(predictor.n_estimators * output == tree_vars.sum(axis=1))
 
     def print_stats(self, abbrev=False, file=None):
-        """Print statistics on model additions stored by this class
+        """Print statistics on model additions stored by this class.
 
         This function prints detailed statistics on the variables
         and constraints that where added to the model.
 
         Includes a summary of the estimators that it contains.
 
         Arguments
         ---------
 
         file: None, optional
             Text stream to which output should be redirected. By default sys.stdout.
         """
-        super().print_stats(file=file)
+        super().print_stats(abbrev=abbrev, file=file)
         if abbrev:
             return
         print(file=file)
 
-        header = f"{'Estimator':13} {'Output Shape':>14} {'Variables':>12} {'Constraints':^38}"
-        print("-" * len(header), file=file)
-        print(header, file=file)
-        print(f"{' '*41} {'Linear':>12} {'Quadratic':>12} {'General':>12}", file=file)
-        print("=" * len(header), file=file)
-        for estimator in self.estimators_:
-            estimator.print_stats(abbrev=True, file=file)
-            print(file=file)
-        print("-" * len(header), file=file)
+        self._print_container_steps("Estimator", self.estimators_, file=file)
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/sklearn/skgetter.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/skgetter.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,51 +9,50 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Implements some utility tools for all scikit-learn objects """
+"""Implements some utility tools for all scikit-learn objects."""
 
 import numpy as np
 from sklearn.utils.validation import check_is_fitted
 
 from ..exceptions import NoSolution
 from ..modeling import AbstractPredictorConstr
 
 
-class SKgetter:
-    """Utility class for sklearn regression models convertors
+class SKgetter(AbstractPredictorConstr):
+    """Utility class for sklearn regression models convertors.
 
     Implement some common functionalities: check predictor is fitted, output dimension, get error
 
     Attributes
     ----------
     predictor
         Scikit-Learn predictor embedded into Gurobi model.
-
     """
 
     def __init__(self, predictor, input_vars, output_type="regular", **kwargs):
         check_is_fitted(predictor)
         self.predictor = predictor
         predictor._check_feature_names(input_vars, reset=False)
         self.output_type = output_type
         if hasattr(predictor, "n_features_in_"):
             self._input_shape = predictor.n_features_in_
         if hasattr(predictor, "n_outputs_"):
             self._output_shape = predictor.n_outputs_
 
     def get_error(self):
-        """Returns error in Gurobi's solution with respect to prediction from input
+        """Return error in Gurobi's solution with respect to prediction from input.
 
         Returns
         -------
-        error: ndarray of same shape as :py:attr:`gurobi_ml.modeling.base_predictor_constr.AbstractPredictorConstr.output`
+        error : ndarray of same shape as :py:attr:`gurobi_ml.modeling.base_predictor_constr.AbstractPredictorConstr.output`
             Assuming that we have a solution for the input and output variables
             `x, y`. Returns the absolute value of the differences between `predictor.predict(x)` and
             `y`. Where predictor is the regression this object is modeling.
 
         Raises
         ------
         NoSolution
@@ -71,35 +70,48 @@
             if len(predicted.shape) == 1 and len(output_values.shape) == 2:
                 predicted = predicted.reshape(-1, 1)
             return np.abs(predicted - output_values)
         raise NoSolution()
 
 
 class SKtransformer(AbstractPredictorConstr):
-    """Utility class for sklearn preprocessing models convertors
+    """Utility class for sklearn preprocessing models convertors.
 
     Implement some common functionalities.
 
     Attributes
     ----------
     transformer
         Scikit-Learn transformer embedded into Gurobi model.
-
     """
 
     def __init__(self, gp_model, transformer, input_vars, **kwargs):
         self.transformer = transformer
         if hasattr(transformer, "n_features_in_"):
             self._input_shape = transformer.n_features_in_
         if hasattr(transformer, "n_output_features_"):
             self._output_shape = transformer.n_output_features_
         check_is_fitted(transformer)
         super().__init__(gp_model, input_vars, **kwargs)
 
     def get_error(self):
+        """Return error in Gurobi's solution with respect to preprocessing from input.
+
+        Returns
+        -------
+        error : ndarray of same shape as :py:attr:`gurobi_ml.modeling.base_predictor_constr.AbstractPredictorConstr.output`
+            Assuming that we have a solution for the input and output variables
+            `x, y`. Returns the absolute value of the differences between `transformer.transform(x)` and
+            `y`. Where transformer is the prepocessing this object is modeling.
+
+        Raises
+        ------
+        NoSolution
+            If the Gurobi model has no solution (either was not optimized or is infeasible).
+        """
         if self._has_solution:
             transformer = self.transformer
             input_values = self.input_values
 
             transformed = transformer.transform(input_values)
             if len(transformed.shape) == 1:
                 transformed = transformed.reshape(-1, 1)
```

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/torch/__init__.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.0b0/src/gurobi_ml/torch/sequential.py` & `gurobi-machinelearning-1.1.1/src/gurobi_ml/torch/sequential.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,77 +9,76 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-""" Module for formulating :external+torch:py:class:`torch.nn.Sequential` model in a
+"""Module for formulating :external+torch:py:class:`torch.nn.Sequential` model in a
 :gurobipy:`model`.
 """
 
 import numpy as np
 import torch
 from torch import nn
 
 from ..exceptions import NoModel, NoSolution
 from ..modeling.neuralnet import BaseNNConstr
 
 
 def add_sequential_constr(
     gp_model, sequential_model, input_vars, output_vars=None, **kwargs
 ):
-    """Formulate sequential_model into gp_model
+    """Formulate sequential_model into gp_model.
 
     The formulation predicts the values of output_vars using input_vars according to sequential_model.
     See our :ref:`Users Guide <Neural Networks>` for details on the mip formulation used.
 
-
     Parameters
     ----------
-    gp_model: :gurobipy:`model`
+    gp_model : :gurobipy:`model`
         The gurobipy model where the sequential model should be inserted.
-    sequential_model: :external+torch:py:class:`torch.nn.Sequential`
+    sequential_model : :external+torch:py:class:`torch.nn.Sequential`
         The sequential model to insert as predictor.
-    input_vars: :gurobipy:`mvar` or :gurobipy:`var` array like
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
         Decision variables used as input for logistic regression in model.
-    output_vars: :gurobipy:`mvar` or :gurobipy:`var` array like, optional
+    output_vars : :gurobipy:`mvar` or :gurobipy:`var` array like, optional
         Decision variables used as output for logistic regression in model.
 
     Returns
     -------
     SequentialConstr
         Object containing information about what was added to model to insert the
         predictor in it
 
-    Warning
-    -------
-    Only :external+torch:py:class:`torch.nn.Linear` layers and
-    :external+torch:py:class:`torch.nn.ReLU` layers are supported.
-
     Raises
     ------
     NoModel
         If the translation for some of the Pytorch model structure
         (layer or activation) is not implemented.
 
+    Warning
+    -------
+    Only :external+torch:py:class:`torch.nn.Linear` layers and
+    :external+torch:py:class:`torch.nn.ReLU` layers are supported.
+
     Note
     ----
     |VariablesDimensionsWarn|
     """
     return SequentialConstr(
         gp_model, sequential_model, input_vars, output_vars, **kwargs
     )
 
 
 class SequentialConstr(BaseNNConstr):
     """Transform a pytorch Sequential Neural Network to Gurobi constraint with
     input and output as matrices of variables.
-
-    |ClassShort|"""
+    |ClassShort|.
+    """
 
     def __init__(self, gp_model, predictor, input_vars, output_vars=None, **kwargs):
         for step in predictor:
             if isinstance(step, nn.ReLU):
                 pass
             elif isinstance(step, nn.Linear):
                 pass
@@ -94,30 +93,31 @@
         num_layers = len(network)
 
         for i, step in enumerate(network):
             if i == num_layers - 1:
                 output = self._output
             if isinstance(step, nn.ReLU):
                 layer = self.add_activation_layer(
-                    _input, self.act_dict["relu"], output, name="relu"
+                    _input, self.act_dict["relu"], output, name=f"relu_{i}", **kwargs
                 )
                 _input = layer.output
             elif isinstance(step, nn.Linear):
                 for name, param in step.named_parameters():
                     if name == "weight":
                         layer_weight = param.detach().numpy().T
                     elif name == "bias":
                         layer_bias = param.detach().numpy()
                 layer = self.add_dense_layer(
                     _input,
                     layer_weight,
                     layer_bias,
                     self.act_dict["identity"],
                     output,
-                    name="linear",
+                    name=f"linear_{i}",
+                    **kwargs,
                 )
                 _input = layer.output
         if self._output is None:
             self._output = layer.output
 
     def get_error(self):
         if self._has_solution:
```

