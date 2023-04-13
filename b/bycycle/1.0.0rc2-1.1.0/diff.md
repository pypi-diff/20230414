# Comparing `tmp/bycycle-1.0.0rc2.tar.gz` & `tmp/bycycle-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bycycle-1.0.0rc2.tar", last modified: Wed Dec  9 23:26:50 2020, max compression
+gzip compressed data, was "bycycle-1.1.0.tar", last modified: Thu Apr 13 22:17:29 2023, max compression
```

## Comparing `bycycle-1.0.0rc2.tar` & `bycycle-1.1.0.tar`

### file list

```diff
@@ -1,82 +1,91 @@
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/
--rw-rw-r--   0 rph       (1000) rph       (1000)    11340 2020-10-19 22:50:29.000000 bycycle-1.0.0rc2/LICENSE
--rw-rw-r--   0 rph       (1000) rph       (1000)       41 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/MANIFEST.in
--rw-rw-r--   0 rph       (1000) rph       (1000)    12631 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/PKG-INFO
--rw-rw-r--   0 rph       (1000) rph       (1000)     9577 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/README.rst
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.107787 bycycle-1.0.0rc2/bycycle/
--rw-rw-r--   0 rph       (1000) rph       (1000)       97 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/__init__.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.107787 bycycle-1.0.0rc2/bycycle/burst/
--rw-rw-r--   0 rph       (1000) rph       (1000)      187 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/burst/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     2068 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/burst/amp.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     4423 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/burst/cycle.py
--rw-rw-r--   0 rph       (1000) rph       (1000)      157 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/burst/dualthresh.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     4595 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/burst/utils.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.107787 bycycle-1.0.0rc2/bycycle/cyclepoints/
--rw-rw-r--   0 rph       (1000) rph       (1000)      145 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/cyclepoints/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     5291 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/cyclepoints/extrema.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     3773 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/cyclepoints/phase.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     4559 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/cyclepoints/zerox.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.107787 bycycle-1.0.0rc2/bycycle/features/
--rw-rw-r--   0 rph       (1000) rph       (1000)      193 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/features/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)    12759 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/features/burst.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     2767 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/features/cyclepoints.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     6714 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/features/features.py
--rw-rw-r--   0 rph       (1000) rph       (1000)    12171 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/features/shape.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.107787 bycycle-1.0.0rc2/bycycle/group/
--rw-rw-r--   0 rph       (1000) rph       (1000)       95 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/group/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)    14519 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/group/features.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     5376 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/group/utils.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/bycycle/plts/
--rw-rw-r--   0 rph       (1000) rph       (1000)      222 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/plts/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)    10404 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/plts/burst.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     6121 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/plts/cyclepoints.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     5594 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/plts/features.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/bycycle/tests/
--rw-rw-r--   0 rph       (1000) rph       (1000)      170 2020-11-30 22:58:04.000000 bycycle-1.0.0rc2/bycycle/tests/__init__.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/bycycle/tests/burst/
--rw-rw-r--   0 rph       (1000) rph       (1000)        0 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/burst/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     1178 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/burst/test_amp.py
--rw-rw-r--   0 rph       (1000) rph       (1000)      952 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/burst/test_cycle.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     2461 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/burst/test_utils.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     2768 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/conftest.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/bycycle/tests/cyclepoints/
--rw-rw-r--   0 rph       (1000) rph       (1000)        0 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/cyclepoints/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     1689 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/cyclepoints/test_extrema.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     1046 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/cyclepoints/test_phase.py
--rw-rw-r--   0 rph       (1000) rph       (1000)      880 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/cyclepoints/test_zerox.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/bycycle/tests/features/
--rw-rw-r--   0 rph       (1000) rph       (1000)        0 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/features/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     2307 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/features/test_burst.py
--rw-rw-r--   0 rph       (1000) rph       (1000)      948 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/features/test_cyclepoints.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     1377 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/features/test_features.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     3992 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/features/test_shapes.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/bycycle/tests/group/
--rw-rw-r--   0 rph       (1000) rph       (1000)        0 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/group/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     4234 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/group/test_features.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     2071 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/group/test_utils.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/bycycle/tests/plts/
--rw-rw-r--   0 rph       (1000) rph       (1000)        0 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/plts/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     1839 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/plts/test_burst.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     1120 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/plts/test_cyclepoints.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     1465 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/plts/test_features.py
--rw-rw-r--   0 rph       (1000) rph       (1000)      506 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/settings.py
--rw-rw-r--   0 rph       (1000) rph       (1000)      831 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/tutils.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/bycycle/tests/utils/
--rw-rw-r--   0 rph       (1000) rph       (1000)        0 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/utils/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     3582 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/utils/test_dataframes.py
--rw-rw-r--   0 rph       (1000) rph       (1000)      666 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/tests/utils/test_timeseries.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/bycycle/utils/
--rw-rw-r--   0 rph       (1000) rph       (1000)      240 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/utils/__init__.py
--rw-rw-r--   0 rph       (1000) rph       (1000)      107 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/utils/checks.py
--rw-rw-r--   0 rph       (1000) rph       (1000)    12119 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/utils/dataframes.py
--rw-rw-r--   0 rph       (1000) rph       (1000)     1597 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/bycycle/utils/timeseries.py
--rw-rw-r--   0 rph       (1000) rph       (1000)       60 2020-12-09 21:08:21.000000 bycycle-1.0.0rc2/bycycle/version.py
-drwxrwxr-x   0 rph       (1000) rph       (1000)        0 2020-12-09 23:26:50.107787 bycycle-1.0.0rc2/bycycle.egg-info/
--rw-rw-r--   0 rph       (1000) rph       (1000)    12631 2020-12-09 23:26:50.000000 bycycle-1.0.0rc2/bycycle.egg-info/PKG-INFO
--rw-rw-r--   0 rph       (1000) rph       (1000)     1853 2020-12-09 23:26:50.000000 bycycle-1.0.0rc2/bycycle.egg-info/SOURCES.txt
--rw-rw-r--   0 rph       (1000) rph       (1000)        1 2020-12-09 23:26:50.000000 bycycle-1.0.0rc2/bycycle.egg-info/dependency_links.txt
--rw-rw-r--   0 rph       (1000) rph       (1000)       46 2020-12-09 23:26:50.000000 bycycle-1.0.0rc2/bycycle.egg-info/requires.txt
--rw-rw-r--   0 rph       (1000) rph       (1000)        8 2020-12-09 23:26:50.000000 bycycle-1.0.0rc2/bycycle.egg-info/top_level.txt
--rw-rw-r--   0 rph       (1000) rph       (1000)       48 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/requirements.txt
--rw-rw-r--   0 rph       (1000) rph       (1000)       38 2020-12-09 23:26:50.111787 bycycle-1.0.0rc2/setup.cfg
--rw-rw-r--   0 rph       (1000) rph       (1000)     2072 2020-12-09 21:03:12.000000 bycycle-1.0.0rc2/setup.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.435823 bycycle-1.1.0/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)    11340 2022-09-26 23:50:26.000000 bycycle-1.1.0/LICENSE
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)       41 2022-09-26 23:50:26.000000 bycycle-1.1.0/MANIFEST.in
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)    11674 2023-04-13 22:17:29.435619 bycycle-1.1.0/PKG-INFO
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)    10312 2023-04-13 22:13:55.000000 bycycle-1.1.0/README.rst
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.425460 bycycle-1.1.0/bycycle/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      137 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/__init__.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.427166 bycycle-1.1.0/bycycle/burst/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      187 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/burst/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     2080 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/burst/amp.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     4453 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/burst/cycle.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      157 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/burst/dualthresh.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     5712 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/burst/utils.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.427817 bycycle-1.1.0/bycycle/cyclepoints/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      145 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/cyclepoints/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     5621 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/cyclepoints/extrema.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     3773 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/cyclepoints/phase.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     4709 2023-04-13 21:53:38.000000 bycycle-1.1.0/bycycle/cyclepoints/zerox.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.428715 bycycle-1.1.0/bycycle/features/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      193 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/features/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)    14167 2023-04-13 21:53:38.000000 bycycle-1.1.0/bycycle/features/burst.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     2779 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/features/cyclepoints.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     7035 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/features/features.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)    12201 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/features/shape.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.429320 bycycle-1.1.0/bycycle/group/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)       95 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/group/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)    14519 2023-04-13 20:13:19.000000 bycycle-1.1.0/bycycle/group/features.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     5394 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/group/utils.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.429580 bycycle-1.1.0/bycycle/objs/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)       68 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/objs/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)    16569 2023-04-13 21:53:38.000000 bycycle-1.1.0/bycycle/objs/fit.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.430441 bycycle-1.1.0/bycycle/plts/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      222 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/plts/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)    10926 2023-04-13 21:53:38.000000 bycycle-1.1.0/bycycle/plts/burst.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     6147 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/plts/cyclepoints.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     5594 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/plts/features.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.431384 bycycle-1.1.0/bycycle/tests/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      170 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/__init__.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.431976 bycycle-1.1.0/bycycle/tests/burst/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)        0 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/burst/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     1178 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/burst/test_amp.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      952 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/burst/test_cycle.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     3082 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/tests/burst/test_utils.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     2784 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/tests/conftest.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.432480 bycycle-1.1.0/bycycle/tests/cyclepoints/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)        0 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/cyclepoints/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     1689 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/cyclepoints/test_extrema.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     1046 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/cyclepoints/test_phase.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      880 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/cyclepoints/test_zerox.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.433059 bycycle-1.1.0/bycycle/tests/features/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)        0 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/features/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     2307 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/features/test_burst.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      948 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/features/test_cyclepoints.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     1387 2023-04-13 21:53:38.000000 bycycle-1.1.0/bycycle/tests/features/test_features.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     4043 2023-04-13 21:53:38.000000 bycycle-1.1.0/bycycle/tests/features/test_shapes.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.433376 bycycle-1.1.0/bycycle/tests/group/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)        0 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/group/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     4234 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/group/test_features.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     2071 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/group/test_utils.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.433580 bycycle-1.1.0/bycycle/tests/objs/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/tests/objs/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     4633 2023-04-13 21:53:38.000000 bycycle-1.1.0/bycycle/tests/objs/test_fit.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.434026 bycycle-1.1.0/bycycle/tests/plts/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)        0 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/plts/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     1839 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/plts/test_burst.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     1120 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/plts/test_cyclepoints.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     1465 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/plts/test_features.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      506 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/settings.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      799 2023-04-13 21:53:38.000000 bycycle-1.1.0/bycycle/tests/test_persistence.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      831 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/tutils.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.434575 bycycle-1.1.0/bycycle/tests/utils/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)        0 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/utils/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     3582 2023-04-13 19:12:51.000000 bycycle-1.1.0/bycycle/tests/utils/test_dataframes.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      980 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/utils/test_download.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      666 2022-09-26 23:50:26.000000 bycycle-1.1.0/bycycle/tests/utils/test_timeseries.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.435412 bycycle-1.1.0/bycycle/utils/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      267 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/utils/__init__.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)      134 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/utils/checks.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)    12385 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/utils/dataframes.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     1784 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/utils/download.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     1615 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/utils/timeseries.py
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)       57 2023-04-13 21:53:36.000000 bycycle-1.1.0/bycycle/version.py
+drwxr-xr-x   0 ryanhammonds   (501) staff       (20)        0 2023-04-13 22:17:29.426048 bycycle-1.1.0/bycycle.egg-info/
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)    11674 2023-04-13 22:17:29.000000 bycycle-1.1.0/bycycle.egg-info/PKG-INFO
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     2057 2023-04-13 22:17:29.000000 bycycle-1.1.0/bycycle.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)        1 2023-04-13 22:17:29.000000 bycycle-1.1.0/bycycle.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)       76 2023-04-13 22:17:29.000000 bycycle-1.1.0/bycycle.egg-info/requires.txt
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)        8 2023-04-13 22:17:29.000000 bycycle-1.1.0/bycycle.egg-info/top_level.txt
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)       87 2023-04-13 22:03:42.000000 bycycle-1.1.0/requirements.txt
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)       38 2023-04-13 22:17:29.435861 bycycle-1.1.0/setup.cfg
+-rw-r--r--   0 ryanhammonds   (501) staff       (20)     2173 2023-04-13 21:53:36.000000 bycycle-1.1.0/setup.py
```

### Comparing `bycycle-1.0.0rc2/LICENSE` & `bycycle-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/PKG-INFO` & `bycycle-1.1.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,254 +1,271 @@
-Metadata-Version: 1.2
-Name: bycycle
-Version: 1.0.0rc2
-Summary: Cycle-by-cycle analyses of neural oscillations.
-Home-page: https://github.com/bycycle-tools/bycycle
-Author: The Voytek Lab
-Author-email: voyteklab@gmail.com
-License: Apache License, 2.0
-Download-URL: https://github.com/bycycle-tools/bycycle/releases
-Project-URL: Documentation, https://bycycle-tools.github.io/bycycle/
-Project-URL: Bug Reports, https://github.com/bycycle-tools/bycycle/issues
-Project-URL: Source, https://github.com/bycycle-tools/bycycle
-Description: ========================================================
-        bycycle - cycle-by-cycle analysis of neural oscillations
-        ========================================================
-        
-        |ProjectStatus|_ |Version|_ |BuildStatus|_ |Coverage|_ |License|_ |PythonVersions|_ |Publication|_
-        
-        .. |ProjectStatus| image:: https://www.repostatus.org/badges/latest/active.svg
-        .. _ProjectStatus: https://www.repostatus.org/#active
-        
-        .. |Version| image:: https://img.shields.io/pypi/v/bycycle.svg
-        .. _Version: https://pypi.python.org/pypi/bycycle/
-        
-        .. |BuildStatus| image:: https://travis-ci.com/bycycle-tools/bycycle.svg
-        .. _BuildStatus: https://travis-ci.com/bycycle-tools/bycycle
-        
-        .. |Coverage| image:: https://codecov.io/gh/bycycle-tools/bycycle/branch/master/graph/badge.svg
-        .. _Coverage: https://codecov.io/gh/bycycle-tools/bycycle
-        
-        .. |License| image:: https://img.shields.io/pypi/l/bycycle.svg
-        .. _License: https://opensource.org/licenses/Apache-2.0
-        
-        .. |PythonVersions| image:: https://img.shields.io/pypi/pyversions/bycycle.svg
-        .. _PythonVersions: https://pypi.python.org/pypi/bycycle/
-        
-        .. |Publication| image:: https://img.shields.io/badge/publication-10.1152%2Fjn.00273.2019-blue
-        .. _Publication: https://journals.physiology.org/doi/abs/10.1152/jn.00273.2019
-        
-        NOTE: `ByCycle` is currently under-going a major new version update.
-        
-        Check the `changelog <https://bycycle-tools.github.io/bycycle/v1.0.0rc/changelog.html>`_ for notes on updating to the new version.
-        
-        The development version in this repository is no longer compatible with prior releases.
-        
-        Overview
-        --------
-        
-        ``bycycle`` is a python implementation of a cycle-by-cycle approach to analyzing neural oscillations
-        (`Cole & Voytek, J Neurophysiol 2019 <https://journals.physiology.org/doi/abs/10.1152/jn.00273.2019>`_).
-        This approach quantifies features of neural oscillations in the time domain as opposed to the
-        frequency domain. Rather than applying narrowband filters and other methods that utilize a
-        sinusoidal basis, this characterization segments a recording into individual cycles and directly
-        measures each of their properties including amplitude, period, and symmetry. This is most
-        advantageous for analyzing the waveform shape properties of neural oscillations, but it may also
-        provide advantages for studying traditional amplitude and frequency effects, as well. It also
-        implements burst detection, which has gained traction recently (
-        `Jones, 2016 <https://www.sciencedirect.com/science/article/pii/S0959438816300769?via%3Dihub>`_).
-        Therefore, we only analyze oscillatory properties when there is indeed an oscillation.
-        
-        A full description of the method and approach is available in the paper below.
-        
-        
-        Reference
-        ---------
-        
-        If you use this code in your project, please cite:
-        ::
-        
-            Cole SR & Voytek B (2019) Cycle-by-cycle analysis of neural oscillations. J Neurophysiol
-            122:2, 849-861. doi: https://doi.org/10.1152/jn.00273.2019
-        
-        Direct Link: https://journals.physiology.org/doi/abs/10.1152/jn.00273.2019
-        
-        
-        Documentation
-        -------------
-        
-        Documentation for ``bycycle`` is available on the
-        `documentation site <https://bycycle-tools.github.io/bycycle/index.html>`_.
-        
-        This documentation includes:
-        
-        - `Tutorials <https://bycycle-tools.github.io/bycycle/auto_tutorials/index.html>`_:
-          with a step-by-step guide through the approach and how to apply it
-        - `Examples <https://bycycle-tools.github.io/bycycle/auto_examples/index.html>`_:
-          demonstrating an example analysis and use case
-        - `API list <https://bycycle-tools.github.io/bycycle/api.html>`_:
-          which lists and describes all the code and functionality available in the module
-        
-        
-        Dependencies
-        ------------
-        
-        ``bycycle`` is written in Python, and is tested to work with Python 3.5.
-        
-        It has the following dependencies:
-        
-        - `numpy <https://github.com/numpy/numpy>`_
-        - `scipy <https://github.com/scipy/scipy>`_ >= 0.19
-        - `pandas <https://github.com/pandas-dev/pandas>`_
-        - `matplotlib <https://github.com/matplotlib/matplotlib>`_
-        - `pytest <https://github.com/pytest-dev/pytest>`_ (optional)
-        
-        
-        Install
-        -------
-        
-        **Stable Version**
-        
-        To install the latest stable release, you can use pip:
-        
-        .. code-block:: shell
-        
-            $ pip install bycycle
-        
-        ByCycle can also be installed with conda, from the conda-forge channel:
-        
-        .. code-block:: shell
-        
-            $ conda install -c conda-forge bycycle
-        
-        **Development Version**
-        
-        To get the lastest, development version, you can get the code using git:
-        
-        .. code-block:: shell
-        
-            $ git clone https://github.com/bycycle-tools/bycycle
-        
-        To install this cloned copy, move into the directory you just cloned, and run:
-        
-        .. code-block:: shell
-        
-            $ pip install .
-        
-        **Editable Version**
-        
-        To install an editable, development version, move into the directory you cloned and install with:
-        
-        .. code-block:: shell
-        
-            $ pip install -e .
-        
-        
-        Quickstart
-        ----------
-        
-        The main function in ``bycycle`` is ``compute_features``, which takes a time series and some
-        parameters as inputs and returns a table of features for each cycle. Consider having a 1-dimensional
-        numpy array, ``sig``, which is a neural signal time series sampled at 1000 Hz (``fs``) that
-        contains an alpha (8-12 Hz, ``f_range``) oscillation. We can compute the table of cycle features
-        with the following:
-        
-        .. code-block:: python
-        
-            from neurodsp.sim import sim_bursty_oscillation
-            from bycycle.features import compute_features
-        
-            fs = 1000
-            f_range = (8, 12)
-        
-            sig = sim_bursty_oscillation(10, fs, freq=10)
-            df_features = compute_features(sig, fs, f_range)
-        
-        
-        It's necessary to note that the above ``compute_features`` command used default parameters to
-        localize extrema and detect bursts of oscillations. However, it is important to knowledgeably select
-        these parameters, as described in the
-        `algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html#sphx-glr-auto-tutorials-plot-2-bycycle-algorithm-py>`_.
-        The following example and text go over the different potential parameter changes:
-        
-        .. code-block:: python
-        
-            threshold_kwargs = {'amp_fraction_threshold': .2,
-                                'amp_consistency_threshold': .5,
-                                'period_consistency_threshold': .5,
-                                'monotonicity_threshold': .8,
-                                'min_n_cycles': 3}
-        
-            narrowband_kwargs = {'n_seconds': .5}
-        
-            df = compute_features(sig, fs, f_range, center_extrema='trough',
-                                  burst_method='cycles', threshold_kwargs=threshold_kwargs,
-                                  find_extrema_kwargs={'filter_kwargs': narrowband_kwargs})
-        
-        
-        - **center_extrema** determines how the cycles are segmented. 'T' indicates the center extrema is \
-          a trough, so cycles are segmented peak-to-peak.
-        - **burst_method** selects which method for burst detection is used. The 'cycles' option \
-          uses features of adjacent cycles in order to detect bursts (e.g. period consistency, see next \
-          item). The 'amp' option uses an amplitude threshold to determine the cycles that are part of an \
-          oscillatory burst.
-        - **threshold_kwargs** set the keyword arguments for the burst detection functions. For the \
-          ``cycles`` method, there are 5 keyword arguments (see the end of the \
-          `algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html#sphx-glr-auto-tutorials-plot-2-bycycle-algorithm-py>`_ \
-          for advice on choosing these parameters).
-        - **find_extrema_kwargs** set the keyword arguments for the function used to localize peaks and \
-          troughs. Most notably, you can change the duration of the bandpass filter (``N_seconds``) used \
-          during extrema localization (see section 1 of the \
-          `algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html#sphx-glr-auto-tutorials-plot-2-bycycle-algorithm-py>`_)
-        
-        DataFrame Output
-        ~~~~~~~~~~~~~~~~
-        
-        The output of ``bycycle`` is a ``pandas.DataFrame``, a table like the one shown below (with many
-        columns, so it is split into two images).
-        
-        Each row of this table corresponds to an individuals segment of the signal, or a putative cycle of
-        the rhythm of interest.
-        
-        .. image:: https://github.com/bycycle-tools/bycycle/raw/master/doc/img/cycledf_1.png
-        
-        |
-        
-        .. image:: https://github.com/bycycle-tools/bycycle/raw/master/doc/img/cycledf_2.png
-        
-        Some of the columns include:
-        
-        - **sample_peak**: the sample of the signal at which the peak of this cycle occurs
-        - **period**: period of the cycle
-        - **time_peak**: duration of the peak period
-        - **volt_amp**: amplitude of this cycle, average of the rise and decay voltage
-        - **time_rdsym**: rise-decay symmetry, the fraction of the cycle in the rise period (0.5 is symmetric)
-        - **time_ptsym**: peak-trough symmetry, the fraction of the cycle in the peak period (0.5 is symmetric)
-        - **period_consistency**: consistency between the periods of the adjacent cycles, used in burst detection
-        - **is_burst**: indicator if the cycle is part of an oscillatory burst
-        
-        The features in this table can then go on to be analyzed, as demonstrated in the
-        `resting-state data tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html#sphx-glr-auto-tutorials-plot-2-bycycle-algorithm-py>`_
-        and the `data example <https://bycycle-tools.github.io/bycycle/auto_examples/plot_theta_feature_distributions.html#sphx-glr-auto-examples-plot-theta-feature-distributions-py>`_.
-        For example, we may be interested in the distribution of rise-decay symmetry values in a resting state recording, shown below.
-        
-        Burst Detection Results
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. image:: https://github.com/bycycle-tools/bycycle/raw/master/doc/img/bursts_detected.png
-        
-Keywords: neuroscience,neural oscillations,waveform,shape,electrophysiology
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
+========================================================
+bycycle - cycle-by-cycle analysis of neural oscillations
+========================================================
+
+|ProjectStatus|_ |Version|_ |BuildStatus|_ |Coverage|_ |License|_ |PythonVersions|_ |Publication|_
+
+.. |ProjectStatus| image:: https://www.repostatus.org/badges/latest/active.svg
+.. _ProjectStatus: https://www.repostatus.org/#active
+
+.. |Version| image:: https://img.shields.io/pypi/v/bycycle.svg
+.. _Version: https://pypi.python.org/pypi/bycycle/
+
+.. |BuildStatus| image:: https://github.com/bycycle-tools/bycycle/actions/workflows/build.yml/badge.svg
+.. _BuildStatus: https://github.com/bycycle-tools/bycycle/actions/workflows/build.yml
+
+.. |Coverage| image:: https://codecov.io/gh/bycycle-tools/bycycle/branch/main/graph/badge.svg
+.. _Coverage: https://codecov.io/gh/bycycle-tools/bycycle
+
+.. |License| image:: https://img.shields.io/pypi/l/bycycle.svg
+.. _License: https://opensource.org/licenses/Apache-2.0
+
+.. |PythonVersions| image:: https://img.shields.io/pypi/pyversions/bycycle.svg
+.. _PythonVersions: https://pypi.python.org/pypi/bycycle/
+
+.. |Publication| image:: https://img.shields.io/badge/publication-10.1152%2Fjn.00273.2019-blue
+.. _Publication: https://journals.physiology.org/doi/abs/10.1152/jn.00273.2019
+
+ByCycle is a module for analyzing neural oscillations in a cycle-by-cycle approach.
+
+Overview
+--------
+
+``bycycle`` is a tool for quantifying features of neural oscillations in the time domain, as opposed to the
+frequency domain, using a cycle-by-cycle approach. Rather than applying narrowband filters and other methods
+that use a sinusoidal basis, this approach segments a recording into individual cycles and directly measures
+each of their properties including amplitude, period, and symmetry.
+
+This is most advantageous for analyzing the waveform shape properties of neural oscillations.
+It may also provide advantages for studying traditional amplitude and frequency effects, as well.
+Using cycle properties can also be used for burst detection.
+
+A full description of the method and approach is available in the paper below.
+
+Documentation
+-------------
+
+Documentation for ``bycycle`` is available on the
+`documentation site <https://bycycle-tools.github.io/bycycle/index.html>`_.
+
+This documentation includes:
+
+- `Tutorials <https://bycycle-tools.github.io/bycycle/auto_tutorials/index.html>`_:
+  with a step-by-step guide through the approach and how to apply it
+- `Examples <https://bycycle-tools.github.io/bycycle/auto_examples/index.html>`_:
+  demonstrating an example analysis and use case
+- `API list <https://bycycle-tools.github.io/bycycle/api.html>`_:
+  which lists and describes all the code and functionality available in the module
+- `Glossary <https://bycycle-tools.github.io/bycycle/glossary.html>`_:
+  which defines key terms used in the module
+
+Dependencies
+------------
+
+``bycycle`` is written in Python, and requires >= Python 3.6 to run.
+
+It has the following dependencies:
+
+- `neurodsp <https://github.com/neurodsp-tools/neurodsp>`_ >= 2.1.0
+- `numpy <https://github.com/numpy/numpy>`_ >= 1.18.5
+- `scipy <https://github.com/scipy/scipy>`_ >=  1.4.1
+- `pandas <https://github.com/pandas-dev/pandas>`_ >= 0.25.3
+- `matplotlib <https://github.com/matplotlib/matplotlib>`_ >= 3.0.3
+
+There are also optional dependencies, that offer extra functionality:
+
+- `tqdm <https://github.com/tqdm/tqdm>`_ is needed to print progress bars
+- `pytest <https://github.com/pytest-dev/pytest>`_ is needed to run tests locally
+
+Install
+-------
+
+The current major release is the 1.X.X series, which is a breaking change from the prior 0.X.X series.
+
+Check the `changelog <https://bycycle-tools.github.io/bycycle/changelog.html>`_ for notes on updating to the new version.
+
+**Stable Version**
+
+To install the latest stable release, you can use pip:
+
+.. code-block:: shell
+
+    $ pip install bycycle
+
+ByCycle can also be installed with conda, from the conda-forge channel:
+
+.. code-block:: shell
+
+    $ conda install -c conda-forge bycycle
+
+**Development Version**
+
+To get the latest, development version, you can get the code using git:
+
+.. code-block:: shell
+
+    $ git clone https://github.com/bycycle-tools/bycycle
+
+To install this cloned copy, move into the directory you just cloned, and run:
+
+.. code-block:: shell
+
+    $ pip install .
+
+**Editable Version**
+
+To install an editable, development version, move into the directory you cloned and install with:
+
+.. code-block:: shell
+
+    $ pip install -e .
+
+Reference
+---------
+
+If you use this code in your project, please cite:
+
+::
+
+    Cole SR & Voytek B (2019) Cycle-by-cycle analysis of neural oscillations. Journal of neurophysiology
+    122(2), 849-861. DOI: 10.1152/jn.00273.2019
+
+Direct Link: https://doi.org/10.1152/jn.00273.2019
+
+Contribute
+----------
+
+This project welcomes and encourages contributions from the community!
+
+To file bug reports and/or ask questions about this project, please use the
+`Github issue tracker <https://github.com/bycycle-tools/bycycle/issues>`_.
+
+To see and get involved in discussions about the module, check out:
+
+- the `issues board <https://github.com/bycycle-tools/bycycle/issues>`_ for topics relating to code updates, bugs, and fixes
+- the `development page <https://github.com/bycycle-tools/Development>`_ for discussion of potential major updates to the module
+
+When interacting with this project, please use the
+`contribution guidelines <https://github.com/bycycle-tools/bycycle/blob/main/CONTRIBUTING.md>`_
+and follow the
+`code of conduct <https://github.com/bycycle-tools/bycycle/blob/main/CODE_OF_CONDUCT.md>`_.
+
+Quickstart
+----------
+
+The classes in ``bycycle`` are ``Bycycle``, which takes a time series and some
+parameters as inputs, and returns a table of features for each cycle. ``BycycleGroup``
+may be used when working with 2d and 3d signals.
+
+For example, consider having a 1-dimensional numpy array, ``sig``, which is a neural signal time series
+sampled at 1000 Hz (``fs``) with an alpha (8-12 Hz, ``f_range``) oscillation. We can compute the table
+of cycle features with the following:
+
+.. code-block:: python
+
+    from neurodsp.sim import sim_bursty_oscillation
+    from bycycle import Bycycle
+
+    # Simulate
+    fs = 1000
+
+    f_range = (8, 12)
+
+    sig = sim_bursty_oscillation(10, fs, freq=10)
+
+    # Fit
+    bm = Bycycle()
+
+    bm.fit(sig, fs, f_range)
+
+    bm.df_features
+
+
+The above example used default parameters to localize extrema and detect
+bursts of oscillations. However, it is important to knowledgeably select these parameters, as described in the
+`algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html>`_.
+
+The following example introduces some potential parameter changes:
+
+.. code-block:: python
+
+    thresholds = {
+        'amp_fraction_threshold': .2,
+        'amp_consistency_threshold': .5,
+        'period_consistency_threshold': .5,
+        'monotonicity_threshold': .8,
+        'min_n_cycles': 3
+    }
+
+    narrowband_kwargs = {'n_seconds': .5}
+
+    bm = Bycycle(
+        center_extrema='trough',
+        burst_method='cycles',
+        thresholds=thresholds,
+        find_extrema_kwargs={'filter_kwargs': narrowband_kwargs}
+    )
+
+    bm.fit(sig, fs, f_range)
+
+
+- **center_extrema** determines how the cycles are segmented. 'T' indicates the center extrema is \
+  a trough, so cycles are segmented peak-to-peak.
+- **burst_method** selects which method to use for burst detection. The 'cycles' option \
+  uses features of adjacent cycles in order to detect bursts (e.g. period consistency, see next \
+  item). The 'amp' option uses an amplitude threshold to determine the cycles that are part of an \
+  oscillatory burst.
+- **thresholds** sets the keyword arguments for the burst detection functions. For the \
+  ``cycles`` method, there are 5 keyword arguments (see the end of the \
+  `algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html>`_ \
+  for advice on choosing these parameters).
+- **find_extrema_kwargs** sets the keyword arguments for the function used to localize peaks and \
+  troughs. Most notably, you can change the duration of the bandpass filter (``n_seconds``) used \
+  during extrema localization (see section 1 of the \
+  `algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html>`_)
+
+DataFrame Output
+~~~~~~~~~~~~~~~~
+
+The output of ``bycycle`` is a ``pandas.DataFrame``, which is a table, as shown below.
+There are many columns, so the table is split into two images here.
+
+Each row of this table corresponds to an individual segment of the signal, or a putative cycle of
+the rhythm of interest.
+
+.. image:: https://github.com/bycycle-tools/bycycle/raw/main/doc/img/cycledf_1.png
+
+|
+
+.. image:: https://github.com/bycycle-tools/bycycle/raw/main/doc/img/cycledf_2.png
+
+Columns include:
+
+- **sample_peak**: the sample of the signal at which the peak of this cycle occurs
+- **period**: period of the cycle
+- **time_peak**: duration of the peak period
+- **volt_amp**: amplitude of this cycle, average of the rise and decay voltage
+- **time_rdsym**: rise-decay symmetry, the fraction of the cycle in the rise period (0.5 is symmetric)
+- **time_ptsym**: peak-trough symmetry, the fraction of the cycle in the peak period (0.5 is symmetric)
+- **period_consistency**: consistency between the periods of the adjacent cycles, used in burst detection
+- **is_burst**: indicator if the cycle is part of an oscillatory burst
+
+The features in this table can be further analyzed, as demonstrated in the
+`resting state data tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html>`_
+and the `data example <https://bycycle-tools.github.io/bycycle/auto_examples/plot_1_theta_feature_distributions.html>`_.
+For example, we may be interested in the distribution of rise-decay symmetry values in a resting state recording, shown below.
+
+Burst Detection Results
+~~~~~~~~~~~~~~~~~~~~~~~
+
+.. image:: https://github.com/bycycle-tools/bycycle/raw/main/doc/img/bursts_detected.png
+
+Funding
+-------
+
+Supported by NIH award R01 GM134363 from the
+`NIGMS <https://www.nigms.nih.gov/>`_.
+
+.. image:: https://www.nih.gov/sites/all/themes/nih/images/nih-logo-color.png
+  :width: 400
+
+|
```

### Comparing `bycycle-1.0.0rc2/README.rst` & `bycycle-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,124 @@
+Metadata-Version: 2.1
+Name: bycycle
+Version: 1.1.0
+Summary: Cycle-by-cycle analyses of neural oscillations.
+Home-page: https://github.com/bycycle-tools/bycycle
+Download-URL: https://github.com/bycycle-tools/bycycle/releases
+Author: The Voytek Lab
+Author-email: voyteklab@gmail.com
+License: Apache License, 2.0
+Project-URL: Documentation, https://bycycle-tools.github.io/bycycle/
+Project-URL: Bug Reports, https://github.com/bycycle-tools/bycycle/issues
+Project-URL: Source, https://github.com/bycycle-tools/bycycle
+Keywords: neuroscience,neural oscillations,waveform,shape,electrophysiology
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+License-File: LICENSE
+
 ========================================================
 bycycle - cycle-by-cycle analysis of neural oscillations
 ========================================================
 
 |ProjectStatus|_ |Version|_ |BuildStatus|_ |Coverage|_ |License|_ |PythonVersions|_ |Publication|_
 
 .. |ProjectStatus| image:: https://www.repostatus.org/badges/latest/active.svg
 .. _ProjectStatus: https://www.repostatus.org/#active
 
 .. |Version| image:: https://img.shields.io/pypi/v/bycycle.svg
 .. _Version: https://pypi.python.org/pypi/bycycle/
 
