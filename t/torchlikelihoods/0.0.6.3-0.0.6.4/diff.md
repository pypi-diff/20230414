# Comparing `tmp/torchlikelihoods-0.0.6.3.tar.gz` & `tmp/torchlikelihoods-0.0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlikelihoods-0.0.6.3.tar", last modified: Wed Jan 18 11:42:50 2023, max compression
+gzip compressed data, was "torchlikelihoods-0.0.6.4.tar", last modified: Fri Apr 14 13:24:59 2023, max compression
```

## Comparing `torchlikelihoods-0.0.6.3.tar` & `torchlikelihoods-0.0.6.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-01-18 11:42:50.773589 torchlikelihoods-0.0.6.3/
--rw-r--r--   0 psanchez  (7328)     1040     1079 2022-12-07 09:05:42.000000 torchlikelihoods-0.0.6.3/LICENSE
--rw-r--r--   0 psanchez  (7328)     1040       42 2022-12-08 20:11:28.000000 torchlikelihoods-0.0.6.3/MANIFEST.in
--rw-r--r--   0 psanchez  (7328)     1040     1697 2023-01-18 11:42:50.773114 torchlikelihoods-0.0.6.3/PKG-INFO
--rw-r--r--   0 psanchez  (7328)     1040      655 2022-12-30 19:16:36.000000 torchlikelihoods-0.0.6.3/README.md
--rw-r--r--   0 psanchez  (7328)     1040        0 2022-12-08 20:01:21.000000 torchlikelihoods-0.0.6.3/conftest.py
-drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-01-18 11:42:50.754389 torchlikelihoods-0.0.6.3/examples/
--rw-r--r--   0 psanchez  (7328)     1040        0 2022-12-09 12:45:23.000000 torchlikelihoods-0.0.6.3/examples/__init__.py
--rw-r--r--   0 psanchez  (7328)     1040     1019 2022-12-31 18:50:44.000000 torchlikelihoods-0.0.6.3/examples/playground.py
--rw-r--r--   0 psanchez  (7328)     1040       38 2023-01-18 11:42:50.773782 torchlikelihoods-0.0.6.3/setup.cfg
--rw-r--r--   0 psanchez  (7328)     1040     1738 2022-12-08 20:13:18.000000 torchlikelihoods-0.0.6.3/setup.py
-drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-01-18 11:42:50.757434 torchlikelihoods-0.0.6.3/tests/
--rw-r--r--   0 psanchez  (7328)     1040        0 2022-12-08 19:50:58.000000 torchlikelihoods-0.0.6.3/tests/__init__.py
--rw-r--r--   0 psanchez  (7328)     1040     1719 2022-12-08 23:31:58.000000 torchlikelihoods-0.0.6.3/tests/test_categorical.py
--rw-r--r--   0 psanchez  (7328)     1040     3285 2022-12-09 12:12:56.000000 torchlikelihoods-0.0.6.3/tests/test_distr_heterogeneous.py
--rw-r--r--   0 psanchez  (7328)     1040     1373 2022-12-09 12:35:46.000000 torchlikelihoods-0.0.6.3/tests/test_lik_heterogeneous.py
--rw-r--r--   0 psanchez  (7328)     1040     2409 2022-12-09 12:22:01.000000 torchlikelihoods-0.0.6.3/tests/test_scaler_heterogeneous.py
--rw-r--r--   0 psanchez  (7328)     1040     4634 2022-12-31 09:27:09.000000 torchlikelihoods-0.0.6.3/tests/test_scaler_heterogeneous_object.py
--rw-r--r--   0 psanchez  (7328)     1040     5503 2023-01-18 11:41:21.000000 torchlikelihoods-0.0.6.3/tests/test_scaler_minmax.py
--rw-r--r--   0 psanchez  (7328)     1040     2667 2022-12-12 13:57:36.000000 torchlikelihoods-0.0.6.3/tests/test_scaler_standard.py
-drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-01-18 11:42:50.758084 torchlikelihoods-0.0.6.3/tests/utils/
--rw-r--r--   0 psanchez  (7328)     1040        0 2022-12-09 09:48:12.000000 torchlikelihoods-0.0.6.3/tests/utils/__init__.py
--rw-r--r--   0 psanchez  (7328)     1040     1780 2022-12-31 09:26:39.000000 torchlikelihoods-0.0.6.3/tests/utils/mock_data.py
-drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-01-18 11:42:50.758442 torchlikelihoods-0.0.6.3/torchlikelihoods/
--rw-r--r--   0 psanchez  (7328)     1040       74 2023-01-18 11:42:24.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/__init__.py
-drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-01-18 11:42:50.761302 torchlikelihoods-0.0.6.3/torchlikelihoods/distributions/
--rw-r--r--   0 psanchez  (7328)     1040       77 2022-12-09 12:43:36.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/distributions/__init__.py
--rw-r--r--   0 psanchez  (7328)     1040      846 2022-12-09 12:53:00.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/distributions/delta.py
--rw-r--r--   0 psanchez  (7328)     1040     4636 2022-12-09 09:31:51.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/distributions/heterogeneous.py
-drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-01-18 11:42:50.764838 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/
--rw-r--r--   0 psanchez  (7328)     1040      836 2022-12-12 13:51:41.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/__init__.py
--rw-r--r--   0 psanchez  (7328)     1040     1801 2022-12-09 12:37:06.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/base.py
--rw-r--r--   0 psanchez  (7328)     1040      627 2022-12-08 20:03:59.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/bernoulli.py
--rw-r--r--   0 psanchez  (7328)     1040      977 2022-12-08 20:02:18.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/beta.py
--rw-r--r--   0 psanchez  (7328)     1040      642 2022-12-09 12:08:47.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/categorical.py
--rw-r--r--   0 psanchez  (7328)     1040      643 2022-12-08 20:03:59.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/continous_bernoulli.py
--rw-r--r--   0 psanchez  (7328)     1040      894 2022-12-09 12:43:36.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/delta.py
--rw-r--r--   0 psanchez  (7328)     1040     1383 2022-12-09 12:36:27.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/heterogeneous.py
--rw-r--r--   0 psanchez  (7328)     1040     1077 2022-12-08 20:03:59.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/normal.py
--rw-r--r--   0 psanchez  (7328)     1040      920 2022-12-12 13:51:04.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/normal_mean.py
-drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-01-18 11:42:50.771068 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/
--rw-r--r--   0 psanchez  (7328)     1040      577 2023-01-18 10:54:16.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/__init__.py
--rw-r--r--   0 psanchez  (7328)     1040     2953 2023-01-16 14:03:55.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/base.py
--rw-r--r--   0 psanchez  (7328)     1040     2125 2023-01-16 14:29:50.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/heterogeneous.py
--rw-r--r--   0 psanchez  (7328)     1040     2674 2023-01-16 14:29:50.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/heterogeneous_object.py
--rw-r--r--   0 psanchez  (7328)     1040      484 2023-01-16 14:29:49.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/identity.py
--rw-r--r--   0 psanchez  (7328)     1040     1152 2023-01-16 14:29:49.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/min.py
--rw-r--r--   0 psanchez  (7328)     1040     2263 2023-01-18 11:42:03.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/minmax.py
--rw-r--r--   0 psanchez  (7328)     1040      948 2023-01-16 14:29:50.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/scale.py
--rw-r--r--   0 psanchez  (7328)     1040      790 2023-01-16 14:29:50.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/scalediff.py
--rw-r--r--   0 psanchez  (7328)     1040     1289 2023-01-16 14:29:50.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/standard.py
-drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-01-18 11:42:50.772146 torchlikelihoods-0.0.6.3/torchlikelihoods/utils/
--rw-r--r--   0 psanchez  (7328)     1040        0 2022-12-30 22:17:06.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/utils/__init__.py
--rw-r--r--   0 psanchez  (7328)     1040      799 2022-12-30 22:22:25.000000 torchlikelihoods-0.0.6.3/torchlikelihoods/utils/struct.py
-drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-01-18 11:42:50.760192 torchlikelihoods-0.0.6.3/torchlikelihoods.egg-info/
--rw-r--r--   0 psanchez  (7328)     1040     1697 2023-01-18 11:42:50.000000 torchlikelihoods-0.0.6.3/torchlikelihoods.egg-info/PKG-INFO
--rw-r--r--   0 psanchez  (7328)     1040     1609 2023-01-18 11:42:50.000000 torchlikelihoods-0.0.6.3/torchlikelihoods.egg-info/SOURCES.txt
--rw-r--r--   0 psanchez  (7328)     1040        1 2023-01-18 11:42:50.000000 torchlikelihoods-0.0.6.3/torchlikelihoods.egg-info/dependency_links.txt
--rw-r--r--   0 psanchez  (7328)     1040       43 2023-01-18 11:42:50.000000 torchlikelihoods-0.0.6.3/torchlikelihoods.egg-info/requires.txt
--rw-r--r--   0 psanchez  (7328)     1040       32 2023-01-18 11:42:50.000000 torchlikelihoods-0.0.6.3/torchlikelihoods.egg-info/top_level.txt
+drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-04-14 13:24:59.525864 torchlikelihoods-0.0.6.4/
+-rw-r--r--   0 psanchez  (7328)     1040     1079 2022-12-07 09:05:42.000000 torchlikelihoods-0.0.6.4/LICENSE
+-rw-r--r--   0 psanchez  (7328)     1040       42 2022-12-08 20:11:28.000000 torchlikelihoods-0.0.6.4/MANIFEST.in
+-rw-r--r--   0 psanchez  (7328)     1040     1697 2023-04-14 13:24:59.525595 torchlikelihoods-0.0.6.4/PKG-INFO
+-rw-r--r--   0 psanchez  (7328)     1040      655 2022-12-30 19:16:36.000000 torchlikelihoods-0.0.6.4/README.md
+-rw-r--r--   0 psanchez  (7328)     1040        0 2022-12-08 20:01:21.000000 torchlikelihoods-0.0.6.4/conftest.py
+drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-04-14 13:24:59.509388 torchlikelihoods-0.0.6.4/examples/
+-rw-r--r--   0 psanchez  (7328)     1040        0 2022-12-09 12:45:23.000000 torchlikelihoods-0.0.6.4/examples/__init__.py
+-rw-r--r--   0 psanchez  (7328)     1040     1019 2022-12-31 18:50:44.000000 torchlikelihoods-0.0.6.4/examples/playground.py
+-rw-r--r--   0 psanchez  (7328)     1040       38 2023-04-14 13:24:59.525973 torchlikelihoods-0.0.6.4/setup.cfg
+-rw-r--r--   0 psanchez  (7328)     1040     1738 2022-12-08 20:13:18.000000 torchlikelihoods-0.0.6.4/setup.py
+drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-04-14 13:24:59.511825 torchlikelihoods-0.0.6.4/tests/
+-rw-r--r--   0 psanchez  (7328)     1040        0 2022-12-08 19:50:58.000000 torchlikelihoods-0.0.6.4/tests/__init__.py
+-rw-r--r--   0 psanchez  (7328)     1040     1719 2022-12-08 23:31:58.000000 torchlikelihoods-0.0.6.4/tests/test_categorical.py
+-rw-r--r--   0 psanchez  (7328)     1040     3285 2022-12-09 12:12:56.000000 torchlikelihoods-0.0.6.4/tests/test_distr_heterogeneous.py
+-rw-r--r--   0 psanchez  (7328)     1040     1373 2022-12-09 12:35:46.000000 torchlikelihoods-0.0.6.4/tests/test_lik_heterogeneous.py
+-rw-r--r--   0 psanchez  (7328)     1040     2409 2022-12-09 12:22:01.000000 torchlikelihoods-0.0.6.4/tests/test_scaler_heterogeneous.py
+-rw-r--r--   0 psanchez  (7328)     1040     4634 2022-12-31 09:27:09.000000 torchlikelihoods-0.0.6.4/tests/test_scaler_heterogeneous_object.py
+-rw-r--r--   0 psanchez  (7328)     1040     5503 2023-01-18 11:41:21.000000 torchlikelihoods-0.0.6.4/tests/test_scaler_minmax.py
+-rw-r--r--   0 psanchez  (7328)     1040     2667 2022-12-12 13:57:36.000000 torchlikelihoods-0.0.6.4/tests/test_scaler_standard.py
+drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-04-14 13:24:59.512406 torchlikelihoods-0.0.6.4/tests/utils/
+-rw-r--r--   0 psanchez  (7328)     1040        0 2022-12-09 09:48:12.000000 torchlikelihoods-0.0.6.4/tests/utils/__init__.py
+-rw-r--r--   0 psanchez  (7328)     1040     1780 2022-12-31 09:26:39.000000 torchlikelihoods-0.0.6.4/tests/utils/mock_data.py
+drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-04-14 13:24:59.512844 torchlikelihoods-0.0.6.4/torchlikelihoods/
+-rw-r--r--   0 psanchez  (7328)     1040       74 2023-04-14 13:24:34.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/__init__.py
+drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-04-14 13:24:59.515772 torchlikelihoods-0.0.6.4/torchlikelihoods/distributions/
+-rw-r--r--   0 psanchez  (7328)     1040       77 2022-12-09 12:43:36.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/distributions/__init__.py
+-rw-r--r--   0 psanchez  (7328)     1040      846 2022-12-09 12:53:00.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/distributions/delta.py
+-rw-r--r--   0 psanchez  (7328)     1040     4636 2022-12-09 09:31:51.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/distributions/heterogeneous.py
+drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-04-14 13:24:59.520051 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/
+-rw-r--r--   0 psanchez  (7328)     1040      899 2023-04-14 13:23:33.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/__init__.py
+-rw-r--r--   0 psanchez  (7328)     1040     1801 2022-12-09 12:37:06.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/base.py
+-rw-r--r--   0 psanchez  (7328)     1040      627 2022-12-08 20:03:59.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/bernoulli.py
+-rw-r--r--   0 psanchez  (7328)     1040      977 2022-12-08 20:02:18.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/beta.py
+-rw-r--r--   0 psanchez  (7328)     1040      642 2022-12-09 12:08:47.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/categorical.py
+-rw-r--r--   0 psanchez  (7328)     1040      643 2022-12-08 20:03:59.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/continous_bernoulli.py
+-rw-r--r--   0 psanchez  (7328)     1040      894 2022-12-09 12:43:36.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/delta.py
+-rw-r--r--   0 psanchez  (7328)     1040     1383 2022-12-09 12:36:27.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/heterogeneous.py
+-rw-r--r--   0 psanchez  (7328)     1040     1077 2022-12-08 20:03:59.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/normal.py
+-rw-r--r--   0 psanchez  (7328)     1040      920 2022-12-12 13:51:04.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/normal_mean.py
+drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-04-14 13:24:59.524482 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/
+-rw-r--r--   0 psanchez  (7328)     1040      577 2023-01-18 10:54:16.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/__init__.py
+-rw-r--r--   0 psanchez  (7328)     1040     2953 2023-01-16 14:03:55.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/base.py
+-rw-r--r--   0 psanchez  (7328)     1040     2125 2023-01-16 14:29:50.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/heterogeneous.py
+-rw-r--r--   0 psanchez  (7328)     1040     2674 2023-01-16 14:29:50.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/heterogeneous_object.py
+-rw-r--r--   0 psanchez  (7328)     1040      484 2023-01-16 14:29:49.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/identity.py
+-rw-r--r--   0 psanchez  (7328)     1040     1152 2023-01-16 14:29:49.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/min.py
+-rw-r--r--   0 psanchez  (7328)     1040     2263 2023-01-18 11:42:03.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/minmax.py
+-rw-r--r--   0 psanchez  (7328)     1040      948 2023-01-16 14:29:50.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/scale.py
+-rw-r--r--   0 psanchez  (7328)     1040      790 2023-01-16 14:29:50.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/scalediff.py
+-rw-r--r--   0 psanchez  (7328)     1040     1289 2023-01-16 14:29:50.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/standard.py
+drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-04-14 13:24:59.525181 torchlikelihoods-0.0.6.4/torchlikelihoods/utils/
+-rw-r--r--   0 psanchez  (7328)     1040        0 2022-12-30 22:17:06.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/utils/__init__.py
+-rw-r--r--   0 psanchez  (7328)     1040      799 2022-12-30 22:22:25.000000 torchlikelihoods-0.0.6.4/torchlikelihoods/utils/struct.py
+drwxr-xr-x   0 psanchez  (7328)     1040        0 2023-04-14 13:24:59.514792 torchlikelihoods-0.0.6.4/torchlikelihoods.egg-info/
+-rw-r--r--   0 psanchez  (7328)     1040     1697 2023-04-14 13:24:59.000000 torchlikelihoods-0.0.6.4/torchlikelihoods.egg-info/PKG-INFO
+-rw-r--r--   0 psanchez  (7328)     1040     1609 2023-04-14 13:24:59.000000 torchlikelihoods-0.0.6.4/torchlikelihoods.egg-info/SOURCES.txt
+-rw-r--r--   0 psanchez  (7328)     1040        1 2023-04-14 13:24:59.000000 torchlikelihoods-0.0.6.4/torchlikelihoods.egg-info/dependency_links.txt
+-rw-r--r--   0 psanchez  (7328)     1040       43 2023-04-14 13:24:59.000000 torchlikelihoods-0.0.6.4/torchlikelihoods.egg-info/requires.txt
+-rw-r--r--   0 psanchez  (7328)     1040       32 2023-04-14 13:24:59.000000 torchlikelihoods-0.0.6.4/torchlikelihoods.egg-info/top_level.txt
```

### Comparing `torchlikelihoods-0.0.6.3/LICENSE` & `torchlikelihoods-0.0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/PKG-INFO` & `torchlikelihoods-0.0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlikelihoods
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: TorchLikelihoods: User-friendly handling of likelihoods in Pytorch
 Home-page: https://github.com/psanch21/torchlikelihoods
 Author: Pablo Sanchez Martin
 Author-email: psanch2103@gmail.com
 License: MIT
 Keywords: Distributions,Likelihoods,Heterogeneous Data,Pytorch,Scalers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchlikelihoods-0.0.6.3/README.md` & `torchlikelihoods-0.0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/examples/playground.py` & `torchlikelihoods-0.0.6.4/examples/playground.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/setup.py` & `torchlikelihoods-0.0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/tests/test_categorical.py` & `torchlikelihoods-0.0.6.4/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/tests/test_distr_heterogeneous.py` & `torchlikelihoods-0.0.6.4/tests/test_distr_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/tests/test_lik_heterogeneous.py` & `torchlikelihoods-0.0.6.4/tests/test_lik_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/tests/test_scaler_heterogeneous.py` & `torchlikelihoods-0.0.6.4/tests/test_scaler_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/tests/test_scaler_heterogeneous_object.py` & `torchlikelihoods-0.0.6.4/tests/test_scaler_heterogeneous_object.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/tests/test_scaler_minmax.py` & `torchlikelihoods-0.0.6.4/tests/test_scaler_minmax.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/tests/test_scaler_standard.py` & `torchlikelihoods-0.0.6.4/tests/test_scaler_standard.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/tests/utils/mock_data.py` & `torchlikelihoods-0.0.6.4/tests/utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/distributions/delta.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/distributions/delta.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/distributions/heterogeneous.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/distributions/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/__init__.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from .beta import BetaLikelihood
 from .bernoulli import BernoulliLikelihood
 from .continous_bernoulli import ContinousBernoulliLikelihood
 from .categorical import CategoricalLikelihood
 from .normal import NormalLikelihood
 from .normal_mean import *
 from .heterogeneous import HeterogeneousLikelihood
