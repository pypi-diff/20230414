# Comparing `tmp/sdnist-2.1.1-2.tar.gz` & `tmp/sdnist-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdnist-2.1.1.tar", last modified: Fri Mar 17 17:39:33 2023, max compression
+gzip compressed data, was "dist/sdnist-2.2.0.tar", last modified: Fri Apr 14 14:39:51 2023, max compression
```

## Comparing `sdnist-2.1.1-2.tar` & `sdnist-2.2.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.388695 sdnist-2.1.1/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      138 2023-02-28 14:33:44.000000 sdnist-2.1.1/MANIFEST.in
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    21523 2023-03-17 17:39:33.388123 sdnist-2.1.1/PKG-INFO
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    18513 2023-03-17 15:41:53.000000 sdnist-2.1.1/README.md
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.325914 sdnist-2.1.1/sdnist/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4118 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      213 2023-03-17 16:54:59.000000 sdnist-2.1.1/sdnist/__main__.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.334172 sdnist-2.1.1/sdnist/challenge/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/challenge/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1344 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/challenge/baseline.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     7883 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/challenge/submission.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      528 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/challenge/subsample.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    11499 2023-03-17 17:23:59.000000 sdnist-2.1.1/sdnist/load.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.351058 sdnist-2.1.1/sdnist/metrics/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/metrics/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     2088 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/metrics/apparent_match_dist.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      276 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/metrics/graph_edge_map.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3518 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/metrics/hoc.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    17892 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/metrics/inconsistency.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    11971 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/metrics/kmarg_old.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     6501 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/metrics/kmarginal.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     8039 2023-03-17 15:41:12.000000 sdnist-2.1.1/sdnist/metrics/pca.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1554 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/metrics/pearson_correlation.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3778 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/metrics/propensity.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     8345 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/metrics/regression.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.351977 sdnist-2.1.1/sdnist/preprocess/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/preprocess/__init__.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.360118 sdnist-2.1.1/sdnist/report/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      296 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/report/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     5775 2023-03-17 16:54:59.000000 sdnist-2.1.1/sdnist/report/__main__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      103 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/report/common.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      628 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/report/config.json
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.364912 sdnist-2.1.1/sdnist/report/dataset/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    12327 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/report/dataset/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4901 2023-03-17 15:41:12.000000 sdnist-2.1.1/sdnist/report/dataset/binning.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1350 2023-03-17 15:41:12.000000 sdnist-2.1.1/sdnist/report/dataset/transform.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4592 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/report/dataset/validate.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3377 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/report/generate.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.374058 sdnist-2.1.1/sdnist/report/plots/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      418 2023-03-17 15:41:12.000000 sdnist-2.1.1/sdnist/report/plots/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3208 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/report/plots/apparent_match_dist.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3403 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/report/plots/correlation.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4404 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/report/plots/grid.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1763 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/report/plots/pearson_correlation.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     2377 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/report/plots/propensity.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    13397 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/report/plots/univariate.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     6904 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/report/report_data.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.315110 sdnist-2.1.1/sdnist/report/resources/
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.374922 sdnist-2.1.1/sdnist/report/resources/templates/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    14664 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/report/resources/templates/main.jinja2
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.378111 sdnist-2.1.1/sdnist/report/score/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/report/score/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     6631 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/report/score/paragraphs.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3624 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/report/score/privacy.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.384196 sdnist-2.1.1/sdnist/report/score/utility/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    29511 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/report/score/utility/__init__.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4875 2023-03-17 15:41:12.000000 sdnist-2.1.1/sdnist/report/score/utility/inconsistency.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     8796 2023-03-17 15:41:12.000000 sdnist-2.1.1/sdnist/report/score/utility/linear_regression.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     7554 2023-03-17 16:54:59.000000 sdnist-2.1.1/sdnist/report/score/utility/pca.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      905 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/report/server.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1376 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/schema.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1034 2023-03-17 15:41:53.000000 sdnist-2.1.1/sdnist/strs.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     9676 2023-03-17 15:41:12.000000 sdnist-2.1.1/sdnist/utils.py
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)       22 2023-03-17 15:51:10.000000 sdnist-2.1.1/sdnist/version.py
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.386144 sdnist-2.1.1/sdnist/visualizer_resources/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     6936 2023-02-28 14:33:44.000000 sdnist-2.1.1/sdnist/visualizer_resources/report2.jinja2
-drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-03-17 17:39:33.329506 sdnist-2.1.1/sdnist.egg-info/
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    21523 2023-03-17 17:39:32.000000 sdnist-2.1.1/sdnist.egg-info/PKG-INFO
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1694 2023-03-17 17:39:33.000000 sdnist-2.1.1/sdnist.egg-info/SOURCES.txt
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        1 2023-03-17 17:39:32.000000 sdnist-2.1.1/sdnist.egg-info/dependency_links.txt
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      125 2023-03-17 17:39:32.000000 sdnist-2.1.1/sdnist.egg-info/requires.txt
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        7 2023-03-17 17:39:32.000000 sdnist-2.1.1/sdnist.egg-info/top_level.txt
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)       38 2023-03-17 17:39:33.388945 sdnist-2.1.1/setup.cfg
--rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1539 2023-03-17 16:32:12.000000 sdnist-2.1.1/setup.py
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.451905 sdnist-2.2.0/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      138 2023-04-14 14:39:17.000000 sdnist-2.2.0/MANIFEST.in
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    21578 2023-04-14 14:39:51.451439 sdnist-2.2.0/PKG-INFO
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    18552 2023-04-14 14:39:17.000000 sdnist-2.2.0/README.md
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.404439 sdnist-2.2.0/sdnist/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4118 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/__init__.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      213 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/__main__.py
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.412891 sdnist-2.2.0/sdnist/challenge/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/challenge/__init__.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1344 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/challenge/baseline.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     7883 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/challenge/submission.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      528 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/challenge/subsample.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    11568 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/load.py
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.428201 sdnist-2.2.0/sdnist/metrics/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/__init__.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     2218 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/apparent_match_dist.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      276 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/graph_edge_map.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3518 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/hoc.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    17892 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/inconsistency.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    11971 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/kmarg_old.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     6501 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/kmarginal.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     8088 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/pca.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1554 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/pearson_correlation.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3778 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/propensity.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     8519 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/regression.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1561 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/metrics/unique_exact_matches.py
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.429112 sdnist-2.2.0/sdnist/preprocess/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/preprocess/__init__.py
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.434190 sdnist-2.2.0/sdnist/report/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      296 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/__init__.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     5788 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/__main__.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      103 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/common.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      628 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/config.json
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.437475 sdnist-2.2.0/sdnist/report/dataset/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    14752 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/dataset/__init__.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4967 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/dataset/binning.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1350 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/dataset/transform.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4643 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/dataset/validate.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3377 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/generate.py
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.442121 sdnist-2.2.0/sdnist/report/plots/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      418 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/__init__.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3208 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/apparent_match_dist.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     3403 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/correlation.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4404 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/grid.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1763 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/pearson_correlation.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     2377 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/propensity.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    13782 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/plots/univariate.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     7599 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/report_data.py
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.394607 sdnist-2.2.0/sdnist/report/resources/
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.442902 sdnist-2.2.0/sdnist/report/resources/templates/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    15672 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/resources/templates/main.jinja2
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.444773 sdnist-2.2.0/sdnist/report/score/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/__init__.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     7026 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/paragraphs.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     5884 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/privacy.py
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.448541 sdnist-2.2.0/sdnist/report/score/utility/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    29763 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/utility/__init__.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     4875 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/utility/inconsistency.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     8868 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/utility/linear_regression.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     7394 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/score/utility/pca.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      905 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/report/server.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1376 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/schema.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1034 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/strs.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     9992 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/utils.py
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)       22 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/version.py
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.449389 sdnist-2.2.0/sdnist/visualizer_resources/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     6936 2023-04-14 14:39:17.000000 sdnist-2.2.0/sdnist/visualizer_resources/report2.jinja2
+drwxr-xr-x   0 gsh3     (65125) NIST\671DIV (36684)        0 2023-04-14 14:39:51.408798 sdnist-2.2.0/sdnist.egg-info/
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)    21578 2023-04-14 14:39:51.000000 sdnist-2.2.0/sdnist.egg-info/PKG-INFO
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1733 2023-04-14 14:39:51.000000 sdnist-2.2.0/sdnist.egg-info/SOURCES.txt
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        1 2023-04-14 14:39:51.000000 sdnist-2.2.0/sdnist.egg-info/dependency_links.txt
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)      170 2023-04-14 14:39:51.000000 sdnist-2.2.0/sdnist.egg-info/requires.txt
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)        7 2023-04-14 14:39:51.000000 sdnist-2.2.0/sdnist.egg-info/top_level.txt
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)       38 2023-04-14 14:39:51.452098 sdnist-2.2.0/setup.cfg
+-rw-r--r--   0 gsh3     (65125) NIST\671DIV (36684)     1584 2023-04-14 14:39:17.000000 sdnist-2.2.0/setup.py
```

### Comparing `sdnist-2.1.1/PKG-INFO` & `sdnist-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: sdnist
-Version: 2.1.1
+Version: 2.2.0
 Summary: SDNist: Deidentified Data Report Generator
 Home-page: https://github.com/usnistgov/SDNist
 Author: National Institute of Standards and Technology
 Author-email: gary.howarth@nist.gov
 License: UNKNOWN
-Description: # SDNist v2.1: Deidentified Data Report Tool
+Description: # SDNist v2.2: Deidentified Data Report Tool
         
         ## [SDNist is the offical software package for engaging in the NIST Collaborative Research Cycle](https://pages.nist.gov/privacy_collaborative_research_cycle)
         
