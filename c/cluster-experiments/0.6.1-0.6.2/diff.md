# Comparing `tmp/cluster_experiments-0.6.1.tar.gz` & `tmp/cluster_experiments-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_experiments-0.6.1.tar", last modified: Wed Apr 12 09:19:36 2023, max compression
+gzip compressed data, was "dist/cluster_experiments-0.6.2.tar", last modified: Fri Apr 14 13:10:47 2023, max compression
```

## Comparing `cluster_experiments-0.6.1.tar` & `cluster_experiments-0.6.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.739387 cluster_experiments-0.6.1/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.1/LICENSE
--rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.1/MANIFEST.in
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-12 09:19:36.738271 cluster_experiments-0.6.1/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-04-05 14:50:51.000000 cluster_experiments-0.6.1/README.md
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.647365 cluster_experiments-0.6.1/cluster_experiments/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.6.1/cluster_experiments/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     7301 2022-12-19 15:58:12.000000 cluster_experiments-0.6.1/cluster_experiments/cupac.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17228 2023-03-01 11:45:41.000000 cluster_experiments-0.6.1/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5032 2023-03-01 11:31:23.000000 cluster_experiments-0.6.1/cluster_experiments/perturbator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    19384 2023-04-12 09:19:03.000000 cluster_experiments-0.6.1/cluster_experiments/power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.1/cluster_experiments/power_config.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17759 2023-04-12 08:53:42.000000 cluster_experiments-0.6.1/cluster_experiments/random_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.1/cluster_experiments/utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.6.1/cluster_experiments/washover.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.655499 cluster_experiments-0.6.1/cluster_experiments.egg-info/
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-12 09:19:36.000000 cluster_experiments-0.6.1/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     1447 2023-04-12 09:19:36.000000 cluster_experiments-0.6.1/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-04-12 09:19:36.000000 cluster_experiments-0.6.1/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)     1071 2023-04-12 09:19:36.000000 cluster_experiments-0.6.1/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-04-12 09:19:36.000000 cluster_experiments-0.6.1/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-04-12 09:19:36.739717 cluster_experiments-0.6.1/setup.cfg
--rw-r--r--   0 davidmasip   (502) staff       (20)     1133 2023-04-12 09:19:03.000000 cluster_experiments-0.6.1/setup.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.668180 cluster_experiments-0.6.1/tests/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.1/tests/__init__.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.674312 cluster_experiments-0.6.1/tests/analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.1/tests/analysis/test_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      488 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.680215 cluster_experiments-0.6.1/tests/cupac/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/cupac/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/cupac/test_aggregator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2141 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.1/tests/examples.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.683447 cluster_experiments-0.6.1/tests/perturbator/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/perturbator/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2317 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.700360 cluster_experiments-0.6.1/tests/power_analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/power_analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.1/tests/power_analysis/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.6.1/tests/power_analysis/test_parallel.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5239 2023-04-12 09:19:03.000000 cluster_experiments-0.6.1/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.1/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-04-07 10:35:06.000000 cluster_experiments-0.6.1/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-12 09:19:36.736675 cluster_experiments-0.6.1/tests/splitter/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/splitter/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5743 2023-04-05 14:50:51.000000 cluster_experiments-0.6.1/tests/splitter/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.1/tests/splitter/test_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.1/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.1/tests/splitter/test_time_col.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.6.1/tests/splitter/test_washover.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.6.1/tests/test_docs.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.1/tests/test_non_clustered.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.1/tests/test_utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1324 2022-10-21 09:42:28.000000 cluster_experiments-0.6.1/tests/utils.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.810590 cluster_experiments-0.6.2/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.6.2/LICENSE
+-rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.6.2/MANIFEST.in
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-14 13:10:47.809940 cluster_experiments-0.6.2/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7140 2023-04-05 14:50:51.000000 cluster_experiments-0.6.2/README.md
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.769650 cluster_experiments-0.6.2/cluster_experiments/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.6.2/cluster_experiments/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.6.2/cluster_experiments/cupac.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17228 2023-03-01 11:45:41.000000 cluster_experiments-0.6.2/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5032 2023-03-01 11:31:23.000000 cluster_experiments-0.6.2/cluster_experiments/perturbator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    19384 2023-04-14 12:56:48.000000 cluster_experiments-0.6.2/cluster_experiments/power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-02-10 16:31:12.000000 cluster_experiments-0.6.2/cluster_experiments/power_config.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17759 2023-04-12 08:53:42.000000 cluster_experiments-0.6.2/cluster_experiments/random_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.6.2/cluster_experiments/utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.6.2/cluster_experiments/washover.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.775126 cluster_experiments-0.6.2/cluster_experiments.egg-info/
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-04-14 13:10:47.000000 cluster_experiments-0.6.2/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1447 2023-04-14 13:10:47.000000 cluster_experiments-0.6.2/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-04-14 13:10:47.000000 cluster_experiments-0.6.2/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1071 2023-04-14 13:10:47.000000 cluster_experiments-0.6.2/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-04-14 13:10:47.000000 cluster_experiments-0.6.2/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-04-14 13:10:47.810785 cluster_experiments-0.6.2/setup.cfg
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1133 2023-04-14 13:06:22.000000 cluster_experiments-0.6.2/setup.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.780835 cluster_experiments-0.6.2/tests/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.6.2/tests/__init__.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.786200 cluster_experiments-0.6.2/tests/analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.6.2/tests/analysis/test_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      488 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.790848 cluster_experiments-0.6.2/tests/cupac/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/cupac/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/cupac/test_aggregator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 13:06:22.000000 cluster_experiments-0.6.2/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2234 2023-02-08 15:47:52.000000 cluster_experiments-0.6.2/tests/examples.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.792850 cluster_experiments-0.6.2/tests/perturbator/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/perturbator/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2317 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.801560 cluster_experiments-0.6.2/tests/power_analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/power_analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3164 2023-02-10 16:31:12.000000 cluster_experiments-0.6.2/tests/power_analysis/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.6.2/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5239 2023-04-12 09:19:03.000000 cluster_experiments-0.6.2/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.6.2/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3109 2023-04-07 10:35:06.000000 cluster_experiments-0.6.2/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-04-14 13:10:47.808841 cluster_experiments-0.6.2/tests/splitter/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/splitter/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5743 2023-04-05 14:50:51.000000 cluster_experiments-0.6.2/tests/splitter/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.6.2/tests/splitter/test_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.6.2/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.6.2/tests/splitter/test_time_col.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.6.2/tests/splitter/test_washover.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.6.2/tests/test_docs.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.6.2/tests/test_non_clustered.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.6.2/tests/test_utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1324 2022-10-21 09:42:28.000000 cluster_experiments-0.6.2/tests/utils.py
```

### Comparing `cluster_experiments-0.6.1/LICENSE` & `cluster_experiments-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/README.md` & `cluster_experiments-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/cluster_experiments/__init__.py` & `cluster_experiments-0.6.2/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/cluster_experiments/cupac.py` & `cluster_experiments-0.6.2/cluster_experiments/cupac.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,7 +184,13 @@
 
     def need_covariates(self, pre_experiment_df: Optional[pd.DataFrame] = None) -> bool:
         return pre_experiment_df is not None and self.is_cupac
 
     def check_cupac_inputs(self, pre_experiment_df: Optional[pd.DataFrame] = None):
         if self.is_cupac and pre_experiment_df is None:
             raise ValueError("If cupac is used, pre_experiment_df should be provided.")
