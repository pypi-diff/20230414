# Comparing `tmp/hapROH-0.63.tar.gz` & `tmp/hapROH-0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hapROH-0.63.tar", last modified: Thu Jan 26 14:58:46 2023, max compression
+gzip compressed data, was "hapROH-0.64.tar", last modified: Fri Apr 14 15:28:07 2023, max compression
```

## Comparing `hapROH-0.63.tar` & `hapROH-0.64.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-01-26 14:58:46.568148 hapROH-0.63/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    68978 2021-03-02 13:08:53.000000 hapROH-0.63/LICENSE
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       20 2021-03-02 13:08:53.000000 hapROH-0.63/MANIFEST.in
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     7161 2023-01-26 14:58:46.573067 hapROH-0.63/PKG-INFO
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     5717 2023-01-26 14:52:49.000000 hapROH-0.63/README.md
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-01-26 14:58:45.913202 hapROH-0.63/hapROH.egg-info/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     7161 2023-01-26 14:58:45.864406 hapROH-0.63/hapROH.egg-info/PKG-INFO
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     1374 2023-01-26 14:58:45.878868 hapROH-0.63/hapROH.egg-info/SOURCES.txt
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        1 2023-01-26 14:58:45.889986 hapROH-0.63/hapROH.egg-info/dependency_links.txt
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       89 2023-01-26 14:58:45.898883 hapROH-0.63/hapROH.egg-info/entry_points.txt
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       68 2023-01-26 14:58:45.907248 hapROH-0.63/hapROH.egg-info/requires.txt
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        9 2023-01-26 14:58:45.917198 hapROH-0.63/hapROH.egg-info/top_level.txt
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-01-26 14:58:46.153480 hapROH-0.63/hapsburg/
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-01-26 14:58:46.168597 hapROH-0.63/hapsburg/.ipynb_checkpoints/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    30184 2023-01-26 13:18:27.000000 hapROH-0.63/hapsburg/.ipynb_checkpoints/cfunc-checkpoint.pyx
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-01-26 14:58:46.324469 hapROH-0.63/hapsburg/PackagesSupport/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:53.000000 hapROH-0.63/hapsburg/PackagesSupport/__init__.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    16943 2021-03-02 13:08:53.000000 hapROH-0.63/hapsburg/PackagesSupport/fit_ne.py
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-01-26 14:58:46.364436 hapROH-0.63/hapsburg/PackagesSupport/h5_python/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:53.000000 hapROH-0.63/hapsburg/PackagesSupport/h5_python/__init__.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    24526 2022-09-08 21:51:46.000000 hapROH-0.63/hapsburg/PackagesSupport/h5_python/h5_functions.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    40876 2023-01-26 13:24:48.000000 hapROH-0.63/hapsburg/PackagesSupport/hapsburg_run.py
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-01-26 14:58:46.433322 hapROH-0.63/hapsburg/PackagesSupport/loadEigenstrat/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:53.000000 hapROH-0.63/hapsburg/PackagesSupport/loadEigenstrat/__init__.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     8801 2021-03-02 13:08:53.000000 hapROH-0.63/hapsburg/PackagesSupport/loadEigenstrat/loadEigenstrat.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    27712 2022-11-20 14:32:22.000000 hapROH-0.63/hapsburg/PackagesSupport/loadEigenstrat/saveHDF5.py
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-01-26 14:58:46.461255 hapROH-0.63/hapsburg/PackagesSupport/parallel_runs/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/PackagesSupport/parallel_runs/__init__.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     7006 2022-02-07 11:23:47.000000 hapROH-0.63/hapsburg/PackagesSupport/parallel_runs/helper_functions.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    16837 2022-11-20 14:32:22.000000 hapROH-0.63/hapsburg/PackagesSupport/pp_individual_roh_csvs.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6352 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/PackagesSupport/roh_expectations.py
--rwxrwxr-x   0 harald_ringbauer  (2929) archgen   (2847)    15473 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/PackagesSupport/simData.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     1676 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/PackagesSupport/sqrt_scale.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/__init__.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)  1313936 2023-01-26 13:18:36.000000 hapROH-0.63/hapsburg/cfunc.c
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    30184 2023-01-26 13:18:27.000000 hapROH-0.63/hapsburg/cfunc.pyx
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    15429 2023-01-26 13:23:55.000000 hapROH-0.63/hapsburg/emissions.py
-drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-01-26 14:58:46.551839 hapROH-0.63/hapsburg/figures/
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/figures/__init__.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    15252 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/figures/plot_bars.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     8793 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/figures/plot_ibdx.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    10815 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/figures/plot_individual_roh.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    12263 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/figures/plot_posterior.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    18239 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/figures/plot_timelines.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     4240 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/func.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     4510 2022-09-07 21:05:46.000000 hapROH-0.63/hapsburg/hapCONX.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     9844 2022-11-20 14:32:22.000000 hapROH-0.63/hapsburg/hapCon_ROH.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    18457 2022-02-07 11:23:47.000000 hapROH-0.63/hapsburg/hmm_inference.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    11432 2022-02-07 11:23:47.000000 hapROH-0.63/hapsburg/postprocessing.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    41936 2022-09-07 21:05:46.000000 hapROH-0.63/hapsburg/preprocessing.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     3330 2021-03-02 13:08:54.000000 hapROH-0.63/hapsburg/transitions.py
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)      809 2023-01-26 14:58:46.584603 hapROH-0.63/setup.cfg
--rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     1054 2023-01-26 14:52:57.000000 hapROH-0.63/setup.py
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-14 15:28:07.684147 hapROH-0.64/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    68978 2021-03-02 13:08:53.000000 hapROH-0.64/LICENSE
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       20 2021-03-02 13:08:53.000000 hapROH-0.64/MANIFEST.in
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     7161 2023-04-14 15:28:07.686497 hapROH-0.64/PKG-INFO
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     5717 2023-01-26 14:52:49.000000 hapROH-0.64/README.md
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-14 15:28:07.398612 hapROH-0.64/hapROH.egg-info/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     7161 2023-04-14 15:28:07.374769 hapROH-0.64/hapROH.egg-info/PKG-INFO
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     1374 2023-04-14 15:28:07.377102 hapROH-0.64/hapROH.egg-info/SOURCES.txt
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        1 2023-04-14 15:28:07.379812 hapROH-0.64/hapROH.egg-info/dependency_links.txt
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       89 2023-04-14 15:28:07.393265 hapROH-0.64/hapROH.egg-info/entry_points.txt
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)       62 2023-04-14 15:28:07.396051 hapROH-0.64/hapROH.egg-info/requires.txt
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        9 2023-04-14 15:28:07.399429 hapROH-0.64/hapROH.egg-info/top_level.txt
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-14 15:28:07.465488 hapROH-0.64/hapsburg/
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-14 15:28:07.468960 hapROH-0.64/hapsburg/.ipynb_checkpoints/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    30184 2023-01-26 13:18:27.000000 hapROH-0.64/hapsburg/.ipynb_checkpoints/cfunc-checkpoint.pyx
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-14 15:28:07.572942 hapROH-0.64/hapsburg/PackagesSupport/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:53.000000 hapROH-0.64/hapsburg/PackagesSupport/__init__.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    17086 2023-04-14 12:52:08.000000 hapROH-0.64/hapsburg/PackagesSupport/fit_ne.py
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-14 15:28:07.587157 hapROH-0.64/hapsburg/PackagesSupport/h5_python/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:53.000000 hapROH-0.64/hapsburg/PackagesSupport/h5_python/__init__.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    24526 2022-09-08 21:51:46.000000 hapROH-0.64/hapsburg/PackagesSupport/h5_python/h5_functions.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    40876 2023-01-26 13:24:48.000000 hapROH-0.64/hapsburg/PackagesSupport/hapsburg_run.py
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-14 15:28:07.612974 hapROH-0.64/hapsburg/PackagesSupport/loadEigenstrat/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:53.000000 hapROH-0.64/hapsburg/PackagesSupport/loadEigenstrat/__init__.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     8801 2021-03-02 13:08:53.000000 hapROH-0.64/hapsburg/PackagesSupport/loadEigenstrat/loadEigenstrat.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    27712 2022-11-20 14:32:22.000000 hapROH-0.64/hapsburg/PackagesSupport/loadEigenstrat/saveHDF5.py
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-14 15:28:07.628099 hapROH-0.64/hapsburg/PackagesSupport/parallel_runs/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/PackagesSupport/parallel_runs/__init__.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     7006 2022-02-07 11:23:47.000000 hapROH-0.64/hapsburg/PackagesSupport/parallel_runs/helper_functions.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    16837 2022-11-20 14:32:22.000000 hapROH-0.64/hapsburg/PackagesSupport/pp_individual_roh_csvs.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     6352 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/PackagesSupport/roh_expectations.py
+-rwxrwxr-x   0 harald_ringbauer  (2929) archgen   (2847)    15473 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/PackagesSupport/simData.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     1676 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/PackagesSupport/sqrt_scale.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/__init__.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)  1314022 2023-04-14 15:27:04.000000 hapROH-0.64/hapsburg/cfunc.c
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    30184 2023-01-26 13:18:27.000000 hapROH-0.64/hapsburg/cfunc.pyx
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    15429 2023-01-26 13:23:55.000000 hapROH-0.64/hapsburg/emissions.py
+drwxrwsr-x   0 harald_ringbauer  (2929) archgen   (2847)        0 2023-04-14 15:28:07.678448 hapROH-0.64/hapsburg/figures/
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)        5 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/figures/__init__.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    15252 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/figures/plot_bars.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     8793 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/figures/plot_ibdx.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    10815 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/figures/plot_individual_roh.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    12263 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/figures/plot_posterior.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    18239 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/figures/plot_timelines.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     4240 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/func.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     4510 2022-09-07 21:05:46.000000 hapROH-0.64/hapsburg/hapCONX.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     9844 2022-11-20 14:32:22.000000 hapROH-0.64/hapsburg/hapCon_ROH.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    18457 2022-02-07 11:23:47.000000 hapROH-0.64/hapsburg/hmm_inference.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    11432 2022-02-07 11:23:47.000000 hapROH-0.64/hapsburg/postprocessing.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)    41936 2022-09-07 21:05:46.000000 hapROH-0.64/hapsburg/preprocessing.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     3330 2021-03-02 13:08:54.000000 hapROH-0.64/hapsburg/transitions.py
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)      809 2023-04-14 15:28:07.692512 hapROH-0.64/setup.cfg
+-rw-rw-r--   0 harald_ringbauer  (2929) archgen   (2847)     1054 2023-04-14 15:26:30.000000 hapROH-0.64/setup.py
```

### Comparing `hapROH-0.63/LICENSE` & `hapROH-0.64/LICENSE`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/PKG-INFO` & `hapROH-0.64/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapROH
-Version: 0.63
+Version: 0.64
 Summary: Identify runs of homozygosity (hapROH) and contamination (hapCon) in low coverage ancient human DNA data (1240K SNPs) using modern reference panel
 Home-page: https://github.com/hringbauer/hapROH
 Author: Harald Ringbauer
 Author-email: harald_ringbauer@eva.mpg.de
 License: GNU GPLv3
 Description: # hapROH & hapCon
         This Python package contains two softwares for ancient DNA, ***hapROH*** and ***hapCon***.
```

