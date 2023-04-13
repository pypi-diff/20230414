# Comparing `tmp/NREL-sup3r-0.0.9.tar.gz` & `tmp/NREL-sup3r-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NREL-sup3r-0.0.9.tar", last modified: Fri Jan 20 16:39:19 2023, max compression
+gzip compressed data, was "NREL-sup3r-0.1.0.tar", last modified: Thu Apr 13 22:50:37 2023, max compression
```

## Comparing `NREL-sup3r-0.0.9.tar` & `NREL-sup3r-0.1.0.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.439031 NREL-sup3r-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.431031 NREL-sup3r-0.0.9/NREL_sup3r.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-01-20 16:39:19.000000 NREL-sup3r-0.0.9/NREL_sup3r.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-01-20 16:39:19.000000 NREL-sup3r-0.0.9/NREL_sup3r.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 16:39:19.000000 NREL-sup3r-0.0.9/NREL_sup3r.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-01-20 16:39:19.000000 NREL-sup3r-0.0.9/NREL_sup3r.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 16:39:19.000000 NREL-sup3r-0.0.9/NREL_sup3r.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-20 16:39:19.000000 NREL-sup3r-0.0.9/NREL_sup3r.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-20 16:39:19.000000 NREL-sup3r-0.0.9/NREL_sup3r.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-01-20 16:39:19.439031 NREL-sup3r-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 16:39:19.439031 NREL-sup3r-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.431031 NREL-sup3r-0.0.9/sup3r/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.431031 NREL-sup3r-0.0.9/sup3r/batch/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/batch/batch_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.431031 NREL-sup3r-0.0.9/sup3r/bias/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/bias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31861 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/bias/bias_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/bias/bias_calc_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/bias/bias_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    23945 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.435031 NREL-sup3r-0.0.9/sup3r/models/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    38158 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19600 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/conditional_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/data_centric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    44392 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/multi_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/solar_cc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27444 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/wind.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/models/wind_conditional_moments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.435031 NREL-sup3r-0.0.9/sup3r/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/pipeline/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    76651 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/pipeline/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/pipeline/forward_pass_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/pipeline/pipeline_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.435031 NREL-sup3r-0.0.9/sup3r/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28621 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/postprocessing/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/postprocessing/data_collect_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28583 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/postprocessing/file_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.435031 NREL-sup3r-0.0.9/sup3r/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56176 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/preprocessing/batch_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    34296 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/preprocessing/conditional_moment_batch_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/preprocessing/data_extract_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   125200 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/preprocessing/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/preprocessing/exogenous_data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    54171 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/preprocessing/feature_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.435031 NREL-sup3r-0.0.9/sup3r/qa/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/qa/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/qa/qa_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    55442 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/qa/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/qa/stats_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/qa/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/qa/visual_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/qa/visual_qa_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.435031 NREL-sup3r-0.0.9/sup3r/solar/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/solar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25150 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/solar/solar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/solar/solar_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 16:39:19.439031 NREL-sup3r-0.0.9/sup3r/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/loss_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)    29470 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/regridder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/regridder_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/stitching.py
--rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    55501 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/utilities/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-20 16:39:10.000000 NREL-sup3r-0.0.9/sup3r/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.973237 NREL-sup3r-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.965237 NREL-sup3r-0.1.0/NREL_sup3r.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-13 22:50:37.000000 NREL-sup3r-0.1.0/NREL_sup3r.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-13 22:50:37.000000 NREL-sup3r-0.1.0/NREL_sup3r.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:50:37.000000 NREL-sup3r-0.1.0/NREL_sup3r.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-13 22:50:37.000000 NREL-sup3r-0.1.0/NREL_sup3r.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:50:37.000000 NREL-sup3r-0.1.0/NREL_sup3r.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-13 22:50:37.000000 NREL-sup3r-0.1.0/NREL_sup3r.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 22:50:37.000000 NREL-sup3r-0.1.0/NREL_sup3r.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-13 22:50:37.973237 NREL-sup3r-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:50:37.973237 NREL-sup3r-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.965237 NREL-sup3r-0.1.0/sup3r/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.969237 NREL-sup3r-0.1.0/sup3r/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/batch/batch_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.969237 NREL-sup3r-0.1.0/sup3r/bias/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/bias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31861 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/bias/bias_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/bias/bias_calc_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/bias/bias_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23945 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.969237 NREL-sup3r-0.1.0/sup3r/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38158 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19600 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/conditional_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/data_centric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44392 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/multi_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/solar_cc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27444 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/wind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/models/wind_conditional_moments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.969237 NREL-sup3r-0.1.0/sup3r/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/pipeline/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76715 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/pipeline/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/pipeline/forward_pass_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/pipeline/pipeline_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.969237 NREL-sup3r-0.1.0/sup3r/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28788 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/postprocessing/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/postprocessing/data_collect_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29319 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/postprocessing/file_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.973237 NREL-sup3r-0.1.0/sup3r/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56176 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/preprocessing/batch_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39388 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/preprocessing/conditional_moment_batch_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/preprocessing/data_extract_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126746 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/preprocessing/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/preprocessing/exogenous_data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53472 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/preprocessing/feature_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.973237 NREL-sup3r-0.1.0/sup3r/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/qa/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/qa/qa_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55442 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/qa/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/qa/stats_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/qa/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/qa/visual_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/qa/visual_qa_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.973237 NREL-sup3r-0.1.0/sup3r/solar/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/solar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25188 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/solar/solar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/solar/solar_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:50:37.973237 NREL-sup3r-0.1.0/sup3r/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/loss_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29957 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/regridder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/regridder_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/stitching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12716 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45455 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/utilities/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 22:50:29.000000 NREL-sup3r-0.1.0/sup3r/version.py
```

### Comparing `NREL-sup3r-0.0.9/LICENSE` & `NREL-sup3r-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/NREL_sup3r.egg-info/PKG-INFO` & `NREL-sup3r-0.1.0/NREL_sup3r.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: NREL-sup3r
-Version: 0.0.9
+Version: 0.1.0
 Summary: Super Resolving Renewable Resource Data (sup3r)
 Home-page: https://github.com/NREL/sup3r
 Author: Brandon Benton
 Author-email: brandon.benton@nrel.gov
 License: BSD 3-Clause
 Keywords: sup3r
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
 
 #################
 Welcome to SUP3R!
 #################
```

### Comparing `NREL-sup3r-0.0.9/NREL_sup3r.egg-info/SOURCES.txt` & `NREL-sup3r-0.1.0/NREL_sup3r.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 sup3r/qa/visual_qa_cli.py
 sup3r/solar/__init__.py
 sup3r/solar/solar.py
 sup3r/solar/solar_cli.py
 sup3r/utilities/__init__.py
 sup3r/utilities/cli.py
 sup3r/utilities/execution.py
+sup3r/utilities/interpolation.py
 sup3r/utilities/loss_metrics.py
 sup3r/utilities/plotting.py
 sup3r/utilities/pytest.py
 sup3r/utilities/regridder.py
 sup3r/utilities/regridder_cli.py
 sup3r/utilities/stitching.py
 sup3r/utilities/topo.py
```

### Comparing `NREL-sup3r-0.0.9/NREL_sup3r.egg-info/entry_points.txt` & `NREL-sup3r-0.1.0/NREL_sup3r.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/PKG-INFO` & `NREL-sup3r-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: NREL-sup3r
-Version: 0.0.9
+Version: 0.1.0
 Summary: Super Resolving Renewable Resource Data (sup3r)
 Home-page: https://github.com/NREL/sup3r
 Author: Brandon Benton
 Author-email: brandon.benton@nrel.gov
 License: BSD 3-Clause
 Keywords: sup3r
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: dev
 License-File: LICENSE
 
 #################
 Welcome to SUP3R!
 #################
```

### Comparing `NREL-sup3r-0.0.9/README.rst` & `NREL-sup3r-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/setup.py` & `NREL-sup3r-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,14 @@
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     test_suite="tests",
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=install_requires,
     extras_require={
         "dev": ["flake8", "pre-commit", "pylint"],
     },
     cmdclass={"develop": PostDevelopCommand},
 )
```

### Comparing `NREL-sup3r-0.0.9/sup3r/batch/batch.py` & `NREL-sup3r-0.1.0/sup3r/batch/batch.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/batch/batch_cli.py` & `NREL-sup3r-0.1.0/sup3r/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/bias/bias_calc.py` & `NREL-sup3r-0.1.0/sup3r/bias/bias_calc.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/bias/bias_calc_cli.py` & `NREL-sup3r-0.1.0/sup3r/bias/bias_calc_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/bias/bias_transforms.py` & `NREL-sup3r-0.1.0/sup3r/bias/bias_transforms.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/cli.py` & `NREL-sup3r-0.1.0/sup3r/cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/models/__init__.py` & `NREL-sup3r-0.1.0/sup3r/models/__init__.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/models/abstract.py` & `NREL-sup3r-0.1.0/sup3r/models/abstract.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/models/base.py` & `NREL-sup3r-0.1.0/sup3r/models/base.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/models/conditional_moments.py` & `NREL-sup3r-0.1.0/sup3r/models/conditional_moments.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/models/data_centric.py` & `NREL-sup3r-0.1.0/sup3r/models/data_centric.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/models/linear.py` & `NREL-sup3r-0.1.0/sup3r/models/linear.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/models/multi_step.py` & `NREL-sup3r-0.1.0/sup3r/models/multi_step.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/models/solar_cc.py` & `NREL-sup3r-0.1.0/sup3r/models/solar_cc.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,20 +121,23 @@
         for tslice in day_slices:
             disc_t = self._tf_discriminate(hi_res_true[:, :, :, tslice, :])
             gen_c = self.calc_loss_gen_content(hi_res_true[:, :, :, tslice, :],
                                                hi_res_gen[:, :, :, tslice, :])
             disc_out_true.append(disc_t)
             loss_gen_content += gen_c
 
-        # strided sampling of all hours for gen adverserial loss
-        time_samples = range(0, t_len - self.STRIDE_LEN, self.STRIDE_LEN)
-        time_samples = [slice(i0, i0 + self.DAYLIGHT_HOURS)
-                        for i0 in time_samples]
-        for t_slice in time_samples:
-            disc_g = self._tf_discriminate(hi_res_gen[:, :, :, t_slice, :])
+        # Randomly sample daylight windows from generated data. Better than
+        # strided samples covering full day because the random samples will
+        # provide an evenly balanced training set for the disc
+        logits = [[1.0] * (t_len - self.DAYLIGHT_HOURS)]
+        time_samples = tf.random.categorical(logits, len(day_slices))
+        for i in range(len(day_slices)):
+            t0 = time_samples[0, i]
+            t1 = t0 + self.DAYLIGHT_HOURS
+            disc_g = self._tf_discriminate(hi_res_gen[:, :, :, t0:t1, :])
             disc_out_gen.append(disc_g)
 
         disc_out_true = tf.concat([disc_out_true], axis=0)
         disc_out_gen = tf.concat([disc_out_gen], axis=0)
         loss_disc = self.calc_loss_disc(disc_out_true, disc_out_gen)
 
         loss_gen_content /= len(day_slices)