-.. |BuildStatus| image:: https://travis-ci.com/bycycle-tools/bycycle.svg
-.. _BuildStatus: https://travis-ci.com/bycycle-tools/bycycle
+.. |BuildStatus| image:: https://github.com/bycycle-tools/bycycle/actions/workflows/build.yml/badge.svg
+.. _BuildStatus: https://github.com/bycycle-tools/bycycle/actions/workflows/build.yml
 
-.. |Coverage| image:: https://codecov.io/gh/bycycle-tools/bycycle/branch/master/graph/badge.svg
+.. |Coverage| image:: https://codecov.io/gh/bycycle-tools/bycycle/branch/main/graph/badge.svg
 .. _Coverage: https://codecov.io/gh/bycycle-tools/bycycle
 
 .. |License| image:: https://img.shields.io/pypi/l/bycycle.svg
 .. _License: https://opensource.org/licenses/Apache-2.0
 
 .. |PythonVersions| image:: https://img.shields.io/pypi/pyversions/bycycle.svg
 .. _PythonVersions: https://pypi.python.org/pypi/bycycle/
 
 .. |Publication| image:: https://img.shields.io/badge/publication-10.1152%2Fjn.00273.2019-blue
 .. _Publication: https://journals.physiology.org/doi/abs/10.1152/jn.00273.2019
 
