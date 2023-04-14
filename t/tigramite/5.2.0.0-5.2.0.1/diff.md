# Comparing `tmp/tigramite-5.2.0.0.tar.gz` & `tmp/tigramite-5.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigramite-5.2.0.0.tar", last modified: Fri Mar 17 21:50:07 2023, max compression
+gzip compressed data, was "tigramite-5.2.0.1.tar", last modified: Thu Apr 13 17:19:11 2023, max compression
```

## Comparing `tigramite-5.2.0.0.tar` & `tigramite-5.2.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-03-17 21:50:07.252729 tigramite-5.2.0.0/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-03-17 21:50:07.252729 tigramite-5.2.0.0/PKG-INFO
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8006 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/README.md
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       79 2023-03-17 21:50:07.252729 tigramite-5.2.0.0/setup.cfg
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3100 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/setup.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-03-17 21:50:07.244729 tigramite-5.2.0.0/tests/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     5485 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tests/test_construct_array.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    38249 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tests/test_independence_tests.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3894 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tests/test_models.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    26762 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tests/test_pcmci_calculations.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17546 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tests/test_pcmci_construction.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13375 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tests/test_var_process.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-03-17 21:50:07.248729 tigramite-5.2.0.0/tigramite/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/__init__.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   102754 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/causal_effects.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    65894 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/data_processing.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-03-17 21:50:07.252729 tigramite-5.2.0.0/tigramite/independence_tests/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    43660 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/LBFGS.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/__init__.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17887 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/cmiknn.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    10370 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/cmisymb.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    23994 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/gpdc.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    31190 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/gpdc_torch.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     6459 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/gsquared.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41968 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/independence_tests_base.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    62833 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/oracle_conditional_independence.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     9979 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/parcorr.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12267 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/parcorr_mult.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17975 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/parcorr_wls.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13647 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/regressionCI.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13402 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/independence_tests/robust_parcorr.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   170545 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/lpcmci.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    75920 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/models.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   171329 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/pcmci.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    46472 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/pcmci_base.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   158209 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/plotting.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-03-17 21:50:07.252729 tigramite-5.2.0.0/tigramite/toymodels/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/toymodels/__init__.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41858 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/toymodels/structural_causal_processes.py
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12722 2023-03-17 21:49:50.000000 tigramite-5.2.0.0/tigramite/toymodels/surrogate_generator.py
-drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-03-17 21:50:07.248729 tigramite-5.2.0.0/tigramite.egg-info/
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-03-17 21:50:07.000000 tigramite-5.2.0.0/tigramite.egg-info/PKG-INFO
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     1298 2023-03-17 21:50:07.000000 tigramite-5.2.0.0/tigramite.egg-info/SOURCES.txt
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        1 2023-03-17 21:50:07.000000 tigramite-5.2.0.0/tigramite.egg-info/dependency_links.txt
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)      402 2023-03-17 21:50:07.000000 tigramite-5.2.0.0/tigramite.egg-info/requires.txt
--rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       10 2023-03-17 21:50:07.000000 tigramite-5.2.0.0/tigramite.egg-info/top_level.txt
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-13 17:19:11.681433 tigramite-5.2.0.1/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-04-13 17:19:11.681433 tigramite-5.2.0.1/PKG-INFO
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8006 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/README.md
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       79 2023-04-13 17:19:11.685433 tigramite-5.2.0.1/setup.cfg
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3100 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/setup.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-13 17:19:11.677433 tigramite-5.2.0.1/tests/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     5485 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tests/test_construct_array.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    38249 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tests/test_independence_tests.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     3894 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tests/test_models.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    26762 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tests/test_pcmci_calculations.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17546 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tests/test_pcmci_construction.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13375 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tests/test_var_process.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-13 17:19:11.677433 tigramite-5.2.0.1/tigramite/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/__init__.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   102754 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/causal_effects.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    65894 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/data_processing.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-13 17:19:11.681433 tigramite-5.2.0.1/tigramite/independence_tests/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    43660 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/LBFGS.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/__init__.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17887 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/cmiknn.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    10370 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/cmisymb.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    23994 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/gpdc.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    31190 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/gpdc_torch.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     6459 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/gsquared.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41968 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/independence_tests_base.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    62833 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/oracle_conditional_independence.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     9979 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/parcorr.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12267 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/parcorr_mult.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    17975 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/parcorr_wls.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13647 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/regressionCI.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    13402 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/independence_tests/robust_parcorr.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   170545 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/lpcmci.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    75920 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/models.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   171329 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/pcmci.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    46472 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/pcmci_base.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)   159911 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/plotting.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-13 17:19:11.681433 tigramite-5.2.0.1/tigramite/toymodels/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/toymodels/__init__.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    41858 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/toymodels/structural_causal_processes.py
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)    12722 2023-04-13 17:18:57.000000 tigramite-5.2.0.1/tigramite/toymodels/surrogate_generator.py
+drwxrwxr-x   0 jakobrunge  (1000) jakobrunge  (1000)        0 2023-04-13 17:19:11.677433 tigramite-5.2.0.1/tigramite.egg-info/
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     8784 2023-04-13 17:19:11.000000 tigramite-5.2.0.1/tigramite.egg-info/PKG-INFO
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)     1298 2023-04-13 17:19:11.000000 tigramite-5.2.0.1/tigramite.egg-info/SOURCES.txt
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)        1 2023-04-13 17:19:11.000000 tigramite-5.2.0.1/tigramite.egg-info/dependency_links.txt
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)      402 2023-04-13 17:19:11.000000 tigramite-5.2.0.1/tigramite.egg-info/requires.txt
+-rw-rw-r--   0 jakobrunge  (1000) jakobrunge  (1000)       10 2023-04-13 17:19:11.000000 tigramite-5.2.0.1/tigramite.egg-info/top_level.txt
```

### Comparing `tigramite-5.2.0.0/PKG-INFO` & `tigramite-5.2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigramite
-Version: 5.2.0.0
+Version: 5.2.0.1
 Summary: Tigramite causal inference for time series
 Home-page: https://github.com/jakobrunge/tigramite/
 Author: Jakob Runge
 Author-email: jakob@jakob-runge.com
 License: GNU General Public License v3.0
 Keywords: causal inference,causal discovery,prediction,time series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tigramite-5.2.0.0/README.md` & `tigramite-5.2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/setup.py` & `tigramite-5.2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 # Use a custom build to handle numpy.include_dirs() when building
 CMDCLASS = {"build_ext": UseNumpyHeadersBuildExt}
 
 # Run the setup
 setup(
     name="tigramite",
-    version="5.2.0.0",
+    version="5.2.0.1",
     packages=["tigramite", "tigramite.independence_tests", "tigramite.toymodels"],
     license="GNU General Public License v3.0",
     description="Tigramite causal inference for time series",
     author="Jakob Runge",
     author_email="jakob@jakob-runge.com",
     url="https://github.com/jakobrunge/tigramite/",
     long_description=long_description,
```

### Comparing `tigramite-5.2.0.0/tests/test_construct_array.py` & `tigramite-5.2.0.1/tests/test_construct_array.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tests/test_independence_tests.py` & `tigramite-5.2.0.1/tests/test_independence_tests.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tests/test_models.py` & `tigramite-5.2.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tests/test_pcmci_calculations.py` & `tigramite-5.2.0.1/tests/test_pcmci_calculations.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tests/test_pcmci_construction.py` & `tigramite-5.2.0.1/tests/test_pcmci_construction.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tests/test_var_process.py` & `tigramite-5.2.0.1/tests/test_var_process.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/causal_effects.py` & `tigramite-5.2.0.1/tigramite/causal_effects.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/data_processing.py` & `tigramite-5.2.0.1/tigramite/data_processing.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/LBFGS.py` & `tigramite-5.2.0.1/tigramite/independence_tests/LBFGS.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/cmiknn.py` & `tigramite-5.2.0.1/tigramite/independence_tests/cmiknn.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/cmisymb.py` & `tigramite-5.2.0.1/tigramite/independence_tests/cmisymb.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/gpdc.py` & `tigramite-5.2.0.1/tigramite/independence_tests/gpdc.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/gpdc_torch.py` & `tigramite-5.2.0.1/tigramite/independence_tests/gpdc_torch.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/gsquared.py` & `tigramite-5.2.0.1/tigramite/independence_tests/gsquared.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/independence_tests_base.py` & `tigramite-5.2.0.1/tigramite/independence_tests/independence_tests_base.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/oracle_conditional_independence.py` & `tigramite-5.2.0.1/tigramite/independence_tests/oracle_conditional_independence.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/parcorr.py` & `tigramite-5.2.0.1/tigramite/independence_tests/parcorr.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/parcorr_mult.py` & `tigramite-5.2.0.1/tigramite/independence_tests/parcorr_mult.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/parcorr_wls.py` & `tigramite-5.2.0.1/tigramite/independence_tests/parcorr_wls.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/regressionCI.py` & `tigramite-5.2.0.1/tigramite/independence_tests/regressionCI.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/independence_tests/robust_parcorr.py` & `tigramite-5.2.0.1/tigramite/independence_tests/robust_parcorr.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/lpcmci.py` & `tigramite-5.2.0.1/tigramite/lpcmci.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/models.py` & `tigramite-5.2.0.1/tigramite/models.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/pcmci.py` & `tigramite-5.2.0.1/tigramite/pcmci.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/pcmci_base.py` & `tigramite-5.2.0.1/tigramite/pcmci_base.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/plotting.py` & `tigramite-5.2.0.1/tigramite/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,15 @@
             # ax.get_xaxis().get_major_formatter().set_useOffset(False)
 
             ax.xaxis.set_major_formatter(FormatStrFormatter("%.0f"))
             ax.label_outer()
 
             ax.set_xlim(time[0], time[-1])
 
-            trans = transforms.blended_transform_factory(fig.transFigure, ax.transAxes)
+            # trans = transforms.blended_transform_factory(fig.transFigure, ax.transAxes)
             if var_units[i]:
                 ax.set_ylabel(r"%s [%s]" % (var_names[i], var_units[i]), fontsize=label_fontsize)
             else:
                 ax.set_ylabel(r"%s" % (var_names[i]), fontsize=label_fontsize)
 
             ax.tick_params(axis='both', which='major', labelsize=tick_label_size)
             # ax.tick_params(axis='both', which='minor', labelsize=tick_label_size)
@@ -1507,15 +1507,15 @@
     label_fontsize=4,
     label_fraction=0.5,
     link_colorbar_label="link",
     tick_label_size=6,
     # link_edge_colorbar_label='link_edge',
     inner_edge_curved=False,
     inner_edge_style="solid",
-    network_lower_bound=0.2,
+    # network_lower_bound=0.2,
     network_left_bound=None,
     show_colorbar=True,
     special_nodes=None,
     autodep_sig_lags=None,
     show_autodependency_lags=False
 ):
     """Function to draw a network from networkx graph instance.
@@ -2160,23 +2160,32 @@
             #     ],
             #     frameon=False,
             # )
             bbox_ax = ax.get_position()
             width = bbox_ax.xmax-bbox_ax.xmin
             height = bbox_ax.ymax-bbox_ax.ymin
             # print(bbox_ax.xmin, bbox_ax.xmax, bbox_ax.ymin, bbox_ax.ymax) 
-            cax_e = fig.add_axes(
-                [
-                    bbox_ax.xmax - width*0.45,
-                    bbox_ax.ymin-0.075*height+network_lower_bound-0.15,
-                    width*0.4,
-                    0.075*height,   #0.025 + (len(all_links_edge_weights) == 0) * 0.035,
+            # cax_e = fig.add_axes(
+            #     [
+            #         bbox_ax.xmax - width*0.45,
+            #         bbox_ax.ymin-0.075*height+network_lower_bound-0.15,
+            #         width*0.4,
+            #         0.075*height,   #0.025 + (len(all_links_edge_weights) == 0) * 0.035,
+            #     ],
+            #     frameon=False,
+            # )
+            cax_e = ax.inset_axes( 
+                          [
+                          0.55, -0.07, 0.4, 0.07
+                    # bbox_ax.xmax - width*0.45,
+                    # bbox_ax.ymin-0.075*height+network_lower_bound-0.15,
+                    # width*0.4,
+                    # 0.075*height,   #0.025 + (len(all_links_edge_weights) == 0) * 0.035,
                 ],
-                frameon=False,
-            )
+                frameon=False,)
             # divider = make_axes_locatable(ax)
 
             # cax_e = divider.append_axes('bottom', size='5%', pad=0.05, frameon=False,)
 
             cb_e = pyplot.colorbar(
                 data_to_rgb_links, cax=cax_e, orientation="horizontal"
             )
@@ -2188,15 +2197,15 @@
                 )
             cb_e.set_ticks(ticks_here[(links_vmin <= ticks_here) & (ticks_here <= links_vmax)])
             # except:
             #     print('no ticks given')
 
             cb_e.outline.clear()
             cax_e.set_xlabel(
-                link_colorbar_label, labelpad=1, fontsize=label_fontsize, zorder=-10
+                link_colorbar_label, labelpad=1, fontsize=label_fontsize, zorder=10
             )
             cax_e.tick_params(axis='both', which='major', labelsize=tick_label_size)
 
     ##
     # Draw nodes
     ##
     node_sizes = np.zeros((len(node_rings), N))
@@ -2259,20 +2268,21 @@
                 # Create colorbars for nodes
                 # cax_n = pyplot.axes([.8 + ring*0.11,
                 # ax.get_subplotspec().get_position(ax.figure).bounds[1]+0.05, 0.025, 0.35], frameon=False) #
                 # setup colorbar axes.
                 # setup colorbar axes.
                 bbox_ax = ax.get_position()
                 # print(bbox_ax.xmin, bbox_ax.xmax, bbox_ax.ymin, bbox_ax.ymax) 
-                cax_n = fig.add_axes(
+                cax_n = ax.inset_axes(
                     [
-                        bbox_ax.xmin + width*0.05,
-                        bbox_ax.ymin-0.075*height+network_lower_bound-0.15,
-                        width*0.4,
-                        0.075*height,   #0.025 + (len(all_links_edge_weights) == 0) * 0.035,
+                    0.05, -0.07, 0.4, 0.07
+                        # bbox_ax.xmin + width*0.05,
+                        # bbox_ax.ymin-0.075*height+network_lower_bound-0.15,
+                        # width*0.4,
+                        # 0.075*height,   #0.025 + (len(all_links_edge_weights) == 0) * 0.035,
                     ],
                     frameon=False,
                 )
                 cb_n = pyplot.colorbar(data_to_rgb, cax=cax_n, orientation="horizontal")
                 # try:
                 ticks_here = np.arange(
                     _myround(vmin, node_rings[ring]["ticks"], "down"),
@@ -2377,19 +2387,19 @@
             d["outer_edge_alpha"] = 1e-8
         if u != v:
             if d["outer_edge"]:
                 seen[(u, v)] = draw_edge(ax, u, v, d, seen, outer_edge=True)
             if d["inner_edge"]:
                 seen[(u, v)] = draw_edge(ax, u, v, d, seen, outer_edge=False)
 
-    if network_left_bound is not None:
-        network_right_bound = 0.98
-    else:
-        network_right_bound = None
-    fig.subplots_adjust(bottom=network_lower_bound, left=network_left_bound, right=network_right_bound) #, right=0.97)
+    # if network_left_bound is not None:
+    #     network_right_bound = 0.98
+    # else:
+    #     network_right_bound = None
+    # fig.subplots_adjust(bottom=network_lower_bound, left=network_left_bound, right=network_right_bound) #, right=0.97)
 
 
 def plot_graph(
     graph,
     val_matrix=None,
     var_names=None,
     fig_ax=None,
@@ -2415,15 +2425,15 @@
     curved_radius=0.2,
     label_fontsize=10,
     tick_label_size=6,
     alpha=1.0,
     node_label_size=10,
     link_label_fontsize=10,
     lag_array=None,
-    network_lower_bound=0.2,
+    # network_lower_bound=0.2,
     show_colorbar=True,
     inner_edge_style="dashed",
     link_matrix=None,
     special_nodes=None,
     show_autodependency_lags=False
 ):
     """Creates a network plot.