```

### Comparing `NREL-sup3r-0.0.9/sup3r/models/surface.py` & `NREL-sup3r-0.1.0/sup3r/models/surface.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/models/wind.py` & `NREL-sup3r-0.1.0/sup3r/models/wind.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/models/wind_conditional_moments.py` & `NREL-sup3r-0.1.0/sup3r/models/wind_conditional_moments.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/pipeline/config.py` & `NREL-sup3r-0.1.0/sup3r/pipeline/config.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/pipeline/forward_pass.py` & `NREL-sup3r-0.1.0/sup3r/pipeline/forward_pass.py`

 * *Files 1% similar despite different names*

```diff
@@ -990,14 +990,15 @@
         node_index : int
             Index of node used to run forward pass
         """
 
         self.strategy = strategy
         self.chunk_index = chunk_index
         self.node_index = node_index
+        self.output_data = None
 
         msg = (f'Requested forward pass on chunk_index={chunk_index} > '
                f'n_chunks={strategy.chunks}')
         assert chunk_index <= strategy.chunks, msg
 
         logger.info(f'Initializing ForwardPass for chunk={chunk_index} '
                     f'(temporal_chunk={self.temporal_chunk_index}, '
@@ -1811,24 +1812,24 @@
         logger.info(msg)
 
         data_chunk = self.input_data
         exo_data = None
         if self.exogenous_data is not None:
             exo_data = self._prep_exogenous_input(data_chunk.shape)
 
-        out_data = self._run_generator(
+        self.output_data = self._run_generator(
             data_chunk, hr_crop_slices=self.hr_crop_slice, model=self.model,
             model_kwargs=self.model_kwargs, model_class=self.model_class,
             s_enhance=self.s_enhance, t_enhance=self.t_enhance,
             exo_data=exo_data)
 
-        self._constant_output_check(out_data)
+        self._constant_output_check(self.output_data)
 
         if self.out_file is not None:
             logger.info(f'Saving forward pass output to {self.out_file}.')
             self.output_handler_class._write_output(
-                data=out_data, features=self.model.output_features,
+                data=self.output_data, features=self.model.output_features,
                 lat_lon=self.hr_lat_lon, times=self.hr_times,
                 out_file=self.out_file, meta_data=self.meta,
                 max_workers=self.output_workers, gids=self.gids)
         else:
-            return out_data
+            return self.output_data
```

### Comparing `NREL-sup3r-0.0.9/sup3r/pipeline/forward_pass_cli.py` & `NREL-sup3r-0.1.0/sup3r/pipeline/forward_pass_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/pipeline/pipeline.py` & `NREL-sup3r-0.1.0/sup3r/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/pipeline/pipeline_cli.py` & `NREL-sup3r-0.1.0/sup3r/pipeline/pipeline_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/postprocessing/collection.py` & `NREL-sup3r-0.1.0/sup3r/postprocessing/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,22 +104,22 @@
         """
 
         final_index = final_meta.index
         new_index = new_meta.index
         row_loc = np.where(final_time_index.isin(new_time_index))[0]
         col_loc = np.where(final_meta['gid'].isin(new_meta['gid']))[0]
 
-        if not any(row_loc):
+        if not len(row_loc) > 0:
             msg = ('Could not find row locations in file collection. '
                    'New time index: {} final time index: {}'
                    .format(new_time_index, final_time_index))
             logger.error(msg)
             raise RuntimeError(msg)
 
-        if not any(col_loc):
+        if not len(col_loc) > 0:
             msg = ('Could not find col locations in file collection. '
                    'New index: {} final index: {}'
                    .format(new_index, final_index))
             logger.error(msg)
             raise RuntimeError(msg)
 
         row_slice = slice(np.min(row_loc), np.max(row_loc) + 1)
@@ -613,14 +613,17 @@
         overwrite : bool
             Whether to overwrite existing output file
         threshold : float
             Threshold distance for finding target coordinates within full meta
         """
         t0 = time.time()
 
+        logger.info(f'Initializing collection for file_paths={file_paths}, '
+                    f'with max_workers={max_workers}.')
+
         if log_level is not None:
             init_logger('sup3r.preprocessing', log_file=log_file,
                         log_level=log_level)
 
         logger.info(f'Using target_final_meta_file={target_final_meta_file}')
 
         if not os.path.exists(os.path.dirname(out_file)):
@@ -660,15 +663,15 @@
 
             else:
                 for j, flist in enumerate(flist_chunks):
                     logger.info('Collecting file list chunk {} out of {} '
                                 .format(j + 1, len(flist_chunks)))
                     time_index, target_final_meta, masked_meta, shape, _ = \
                         collector._get_collection_attrs(
-                            flist,
+                            flist, max_workers=max_workers,
                             target_final_meta_file=target_final_meta_file,
                             threshold=threshold)
                     collector._collect_flist(dset, masked_meta, time_index,
                                              shape, flist, out_file,
                                              target_masked_meta,
                                              max_workers=max_workers)
```

### Comparing `NREL-sup3r-0.0.9/sup3r/postprocessing/data_collect_cli.py` & `NREL-sup3r-0.1.0/sup3r/postprocessing/data_collect_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/postprocessing/file_handling.py` & `NREL-sup3r-0.1.0/sup3r/postprocessing/file_handling.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from datetime import datetime as dt
 import json
 import os
 from warnings import warn
 
 from sup3r.version import __version__
 from sup3r.utilities import VERSION_RECORD
-from sup3r.utilities.utilities import (invert_uv, estimate_max_workers,
+from sup3r.utilities.utilities import (invert_uv,
+                                       get_time_dim_name,
+                                       estimate_max_workers,
                                        pd_date_range)
 from sup3r.preprocessing.feature_handling import Feature
 
 from rex.outputs import Outputs as BaseRexOutputs
 
 logger = logging.getLogger(__name__)
 
@@ -116,14 +118,37 @@
 
 
 class OutputMixIn:
     """MixIn class with methods used by various Output and Collection classes
     """
 
     @staticmethod
+    def get_time_dim_name(filepath):
+        """Get the name of the time dimension in the given file
+
+        Parameters
+        ----------
+        filepath : str
+            Path to the file
+
+        Returns
+        -------
+        time_key : str
+            Name of the time dimension in the given file
+        """
+
+        handle = xr.open_dataset(filepath)
+        valid_vars = set(handle.dims)
+        time_key = list({'time', 'Time'}.intersection(valid_vars))
+        if len(time_key) > 0:
+            return time_key[0]
+        else:
+            return 'time'
+
+    @staticmethod
     def get_dset_attrs(feature):
         """Get attrributes for output feature
 
         Parameters
         ----------
         feature : str
             Name of feature to write
@@ -546,26 +571,27 @@
                      for k, v in meta_data.items()}
 
         with xr.Dataset(data_vars=data_vars, coords=coords,
                         attrs=attrs) as ncfile:
             ncfile.to_netcdf(out_file)
         logger.info(f'Saved output of size {data.shape} to: {out_file}')
 
-    @staticmethod
-    def combine_file(files, outfile):
+    @classmethod
+    def combine_file(cls, files, outfile):
         """Combine all chunked output files from ForwardPass into a single file
 
         Parameters
         ----------
         files : list
             List of chunked output files from ForwardPass runs
         outfile : str
             Output file name for combined file
         """
-        ds = xr.open_mfdataset(files, combine='nested', concat_dim='Time')
+        time_key = get_time_dim_name(files[0])
+        ds = xr.open_mfdataset(files, combine='nested', concat_dim=time_key)
         ds.to_netcdf(outfile)
         logger.info(f'Saved combined file: {outfile}')
 
 
 class OutputHandlerH5(OutputHandler):
     """Class to handle writing output to H5 file"""
 
@@ -751,12 +777,12 @@
                                                max_workers)
         gids = (gids if gids is not None
                 else np.arange(np.product(lat_lon.shape[:-1])))
         meta = pd.DataFrame({'gid': gids.flatten(),
                              'latitude': lat_lon[..., 0].flatten(),
                              'longitude': lat_lon[..., 1].flatten()})
         data_list = []
-        for i, f in enumerate(features):
+        for i, _ in enumerate(features):
             flat_data = data[..., i].reshape((-1, len(times)))
             flat_data = np.transpose(flat_data, (1, 0))
             data_list.append(flat_data)
         cls.write_data(out_file, features, times, data_list, meta, meta_data)
```

### Comparing `NREL-sup3r-0.0.9/sup3r/preprocessing/batch_handling.py` & `NREL-sup3r-0.1.0/sup3r/preprocessing/batch_handling.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/preprocessing/conditional_moment_batch_handling.py` & `NREL-sup3r-0.1.0/sup3r/preprocessing/conditional_moment_batch_handling.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,16 @@
         """Get the mask for the batch."""
         return self._mask
 
     # pylint: disable=W0613
     @staticmethod
     def make_output(low_res, high_res,
                     s_enhance=None, t_enhance=None,
-                    model_mom1=None, output_features_ind=None):
+                    model_mom1=None, output_features_ind=None,
+                    t_enhance_mode='constant'):
         """Make custom batch output
 
         Parameters
         ----------
         low_res : np.ndarray
             4D | 5D array
             (batch_size, spatial_1, spatial_2, features)
@@ -89,20 +90,25 @@
         t_enhance : int | None
             Temporal enhancement factor
         model_mom1 : Sup3rCondMom | None
             Model used to modify the make the batch output
         output_features_ind : list | np.ndarray | None
             List/array of feature channel indices that are used for generative
             output, without any feature indices used only for training.
+        t_enhance_mode : str
+            Enhancing mode for temporal subfilter.
+            Can be either constant or linear
         """
         return high_res
 
     # pylint: disable=E1130
     @staticmethod
-    def make_mask(high_res, s_padding=None, t_padding=None):
+    def make_mask(high_res,
+                  s_padding=None, t_padding=None,
+                  end_t_padding=False, t_enhance=None):
         """Make mask for output.
         The mask is used to ensure consistency when training conditional
         moments.
         Consider the case of learning E(HR|LR) where HR is the high_res and
         LR is the low_res.
         In theory, the conditional moment estimation works if
         the full LR is passed as input and predicts the full HR.
@@ -124,46 +130,61 @@
             (batch_size, spatial_1, spatial_2, temporal, features)
         s_padding : int | None
             Spatial padding size. If None or 0, no padding is applied.
             None by default
         t_padding : int | None
             Temporal padding size. If None or 0, no padding is applied.
             None by default
+        end_t_padding : bool | False
+            Zero pad the end of temporal space.
+            Ensures that loss is calculated only if snapshot is surrounded
+            by temporal landmarks.
+            False by default
+        t_enhance : int | None
+            Temporal enhancement factor to define end padding.
+            None by default
         model_mom1 : Sup3rCondMom | None
             Model used to modify the make the batch output
         output_features_ind : list | np.ndarray | None
             List/array of feature channel indices that are used for generative
             output, without any feature indices used only for training.
         """
         mask = np.zeros(high_res.shape, dtype=np.float32)
         s_min = s_padding if s_padding is not None else 0
         t_min = t_padding if t_padding is not None else 0
         s_max = -s_padding if s_min > 0 else None
         t_max = -t_padding if t_min > 0 else None
