# Comparing `tmp/graphomaly-0.2.7.tar.gz` & `tmp/graphomaly-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphomaly-0.2.7.tar", last modified: Wed Apr 12 15:04:12 2023, max compression
+gzip compressed data, was "graphomaly-0.2.8.tar", last modified: Fri Apr 14 14:03:41 2023, max compression
```

## Comparing `graphomaly-0.2.7.tar` & `graphomaly-0.2.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.261259 graphomaly-0.2.7/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      718 2021-10-11 19:50:38.000000 graphomaly-0.2.7/LICENSE
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2670 2023-04-12 15:04:12.261259 graphomaly-0.2.7/PKG-INFO
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1955 2022-05-03 07:20:54.000000 graphomaly-0.2.7/README.md
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.254592 graphomaly-0.2.7/graphomaly/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       43 2022-03-01 20:47:00.000000 graphomaly-0.2.7/graphomaly/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    31674 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/estimator.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    25465 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/grid_search.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.254592 graphomaly-0.2.7/graphomaly/models/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       46 2022-02-27 21:19:37.000000 graphomaly-0.2.7/graphomaly/models/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    24065 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/models/autoencoder.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2684 2022-02-27 21:07:58.000000 graphomaly-0.2.7/graphomaly/models/base_model.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7950 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/models/dictlearn.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7111 2022-05-03 07:25:03.000000 graphomaly-0.2.7/graphomaly/models/models.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      731 2022-02-27 21:06:44.000000 graphomaly-0.2.7/graphomaly/models/sklearn.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    26574 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/models/vae.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4813 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/normalizations.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.257926 graphomaly-0.2.7/graphomaly/preprocessing/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-02-27 22:16:17.000000 graphomaly-0.2.7/graphomaly/preprocessing/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8556 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/egonet.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.257926 graphomaly-0.2.7/graphomaly/preprocessing/fe_base/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_base/__init__.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4642 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_base/historical_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    18634 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_base/statistical_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    12728 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_base/time_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     5112 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_difference_transformer.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8427 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_statistical_transformer.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9538 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/fe_time_transformers.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    33228 2022-09-27 19:49:32.000000 graphomaly-0.2.7/graphomaly/preprocessing/graph_to_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9095 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/graph_to_spectrum_features.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7204 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/rwalk.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6850 2022-05-03 07:20:54.000000 graphomaly-0.2.7/graphomaly/preprocessing/spectrum.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6129 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/preprocessing/transactions_to_graph.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)    36401 2023-04-12 14:59:15.000000 graphomaly-0.2.7/graphomaly/voting.py
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.257926 graphomaly-0.2.7/graphomaly.egg-info/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2670 2023-04-12 15:04:12.000000 graphomaly-0.2.7/graphomaly.egg-info/PKG-INFO
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1494 2023-04-12 15:04:12.000000 graphomaly-0.2.7/graphomaly.egg-info/SOURCES.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)        1 2023-04-12 15:04:12.000000 graphomaly-0.2.7/graphomaly.egg-info/dependency_links.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)      168 2023-04-12 15:04:12.000000 graphomaly-0.2.7/graphomaly.egg-info/requires.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       11 2023-04-12 15:04:12.000000 graphomaly-0.2.7/graphomaly.egg-info/top_level.txt
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)       99 2021-10-11 19:50:38.000000 graphomaly-0.2.7/pyproject.toml
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1180 2023-04-12 15:04:12.261259 graphomaly-0.2.7/setup.cfg
-drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-12 15:04:12.261259 graphomaly-0.2.7/tests/
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1619 2022-03-31 19:27:11.000000 graphomaly-0.2.7/tests/test_dl.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1501 2022-05-03 07:20:54.000000 graphomaly-0.2.7/tests/test_fe_time.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1991 2022-04-02 17:39:48.000000 graphomaly-0.2.7/tests/test_graphomaly_ctor.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1035 2022-04-02 17:24:08.000000 graphomaly-0.2.7/tests/test_synthetic.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1023 2022-04-02 17:10:58.000000 graphomaly-0.2.7/tests/test_synthetic_gridsearch.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     3264 2022-05-03 07:20:54.000000 graphomaly-0.2.7/tests/test_synthetic_preprocessing.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1084 2022-04-02 15:48:52.000000 graphomaly-0.2.7/tests/test_synthetic_voting.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1722 2022-03-15 18:50:57.000000 graphomaly-0.2.7/tests/test_tf_save.py
--rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1535 2022-03-01 23:27:25.000000 graphomaly-0.2.7/tests/test_voting.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.746382 graphomaly-0.2.8/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      718 2021-10-11 19:50:38.000000 graphomaly-0.2.8/LICENSE
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2670 2023-04-14 14:03:41.746382 graphomaly-0.2.8/PKG-INFO
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1955 2022-05-03 07:20:54.000000 graphomaly-0.2.8/README.md
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.739715 graphomaly-0.2.8/graphomaly/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       43 2022-03-01 20:47:00.000000 graphomaly-0.2.8/graphomaly/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    31674 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/estimator.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    25465 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/grid_search.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.743048 graphomaly-0.2.8/graphomaly/models/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       46 2022-02-27 21:19:37.000000 graphomaly-0.2.8/graphomaly/models/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    24065 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/models/autoencoder.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2684 2022-02-27 21:07:58.000000 graphomaly-0.2.8/graphomaly/models/base_model.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7950 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/models/dictlearn.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7111 2022-05-03 07:25:03.000000 graphomaly-0.2.8/graphomaly/models/models.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      731 2022-02-27 21:06:44.000000 graphomaly-0.2.8/graphomaly/models/sklearn.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    26574 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/models/vae.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4813 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/normalizations.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.743048 graphomaly-0.2.8/graphomaly/preprocessing/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-02-27 22:16:17.000000 graphomaly-0.2.8/graphomaly/preprocessing/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8556 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/egonet.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.743048 graphomaly-0.2.8/graphomaly/preprocessing/fe_base/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        0 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_base/__init__.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     4642 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_base/historical_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    18634 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_base/statistical_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    12728 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_base/time_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     5112 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_difference_transformer.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     8427 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_statistical_transformer.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9538 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/fe_time_transformers.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    33228 2022-09-27 19:49:32.000000 graphomaly-0.2.8/graphomaly/preprocessing/graph_to_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     9095 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/graph_to_spectrum_features.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     7204 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/rwalk.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6850 2022-05-03 07:20:54.000000 graphomaly-0.2.8/graphomaly/preprocessing/spectrum.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     6129 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/preprocessing/transactions_to_graph.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)    36401 2023-04-12 14:59:15.000000 graphomaly-0.2.8/graphomaly/voting.py
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.746382 graphomaly-0.2.8/graphomaly.egg-info/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     2670 2023-04-14 14:03:41.000000 graphomaly-0.2.8/graphomaly.egg-info/PKG-INFO
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1494 2023-04-14 14:03:41.000000 graphomaly-0.2.8/graphomaly.egg-info/SOURCES.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)        1 2023-04-14 14:03:41.000000 graphomaly-0.2.8/graphomaly.egg-info/dependency_links.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)      176 2023-04-14 14:03:41.000000 graphomaly-0.2.8/graphomaly.egg-info/requires.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       11 2023-04-14 14:03:41.000000 graphomaly-0.2.8/graphomaly.egg-info/top_level.txt
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)       99 2021-10-11 19:50:38.000000 graphomaly-0.2.8/pyproject.toml
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1188 2023-04-14 14:03:41.746382 graphomaly-0.2.8/setup.cfg
+drwxr-xr-x   0 pirofti   (1000) pirofti   (1000)        0 2023-04-14 14:03:41.746382 graphomaly-0.2.8/tests/
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1619 2022-03-31 19:27:11.000000 graphomaly-0.2.8/tests/test_dl.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1501 2022-05-03 07:20:54.000000 graphomaly-0.2.8/tests/test_fe_time.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1991 2022-04-02 17:39:48.000000 graphomaly-0.2.8/tests/test_graphomaly_ctor.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1035 2022-04-02 17:24:08.000000 graphomaly-0.2.8/tests/test_synthetic.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1023 2022-04-02 17:10:58.000000 graphomaly-0.2.8/tests/test_synthetic_gridsearch.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     3264 2022-05-03 07:20:54.000000 graphomaly-0.2.8/tests/test_synthetic_preprocessing.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1084 2022-04-02 15:48:52.000000 graphomaly-0.2.8/tests/test_synthetic_voting.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1722 2022-03-15 18:50:57.000000 graphomaly-0.2.8/tests/test_tf_save.py
+-rw-r--r--   0 pirofti   (1000) pirofti   (1000)     1535 2022-03-01 23:27:25.000000 graphomaly-0.2.8/tests/test_voting.py
```

### Comparing `graphomaly-0.2.7/LICENSE` & `graphomaly-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/PKG-INFO` & `graphomaly-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphomaly
-Version: 0.2.7
+Version: 0.2.8
 Summary: software package for anomaly detection in graphs modeling financial transactions
 Home-page: https://gitlab.com/unibuc/graphomaly/graphomaly
 Author: Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu
 Author-email: graphomaly@fmi.unibuc.ro
 Project-URL: Bug Tracker, https://gitlab.com/unibuc/graphomaly/graphomaly/-/issues
 Keywords: anomaly detection,graphs,financial transactions,machine learning,security
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphomaly-0.2.7/README.md` & `graphomaly-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/estimator.py` & `graphomaly-0.2.8/graphomaly/estimator.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/grid_search.py` & `graphomaly-0.2.8/graphomaly/grid_search.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/models/autoencoder.py` & `graphomaly-0.2.8/graphomaly/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/models/base_model.py` & `graphomaly-0.2.8/graphomaly/models/base_model.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/models/dictlearn.py` & `graphomaly-0.2.8/graphomaly/models/dictlearn.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/models/models.py` & `graphomaly-0.2.8/graphomaly/models/models.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/models/sklearn.py` & `graphomaly-0.2.8/graphomaly/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/models/vae.py` & `graphomaly-0.2.8/graphomaly/models/vae.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/normalizations.py` & `graphomaly-0.2.8/graphomaly/normalizations.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/egonet.py` & `graphomaly-0.2.8/graphomaly/preprocessing/egonet.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/fe_base/historical_features.py` & `graphomaly-0.2.8/graphomaly/preprocessing/fe_base/historical_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/fe_base/statistical_features.py` & `graphomaly-0.2.8/graphomaly/preprocessing/fe_base/statistical_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/fe_base/time_features.py` & `graphomaly-0.2.8/graphomaly/preprocessing/fe_base/time_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/fe_difference_transformer.py` & `graphomaly-0.2.8/graphomaly/preprocessing/fe_difference_transformer.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/fe_statistical_transformer.py` & `graphomaly-0.2.8/graphomaly/preprocessing/fe_statistical_transformer.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/fe_time_transformers.py` & `graphomaly-0.2.8/graphomaly/preprocessing/fe_time_transformers.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/graph_to_features.py` & `graphomaly-0.2.8/graphomaly/preprocessing/graph_to_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/graph_to_spectrum_features.py` & `graphomaly-0.2.8/graphomaly/preprocessing/graph_to_spectrum_features.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/rwalk.py` & `graphomaly-0.2.8/graphomaly/preprocessing/rwalk.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/spectrum.py` & `graphomaly-0.2.8/graphomaly/preprocessing/spectrum.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/preprocessing/transactions_to_graph.py` & `graphomaly-0.2.8/graphomaly/preprocessing/transactions_to_graph.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly/voting.py` & `graphomaly-0.2.8/graphomaly/voting.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/graphomaly.egg-info/PKG-INFO` & `graphomaly-0.2.8/graphomaly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphomaly
-Version: 0.2.7
+Version: 0.2.8
 Summary: software package for anomaly detection in graphs modeling financial transactions
 Home-page: https://gitlab.com/unibuc/graphomaly/graphomaly
 Author: Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu
 Author-email: graphomaly@fmi.unibuc.ro
 Project-URL: Bug Tracker, https://gitlab.com/unibuc/graphomaly/graphomaly/-/issues
 Keywords: anomaly detection,graphs,financial transactions,machine learning,security
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphomaly-0.2.7/graphomaly.egg-info/SOURCES.txt` & `graphomaly-0.2.8/graphomaly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/setup.cfg` & `graphomaly-0.2.8/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = graphomaly
-version = 0.2.7
+version = 0.2.8
 author = Paul Irofti, Ștefania Budulan, Bogdan Dumitrescu, Andra Băltoiu
 author_email = graphomaly@fmi.unibuc.ro
 description = software package for anomaly detection in graphs modeling financial transactions
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = anomaly detection, graphs, financial transactions, machine learning, security
 url = https://gitlab.com/unibuc/graphomaly/graphomaly