### Comparing `hapROH-0.63/README.md` & `hapROH-0.64/README.md`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapROH.egg-info/PKG-INFO` & `hapROH-0.64/hapROH.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapROH
-Version: 0.63
+Version: 0.64
 Summary: Identify runs of homozygosity (hapROH) and contamination (hapCon) in low coverage ancient human DNA data (1240K SNPs) using modern reference panel
 Home-page: https://github.com/hringbauer/hapROH
 Author: Harald Ringbauer
 Author-email: harald_ringbauer@eva.mpg.de
 License: GNU GPLv3
 Description: # hapROH & hapCon
         This Python package contains two softwares for ancient DNA, ***hapROH*** and ***hapCon***.
```

### Comparing `hapROH-0.63/hapROH.egg-info/SOURCES.txt` & `hapROH-0.64/hapROH.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/.ipynb_checkpoints/cfunc-checkpoint.pyx` & `hapROH-0.64/hapsburg/.ipynb_checkpoints/cfunc-checkpoint.pyx`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/PackagesSupport/fit_ne.py` & `hapROH-0.64/hapsburg/PackagesSupport/fit_ne.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,14 +350,16 @@
 ### Helper Functions related to Ne estimation.
 
 def load_roh_vec(iids=[], base_path = "./output/roh/", suffix="_roh_full.csv"):
     """Load and return ROH length vector """
     paths = give_iid_paths(iids, base_folder=base_path, suffix=suffix)
     roh_dfs = [pd.read_csv(p) for p in paths]
     roh_vec = [df["lengthM"].values*100 for df in roh_dfs]
+    ### Transform to np.array of np.array - to avoid errors downstream:
+    roh_vec = np.array([np.array(l) for l in roh_vec], dtype="object")
     return roh_vec
 
 def get_default_res():
     """REturn default line of results dataframe.
     Used for unfittable scenarios"""
     dct= {"coef":[np.nan],
           "std err":[np.nan],
```