-NOTE: `ByCycle` is currently under-going a major new version update.
-
-Check the `changelog <https://bycycle-tools.github.io/bycycle/v1.0.0rc/changelog.html>`_ for notes on updating to the new version.
-
-The development version in this repository is no longer compatible with prior releases.
+ByCycle is a module for analyzing neural oscillations in a cycle-by-cycle approach.
 
 Overview
 --------
 
-``bycycle`` is a python implementation of a cycle-by-cycle approach to analyzing neural oscillations
-(`Cole & Voytek, J Neurophysiol 2019 <https://journals.physiology.org/doi/abs/10.1152/jn.00273.2019>`_).
-This approach quantifies features of neural oscillations in the time domain as opposed to the
-frequency domain. Rather than applying narrowband filters and other methods that utilize a
-sinusoidal basis, this characterization segments a recording into individual cycles and directly
-measures each of their properties including amplitude, period, and symmetry. This is most
-advantageous for analyzing the waveform shape properties of neural oscillations, but it may also
-provide advantages for studying traditional amplitude and frequency effects, as well. It also
-implements burst detection, which has gained traction recently (
-`Jones, 2016 <https://www.sciencedirect.com/science/article/pii/S0959438816300769?via%3Dihub>`_).
-Therefore, we only analyze oscillatory properties when there is indeed an oscillation.
+``bycycle`` is a tool for quantifying features of neural oscillations in the time domain, as opposed to the
+frequency domain, using a cycle-by-cycle approach. Rather than applying narrowband filters and other methods
+that use a sinusoidal basis, this approach segments a recording into individual cycles and directly measures
+each of their properties including amplitude, period, and symmetry.
+
+This is most advantageous for analyzing the waveform shape properties of neural oscillations.
+It may also provide advantages for studying traditional amplitude and frequency effects, as well.
+Using cycle properties can also be used for burst detection.
 
 A full description of the method and approach is available in the paper below.
 
-
-Reference
----------
-
-If you use this code in your project, please cite:
-::
-
-    Cole SR & Voytek B (2019) Cycle-by-cycle analysis of neural oscillations. J Neurophysiol
-    122:2, 849-861. doi: https://doi.org/10.1152/jn.00273.2019
-
-Direct Link: https://journals.physiology.org/doi/abs/10.1152/jn.00273.2019
-
-
 Documentation
 -------------
 
 Documentation for ``bycycle`` is available on the
 `documentation site <https://bycycle-tools.github.io/bycycle/index.html>`_.
 
 This documentation includes:
 
 - `Tutorials <https://bycycle-tools.github.io/bycycle/auto_tutorials/index.html>`_:
   with a step-by-step guide through the approach and how to apply it
 - `Examples <https://bycycle-tools.github.io/bycycle/auto_examples/index.html>`_:
   demonstrating an example analysis and use case
 - `API list <https://bycycle-tools.github.io/bycycle/api.html>`_:
   which lists and describes all the code and functionality available in the module
-
+- `Glossary <https://bycycle-tools.github.io/bycycle/glossary.html>`_:
+  which defines key terms used in the module
 
 Dependencies
 ------------
 
-``bycycle`` is written in Python, and is tested to work with Python 3.5.
+``bycycle`` is written in Python, and requires >= Python 3.6 to run.
 
 It has the following dependencies:
 
-- `numpy <https://github.com/numpy/numpy>`_
-- `scipy <https://github.com/scipy/scipy>`_ >= 0.19
-- `pandas <https://github.com/pandas-dev/pandas>`_
-- `matplotlib <https://github.com/matplotlib/matplotlib>`_
-- `pytest <https://github.com/pytest-dev/pytest>`_ (optional)
+- `neurodsp <https://github.com/neurodsp-tools/neurodsp>`_ >= 2.1.0
+- `numpy <https://github.com/numpy/numpy>`_ >= 1.18.5
+- `scipy <https://github.com/scipy/scipy>`_ >=  1.4.1
+- `pandas <https://github.com/pandas-dev/pandas>`_ >= 0.25.3
+- `matplotlib <https://github.com/matplotlib/matplotlib>`_ >= 3.0.3
 
+There are also optional dependencies, that offer extra functionality:
+
+- `tqdm <https://github.com/tqdm/tqdm>`_ is needed to print progress bars
+- `pytest <https://github.com/pytest-dev/pytest>`_ is needed to run tests locally
 
 Install
 -------
 
+The current major release is the 1.X.X series, which is a breaking change from the prior 0.X.X series.
+
+Check the `changelog <https://bycycle-tools.github.io/bycycle/changelog.html>`_ for notes on updating to the new version.
+
 **Stable Version**
 
 To install the latest stable release, you can use pip:
 
 .. code-block:: shell
 
     $ pip install bycycle