@@ -2499,16 +2509,14 @@
         Fontsize of node labels.
     link_label_fontsize : int, optional (default: 6)
         Fontsize of link labels.
     tick_label_size : int, optional (default: 6)
         Fontsize of tick labels.
     lag_array : array, optional (default: None)
         Optional specification of lags overwriting np.arange(0, tau_max+1)
-    network_lower_bound : float, optional (default: 0.2)
-        Fraction of vertical space below graph plot.
     show_colorbar : bool
         Whether to show colorbars for links and nodes.
     show_autodependency_lags : bool (default: False)
         Shows significant autodependencies for a node.
     """
 
     if link_matrix is not None:
@@ -2779,15 +2787,15 @@
         # links_edges_ticks=.2, link_edge_colorbar_label='link_edge',
         arrowstyle="simple",
         arrowhead_size=arrowhead_size,
         curved_radius=curved_radius,
         label_fontsize=label_fontsize,
         link_label_fontsize=link_label_fontsize,
         link_colorbar_label=link_colorbar_label,
-        network_lower_bound=network_lower_bound,
+        # network_lower_bound=network_lower_bound,
         show_colorbar=show_colorbar,
         # label_fraction=label_fraction,
         special_nodes=special_nodes,
         autodep_sig_lags=autodep_sig_lags,
         show_autodependency_lags=show_autodependency_lags
     )
 
@@ -2975,17 +2983,14 @@
     node_size=0.1,
     node_aspect=None,
     arrowhead_size=20,
     curved_radius=0.2,
     label_fontsize=10,
     tick_label_size=6,
     alpha=1.0,
-    label_space_left=0.1,
-    label_space_top=0.0,
-    network_lower_bound=0.2,
     inner_edge_style="dashed",
     link_matrix=None,
     special_nodes=None,
     # aux_graph=None,
     standard_color_links='black',
     standard_color_nodes='lightgrey',
 ):
@@ -3042,20 +3047,14 @@
         Opacity.
     node_label_size : int, optional (default: 10)
         Fontsize of node labels.
     link_label_fontsize : int, optional (default: 6)
         Fontsize of link labels.
     tick_label_size : int, optional (default: 6)
         Fontsize of tick labels.
-    label_space_left : float, optional (default: 0.1)
-        Fraction of horizontal figure space to allocate left of plot for labels.
-    label_space_top : float, optional (default: 0.)
-        Fraction of vertical figure space to allocate top of plot for labels.
-    network_lower_bound : float, optional (default: 0.2)
-        Fraction of vertical space below graph plot.
     inner_edge_style : string, optional (default: 'dashed')
         Style of inner_edge contemporaneous links.
     special_nodes : dict
         Dictionary of format {(i, -tau): 'blue', ...} to color special nodes.
     """
 
     if link_matrix is not None:
@@ -3292,56 +3291,59 @@
         arrowhead_size=arrowhead_size,
         curved_radius=curved_radius,
         label_fontsize=label_fontsize,
         tick_label_size=tick_label_size,
         label_fraction=0.5,
         link_colorbar_label=link_colorbar_label,
         inner_edge_curved=False,
-        network_lower_bound=network_lower_bound,
-        network_left_bound=label_space_left,
+        # network_lower_bound=network_lower_bound,
+        # network_left_bound=label_space_left,
         inner_edge_style=inner_edge_style,
         special_nodes=special_nodes,
         show_colorbar=show_colorbar,
     )
 
     for i in range(N):
-        trans = transforms.blended_transform_factory(fig.transFigure, ax.transData)
+        trans = transforms.blended_transform_factory(ax.transAxes, ax.transData)
+        # trans = transforms.blended_transform_factory(fig.transFigure, ax.transData)
         ax.text(
             0.,
             pos[order[i] * max_lag][1],
             f"{var_names[order[i]]}",
             fontsize=label_fontsize,
-            horizontalalignment="left",
+            horizontalalignment="right",
             verticalalignment="center",
             transform=trans,
         )
 
     for tau in np.arange(max_lag - 1, -1, -1):
-        trans = transforms.blended_transform_factory(ax.transData, fig.transFigure)
+        trans = transforms.blended_transform_factory(ax.transData, ax.transAxes)
+        # trans = transforms.blended_transform_factory(ax.transData, fig.transFigure)
         if tau == max_lag - 1:
             ax.text(
                 pos[tau][0],
-                1.0 - label_space_top,
+                1.0, # - label_space_top,
                 r"$t$",
                 fontsize=int(label_fontsize * 0.8),
                 horizontalalignment="center",
-                verticalalignment="top",
+                verticalalignment="bottom",
                 transform=trans,
             )
         else:
             ax.text(
                 pos[tau][0],
-                1.0 - label_space_top,
+                1.0, # - label_space_top,
                 r"$t-%s$" % str(max_lag - tau - 1),
                 fontsize=int(label_fontsize * 0.8),
                 horizontalalignment="center",
-                verticalalignment="top",
+                verticalalignment="bottom",
                 transform=trans,
             )
 