### Comparing `hapROH-0.63/hapsburg/PackagesSupport/h5_python/h5_functions.py` & `hapROH-0.64/hapsburg/PackagesSupport/h5_python/h5_functions.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/PackagesSupport/hapsburg_run.py` & `hapROH-0.64/hapsburg/PackagesSupport/hapsburg_run.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/PackagesSupport/loadEigenstrat/loadEigenstrat.py` & `hapROH-0.64/hapsburg/PackagesSupport/loadEigenstrat/loadEigenstrat.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/PackagesSupport/loadEigenstrat/saveHDF5.py` & `hapROH-0.64/hapsburg/PackagesSupport/loadEigenstrat/saveHDF5.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/PackagesSupport/parallel_runs/helper_functions.py` & `hapROH-0.64/hapsburg/PackagesSupport/parallel_runs/helper_functions.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/PackagesSupport/pp_individual_roh_csvs.py` & `hapROH-0.64/hapsburg/PackagesSupport/pp_individual_roh_csvs.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/PackagesSupport/roh_expectations.py` & `hapROH-0.64/hapsburg/PackagesSupport/roh_expectations.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/PackagesSupport/simData.py` & `hapROH-0.64/hapsburg/PackagesSupport/simData.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/PackagesSupport/sqrt_scale.py` & `hapROH-0.64/hapsburg/PackagesSupport/sqrt_scale.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/cfunc.c` & `hapROH-0.64/hapsburg/cfunc.c`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "hapsburg.cfunc",
         "sources": [
-            "/mnt/archgen/users/hringbauer/git/hapROH/package/hapsburg/cfunc.pyx"
+            "hapsburg/cfunc.pyx"
         ]
     },
     "module_name": "hapsburg.cfunc"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -965,15 +965,15 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "cfunc.pyx",