@@ -106,15 +127,15 @@
 
 .. code-block:: shell
 
     $ conda install -c conda-forge bycycle
 
 **Development Version**
 
-To get the lastest, development version, you can get the code using git:
+To get the latest, development version, you can get the code using git:
 
 .. code-block:: shell
 
     $ git clone https://github.com/bycycle-tools/bycycle
 
 To install this cloned copy, move into the directory you just cloned, and run:
 
@@ -126,100 +147,157 @@
 
 To install an editable, development version, move into the directory you cloned and install with:
 
 .. code-block:: shell
 
     $ pip install -e .
 
+Reference
+---------
+
+If you use this code in your project, please cite:
+
+::
+
+    Cole SR & Voytek B (2019) Cycle-by-cycle analysis of neural oscillations. Journal of neurophysiology
+    122(2), 849-861. DOI: 10.1152/jn.00273.2019
+
+Direct Link: https://doi.org/10.1152/jn.00273.2019
+
+Contribute
+----------
+
+This project welcomes and encourages contributions from the community!
+
+To file bug reports and/or ask questions about this project, please use the
+`Github issue tracker <https://github.com/bycycle-tools/bycycle/issues>`_.
+
+To see and get involved in discussions about the module, check out:
+
+- the `issues board <https://github.com/bycycle-tools/bycycle/issues>`_ for topics relating to code updates, bugs, and fixes
+- the `development page <https://github.com/bycycle-tools/Development>`_ for discussion of potential major updates to the module
+
+When interacting with this project, please use the
+`contribution guidelines <https://github.com/bycycle-tools/bycycle/blob/main/CONTRIBUTING.md>`_
+and follow the
+`code of conduct <https://github.com/bycycle-tools/bycycle/blob/main/CODE_OF_CONDUCT.md>`_.
 
 Quickstart
 ----------
 
-The main function in ``bycycle`` is ``compute_features``, which takes a time series and some
-parameters as inputs and returns a table of features for each cycle. Consider having a 1-dimensional
-numpy array, ``sig``, which is a neural signal time series sampled at 1000 Hz (``fs``) that
-contains an alpha (8-12 Hz, ``f_range``) oscillation. We can compute the table of cycle features
-with the following:
+The classes in ``bycycle`` are ``Bycycle``, which takes a time series and some
+parameters as inputs, and returns a table of features for each cycle. ``BycycleGroup``
+may be used when working with 2d and 3d signals.
+
+For example, consider having a 1-dimensional numpy array, ``sig``, which is a neural signal time series
+sampled at 1000 Hz (``fs``) with an alpha (8-12 Hz, ``f_range``) oscillation. We can compute the table
+of cycle features with the following:
 
 .. code-block:: python
 
     from neurodsp.sim import sim_bursty_oscillation
-    from bycycle.features import compute_features
+    from bycycle import Bycycle
 
+    # Simulate
     fs = 1000
+
     f_range = (8, 12)
 
     sig = sim_bursty_oscillation(10, fs, freq=10)
-    df_features = compute_features(sig, fs, f_range)
 
+    # Fit
+    bm = Bycycle()
 
-It's necessary to note that the above ``compute_features`` command used default parameters to
-localize extrema and detect bursts of oscillations. However, it is important to knowledgeably select
-these parameters, as described in the
-`algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html#sphx-glr-auto-tutorials-plot-2-bycycle-algorithm-py>`_.
-The following example and text go over the different potential parameter changes:
+    bm.fit(sig, fs, f_range)
+
+    bm.df_features
+
+
+The above example used default parameters to localize extrema and detect
+bursts of oscillations. However, it is important to knowledgeably select these parameters, as described in the
+`algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html>`_.
+
+The following example introduces some potential parameter changes:
 
 .. code-block:: python
 
-    threshold_kwargs = {'amp_fraction_threshold': .2,
-                        'amp_consistency_threshold': .5,
-                        'period_consistency_threshold': .5,
-                        'monotonicity_threshold': .8,
-                        'min_n_cycles': 3}
+    thresholds = {
+        'amp_fraction_threshold': .2,
+        'amp_consistency_threshold': .5,
+        'period_consistency_threshold': .5,
+        'monotonicity_threshold': .8,
+        'min_n_cycles': 3
+    }
 
     narrowband_kwargs = {'n_seconds': .5}
 
-    df = compute_features(sig, fs, f_range, center_extrema='trough',
-                          burst_method='cycles', threshold_kwargs=threshold_kwargs,
-                          find_extrema_kwargs={'filter_kwargs': narrowband_kwargs})
+    bm = Bycycle(
+        center_extrema='trough',
+        burst_method='cycles',
+        thresholds=thresholds,
+        find_extrema_kwargs={'filter_kwargs': narrowband_kwargs}
+    )
+
+    bm.fit(sig, fs, f_range)
 
 
 - **center_extrema** determines how the cycles are segmented. 'T' indicates the center extrema is \
   a trough, so cycles are segmented peak-to-peak.
-- **burst_method** selects which method for burst detection is used. The 'cycles' option \
+- **burst_method** selects which method to use for burst detection. The 'cycles' option \
   uses features of adjacent cycles in order to detect bursts (e.g. period consistency, see next \
   item). The 'amp' option uses an amplitude threshold to determine the cycles that are part of an \
   oscillatory burst.
-- **threshold_kwargs** set the keyword arguments for the burst detection functions. For the \
+- **thresholds** sets the keyword arguments for the burst detection functions. For the \
   ``cycles`` method, there are 5 keyword arguments (see the end of the \
-  `algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html#sphx-glr-auto-tutorials-plot-2-bycycle-algorithm-py>`_ \
+  `algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html>`_ \
   for advice on choosing these parameters).
-- **find_extrema_kwargs** set the keyword arguments for the function used to localize peaks and \
-  troughs. Most notably, you can change the duration of the bandpass filter (``N_seconds``) used \
+- **find_extrema_kwargs** sets the keyword arguments for the function used to localize peaks and \
+  troughs. Most notably, you can change the duration of the bandpass filter (``n_seconds``) used \
   during extrema localization (see section 1 of the \
-  `algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html#sphx-glr-auto-tutorials-plot-2-bycycle-algorithm-py>`_)
+  `algorithm tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html>`_)
 
 DataFrame Output
 ~~~~~~~~~~~~~~~~
 
-The output of ``bycycle`` is a ``pandas.DataFrame``, a table like the one shown below (with many
-columns, so it is split into two images).
+The output of ``bycycle`` is a ``pandas.DataFrame``, which is a table, as shown below.
+There are many columns, so the table is split into two images here.
 
-Each row of this table corresponds to an individuals segment of the signal, or a putative cycle of
+Each row of this table corresponds to an individual segment of the signal, or a putative cycle of
 the rhythm of interest.
 
-.. image:: https://github.com/bycycle-tools/bycycle/raw/master/doc/img/cycledf_1.png
+.. image:: https://github.com/bycycle-tools/bycycle/raw/main/doc/img/cycledf_1.png
 
 |
 
-.. image:: https://github.com/bycycle-tools/bycycle/raw/master/doc/img/cycledf_2.png
+.. image:: https://github.com/bycycle-tools/bycycle/raw/main/doc/img/cycledf_2.png
 
-Some of the columns include:
+Columns include:
 
 - **sample_peak**: the sample of the signal at which the peak of this cycle occurs
 - **period**: period of the cycle
 - **time_peak**: duration of the peak period
 - **volt_amp**: amplitude of this cycle, average of the rise and decay voltage
 - **time_rdsym**: rise-decay symmetry, the fraction of the cycle in the rise period (0.5 is symmetric)
 - **time_ptsym**: peak-trough symmetry, the fraction of the cycle in the peak period (0.5 is symmetric)
 - **period_consistency**: consistency between the periods of the adjacent cycles, used in burst detection
 - **is_burst**: indicator if the cycle is part of an oscillatory burst
 
-The features in this table can then go on to be analyzed, as demonstrated in the
-`resting-state data tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html#sphx-glr-auto-tutorials-plot-2-bycycle-algorithm-py>`_
-and the `data example <https://bycycle-tools.github.io/bycycle/auto_examples/plot_theta_feature_distributions.html#sphx-glr-auto-examples-plot-theta-feature-distributions-py>`_.
+The features in this table can be further analyzed, as demonstrated in the
+`resting state data tutorial <https://bycycle-tools.github.io/bycycle/auto_tutorials/plot_2_bycycle_algorithm.html>`_
+and the `data example <https://bycycle-tools.github.io/bycycle/auto_examples/plot_1_theta_feature_distributions.html>`_.
 For example, we may be interested in the distribution of rise-decay symmetry values in a resting state recording, shown below.
 
 Burst Detection Results
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-.. image:: https://github.com/bycycle-tools/bycycle/raw/master/doc/img/bursts_detected.png
+.. image:: https://github.com/bycycle-tools/bycycle/raw/main/doc/img/bursts_detected.png
+
+Funding
+-------
+
+Supported by NIH award R01 GM134363 from the
+`NIGMS <https://www.nigms.nih.gov/>`_.
+
+.. image:: https://www.nih.gov/sites/all/themes/nih/images/nih-logo-color.png
+  :width: 400
+
+|
```

### Comparing `bycycle-1.0.0rc2/bycycle/burst/amp.py` & `bycycle-1.1.0/bycycle/burst/amp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Detect bursts: amplitude threshold approach."""
 
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range
 from bycycle.burst.utils import check_min_burst_cycles
 
 ###################################################################################################
 ###################################################################################################
 
 def detect_bursts_amp(df_features, burst_fraction_threshold=1, min_n_cycles=3):
     """Detect bursts based on amplitude thresholding.
@@ -34,15 +34,15 @@
     >>> df_shapes = compute_shape_features(sig, fs, f_range=(8, 12))
     >>> df_burst = compute_burst_features(df_shapes, sig, burst_method='amp',
     ...                                   burst_kwargs={'fs': fs, 'f_range': (8, 12)})
     >>> df_burst = detect_bursts_amp(df_burst)
     """
 
     # Ensure arguments are within valid ranges
-    check_param(burst_fraction_threshold, 'burst_fraction_threshold', (0, 1))
+    check_param_range(burst_fraction_threshold, 'burst_fraction_threshold', (0, 1))
 
     # Determine cycles that are defined as bursting throughout the whole cycle
     is_burst = [frac >= burst_fraction_threshold for frac in df_features['burst_fraction']]
 
     df_features['is_burst'] = check_min_burst_cycles(is_burst, min_n_cycles=min_n_cycles)
 
     return df_features
```

### Comparing `bycycle-1.0.0rc2/bycycle/burst/cycle.py` & `bycycle-1.1.0/bycycle/burst/cycle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Detect bursts: cycle consistency approach."""
 
 import pandas as pd
 
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range
 from bycycle.burst.utils import check_min_burst_cycles
 
 ###################################################################################################
 ###################################################################################################
 
 pd.options.mode.chained_assignment = None
 
@@ -73,18 +73,18 @@
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_shapes = compute_shape_features(sig, fs, f_range=(8, 12))
     >>> df_burst = compute_burst_features(df_shapes, sig)
     >>> df_burst = detect_bursts_cycles(df_burst)
     """
 
     # Ensure arguments are within valid ranges
-    check_param(amp_fraction_threshold, 'amp_fraction_threshold', (0, 1))
-    check_param(amp_consistency_threshold, 'amp_consistency_threshold', (0, 1))
-    check_param(period_consistency_threshold, 'period_consistency_threshold', (0, 1))
-    check_param(monotonicity_threshold, 'monotonicity_threshold', (0, 1))
+    check_param_range(amp_fraction_threshold, 'amp_fraction_threshold', (0, 1))
+    check_param_range(amp_consistency_threshold, 'amp_consistency_threshold', (0, 1))
+    check_param_range(period_consistency_threshold, 'period_consistency_threshold', (0, 1))
+    check_param_range(monotonicity_threshold, 'monotonicity_threshold', (0, 1))
 
     # Compute if each period is part of an oscillation
     amp_fraction = df_features['amp_fraction'] > amp_fraction_threshold
     amp_consistency = df_features['amp_consistency'] > amp_consistency_threshold
     period_consistency = df_features['period_consistency'] > period_consistency_threshold
     monotonicity = df_features['monotonicity'] > monotonicity_threshold
```

### Comparing `bycycle-1.0.0rc2/bycycle/burst/utils.py` & `bycycle-1.1.0/bycycle/burst/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Utilities for burst detection."""
 
 from copy import deepcopy
 import numpy as np
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range, check_param_options
 
 ####################################################################################################
 ####################################################################################################
 
 def check_min_burst_cycles(is_burst, min_n_cycles=3):
     """Enforce minimum number of consecutive cycles to be considered a burst.
 
@@ -28,15 +28,15 @@
 
     >>> is_burst = np.array([False, True, True, False, True, True, True, True, False])
     >>> check_min_burst_cycles(is_burst)
     array([False, False, False, False,  True,  True,  True,  True, False])
     """
 
     # Ensure argument is within valid range
-    check_param(min_n_cycles, 'min_n_cycles', (0, np.inf))
+    check_param_range(min_n_cycles, 'min_n_cycles', (0, np.inf))
 
     temp_cycle_count = 0
 
     for idx, bursting in enumerate(is_burst):
 
         if bursting:
             temp_cycle_count += 1
@@ -48,22 +48,22 @@
                     is_burst[idx - 1 - c_rm] = False
 
             temp_cycle_count = 0
 
     return is_burst
 
 