+        if end_t_padding and t_enhance > 1:
+            if t_max is None:
+                t_max = -(t_enhance - 1)
+            else:
+                t_max = -(t_enhance - 1) - t_padding
 
         if len(high_res.shape) == 4:
             mask[:, s_min:s_max, s_min:s_max, :] = 1.0
         elif len(high_res.shape) == 5:
             mask[:, s_min:s_max, s_min:s_max, t_min:t_max, :] = 1.0
 
         return mask
 
     # pylint: disable=W0613
     @classmethod
     def get_coarse_batch(cls, high_res,
                          s_enhance, t_enhance=1,
                          temporal_coarsening_method='subsample',
+                         temporal_enhancing_method='constant',
                          output_features_ind=None,
                          output_features=None,
                          training_features=None,
                          smoothing=None,
                          smoothing_ignore=None,
                          model_mom1=None,
                          s_padding=None,
-                         t_padding=None):
+                         t_padding=None,
+                         end_t_padding=False):
         """Coarsen high res data and return Batch with high res and
         low res data
 
         Parameters
         ----------
         high_res : np.ndarray
             4D | 5D array
@@ -174,14 +195,23 @@
             resolution data
         t_enhance : int
             Factor by which to coarsen temporal dimension of the high
             resolution data
         temporal_coarsening_method : str
             Method to use for temporal coarsening. Can be subsample, average,
             or total
+        temporal_enhancing_method : str
+            [constant, linear]
+            Method to enhance temporally when constructing subfilter.
+            At every temporal location, a low-res temporal data is substracted
+            from the high-res temporal data predicted.
+            constant will assume that the low-res temporal data is constant
+            between landmarks.
+            linear will linearly interpolate between landmarks to generate the
+            low-res data to remove from the high-res.
         output_features_ind : list | np.ndarray | None
             List/array of feature channel indices that are used for generative
             output, without any feature indices used only for training.
         output_features : list
             List of Generative model output feature names
         training_features : list | None
             Ordered list of training features input to the generative model
@@ -198,14 +228,19 @@
             Model used to modify the make the batch output
         s_padding : int | None
             Width of spatial padding to predict only middle part. If None,
             no padding is used
         t_padding : int | None
             Width of temporal padding to predict only middle part. If None,
             no padding is used
+        end_t_padding : bool | False
+            Zero pad the end of temporal space.
+            Ensures that loss is calculated only if snapshot is surrounded
+            by temporal landmarks.
+            False by default
 
         Returns
         -------
         Batch
             Batch instance with low and high res data
         """
         low_res = spatial_coarsening(high_res, s_enhance)
@@ -221,30 +256,32 @@
                                           temporal_coarsening_method)
 
         low_res = smooth_data(low_res, training_features, smoothing_ignore,
                               smoothing)
         high_res = cls.reduce_features(high_res, output_features_ind)
         output = cls.make_output(low_res, high_res,
                                  s_enhance, t_enhance,
-                                 model_mom1, output_features_ind)
+                                 model_mom1, output_features_ind,
+                                 temporal_enhancing_method)
         mask = cls.make_mask(high_res,
-                             s_padding, t_padding)
+                             s_padding, t_padding, end_t_padding, t_enhance)
         batch = cls(low_res, high_res, output, mask)
 
         return batch
 
 
 class BatchMom1SF(BatchMom1):
     """Batch of low_res, high_res and output data
     when learning first moment of subfilter vel"""
 
     @staticmethod
     def make_output(low_res, high_res,
                     s_enhance=None, t_enhance=None,
-                    model_mom1=None, output_features_ind=None):
+                    model_mom1=None, output_features_ind=None,
+                    t_enhance_mode='constant'):
         """Make custom batch output
 
         Parameters
         ----------
         low_res : np.ndarray
             4D | 5D array
             (batch_size, spatial_1, spatial_2, features)
@@ -258,32 +295,37 @@
         t_enhance : int | None
             Temporal enhancement factor
         model_mom1 : Sup3rCondMom | None
             Model used to modify the make the batch output
         output_features_ind : list | np.ndarray | None
             List/array of feature channel indices that are used for generative
             output, without any feature indices used only for training.
+        t_enhance_mode : str
+            Enhancing mode for temporal subfilter.
+            Can be either constant or linear
         """
         # Remove LR from HR
         enhanced_lr = spatial_simple_enhancing(low_res,
                                                s_enhance=s_enhance)
         enhanced_lr = temporal_simple_enhancing(enhanced_lr,
-                                                t_enhance=t_enhance)
+                                                t_enhance=t_enhance,
+                                                mode=t_enhance_mode)
         enhanced_lr = Batch.reduce_features(enhanced_lr, output_features_ind)
         return high_res - enhanced_lr
 
 
 class BatchMom2(BatchMom1):
     """Batch of low_res, high_res and output data
     when learning second moment"""
 
     @staticmethod
     def make_output(low_res, high_res,
                     s_enhance=None, t_enhance=None,
-                    model_mom1=None, output_features_ind=None):
+                    model_mom1=None, output_features_ind=None,
+                    t_enhance_mode='constant'):
         """Make custom batch output
 
         Parameters
         ----------
         low_res : np.ndarray
             4D | 5D array
             (batch_size, spatial_1, spatial_2, features)
@@ -297,28 +339,32 @@
         t_enhance : int | None
             Temporal enhancement factor
         model_mom1 : Sup3rCondMom | None
             Model used to modify the make the batch output
         output_features_ind : list | np.ndarray | None
             List/array of feature channel indices that are used for generative
             output, without any feature indices used only for training.
+        t_enhance_mode : str
+            Enhancing mode for temporal subfilter.
+            Can be either constant or linear
         """
         # Remove first moment from HR and square it
         out = model_mom1._tf_generate(low_res).numpy()
         return (high_res - out)**2
 
 
 class BatchMom2Sep(BatchMom1):
     """Batch of low_res, high_res and output data
     when learning second moment separate from first moment"""
 
     @staticmethod
     def make_output(low_res, high_res,
                     s_enhance=None, t_enhance=None,
-                    model_mom1=None, output_features_ind=None):
+                    model_mom1=None, output_features_ind=None,
+                    t_enhance_mode='constant'):
         """Make custom batch output
 
         Parameters
         ----------
         low_res : np.ndarray
             4D | 5D array
             (batch_size, spatial_1, spatial_2, features)
@@ -332,30 +378,35 @@
         t_enhance : int | None
             Temporal enhancement factor
         model_mom1 : Sup3rCondMom | None
             Model used to modify the make the batch output
         output_features_ind : list | np.ndarray | None
             List/array of feature channel indices that are used for generative
             output, without any feature indices used only for training.
+        t_enhance_mode : str
+            Enhancing mode for temporal subfilter.
+            Can be either constant or linear
         """
         return super(BatchMom2Sep,
                      BatchMom2Sep).make_output(low_res, high_res,
                                                s_enhance, t_enhance,
                                                model_mom1,
-                                               output_features_ind)**2
+                                               output_features_ind,
+                                               t_enhance_mode)**2
 
 
 class BatchMom2SF(BatchMom1):
     """Batch of low_res, high_res and output data
     when learning second moment of subfilter vel"""
 
     @staticmethod
     def make_output(low_res, high_res,
                     s_enhance=None, t_enhance=None,
-                    model_mom1=None, output_features_ind=None):
+                    model_mom1=None, output_features_ind=None,
+                    t_enhance_mode='constant'):
         """Make custom batch output
 
         Parameters
         ----------
         low_res : np.ndarray
             4D | 5D array
             (batch_size, spatial_1, spatial_2, features)
@@ -369,34 +420,39 @@
         t_enhance : int | None
             Temporal enhancement factor
         model_mom1 : Sup3rCondMom | None
             Model used to modify the make the batch output
         output_features_ind : list | np.ndarray | None
             List/array of feature channel indices that are used for generative
             output, without any feature indices used only for training.
+        t_enhance_mode : str
+            Enhancing mode for temporal subfilter.
+            Can be either 'constant' or 'linear'
         """
         # Remove LR and first moment from HR and square it
         out = model_mom1._tf_generate(low_res).numpy()
         enhanced_lr = spatial_simple_enhancing(low_res,
                                                s_enhance=s_enhance)
         enhanced_lr = temporal_simple_enhancing(enhanced_lr,
-                                                t_enhance=t_enhance)
+                                                t_enhance=t_enhance,
+                                                mode=t_enhance_mode)
         enhanced_lr = Batch.reduce_features(enhanced_lr, output_features_ind)
         return (high_res - enhanced_lr - out)**2
 
 
 class BatchMom2SepSF(BatchMom1SF):
     """Batch of low_res, high_res and output data
     when learning second moment of subfilter vel
     separate from first moment"""
 
     @staticmethod
     def make_output(low_res, high_res,
                     s_enhance=None, t_enhance=None,
-                    model_mom1=None, output_features_ind=None):
+                    model_mom1=None, output_features_ind=None,
+                    t_enhance_mode='constant'):
         """Make custom batch output
 
         Parameters
         ----------
         low_res : np.ndarray
             4D | 5D array
             (batch_size, spatial_1, spatial_2, features)
@@ -410,36 +466,41 @@
         t_enhance : int | None
             Temporal enhancement factor
         model_mom1 : Sup3rCondMom | None
             Model used to modify the make the batch output
         output_features_ind : list | np.ndarray | None
             List/array of feature channel indices that are used for generative
             output, without any feature indices used only for training.
+        t_enhance_mode : str
+            Enhancing mode for temporal subfilter.
+            Can be either constant or linear
         """
         # Remove LR from HR and square it
         return super(BatchMom2SepSF,
                      BatchMom2SepSF).make_output(low_res, high_res,
                                                  s_enhance, t_enhance,
                                                  model_mom1,
-                                                 output_features_ind)**2
+                                                 output_features_ind,
+                                                 t_enhance_mode)**2
 
 
 class ValidationDataMom1(ValidationData):
     """Iterator for validation data"""
 
     # Classes to use for handling an individual batch obj.
     BATCH_CLASS = BatchMom1
 
     def __init__(self, data_handlers, batch_size=8, s_enhance=3, t_enhance=1,
                  temporal_coarsening_method='subsample',
+                 temporal_enhancing_method='constant',
                  output_features_ind=None,
                  output_features=None,
                  smoothing=None, smoothing_ignore=None,
                  model_mom1=None,
-                 s_padding=None, t_padding=None):
+                 s_padding=None, t_padding=None, end_t_padding=False):
         """
         Parameters
         ----------
         handlers : list[DataHandler]
             List of DataHandler instances
         batch_size : int
             Size of validation data batches
@@ -450,14 +511,23 @@
             Factor by which to coarsen temporal dimension of the high
             resolution data
         temporal_coarsening_method : str
             [subsample, average, total]
             Subsample will take every t_enhance-th time step, average will
             average over t_enhance time steps, total will sum over t_enhance
             time steps
+        temporal_enhancing_method : str
+            [constant, linear]
+            Method to enhance temporally when constructing subfilter.
+            At every temporal location, a low-res temporal data is substracted
+            from the high-res temporal data predicted.
+            constant will assume that the low-res temporal data is constant
+            between landmarks.
+            linear will linearly interpolate between landmarks to generate the
+            low-res data to remove from the high-res.
         output_features_ind : list | np.ndarray | None
             List/array of feature channel indices that are used for generative
             output, without any feature indices used only for training.
         output_features : list
             List of Generative model output feature names
         smoothing : float | None
             Standard deviation to use for gaussian filtering of the coarse
@@ -473,14 +543,19 @@
             Useful to prepare data for learning second conditional moment.
         s_padding : int | None
             Width of spatial padding to predict only middle part. If None,
             no padding is used
         t_padding : int | None
             Width of temporal padding to predict only middle part. If None,
             no padding is used
+        end_t_padding : bool | False
+            Zero pad the end of temporal space.
+            Ensures that loss is calculated only if snapshot is surrounded
+            by temporal landmarks.
+            False by default
         """
 
         handler_shapes = np.array([d.sample_shape for d in data_handlers])
         assert np.all(handler_shapes[0] == handler_shapes)
 
         self.handlers = data_handlers
         self.batch_size = batch_size