+  "hapsburg/cfunc.pyx",
   "stringsource",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
   struct __pyx_memoryview_obj *memview;
   char *data;
@@ -2120,15 +2120,14 @@
 static const char __pyx_k_n_states[] = "n_states";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_three_vi[] = "three_vi";
 static const char __pyx_k_trans_ll[] = "trans_ll";
 static const char __pyx_k_DTYPE_INT[] = "DTYPE_INT";
 static const char __pyx_k_TypeError[] = "TypeError";
-static const char __pyx_k_cfunc_pyx[] = "cfunc.pyx";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_post_view[] = "post_view";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_trans_ll1[] = "trans_ll1";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
@@ -2157,14 +2156,15 @@
 static const char __pyx_k_fwd_bkwd_lowmem[] = "fwd_bkwd_lowmem";
 static const char __pyx_k_fwd_bkwd_scaled[] = "fwd_bkwd_scaled";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_Memory_Usage_Full[] = "Memory Usage Full:";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_hapsburg_cfunc_pyx[] = "hapsburg/cfunc.pyx";
 static const char __pyx_k_print_memory_usage[] = "print_memory_usage";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
 static const char __pyx_k_Log_likelihood_Path[] = "Log likelihood Path: ";
 static const char __pyx_k_Total_Log_likelihood[] = "Total Log likelihood: ";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