-def recompute_edges(df_features, threshold_kwargs):
+def recompute_edges(df_features, threshold_kwargs, burst_method='cycles', burst_kwargs=None):
     """Recompute the is_burst column for cycles on the edges of bursts.
 
     Parameters
     ----------
     df_features : pandas.DataFrame
         A dataframe containing shape and burst features for each cycle.
-    threshold_kwargs : dict, optional, default: None
+    threshold_kwargs : dict
         Feature thresholds for cycles to be considered bursts, matching keyword arguments for:
 
         - :func:`~.detect_bursts_cycles` for consistency burst detection
           (i.e. when burst_method == 'cycles')
 
     Returns
     -------
@@ -88,38 +88,73 @@
     ...                     'min_n_cycles': 3}
     >>> df_features = compute_features(sig, fs=1000, f_range=(8, 12),
     ...                                threshold_kwargs=threshold_kwargs)
     >>> threshold_kwargs['amp_consistency_threshold'] = 0
     >>> df_features_edges = recompute_edges(df_features, threshold_kwargs)
     """
 
-    # Prevent circular import between burst.utils and burst.cycle
+    # Prevent circular imports between burst.utils and burst.cycle
     from bycycle.burst import detect_bursts_cycles
 
     # Prevent overwriting the original dataframe
     df_features_edges = df_features.copy()
 
     # Identify all cycles where is_burst changes on the following cycle
     #   Use copy to keep dataframe columns unlinked
     is_burst = deepcopy(df_features_edges['is_burst'].values)
     burst_edges = np.where(is_burst[1:] == ~is_burst[:-1])[0]
 
-    # Adjust odd edges such that all edges fall on is_burst == False
-    burst_edges = np.array([edge if idx % 2 == 0 else edge+1 for idx, edge in
-                            enumerate(burst_edges)])
-
-    # Recompute is_burst
-    df_features_edges = detect_bursts_cycles(
-        df_features_edges,
-        amp_fraction_threshold=threshold_kwargs['amp_fraction_threshold'],
-        amp_consistency_threshold=threshold_kwargs['amp_consistency_threshold'],
-        period_consistency_threshold=threshold_kwargs['period_consistency_threshold'],
-        monotonicity_threshold=threshold_kwargs['monotonicity_threshold'],
-        min_n_cycles=threshold_kwargs['min_n_cycles']
-    )
+    # Get cycles outside of bursts
+    burst_starts = np.array([edge for idx, edge in enumerate(burst_edges) if idx % 2 == 0])
+    burst_ends = np.array([edge+1 for idx, edge in enumerate(burst_edges) if idx % 2 == 1 ])
 
-    # Confine recomputed is_burst to edges
-    is_burst[burst_edges] = df_features_edges.iloc[burst_edges]['is_burst'].values
+    # Recompute is_burst for cycles at the edge
+    for start_idx, end_idx in zip(burst_starts, burst_ends):
 
-    df_features_edges['is_burst'] = is_burst
+        df_features_edges = recompute_edge(df_features_edges, start_idx, 'next')
+        df_features_edges = recompute_edge(df_features_edges, end_idx, 'last')
+
+    # Apply thresholding
+    df_features_edges = detect_bursts_cycles(df_features_edges, **threshold_kwargs)
 
     return df_features_edges
+
+
+def recompute_edge(df_features, cyc_idx, direction):
+    """Recompute consistency features at the edge of a cycle.
+
+    Parameters
+    ----------
+    df_features : pandas.DataFrame
+        A dataframe containing shape and burst features for each cycle.
+    cyc_idx : int
+        The dataframe index of the edge.
+    direction : {'both', 'next', 'last'}
+        The direction to compute consistency.
+
+    Returns
+    -------
+    df_features : pandas.DataFrame
+        A dataframe with updated consistency features.
+    """
+
+    # Check that param validity
+    check_param_options(direction, 'direction', ['both', 'next', 'last'])
+
+    # Prevent circular imports between burst.utils and burst.cycle
+    from bycycle.features.burst import compute_amp_consistency, compute_period_consistency
+
+    # Slice edges rows and recompute burst features
+    lower = max(cyc_idx-1, 0)
+    upper = min(cyc_idx+2, len(df_features))
+    edge_range = range(lower, upper)
+
+    edge = df_features.iloc[edge_range].copy()
+
+    # Update dataframe with recomputed consistency features
+    df_features['amp_consistency'][cyc_idx] = \
+        compute_amp_consistency(edge, direction=direction)[1]
+
+    df_features['period_consistency'][cyc_idx] = \
+        compute_period_consistency(edge, direction=direction)[1]
+
+    return df_features
```

### Comparing `bycycle-1.0.0rc2/bycycle/cyclepoints/extrema.py` & `bycycle-1.1.0/bycycle/cyclepoints/extrema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Find extrema for individual cycles."""
 
 import numpy as np
 
 from neurodsp.filt import filter_signal
 from neurodsp.filt.fir import compute_filter_length
 
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range
 from bycycle.cyclepoints.zerox import find_flank_zerox
 
 ###################################################################################################
 ###################################################################################################
 
 def find_extrema(sig, fs, f_range, boundary=0, first_extrema='peak',
                  filter_kwargs=None, pass_type='bandpass', pad=True):
@@ -56,15 +56,15 @@
     >>> from neurodsp.sim import sim_bursty_oscillation
     >>> fs = 500
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> peaks, troughs = find_extrema(sig, fs, f_range=(8, 12))
     """
 
     # Ensure arguments are within valid range