+
+        if not self.is_cupac and pre_experiment_df is not None:
+            raise ValueError(
+                "If cupac is not used, pre_experiment_df should not be provided - "
+                "remove pre_experiment_df argument or set cupac_model to not None."
+            )
```

### Comparing `cluster_experiments-0.6.1/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.6.2/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/cluster_experiments/perturbator.py` & `cluster_experiments-0.6.2/cluster_experiments/perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/cluster_experiments/power_analysis.py` & `cluster_experiments-0.6.2/cluster_experiments/power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/cluster_experiments/power_config.py` & `cluster_experiments-0.6.2/cluster_experiments/power_config.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/cluster_experiments/random_splitter.py` & `cluster_experiments-0.6.2/cluster_experiments/random_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/cluster_experiments/washover.py` & `cluster_experiments-0.6.2/cluster_experiments/washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.6.2/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.6.2/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/setup.py` & `cluster_experiments-0.6.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "mkdocs-jupyter==0.22.0",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.6.1",
+    version="0.6.2",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.6.1/tests/analysis/test_analysis.py` & `cluster_experiments-0.6.2/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/cupac/test_aggregator.py` & `cluster_experiments-0.6.2/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.6.2/tests/cupac/test_cupac_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -77,14 +77,22 @@
     df = cupac_handler.add_covariates(df_feats, df_feats.head(10))
     assert df["estimate_target"].isna().sum() == 0
     assert (df["estimate_target"] <= df["target"].max()).all()
     assert (df["estimate_target"] >= df["target"].min()).all()
 
 
 def test_no_target(missing_cupac, df_feats):
-    df = missing_cupac.add_covariates(df_feats, df_feats.head(10))
+    """Checks that no target is added when the there is no cupac model"""
+    df = missing_cupac.add_covariates(df_feats)
     assert "estimate_target" not in df.columns
 
 
 def test_no_pre_experiment(cupac_handler_base, df_feats):
-    with pytest.raises(ValueError):
+    """Checks that if there is a cupac model, pre_experiment_df should be provided"""
+    with pytest.raises(ValueError, match="pre_experiment_df should be provided"):
         cupac_handler_base.add_covariates(df_feats)
+
+
+def test_no_cupac(missing_cupac, df_feats):
+    """Checks that if there is no cupac model, pre_experiment_df should not be provided"""
+    with pytest.raises(ValueError, match="remove pre_experiment_df argument"):
+        missing_cupac.add_covariates(df_feats, df_feats.head(10))
```

### Comparing `cluster_experiments-0.6.1/tests/examples.py` & `cluster_experiments-0.6.2/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.6.2/tests/perturbator/test_perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/power_analysis/conftest.py` & `cluster_experiments-0.6.2/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.6.2/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.6.2/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.6.2/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.6.2/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.6.2/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.6.2/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/splitter/conftest.py` & `cluster_experiments-0.6.2/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/splitter/test_splitter.py` & `cluster_experiments-0.6.2/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.6.2/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/splitter/test_time_col.py` & `cluster_experiments-0.6.2/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/splitter/test_washover.py` & `cluster_experiments-0.6.2/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/test_docs.py` & `cluster_experiments-0.6.2/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/test_non_clustered.py` & `cluster_experiments-0.6.2/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.6.1/tests/utils.py` & `cluster_experiments-0.6.2/tests/utils.py`

 * *Files identical despite different names*