@@ -2229,15 +2229,14 @@
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_bwd;
 static PyObject *__pyx_n_s_bwd0;
 static PyObject *__pyx_n_s_bwd1;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_c_view;
-static PyObject *__pyx_kp_s_cfunc_pyx;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_is_object;
@@ -2266,14 +2265,15 @@
 static PyObject *__pyx_n_s_fwd_bkwd_lowmem;
 static PyObject *__pyx_n_s_fwd_bkwd_scaled;
 static PyObject *__pyx_n_s_fwd_bkwd_scaled_lowmem;
 static PyObject *__pyx_n_s_getpid;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
 static PyObject *__pyx_n_s_hapsburg_cfunc;
+static PyObject *__pyx_kp_s_hapsburg_cfunc_pyx;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_in_val;
 static PyObject *__pyx_n_s_int16;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
@@ -27561,15 +27561,14 @@
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_bwd, __pyx_k_bwd, sizeof(__pyx_k_bwd), 0, 0, 1, 1},
   {&__pyx_n_s_bwd0, __pyx_k_bwd0, sizeof(__pyx_k_bwd0), 0, 0, 1, 1},
   {&__pyx_n_s_bwd1, __pyx_k_bwd1, sizeof(__pyx_k_bwd1), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_c_view, __pyx_k_c_view, sizeof(__pyx_k_c_view), 0, 0, 1, 1},