-        Welcome! SDNist v2.1 is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
+        Welcome! SDNist is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
         
         The deidentified data report evaluates utility and privacy of a given deidentified dataset and generates a summary quality report with performance of a deidentified dataset enumerated and illustrated for each utility and privacy metric.
         
         [Preview sample reports produced by the tool here.](https://github.com/usnistgov/SDNist/tree/main/sdnist/report/sample-reports)
         
         This tool is being actively developed. Please (raise an Issue)[https://github.com/usnistgov/SDNist/issues]  if you catch a bug or would like have feature suggestions. 
         
@@ -37,16 +37,18 @@
         
         
         Setting Up the SDNIST Report Tool
         ------------------------
         
         ### Brief Setup Instructions
         
-        SDNist v2.1 requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend uninstalling or installing v2.1 in a virtual environment. v2.1 can be installed via [Release 2.1](https://github.com/usnistgov/SDNist/releases/tag/v2.1.1). The NIST Diverse Community Exceprt data will download on the fly.
-        
+        SDNist requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend uninstalling or installing v2.2 in a virtual environment. v2.2 can be installed via [Release 2.2](https://github.com/usnistgov/SDNist/releases/tag/v2.2.0). The NIST Diverse Community Exceprt data will download on the fly.
+        ```
+        pip install sdnist
+        ```
         
         ### Detailed Setup Instructions
         
         1. The SDNist Report Tool is a part of the sdnist Python library that can be installed on a user’s MAC OS, Windows, or Linux machine.
         
         
         2. The sdnist library requires Python version 3.7 or greater to be installed on the user's machine. Check whether an installation exists on the machine by executing the following command in your terminal on Mac/Linux or powershell on Windows:
@@ -57,18 +59,18 @@
         
         
         3.  Create a local directory/folder on the machine to set up the SDNist library. This guide assumes the local directory to be sdnist-project; an example of a complete file path is c:\\sdnist-project:
             ```
             c:\\sdnist-project>     
             ```
         
-        4.  Download the sdnist installable wheel (sdnist-2.1.1-py3-none-any.whl) from the Github: [Release 2.1](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/sdnist-2.1.1-py3-none-any.whl).
+        4.  Download the sdnist installable wheel (sdnist-2.2.0-py3-none-any.whl) from the Github: [Release 2.2](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/sdnist-2.2.0-py3-none-any.whl).
         
         
-        5.  Move the downloaded sdnist-2.1.1-py3-none-any.whl file to the sdnist-project directory.
+        5.  Move the downloaded sdnist-2.2.0-py3-none-any.whl file to the sdnist-project directory.
         
         
         6.  Using the terminal on Mac/Linux or powershell on Windows, navigate to the sdnist-project directory.
         
         
         7.  In the already-opened terminal or powershell window, execute the following command to create a new Python environment. The sdnist library will be installed in this newly created Python environment:
         
@@ -113,30 +115,30 @@
             ```
             Run the following command to let Windows execute scripts:
             ```
             Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
             ```
         
         
-        10. Per step 5 above, the sdnist-2.1.1-py3-none-any.whl file should already be present in the sdnist-project directory. Check whether that is true by listing the files in the sdnist-project directory.
+        10. Per step 5 above, the sdnist-2.2.0-py3-none-any.whl file should already be present in the sdnist-project directory. Check whether that is true by listing the files in the sdnist-project directory.
         
               **MAC OS/Linux:**
                ```
                (venv) sdnist-project> ls
                ```
               **Windows:**
                ```
                (venv) c:\\sdnist-project> dir
                ```
-               The sdnist-2.1.1-py3-none-any.whl file should be in the list printed by the above command; otherwise, follow steps 4 and 5 again to download the .whl file.
+               The sdnist-2.2.0-py3-none-any.whl file should be in the list printed by the above command; otherwise, follow steps 4 and 5 again to download the .whl file.
         
         
         11. Install sdnist Python library:
                ```
-               (venv) c:\\sdnist-project> pip install sdnist-2.1.1-py3-none-any.whl
+               (venv) c:\\sdnist-project> pip install sdnist-2.2.0-py3-none-any.whl
                ```
         
         
         12. Installation is successful if executing the following command outputs a help menu for the sdnist.report package:
                ```
                (venv) c:\\sdnist-project> python -m sdnist.report -h
                ```
@@ -206,15 +208,15 @@
               ```
         
         
         5.  Use the following command to generate a data quality report for the example deidentified dataset (syn_national.csv) that is generated using the bundled dataset NATIONAL:
               ```
               (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL
               ```
-        6.  SDNist 2.1 allow users to add labels for the deidentified dataset used to generate report:
+        6.  Starting from version 2.1, SDNist allow users to add labels for the deidentified dataset used to generate report:
             * To add single string label to the report, use command line option **--labels** followed by a string as given in the following example command:
               ```
               (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels used_epsilon_1
               ```
               This is how the string label *used_epsilon_1* will appear in the report:
               ![string label in report](readme_resource/string_label.png)
             * To add multiple string labels to the report, use command line option **--labels** followed by a path to the json file containing labels:
@@ -247,15 +249,15 @@
         ---------------------------------
         
         1.  The sdnist.report package comes with built-in datasets. The package will automatically download the datasets from Github if they are not already available locally on your machine. You should see following message on your terminal or powershell window when the datasets are downloaded by the sdnist.report package:
               ```
               (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
         
               Downloading all SDNist datasets from:  
-              https://github.com/usnistgov/SDNist/releases/download/v2.1.1/diverse_communities_data_excerpts.zip ...  
+              https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip ...  
               ...5%, 47352 KB, 8265 KB/s, 5 seconds elapsed
               ```
         
               Follow the next subsection, Download Data Manually, if the sdnist.report package is unable to download the datasets.
         
         
         2. All the datasets required by the sdnist.report package are installed into the sdnist _toy _data directory, which should be now present inside the sdnist-project directory. sdnist _toy _data is also a data root directory. You can use some other directory as a data root by providing the –data-root argument to the sdnist.report package. If you provide a –data-root argument with a path, the sdnist.report package will look for datasets in the data root directory you have specified, and the package will download it if it is not present in the data root.
@@ -265,15 +267,15 @@
         
            You can download a copy of the datasets from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts). This copy is similar to the one bundled with the sdnist.report package, but it contains more documentation and a description of the datasets.
         
         
         4. You can download the toy deidentified datasets from Github [Sdnist Toy Deidentified Dataset](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/toy_deidentified_data.zip). Unzip the downloaded file, and move the unzipped toy_deidentified_dataset directory to the sdnist-project directory.
         
         
-        5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/diverse_communities_excerpts_data.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
+        5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_excerpts_data.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
         
         
         6. Use the following commands for generating reports if you are using a toy deidentified dataset file:
         
            For evaluating the Massachusetts dataset:
            ```
            (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_ma.csv MA
@@ -292,15 +294,15 @@
         7.  A deidentified dataset can be a .csv or a parquet file, and the path of this file is required
         by the sdnist.report package to generate a data quality report.
         
         
         Download Data Manually
         ----------------------
         
-        1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/diverse_communities_data_excerpts.zip).
+        1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip).
         3.  Unzip the **diverse_community_excerpts_data.zip** file and move the unzipped **diverse_community_excerpts_data** directory to the **sdnist-project** directory.
         4.  Delete the **diverse_community_excerpts_data.zip** file once the data is successfully extracted from the zip.
         
         Citing SDNist Deidentified Data Report Tool
         -------------------------------------------
         
         If you publish work that utilizes the SDNist Deidentified Data Tool, please cite the software. Citation recommendation:
```

### Comparing `sdnist-2.1.1/README.md` & `sdnist-2.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# SDNist v2.1: Deidentified Data Report Tool
+# SDNist v2.2: Deidentified Data Report Tool
 
 ## [SDNist is the offical software package for engaging in the NIST Collaborative Research Cycle](https://pages.nist.gov/privacy_collaborative_research_cycle)
 
-Welcome! SDNist v2.1 is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
+Welcome! SDNist is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
 
 The deidentified data report evaluates utility and privacy of a given deidentified dataset and generates a summary quality report with performance of a deidentified dataset enumerated and illustrated for each utility and privacy metric.
 
 [Preview sample reports produced by the tool here.](https://github.com/usnistgov/SDNist/tree/main/sdnist/report/sample-reports)
 
 This tool is being actively developed. Please (raise an Issue)[https://github.com/usnistgov/SDNist/issues]  if you catch a bug or would like have feature suggestions. 
 
@@ -29,16 +29,18 @@
 
 
 Setting Up the SDNIST Report Tool
 ------------------------
 
 ### Brief Setup Instructions
 
-SDNist v2.1 requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend uninstalling or installing v2.1 in a virtual environment. v2.1 can be installed via [Release 2.1](https://github.com/usnistgov/SDNist/releases/tag/v2.1.1). The NIST Diverse Community Exceprt data will download on the fly.
-
+SDNist requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend uninstalling or installing v2.2 in a virtual environment. v2.2 can be installed via [Release 2.2](https://github.com/usnistgov/SDNist/releases/tag/v2.2.0). The NIST Diverse Community Exceprt data will download on the fly.
+```
+pip install sdnist
+```
 
 ### Detailed Setup Instructions
 
 1. The SDNist Report Tool is a part of the sdnist Python library that can be installed on a user’s MAC OS, Windows, or Linux machine.
 
 
 2. The sdnist library requires Python version 3.7 or greater to be installed on the user's machine. Check whether an installation exists on the machine by executing the following command in your terminal on Mac/Linux or powershell on Windows:
@@ -49,18 +51,18 @@
 
 
 3.  Create a local directory/folder on the machine to set up the SDNist library. This guide assumes the local directory to be sdnist-project; an example of a complete file path is c:\\sdnist-project:
     ```
     c:\\sdnist-project>     
     ```
 
-4.  Download the sdnist installable wheel (sdnist-2.1.1-py3-none-any.whl) from the Github: [Release 2.1](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/sdnist-2.1.1-py3-none-any.whl).
+4.  Download the sdnist installable wheel (sdnist-2.2.0-py3-none-any.whl) from the Github: [Release 2.2](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/sdnist-2.2.0-py3-none-any.whl).
 
 
-5.  Move the downloaded sdnist-2.1.1-py3-none-any.whl file to the sdnist-project directory.
+5.  Move the downloaded sdnist-2.2.0-py3-none-any.whl file to the sdnist-project directory.
 
 
 6.  Using the terminal on Mac/Linux or powershell on Windows, navigate to the sdnist-project directory.
 
 
 7.  In the already-opened terminal or powershell window, execute the following command to create a new Python environment. The sdnist library will be installed in this newly created Python environment:
 
@@ -105,30 +107,30 @@
     ```
     Run the following command to let Windows execute scripts:
     ```
     Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
     ```
 
 
-10. Per step 5 above, the sdnist-2.1.1-py3-none-any.whl file should already be present in the sdnist-project directory. Check whether that is true by listing the files in the sdnist-project directory.
+10. Per step 5 above, the sdnist-2.2.0-py3-none-any.whl file should already be present in the sdnist-project directory. Check whether that is true by listing the files in the sdnist-project directory.
 
       **MAC OS/Linux:**
        ```
        (venv) sdnist-project> ls
        ```
       **Windows:**
        ```
        (venv) c:\\sdnist-project> dir
        ```
-       The sdnist-2.1.1-py3-none-any.whl file should be in the list printed by the above command; otherwise, follow steps 4 and 5 again to download the .whl file.
+       The sdnist-2.2.0-py3-none-any.whl file should be in the list printed by the above command; otherwise, follow steps 4 and 5 again to download the .whl file.
 
 
 11. Install sdnist Python library:
        ```
-       (venv) c:\\sdnist-project> pip install sdnist-2.1.1-py3-none-any.whl
+       (venv) c:\\sdnist-project> pip install sdnist-2.2.0-py3-none-any.whl
        ```
 
 
 12. Installation is successful if executing the following command outputs a help menu for the sdnist.report package:
        ```
        (venv) c:\\sdnist-project> python -m sdnist.report -h
        ```
@@ -198,15 +200,15 @@
       ```
 
 
 5.  Use the following command to generate a data quality report for the example deidentified dataset (syn_national.csv) that is generated using the bundled dataset NATIONAL:
       ```
       (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL
       ```
-6.  SDNist 2.1 allow users to add labels for the deidentified dataset used to generate report:
+6.  Starting from version 2.1, SDNist allow users to add labels for the deidentified dataset used to generate report:
     * To add single string label to the report, use command line option **--labels** followed by a string as given in the following example command:
       ```
       (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels used_epsilon_1
       ```
       This is how the string label *used_epsilon_1* will appear in the report:
       ![string label in report](readme_resource/string_label.png)
     * To add multiple string labels to the report, use command line option **--labels** followed by a path to the json file containing labels:
@@ -239,15 +241,15 @@
 ---------------------------------
 
 1.  The sdnist.report package comes with built-in datasets. The package will automatically download the datasets from Github if they are not already available locally on your machine. You should see following message on your terminal or powershell window when the datasets are downloaded by the sdnist.report package:
       ```
       (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
 
       Downloading all SDNist datasets from:  
-      https://github.com/usnistgov/SDNist/releases/download/v2.1.1/diverse_communities_data_excerpts.zip ...  
+      https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip ...  
       ...5%, 47352 KB, 8265 KB/s, 5 seconds elapsed
       ```
 
       Follow the next subsection, Download Data Manually, if the sdnist.report package is unable to download the datasets.
 
 
 2. All the datasets required by the sdnist.report package are installed into the sdnist _toy _data directory, which should be now present inside the sdnist-project directory. sdnist _toy _data is also a data root directory. You can use some other directory as a data root by providing the –data-root argument to the sdnist.report package. If you provide a –data-root argument with a path, the sdnist.report package will look for datasets in the data root directory you have specified, and the package will download it if it is not present in the data root.
@@ -257,15 +259,15 @@
 
    You can download a copy of the datasets from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts). This copy is similar to the one bundled with the sdnist.report package, but it contains more documentation and a description of the datasets.
 
 
 4. You can download the toy deidentified datasets from Github [Sdnist Toy Deidentified Dataset](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/toy_deidentified_data.zip). Unzip the downloaded file, and move the unzipped toy_deidentified_dataset directory to the sdnist-project directory.
 
 
-5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/diverse_communities_excerpts_data.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
+5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_excerpts_data.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
 
 
 6. Use the following commands for generating reports if you are using a toy deidentified dataset file:
 
    For evaluating the Massachusetts dataset:
    ```
    (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_ma.csv MA
@@ -284,15 +286,15 @@
 7.  A deidentified dataset can be a .csv or a parquet file, and the path of this file is required
 by the sdnist.report package to generate a data quality report.
 
 
 Download Data Manually
 ----------------------
 
-1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/diverse_communities_data_excerpts.zip).
+1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip).
 3.  Unzip the **diverse_community_excerpts_data.zip** file and move the unzipped **diverse_community_excerpts_data** directory to the **sdnist-project** directory.
 4.  Delete the **diverse_community_excerpts_data.zip** file once the data is successfully extracted from the zip.
 
 Citing SDNist Deidentified Data Report Tool
 -------------------------------------------
 
 If you publish work that utilizes the SDNist Deidentified Data Tool, please cite the software. Citation recommendation:
```

### Comparing `sdnist-2.1.1/sdnist/__init__.py` & `sdnist-2.2.0/sdnist/__init__.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/challenge/baseline.py` & `sdnist-2.2.0/sdnist/challenge/baseline.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/challenge/submission.py` & `sdnist-2.2.0/sdnist/challenge/submission.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/challenge/subsample.py` & `sdnist-2.2.0/sdnist/challenge/subsample.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/load.py` & `sdnist-2.2.0/sdnist/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 
 def check_exists(root: Path, name: Path, download: bool, data_name: str = strs.DATA):
     root = root.expanduser()
     if not name.exists():
         print(f"{name} does not exist.")
         zip_path = Path(root.parent, 'data.zip')
-        version = "2.1.1"
+        version = "2.2.0"
 
         version_v = f"v{version}"
         sdnist_version = DEFAULT_DATASET
 
         download_link = f"https://github.com/usnistgov/SDNist/releases/download/{version_v}/{sdnist_version}.zip"
         if zip_path.exists() and error_opening_zip(zip_path):
             os.remove(zip_path)
@@ -120,14 +120,15 @@
                     except zipfile.error as e:
                         raise e
             # delete zipfile
             os.remove(zip_path)
             print()
             copy_from_path = str(Path(extract_path, sdnist_version))
             copy_to_path = str(Path(root))
+            print(f"Copying {copy_from_path} to {copy_to_path} ...")
             copy_tree(copy_from_path, copy_to_path)
             shutil.rmtree(extract_path)
         else:
             raise ValueError(f"{name} does not exist.")
 
 
 def build_name(challenge: str,
```

### Comparing `sdnist-2.1.1/sdnist/metrics/apparent_match_dist.py` & `sdnist-2.2.0/sdnist/metrics/apparent_match_dist.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from pathlib import Path
 
 import pandas as pd
 import matplotlib.pyplot as plt
 
 
 def cellchange(df1, df2, quasi, exclude_cols):
+    # use drop duplicates with keep argument as False,
+    # to retain only those records that occur only
+    # once in the data.
     uniques1 = df1.drop_duplicates(subset=quasi, keep=False)
     uniques2 = df2.drop_duplicates(subset=quasi, keep=False)
     matcheduniq = uniques1.merge(uniques2, how='inner', on=quasi)
     allcols = set(df1.columns).intersection(set(df2.columns))
     cols = allcols - set(quasi) - set(exclude_cols)
     return match(matcheduniq, cols), uniques1, uniques2, matcheduniq
```

### Comparing `sdnist-2.1.1/sdnist/metrics/hoc.py` & `sdnist-2.2.0/sdnist/metrics/hoc.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/metrics/inconsistency.py` & `sdnist-2.2.0/sdnist/metrics/inconsistency.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/metrics/kmarg_old.py` & `sdnist-2.2.0/sdnist/metrics/kmarg_old.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/metrics/kmarginal.py` & `sdnist-2.2.0/sdnist/metrics/kmarginal.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/metrics/pca.py` & `sdnist-2.2.0/sdnist/metrics/pca.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,16 +141,18 @@
             plot_single_component_pair(f'Target Dataset: PC{hc[0]}-PC{hc[1]}',
                                        f_tdf, h_tar_path, h_t_cp_o_path, t_cp_o_path, hc)
             plot_single_component_pair(f'Deidentified Dataset: : PC{hc[0]}-PC{hc[1]}',
                                        f_sdf, h_syn_path, h_s_cp_o_path, s_cp_o_path, hc)
             plot_paths[strs.HIGHLIGHTED][(h_type, h_name, h_caption)] = \
                 [h_tar_path, h_syn_path]
 
-        e = time.time() - s
-        # print('PCA TOOK TIME: ', e)
+        # clear temporary data from report data
+        remove_path(t_cp_o_path)
+        remove_path(s_cp_o_path)
+
         return plot_paths
 
 
 def min_max_scaling(series):
     return (series - series.min()) / (series.max() - series.min())
```

### Comparing `sdnist-2.1.1/sdnist/metrics/pearson_correlation.py` & `sdnist-2.2.0/sdnist/metrics/pearson_correlation.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/metrics/propensity.py` & `sdnist-2.2.0/sdnist/metrics/propensity.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/metrics/regression.py` & `sdnist-2.2.0/sdnist/metrics/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,21 +148,21 @@
         self.scm = self.scm.transpose()
 
         # calculated difference of density distribution
         # between target and deindentifed data
         self.diff = self.tcm - self.scm
 
         # calculate regression lines for target and synthetic data
-        if self.ts.shape[0] > 1:
-            self.t_reg = stats.linregress(self.ts[xc], self.ts[yc])
+        if self.ts.shape[0] > 1 and len(self.ts[xc].unique()) > 1:
+            self.t_reg = stats.linregress(self.ts[xc].astype(float), self.ts[yc].astype(float))
             self.t_slope = round(self.t_reg.slope, 2)
             self.t_intercept = round(self.t_reg.intercept, 2)
 
-        if self.ss.shape[0] > 1:
-            self.s_reg = stats.linregress(self.ss[xc], self.ss[yc])
+        if self.ss.shape[0] > 1 and len(self.ss[xc].unique()) > 1:
+            self.s_reg = stats.linregress(self.ss[xc].astype(float), self.ss[yc].astype(float))
             self.s_slope = round(self.s_reg.slope, 2)
             self.s_intercept = round(self.s_reg.intercept, 2)
 
     def plots(self) -> List[Path]:
         """
         Create plots for target and deidentified data's density distribution and
         overlay regression lines on the density grid.
@@ -182,18 +182,18 @@
         apc1 = ax1.pcolor(self.diff, cmap='PuOr', vmin=-0.3, vmax=0.3)
         fig.colorbar(apc1, ax=ax1)
 
         tx = self.ts[self.xc].values
 
         r_tx_df = pd.DataFrame([[_ + 0.5, self.t_intercept + self.t_slope * (_ + 0.5)]
                                 for _ in tx], columns=['x', 'y'])
-        r_tx_df = r_tx_df[r_tx_df['y'] >= 0]
+        r_tx_df = r_tx_df[(r_tx_df['y'] >= 0) & (r_tx_df['y'] <= 10)]
         r_sx_df = pd.DataFrame([[_ + 0.5, self.s_intercept + self.s_slope * (_ + 0.5)]
                                 for _ in tx], columns=['x', 'y'])
-        r_sx_df = r_sx_df[r_sx_df['y'] >= 0]
+        r_sx_df = r_sx_df[(r_sx_df['y'] >= 0) & (r_sx_df['y'] <= 10)]
 
         ax0.plot(r_tx_df['x'],
                  r_tx_df['y'], color='red', label='Target')
         ax1.plot(r_tx_df['x'],
                  r_tx_df['y'], color='red')
         ax1.plot(r_sx_df['x'],
                  r_sx_df['y'], color='green', label='Deid.')
```

### Comparing `sdnist-2.1.1/sdnist/report/__main__.py` & `sdnist-2.2.0/sdnist/report/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     log.msg('SDNist: Deidentified Data Report Tool', level=0, timed=False)
     log.msg(f'Creating Evaluation Report for Deidentified Data at path: {synthetic_filepath}',
             level=1)
 
     if not outfile.exists():
         log.msg('Loading Datasets', level=2)
         dataset = Dataset(synthetic_filepath, log, dataset_name, data_root, download)
-        ui_data = data_description(dataset, ui_data, labels_dict)
+        ui_data = data_description(dataset, ui_data, report_data, labels_dict)
         log.end_msg()
 
         # Create scores
         log.msg('Computing Utility Scores', level=2)
         ui_data, report_data = utility_score(dataset, ui_data, report_data, log)
         log.end_msg()
```

### Comparing `sdnist-2.1.1/sdnist/report/config.json` & `sdnist-2.2.0/sdnist/report/config.json`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/report/dataset/__init__.py` & `sdnist-2.2.0/sdnist/report/dataset/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,87 @@
 import math
 from pathlib import Path
 from typing import Dict, List, Optional
 from dataclasses import dataclass, field
-
+import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 
 from sdnist.report import ReportUIData, FILE_DIR
 from sdnist.report.report_data import \
-    DatasetType, DataDescriptionPacket, ScorePacket,\
-    Attachment, AttachmentType
+    DatasetType, DataDescriptionPacket, ScorePacket, \
+    Attachment, AttachmentType, ReportData
 from sdnist.load import \
     TestDatasetName, load_dataset, build_name
 from sdnist.report.dataset.transform import transform
 from sdnist.report.dataset.validate import validate
 from sdnist.report.dataset.binning import *
 
 import sdnist.strs as strs
 
 import sdnist.utils as u
 from sdnist.load import DEFAULT_DATASET
 
+st_code_to_str = {
+    '25': 'MA',
+    '48': 'TX',
+    '01': 'AL',
+    '06': 'CA',
+    '08': 'CO',
+    '13': 'GA',
+    '17': 'IL',
+    '19': 'IA',
+    '24': 'MD',
+    '26': 'MI',
+    '28': 'MS',
+    '29': 'MO',
+    '30': 'MT',
+    '32': 'NV',
+    '36': 'NY',
+    '38': 'ND',
+    '40': 'OK',
+    '51': 'VA'
+}
+
 def unavailable_features(config: Dict, synthetic_data: pd.DataFrame):
     """remove features from configuration that are not available in
     the input synthetic data"""
     cnf = config
     fl = synthetic_data.columns.tolist()
     if 'k_marginal' in cnf and 'group_features' in cnf['k_marginal']:
         for f in cnf['k_marginal']['group_features'].copy():
             if f not in fl:
                 cnf['k_marginal']['group_features'].remove(f)
 
     return cnf
 
+def compute_feature_space(data_dict: Dict,
+                          features: List[str]):
+    # list of features and their value length
+    f_list = []
+    for f in features:
+        if "values" not in data_dict[f]:
+            vals = [0] * 269  # in case of INDP feature
+        else:
+            vals = data_dict[f]["values"]
+        if "min" in vals and f != 'AGEP':
+            continue
+        if f == 'AGEP':
+            f_list.append([f, 100])
+        else:
+            f_list.append([f, len(vals)])
+
+    f_df = pd.DataFrame(f_list, columns=['feature', 'len'])
+    f_df = f_df.sort_values(by='len')
+
+    # get product of all feature lengths
+    n_features = f_df['len'].astype(object).product()
+
+    # return number of features and sorted list of features
+    return n_features
 
 @dataclass
 class Dataset:
     synthetic_filepath: Path
     log: u.SimpleLogger
     test: TestDatasetName = TestDatasetName.NONE
     data_root: Path = Path(DEFAULT_DATASET)
@@ -44,14 +89,15 @@
 
     challenge: str = strs.CENSUS
     target_data: pd.DataFrame = field(init=False)
     target_data_path: Path = field(init=False)
     synthetic_data: pd.DataFrame = field(init=False)
     schema: Dict = field(init=False)
     validation_log: Dict = field(init=False)
+    feature_space: int = field(init=False)
 
     def __post_init__(self):
         # load target dataset which is used to score synthetic dataset
         self.target_data, params = load_dataset(
             challenge=strs.CENSUS,
             root=self.data_root,
             download=self.download,
@@ -61,14 +107,17 @@
         )
         self.target_data_path = build_name(
             challenge=strs.CENSUS,
             root=self.data_root,
             public=False,
             test=self.test
         )
+        # raw target data
+        self.raw_target_data = self.target_data.copy()
+
         self.schema = params[strs.SCHEMA]
         configs_path = self.target_data_path.parent.parent
         # add config packaged with data and also the config package with sdnist.report package
         config_1 = u.read_json(Path(configs_path, 'config.json'))
         config_2 = u.read_json(Path(FILE_DIR, 'config.json'))
         self.config = {**config_1, **config_2}
 
@@ -82,15 +131,15 @@
             if strs.DROP_FEATURES in self.config else []
         self.features = self._fix_features(drop_features,
                                            self.config[strs.K_MARGINAL][strs.GROUP_FEATURES])
 
         # load synthetic dataset
         dtypes = {feature: desc["dtype"] for feature, desc in self.schema.items()}
         if str(self.synthetic_filepath).endswith('.csv'):
-            self.synthetic_data = pd.read_csv(self.synthetic_filepath, dtype=dtypes)
+            self.synthetic_data = pd.read_csv(self.synthetic_filepath)
         elif str(self.synthetic_filepath).endswith('.parquet'):
             self.synthetic_data = pd.read_parquet(self.synthetic_filepath)
         else:
             raise Exception(f'Unknown synthetic data file type: {self.synthetic_filepath}')
 
         common_columns = list(set(self.synthetic_data.columns.tolist()).intersection(
             set(self.target_data.columns.tolist())
@@ -106,22 +155,25 @@
         self.synthetic_data = self.synthetic_data[common_columns]
 
         ind_features = [c for c in self.target_data.columns.tolist()
                         if c.startswith('IND_')]
         self.features = list(set(self.features).difference(set(ind_features)))
         self.features = list(set(self.features).intersection(list(common_columns)))
 
-        # raw data
+        self.feature_space = compute_feature_space(self.data_dict, self.features)
+
+        # raw subset data
         self.target_data = self.target_data[self.features]
         self.synthetic_data = self.synthetic_data[self.features]
 
         # validation and clean data
-        self.c_synthetic_data, self.validation_log \
-            = validate(self.synthetic_data, self.schema, self.features, self.log)
-        self.c_target_data, _ = validate(self.target_data, self.schema, self.features, self.log)
+        self.c_synthetic_data, self.validation_log = \
+            validate(self.synthetic_data, self.data_dict, self.features, self.log)
+        self.c_target_data, _ = \
+            validate(self.target_data, self.data_dict, self.features, self.log)
         self.features = self.c_synthetic_data.columns.tolist()
 
         # update data after validation and cleaning
         self.synthetic_data = self.synthetic_data[self.features]
         self.target_data = self.target_data[self.features]
 
         # sort columns in the data
@@ -129,23 +181,22 @@
         self.synthetic_data = self.synthetic_data.reindex(sorted(self.target_data.columns), axis=1)
         self.c_synthetic_data = self.c_synthetic_data.reindex(sorted(self.target_data.columns), axis=1)
         self.c_target_data = self.c_target_data.reindex(sorted(self.target_data.columns), axis=1)
         self.features = self.synthetic_data.columns.tolist()
 
         # bin the density feature if present in the datasets
         self.density_bin_desc = dict()
+
+        self.density_bin_desc = get_density_bins_description(self.raw_target_data,
+                                                             self.data_dict,
+                                                             self.mappings)
         if 'DENSITY' in self.features:
-            self.density_bin_desc = get_density_bins_description(self.c_target_data,
-                                                                 self.data_dict,
-                                                                 self.mappings)
             self.target_data = bin_density(self.c_target_data, self.data_dict)
             self.synthetic_data = bin_density(self.c_synthetic_data, self.data_dict)
 
-
-
         self.log.msg(f'Features ({len(self.features)}): {self.features}', level=3, timed=False)
         self.log.msg(f'Deidentified Data Records Count: {self.c_synthetic_data.shape[0]}', level=3, timed=False)
         self.log.msg(f'Target Data Records Count: {self.c_target_data.shape[0]}', level=3, timed=False)
 
         # update config to contain only available features
         self.config = unavailable_features(self.config, self.synthetic_data)
 
@@ -194,41 +245,58 @@
     def _fix_corr_features(features, corr_features):
         unavailable_features = set(corr_features).difference(features)
         return list(set(corr_features).difference(unavailable_features))
 
 
 def data_description(dataset: Dataset,
                      ui_data: ReportUIData,
+                     report_data: ReportData,
                      labels: Optional[Dict] = None) -> ReportUIData:
     ds = dataset
     r_ui_d = ui_data
 
+    dataset_report = dict()
+
     if labels is None:
         labels = dict()
 
-    r_ui_d.add_data_description(DatasetType.Target,
-                                DataDescriptionPacket(ds.target_data_path.stem,
+    target_desc = DataDescriptionPacket(ds.target_data_path.stem,
                                                       ds.target_data.shape[0],
-                                                      len(ds.target_data_features)))
+                                                      len(ds.target_data_features))
+    r_ui_d.add_data_description(DatasetType.Target,
+                                target_desc)
+    dataset_report['target'] = {"filename": ds.target_data_path.stem,
+                                "records": ds.target_data.shape[0],
+                                "features": len(ds.target_data_features)}
 
-    r_ui_d.add_data_description(DatasetType.Synthetic,
-                                DataDescriptionPacket(ds.synthetic_filepath.stem,
+    deid_desc = DataDescriptionPacket(ds.synthetic_filepath.stem,
                                                       ds.synthetic_data.shape[0],
                                                       ds.synthetic_data.shape[1],
                                                       labels,
-                                                      ds.validation_log))
+                                                      ds.validation_log)
+    r_ui_d.add_data_description(DatasetType.Synthetic,
+                                deid_desc)
+    dataset_report['deid'] = {"filename": ds.synthetic_filepath.stem,
+                              "records": ds.synthetic_data.shape[0],
+                              "features": ds.synthetic_data.shape[1],
+                              "labels": labels,
+                              "validations": ds.validation_log}
 
     f = dataset.features
     f = [_ for _ in dataset.data_dict.keys() if _ in f]
     ft = [dataset.schema[_]['dtype'] for _ in f]
     ft = ['object of type string' if _ == 'object' else _ for _ in ft]
     fd = [dataset.data_dict[_]['description'] for _ in f]
     hn = [True if 'has_null' in dataset.schema[_] else False for _ in f]
     r_ui_d.add_feature_description(f, fd, ft, hn)
 
+    dataset_report['features'] = r_ui_d.feature_desc['Evaluated Data Features'].data
+
+    report_data.add('data_description', dataset_report)
+
     # create data dictionary appendix attachments
     dd_as = []
     for feat in dataset.data_dict.keys():
         f_desc = dataset.data_dict[feat]['description']
         feat_title = f'{feat}: {f_desc}'
         if 'link' in dataset.data_dict[feat] and feat == 'INDP':
             data = f"<a href={dataset.data_dict[feat]['link']}>" \
@@ -236,26 +304,32 @@
                    f"Find codes by searching the string: {feat}, in " \
                    f"the ACS data dictionary"
             dd_as.append(Attachment(name=feat_title,
                                     _data=data,
                                     _type=AttachmentType.String))
 
         elif 'values' in dataset.data_dict[feat]:
-            data = [{f"{feat} Code": k,
-                     f"Code Description": v}
-                for k, v in dataset.data_dict[feat]['values'].items()
-            ]
             f_name = feat_title
             if 'link' in dataset.data_dict[feat] and feat in ['WGTP', 'PWGTP']:
                 s_data = f"<a href={dataset.data_dict[feat]['link']}>" \
                        f"See description of weights.</a>"
                 dd_as.append(Attachment(name=f_name,
                                         _data=s_data,
                                         _type=AttachmentType.String))
                 f_name = None
+
+            data = [{f"{feat} Code": k,
+                     f"Code Description": v}
+                for k, v in dataset.data_dict[feat]['values'].items()
+            ]
+            if feat == 'PUMA':
+                data = [{f"{feat} Code": k,
+                         f"Code Description": f'{st_code_to_str[k.split("-")[0]]}: {v}'}
+                        for k, v in dataset.data_dict[feat]['values'].items()
+                        ]
             dd_as.append(Attachment(name=f_name,
                                     _data=data,
                                     _type=AttachmentType.Table))
             if feat == 'DENSITY':
                 for bin, bdata in dataset.density_bin_desc.items():
                     bdc = bdata[1].columns.tolist()  # bin data columns
                     # report bin data: bin data format for report
```

### Comparing `sdnist-2.1.1/sdnist/report/dataset/binning.py` & `sdnist-2.2.0/sdnist/report/dataset/binning.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,17 @@
     else:
         d['binned_density'] = pd.cut(d['DENSITY'], bins=bins, labels=labels)
 
         d['bin_range'] = d['binned_density'].apply(lambda x: get_bin_range_log(x))
         return d
 
 
-def get_density_bins_description(data: pd.DataFrame, data_dict: Dict, mappings: Dict) -> Dict:
+def get_density_bins_description(data: pd.DataFrame,
+                                 data_dict: Dict,
+                                 mappings: Dict) -> Dict:
     bin_desc = dict()
     # If puma is not available in the features, return empty description dictionary
     if 'PUMA' not in data:
         return bin_desc
 
     d = bin_density(data.copy(), data_dict, update=False)
```

### Comparing `sdnist-2.1.1/sdnist/report/dataset/transform.py` & `sdnist-2.2.0/sdnist/report/dataset/transform.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/report/dataset/validate.py` & `sdnist-2.2.0/sdnist/report/dataset/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, Optional, List
 import pandas as pd
 
 from sdnist.utils import SimpleLogger
 
 def validate(synth_data: pd.DataFrame,
-             schema: Dict,
+             data_dict: Dict,
              features: List[str],
              log: Optional[SimpleLogger] = None):
     """
     Removes all columns with the out of bound values.
     """
     def console_out(text: str):
         if log is not None:
@@ -27,77 +27,80 @@
         }
         sd = sd.dropna()
         console_out(f'Found {len(nan_df)} records with NaN values. '
                     f'Removed records with NaN values.')
 
     for f in features:
         # check feature has out of bound value
-        f_data = schema[f]
+        f_data = data_dict[f]
         has_nan = f in nan_features
+        has_N = 'N' in f_data['values'] if f != 'INDP' else True
+        f_vals = f_data['values'] if "values" in f_data else []
 
-        if 'min' in f_data:
+        if 'min' in f_vals:
             fd = sd[[f]].copy()
-            mask = fd[fd[f] != 'N'].index if 'has_null' in f_data else fd.index
+            mask = fd[fd[f] != 'N'].index if has_N else fd.index
             fd.loc[mask, f] = pd.to_numeric(fd.loc[mask, f], errors="coerce")
             nans = fd[fd.isna().any(axis=1)]
             if len(nans):
                 vob_vals = list(set(synth_data.loc[nans.index, f].values.tolist()))
                 vob_features.append((f, vob_vals))
                 console_out(f'Value out of bound for feature {f}, '
                       f'out of bound values: {vob_vals}. '
                             f'Dropping feature from evaluation.')
 
-            mask = sd[sd[f] != 'N'].index if 'has_null' in f_data else sd.index
+            mask = sd[sd[f] != 'N'].index if has_N else sd.index
 
             if f in ['PINCP'] and not len(nans):
                 sd.loc[mask, f] = pd.to_numeric(sd.loc[mask, f])
                 sd.loc[mask, f] = sd.loc[mask, f].astype(float)
             elif not len(nans):
                 sd.loc[mask, f] = pd.to_numeric(sd.loc[mask, f])
                 sd.loc[mask, f] = sd.loc[mask, f].astype(int)
         elif f == 'PUMA':
             # values intersection
             f_unique = sd['PUMA'].unique().tolist()
-            v_intersect = set(f_unique).intersection(set(f_data['values']))
+            v_intersect = set(f_unique).intersection(set(f_vals))
             if len(v_intersect) < len(f_unique):
                 vob_vals = list(set(f_unique).difference(v_intersect))
                 vob_features.append((f, vob_vals))
                 console_out(f'Value out of bound for feature {f}, '
                             f'out of bound values: {vob_vals}. Dropping feature from evaluation.')
         else:
             fd = sd[[f]].copy()
-            mask = fd[fd[f] != 'N'].index if 'has_null' in f_data else fd.index
+            mask = fd[fd[f] != 'N'].index if has_N else fd.index
             fd.loc[mask, f] = pd.to_numeric(fd.loc[mask, f], errors="coerce")
             nans = fd[fd.isna().any(axis=1)]
             vob_vals = []
             if len(nans):
                 vob_vals.extend(list(set(synth_data.loc[nans.index, f].values.tolist())))
                 fd = fd.dropna()
 
-            mask = fd[fd[f] != 'N'].index if 'has_null' in f_data else fd.index
+            mask = fd[fd[f] != 'N'].index if has_N else fd.index
             fd.loc[mask, f] = fd.loc[mask, f].astype(int)
-            real_vals = f_data['values']
-            if 'N' in real_vals:
-                real_vals.remove('N')
+
             if f != 'INDP':
+                real_vals = list(f_vals.keys())
+                if 'N' in real_vals:
+                    real_vals.remove('N')
                 f_unique = set(fd.loc[mask, f].unique().tolist())
                 real_vals = [int(v) for v in real_vals]
                 v_intersect = set(f_unique).intersection(set(real_vals))
                 if len(v_intersect) < len(f_unique):
                     vob_vals.extend(list(set(f_unique).difference(v_intersect)))
 
             if len(vob_vals):
                 vob_features.append((f, vob_vals))
                 console_out(f'Value out of bound for feature {f}, '
                       f'out of bound values: {vob_vals}. Dropping feature from evaluation.')
             else:
-                mask = sd[sd[f] != 'N'].index if 'has_null' in f_data else sd.index
+                mask = sd[sd[f] != 'N'].index if has_N else sd.index
                 sd.loc[mask, f] = pd.to_numeric(sd.loc[mask, f])
                 sd.loc[mask, f] = sd.loc[mask, f].astype(int)
-        if 'has_null' in f_data:
+        if has_N:
             sd[f] = sd[f].astype(object)
 
         if len(vob_features):
             last_vob_f, vob_vals = vob_features[-1]
 
             if last_vob_f == f:
                 sd = sd.loc[:, sd.columns != f]
```

### Comparing `sdnist-2.1.1/sdnist/report/generate.py` & `sdnist-2.2.0/sdnist/report/generate.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/report/plots/apparent_match_dist.py` & `sdnist-2.2.0/sdnist/report/plots/apparent_match_dist.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/report/plots/correlation.py` & `sdnist-2.2.0/sdnist/report/plots/correlation.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/report/plots/grid.py` & `sdnist-2.2.0/sdnist/report/plots/grid.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/report/plots/pearson_correlation.py` & `sdnist-2.2.0/sdnist/report/plots/pearson_correlation.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/report/plots/propensity.py` & `sdnist-2.2.0/sdnist/report/plots/propensity.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/report/plots/univariate.py` & `sdnist-2.2.0/sdnist/report/plots/univariate.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 class UnivariatePlots:
     def __init__(self,
                  synthetic: pd.DataFrame,
                  target: pd.DataFrame,
                  dataset: Dataset,
                  output_directory: Path,
                  challenge: str = CENSUS,
-                 n: int = 3):
+                 worst_univariates_to_display: Optional[int] = None):
         """
         Computes and creates univariate distribution plots of the worst
         performing variables in synthetic data
 
         Parameters
         ----------
             synthetic : pd.Dataframe
@@ -63,15 +63,15 @@
         self.syn = synthetic
         self.tar = target
 
         self.schema = dataset.schema
         self.dataset = dataset
         self.o_dir = output_directory
         self.out_path = Path(self.o_dir, 'univariate')
-        self.n = n
+        self.worst_univariates_to_display = worst_univariates_to_display
         self.challenge = challenge
         self.feat_data = dict()
         self._setup()
 
         self.div_data = None  # feature divergence data
         self.uni_counts = dict()  # univariate counts of target and synthetic data
 
@@ -225,27 +225,29 @@
                 self.uni_counts[f] = {
                     "counts": relative_path(save_data_frame(c_sort_merged.copy(),
                                                             o_path,
                                                             f'{f}_counts')),
                     "plot": relative_path(file_path)
                 }
 
-                self.feat_data[title] = dict()
-                if c1 >= c2*3 or f in ['PINCP']:
-                    f_val = c_sort_merged.loc[0, f]
-                    f_tc = c_sort_merged.loc[0, 'count_target']
-                    f_sc = c_sort_merged.loc[0, 'count_deidentified']
-                    c_sort_merged = c_sort_merged[~c_sort_merged[f].isin([f_val])]
-                    self.feat_data[title] = {
-                        "excluded": {
-                            "feature_value": f_val,
-                            "target_counts": int(f_tc),
-                            "deidentified_counts": int(f_sc)
+                if self.worst_univariates_to_display is None \
+                        or i < self.worst_univariates_to_display:
+                    self.feat_data[title] = dict()
+                    if c1 >= c2*3 or f in ['PINCP']:
+                        f_val = c_sort_merged.loc[0, f]
+                        f_tc = c_sort_merged.loc[0, 'count_target']
+                        f_sc = c_sort_merged.loc[0, 'count_deidentified']
+                        c_sort_merged = c_sort_merged[~c_sort_merged[f].isin([f_val])]
+                        self.feat_data[title] = {
+                            "excluded": {
+                                "feature_value": f_val,
+                                "target_counts": int(f_tc),
+                                "deidentified_counts": int(f_sc)
+                            }
                         }
-                    }
 
                 merged = c_sort_merged.sort_values(by=f)
 
                 x_axis = np.arange(merged.shape[0])
                 plt.bar(x_axis - 0.2, merged['count_target'], width=bar_width, label='Target')
                 plt.bar(x_axis + 0.2, merged['count_deidentified'], width=bar_width, label='Deidentified')
                 plt.xlabel('Feature Values')
@@ -280,17 +282,19 @@
 
                 plt.title(title,
                           fontdict={'fontsize': 12})
 
                 plt.savefig(Path(o_path, f'{f}.jpg'), bbox_inches='tight')
                 plt.close()
 
-                # if i < 3:
-                saved_file_paths.append(file_path)
-                self.feat_data[title]['path'] = file_path
+                if self.worst_univariates_to_display is None \
+                        or i < self.worst_univariates_to_display:
+                    saved_file_paths.append(file_path)
+                    self.feat_data[title]['path'] = file_path
+
         return saved_file_paths
 
 
 def divergence(synthetic: pd.DataFrame,
                target: pd.DataFrame,
                schema: Dict[str, any],
                ignore_features: Optional[List[str]] = None):
```

### Comparing `sdnist-2.1.1/sdnist/report/report_data.py` & `sdnist-2.2.0/sdnist/report/report_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     Target = "target"
     Synthetic = "synthetic"
 
 
 class EvaluationType(Enum):
     Utility = "utility"
     Privacy = "privacy"
+    Meta = "meta"
+    Motivation = "motivation"
+    Observations = "observations"
 
 
 class AttachmentType(Enum):
     Table = "table"
     WideTable = 'wide_table'
     ImageLinks = "image_links"
     ImageLinksHorizontal = "image_links_horizontal"
@@ -141,26 +144,29 @@
                 in zip(self.features, self.feature_desc, self.feature_types, self.has_nans)]
 
 
 @dataclass
 class ReportUIData:
     output_directory: Path = REPORTS_DIR
     # dictionary containing description of datasets
-    datasets: Dict[str, DataDescriptionPacket] = field(default_factory=dict, init=False)
+    datasets: Dict[str, List[DataDescriptionPacket]] = field(default_factory=dict, init=False)
     feature_desc: Dict[str, any] = field(default_factory=dict, init=False)
     # list containing ScorePacket objects
     scores: List[ScorePacket] = field(default_factory=list, init=False)
 
     def add(self, score_packet: ScorePacket):
         self.scores.append(score_packet)
 
     def add_data_description(self,
                              dataset_type: DatasetType,
                              data_description: DataDescriptionPacket):
-        self.datasets[dataset_type.value] = data_description
+        if dataset_type.value in self.datasets:
+            self.datasets[dataset_type.value].append(data_description)
+        else:
+            self.datasets[dataset_type.value] = [data_description]
 
     def add_feature_description(self,
                                 features: List[str],
                                 feature_desc: List[str],
                                 dtypes: List[str],
                                 has_nans: List[bool]):
         dp = FeatureDescriptionPacket(features=features,
@@ -172,27 +178,36 @@
     @property
     def data(self) -> Dict[str, any]:
         d = dict()
         d['Created on'] = datetime.datetime.now().strftime("%B %d, %Y %H:%M:%S")
         d['version'] = __version__
         d[strs.DATA_DESCRIPTION] = dict()
         for d_type_name, d_desc in self.datasets.items():
-            d[strs.DATA_DESCRIPTION][d_type_name] = d_desc.data
+            d[strs.DATA_DESCRIPTION][d_type_name] = [desc.data for desc in d_desc]
 
         for k, v in self.feature_desc.items():
             d[strs.DATA_DESCRIPTION][k] = v.data
 
         d[EvaluationType.Utility.value] = []
         d[EvaluationType.Privacy.value] = []
+        d['comparisons'] = []
+        d['motivation'] = []
+        d['observations'] = []
 
         for s_pkt in self.scores:
             if s_pkt.evaluation_type == EvaluationType.Utility:
                 d[EvaluationType.Utility.value].append(s_pkt.data)
             elif s_pkt.evaluation_type == EvaluationType.Privacy:
                 d[EvaluationType.Privacy.value].append(s_pkt.data)
+            elif s_pkt.evaluation_type == EvaluationType.Meta:
+                d['comparisons'].append(s_pkt.data)
+            elif s_pkt.evaluation_type == EvaluationType.Motivation:
+                d['motivation'].append(s_pkt.data)
+            elif s_pkt.evaluation_type == EvaluationType.Observations:
+                d['observations'].append(s_pkt.data)
             elif s_pkt.evaluation_type == None:
                 d['Appendix'] = [s_pkt.data]
         return d
 
     def save(self, output_path: Optional[Path] = None):
         o_path = Path(self.output_directory, 'ui.json')
```

### Comparing `sdnist-2.1.1/sdnist/report/resources/templates/main.jinja2` & `sdnist-2.2.0/sdnist/report/resources/templates/main.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -307,17 +307,19 @@
             <div class="horizontal-img">
                 <img src={{ image_link['path'] }} alt={{ image_link['image_name'] }}>
             </div>
         {% endfor %}
     </div>
 {% endmacro %}
 
-{% macro data_description(title, key) %}
+{% macro data_description(title, key, index) %}
     {{ heading_2(title) }}
-    {% set ddict=data['data_description'][key] %}
+
+    {% set ddict=data['data_description'][key][index] %}
+
     {% if 'label' in ddict %}
         <div>
             <p ><span style="color: var(--theme-color); font-weight: bold">
                 Deidentified data label:</span>
                 <b>{{ ddict['label'] }}</b></p>
         </div>
 {#        {% set ddict=ddict['data'] %}#}
@@ -351,14 +353,29 @@
         </div>
     {% elif data.startswith('h3') %}
         <div>
             {{ heading_3(data[2:]) }}
         </div>
     {% elif data.startswith('h4') %}
         {{ heading_4(data[2:]) }}
+    {% elif '-Highlight-' in data %}
+        <div>
+            {% set parts = data.split('-Highlight-') %}
+            <p style="margin-bottom: 0px">
+            {% for i, part in enumerate(parts) %}
+                {% if i%2 == 0 %}
+                    {{ part }}
+                {% else %}
+                    <span style="color: var(--theme-color); font-weight: bold">
+                        {{ part }}
+                    </span>
+                {% endif %}
+            {% endfor %}
+            </p>
+        </div>
     {% else %}
         <div>
             {{ data }}
         </div>
     {% endif %}
 {% endmacro %}
 
@@ -436,16 +453,25 @@
                     href="https://github.com/usnistgov/SDNist">
                     SDNIST v{{ data['version'] }}
                 </a>
             </p>
         </div>
         <div class="heading-2-div">
             {{ section_title('Data Description') }}
-            {{ data_description('Deidentified (Deid.) Data', 'synthetic') }}
-            {{ data_description('Target Data', 'target')}}
+            {% if 'synthetic' in data['data_description'] %}
+                {% for i, _ in enumerate(data['data_description']['synthetic']) %}
+                    {% set ddict=data['data_description'] %}
+                    {{ data_description('Deidentified (Deid.) Data', 'synthetic', i) }}
+                {% endfor %}
+            {% endif %}
+            {% if 'target' in data['data_description'] %}
+                {% for i, _ in enumerate(data['data_description']['target']) %}
+                    {{ data_description('Target Data', 'target', i) }}
+                {% endfor %}
+            {% endif %}
             {{ feature_description('Evaluated Data Features')}}
         </div>
         <br>
         <div class="heading-2-div">
             {{ section_title('Utility Evaluation') }}
             {% for i, item in enumerate(data['utility']) %}
                 <div class="evaluation-div">
```

#### html2text {}

```diff
@@ -24,16 +24,17 @@
 {% endif %} {% endmacro %} {% macro draw_images(data) %} {% for image_link in
 data %}
 'path'] }} alt={{ image_link['image_name'] }}>
 {% endfor %} {% endmacro %} {% macro draw_images_horizontal(data) %}
 {% for image_link in data %}
 'path'] }} alt={{ image_link['image_name'] }}>
 {% endfor %}
-{% endmacro %} {% macro data_description(title, key) %} {{ heading_2(title) }}
-{% set ddict=data['data_description'][key] %} {% if 'label' in ddict %}
+{% endmacro %} {% macro data_description(title, key, index) %} {{ heading_2
+(title) }} {% set ddict=data['data_description'][key][index] %} {% if 'label'
+in ddict %}
 Deidentified data label: {{ ddict['label'] }}
 {# {% set ddict=ddict['data'] %}#} {% elif 'labels' in ddict %} {{ table(ddict
 ['labels']) }}
 {# {% set ddict=ddict['data'] %}#} {# {% else %}#} {# {% set ddict=ddict
 ['data'] %}#} {% endif %}
 {{ table(ddict['data']) }} {% if ddict['validations']|length %}
 {{ string_data('Following features has out of bound values, and these are not
@@ -41,15 +42,20 @@
 {{ table(ddict['validations']) }} {% endif %} {% endmacro %} {% macro
 feature_description(title) %} {{ heading_2(title) }} {{ table(data
 ['data_description'][title]) }} {% endmacro %} {% macro string_data(data) %} {%
 if data.startswith('Highlight-') %}
 {{ data[10:] }}
 {% elif data.startswith('h3') %}
 {{ heading_3(data[2:]) }}
-{% elif data.startswith('h4') %} {{ heading_4(data[2:]) }} {% else %}
+{% elif data.startswith('h4') %} {{ heading_4(data[2:]) }} {% elif '-Highlight-
+' in data %}
+{% set parts = data.split('-Highlight-') %}
+{% for i, part in enumerate(parts) %} {% if i%2 == 0 %} {{ part }} {% else %}
+{{ part }}  {% endif %} {% endfor %}
+{% else %}
 {{ data }}
 {% endif %} {% endmacro %} {% macro evaluation(data) %} {{ heading_2(data
 ['metric_name']) }} {% if 'scores' in data %}
 Score: {{ data['scores'] }}
 {% endif %} {% for i, a in enumerate(data['attachments']) %} {% if a.type ==
 'image_links' and i > 0 %} {% set style = 'attachment-div-break' %} {% else %}
 {% set style = 'attachment-div' %} {% endif %} {% if a.dotted_break == True and
@@ -72,17 +78,22 @@
 ===============================================================================
 #} {#
 #} {# {% endif %}#} {% endfor %} {% endmacro %}
 ****** Data Evaluation Report ******
 
 Report created on: {{ data['Created on'] }}
 Created with SDNIST_v{{_data['version']_}}
-{{ section_title('Data Description') }} {{ data_description('Deidentified
-(Deid.) Data', 'synthetic') }} {{ data_description('Target Data', 'target')}} {
-{ feature_description('Evaluated Data Features')}}
+{{ section_title('Data Description') }} {% if 'synthetic' in data
+['data_description'] %} {% for i, _ in enumerate(data['data_description']
+['synthetic']) %} {% set ddict=data['data_description'] %} {{ data_description
+('Deidentified (Deid.) Data', 'synthetic', i) }} {% endfor %} {% endif %} {% if
+'target' in data['data_description'] %} {% for i, _ in enumerate(data
+['data_description']['target']) %} {{ data_description('Target Data', 'target',
+i) }} {% endfor %} {% endif %} {{ feature_description('Evaluated Data
+Features')}}
 
 {{ section_title('Utility Evaluation') }} {% for i, item in enumerate(data
 ['utility']) %}
 {% if i > 0 %}
 
 
 {% endif %} {{ evaluation(item) }}
```

### Comparing `sdnist-2.1.1/sdnist/report/score/paragraphs.py` & `sdnist-2.2.0/sdnist/report/score/paragraphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,18 +62,23 @@
                  "in the target data. Can we be sure that the deidentified data does not include real people? " \
                  "The apparent match metric first considers which deidentified individuals look like they might be " \
                  "real people (they are unique matches on quasi-identifier features) and then considers whether " \
                  "the deidentified records actually represent real individuals. "
 
 quasi_idf_para = "These features are used to determine if a deidentified record looks like it might be a real person in the target data."
 
-rec_matched_para = "Based only on the quasi-identifier features, how many deidentified " \
-                   "records uniquely match an individual in the target data? What percentage of the " \
-                   "deidentified data has apparent real matches?"
+rec_matched_para = "Based only on the quasi-identifier features, how much of the target data has " \
+                   "apparent unique matches in the deidentified data? and then the " \
+                   "percent should be a percent of target data"
 
 percn_matched_para = "Considering the set of apparent matches, to what extent are they real matches? " \
                      "This distribution shows edit similarity between apparently matched pairs on how many of " \
                      "the 22 features does the deidentified record have the same value as the real record. " \
                      "If the distribution is centered near 100% that means these deidentified records largely " \
                      "mimic target records and are potentially leaking information about real individuals. " \
                      "If the distribution is centered below 50% that means the deidentified records are very " \
-                     "different from the target records, and the apparent matches are not real matches."
+                     "different from the target records, and the apparent matches are not real matches."
+
+unique_exact_match_para = "This is a count of unique records in the target data that were exactly reproduced " \
+                          "in the deidentified data. Because these records were unique outliers in the " \
+                          "target data, and they still appear unchanged in the deidentified data, " \
+                          "they are potentially vulnerable to reidentification."
```

#### html2text {}

```diff
@@ -50,19 +50,23 @@
 individuals " \ "in the target data. Can we be sure that the deidentified data
 does not include real people? " \ "The apparent match metric first considers
 which deidentified individuals look like they might be " \ "real people (they
 are unique matches on quasi-identifier features) and then considers whether " \
 "the deidentified records actually represent real individuals. " quasi_idf_para
 = "These features are used to determine if a deidentified record looks like it
 might be a real person in the target data." rec_matched_para = "Based only on
-the quasi-identifier features, how many deidentified " \ "records uniquely
-match an individual in the target data? What percentage of the " \
-"deidentified data has apparent real matches?" percn_matched_para =
-"Considering the set of apparent matches, to what extent are they real matches?
-" \ "This distribution shows edit similarity between apparently matched pairs
-on how many of " \ "the 22 features does the deidentified record have the same
-value as the real record. " \ "If the distribution is centered near 100% that
-means these deidentified records largely " \ "mimic target records and are
-potentially leaking information about real individuals. " \ "If the
-distribution is centered below 50% that means the deidentified records are very
-" \ "different from the target records, and the apparent matches are not real
-matches."
+the quasi-identifier features, how much of the target data has " \ "apparent
+unique matches in the deidentified data? and then the " \ "percent should be a
+percent of target data" percn_matched_para = "Considering the set of apparent
+matches, to what extent are they real matches? " \ "This distribution shows
+edit similarity between apparently matched pairs on how many of " \ "the 22
+features does the deidentified record have the same value as the real record. "
+\ "If the distribution is centered near 100% that means these deidentified
+records largely " \ "mimic target records and are potentially leaking
+information about real individuals. " \ "If the distribution is centered below
+50% that means the deidentified records are very " \ "different from the target
+records, and the apparent matches are not real matches."
+unique_exact_match_para = "This is a count of unique records in the target data
+that were exactly reproduced " \ "in the deidentified data. Because these
+records were unique outliers in the " \ "target data, and they still appear
+unchanged in the deidentified data, " \ "they are potentially vulnerable to
+reidentification."
```

### Comparing `sdnist-2.1.1/sdnist/report/score/utility/__init__.py` & `sdnist-2.2.0/sdnist/report/score/utility/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     s = s[dataset.synthetic_data[feature].isin(wpf)]
 
     out_dir = Path(r_ui_d.output_directory, 'k_marginal_breakdown')
     if not out_dir.exists():
         os.mkdir(out_dir)
 
     up = UnivariatePlots(s, t,
-                         ds, out_dir, ds.challenge)
+                         ds, out_dir, ds.challenge, worst_univariates_to_display=3)
     u_feature_data = up.save()
     k_marg_break_rd[f'worst_{len(wpf)}_puma_univariate'] = up.report_data()
     k_marg_break_rd[f'worst_{len(wpf)}_puma_k_marginal_scores'] = \
         relative_path(save_data_frame(wsh,
                                       out_dir,
                                       f'worst_{len(wpf)}_puma_k_marginal_scores'))
     u_as = []
@@ -162,15 +162,17 @@
                 f_detail = '[N/A]'
                 if 'values' in ds.data_dict[f_name]:
                     f_detail = ds.data_dict[f_name]['values']['N']
                 fv = f'N [{f_detail}]'
             else:
                 f_detail = ''
                 if 'values' in ds.data_dict[f_name]:
-                    f_detail = ds.data_dict[f_name]['values'][str(fv)]
+                    v_data = ds.data_dict[f_name]['values']
+                    if str(fv) in v_data:
+                        f_detail = ds.data_dict[f_name]['values'][str(fv)]
                 fv = f'{fv} [{f_detail}]'
             a = Attachment(name=None,
                            _data=f"Feature Values not shown in the chart:"
                                  f"<br>Value: {fv}"
                                  f"<br>Target Data Counts: {tc}"
                                  f"<br>Deidentified Data Counts: {sc}",
                            _type=AttachmentType.String)
@@ -509,15 +511,17 @@
                     f_detail = '[N/A]'
                     if 'values' in ds.data_dict[f_name]:
                         f_detail = ds.data_dict[f_name]['values']['N']
                     fv = f'N [{f_detail}]'
                 else:
                     f_detail = ''
                     if 'values' in ds.data_dict[f_name]:
-                        f_detail = ds.data_dict[f_name]['values'][str(fv)]
+                        v_data = ds.data_dict[f_name]['values']
+                        if str(fv) in v_data:
+                            f_detail = ds.data_dict[f_name]['values'][str(fv)]
                     fv = f'{fv} [{f_detail}]'
 
                 a = Attachment(name=None,
                                _data=f"Feature Values not shown in the chart:"
                                      f"<br>Value: {fv}"
                                      f"<br>Target Data Counts: {tc}"
                                      f"<br>Deidentified Data Counts: {sc}",
```

### Comparing `sdnist-2.1.1/sdnist/report/score/utility/inconsistency.py` & `sdnist-2.2.0/sdnist/report/score/utility/inconsistency.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/report/score/utility/linear_regression.py` & `sdnist-2.2.0/sdnist/report/score/utility/linear_regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,19 +40,20 @@
 
         "For this metric we're just looking at data from adults (AGEP > 15) and "
         "we're only considering the distribution of the data across two features:"
         "<ul>"
         "<li>EDU: The highest education level this individual has attained, ranging "
         "from 1 (elementary school) to 12 (PhD). See Appendix of this report for "
         "the full list of code values.</li>"
-        "<li>PINCP_DECILE: The individual's income decile relative to their PUMA. "
+        "<li>PINCP_DECILE: The individual's income rank relative to other incomes from "
+        "their state, discretized into ten equal-width range bins. "
         "This helps us account for differences in cost of living across the country. "
-        "If an individual makes a moderate income but lives in a very low income area, "
+        "If an individual makes a moderate income but lives in a lower income area, "
         "they may have a high value for PINCP_DECILE indicating that they have a high "
-        "income for their PUMA).</li>"
+        "income for their state. </li>"
         "</ul>",
 
         "The basic idea is that higher values of EDU should lead to higher values of "
         "PINCP_DECILE, and this is broadly true. However, it is known that the relationship "
         "between EDU and PINCP_DECILE is different for different demographic subgroups. "
         "The heatmaps in the left column below show the density distribution of the true "
         "data for each subgroup, normalized by education category (so the density values "
```

### Comparing `sdnist-2.1.1/sdnist/report/score/utility/pca.py` & `sdnist-2.2.0/sdnist/report/score/utility/pca.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,24 +83,19 @@
 
         # Add json report data for pca
         pca_rd = {
          "components_eigenvector": relative_path(
              save_data_frame(pca_m.comp_df,
                              o_path,
                              'components_eigenvector')),
-         "target_components": relative_path(
-             save_data_frame(pca_m.t_pdf,
-                             o_path,
-                             'target_components')),
-         "deidentified_components": relative_path(
-             save_data_frame(pca_m.s_pdf,
-                             o_path,
-                             'deidentified_components')),
          "target_all_components_plot": relative_path(acpp_tar),
-         "deidentified_all_components_plot": relative_path(acpp_deid)
+         "deidentified_all_components_plot": relative_path(acpp_deid),
+         "highlighted_plots": {f'{k[0]}-{k[1]}-{k[2]}':
+                                   [relative_path(v[0], 3), relative_path(v[1], 3)]
+             for k, v in plot_paths[strs.HIGHLIGHTED].items()}
         }
 
         self.rd.add('pca', pca_rd)
 
         # create attachment objects for report UI data
         rel_pca_plot_paths = relative_path([acpp_tar, acpp_deid])
```

### Comparing `sdnist-2.1.1/sdnist/report/server.py` & `sdnist-2.2.0/sdnist/report/server.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/schema.py` & `sdnist-2.2.0/sdnist/schema.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/strs.py` & `sdnist-2.2.0/sdnist/strs.py`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist/utils.py` & `sdnist-2.2.0/sdnist/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import shutil
 from typing import List, Union, Optional
 import numpy as np
 import pandas as pd
 import json
 import os
 import time
 import sys
@@ -155,14 +156,28 @@
                 for p in path]
 
 
 def create_path(path: Path):
     if not path.exists():
         os.mkdir(path)
 
+def remove_path(path: Path):
+    if path.exists():
+        shutil.rmtree(str(path))
+
+def adaptive_round(decimal_num):
+    dn = decimal_num
+
+    l = 10
+    round_by = 2
+    for i in range(1, l+1):
+        if 10**i * dn >= 1:
+            round_by = i + 1
+            break
+    return round(dn, round_by)
 
 def to_num(data: pd.DataFrame) -> pd.DataFrame:
     """Converts data to numeric and drops all the records
     with N values"""
     d = data
 
     for f in d.columns:
```

### Comparing `sdnist-2.1.1/sdnist/visualizer_resources/report2.jinja2` & `sdnist-2.2.0/sdnist/visualizer_resources/report2.jinja2`

 * *Files identical despite different names*

### Comparing `sdnist-2.1.1/sdnist.egg-info/PKG-INFO` & `sdnist-2.2.0/sdnist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: sdnist
-Version: 2.1.1
+Version: 2.2.0
 Summary: SDNist: Deidentified Data Report Generator
 Home-page: https://github.com/usnistgov/SDNist
 Author: National Institute of Standards and Technology
 Author-email: gary.howarth@nist.gov
 License: UNKNOWN
-Description: # SDNist v2.1: Deidentified Data Report Tool
+Description: # SDNist v2.2: Deidentified Data Report Tool
         
         ## [SDNist is the offical software package for engaging in the NIST Collaborative Research Cycle](https://pages.nist.gov/privacy_collaborative_research_cycle)
         
-        Welcome! SDNist v2.1 is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
+        Welcome! SDNist is a python package that provides benchmark data and evaluation metrics for deidentified data generators. This version of SDNist supports using the [NIST Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts), a geographically partioned, limited feature data set.
         
         The deidentified data report evaluates utility and privacy of a given deidentified dataset and generates a summary quality report with performance of a deidentified dataset enumerated and illustrated for each utility and privacy metric.
         
         [Preview sample reports produced by the tool here.](https://github.com/usnistgov/SDNist/tree/main/sdnist/report/sample-reports)
         
         This tool is being actively developed. Please (raise an Issue)[https://github.com/usnistgov/SDNist/issues]  if you catch a bug or would like have feature suggestions. 
         
@@ -37,16 +37,18 @@
         
         
         Setting Up the SDNIST Report Tool
         ------------------------
         
         ### Brief Setup Instructions
         
-        SDNist v2.1 requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend uninstalling or installing v2.1 in a virtual environment. v2.1 can be installed via [Release 2.1](https://github.com/usnistgov/SDNist/releases/tag/v2.1.1). The NIST Diverse Community Exceprt data will download on the fly.
-        
+        SDNist requires Python version 3.7 or greater. If you have installed a previous version of the SDNist library, we recommend uninstalling or installing v2.2 in a virtual environment. v2.2 can be installed via [Release 2.2](https://github.com/usnistgov/SDNist/releases/tag/v2.2.0). The NIST Diverse Community Exceprt data will download on the fly.
+        ```
+        pip install sdnist
+        ```
         
         ### Detailed Setup Instructions
         
         1. The SDNist Report Tool is a part of the sdnist Python library that can be installed on a user’s MAC OS, Windows, or Linux machine.
         
         
         2. The sdnist library requires Python version 3.7 or greater to be installed on the user's machine. Check whether an installation exists on the machine by executing the following command in your terminal on Mac/Linux or powershell on Windows:
@@ -57,18 +59,18 @@
         
         
         3.  Create a local directory/folder on the machine to set up the SDNist library. This guide assumes the local directory to be sdnist-project; an example of a complete file path is c:\\sdnist-project:
             ```
             c:\\sdnist-project>     
             ```
         
-        4.  Download the sdnist installable wheel (sdnist-2.1.1-py3-none-any.whl) from the Github: [Release 2.1](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/sdnist-2.1.1-py3-none-any.whl).
+        4.  Download the sdnist installable wheel (sdnist-2.2.0-py3-none-any.whl) from the Github: [Release 2.2](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/sdnist-2.2.0-py3-none-any.whl).
         
         
-        5.  Move the downloaded sdnist-2.1.1-py3-none-any.whl file to the sdnist-project directory.
+        5.  Move the downloaded sdnist-2.2.0-py3-none-any.whl file to the sdnist-project directory.
         
         
         6.  Using the terminal on Mac/Linux or powershell on Windows, navigate to the sdnist-project directory.
         
         
         7.  In the already-opened terminal or powershell window, execute the following command to create a new Python environment. The sdnist library will be installed in this newly created Python environment:
         
@@ -113,30 +115,30 @@
             ```
             Run the following command to let Windows execute scripts:
             ```
             Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope LocalMachine
             ```
         
         
-        10. Per step 5 above, the sdnist-2.1.1-py3-none-any.whl file should already be present in the sdnist-project directory. Check whether that is true by listing the files in the sdnist-project directory.
+        10. Per step 5 above, the sdnist-2.2.0-py3-none-any.whl file should already be present in the sdnist-project directory. Check whether that is true by listing the files in the sdnist-project directory.
         
               **MAC OS/Linux:**
                ```
                (venv) sdnist-project> ls
                ```
               **Windows:**
                ```
                (venv) c:\\sdnist-project> dir
                ```
-               The sdnist-2.1.1-py3-none-any.whl file should be in the list printed by the above command; otherwise, follow steps 4 and 5 again to download the .whl file.
+               The sdnist-2.2.0-py3-none-any.whl file should be in the list printed by the above command; otherwise, follow steps 4 and 5 again to download the .whl file.
         
         
         11. Install sdnist Python library:
                ```
-               (venv) c:\\sdnist-project> pip install sdnist-2.1.1-py3-none-any.whl
+               (venv) c:\\sdnist-project> pip install sdnist-2.2.0-py3-none-any.whl
                ```
         
         
         12. Installation is successful if executing the following command outputs a help menu for the sdnist.report package:
                ```
                (venv) c:\\sdnist-project> python -m sdnist.report -h
                ```
@@ -206,15 +208,15 @@
               ```
         
         
         5.  Use the following command to generate a data quality report for the example deidentified dataset (syn_national.csv) that is generated using the bundled dataset NATIONAL:
               ```
               (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL
               ```
-        6.  SDNist 2.1 allow users to add labels for the deidentified dataset used to generate report:
+        6.  Starting from version 2.1, SDNist allow users to add labels for the deidentified dataset used to generate report:
             * To add single string label to the report, use command line option **--labels** followed by a string as given in the following example command:
               ```
               (venv) c:\\sdnist-project> python -m sdnist.report syn_national.csv NATIONAL --labels used_epsilon_1
               ```
               This is how the string label *used_epsilon_1* will appear in the report:
               ![string label in report](readme_resource/string_label.png)
             * To add multiple string labels to the report, use command line option **--labels** followed by a path to the json file containing labels:
@@ -247,15 +249,15 @@
         ---------------------------------
         
         1.  The sdnist.report package comes with built-in datasets. The package will automatically download the datasets from Github if they are not already available locally on your machine. You should see following message on your terminal or powershell window when the datasets are downloaded by the sdnist.report package:
               ```
               (venv) c:\\sdnist-project> python -m sdnist.report syn_tx.csv TX
         
               Downloading all SDNist datasets from:  
-              https://github.com/usnistgov/SDNist/releases/download/v2.1.1/diverse_communities_data_excerpts.zip ...  
+              https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip ...  
               ...5%, 47352 KB, 8265 KB/s, 5 seconds elapsed
               ```
         
               Follow the next subsection, Download Data Manually, if the sdnist.report package is unable to download the datasets.
         
         
         2. All the datasets required by the sdnist.report package are installed into the sdnist _toy _data directory, which should be now present inside the sdnist-project directory. sdnist _toy _data is also a data root directory. You can use some other directory as a data root by providing the –data-root argument to the sdnist.report package. If you provide a –data-root argument with a path, the sdnist.report package will look for datasets in the data root directory you have specified, and the package will download it if it is not present in the data root.
@@ -265,15 +267,15 @@
         
            You can download a copy of the datasets from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/tree/main/nist%20diverse%20communities%20data%20excerpts). This copy is similar to the one bundled with the sdnist.report package, but it contains more documentation and a description of the datasets.
         
         
         4. You can download the toy deidentified datasets from Github [Sdnist Toy Deidentified Dataset](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/toy_deidentified_data.zip). Unzip the downloaded file, and move the unzipped toy_deidentified_dataset directory to the sdnist-project directory.
         
         
-        5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/diverse_communities_excerpts_data.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
+        5. Each toy deidentified dataset file is generated using the [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_excerpts_data.zip). The syn_ma.csv, syn_tx.csv, and syn_national.csv deidentified dataset files are created from target datasets MA (ma2019.csv), TX (tx2019.csv), and NATIONAL(national2019.csv), respectively. You can use one of the toy deidentified dataset files for testing whether the sdnist.report package is installed correctly on your system.
         
         
         6. Use the following commands for generating reports if you are using a toy deidentified dataset file:
         
            For evaluating the Massachusetts dataset:
            ```
            (venv) c:\\sdnist-project> python -m sdnist.report toy_deidentified_data/syn_ma.csv MA
@@ -292,15 +294,15 @@
         7.  A deidentified dataset can be a .csv or a parquet file, and the path of this file is required
         by the sdnist.report package to generate a data quality report.
         
         
         Download Data Manually
         ----------------------
         
-        1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.1.1/diverse_communities_data_excerpts.zip).
+        1.  If the sdnist.report package is not able to download the datasets, you can download them from Github [Diverse Communities Data Excerpts](https://github.com/usnistgov/SDNist/releases/download/v2.2.0/diverse_communities_data_excerpts.zip).
         3.  Unzip the **diverse_community_excerpts_data.zip** file and move the unzipped **diverse_community_excerpts_data** directory to the **sdnist-project** directory.
         4.  Delete the **diverse_community_excerpts_data.zip** file once the data is successfully extracted from the zip.
         
         Citing SDNist Deidentified Data Report Tool
         -------------------------------------------
         
         If you publish work that utilizes the SDNist Deidentified Data Tool, please cite the software. Citation recommendation:
```

### Comparing `sdnist-2.1.1/sdnist.egg-info/SOURCES.txt` & `sdnist-2.2.0/sdnist.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 sdnist/metrics/inconsistency.py
 sdnist/metrics/kmarg_old.py
 sdnist/metrics/kmarginal.py
 sdnist/metrics/pca.py
 sdnist/metrics/pearson_correlation.py
 sdnist/metrics/propensity.py
 sdnist/metrics/regression.py
+sdnist/metrics/unique_exact_matches.py
 sdnist/preprocess/__init__.py
 sdnist/report/__init__.py
 sdnist/report/__main__.py
 sdnist/report/common.py
 sdnist/report/config.json
 sdnist/report/generate.py
 sdnist/report/report_data.py
```