-
-
+from .delta import DeltaLikelihood
 
 likelihood_dict = {
     'beta': BetaLikelihood,
     'ber': BernoulliLikelihood,
     'cb': ContinousBernoulliLikelihood,
     'cat': CategoricalLikelihood,
     'normal': NormalLikelihood,
     'normal1': NormalMean1Likelihood,
     'normal01': NormalMean01Likelihood,
-    'het': HeterogeneousLikelihood
+    'het': HeterogeneousLikelihood,
+    'delta': DeltaLikelihood
 }
 
 
 def build_likelihoods_list(lik_info_list):
     likelihoods = []
     for (lik_name_i, domain_size_i) in lik_info_list:
         lik = likelihood_dict[lik_name_i](domain_size_i)
```

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/base.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/base.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/bernoulli.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/bernoulli.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/beta.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/beta.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/categorical.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/categorical.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/continous_bernoulli.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/continous_bernoulli.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/delta.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/delta.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/heterogeneous.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/normal.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/normal.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/likelihoods/normal_mean.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/likelihoods/normal_mean.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/__init__.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/base.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/base.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/heterogeneous.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/heterogeneous_object.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/heterogeneous_object.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/min.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/min.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/minmax.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/minmax.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/scale.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/scale.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/scalediff.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/scalediff.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/scalers/standard.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/scalers/standard.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods/utils/struct.py` & `torchlikelihoods-0.0.6.4/torchlikelihoods/utils/struct.py`

 * *Files identical despite different names*

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods.egg-info/PKG-INFO` & `torchlikelihoods-0.0.6.4/torchlikelihoods.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlikelihoods
-Version: 0.0.6.3
+Version: 0.0.6.4
 Summary: TorchLikelihoods: User-friendly handling of likelihoods in Pytorch
 Home-page: https://github.com/psanch21/torchlikelihoods
 Author: Pablo Sanchez Martin
 Author-email: psanch2103@gmail.com
 License: MIT
 Keywords: Distributions,Likelihoods,Heterogeneous Data,Pytorch,Scalers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchlikelihoods-0.0.6.3/torchlikelihoods.egg-info/SOURCES.txt` & `torchlikelihoods-0.0.6.4/torchlikelihoods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