-  {&__pyx_kp_s_cfunc_pyx, __pyx_k_cfunc_pyx, sizeof(__pyx_k_cfunc_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
@@ -27598,14 +27597,15 @@
   {&__pyx_n_s_fwd_bkwd_lowmem, __pyx_k_fwd_bkwd_lowmem, sizeof(__pyx_k_fwd_bkwd_lowmem), 0, 0, 1, 1},
   {&__pyx_n_s_fwd_bkwd_scaled, __pyx_k_fwd_bkwd_scaled, sizeof(__pyx_k_fwd_bkwd_scaled), 0, 0, 1, 1},
   {&__pyx_n_s_fwd_bkwd_scaled_lowmem, __pyx_k_fwd_bkwd_scaled_lowmem, sizeof(__pyx_k_fwd_bkwd_scaled_lowmem), 0, 0, 1, 1},
   {&__pyx_n_s_getpid, __pyx_k_getpid, sizeof(__pyx_k_getpid), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
   {&__pyx_n_s_hapsburg_cfunc, __pyx_k_hapsburg_cfunc, sizeof(__pyx_k_hapsburg_cfunc), 0, 0, 1, 1},
+  {&__pyx_kp_s_hapsburg_cfunc_pyx, __pyx_k_hapsburg_cfunc_pyx, sizeof(__pyx_k_hapsburg_cfunc_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_in_val, __pyx_k_in_val, sizeof(__pyx_k_in_val), 0, 0, 1, 1},
   {&__pyx_n_s_int16, __pyx_k_int16, sizeof(__pyx_k_int16), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
@@ -28020,99 +28020,99 @@
  * def print_memory_usage():             # <<<<<<<<<<<<<<
  *     """Print the current Memory Usage in mB"""
  *     process = psutil.Process(os.getpid())
  */
   __pyx_tuple__29 = PyTuple_Pack(2, __pyx_n_s_process, __pyx_n_s_mb_usage); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_print_memory_usage, 49, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hapsburg_cfunc_pyx, __pyx_n_s_print_memory_usage, 49, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 49, __pyx_L1_error)
 
   /* "hapsburg/cfunc.pyx":58
  * #### The main functions
  * 
  * def fwd_bkwd_fast(double[:, :] e_mat, double[:, :, :] t_mat,             # <<<<<<<<<<<<<<
  *                   double in_val = 1e-4, full=False, output=True):
  *     """Takes emission and transition probabilities, and calculates posteriors.
  */
   __pyx_tuple__31 = PyTuple_Pack(30, __pyx_n_s_e_mat, __pyx_n_s_t_mat, __pyx_n_s_in_val, __pyx_n_s_full, __pyx_n_s_output, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_stay, __pyx_n_s_post, __pyx_n_s_trans_ll, __pyx_n_s_trans_ll_view, __pyx_n_s_trans_ll1, __pyx_n_s_trans_ll_view1, __pyx_n_s_three_v, __pyx_n_s_three_v_view, __pyx_n_s_two_v, __pyx_n_s_two_v_view, __pyx_n_s_t0, __pyx_n_s_e_mat0, __pyx_n_s_fwd0, __pyx_n_s_fwd, __pyx_n_s_bwd0, __pyx_n_s_bwd, __pyx_n_s_f_l, __pyx_n_s_tot_ll, __pyx_n_s_fwd1, __pyx_n_s_bwd1); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__31);
   __Pyx_GIVEREF(__pyx_tuple__31);
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(5, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_fwd_bkwd_fast, 58, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(5, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hapsburg_cfunc_pyx, __pyx_n_s_fwd_bkwd_fast, 58, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 58, __pyx_L1_error)
 
   /* "hapsburg/cfunc.pyx":175
  * 
  * 
  * def fwd_bkwd_lowmem(double[:, :] e_mat, double[:, :, :] t_mat,             # <<<<<<<<<<<<<<
  *                     double in_val = 1e-4, full=False, output=True):
  *     """Takes emission and transition probabilities, and calculates posteriors.
  */
   __pyx_tuple__33 = PyTuple_Pack(31, __pyx_n_s_e_mat, __pyx_n_s_t_mat, __pyx_n_s_in_val, __pyx_n_s_full, __pyx_n_s_output, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_stay, __pyx_n_s_tot_ll, __pyx_n_s_t0, __pyx_n_s_e_mat0, __pyx_n_s_post, __pyx_n_s_post_view, __pyx_n_s_trans_ll, __pyx_n_s_trans_ll_view, __pyx_n_s_trans_ll1, __pyx_n_s_trans_ll_view1, __pyx_n_s_three_v, __pyx_n_s_three_v_view, __pyx_n_s_two_v, __pyx_n_s_two_v_view, __pyx_n_s_fwd0, __pyx_n_s_fwd, __pyx_n_s_bwd0, __pyx_n_s_bwd, __pyx_n_s_tmp0, __pyx_n_s_tmp, __pyx_n_s_f_l); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(5, 0, 31, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_fwd_bkwd_lowmem, 175, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(5, 0, 31, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hapsburg_cfunc_pyx, __pyx_n_s_fwd_bkwd_lowmem, 175, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 175, __pyx_L1_error)
 
   /* "hapsburg/cfunc.pyx":314
  * 
  * 
  * def fwd_bkwd_scaled(double[:, :] e_mat, double[:, :, :] t_mat,             # <<<<<<<<<<<<<<
  *                     double in_val = 1e-4, full=False, output=True):
  *     """
  */
   __pyx_tuple__35 = PyTuple_Pack(28, __pyx_n_s_e_mat, __pyx_n_s_t_mat, __pyx_n_s_in_val, __pyx_n_s_full, __pyx_n_s_output, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_stay, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_x3, __pyx_n_s_post, __pyx_n_s_c, __pyx_n_s_c_view, __pyx_n_s_temp, __pyx_n_s_temp_v, __pyx_n_s_temp1, __pyx_n_s_temp1_v, __pyx_n_s_t, __pyx_n_s_fwd1, __pyx_n_s_fwd, __pyx_n_s_bwd1, __pyx_n_s_bwd, __pyx_n_s_f_l, __pyx_n_s_tot_ll); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(5, 0, 28, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_fwd_bkwd_scaled, 314, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 314, __pyx_L1_error)
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(5, 0, 28, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hapsburg_cfunc_pyx, __pyx_n_s_fwd_bkwd_scaled, 314, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 314, __pyx_L1_error)
 
   /* "hapsburg/cfunc.pyx":434
  * 
  * 
  * def fwd_bkwd_scaled_lowmem(double[:, :] e_mat, double[:, :, :] t_mat,             # <<<<<<<<<<<<<<
  *                            double in_val = 1e-4, full=False, output=True):
  *     """
  */
   __pyx_tuple__37 = PyTuple_Pack(31, __pyx_n_s_e_mat, __pyx_n_s_t_mat, __pyx_n_s_in_val, __pyx_n_s_full, __pyx_n_s_output, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_stay, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_x3, __pyx_n_s_post, __pyx_n_s_post_view, __pyx_n_s_temp, __pyx_n_s_temp_v, __pyx_n_s_temp1, __pyx_n_s_temp1_v, __pyx_n_s_t, __pyx_n_s_c, __pyx_n_s_c_view, __pyx_n_s_fwd0, __pyx_n_s_fwd, __pyx_n_s_bwd0, __pyx_n_s_bwd, __pyx_n_s_tmp0, __pyx_n_s_tmp, __pyx_n_s_f_l, __pyx_n_s_tot_ll); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
-  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(5, 0, 31, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_fwd_bkwd_scaled_lowmem, 434, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 434, __pyx_L1_error)
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(5, 0, 31, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hapsburg_cfunc_pyx, __pyx_n_s_fwd_bkwd_scaled_lowmem, 434, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 434, __pyx_L1_error)
 
   /* "hapsburg/cfunc.pyx":567
  * ######################### Yilei  ##############################
  * # returns total loglikelihood, copied from fwd_bkwd_scaled_lowmem but without the backward iteration
  * def fwd(double[:, :] e_mat, double[:, :, :] t_mat, double in_val = 1e-4):             # <<<<<<<<<<<<<<
  *     cdef int n_states = e_mat.shape[0]
  *     cdef int n_loci = e_mat.shape[1]
  */
   __pyx_tuple__39 = PyTuple_Pack(25, __pyx_n_s_e_mat, __pyx_n_s_t_mat, __pyx_n_s_in_val, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_stay, __pyx_n_s_x1, __pyx_n_s_x2, __pyx_n_s_x3, __pyx_n_s_temp, __pyx_n_s_temp_v, __pyx_n_s_temp1, __pyx_n_s_temp1_v, __pyx_n_s_t, __pyx_n_s_c, __pyx_n_s_c_view, __pyx_n_s_fwd0, __pyx_n_s_fwd, __pyx_n_s_tmp0, __pyx_n_s_tmp, __pyx_n_s_f_l, __pyx_n_s_tot_ll); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__39);
   __Pyx_GIVEREF(__pyx_tuple__39);
-  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_fwd, 567, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 567, __pyx_L1_error)
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hapsburg_cfunc_pyx, __pyx_n_s_fwd, 567, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 567, __pyx_L1_error)
 
   /* "hapsburg/cfunc.pyx":639
  * #### LEGACY FUNCTIONS [NOT INT PRODUCTION ANYMORE]
  * 
  * def fwd_bkwd(double[:, :] e_prob0, double[:, :] t_mat,             # <<<<<<<<<<<<<<
  *     double[:, :] fwd, double[:, :] bwd, double[:,:,:] t, full=False):
  *     """Takes emission and transition probabilities, and calculates posteriors.
  */
   __pyx_tuple__41 = PyTuple_Pack(18, __pyx_n_s_e_prob0, __pyx_n_s_t_mat, __pyx_n_s_fwd, __pyx_n_s_bwd, __pyx_n_s_t, __pyx_n_s_full, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_post, __pyx_n_s_trans_ll, __pyx_n_s_trans_ll_view, __pyx_n_s_t_mat0, __pyx_n_s_tot_ll, __pyx_n_s_fwd1, __pyx_n_s_bwd1); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 639, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(6, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_fwd_bkwd, 639, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 639, __pyx_L1_error)
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(6, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hapsburg_cfunc_pyx, __pyx_n_s_fwd_bkwd, 639, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 639, __pyx_L1_error)
 
   /* "hapsburg/cfunc.pyx":691
  * 
  * 
  * def viterbi_path(double[:, :] e_prob0, double[:, :, :] t_mat0, double[:] end_p0):             # <<<<<<<<<<<<<<
  *     """Implementation of a Viterbi Path.
  *     e_prob0  Matrices with Emission Probabilities, [k,l] (log space)
  */
   __pyx_tuple__43 = PyTuple_Pack(25, __pyx_n_s_e_prob0, __pyx_n_s_t_mat0, __pyx_n_s_end_p0, __pyx_n_s_n_states, __pyx_n_s_n_loci, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_m, __pyx_n_s_v, __pyx_n_s_mp, __pyx_n_s_new_p, __pyx_n_s_pt, __pyx_n_s_trans_ll, __pyx_n_s_trans_ll_view, __pyx_n_s_three_v, __pyx_n_s_three_v_view, __pyx_n_s_three_vi, __pyx_n_s_three_vi_view, __pyx_n_s_two_v, __pyx_n_s_two_v_view, __pyx_n_s_two_vi, __pyx_n_s_two_vi_view, __pyx_n_s_path, __pyx_n_s_x); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 691, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(3, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cfunc_pyx, __pyx_n_s_viterbi_path, 691, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 691, __pyx_L1_error)
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(3, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hapsburg_cfunc_pyx, __pyx_n_s_viterbi_path, 691, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 691, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
```

### Comparing `hapROH-0.63/hapsburg/cfunc.pyx` & `hapROH-0.64/hapsburg/cfunc.pyx`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/emissions.py` & `hapROH-0.64/hapsburg/emissions.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/figures/plot_bars.py` & `hapROH-0.64/hapsburg/figures/plot_bars.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/figures/plot_ibdx.py` & `hapROH-0.64/hapsburg/figures/plot_ibdx.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/figures/plot_individual_roh.py` & `hapROH-0.64/hapsburg/figures/plot_individual_roh.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/figures/plot_posterior.py` & `hapROH-0.64/hapsburg/figures/plot_posterior.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/figures/plot_timelines.py` & `hapROH-0.64/hapsburg/figures/plot_timelines.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/func.py` & `hapROH-0.64/hapsburg/func.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/hapCONX.py` & `hapROH-0.64/hapsburg/hapCONX.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/hapCon_ROH.py` & `hapROH-0.64/hapsburg/hapCon_ROH.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/hmm_inference.py` & `hapROH-0.64/hapsburg/hmm_inference.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/postprocessing.py` & `hapROH-0.64/hapsburg/postprocessing.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/preprocessing.py` & `hapROH-0.64/hapsburg/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/hapsburg/transitions.py` & `hapROH-0.64/hapsburg/transitions.py`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/setup.cfg` & `hapROH-0.64/setup.cfg`

 * *Files identical despite different names*

### Comparing `hapROH-0.63/setup.py` & `hapROH-0.64/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     extensions = cythonize(extensions)
   
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="hapROH",
-    version="0.63",  # a would mean alpha, for example 0.3a4
+    version="0.64",  # a would mean alpha, for example 0.3a4
     packages=find_packages(),
     ext_modules=extensions,
     python_requires='>=3.6',
-    install_requires=['numpy', 'pandas', 'scipy', 'h5py', 'psutil', 'numdifftools', 'cython', 'matplotlib', 'pysam'],
+    install_requires=['numpy', 'pandas', 'scipy', 'h5py', 'psutil', 'numdifftools', 'cython', 'matplotlib'], #'pysam'
     entry_points ={
             'console_scripts': [
                 'hapConX = hapsburg.hapCONX:main',
                 'hapCon_ROH = hapsburg.hapCon_ROH:main'
             ]
         },
 )
```