@@ -488,16 +563,18 @@
         self.val_indices = self._get_val_indices()
         self.max = np.ceil(
             len(self.val_indices) / (batch_size))
         self.s_enhance = s_enhance
         self.t_enhance = t_enhance
         self.s_padding = s_padding
         self.t_padding = t_padding
+        self.end_t_padding = end_t_padding
         self._remaining_observations = len(self.val_indices)
         self.temporal_coarsening_method = temporal_coarsening_method
+        self.temporal_enhancing_method = temporal_enhancing_method
         self._i = 0
         self.output_features_ind = output_features_ind
         self.output_features = output_features
         self.smoothing = smoothing
         self.smoothing_ignore = smoothing_ignore
         self.model_mom1 = model_mom1
 
@@ -515,38 +592,41 @@
         -------
         batch : Batch
         """
         return self.BATCH_CLASS.get_coarse_batch(
             high_res, self.s_enhance,
             t_enhance=self.t_enhance,
             temporal_coarsening_method=self.temporal_coarsening_method,
+            temporal_enhancing_method=self.temporal_enhancing_method,
             output_features_ind=self.output_features_ind,
             smoothing=self.smoothing,
             smoothing_ignore=self.smoothing_ignore,
             output_features=self.output_features,
             model_mom1=self.model_mom1,
             s_padding=self.s_padding,
-            t_padding=self.t_padding)
+            t_padding=self.t_padding,
+            end_t_padding=self.end_t_padding)
 
 
 class BatchHandlerMom1(BatchHandler):
     """Sup3r base batch handling class"""
 
     # Classes to use for handling an individual batch obj.
     VAL_CLASS = ValidationDataMom1
     BATCH_CLASS = BatchMom1
     DATA_HANDLER_CLASS = None
 
     def __init__(self, data_handlers, batch_size=8, s_enhance=3, t_enhance=1,
                  means=None, stds=None, norm=True, n_batches=10,
-                 temporal_coarsening_method='subsample', stdevs_file=None,
+                 temporal_coarsening_method='subsample',
+                 temporal_enhancing_method='constant', stdevs_file=None,
                  means_file=None, overwrite_stats=False, smoothing=None,
                  smoothing_ignore=None, stats_workers=None, norm_workers=None,
                  load_workers=None, max_workers=None, model_mom1=None,
-                 s_padding=None, t_padding=None):
+                 s_padding=None, t_padding=None, end_t_padding=False):
         """
         Parameters
         ----------
         data_handlers : list[DataHandler]
             List of DataHandler instances
         batch_size : int
             Number of observations in a batch
@@ -572,14 +652,23 @@
             Number of batches in an epoch, this sets the iteration limit for
             this object.
         temporal_coarsening_method : str
             [subsample, average, total]
             Subsample will take every t_enhance-th time step, average will
             average over t_enhance time steps, total will sum over t_enhance
             time steps
+        temporal_enhancing_method : str
+            [constant, linear]
+            Method to enhance temporally when constructing subfilter.
+            At every temporal location, a low-res temporal data is substracted
+            from the high-res temporal data predicted.
+            constant will assume that the low-res temporal data is constant
+            between landmarks.
+            linear will linearly interpolate between landmarks to generate the
+            low-res data to remove from the high-res.
         stdevs_file : str | None
             Path to stdevs data or where to save data after calling get_stats
         means_file : str | None
             Path to means data or where to save data after calling get_stats
         overwrite_stats : bool
             Whether to overwrite stats cache files.
         smoothing : float | None
@@ -609,14 +698,19 @@
             Useful to prepare data for learning second conditional moment.
         s_padding : int | None
             Width of spatial padding to predict only middle part. If None,
             no padding is used
         t_padding : int | None
             Width of temporal padding to predict only middle part. If None,
             no padding is used
+        end_t_padding : bool | False
+            Zero pad the end of temporal space.
+            Ensures that loss is calculated only if snapshot is surrounded
+            by temporal landmarks.
+            False by default
         """
         if max_workers is not None:
             norm_workers = stats_workers = load_workers = max_workers
 
         msg = ('All data handlers must have the same sample_shape')
         handler_shapes = np.array([d.sample_shape for d in data_handlers])
         assert np.all(handler_shapes[0] == handler_shapes), msg
@@ -628,19 +722,21 @@
         self.output = None
         self.batch_size = batch_size
         self._val_data = None
         self.s_enhance = s_enhance
         self.t_enhance = t_enhance
         self.s_padding = s_padding
         self.t_padding = t_padding
+        self.end_t_padding = end_t_padding
         self.sample_shape = handler_shapes[0]
         self.means = means
         self.stds = stds
         self.n_batches = n_batches
         self.temporal_coarsening_method = temporal_coarsening_method
+        self.temporal_enhancing_method = temporal_enhancing_method
         self.current_batch_indices = None
         self.current_handler_index = None
         self.stdevs_file = stdevs_file
         self.means_file = means_file
         self.overwrite_stats = overwrite_stats
         self.smoothing = smoothing
         self.smoothing_ignore = smoothing_ignore or []
@@ -667,21 +763,23 @@
             self.normalize(self.means, self.stds)
 
         logger.debug('Getting validation data for BatchHandler.')
         self.val_data = self.VAL_CLASS(
             data_handlers, batch_size=batch_size,
             s_enhance=s_enhance, t_enhance=t_enhance,
             temporal_coarsening_method=temporal_coarsening_method,
+            temporal_enhancing_method=temporal_enhancing_method,
             output_features_ind=self.output_features_ind,
             output_features=self.output_features,
             smoothing=self.smoothing,
             smoothing_ignore=self.smoothing_ignore,
             model_mom1=self.model_mom1,
             s_padding=self.s_padding,
-            t_padding=self.t_padding)
+            t_padding=self.t_padding,
+            end_t_padding=self.end_t_padding)
 
         logger.info('Finished initializing BatchHandler.')
         log_mem(logger, log_level='INFO')
 
     def __next__(self):
         """Get the next iterator output.
 
@@ -703,22 +801,24 @@
             for i in range(self.batch_size):
                 high_res[i, ...] = handler.get_next()
                 self.current_batch_indices.append(handler.current_obs_index)
 
             batch = self.BATCH_CLASS.get_coarse_batch(
                 high_res, self.s_enhance, t_enhance=self.t_enhance,
                 temporal_coarsening_method=self.temporal_coarsening_method,
+                temporal_enhancing_method=self.temporal_enhancing_method,
                 output_features_ind=self.output_features_ind,
                 output_features=self.output_features,
                 training_features=self.training_features,
                 smoothing=self.smoothing,
                 smoothing_ignore=self.smoothing_ignore,
                 model_mom1=self.model_mom1,
                 s_padding=self.s_padding,
-                t_padding=self.t_padding)
+                t_padding=self.t_padding,
+                end_t_padding=self.end_t_padding)
 
             self._i += 1
             return batch
         else:
             raise StopIteration
 
 
@@ -740,15 +840,16 @@
                 high_res, self.s_enhance,
                 output_features_ind=self.output_features_ind,
                 training_features=self.training_features,
                 smoothing=self.smoothing,
                 smoothing_ignore=self.smoothing_ignore,
                 model_mom1=self.model_mom1,
                 s_padding=self.s_padding,
-                t_padding=self.t_padding)
+                t_padding=self.t_padding,
+                end_t_padding=self.end_t_padding)
 
             self._i += 1
             return batch
         else:
             raise StopIteration
```

### Comparing `NREL-sup3r-0.0.9/sup3r/preprocessing/data_extract_cli.py` & `NREL-sup3r-0.1.0/sup3r/preprocessing/data_extract_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/preprocessing/data_handling.py` & `NREL-sup3r-0.1.0/sup3r/preprocessing/data_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,36 +23,35 @@
 
 from rex import MultiFileWindX, MultiFileNSRDBX, Resource
 from rex.utilities import log_mem
 from rex.utilities.fun_utils import get_fun_call_str
 
 from sup3r.utilities.utilities import (estimate_max_workers,
                                        get_chunk_slices,
-                                       interp_var_to_height,
-                                       interp_var_to_pressure,
+                                       get_time_dim_name,
                                        uniform_box_sampler,
                                        uniform_time_sampler,
                                        weighted_time_sampler,
                                        weighted_box_sampler,
                                        get_raster_shape,
                                        get_source_type,
                                        ignore_case_path_fetch,
                                        daily_temporal_coarsening,
                                        spatial_coarsening,
                                        np_to_pd_times)