-    check_param(fs, 'fs', (0, np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
 
     # Set default filtering parameters
     if filter_kwargs is None:
         filter_kwargs = {}
 
     # Get the original signal and filter lengths
     sig_len = len(sig)
@@ -93,29 +93,45 @@
         n_troughs = len(decay_xs)
     else:
         n_peaks = len(rise_xs)
         n_troughs = len(decay_xs) - 1
 
     # Calculate peak samples
     peaks = np.zeros(n_peaks, dtype=int)
+    _decay_xs = decay_xs.copy()
     for p_idx in range(n_peaks):
 
         # Calculate the sample range between the most recent zero rise and the next zero decay
         last_rise = rise_xs[p_idx]
-        next_decay = decay_xs[decay_xs > last_rise][0]
+
+        for idx, decay in enumerate(_decay_xs):
+            if decay > last_rise:
+                _decay_xs = _decay_xs[idx:]
+                break
+
+        next_decay = _decay_xs[0]
+
         # Identify time of peak
         peaks[p_idx] = np.argmax(sig[last_rise:next_decay]) + last_rise
 
     # Calculate trough samples
     troughs = np.zeros(n_troughs, dtype=int)
+    _rise_xs = rise_xs.copy()
     for t_idx in range(n_troughs):
 
         # Calculate the sample range between the most recent zero decay and the next zero rise
         last_decay = decay_xs[t_idx]
-        next_rise = rise_xs[rise_xs > last_decay][0]
+
+        for idx, rise in enumerate(_rise_xs):
+            if rise > last_decay:
+                _rise_xs = _rise_xs[idx:]
+                break
+
+        next_rise = _rise_xs[0]
+
         # Identify time of trough
         troughs[t_idx] = np.argmin(sig[last_decay:next_rise]) + last_decay
 
     # Remove padding
     peaks = peaks - int(np.ceil(filt_len/2))
     troughs = troughs - int(np.ceil(filt_len/2))
```

### Comparing `bycycle-1.0.0rc2/bycycle/cyclepoints/phase.py` & `bycycle-1.1.0/bycycle/cyclepoints/phase.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/cyclepoints/zerox.py` & `bycycle-1.1.0/bycycle/cyclepoints/zerox.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     rises = _find_flank_midpoints(sig, 'rise', n_rises, troughs, peaks, idx_bias)
     decays = _find_flank_midpoints(sig, 'decay', n_decays, peaks, troughs, idx_bias)
 
     return rises, decays
 
 
-def find_flank_zerox(sig, flank):
+def find_flank_zerox(sig, flank, midpoint=None):
     """Find zero-crossings on rising or decaying flanks of a filtered signal.
 
     Parameters
     ----------
     sig : 1d array
         Time series to detect zero-crossings in.
     flank : {'rise', 'decay'}
@@ -91,16 +91,19 @@
     >>> from neurodsp.sim import sim_bursty_oscillation
     >>> from neurodsp.filt import filter_signal
     >>> sig = sim_bursty_oscillation(10, 500, freq=10)
     >>> sig_filt = filter_signal(sig, 500, 'lowpass', 30)
     >>> rises_flank = find_flank_zerox(sig_filt, 'rise')
     """
 
+    if midpoint is None:
+        midpoint = 0
+
     assert flank in ['rise', 'decay']
-    pos = sig <= 0 if flank == 'rise' else sig > 0
+    pos = sig <= midpoint if flank == 'rise' else sig > midpoint
 
     zero_xs = (pos[:-1] & ~pos[1:]).nonzero()[0]
 
     # If no zero-crossing's found (peak and trough are same voltage), output dummy value
     zero_xs = [int(len(sig) / 2)] if len(zero_xs) == 0 else zero_xs
 
     return zero_xs
@@ -112,22 +115,23 @@
     assert flank in ['rise', 'decay']
     idx_bias = -idx_bias + 1 if flank == 'rise' else idx_bias
     comp = gt if flank == 'rise' else lt
 
     flanks = np.zeros(n_flanks, dtype=int)
     for idx in range(n_flanks):
 
-        sig_temp = np.copy(sig[extrema_start[idx]:extrema_end[idx + idx_bias] + 1])
-        sig_temp -= (sig_temp[0] + sig_temp[-1]) / 2.
+        sig_temp = sig[extrema_start[idx]:extrema_end[idx + idx_bias] + 1]
+        midpoint = (sig_temp[0] + sig_temp[-1]) / 2.
 
         # If data is all zeros, just set the zero-crossing to be halfway between
         if np.sum(np.abs(sig_temp)) == 0:
             flanks[idx] = extrema_start[idx] + int(len(sig_temp) / 2.)
 
         # If flank is actually an extrema, just set the zero-crossing to be halfway between
         elif comp(sig_temp[0], sig_temp[-1]):
             flanks[idx] = extrema_start[idx] + int(len(sig_temp) / 2.)
-
         else:
-            flanks[idx] = extrema_start[idx] + int(np.median(find_flank_zerox(sig_temp, flank)))
+            midpoint = (sig_temp[0] + sig_temp[-1]) / 2.
+            flanks[idx] = extrema_start[idx] + \
+                int(np.median(find_flank_zerox(sig_temp, flank, midpoint)))
 
     return flanks
```

### Comparing `bycycle-1.0.0rc2/bycycle/features/burst.py` & `bycycle-1.1.0/bycycle/features/burst.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Compute burst features for individual cycles."""
 
 import numpy as np
 import pandas as pd
 
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range, check_param_options
 from bycycle.burst import detect_bursts_dual_threshold
 
 ###################################################################################################
 ###################################################################################################
 
 def compute_burst_features(df_shape_features, sig, burst_method='cycles', burst_kwargs=None):
     """Compute burst features for each cycle.
@@ -28,14 +28,15 @@
         Additional arguments required for amplitude burst detection. Defined in
         :func:`~.compute_burst_fraction`, keys include:
 
         - ``fs`` : required for dual amplitude threshold burst detection
         - ``f_range`` : required for dual amplitude threshold burst detection
         - ``amp_threshes`` : optional, default: (1, 2)
         - ``min_n_cycles`` : optional, default: 3
+        - ``min_burst_duration`` : optional, default: None
         - ``filter_kwargs`` : optional, default: None
 
     Returns
     -------
     df_burst_features : pandas.DataFrame
         Dataframe containing burst features. Each row is one cycle. Columns:
 
@@ -70,18 +71,18 @@
     # Use feature consistency burst detection
     if burst_method == 'cycles':
 
         # Custom feature functions may be inserted here as long as an array is returned
         #   with length equal to the number of cycles, or rows in df_shapes
         df_burst_features['amp_fraction'] = compute_amp_fraction(df_shape_features)
 
-        df_burst_features['amp_consistency'] = \
-                compute_amp_consistency(df_shape_features)
+        df_burst_features['amp_consistency'] = compute_amp_consistency(df_shape_features)
 
         df_burst_features['period_consistency'] = compute_period_consistency(df_shape_features)
+
         df_burst_features['monotonicity'] = compute_monotonicity(df_shape_features, sig)
 
     # Use dual threshold burst detection
     elif burst_method == 'amp':
 
         fs = burst_kwargs.pop('fs', None)
         f_range = burst_kwargs.pop('f_range', None)
@@ -123,23 +124,23 @@
     >>> df_shapes = compute_shape_features(sig, fs, (8, 12))
     >>> amp_fraction = compute_amp_fraction(df_shapes)
     """
 
     return df_shape_features['volt_amp'].rank() / len(df_shape_features)
 
 
-def compute_amp_consistency(df_shape_features):
+def compute_amp_consistency(df_shape_features, direction='both'):
     """Compute amplitude consistency for each cycle.
 
     Parameters
     ----------
     df_shape_features : pandas.DataFrame
         Shape features for each cycle, determined using :func:`~.compute_shape_features`.
-    df_samples : pandas.DataFrame
-        Indices of cyclepoints returned from :func:`~.compute_cyclepoints`.
+    direction : {'both', 'next', 'last'}
+        The direction to compute consistency. Defaults to bi-directional.
 
     Returns
     -------
     amp_consist : 1d array
         The amplitude consistency of each cycle.
 
     Examples
@@ -150,17 +151,23 @@
     >>> from neurodsp.sim import sim_bursty_oscillation
     >>> fs = 500
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_shapes = compute_shape_features(sig, fs, f_range=(8, 12))
     >>> amp_consistency = compute_amp_consistency(df_shapes)
     """
 
+    # Check that param validity
+    check_param_options(direction, 'direction', ['both', 'next', 'last'])
+
     # Compute amplitude consistency
     cycles = len(df_shape_features)
-    amp_consistency = np.ones(cycles) * np.nan
+    amp_consistency = np.zeros(cycles)
+    amp_consistency[0] = np.nan
+    amp_consistency[-1] = np.nan
+
     rises = df_shape_features['volt_rise'].values
     decays = df_shape_features['volt_decay'].values
 
     for cyc in range(1, cycles-1):
 
         # Division by zero will return np.nan, suppress warning.
         with np.errstate(invalid='ignore', divide='ignore'):
@@ -181,27 +188,38 @@
                     np.max([rises[cyc-1], decays[cyc]])
 
                 consist_next = np.min([rises[cyc], decays[cyc+1]]) / \
                     np.max([rises[cyc], decays[cyc+1]])
 
             if np.isnan([consist_current, consist_next, consist_last]).all():
                 amp_consistency[cyc] = np.nan
-            else:
+            elif direction == 'next':
+                amp_consistency[cyc] = np.nanmin([consist_current, consist_next])
+            elif direction == 'last':
+                amp_consistency[cyc] = np.nanmin([consist_current, consist_last])
+            elif direction == 'both':
                 amp_consistency[cyc] = np.nanmin([consist_current, consist_next, consist_last])
 
+    # Prevent negative consistency
+    if (amp_consistency < 0).any():
+
+        amp_consistency[np.where(amp_consistency < 0)[0]] = 0
+
     return amp_consistency
 
 
-def compute_period_consistency(df_shape_features):
+def compute_period_consistency(df_shape_features, direction='both'):
     """Compute the period consistency of each cycle.
 
     Parameters
     ----------
     df_shape_features : pandas.DataFrame
         Shape features for each cycle, determined using :func:`~.compute_shape_features`.
+    direction : {'both', 'next', 'last'}
+        The direction to compute consistency. Defaults to bi-directional.
 
     Returns
     -------
     period_consistency : 1d array
         The period consistency of each cycle.
 
     Examples
@@ -212,27 +230,37 @@
     >>> from neurodsp.sim import sim_bursty_oscillation
     >>> fs = 500
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_shapes = compute_shape_features(sig, fs, f_range=(8, 12))
     >>> period_consistency = compute_period_consistency(df_shapes)
     """
 
+    # Check that param validity
+    check_param_options(direction, 'direction', ['both', 'next', 'last'])
+
     # Compute period consistency
     cycles = len(df_shape_features)
-    period_consistency = np.ones(cycles) * np.nan
+    period_consistency = np.zeros(cycles)
+    period_consistency[0] = np.nan
+    period_consistency[-1] = np.nan
     periods = df_shape_features['period'].values
 
     for cyc in range(1, cycles-1):
 
         consist_last = np.min([periods[cyc], periods[cyc-1]]) / \
             np.max([periods[cyc], periods[cyc-1]])
         consist_next = np.min([periods[cyc+1], periods[cyc]]) / \
             np.max([periods[cyc+1], periods[cyc]])
 
-        period_consistency[cyc] = np.min([consist_next, consist_last])
+        if direction == 'next':
+            period_consistency[cyc] = consist_next
+        elif direction == 'last':
+            period_consistency[cyc] = consist_last
+        elif direction == 'both':
+            period_consistency[cyc] = np.min([consist_next, consist_last])
 
     return period_consistency
 
 
 def compute_monotonicity(df_samples, sig):
     """Compute the monotonicity of each cycle.
 
@@ -258,17 +286,17 @@
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_samples = compute_cyclepoints(sig, fs, f_range=(8, 12))
     >>> monotonicity = compute_monotonicity(df_samples, sig)
     """
 
     # Compute monotonicity
     cycles = len(df_samples)
-    monotonicity = np.ones(cycles) * np.nan
+    monotonicity = np.zeros(cycles)
 
-    for idx, row in df_samples.iterrows():
+    for idx, row in enumerate(df_samples.to_dict('records')):
 
         if 'sample_peak' in df_samples.columns:
             rise_period = sig[int(row['sample_last_trough']):int(row['sample_peak'])+1]
             decay_period = sig[int(row['sample_peak']):int(row['sample_next_trough'])+1]
 
         else:
             decay_period = sig[int(row['sample_last_peak']):int(row['sample_trough'])+1]
@@ -278,15 +306,15 @@
         rise_mono = np.mean(np.diff(rise_period) > 0)
         monotonicity[idx] = np.mean([decay_mono, rise_mono])
 
     return monotonicity
 
 
 def compute_burst_fraction(df_samples, sig, fs, f_range, amp_threshes=(1, 2),
-                           min_n_cycles=3, filter_kwargs=None):
+                           min_n_cycles=3, min_burst_duration=None, filter_kwargs=None):
     """Compute the proportion of each cycle that is bursting using a dual threshold algorithm.
 
     Parameters
     ----------
     df_samples : pandas.DataFrame
         Indices of cyclepoints returned from :func:`~.compute_cyclepoints`.
     sig : 1d array
@@ -297,14 +325,16 @@
         Frequency range (Hz) for oscillaton of interest.
     amp_threshes : tuple (low, high), optional, default: (1, 2)
         Threshold values for determining timing of bursts.
         These values are in units of amplitude (or power, if specified) normalized to
         the median amplitude (value 1).
     min_n_cycles : int, optional, default: 3
         Minimum number of consecutive cycles to be identified as an oscillation.
+    min_burst_duration : float, optional, default: None
+        Minimum length of a burst, in seconds.
     filter_kwargs : dict, optional, default: None
         Keyword arguments to :func:`~neurodsp.filt.filter.filter_signal`.
 
     Returns
     -------
     burst_fraction : 1d array
         The proportion of each cycle that is bursting.
@@ -323,31 +353,36 @@
     >>> fs = 500
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_samples = compute_cyclepoints(sig, fs, f_range=(8, 12))
     >>> burst_fraction = compute_burst_fraction(df_samples, sig, fs, f_range=(8, 12))
     """
 
     # Ensure arguments are within valid ranges
-    check_param(fs, 'fs', (0, np.inf))
-    check_param(amp_threshes[0], 'lower amp_threshes', (0, amp_threshes[1]))
-    check_param(amp_threshes[1], 'upper amp_threshes', (amp_threshes[0], np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
+    check_param_range(amp_threshes[0], 'lower amp_threshes', (0, amp_threshes[1]))
+    check_param_range(amp_threshes[1], 'upper amp_threshes', (amp_threshes[0], np.inf))
 
     filter_kwargs = {} if filter_kwargs is None else filter_kwargs
 
     # Detect bursts using the dual amplitude threshold approach
-    is_burst = detect_bursts_dual_threshold(sig, fs, amp_threshes, f_range,
-                                            min_n_cycles=min_n_cycles, **filter_kwargs)
+    if min_burst_duration is not None:
+        min_n_cycles = None
+
+    is_burst = detect_bursts_dual_threshold(
+        sig, fs, amp_threshes, f_range, min_n_cycles=min_n_cycles,
+        min_burst_duration=min_burst_duration, **filter_kwargs
+    )
 
     # Convert the boolean array to binary
     is_burst = is_burst.astype(int)
 
     # Determine cycle sides
     side_e = 'trough' if 'sample_peak' in df_samples.columns else 'peak'
 
     # Compute fraction of each cycle that's bursting
     burst_fraction = []
-    for _, row in df_samples.iterrows():
+    for row in df_samples.to_dict('records'):
         fraction_bursting = np.mean(is_burst[int(row['sample_last_' + side_e]):
                                              int(row['sample_next_' + side_e] + 1)])
         burst_fraction.append(fraction_bursting)
 
     return burst_fraction
```

### Comparing `bycycle-1.0.0rc2/bycycle/features/cyclepoints.py` & `bycycle-1.1.0/bycycle/features/cyclepoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Compute cyclepoint features for individual cycles."""
 
 import pandas as pd
 import numpy as np
 
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range
 from bycycle.cyclepoints import find_extrema, find_zerox
 
 ###################################################################################################
 ###################################################################################################
 
 def compute_cyclepoints(sig, fs, f_range, **find_extrema_kwargs):
     """Compute sample indices of cyclepoints.
@@ -47,15 +47,15 @@
     >>> from neurodsp.sim import sim_bursty_oscillation
     >>> fs = 500
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_samples = compute_cyclepoints(sig, fs, f_range=(8, 12))
     """
 
     # Ensure arguments are within valid range
-    check_param(fs, 'fs', (0, np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
 
     # Find extrema and zero-crossings locations in the signal
     peaks, troughs = find_extrema(sig, fs, f_range, **find_extrema_kwargs)
     rises, decays = find_zerox(sig, peaks, troughs)
 
     # For each cycle, identify the sample of each extrema and zero-crossing
     samples = {}
```

### Comparing `bycycle-1.0.0rc2/bycycle/features/features.py` & `bycycle-1.1.0/bycycle/features/features.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Compute cycle-by-cycle features."""
 
 import warnings
 import numpy as np
 import pandas as pd
 
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range
 from bycycle.utils.dataframes import drop_samples_df
 from bycycle.features.shape import compute_shape_features
 from bycycle.features.burst import compute_burst_features
 from bycycle.burst import detect_bursts_cycles, detect_bursts_amp
 
 ###################################################################################################
 ###################################################################################################
@@ -103,15 +103,15 @@
     >>> from neurodsp.sim import sim_bursty_oscillation
     >>> fs = 500
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_features = compute_features(sig, fs, f_range=(8, 12))
     """
 
     # Ensure arguments are within valid range
-    check_param(fs, 'fs', (0, np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
 
     # Compute shape features for each cycle
     df_shape_features = compute_shape_features(sig, fs, f_range, center_extrema=center_extrema,
                                                find_extrema_kwargs=find_extrema_kwargs)
 
     # Ensure kwargs are a dictionaries
     if burst_method == 'amp' and not isinstance(burst_kwargs, dict):
@@ -127,14 +127,19 @@
             """)
 
     # Ensure required kwargs are set for amplitude burst detection
     if burst_method == 'amp':
         burst_kwargs['fs'] = fs
         burst_kwargs['f_range'] = f_range
 
+    if burst_method == 'amp' and 'min_n_cycles' not in burst_kwargs.keys():
+        burst_kwargs['min_n_cycles'] = threshold_kwargs.copy().pop('min_n_cycles', 3)
+    elif burst_method == 'amp' and 'min_n_cycles' in burst_kwargs.keys():
+        threshold_kwargs['min_n_cycles'] = burst_kwargs['min_n_cycles']
+
     # Compute burst features for each cycle
     df_burst_features = compute_burst_features(df_shape_features, sig, burst_method=burst_method,
                                                burst_kwargs=burst_kwargs)
 
     # Concatenate shape and burst features
     df_features = pd.concat((df_burst_features, df_shape_features), axis=1)
```

### Comparing `bycycle-1.0.0rc2/bycycle/features/shape.py` & `bycycle-1.1.0/bycycle/features/shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Compute shape features for individual cycles."""
 
 import numpy as np
 import pandas as pd
 
 from neurodsp.timefrequency import amp_by_time
 
-from bycycle.utils import rename_extrema_df, check_param
+from bycycle.utils import rename_extrema_df, check_param_range
 from bycycle.features.cyclepoints import compute_cyclepoints
 
 ###################################################################################################
 ###################################################################################################
 
 def compute_shape_features(sig, fs, f_range, center_extrema='peak',
                            find_extrema_kwargs=None, n_cycles=3):
@@ -75,16 +75,16 @@
     >>> from neurodsp.sim import sim_bursty_oscillation
     >>> fs = 500
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_shapes = compute_shape_features(sig, fs, f_range=(8, 12))
     """
 
     # Ensure arguments are within valid ranges
-    check_param(fs, 'fs', (0, np.inf))
-    check_param(n_cycles, 'n_cycles', (0, np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
+    check_param_range(n_cycles, 'n_cycles', (0, np.inf))
 
     # Set defaults if user input is None
     if find_extrema_kwargs is None:
         find_extrema_kwargs = {'filter_kwargs': {'n_cycles': n_cycles}}
 
     elif 'first_extrema' in find_extrema_kwargs.keys():
         raise ValueError("This function has been designed to assume that the first extrema "
@@ -308,16 +308,16 @@
     >>> fs = 500
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_samples = compute_cyclepoints(sig, fs, f_range=(8, 12))
     >>> band_amp = compute_band_amp(df_samples, sig, fs, f_range=(8, 12))
     """
 
     # Ensure arguments are within valid ranges
-    check_param(fs, 'fs', (0, np.inf))
-    check_param(n_cycles, 'n_cycles', (0, np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
+    check_param_range(n_cycles, 'n_cycles', (0, np.inf))
 
     amp = amp_by_time(sig, fs, f_range, remove_edges=False, n_cycles=n_cycles)
 
     troughs = np.append(df_samples['sample_last_trough'].values[0],
                         df_samples['sample_next_trough'].values)
 
     band_amp = [np.mean(amp[troughs[sig_idx]:troughs[sig_idx + 1]]) for
```

### Comparing `bycycle-1.0.0rc2/bycycle/group/features.py` & `bycycle-1.1.0/bycycle/group/features.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/group/utils.py` & `bycycle-1.1.0/bycycle/group/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 from importlib import import_module
 import numpy as np
 
 ###################################################################################################
 ###################################################################################################
 
-def progress_bar(iterable, progress, n_to_run):
+def progress_bar(iterable, progress, n_to_run, pbar_desc='Computing Bycycle Features'):
     """Add a progress bar to an iterable to be processed.
 
     Parameters
     ----------
     iterable : list or iterable
         Iterable object to potentially apply progress tracking to.
     progress : {None, 'tqdm', 'tqdm.notebook'}
         Which kind of progress bar to use. If None, no progress bar is used.
     n_to_run : int
         Number of jobs to complete.
+    pbar_desc: str, optional
+        Display text for the progress bar.
 
     Returns
     -------
     pbar : iterable or tqdm object
         Iterable object, with tqdm progress functionality, if requested.
 
     Raises
@@ -53,17 +55,14 @@
     """
 
     # Check progress specifier is okay
     tqdm_options = ['tqdm', 'tqdm.notebook']
     if progress is not None and progress not in tqdm_options:
         raise ValueError("Progress bar option not understood.")
 
-    # Set the display text for the progress bar
-    pbar_desc = 'Computing Bycycle Features'
-
     # Use a tqdm, progress bar, if requested
     if progress:
 
         # Try loading the tqdm module
         try:
             tqdm = import_module(progress)
```

### Comparing `bycycle-1.0.0rc2/bycycle/plts/burst.py` & `bycycle-1.1.0/bycycle/plts/burst.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import matplotlib.pyplot as plt
 
 from neurodsp.plts import plot_time_series, plot_bursts
 from neurodsp.plts.utils import savefig
 
 from bycycle.plts.cyclepoints import plot_cyclepoints_df
 from bycycle.utils import limit_df, limit_signal, get_extrema_df
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range
 
 ###################################################################################################
 ###################################################################################################
 
 @savefig
 def plot_burst_detect_summary(df_features, sig, fs, threshold_kwargs, xlim=None,
                               figsize=(15, 3), plot_only_result=False, interp=True):
@@ -70,85 +70,93 @@
     >>> threshold_kwargs = {'amp_fraction_threshold': 0., 'amp_consistency_threshold': .5,
     ...                     'period_consistency_threshold': .5, 'monotonicity_threshold': .8}
     >>> df_features = compute_features(sig, fs, f_range=(8, 12), threshold_kwargs=threshold_kwargs)
     >>> plot_burst_detect_summary(df_features, sig, fs, threshold_kwargs)
     """
 
     # Ensure arguments are within valid range
-    check_param(fs, 'fs', (0, np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
 
     # Normalize signal
-    sig = zscore(sig)
+    sig_full = zscore(sig)
+    times_full = np.arange(0, len(sig_full) / fs, 1 / fs)
 
-    # Determine time array and limits
-    times = np.arange(0, len(sig) / fs, 1 / fs)
-    xlim = (times[0], times[-1]) if xlim is None else xlim
+    # Limit arrays and dataframe
+    if xlim is not None:
+        sig, times = limit_signal(times_full, sig_full, start=xlim[0], stop=xlim[1])
+        df_features = limit_df(df_features, fs, start=xlim[0], stop=xlim[1], reset_indices=False)
+    else:
+        sig, times, = sig_full, times_full
 
     # Determine if peak of troughs are the sides of an oscillation
     _, side_e = get_extrema_df(df_features)
 
     # Remove this kwarg since it isn't stored cycle by cycle in the df (nothing to plot)
-    if 'min_n_cycles' in threshold_kwargs.keys():
-        del threshold_kwargs['min_n_cycles']
+    thresholds = threshold_kwargs.copy()
+    if 'min_n_cycles' in thresholds.keys():
+        del thresholds['min_n_cycles']
 
-    n_kwargs = len(threshold_kwargs.keys())
+    n_kwargs = len(thresholds.keys())
 
     # Create figure and subplots
     if plot_only_result:
         fig, axes = plt.subplots(figsize=figsize, nrows=1)
         axes = [axes]
     else:
         fig, axes = plt.subplots(figsize=(figsize[0], figsize[1]*(n_kwargs+1)),
                                  nrows=n_kwargs+1, sharex=True)
 
     # Determine which samples are defined as bursting
     is_osc = np.zeros(len(sig), dtype=bool)
     df_osc = df_features.loc[df_features['is_burst']]
+    start = 0 if xlim is None else xlim[0]
 
-    for _, cyc in df_osc.iterrows():
+    for cyc in df_osc.to_dict('records'):
+
+        samp_start_burst = int(cyc['sample_last_' + side_e]) - int(fs * start)
+        samp_end_burst = int(cyc['sample_next_' + side_e] + 1) - int(fs * start)
 
-        samp_start_burst = int(cyc['sample_last_' + side_e])
-        samp_end_burst = int(cyc['sample_next_' + side_e] + 1)
         is_osc[samp_start_burst:samp_end_burst] = True
 
     # Plot bursts with extrema points
     xlabel = 'Time (s)' if len(axes) == 1 else ''
 
-    plot_bursts(times, sig, is_osc, ax=axes[0], xlim=xlim, lw=2,
+    plot_bursts(times, sig, is_osc, ax=axes[0], lw=2,
                 labels=['Signal', 'Bursts'], xlabel='', ylabel='')
 
-    plot_cyclepoints_df(df_features, sig, fs, ax=axes[0], xlim=xlim, plot_zerox=False,
+    plot_cyclepoints_df(df_features, sig_full, fs, xlim=xlim, ax=axes[0], plot_zerox=False,
                         plot_sig=False, xlabel=xlabel, ylabel='Voltage\n(normalized)',
                         colors=['m', 'c'])
 
     # Plot each burst param
     colors = cycle(['blue', 'red', 'yellow', 'green', 'cyan', 'magenta', 'orange'])
 
-    for idx, osc_key in enumerate(threshold_kwargs.keys()):
+    for idx, osc_key in enumerate(thresholds.keys()):
 
         column = osc_key.replace('_threshold', '')
 
         color = next(colors)
 
         # Highlight where a burst param falls below threshold
-        for _, cyc in df_features.iterrows():
+        for cyc in df_features.to_dict('records'):
 
-            if cyc[column] < threshold_kwargs[osc_key]:
-                axes[0].axvspan(times[int(cyc['sample_last_' + side_e])],
-                                times[int(cyc['sample_next_' + side_e])],
-                                alpha=0.5, color=color, lw=0)
+            last_cyc = int(cyc['sample_last_' + side_e]) - int(fs * start)
+            next_cyc = int(cyc['sample_next_' + side_e]) - int(fs * start)
+            if cyc[column] < threshold_kwargs[osc_key] and last_cyc > 0:
+                axes[0].axvspan(times[last_cyc], times[next_cyc],
+                 alpha=0.5, color=color, lw=0)
 
         # Plot each burst param on separate axes
         if not plot_only_result:
 
             ylabel = column.replace('_', ' ').capitalize()
             xlabel = 'Time (s)' if idx == n_kwargs-1 else ''
 
-            plot_burst_detect_param(df_features, sig, fs, column, threshold_kwargs[osc_key],
-                                    figsize=figsize, ax=axes[idx+1], xlim=xlim, xlabel=xlabel,
+            plot_burst_detect_param(df_features, sig_full, fs, column, thresholds[osc_key],
+                                    xlim=xlim, figsize=figsize, ax=axes[idx+1], xlabel=xlabel,
                                     ylabel=ylabel, color=color, interp=interp)
 
 
 @savefig
 def plot_burst_detect_param(df_features, sig, fs, burst_param, thresh,
                             xlim=None, interp=True, ax=None, **kwargs):
     """Plot a burst detection parameter and threshold.
@@ -198,70 +206,70 @@
     ...                     'period_consistency_threshold': .5, 'monotonicity_threshold': .8}
     >>> df_features = compute_features(sig, fs, f_range=(8, 12),
     ...                                            threshold_kwargs=threshold_kwargs)
     >>> plot_burst_detect_param(df_features, sig, fs, 'monotonicity', .8)
     """
 
     # Ensure arguments are within valid range
-    check_param(fs, 'fs', (0, np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
 
     # Set default kwargs
     figsize = kwargs.pop('figsize', (15, 3))
     xlabel = kwargs.pop('xlabel', 'Time (s)')
     ylabel = kwargs.pop('ylabel', burst_param)
     color = kwargs.pop('color', 'r')
 
     # Determine time array and limits
     times = np.arange(0, len(sig) / fs, 1 / fs)
-    xlim = (times[0], times[-1]) if xlim is None else xlim
 
     if ax is None:
         fig, ax = plt.subplots(figsize=figsize)
 
     # Determine extrema strings
     center_e, side_e = get_extrema_df(df_features)
 
-    # Limit dataframe, sig and times
-    df = limit_df(df_features, fs, start=xlim[0], stop=xlim[1])
-
-    sig, times = limit_signal(times, sig, start=xlim[0], stop=xlim[1])
+    if xlim is not None:
 
-    # Remove start / end cycles that tlims falls between
-    df = df[(df['sample_last_' + side_e] >= 0) & \
-            (df['sample_next_' + side_e] < xlim[1]*fs)]
+        # Limit dataframe, sig and times
+        df_features = limit_df(df_features, fs, start=xlim[0], stop=xlim[1])
+        sig, times = limit_signal(times, sig, start=xlim[0], stop=xlim[1])
+
+        # Remove start / end cycles that tlims falls between
+        df_features = df_features[(df_features['sample_last_' + side_e] >= 0) & \
+                                  (df_features['sample_next_' + side_e] < xlim[1]*fs)]
 
     # Plot burst param
     if interp:
 
-        plot_time_series([times[df['sample_' + center_e]], xlim],
-                         [df[burst_param], [thresh]*2], ax=ax, colors=['k', 'k'],
+        plot_time_series([times[df_features['sample_' + center_e]], (times[0], times[-1])],
+                         [df_features[burst_param], [thresh]*2], ax=ax, colors=['k', 'k'],
                          ls=['-', '--'], marker=["o", None], xlabel=xlabel,
                          ylabel="{0:s}\nthreshold={1:.2f}".format(ylabel, thresh), **kwargs)
 
     else:
 
         # Create steps, from side to side of each cycle, and set the y-value
         #   to the burst parameter value for that cycle
         side_times = np.array([])
         side_param = np.array([])
 
-        for _, cyc in df.iterrows():
+        for cyc in df_features.to_dict('records'):
 
             # Get the times for the last and next side of a cycle
             side_times = np.append(side_times, [times[int(cyc['sample_last_' + side_e])],
                                                 times[int(cyc['sample_next_' + side_e])]])
 
             # Set the y-value, from side to side, to the burst param for each cycle
             side_param = np.append(side_param, [cyc[burst_param]] * 2)
 
-        plot_time_series([side_times, xlim], [side_param, [thresh]*2], ax=ax, colors=['k', 'k'],
-                         ls=['-', '--'], marker=["o", None], xlim=xlim, xlabel=xlabel,
+        plot_time_series([side_times, (times[0], times[-1])], [side_param, [thresh]*2], ax=ax,
+                         colors=['k', 'k'], ls=['-', '--'], marker=["o", None], xlabel=xlabel,
                          ylabel="{0:s}\nthreshold={1:.2f}".format(ylabel, thresh), **kwargs)
 
     # Highlight where param falls below threshold
-    for _, cyc in df.iterrows():
+    for cyc in df_features.to_dict('records'):
 
         if cyc[burst_param] <= thresh:
 
             ax.axvspan(times[int(cyc['sample_last_' + side_e])],
                        times[int(cyc['sample_next_' + side_e])],
                        alpha=0.5, color=color, lw=0)
```

### Comparing `bycycle-1.0.0rc2/bycycle/plts/cyclepoints.py` & `bycycle-1.1.0/bycycle/plts/cyclepoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from neurodsp.plts import plot_time_series
 from neurodsp.plts.utils import savefig
 
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range
 from bycycle.utils import limit_signal, get_extrema_df
 
 ###################################################################################################
 ###################################################################################################
 
 @savefig
 def plot_cyclepoints_df(df_samples, sig, fs, plot_sig=True, plot_extrema=True,
@@ -55,26 +55,28 @@
     >>> fs = 500
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_samples = compute_cyclepoints(sig, fs, f_range=(8, 12))
     >>> plot_cyclepoints_df(df_samples, sig, fs)
     """
 
     # Ensure arguments are within valid range
-    check_param(fs, 'fs', (0, np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
 
     # Determine extrema/zero-crossings from dataframe
     center_e, side_e = get_extrema_df(df_samples)
 
     peaks, troughs, rises, decays = [None]*4
 
     if plot_extrema:
 
         peaks = df_samples['sample_' + center_e].values
         troughs = np.append(df_samples['sample_last_' + side_e].values,
-                            df_samples['sample_next_' + side_e].values[-1])
+                            df_samples['sample_next_' + side_e].values)
+        troughs = np.unique(troughs)
+
     if plot_zerox:
 
         rises = df_samples['sample_zerox_rise'].values
         decays = df_samples['sample_zerox_decay'].values
 
     plot_cyclepoints_array(sig, fs, peaks=peaks, troughs=troughs, rises=rises,
                            decays=decays, plot_sig=plot_sig, xlim=xlim, ax=ax, **kwargs)
@@ -127,22 +129,22 @@
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> peaks, troughs = find_extrema(sig, fs, f_range=(8, 12), boundary=0)
     >>> rises, decays = find_zerox(sig, peaks, troughs)
     >>> plot_cyclepoints_array(sig, fs, peaks=peaks, troughs=troughs, rises=rises, decays=decays)
     """
 
     # Ensure arguments are within valid range
-    check_param(fs, 'fs', (0, np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
 
     # Set times and limits
     times = np.arange(0, len(sig) / fs, 1 / fs)
-    xlim = (times[0], times[-1]) if xlim is None else xlim
 
     # Restrict sig and times to xlim
-    sig, times = limit_signal(times, sig, start=xlim[0], stop=xlim[1])
+    if xlim is not None:
+        sig, times = limit_signal(times, sig, start=xlim[0], stop=xlim[1])
 
     # Set default kwargs
     figsize = kwargs.pop('figsize', (15, 3))
     xlabel = kwargs.pop('xlabel', 'Time (s)')
     ylabel = kwargs.pop('ylabel', 'Voltage (uV)')
     default_colors = ['b', 'r', 'g', 'm']
 
@@ -152,16 +154,16 @@
     colors = ['k']
 
     for idx, points in enumerate([peaks, troughs, rises, decays]):
 
         if points is not None:
 
             # Limit times and shift indices of cyclepoints (cps)
-            cps = points[(points >= xlim[0]*fs) & (points < xlim[1]*fs)]
-            cps = cps - int(xlim[0]*fs)
+            cps = points[(points >= times[0]*fs) & (points < times[-1]*fs)]
+            cps = cps - int(times[0]*fs)
 
             y_values.append(sig[cps])
             x_values.append(times[cps])
             colors.append(default_colors[idx])
 
     # Allow custom colors to overwrite default
     colors = kwargs.pop('colors', colors)
```

### Comparing `bycycle-1.0.0rc2/bycycle/plts/features.py` & `bycycle-1.1.0/bycycle/plts/features.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/burst/test_amp.py` & `bycycle-1.1.0/bycycle/tests/burst/test_amp.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/burst/test_cycle.py` & `bycycle-1.1.0/bycycle/tests/burst/test_cycle.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/burst/test_utils.py` & `bycycle-1.1.0/bycycle/tests/burst/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,7 +56,23 @@
     df_features_edges = recompute_edges(df_features, threshold_kwargs)
 
     # Ensure that at least one cycle was added to is_burst after recomputed
     is_burst_orig = len(np.where(df_features['is_burst'] == True)[0])
     is_burst_recompute = len(np.where(df_features_edges['is_burst'] == True)[0])
 
     assert is_burst_recompute > is_burst_orig
+
+
+def test_recompute_edge(sim_args_comb):
+
+    # Grab sim arguments from fixture
+    threshold_kwargs = sim_args_comb['threshold_kwargs']
+    df_features = sim_args_comb['df_features']
+
+    threshold_kwargs['amp_consistency_threshold'] = 0
+    threshold_kwargs['period_consistency_threshold'] = 0
+
+    df_features_edge = recompute_edge(df_features.copy(), 0, 'next')
+
+    # The first cycle's consistency will now be a value, rather than nan
+    assert df_features_edge['amp_consistency'][0] != df_features['amp_consistency'][0]
+    assert df_features_edge['period_consistency'][0] != df_features['period_consistency'][0]
```

### Comparing `bycycle-1.0.0rc2/bycycle/tests/conftest.py` & `bycycle-1.1.0/bycycle/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Configuration file for pytest for bycycle."""
 
 import os
 import shutil
 
 import pytest
 
+import numpy as np
+
 from neurodsp.sim import sim_oscillation, sim_combined
 from neurodsp.utils.sim import set_random_seed
 
 from bycycle.features import compute_shape_features, compute_burst_features, compute_features
 from bycycle.tests.settings import (N_SECONDS, FS, FREQ, F_RANGE,
                                     BASE_TEST_FILE_PATH, TEST_PLOTS_PATH)
 
@@ -73,9 +75,9 @@
     os.mkdir(TEST_PLOTS_PATH)
 
 
 @pytest.fixture(scope='module')
 def sim_stationary():
 
     sig = sim_oscillation(N_SECONDS, FS, FREQ, phase=0.15, cycle="asine", rdsym=.3)
-    
+
     yield sig
```

### Comparing `bycycle-1.0.0rc2/bycycle/tests/cyclepoints/test_extrema.py` & `bycycle-1.1.0/bycycle/tests/cyclepoints/test_extrema.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/cyclepoints/test_phase.py` & `bycycle-1.1.0/bycycle/tests/cyclepoints/test_phase.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/cyclepoints/test_zerox.py` & `bycycle-1.1.0/bycycle/tests/cyclepoints/test_zerox.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/features/test_burst.py` & `bycycle-1.1.0/bycycle/tests/features/test_burst.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/features/test_cyclepoints.py` & `bycycle-1.1.0/bycycle/tests/features/test_cyclepoints.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/features/test_features.py` & `bycycle-1.1.0/bycycle/tests/features/test_features.py`

 * *Files 20% similar despite different names*

```diff
@@ -38,10 +38,10 @@
 
     if return_samples:
 
         sample_cols = [col for col in list(df_features.columns) if "sample_" in col]
         assert len(sample_cols) == 6
 
     # Assert that np.nan isn't in dataframe columns
-    for _, column in df_features.iteritems():
+    for column in df_features.keys():
 
-        assert not np.isnan(column[1:-1]).any()
+        assert not np.isnan(df_features[column].iloc[1:-1]).any()
```

### Comparing `bycycle-1.0.0rc2/bycycle/tests/features/test_shapes.py` & `bycycle-1.1.0/bycycle/tests/features/test_shapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
                                        find_extrema_kwargs=find_extrema_kwargs)
 
     # Ensure sample columns are returned
     sample_cols = [col for col in list(df_shapes.columns) if "sample_" in col]
     assert len(sample_cols) == 6
 
     # Assert that np.nan isn't in dataframe(s), with the exception of the first and last row
-    for idx, row in df_shapes.iterrows():
-
+    for idx, row in enumerate(df_shapes.to_dict('records')):
+        row = list(row.values())
         assert not np.isnan(row[1:-1]).any()
 
     # Check inverted signal gives appropriately opposite data
     extrema_opp = 'trough' if center_extrema == 'peak' else 'peak'
 
     df_opp = compute_shape_features(-sig, fs, f_range,
                                     center_extrema=extrema_opp,
```

### Comparing `bycycle-1.0.0rc2/bycycle/tests/group/test_features.py` & `bycycle-1.1.0/bycycle/tests/group/test_features.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/group/test_utils.py` & `bycycle-1.1.0/bycycle/tests/group/test_utils.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/plts/test_burst.py` & `bycycle-1.1.0/bycycle/tests/plts/test_burst.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/plts/test_cyclepoints.py` & `bycycle-1.1.0/bycycle/tests/plts/test_cyclepoints.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/plts/test_features.py` & `bycycle-1.1.0/bycycle/tests/plts/test_features.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/tutils.py` & `bycycle-1.1.0/bycycle/tests/tutils.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/utils/test_dataframes.py` & `bycycle-1.1.0/bycycle/tests/utils/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/tests/utils/test_timeseries.py` & `bycycle-1.1.0/bycycle/tests/utils/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `bycycle-1.0.0rc2/bycycle/utils/dataframes.py` & `bycycle-1.1.0/bycycle/utils/dataframes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """Utility functions for working with ByCycle DataFrames."""
 
 from itertools import product
 
 import numpy as np
 import pandas as pd
 
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range
 
 ###################################################################################################
 ###################################################################################################
 
-def limit_df(df, fs, start=None, stop=None):
+def limit_df(df, fs, start=None, stop=None, reset_indices=True):
     """Restrict dataframe to be within time limits.
 
     Parameters
     ----------
     df : pandas.DataFrame
         Dataframe output of :func:`~.compute_features`.
     fs : float
         Sampling rate, in Hz.
     start : float, optional
         The lower time limit, in seconds, to restrict the df.
     stop : float, optional
         The upper time limit, in seconds, to restrict the df.
+    reset_indices : bool, optional, default: True
+        Samples start at zero when True.
 
     Returns
     -------
     df : pandas.DataFrame
         A limited dataframe of cycle features.
 
     Notes
@@ -43,33 +45,35 @@
     >>> fs = 500
     >>> sig = sim_bursty_oscillation(10, fs, freq=10)
     >>> df_features = compute_features(sig, fs, f_range=(8, 12))
     >>> df_features = limit_df(df_features, fs, start=0, stop=1)
     """
 
     # Ensure arguments are within valid range
-    check_param(fs, 'fs', (0, np.inf))
-    check_param(start, 'start', (0, stop))
-    check_param(stop, 'stop', (start, np.inf))
+    check_param_range(fs, 'fs', (0, np.inf))
+    check_param_range(start, 'start', (0, stop))
+    check_param_range(stop, 'stop', (start, np.inf))
 
     center_e, side_e = get_extrema_df(df)
 
     start = 0 if start is None else start
 
-    df = df[df['sample_next_' + side_e].values >= start*fs]
+    df = df[df['sample_last_' + side_e].values >= start*fs]
 
     if stop is not None:
-        df = df[df['sample_last_' + side_e].values < stop*fs]
+        df = df[df['sample_next_' + side_e].values <= stop*fs]
 
     # Shift sample indices to start at 0
-    df['sample_last_' + side_e] = df['sample_last_' + side_e] - int(fs * start)
-    df['sample_next_' + side_e] = df['sample_next_' + side_e] - int(fs * start)
-    df['sample_' + center_e] = df['sample_' + center_e] - int(fs * start)
-    df['sample_zerox_rise'] = df['sample_zerox_rise'] - int(fs * start)
-    df['sample_zerox_decay'] = df['sample_zerox_decay'] - int(fs * start)
+    if reset_indices:
+        df['sample_last_' + side_e] = df['sample_last_' + side_e] - int(fs * start)
+        df['sample_next_' + side_e] = df['sample_next_' + side_e] - int(fs * start)
+        df['sample_' + center_e] = df['sample_' + center_e] - int(fs * start)
+        df['sample_zerox_rise'] = df['sample_zerox_rise'] - int(fs * start)
+        df['sample_zerox_decay'] = df['sample_zerox_decay'] - int(fs * start)
+        df['sample_last_zerox_decay'] = df['sample_last_zerox_decay'] - int(fs * start)
 
     return df
 
 
 def get_extrema_df(df):
     """Determine whether cycles are peak or trough centered.
```

### Comparing `bycycle-1.0.0rc2/bycycle/utils/timeseries.py` & `bycycle-1.1.0/bycycle/utils/timeseries.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Utility functions for working with time series."""
 
 import numpy as np
 
-from bycycle.utils.checks import check_param
+from bycycle.utils.checks import check_param_range
 
 ###################################################################################################
 ###################################################################################################
 
 def limit_signal(times, sig, start=None, stop=None):
     """Restrict signal and times to be within time limits.
 
@@ -36,16 +36,16 @@
     >>> from neurodsp.utils import create_times
     >>> sig = sim_bursty_oscillation(n_seconds=10, fs=500, freq=10)
     >>> times = create_times(n_seconds=10, fs=500)
     >>> sig, times = limit_signal(times, sig, start=0, stop=1)
     """
 
     # Ensure arguments are within valid range
-    check_param(start, 'start', (0, stop))
-    check_param(stop, 'stop', (start, np.inf))
+    check_param_range(start, 'start', (0, stop))
+    check_param_range(stop, 'stop', (start, np.inf))
 
     if start is not None:
         sig = sig[times >= start]
         times = times[times >= start]
 
     if stop is not None:
         sig = sig[times < stop]
```

### Comparing `bycycle-1.0.0rc2/bycycle.egg-info/SOURCES.txt` & `bycycle-1.1.0/bycycle.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,21 +23,24 @@
 bycycle/features/burst.py
 bycycle/features/cyclepoints.py
 bycycle/features/features.py
 bycycle/features/shape.py
 bycycle/group/__init__.py
 bycycle/group/features.py
 bycycle/group/utils.py
+bycycle/objs/__init__.py
+bycycle/objs/fit.py
 bycycle/plts/__init__.py
 bycycle/plts/burst.py
 bycycle/plts/cyclepoints.py
 bycycle/plts/features.py
 bycycle/tests/__init__.py
 bycycle/tests/conftest.py
 bycycle/tests/settings.py
+bycycle/tests/test_persistence.py
 bycycle/tests/tutils.py
 bycycle/tests/burst/__init__.py
 bycycle/tests/burst/test_amp.py
 bycycle/tests/burst/test_cycle.py
 bycycle/tests/burst/test_utils.py
 bycycle/tests/cyclepoints/__init__.py
 bycycle/tests/cyclepoints/test_extrema.py
@@ -47,18 +50,22 @@
 bycycle/tests/features/test_burst.py
 bycycle/tests/features/test_cyclepoints.py
 bycycle/tests/features/test_features.py
 bycycle/tests/features/test_shapes.py
 bycycle/tests/group/__init__.py
 bycycle/tests/group/test_features.py
 bycycle/tests/group/test_utils.py
+bycycle/tests/objs/__init__.py
+bycycle/tests/objs/test_fit.py
 bycycle/tests/plts/__init__.py
 bycycle/tests/plts/test_burst.py
 bycycle/tests/plts/test_cyclepoints.py
 bycycle/tests/plts/test_features.py
 bycycle/tests/utils/__init__.py
 bycycle/tests/utils/test_dataframes.py
+bycycle/tests/utils/test_download.py
 bycycle/tests/utils/test_timeseries.py
 bycycle/utils/__init__.py
 bycycle/utils/checks.py
 bycycle/utils/dataframes.py
+bycycle/utils/download.py
 bycycle/utils/timeseries.py
```

### Comparing `bycycle-1.0.0rc2/setup.py` & `bycycle-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     install_requires = [req for req in requirements_file.read().splitlines()]
 
 setup(
     name = 'bycycle',
     version = __version__,
     description = 'Cycle-by-cycle analyses of neural oscillations.',
     long_description = long_description,
-    python_requires = '>=3.5',
+    python_requires = '>=3.6',
     author = 'The Voytek Lab',
     author_email = 'voyteklab@gmail.com',
     url = 'https://github.com/bycycle-tools/bycycle',
     packages = find_packages(),
     license = 'Apache License, 2.0',
     classifiers = [
         'Development Status :: 4 - Beta',
@@ -32,18 +32,20 @@
         'Topic :: Scientific/Engineering',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: MacOS',
         'Operating System :: POSIX',
         'Operating System :: Unix',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8'
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     platforms = 'any',
     project_urls = {
         'Documentation' : 'https://bycycle-tools.github.io/bycycle/',
         'Bug Reports' : 'https://github.com/bycycle-tools/bycycle/issues',
         'Source' : 'https://github.com/bycycle-tools/bycycle'
     },
```