+    # pyplot.tight_layout()
     if save_name is not None:
         pyplot.savefig(save_name, dpi=300)
     else:
         return fig, ax
 
 
 def plot_mediation_time_series_graph(
@@ -3368,17 +3370,14 @@
     node_aspect=None,
     arrowhead_size=20,
     curved_radius=0.2,
     label_fontsize=12,
     alpha=1.0,
     node_label_size=12,
     tick_label_size=6,
-    label_space_left=0.1,
-    label_space_top=0.0,
-    network_lower_bound=0.2,
     standard_color_links='black',
     standard_color_nodes='lightgrey',
 ):
     """Creates a mediation time series graph plot.
     This is still in beta. The time series graph's links are colored by
     val_matrix.
 
@@ -3435,20 +3434,14 @@
         Fontsize of colorbar labels.
     alpha : float, optional (default: 1.)
         Opacity.
     node_label_size : int, optional (default: 10)
         Fontsize of node labels.
     link_label_fontsize : int, optional (default: 6)
         Fontsize of link labels.
-    label_space_left : float, optional (default: 0.1)
-        Fraction of horizontal figure space to allocate left of plot for labels.
-    label_space_top : float, optional (default: 0.)
-        Fraction of vertical figure space to allocate top of plot for labels.
-    network_lower_bound : float, optional (default: 0.2)
-        Fraction of vertical space below graph plot.
     """
     N = len(path_node_array)
     Nmaxlag = tsg_path_val_matrix.shape[0]
     max_lag = Nmaxlag // N
 
     if var_names is None:
         var_names = range(N)