+from sup3r.utilities.interpolation import Interpolator
 from sup3r.utilities import ModuleName
 from sup3r.utilities.cli import BaseCLI
 from sup3r.preprocessing.feature_handling import (FeatureHandler,
                                                   Feature,
                                                   BVFreqMon,
                                                   BVFreqSquaredH5,
                                                   BVFreqSquaredNC,
                                                   InverseMonNC,
                                                   LatLonNC,
-                                                  LatLonNCforCC,
                                                   TempNC,
                                                   TempNCforCC,
                                                   PotentialTempNC,
                                                   PressureNC,
                                                   UWind,
                                                   VWind,
                                                   LatLonH5,
@@ -379,39 +378,55 @@
     @property
     def invert_lat(self):
         """Whether to invert the latitude axis during data extraction. This is
         to enforce a descending latitude ordering so that the lower left corner
         of the grid is at idx=(-1, 0) instead of idx=(0, 0)"""
         if self._invert_lat is None:
             lat_lon = self.raw_lat_lon
-            self._invert_lat = (lat_lon[0, 0, 0] < lat_lon[-1, 0, 0])
+            self._invert_lat = (not self.lats_are_descending(lat_lon))
         return self._invert_lat
 
     @property
     def target(self):
         """Get lower left corner of raster
 
         Returns
         -------
         _target: tuple
             (lat, lon) lower left corner of raster.
         """
         if self._target is None:
             lat_lon = self.lat_lon
-            if lat_lon[0, 0, 0] < lat_lon[-1, 0, 0]:
+            if not self.lats_are_descending(lat_lon):
                 self._target = tuple(lat_lon[0, 0, :])
             else:
                 self._target = tuple(lat_lon[-1, 0, :])
         return self._target
 
     @target.setter
     def target(self, target):
         """Update target property"""
         self._target = target
 
+    @classmethod
+    def lats_are_descending(cls, lat_lon):
+        """Check if latitudes are in descending order (i.e. the target
+        coordinate is already at the bottom left corner)
+
+        Parameters
+        ----------
+        lat_lon : np.ndarray
+            Lat/Lon array with shape (n_lats, n_lons, 2)
+
+        Returns
+        -------
+        bool
+        """
+        return lat_lon[-1, 0, 0] < lat_lon[0, 0, 0]
+
     @property
     def grid_shape(self):
         """Get shape of raster
 
         Returns
         -------
         _grid_shape: tuple
@@ -514,15 +529,15 @@
         """Update time index"""
         self._time_index = time_index
 
     @property
     def time_freq_hours(self):
         """Get the time frequency in hours as a float"""
         ti_deltas = self.raw_time_index - np.roll(self.raw_time_index, 1)
-        ti_deltas_hours = ti_deltas.total_seconds()[1:-1] / 3600
+        ti_deltas_hours = pd.Series(ti_deltas).dt.total_seconds()[1:-1] / 3600
         time_freq = float(mode(ti_deltas_hours).mode[0])
         return time_freq
 
     @property
     def timestamp_0(self):
         """Get a string timestamp for the first time index value with the
         format YYYYMMDDHHMMSS"""
@@ -688,27 +703,30 @@
             one, time indices for input files will be extracted in parallel
             and then concatenated to get the full time index. If input files
             do not all have time indices or if there are few input files this
             should be set to one.
         res_kwargs : dict | None
             kwargs passed to source handler for data extraction. e.g. This
             could be {'parallel': True,
+                      'concat_dim': 'Time',
+                      'combine': 'nested',
                       'chunks': {'south_north': 120, 'west_east': 120}}
             which then gets passed to xr.open_mfdataset(file, **res_kwargs)
         """
         InputMixIn.__init__(self, target=target, shape=shape,
                             raster_file=raster_file,
                             raster_index=raster_index,
                             temporal_slice=temporal_slice)
 
         msg = 'No files provided to DataHandler. Aborting.'
         assert file_paths is not None and bool(file_paths), msg
 
         self.file_paths = file_paths
-        self.features = features
+        self.features = (features if isinstance(features, (list, tuple))
+                         else [features])
         self.val_time_index = None
         self.max_delta = max_delta
         self.val_split = val_split
         self.sample_shape = sample_shape
         self.hr_spatial_coarsen = hr_spatial_coarsen or 1
         self.time_roll = time_roll
         self.shuffle_time = shuffle_time
@@ -1949,18 +1967,19 @@
                       'chunks': {'south_north': 120, 'west_east': 120}}
             which then gets passed to xr.open_mfdataset(file, **kwargs)
 
         Returns
         -------
         data : xarray.Dataset
         """
-        default_kws = {'combine': 'nested', 'concat_dim': 'Time',
+        time_key = get_time_dim_name(file_paths[0])
+        default_kws = {'combine': 'nested', 'concat_dim': time_key,
                        'chunks': cls.CHUNKS}
-        kwargs.update(default_kws)
-        return xr.open_mfdataset(file_paths, **kwargs)
+        default_kws.update(kwargs)
+        return xr.open_mfdataset(file_paths, **default_kws)
 
     @classmethod
     def get_file_times(cls, file_paths, **kwargs):
         """Get time index from data files
 
         Parameters
         ----------
@@ -2115,23 +2134,21 @@
 
         if feature in handle:
             fdata = cls.direct_extract(handle, feature, raster_index,
                                        time_slice)
 
         elif basename in handle:
             if interp_height is not None:
-                fdata = interp_var_to_height(handle, basename,
-                                             raster_index,
-                                             np.float32(interp_height),
-                                             time_slice)
+                fdata = Interpolator.interp_var_to_height(
+                    handle, basename, raster_index, np.float32(interp_height),
+                    time_slice)
             elif interp_pressure is not None:
-                fdata = interp_var_to_pressure(handle, basename,
-                                               raster_index,
-                                               np.float32(interp_pressure),
-                                               time_slice)
+                fdata = Interpolator.interp_var_to_pressure(
+                    handle, basename, raster_index,
+                    np.float32(interp_pressure), time_slice)
 
         else:
             msg = f'{feature} cannot be extracted from source data.'
             logger.exception(msg)
             raise ValueError(msg)
 
         fdata = np.transpose(fdata, (1, 2, 0))
@@ -2249,17 +2266,22 @@
         closest = tuple(lat_lon[row, col])
         logger.debug(f'Found closest coordinate {closest} to target={target}')
         if np.hypot(closest[0] - target[0], closest[1] - target[1]) > 1:
             msg = 'Closest coordinate to target is more than 1 degree away'
             logger.warning(msg)
             warnings.warn(msg)
 
-        raster_index = [slice(row, row + grid_shape[0]),
+        if cls.lats_are_descending(lat_lon):
+            row_end = row + 1
+            row_start = row_end - grid_shape[0]
+        else:
+            row_end = row + grid_shape[0]
+            row_start = row
+        raster_index = [slice(row_start, row_end),
                         slice(col, col + grid_shape[1])]
-
         cls._validate_raster_shape(target, grid_shape, lat_lon, raster_index)
         return raster_index
 
     @classmethod
     def _check_grid_extent(cls, target, grid_shape, lat_lon):
         """Make sure the requested target coordinate lies within the available
         lat/lon grid.
@@ -2303,15 +2325,16 @@
             Array of lat/lon coordinates for entire available grid. Used to
             check whether computed raster only includes coordinates within this
             grid.
         raster_index : list
             List of slices selecting region from entire available grid.
         """
         if (raster_index[0].stop > lat_lon.shape[0]
-           or raster_index[1].stop > lat_lon.shape[1]):
+           or raster_index[1].stop > lat_lon.shape[1]
+           or raster_index[0].start < 0 or raster_index[1].start < 0):
             msg = (f'Invalid target {target}, shape {grid_shape}, and raster '
                    f'{raster_index} for data domain of size '
                    f'{lat_lon.shape[:-1]} with lower left corner '
                    f'({np.min(lat_lon[..., 0])}, {np.min(lat_lon[..., 1])}).')
             raise ValueError(msg)
 
     def get_raster_index(self):
@@ -2345,14 +2368,42 @@
             if self.raster_file is not None:
                 logger.debug(f'Saving raster index: {self.raster_file}')
                 np.save(self.raster_file.replace('.txt', '.npy'), raster_index)
 
         return raster_index
 
 
+class DataHandlerNCforERA(DataHandlerNC):
+    """Data Handler for NETCDF ERA5 data"""
+
+    CHUNKS = {'time': 5, 'lat': 20, 'lon': 20}
+    """CHUNKS sets the chunk sizes to extract from the data in each dimension.
+    Chunk sizes that approximately match the data volume being extracted
+    typically results in the most efficient IO."""
+
+    @classmethod
+    def feature_registry(cls):
+        """Registry of methods for computing features or extracting renamed
+        features
+
+        Returns
+        -------
+        dict
+            Method registry
+        """
+        registry = {
+            'U_(.*)': 'u_(.*)',
+            'V_(.*)': 'v_(.*)',
+            'Windspeed_(.*)m': WindspeedNC,
+            'Winddirection_(.*)m': WinddirectionNC,
+            'topography': 'orog',
+            'lat_lon': LatLonNC}
+        return registry
+
+
 class DataHandlerNCforCC(DataHandlerNC):
     """Data Handler for NETCDF climate change data"""
 
     CHUNKS = {'time': 5, 'lat': 20, 'lon': 20}
     """CHUNKS sets the chunk sizes to extract from the data in each dimension.
     Chunk sizes that approximately match the data volume being extracted
     typically results in the most efficient IO."""
@@ -2402,15 +2453,15 @@
             'Windspeed_(.*)m': WindspeedNC,
             'Winddirection_(.*)m': WinddirectionNC,
             'topography': 'orog',
             'relativehumidity_2m': 'hurs',
             'relativehumidity_min_2m': 'hursmin',
             'relativehumidity_max_2m': 'hursmax',
             'clearsky_ratio': ClearSkyRatioCC,
-            'lat_lon': LatLonNCforCC,
+            'lat_lon': LatLonNC,
             'Pressure_(.*)': 'plev_(.*)',
             'Temperature_(.*)': TempNCforCC,
             'temperature_2m': Tas,
             'temperature_max_2m': TasMax,
             'temperature_min_2m': TasMin}
         return registry
 
@@ -2433,16 +2484,16 @@
             which then gets passed to xr.open_mfdataset(file, **kwargs)
 
         Returns
         -------
         data : xarray.Dataset
         """
         default_kws = {'chunks': cls.CHUNKS}
-        kwargs.update(default_kws)
-        return xr.open_mfdataset(file_paths, **kwargs)
+        default_kws.update(kwargs)
+        return xr.open_mfdataset(file_paths, **default_kws)
 
     def run_data_extraction(self):
         """Run the raw dataset extraction process from disk to raw
         un-manipulated datasets.
 
         Includes a special method to extract clearsky_ghi from a exogenous
         NSRDB source h5 file (required to compute clearsky_ratio).
@@ -2496,15 +2547,15 @@
                 | (self.temporal_slice.step == 1)), msg
 
         with Resource(self._nsrdb_source_fp) as res:
             ti_nsrdb = res.time_index
             meta_nsrdb = res.meta
 
         ti_deltas = ti_nsrdb - np.roll(ti_nsrdb, 1)
-        ti_deltas_hours = ti_deltas.total_seconds()[1:-1] / 3600
+        ti_deltas_hours = pd.Series(ti_deltas).dt.total_seconds()[1:-1] / 3600
         time_freq = float(mode(ti_deltas_hours).mode[0])
         t_start = self.temporal_slice.start or 0
         t_end_target = self.temporal_slice.stop or len(self.raw_time_index)
         t_start = int(t_start * 24 * (1 / time_freq))
         t_end = int(t_end_target * 24 * (1 / time_freq))
         t_end = np.minimum(t_end, len(ti_nsrdb))
         t_slice = slice(t_start, t_end)