@@ -22,22 +22,22 @@
 python_requires = >=3.6
 install_requires = 
 	attrdict3
 	combo
 	dirty-cat
 	dictlearn
 	keras
-	networkx
+	networkx<3
 	numpy<1.22,>=1.18
 	pandas
 	tqdm
 	pyod
 	python-louvain
 	PyYAML
-	scikit-learn
+	scikit-learn>1.1.3
 	scipy
 	tensorflow
 	wheel
 	wrapt-timeout-decorator
 
 [options.packages.find]
 where = .
```

### Comparing `graphomaly-0.2.7/tests/test_dl.py` & `graphomaly-0.2.8/tests/test_dl.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/tests/test_fe_time.py` & `graphomaly-0.2.8/tests/test_fe_time.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/tests/test_graphomaly_ctor.py` & `graphomaly-0.2.8/tests/test_graphomaly_ctor.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/tests/test_synthetic.py` & `graphomaly-0.2.8/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/tests/test_synthetic_gridsearch.py` & `graphomaly-0.2.8/tests/test_synthetic_gridsearch.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/tests/test_synthetic_preprocessing.py` & `graphomaly-0.2.8/tests/test_synthetic_preprocessing.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/tests/test_synthetic_voting.py` & `graphomaly-0.2.8/tests/test_synthetic_voting.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/tests/test_tf_save.py` & `graphomaly-0.2.8/tests/test_tf_save.py`

 * *Files identical despite different names*

### Comparing `graphomaly-0.2.7/tests/test_voting.py` & `graphomaly-0.2.8/tests/test_voting.py`

 * *Files identical despite different names*