@@ -3609,50 +3602,52 @@
         # links_edges_ticks=.2, link_edge_colorbar_label='link_edge',
         arrowhead_size=arrowhead_size,
         curved_radius=curved_radius,
         label_fontsize=label_fontsize,
         label_fraction=0.5,
         link_colorbar_label=link_colorbar_label,
         inner_edge_curved=True,
-        network_lower_bound=network_lower_bound
+        # network_lower_bound=network_lower_bound
         # inner_edge_style=inner_edge_style
     )
 
     for i in range(N):
-        trans = transforms.blended_transform_factory(fig.transFigure, ax.transData)
+        trans = transforms.blended_transform_factory(ax.transAxes, ax.transData)
+        # trans = transforms.blended_transform_factory(fig.transFigure, ax.transData)
         ax.text(
             label_space_left,
             pos[order[i] * max_lag][1],
             "%s" % str(var_names[order[i]]),
             fontsize=label_fontsize,
-            horizontalalignment="left",
+            horizontalalignment="right",
             verticalalignment="center",
             transform=trans,
         )
 
     for tau in np.arange(max_lag - 1, -1, -1):
-        trans = transforms.blended_transform_factory(ax.transData, fig.transFigure)
+        trans = transforms.blended_transform_factory(ax.transData, ax.transAxes)
+        # trans = transforms.blended_transform_factory(ax.transData, fig.transFigure)
         if tau == max_lag - 1:
             ax.text(
                 pos[tau][0],
-                1.0 - label_space_top,
+                1.0, # - label_space_top,
                 r"$t$",
                 fontsize=label_fontsize,
                 horizontalalignment="center",
-                verticalalignment="top",
+                verticalalignment="bottom",
                 transform=trans,
             )
         else:
             ax.text(
                 pos[tau][0],
-                1.0 - label_space_top,
+                1.0, # - label_space_top,
                 r"$t-%s$" % str(max_lag - tau - 1),
                 fontsize=label_fontsize,
                 horizontalalignment="center",
-                verticalalignment="top",
+                verticalalignment="bottom",
                 transform=trans,
             )
 
     # fig.subplots_adjust(left=0.1, right=.98, bottom=.25, top=.9)
     # savestring = os.path.expanduser(save_name)
     if save_name is not None:
         pyplot.savefig(save_name)