```

### Comparing `NREL-sup3r-0.0.9/sup3r/preprocessing/exogenous_data_handling.py` & `NREL-sup3r-0.1.0/sup3r/preprocessing/exogenous_data_handling.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Sup3r exogenous data handling"""
-
+import os
+import shutil
 import logging
 import numpy as np
+import pickle
 from warnings import warn
 
 from sup3r.utilities.topo import TopoExtractH5, TopoExtractNC
 import sup3r.preprocessing.data_handling
 import sup3r.utilities.topo
 from sup3r.utilities.utilities import get_source_type
 
@@ -16,15 +18,15 @@
     """Class to extract exogenous features for multistep forward passes. e.g.
     Multiple topography arrays at different resolutions for multiple spatial
     enhancement steps."""
 
     def __init__(self, file_paths, features, source_file, s_enhancements,
                  agg_factors, target=None, shape=None, raster_file=None,
                  max_delta=20, input_handler=None, topo_handler=None,
-                 exo_steps=None):
+                 exo_steps=None, cache_data=True):
         """
         Parameters
         ----------
         file_paths : str | list
             A single source h5 file or netcdf file to extract raster data from.
             The string can be a unix-style file path which will be passed
             through glob.glob. This is typically low-res WRF output or GCM
@@ -75,19 +77,31 @@
             match a class in topo.py. If None the correct handler will
             be guessed based on file type and time series properties.
         exo_steps : list
             List of model step indices for which exogenous data is required.
             e.g. If we have two model steps which take exo data and one which
             does not exo_steps = [0, 1]. The length of this list should be
             equal to the number of s_enhancements and the number of agg_factors
+        cache_data : bool
+            Flag to cache exogeneous data in ./exo_cache/ this can speed up
+            forward passes with large temporal extents
         """
 
         self.features = features
         self.s_enhancements = s_enhancements
         self.agg_factors = agg_factors
+        self.source_file = source_file
+        self.file_paths = file_paths
+        self.topo_handler = topo_handler
+        self.target = target
+        self.shape = shape
+        self.raster_file = raster_file
+        self.max_delta = max_delta
+        self.input_handler = input_handler
+        self.cache_data = cache_data
         self.data = []
         exo_steps = exo_steps or np.arange(len(self.s_enhancements))
 
         if self.s_enhancements[0] != 1:
             msg = ('s_enhancements typically starts with 1 so the first '
                    'exogenous data input matches the spatial resolution of '
                    'the source low-res input data, but received '
@@ -107,31 +121,72 @@
         for i in range(len(self.s_enhancements)):
             s_enhance = np.product(self.s_enhancements[:i + 1])
             agg_factor = self.agg_factors[i]
             fdata = []
             if i in exo_steps:
                 for f in features:
                     if f == 'topography':
-                        topo_handler = self.get_topo_handler(source_file,
-                                                             topo_handler)
-                        data = topo_handler(file_paths, source_file, s_enhance,
-                                            agg_factor, target=target,
-                                            shape=shape,
-                                            raster_file=raster_file,
-                                            max_delta=max_delta,
-                                            input_handler=input_handler)
-                        data = data.hr_elev
+                        data = self.get_topo_data(s_enhance, agg_factor)
                         fdata.append(data)
                     else:
                         msg = (f"Can only extract topography. Recived {f}.")
                         raise NotImplementedError(msg)
                 self.data.append(np.stack(fdata, axis=-1))
             else:
                 self.data.append(None)
 
+    def get_topo_data(self, s_enhance, agg_factor):
+        """Get the exogenous topography data
+
+        Parameters
+        ----------
+        s_enhance : int
+            Spatial enhancement for this exogeneous data step (cumulative for
+            all model steps up to the current step).
+        agg_factor : int
+            Factor by which to aggregate the topo_source_h5 elevation
+            data to the resolution of the file_paths input enhanced by
+            s_enhance.
+
+        Returns
+        -------
+        data : np.ndarray
+            2D array of elevation data with shape (lat, lon)
+        """
+
+        cache_dir = './exo_cache/'
+        fn = f'exo_{self.target}_{self.shape}_agg{agg_factor}_{s_enhance}x.pkl'
+        fn = fn.replace('(', '').replace(')', '')
+        fn = fn.replace('[', '').replace(']', '')
+        fn = fn.replace(',', 'x').replace(' ', '')
+        cache_fp = os.path.join(cache_dir, fn)
+        temp_fp = cache_fp + '.tmp'
+
+        if os.path.exists(cache_fp):
+            with open(cache_fp, 'rb') as f:
+                data = pickle.load(f)
+
+        else:
+            topo_handler = self.get_topo_handler(self.source_file,
+                                                 self.topo_handler)
+            data = topo_handler(self.file_paths, self.source_file, s_enhance,
+                                agg_factor, target=self.target,
+                                shape=self.shape,
+                                raster_file=self.raster_file,
+                                max_delta=self.max_delta,
+                                input_handler=self.input_handler)
+            data = data.hr_elev
+            if self.cache_data:
+                os.makedirs(cache_dir, exist_ok=True)
+                with open(temp_fp, 'wb') as f:
+                    pickle.dump(data, f)
+                shutil.move(temp_fp, cache_fp)
+
+        return data
+
     @staticmethod
     def get_topo_handler(source_file, topo_handler):
         """Get topo extraction class for source file
 
         Parameters
         ----------
         source_file : str
```

### Comparing `NREL-sup3r-0.0.9/sup3r/preprocessing/feature_handling.py` & `NREL-sup3r-0.1.0/sup3r/preprocessing/feature_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -977,68 +977,38 @@
         ndarray
             lat lon array
             (spatial_1, spatial_2, 2)
         """
 
         fp = file_paths if isinstance(file_paths, str) else file_paths[0]
         handle = xr.open_dataset(fp)
-        lat_key = 'XLAT'
-        lon_key = 'XLONG'
-        if lat_key not in handle.variables:
-            lat_key = 'latitude'
-        if lon_key not in handle.variables:
-            lon_key = 'longitude'
-        if len(handle.variables[lat_key].dims) == 3:
-            idx = (0, raster_index[0], raster_index[1])
-        elif len(handle.variables[lat_key].dims) == 4:
+        valid_vars = set(handle.variables)
+        lat_key = {'XLAT', 'lat', 'latitude'}.intersection(valid_vars)
+        lat_key = list(lat_key)[0]
+        lon_key = {'XLONG', 'lon', 'longitude'}.intersection(valid_vars)
+        lon_key = list(lon_key)[0]
+
+        if len(handle.variables[lat_key].dims) == 4:
             idx = (0, raster_index[0], raster_index[1], 0)
-        else:
+        elif len(handle.variables[lat_key].dims) == 3:
+            idx = (0, raster_index[0], raster_index[1])
+        elif len(handle.variables[lat_key].dims) == 2:
             idx = (raster_index[0], raster_index[1])
-        lats = handle.variables[lat_key].values[idx]
-        lons = handle.variables[lon_key].values[idx]
-        lat_lon = np.dstack((lats, lons))
-        return lat_lon
-
-
-class LatLonNCforCC:
-    """Lat Lon feature class with compute method"""
-
-    @staticmethod
-    def compute(file_paths, raster_index):
-        """Get lats and lons
 
-        Parameters
-        ----------
-        file_paths : list
-            path to data file
-        raster_index : list
-            List of slices for raster
-
-        Returns
-        -------
-        ndarray
-            lat lon array
-            (spatial_1, spatial_2, 2)
-        """
+        if len(handle.variables[lat_key].dims) == 1:
+            lons = handle.variables[lon_key].values
+            lats = handle.variables[lat_key].values
+            lons, lats = np.meshgrid(lons, lats)
+            lat_lon = np.dstack((lats[tuple(raster_index)],
+                                 lons[tuple(raster_index)]))
+        else:
+            lats = handle.variables[lat_key].values[idx]
+            lons = handle.variables[lon_key].values[idx]
+            lat_lon = np.dstack((lats, lons))
 
-        fp = file_paths if isinstance(file_paths, str) else file_paths[0]
-        handle = xr.open_dataset(fp)
-        lats = handle.lat.values
-        lons = handle.lon.values
-        if handle.lat.dims != ('lat',):
-            lats = lats[handle.lat.dims.index('lat')]
-        if handle.lon.dims != ('lon',):
-            lons = lons[handle.lon.dims.index('lon')]
-
-        assert len(lats.shape) == 1, f'Got bad lats shape: {lats.shape}'
-        assert len(lons.shape) == 1, f'Got bad lons shape: {lons.shape}'
-
-        lons, lats = np.meshgrid(lons, lats)
-        lat_lon = np.dstack((lats[tuple(raster_index)],
-                             lons[tuple(raster_index)]))
         return lat_lon
 
 
 class TopoH5:
     """Topography feature class with compute method"""
 
     @staticmethod
```

### Comparing `NREL-sup3r-0.0.9/sup3r/qa/qa.py` & `NREL-sup3r-0.1.0/sup3r/qa/qa.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/qa/qa_cli.py` & `NREL-sup3r-0.1.0/sup3r/qa/qa_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/qa/stats.py` & `NREL-sup3r-0.1.0/sup3r/qa/stats.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/qa/stats_cli.py` & `NREL-sup3r-0.1.0/sup3r/qa/stats_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/qa/utilities.py` & `NREL-sup3r-0.1.0/sup3r/qa/utilities.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/qa/visual_qa.py` & `NREL-sup3r-0.1.0/sup3r/qa/visual_qa.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/qa/visual_qa_cli.py` & `NREL-sup3r-0.1.0/sup3r/qa/visual_qa_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/solar/solar.py` & `NREL-sup3r-0.1.0/sup3r/solar/solar.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 as daily average GHI / daily average clearsky GHI.
 """
 import glob
 import json
 import os
 import numpy as np
 import logging
+import pandas as pd
 from scipy.spatial import KDTree
 from farms.disc import disc
 from farms.utilities import calc_dhi, dark_night
 from rex import Resource, MultiTimeResource
 from rex.utilities.fun_utils import get_fun_call_str
 
 from sup3r.utilities import ModuleName
@@ -118,15 +119,15 @@
         assert 'clearsky_dni' in self.nsrdb.dsets
         assert 'solar_zenith_angle' in self.nsrdb.dsets
         assert 'surface_pressure' in self.nsrdb.dsets
         assert isinstance(self.nsrdb_tslice, slice)
 
         ti_gan = self.gan_data.time_index
         ti_gan_1 = np.roll(ti_gan, 1)
-        delta = (ti_gan - ti_gan_1)[1:].mean().total_seconds()
+        delta = pd.Series(ti_gan - ti_gan_1)[1:].mean().total_seconds()
         msg = ('Its assumed that the sup3r GAN output solar data will be '
                'hourly but received time index: {}'.format(ti_gan))
         assert delta == 3600, msg
 
     def close(self):
         """Close all internal file handlers"""
         self.gan_data.close()