@@ -3686,15 +3681,15 @@
     curved_radius=0.2,
     label_fontsize=10,
     tick_label_size=6,
     lag_array=None,
     alpha=1.0,
     node_label_size=10,
     link_label_fontsize=10,
-    network_lower_bound=0.2,
+    # network_lower_bound=0.2,
     standard_color_links='black',
     standard_color_nodes='lightgrey',
 ):
     """Creates a network plot visualizing the pathways of a mediation analysis.
     This is still in beta. The network is defined from non-zero entries in
     ``path_val_matrix``.  Nodes denote variables, straight links contemporaneous
     dependencies and curved arrows lagged dependencies. The node color denotes
@@ -3759,16 +3754,14 @@
         Fontsize of colorbar labels.
     alpha : float, optional (default: 1.)
         Opacity.
     node_label_size : int, optional (default: 10)
         Fontsize of node labels.
     link_label_fontsize : int, optional (default: 6)
         Fontsize of link labels.
-    network_lower_bound : float, optional (default: 0.2)
-        Fraction of vertical space below graph plot.
     lag_array : array, optional (default: None)
         Optional specification of lags overwriting np.arange(0, tau_max+1)
     """
     val_matrix = path_val_matrix
 
     if fig_ax is None:
         fig = pyplot.figure(figsize=figsize)
@@ -3942,15 +3935,15 @@
         # cmap_links_edges='YlOrRd', links_edges_vmin=-1., links_edges_vmax=1.,
         # links_edges_ticks=.2, link_edge_colorbar_label='link_edge',
         arrowhead_size=arrowhead_size,
         curved_radius=curved_radius,
         label_fontsize=label_fontsize,
         link_label_fontsize=link_label_fontsize,
         link_colorbar_label=link_colorbar_label,
-        network_lower_bound=network_lower_bound,
+        # network_lower_bound=network_lower_bound,
         # label_fraction=label_fraction,
         # inner_edge_style=inner_edge_style
     )
 
     # fig.subplots_adjust(left=0.1, right=.9, bottom=.25, top=.95)
     # savestring = os.path.expanduser(save_name)
     if save_name is not None:
@@ -4078,15 +4071,15 @@
     arrowhead_size = 20
     curved_radius = 0.2
     label_fontsize = 10
     alpha = 1.0
     node_label_size = 10
     label_space_left = 0.1
     label_space_top = 0.0
-    network_lower_bound = 0.2
+    # network_lower_bound = 0.2
     inner_edge_style = "dashed"
 
     node_color = np.ones(N * max_lag)  # , dtype = 'object')
     node_color[:] = 0
 
     if anc_x is not None:
         for n in [varlag2node(itau[0], max_lag - 1 + itau[1]) for itau in anc_x]:
@@ -4200,50 +4193,50 @@
         arrowstyle="simple",
         arrowhead_size=arrowhead_size,
         curved_radius=curved_radius,
         label_fontsize=label_fontsize,
         label_fraction=0.5,
         link_colorbar_label=link_colorbar_label,
         inner_edge_curved=True,
-        network_lower_bound=network_lower_bound,
+        # network_lower_bound=network_lower_bound,
         inner_edge_style=inner_edge_style,
     )
 
     for i in range(N):