@@ -212,15 +213,15 @@
                 raise RuntimeError(msg)
 
             ilocs = np.where(mask)[0]
             t0, t1 = ilocs[0], ilocs[-1] + 1
 
             ti_nsrdb = self.nsrdb.time_index
             ti_nsrdb_1 = np.roll(ti_nsrdb, 1)
-            delta = (ti_nsrdb - ti_nsrdb_1)[1:].mean().total_seconds()
+            delta = pd.Series(ti_nsrdb - ti_nsrdb_1)[1:].mean().total_seconds()
             step = int(3600 // delta)
             self._nsrdb_tslice = slice(t0, t1, step)
 
             logger.debug('Found nsrdb_tslice {} with corresponding '
                          'time index:\n\t{}'
                          .format(self._nsrdb_tslice,
                                  self.nsrdb.time_index[self._nsrdb_tslice]))
```

### Comparing `NREL-sup3r-0.0.9/sup3r/solar/solar_cli.py` & `NREL-sup3r-0.1.0/sup3r/solar/solar_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/__init__.py` & `NREL-sup3r-0.1.0/sup3r/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/cli.py` & `NREL-sup3r-0.1.0/sup3r/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/execution.py` & `NREL-sup3r-0.1.0/sup3r/utilities/execution.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/loss_metrics.py` & `NREL-sup3r-0.1.0/sup3r/utilities/loss_metrics.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/plotting.py` & `NREL-sup3r-0.1.0/sup3r/utilities/plotting.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/pytest.py` & `NREL-sup3r-0.1.0/sup3r/utilities/pytest.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/regridder.py` & `NREL-sup3r-0.1.0/sup3r/utilities/regridder.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,39 +275,48 @@
 
         Parameters
         ----------
         distance_chunk : ndarray
             Chunk of the full array of distances where distances[i] gives the
             list of distances to the source coordinates to be used for
             interpolation for the i-th coordinate in the target data.
+            (temporal, n_points, k_neighbors)
         values : ndarray
             Array of values corresponding to the point distances with shape
             (temporal, n_points, k_neighbors)
 
         Returns
         -------
         ndarray
             Time series of values at interpolated point with shape
             (temporal, n_points)
         """
-        weights = 1 / np.array(distance_chunk)
+        dists = np.array(distance_chunk)
+        min_dist = 1e-12
+        mask = (dists < min_dist)
+        if mask.sum() > 0:
+            logger.info(f'{np.sum(mask)} of {np.product(mask.shape)} '
+                        'distances are zero.')
+        dists[mask] = min_dist
+        weights = 1 / dists
         norm = np.sum(weights, axis=-1)
         out = np.einsum('ijk,jk->ij', values, weights) / norm
         return out
 
     @classmethod
     def get_source_values(cls, index_chunk, feature, source_files):
         """Get values to use for interpolation
 
         Parameters
         ----------
         index_chunk : ndarray
             Chunk of the full array of indices where indices[i] gives the
             list of coordinate indices in the source data to be used for
             interpolation for the i-th coordinate in the target data.
+            (temporal, n_points, k_neighbors)
         feature : str
             Name of feature to interpolate
         source_files : list
             List of paths to source files
 
         Returns
         -------
@@ -335,14 +344,15 @@
 
         Parameters
         ----------
         index_chunk : ndarray
             Chunk of the full array of indices where indices[i] gives the
             list of coordinate indices in the source data to be used for
             interpolation for the i-th coordinate in the target data.
+            (temporal, n_points, k_neighbors)
         height : int
             Wind height level
         source_files : list
             List of paths to source files
 
         Returns
         -------
@@ -397,18 +407,20 @@
 
         Parameters
         ----------
         index_chunk : ndarray
             Chunk of the full array of indices where indices[i] gives the
             list of coordinate indices in the source data to be used for
             interpolation for the i-th coordinate in the target data.
+            (temporal, n_points, k_neighbors)
         distance_chunk : ndarray
             Chunk of the full array of distances where distances[i] gives the
             list of distances to the source coordinates to be used for
             interpolation for the i-th coordinate in the target data.
+            (temporal, n_points, k_neighbors)
         height : int
             Wind height level
         source_files : list
             List of paths to source files
 
         Returns
         -------
```

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/regridder_cli.py` & `NREL-sup3r-0.1.0/sup3r/utilities/regridder_cli.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/stitching.py` & `NREL-sup3r-0.1.0/sup3r/utilities/stitching.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/topo.py` & `NREL-sup3r-0.1.0/sup3r/utilities/topo.py`

 * *Files identical despite different names*

### Comparing `NREL-sup3r-0.0.9/sup3r/utilities/utilities.py` & `NREL-sup3r-0.1.0/sup3r/utilities/utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,30 +5,54 @@
 """
 
 import numpy as np
 import logging
 import glob
 from scipy import ndimage as nd
 from scipy.interpolate import RegularGridInterpolator
-from scipy.ndimage.filters import gaussian_filter
 from scipy.interpolate import interp1d
-from scipy.ndimage import interpolation
+from scipy.ndimage import zoom
+from scipy.ndimage.filters import gaussian_filter
 from fnmatch import fnmatch
 import os
 import re
 from warnings import warn
 import psutil
 import pandas as pd
 from packaging import version
+import xarray as xr
 
 np.random.seed(42)
 
 logger = logging.getLogger(__name__)
 
 
+def get_time_dim_name(filepath):
+    """Get the name of the time dimension in the given file. This is
+    specifically for netcdf files.
+
+    Parameters
+    ----------
+    filepath : str
+        Path to the file
+
+    Returns
+    -------
+    time_key : str
+        Name of the time dimension in the given file
+    """
+    with xr.open_dataset(filepath) as handle:
+        valid_vars = set(handle.dims)
+        time_key = list({'time', 'Time'}.intersection(valid_vars))
+    if len(time_key) > 0:
+        return time_key[0]
+    else:
+        return 'time'
+
+
 def correct_path(path):
     """If running on windows we need to replace backslashes with double
     backslashes so paths can be parsed correctly with safe_open_json"""
     return path.replace('\\', '\\\\')
 
 
 def estimate_max_workers(max_workers, process_mem, n_processes):
@@ -607,15 +631,15 @@
 
     else:
         coarse_data = data
 
     return coarse_data
 
 
-def temporal_simple_enhancing(data, t_enhance=4):
+def temporal_simple_enhancing(data, t_enhance=4, mode='constant'):
     """"Upsample data according to t_enhance resolution
 
     Parameters
     ----------
     data : np.ndarray
         5D array with dimensions
         (observations, spatial_1, spatial_2, temporal, features)
@@ -627,18 +651,29 @@
     enhanced_data : np.ndarray
         5D array with same dimensions as data with new enhanced resolution
     """
 
     if t_enhance in [None, 1]:
         enhanced_data = data
     elif t_enhance not in [None, 1] and len(data.shape) == 5:
-        enhancement = [1, 1, 1, t_enhance, 1]
-        enhanced_data = interpolation.zoom(data,
-                                           enhancement,
-                                           order=0)
+        if mode == 'constant':
+            enhancement = [1, 1, 1, t_enhance, 1]
+            enhanced_data = zoom(data,
+                                 enhancement,
+                                 order=0,
+                                 mode='nearest',
+                                 grid_mode=True)
+        elif mode == 'linear':
+            index_t_hr = np.array(list(range(data.shape[3] * t_enhance)))
+            index_t_lr = index_t_hr[::t_enhance]
+            enhanced_data = interp1d(index_t_lr,
+                                     data,
+                                     axis=3,
+                                     fill_value='extrapolate')(index_t_hr)
+            enhanced_data = np.array(enhanced_data, dtype=np.float32)
     elif len(data.shape) != 5:
         msg = ('Data must be 5D to do temporal enhancing, but '
                f'received: {data.shape}')
         logger.error(msg)
         raise ValueError(msg)
 
     return enhanced_data
@@ -828,35 +863,43 @@
         logger.error(msg)
         raise ValueError(msg)
 
     if s_enhance is not None and s_enhance > 1:
 
         if obs_axis and len(data.shape) == 5:
             enhancement = [1, s_enhance, s_enhance, 1, 1]
-            enhanced_data = interpolation.zoom(data,
-                                               enhancement,
-                                               order=0)
+            enhanced_data = zoom(data,
+                                 enhancement,
+                                 order=0,
+                                 mode='nearest',
+                                 grid_mode=True)
 
         elif obs_axis and len(data.shape) == 4:
             enhancement = [1, s_enhance, s_enhance, 1]
-            enhanced_data = interpolation.zoom(data,
-                                               enhancement,
-                                               order=0)
+            enhanced_data = zoom(data,
+                                 enhancement,
+                                 order=0,
+                                 mode='nearest',
+                                 grid_mode=True)
 
         elif not obs_axis and len(data.shape) == 4:
             enhancement = [s_enhance, s_enhance, 1, 1]
-            enhanced_data = interpolation.zoom(data,
-                                               enhancement,
-                                               order=0)
+            enhanced_data = zoom(data,
+                                 enhancement,
+                                 order=0,
+                                 mode='nearest',
+                                 grid_mode=True)
 
         elif not obs_axis and len(data.shape) == 3:
             enhancement = [s_enhance, s_enhance, 1]
-            enhanced_data = interpolation.zoom(data,
-                                               enhancement,
-                                               order=0)
+            enhanced_data = zoom(data,
+                                 enhancement,
+                                 order=0,
+                                 mode='nearest',
+                                 grid_mode=True)
         else:
             msg = ('Data must be 3D, 4D, or 5D to do spatial enhancing, but '
                    f'received: {data.shape}')
             logger.error(msg)
             raise ValueError(msg)
 
     else:
@@ -902,347 +945,14 @@
     -------
     ndarray
         Array of average values, length will be 1 less than array_in
     """
     return (array_in[:-1] + array_in[1:]) * 0.5
 
 
-def extract_var(data, var, raster_index, time_slice=slice(None)):
-    """Extract WRF variable values. This is meant to extract values from
-    fields without staggered dimensions
-
-    Parameters
-    ----------
-    data : xarray
-        netcdf data object
-    var : str
-        Name of variable to be extracted
-    raster_index : list
-        List of slices for raster index of spatial domain
-    time_slice : slice
-        slice of time to extract
-
-    Returns
-    -------
-    ndarray
-        Extracted array of variable values.
-    """
-
-    idx = [time_slice, slice(None), raster_index[0], raster_index[1]]
-
-    assert not any('stag' in d for d in data[var].dims)
-
-    return np.array(data[var][tuple(idx)], dtype=np.float32)
-
-
-def unstagger_var(data, var, raster_index, time_slice=slice(None)):
-    """Unstagger WRF variable values. Some variables use a staggered grid with
-    values associated with grid cell edges. We want to center these values.
-
-    Parameters
-    ----------
-    data : xarray
-        netcdf data object
-    var : str
-        Name of variable to be unstaggered
-    raster_index : list
-        List of slices for raster index of spatial domain
-    time_slice : slice
-        slice of time to extract
-
-    Returns
-    -------
-    ndarray
-        Unstaggered array of variable values.
-    """
-
-    idx = [time_slice, slice(None), raster_index[0], raster_index[1]]
-    assert any('stag' in d for d in data[var].dims)
-
-    if 'stag' in data[var].dims[2]:
-        idx[2] = slice(idx[2].start, idx[2].stop + 1)
-    if 'stag' in data[var].dims[3]:
-        idx[3] = slice(idx[3].start, idx[3].stop + 1)
-
-    array_in = np.array(data[var][tuple(idx)], dtype=np.float32)
-
-    for i, d in enumerate(data[var].dims):
-        if 'stag' in d:
-            array_in = np.apply_along_axis(forward_average, i, array_in)
-
-    return array_in
-
-
-def calc_height(data, raster_index, time_slice=slice(None)):
-    """Calculate height from the ground
-
-    Parameters
-    ----------
-    data : xarray
-        netcdf data object
-    raster_index : list
-        List of slices for raster index of spatial domain
-    time_slice : slice
-        slice of time to extract
-
-    Returns
-    -------
-    height_arr : ndarray
-        (temporal, vertical_level, spatial_1, spatial_2)
-        4D array of heights above ground. In meters.
-    """
-    if all(field in data for field in ('PHB', 'PH', 'HGT')):
-        # Base-state Geopotential(m^2/s^2)
-        if any('stag' in d for d in data['PHB'].dims):
-            gp = unstagger_var(data, 'PHB', raster_index, time_slice)
-        else:
-            gp = extract_var(data, 'PHB', raster_index, time_slice)
-
-        # Perturbation Geopotential (m^2/s^2)
-        if any('stag' in d for d in data['PH'].dims):
-            gp += unstagger_var(data, 'PH', raster_index, time_slice)
-        else:
-            gp += extract_var(data, 'PH', raster_index, time_slice)
-
-        # Terrain Height (m)
-        hgt = data['HGT'][(time_slice,) + tuple(raster_index)]
-        if gp.shape != hgt.shape:
-            hgt = np.repeat(np.expand_dims(hgt, axis=1), gp.shape[-3], axis=1)
-        hgt = gp / 9.81 - hgt
-        del gp
-
-    elif all(field in data for field in ('zg', 'orog')):
-        gp = data['zg'][(time_slice, slice(None),) + tuple(raster_index)]
-        hgt = data['orog'][tuple(raster_index)]
-        hgt = np.repeat(np.expand_dims(hgt, axis=0), gp.shape[1], axis=0)
-        hgt = np.repeat(np.expand_dims(hgt, axis=0), gp.shape[0], axis=0)
-        hgt = gp - hgt
-        del gp
-
-    else:
-        msg = ('Need either PHB/PH/HGT or zg/orog in data to perform height '
-               'interpolation')
-        raise ValueError(msg)
-    return np.array(hgt)
-
-
-def calc_pressure(data, var, raster_index, time_slice=slice(None)):
-    """Calculate pressure array
-
-    Parameters
-    ----------
-    data : xarray
-        netcdf data object
-    var : str
-        Feature to extract from data
-    raster_index : list
-        List of slices for raster index of spatial domain
-    time_slice : slice
-        slice of time to extract
-
-    Returns
-    -------
-    height_arr : ndarray
-        (temporal, vertical_level, spatial_1, spatial_2)
-        4D array of pressure levels in pascals
-    """
-    idx = (time_slice, slice(None),) + tuple(raster_index)
-    p_array = np.zeros(data[var][idx].shape, dtype=np.float32)
-    for i in range(p_array.shape[1]):
-        p_array[:, i, ...] = data.plev[i]
-
-    return p_array
-
-
-def interp_to_level(var_array, lev_array, levels):
-    """Interpolate var_array to given level(s) based on h_array. Interpolation
-    is linear and done for every 'z' column of [var, h] data.
-
-    Parameters
-    ----------
-    var_array : ndarray
-        Array of variable data, for example u-wind in a 4D array of shape
-        (time, vertical, lat, lon)
-    lev_array : ndarray
-        Array of height or pressure values corresponding to the wrf source data
-        in the same shape as var_array. If this is height and the requested
-        levels are input is a hub height above surface, lev_array should be the
-        geopotential height corresponding to every var_array index relative to
-        the surface elevation (subtract the elevation at the surface from the
-        geopotential height)
-    levels : float | list
-        level or levels to interpolate to (e.g. final desired hub heights above
-        surface elevation)
-
-    Returns
-    -------
-    out_array : ndarray
-        Array of interpolated values.
-    """
-
-    msg = ('Input arrays must be the same shape.'
-           f'\nvar_array: {var_array.shape}'
-           f'\nh_array: {lev_array.shape}')
-    assert var_array.shape == lev_array.shape, msg
-
-    levels = ([levels] if isinstance(levels, (int, float, np.float32))
-              else levels)
-
-    if np.isnan(lev_array).all():
-        msg = 'All pressure level height data is NaN!'
-        logger.error(msg)
-        raise RuntimeError(msg)
-
-    nans = np.isnan(lev_array)
-    bad_min = min(levels) < lev_array[:, 0, :, :]
-    bad_max = max(levels) > lev_array[:, -1, :, :]
-
-    if nans.any():
-        msg = ('Approximately {:.2f}% of the vertical level '
-               'array is NaN. Data will be interpolated or extrapolated '
-               'past these NaN values.'
-               .format(100 * nans.sum() / nans.size))
-        logger.warning(msg)
-        warn(msg)
-
-    if bad_min.any():
-        msg = ('Approximately {:.2f}% of the lowest vertical levels '
-               '(maximum value of {:.3f}) '
-               'were greater than the minimum requested level: {}'
-               .format(100 * bad_min.sum() / bad_min.size,
-                       lev_array[:, 0, :, :].max(), min(levels)))
-        logger.warning(msg)
-        warn(msg)
-
-    if bad_max.any():
-        msg = ('Approximately {:.2f}% of the highest vertical levels '
-               '(minimum value of {:.3f}) '
-               'were lower than the maximum requested level: {}'
-               .format(100 * bad_max.sum() / bad_max.size,
-                       lev_array[:, -1, :, :].min(), max(levels)))
-        logger.warning(msg)
-        warn(msg)
-
-    array_shape = var_array.shape
-
-    # Flatten h_array and var_array along lat, long axis
-    shape = (len(levels), array_shape[-4], np.product(array_shape[-2:]))
-    out_array = np.zeros(shape, dtype=np.float32).T
-
-    # if multiple vertical levels have identical heights at the desired
-    # interpolation level, interpolation to that value will fail because linear
-    # slope will be NaN. This is most common if you have multiple pressure
-    # levels at zero height at the surface in the case that the data didnt
-    # provide underground data.
-    for level in levels:
-        mask = (lev_array == level)
-        lev_array[mask] += np.random.uniform(-1e-5, 0, size=mask.sum())
-
-    # iterate through time indices
-    for idt in range(array_shape[0]):
-        shape = (array_shape[-3], np.product(array_shape[-2:]))
-        h_tmp = lev_array[idt].reshape(shape).T
-        var_tmp = var_array[idt].reshape(shape).T
-        not_nan = ~np.isnan(h_tmp) & ~np.isnan(var_tmp)
-
-        # Interp each vertical column of height and var to requested levels
-        zip_iter = zip(h_tmp, var_tmp, not_nan)
-        out_array[:, idt, :] = np.array(
-            [interp1d(h[mask], var[mask], fill_value='extrapolate')(levels)
-             for h, var, mask in zip_iter], dtype=np.float32)
-
-    # Reshape out_array
-    if isinstance(levels, (float, np.float32, int)):
-        shape = (1, array_shape[-4], array_shape[-2], array_shape[-1])
-        out_array = out_array.T.reshape(shape)
-    else:
-        shape = (len(levels), array_shape[-4], array_shape[-2],
-                 array_shape[-1])
-        out_array = out_array.T.reshape(shape)
-
-    return out_array
-
-
-def interp_var_to_height(data, var, raster_index, heights,
-                         time_slice=slice(None)):
-    """Interpolate var_array to given level(s) based on h_array. Interpolation
-    is linear and done for every 'z' column of [var, h] data.
-
-    Parameters
-    ----------
-    data : xarray
-        netcdf data object
-    var : str
-        Name of variable to be interpolated
-    raster_index : list
-        List of slices for raster index of spatial domain
-    heights : float | list
-        level or levels to interpolate to (e.g. final desired hub heights)
-    time_slice : slice
-        slice of time to extract
-
-    Returns
-    -------
-    out_array : ndarray
-        Array of interpolated values.
-    """
-    if len(data[var].dims) == 5:
-        raster_index = [0] + raster_index
-    logger.debug(f'Interpolating {var} to heights (meters): {heights}')
-    hgt = calc_height(data, raster_index, time_slice)
-    if data[var].dims == ('plev',):
-        arr = np.array(data[var])
-        arr = np.expand_dims(arr, axis=(0, 2, 3))
-        arr = np.repeat(arr, hgt.shape[0], axis=0)
-        arr = np.repeat(arr, hgt.shape[2], axis=2)
-        arr = np.repeat(arr, hgt.shape[3], axis=3)
-    elif all('stag' not in d for d in data[var].dims):
-        arr = extract_var(data, var, raster_index, time_slice)
-    else:
-        arr = unstagger_var(data, var, raster_index, time_slice)
-    return interp_to_level(arr, hgt, heights)[0]
-
-
-def interp_var_to_pressure(data, var, raster_index, pressures,
-                           time_slice=slice(None)):
-    """Interpolate var_array to given level(s) based on h_array. Interpolation
-    is linear and done for every 'z' column of [var, h] data.
-
-    Parameters
-    ----------
-    data : xarray
-        netcdf data object
-    var : str
-        Name of variable to be interpolated
-    raster_index : list
-        List of slices for raster index of spatial domain
-    pressures : float | list
-        level or levels to interpolate to (e.g. final desired hub heights)
-    time_slice : slice
-        slice of time to extract
-
-    Returns
-    -------
-    out_array : ndarray
-        Array of interpolated values.
-    """
-    logger.debug(f'Interpolating {var} to pressures (Pa): {pressures}')
-    if len(data[var].dims) == 5:
-        raster_index = [0] + raster_index
-
-    if all('stag' not in d for d in data[var].dims):
-        arr = extract_var(data, var, raster_index, time_slice)
-    else:
-        arr = unstagger_var(data, var, raster_index, time_slice)
-
-    p_levels = calc_pressure(data, var, raster_index, time_slice)
-
-    return interp_to_level(arr[:, ::-1], p_levels[:, ::-1], pressures)[0]
-
-
 def potential_temperature(T, P):
     """Potential temperature of fluid at pressure P and temperature T
 
     Parameters
     ----------
     T : ndarray
         Temperature in celsius
```