-        trans = transforms.blended_transform_factory(fig.transFigure, ax.transData)
+        trans = transforms.blended_transform_factory(ax.transAxes, ax.transData)
         ax.text(
             label_space_left,
             pos[order[i] * max_lag][1],
             "%s" % str(var_names[order[i]]),
             fontsize=label_fontsize,
-            horizontalalignment="left",
+            horizontalalignment="right",
             verticalalignment="center",
             transform=trans,
         )
 
     for tau in np.arange(max_lag - 1, -1, -1):
-        trans = transforms.blended_transform_factory(ax.transData, fig.transFigure)
+        trans = transforms.blended_transform_factory(ax.transData, ax.transAxes)
         if tau == max_lag - 1:
             ax.text(
                 pos[tau][0],
                 1.0 - label_space_top,
                 r"$t$",
                 fontsize=int(label_fontsize * 0.7),
                 horizontalalignment="center",
-                verticalalignment="top",
+                verticalalignment="bottom",
                 transform=trans,
             )
         else:
             ax.text(
                 pos[tau][0],
                 1.0 - label_space_top,
                 r"$t-%s$" % str(max_lag - tau - 1),
                 fontsize=int(label_fontsize * 0.7),
                 horizontalalignment="center",
-                verticalalignment="top",
+                verticalalignment="bottom",
                 transform=trans,
             )
 
     return fig, ax
 
 def write_csv(
     graph,
@@ -4318,15 +4311,15 @@
         # write the header
         writer.writerow(header)
 
         # write the link data
         for (i, j, tau) in zip(*np.where(graph!='')):
             # Only consider contemporaneous links once
             if tau > 0 or i <= j:
-                row = [var_names[i], var_names[i], f"{tau}", graph[i,j,tau]]
+                row = [str(var_names[i]), str(var_names[i]), f"{tau}", graph[i,j,tau]]
                 if val_matrix_exists:
                     row.append(f"{val_matrix[i,j,tau]:.{digits}}")
                 if link_attribute is not None:
                     row.append(link_attribute[i,j,tau])
                 if link_width is not None:
                     row.append(f"{link_width[i,j,tau]:.{digits}}")
 
@@ -4414,56 +4407,109 @@
 
     # pyplot.show()
     # sys.exit(0)
 
 
     # val_matrix = np.zeros((4, 4, 3))
 
-    # # Complete test case
-    # graph = np.zeros((3,3,2), dtype='<U3')
-    # graph[:] = ""
-    # graph[0, 1, 0] = "<-+"
-    # graph[1, 0, 0] = "+->"
-
-    # graph[0, 1, 1] = "+->"
-    # graph[1, 0, 1] = "o-o"
-
-    # graph[1, 2, 0] = "<->"
-    # graph[2, 1, 0] = "<->"
-
-    # graph[0, 2, 0] = "x-x"
-    # graph[2, 0, 0] = "x-x"
-    # nolinks = np.zeros(graph.shape)
-    # # nolinks[range(4), range(4), 1] = 1
-
-    # # plot_time_series_graph(graph=nolinks)
-    # plot_graph(graph=graph, 
-    #     figsize=(5, 5),
-    #     arrow_linewidth=6,
-    #     save_name="tsg_test.pdf")
+    # Complete test case
+    graph = np.zeros((3,3,2), dtype='<U3')
+    val_matrix = np.random.rand(*graph.shape)
+    val_matrix[:,:,0] = 0.2
+    graph[:] = ""
+    graph[0, 1, 0] = "<-+"
+    graph[1, 0, 0] = "+->"
+    graph[0, 0, 1] = "-->"
+    graph[1, 1, 1] = "-->"
+
+    graph[0, 1, 1] = "+->"
+    graph[1, 0, 1] = "o-o"
+
+    graph[1, 2, 0] = "<->"
+    graph[2, 1, 0] = "<->"
+
+    graph[0, 2, 0] = "x-x"
+    graph[2, 0, 0] = "x-x"
+    nolinks = np.zeros(graph.shape)
+    # nolinks[range(4), range(4), 1] = 1
+
+    fig, axes = pyplot.subplots(nrows=2, ncols=2, figsize=(6, 5))
+    label_space_left = 0.2
+    label_space_top = 0.
+    # network_lower_bound = 0.
+    show_colorbar=True
+    # plot_graph(graph=graph,
+    #     # fig_ax = (fig, axes),
+    #     val_matrix=val_matrix,
+    #     # figsize=(5, 5),
+    #     var_names = ['Var %s' %i for i in range(len(graph))],
+    #     # arrow_linewidth=6,
+    #     # label_space_left = label_space_left,
+    #     # label_space_top = label_space_top,
+    #     # # network_lower_bound=network_lower_bound,
+    #     # save_name="tsg_test.pdf"
+    #     )
 
-    # pyplot.show()
+    # axes[0,0].scatter(np.random.rand(100), np.random.rand(100))
+
+    plot_graph(graph=graph,
+        fig_ax = (fig, axes[0,0]),
+        val_matrix=val_matrix,
+        # figsize=(5, 5),
+        var_names = ['Variable %s' %i for i in range(len(graph))],
+        arrow_linewidth=6,
+        # label_space_left = label_space_left,
+        # label_space_top = label_space_top,
+        # save_name="tsg_test.pdf"
+        )
+    plot_graph(graph=graph,
+        fig_ax = (fig, axes[0,1]),
+        val_matrix=val_matrix,
+        var_names = ['Var %s' %i for i in range(len(graph))],
+        arrow_linewidth=6,
+        # label_space_left = label_space_left,
+        # label_space_top = label_space_top,
+        )
+    plot_graph(graph=graph,
+        fig_ax = (fig, axes[1,0]),
+        val_matrix=val_matrix,
+        var_names = ['Var %s' %i for i in range(len(graph))],
+        arrow_linewidth=6,
+        # label_space_left = label_space_left,
+        # label_space_top = label_space_top,
+        )
+    plot_graph(graph=graph,
+        fig_ax = (fig, axes[1,1]),
+        val_matrix=val_matrix,
+        var_names = ['Var %s' %i for i in range(len(graph))],
+        arrow_linewidth=6,
+        # label_space_left = label_space_left,
+        # label_space_top = label_space_top,
+        )
+    # pyplot.subplots_adjust(wspace=0.3, hspace=0.2)
+    pyplot.tight_layout()
+    pyplot.savefig("test.pdf")
 
     # def lin_f(x): return x
 
-    links_coeffs = {0: [((0, -1), 0.3, lin_f)], #, ((1, -1), 0.5, lin_f)],
-                1: [((1, -1), 0.3, lin_f), ((0, 0), 0.7, lin_f), ((2, -1), 0.5, lin_f)],
-                2: [],
-                3: [((3, -1), 0., lin_f), ((2, 0), 0.6, lin_f),]
-                }
-    graph = CausalEffects.get_graph_from_dict(links_coeffs, tau_max=None)
-
-    val_matrix = np.random.randn(*graph.shape)
-    val_matrix[:,:,0] = 0.
-    write_csv(graph=graph,
-        val_matrix=val_matrix,
-        var_names=['s %d' %i for i in range(graph.shape[0])],
-        link_width=np.ones(graph.shape),
-        link_attribute = np.ones(graph.shape, dtype='<U10'),
-        save_name='test.cv')
+    # links_coeffs = {0: [((0, -1), 0.3, lin_f)], #, ((1, -1), 0.5, lin_f)],
+    #             1: [((1, -1), 0.3, lin_f), ((0, 0), 0.7, lin_f), ((2, -1), 0.5, lin_f)],
+    #             2: [],
+    #             3: [((3, -1), 0., lin_f), ((2, 0), 0.6, lin_f),]
+    #             }
+    # graph = CausalEffects.get_graph_from_dict(links_coeffs, tau_max=None)
+
+    # val_matrix = np.random.randn(*graph.shape)
+    # val_matrix[:,:,0] = 0.
+    # write_csv(graph=graph,
+    #     val_matrix=val_matrix,
+    #     var_names=[r'$X^{%d}$' %i for i in range(graph.shape[0])],
+    #     link_width=np.ones(graph.shape),
+    #     link_attribute = np.ones(graph.shape, dtype='<U10'),
+    #     save_name='test.csv')
 
     # # print(graph)
     # X = [(0,-1)]
     # Y = [(1,0)]
     # causal_effects = CausalEffects(graph, graph_type='stationary_dag', X=X, Y=Y, S=None, 
     #                                hidden_variables=[(2, 0), (2, -1), (2, -2)], 
     #                                verbosity=0)
```

### Comparing `tigramite-5.2.0.0/tigramite/toymodels/structural_causal_processes.py` & `tigramite-5.2.0.1/tigramite/toymodels/structural_causal_processes.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite/toymodels/surrogate_generator.py` & `tigramite-5.2.0.1/tigramite/toymodels/surrogate_generator.py`

 * *Files identical despite different names*

### Comparing `tigramite-5.2.0.0/tigramite.egg-info/PKG-INFO` & `tigramite-5.2.0.1/tigramite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigramite
-Version: 5.2.0.0
+Version: 5.2.0.1
 Summary: Tigramite causal inference for time series
 Home-page: https://github.com/jakobrunge/tigramite/
 Author: Jakob Runge
 Author-email: jakob@jakob-runge.com
 License: GNU General Public License v3.0
 Keywords: causal inference,causal discovery,prediction,time series
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tigramite-5.2.0.0/tigramite.egg-info/SOURCES.txt` & `tigramite-5.2.0.1/tigramite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

