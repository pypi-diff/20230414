# Comparing `tmp/pymeos-1.2.0a0.tar.gz` & `tmp/pymeos-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeos-1.2.0a0.tar", last modified: Mon Apr  3 10:36:09 2023, max compression
+gzip compressed data, was "pymeos-1.2.0a1.tar", last modified: Mon Apr  3 11:13:02 2023, max compression
```

## Comparing `pymeos-1.2.0a0.tar` & `pymeos-1.2.0a1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 10:36:09.837507 pymeos-1.2.0a0/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1298 2022-08-28 11:32:58.000000 pymeos-1.2.0a0/LICENSE
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)       39 2022-08-22 13:17:01.000000 pymeos-1.2.0a0/MANIFEST.in
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2601 2023-04-03 10:36:09.837507 pymeos-1.2.0a0/PKG-INFO
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1894 2022-11-19 15:16:53.000000 pymeos-1.2.0a0/README.md
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 10:36:09.817435 pymeos-1.2.0a0/pymeos/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1497 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/__init__.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 10:36:09.827471 pymeos-1.2.0a0/pymeos/aggregators/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      886 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/aggregators/__init__.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    10851 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/aggregators/aggregator.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      589 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/aggregators/bool_aggregators.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3731 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/aggregators/general_aggregators.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2506 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/aggregators/number_aggregators.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      587 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/aggregators/point_aggregators.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      607 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/aggregators/text_aggregators.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1836 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/aggregators/time_aggregators.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 10:36:09.827471 pymeos-1.2.0a0/pymeos/boxes/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      110 2022-10-25 17:28:37.000000 pymeos-1.2.0a0/pymeos/boxes/__init__.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      302 2023-02-28 14:35:14.000000 pymeos-1.2.0a0/pymeos/boxes/box.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    43637 2023-04-03 08:50:32.000000 pymeos-1.2.0a0/pymeos/boxes/stbox.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    35227 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/boxes/tbox.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 10:36:09.827471 pymeos-1.2.0a0/pymeos/db/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)        0 2022-11-19 15:17:03.000000 pymeos-1.2.0a0/pymeos/db/__init__.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1711 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/db/asyncpg.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2177 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/db/psycopg.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2061 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/db/psycopg2.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     4545 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/factory.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 10:36:09.827471 pymeos-1.2.0a0/pymeos/main/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      924 2022-10-07 17:31:01.000000 pymeos-1.2.0a0/pymeos/main/__init__.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    14420 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/main/tbool.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    27903 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/main/tfloat.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    24741 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/main/tint.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    16827 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/main/tnumber.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    56319 2023-04-03 08:10:58.000000 pymeos-1.2.0a0/pymeos/main/tpoint.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    24110 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/main/ttext.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      702 2023-04-03 08:37:43.000000 pymeos-1.2.0a0/pymeos/meos_init.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 10:36:09.827471 pymeos-1.2.0a0/pymeos/plotters/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      371 2022-10-26 09:44:53.000000 pymeos-1.2.0a0/pymeos/plotters/__init__.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     4802 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/plotters/box_plotter.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3516 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/plotters/point_sequence_plotter.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1600 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/plotters/point_sequenceset_plotter.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1191 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/plotters/range_plotter.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2828 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/plotters/sequence_plotter.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1439 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/plotters/sequenceset_plotter.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3815 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/plotters/time_plotter.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 10:36:09.837507 pymeos-1.2.0a0/pymeos/temporal/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      266 2022-09-21 00:54:06.000000 pymeos-1.2.0a0/pymeos/temporal/__init__.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1312 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/temporal/interpolation.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    40838 2023-04-03 08:56:46.000000 pymeos-1.2.0a0/pymeos/temporal/temporal.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2980 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/temporal/tinstant.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3986 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/temporal/tsequence.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3854 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/temporal/tsequenceset.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 10:36:09.837507 pymeos-1.2.0a0/pymeos/time/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      254 2022-11-11 09:22:02.000000 pymeos-1.2.0a0/pymeos/time/__init__.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    35757 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/time/period.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    36093 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/time/periodset.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      544 2023-02-28 14:34:59.000000 pymeos-1.2.0a0/pymeos/time/time.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    34484 2023-04-03 08:09:40.000000 pymeos-1.2.0a0/pymeos/time/timestampset.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 10:36:09.817435 pymeos-1.2.0a0/pymeos.egg-info/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2601 2023-04-03 10:36:09.000000 pymeos-1.2.0a0/pymeos.egg-info/PKG-INFO
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1464 2023-04-03 10:36:09.000000 pymeos-1.2.0a0/pymeos.egg-info/SOURCES.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)        1 2023-04-03 10:36:09.000000 pymeos-1.2.0a0/pymeos.egg-info/dependency_links.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      134 2023-04-03 10:36:09.000000 pymeos-1.2.0a0/pymeos.egg-info/requires.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)        7 2023-04-03 10:36:09.000000 pymeos-1.2.0a0/pymeos.egg-info/top_level.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1126 2023-04-03 10:35:48.000000 pymeos-1.2.0a0/pyproject.toml
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)       38 2023-04-03 10:36:09.837507 pymeos-1.2.0a0/setup.cfg
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 11:13:02.752102 pymeos-1.2.0a1/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1298 2022-08-28 11:32:58.000000 pymeos-1.2.0a1/LICENSE
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)       39 2022-08-22 13:17:01.000000 pymeos-1.2.0a1/MANIFEST.in
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2601 2023-04-03 11:13:02.752102 pymeos-1.2.0a1/PKG-INFO
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1894 2022-11-19 15:16:53.000000 pymeos-1.2.0a1/README.md
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 11:13:02.742065 pymeos-1.2.0a1/pymeos/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1497 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/__init__.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 11:13:02.742065 pymeos-1.2.0a1/pymeos/aggregators/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      886 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/aggregators/__init__.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    10851 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/aggregators/aggregator.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      589 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/aggregators/bool_aggregators.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3735 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/aggregators/general_aggregators.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2506 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/aggregators/number_aggregators.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      587 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/aggregators/point_aggregators.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      607 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/aggregators/text_aggregators.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1836 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/aggregators/time_aggregators.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 11:13:02.742065 pymeos-1.2.0a1/pymeos/boxes/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      110 2022-10-25 17:28:37.000000 pymeos-1.2.0a1/pymeos/boxes/__init__.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      302 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/boxes/box.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    43639 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/boxes/stbox.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    35227 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/boxes/tbox.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 11:13:02.742065 pymeos-1.2.0a1/pymeos/db/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)        0 2022-11-19 15:17:03.000000 pymeos-1.2.0a1/pymeos/db/__init__.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1711 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/db/asyncpg.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2177 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/db/psycopg.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2061 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/db/psycopg2.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     4545 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/factory.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 11:13:02.742065 pymeos-1.2.0a1/pymeos/main/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      924 2022-10-07 17:31:01.000000 pymeos-1.2.0a1/pymeos/main/__init__.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    14420 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/main/tbool.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    27903 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/main/tfloat.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    24741 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/main/tint.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    16827 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/main/tnumber.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    56323 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/main/tpoint.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    24110 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/main/ttext.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      702 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/meos_init.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 11:13:02.742065 pymeos-1.2.0a1/pymeos/plotters/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      371 2022-10-26 09:44:53.000000 pymeos-1.2.0a1/pymeos/plotters/__init__.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     4802 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/plotters/box_plotter.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3518 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/plotters/point_sequence_plotter.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1600 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/plotters/point_sequenceset_plotter.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1191 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/plotters/range_plotter.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2832 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/plotters/sequence_plotter.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1439 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/plotters/sequenceset_plotter.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3815 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/plotters/time_plotter.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 11:13:02.742065 pymeos-1.2.0a1/pymeos/temporal/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      266 2022-09-21 00:54:06.000000 pymeos-1.2.0a1/pymeos/temporal/__init__.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1312 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/temporal/interpolation.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    40838 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/temporal/temporal.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2980 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/temporal/tinstant.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3986 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/temporal/tsequence.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3854 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/temporal/tsequenceset.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 11:13:02.742065 pymeos-1.2.0a1/pymeos/time/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      254 2022-11-11 09:22:02.000000 pymeos-1.2.0a1/pymeos/time/__init__.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    35757 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/time/period.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    36093 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/time/periodset.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      544 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/time/time.py
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)    34484 2023-04-03 10:47:11.000000 pymeos-1.2.0a1/pymeos/time/timestampset.py
+drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2023-04-03 11:13:02.742065 pymeos-1.2.0a1/pymeos.egg-info/
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     2601 2023-04-03 11:13:02.000000 pymeos-1.2.0a1/pymeos.egg-info/PKG-INFO
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1464 2023-04-03 11:13:02.000000 pymeos-1.2.0a1/pymeos.egg-info/SOURCES.txt
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)        1 2023-04-03 11:13:02.000000 pymeos-1.2.0a1/pymeos.egg-info/dependency_links.txt
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)      144 2023-04-03 11:13:02.000000 pymeos-1.2.0a1/pymeos.egg-info/requires.txt
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)        7 2023-04-03 11:13:02.000000 pymeos-1.2.0a1/pymeos.egg-info/top_level.txt
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1146 2023-04-03 11:08:41.000000 pymeos-1.2.0a1/pyproject.toml
+-rw-r--r--   0 diviloper  (1000) diviloper  (1000)       38 2023-04-03 11:13:02.752102 pymeos-1.2.0a1/setup.cfg
```

### Comparing `pymeos-1.2.0a0/LICENSE` & `pymeos-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/PKG-INFO` & `pymeos-1.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeos
-Version: 1.2.0a0
+Version: 1.2.0a1
 Summary: Python wrapper for the MEOS C Library.
 Author-email: Victor Divi <vdiviloper@gmail.com>, Zhicheng Luo <zhicheng.luo@ulb.be>, Krishna Chaitanya Bommakanti <bkchaitan94@gmail.com>
 License: PostgreSQL
 Project-URL: Homepage, https://github.com/MobilityDB/PyMEOS
 Project-URL: Bug Tracker, https://github.com/MobilityDB/PyMEOS/issues
 Project-URL: Changelog, https://github.com/MobilityDB/PyMEOS/blob/master/pymeos/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymeos-1.2.0a0/README.md` & `pymeos-1.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/__init__.py` & `pymeos-1.2.0a1/pymeos/__init__.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/aggregators/__init__.py` & `pymeos-1.2.0a1/pymeos/aggregators/__init__.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/aggregators/aggregator.py` & `pymeos-1.2.0a1/pymeos/aggregators/aggregator.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/aggregators/bool_aggregators.py` & `pymeos-1.2.0a1/pymeos/aggregators/bool_aggregators.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/aggregators/general_aggregators.py` & `pymeos-1.2.0a1/pymeos/aggregators/general_aggregators.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     @classmethod
     def _add(cls, state, temporal):
         if isinstance(temporal, datetime):
             state = timestamp_tcount_transfn(state, datetime_to_timestamptz(temporal))
         elif isinstance(temporal, TimestampSet):
             state = tstzset_tcount_transfn(state, temporal._inner)
-        elif isinstance(temporal, Temporal) and temporal.interpolation == TInterpolation.DISCRETE:
+        elif isinstance(temporal, Temporal) and temporal.interpolation() == TInterpolation.DISCRETE:
             state = temporal_tcount_transfn(state, temporal._inner)
         else:
             cls._error(temporal)
         return state
 
 
 class TemporalPeriodCountAggregator(BaseAggregator[Union[Period, PeriodSet, Temporal], TIntSeqSet]):
@@ -51,15 +51,15 @@
 
     @classmethod
     def _add(cls, state, temporal):
         if isinstance(temporal, Period):
             state = period_tcount_transfn(state, temporal._inner)
         elif isinstance(temporal, PeriodSet):
             state = periodset_tcount_transfn(state, temporal._inner)
-        elif isinstance(temporal, Temporal) and temporal.interpolation != TInterpolation.DISCRETE:
+        elif isinstance(temporal, Temporal) and temporal.interpolation() != TInterpolation.DISCRETE:
             state = temporal_tcount_transfn(state, temporal._inner)
         else:
             cls._error(temporal)
         return state
 
 
 class TemporalExtentAggregator(BaseAggregator[Union[Time, Temporal], Period]):
```

### Comparing `pymeos-1.2.0a0/pymeos/aggregators/number_aggregators.py` & `pymeos-1.2.0a1/pymeos/aggregators/number_aggregators.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/aggregators/point_aggregators.py` & `pymeos-1.2.0a1/pymeos/aggregators/point_aggregators.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/aggregators/text_aggregators.py` & `pymeos-1.2.0a1/pymeos/aggregators/text_aggregators.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/aggregators/time_aggregators.py` & `pymeos-1.2.0a1/pymeos/aggregators/time_aggregators.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/boxes/stbox.py` & `pymeos-1.2.0a1/pymeos/boxes/stbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
         """
         sz = size or (max(self.xmax() - self.xmin(), self.ymax() - self.ymin(), self.zmax() - self.zmin()) + 1)
         dt = timedelta_to_interval(duration) if isinstance(duration, timedelta) \
             else pg_interval_in(duration, -1) if isinstance(duration, str) \
             else None
         st = datetime_to_timestamptz(start) if isinstance(start, datetime) \
             else pg_timestamptz_in(start, -1) if isinstance(start, str) \
-            else datetime_to_timestamptz(self.tmin()) if self.has_t \
+            else datetime_to_timestamptz(self.tmin()) if self.has_t() \
             else 0
         gs = geometry_to_gserialized(origin) if origin is not None \
             else gserialized_in('Point(0 0 0)', -1)
         tiles, dimensions = stbox_tile_list(self._inner, sz, dt, gs, st)
         x_size = dimensions[0] or 1
         y_size = dimensions[1] or 1
         z_size = dimensions[2] or 1
```

### Comparing `pymeos-1.2.0a0/pymeos/boxes/tbox.py` & `pymeos-1.2.0a1/pymeos/boxes/tbox.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/db/asyncpg.py` & `pymeos-1.2.0a1/pymeos/db/asyncpg.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/db/psycopg.py` & `pymeos-1.2.0a1/pymeos/db/psycopg.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/db/psycopg2.py` & `pymeos-1.2.0a1/pymeos/db/psycopg2.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/factory.py` & `pymeos-1.2.0a1/pymeos/factory.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/main/__init__.py` & `pymeos-1.2.0a1/pymeos/main/__init__.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/main/tbool.py` & `pymeos-1.2.0a1/pymeos/main/tbool.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/main/tfloat.py` & `pymeos-1.2.0a1/pymeos/main/tfloat.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/main/tint.py` & `pymeos-1.2.0a1/pymeos/main/tint.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/main/tnumber.py` & `pymeos-1.2.0a1/pymeos/main/tnumber.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/main/tpoint.py` & `pymeos-1.2.0a1/pymeos/main/tpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -812,15 +812,15 @@
         Returns:
             A new :class:`GeoDataFrame` representing the trajectory.
         """
         data = {
             'time': self.timestamps(),
             'geometry': [i.value() for i in self.instants()]
         }
-        return GeoDataFrame(data, crs=self.srid).set_index(keys=['time'])
+        return GeoDataFrame(data, crs=self.srid()).set_index(keys=['time'])
 
     def __str__(self):
         """
         Returns the string representation of the trajectory.
 
         Returns:
             A new :class:`str` representing the trajectory.
@@ -952,15 +952,15 @@
         """
         sequences = self.sequences()
         data = {
             'sequence': [i + 1 for i, seq in enumerate(sequences) for _ in range(seq.num_instants())],
             'time': [t for seq in sequences for t in seq.timestamps()],
             'geometry': [v for seq in sequences for v in seq.values(precision=precision)]
         }
-        return GeoDataFrame(data, crs=self.srid).set_index(keys=['sequence', 'time'])
+        return GeoDataFrame(data, crs=self.srid()).set_index(keys=['sequence', 'time'])
 
     def plot(self, *args, **kwargs):
         """
         Plots the temporal point sequence set.
 
         Args:
             *args: Additional arguments to pass to the plot function.
```

### Comparing `pymeos-1.2.0a0/pymeos/main/ttext.py` & `pymeos-1.2.0a1/pymeos/main/ttext.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/meos_init.py` & `pymeos-1.2.0a1/pymeos/meos_init.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/plotters/box_plotter.py` & `pymeos-1.2.0a1/pymeos/plotters/box_plotter.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/plotters/point_sequence_plotter.py` & `pymeos-1.2.0a1/pymeos/plotters/point_sequence_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         Returns:
             List with the plotted elements.
         """
         base = axes or plt.gca()
         linear = False
         if isinstance(sequence, list):
             plot_func = base.scatter
-        elif sequence.interpolation == TInterpolation.LINEAR:
+        elif sequence.interpolation() == TInterpolation.LINEAR:
             plot_func = base.plot
             linear = True
         else:
             plot_func = base.scatter
 
         ins = sequence.instants() if isinstance(sequence, TPointSeq) else sequence
         x = [i.x().value() for i in ins]
```

### Comparing `pymeos-1.2.0a0/pymeos/plotters/point_sequenceset_plotter.py` & `pymeos-1.2.0a1/pymeos/plotters/point_sequenceset_plotter.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/plotters/range_plotter.py` & `pymeos-1.2.0a1/pymeos/plotters/range_plotter.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/plotters/sequence_plotter.py` & `pymeos-1.2.0a1/pymeos/plotters/sequence_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         Returns:
             List with the plotted elements.
         """
         base = axes or plt.gca()
         if isinstance(sequence, list):
             plot_func = base.scatter
             show_markers = False
-        elif sequence.interpolation == TInterpolation.LINEAR:
+        elif sequence.interpolation() == TInterpolation.LINEAR:
             plot_func = base.plot
-        elif sequence.interpolation == TInterpolation.STEPWISE:
+        elif sequence.interpolation() == TInterpolation.STEPWISE:
             plot_func = partial(base.step, where='post')
         else:
             plot_func = base.scatter
             show_markers = False
 
         ins = sequence.instants() if isinstance(sequence, TSequence) else sequence
         x = [i.timestamp() for i in ins]
```

### Comparing `pymeos-1.2.0a0/pymeos/plotters/sequenceset_plotter.py` & `pymeos-1.2.0a1/pymeos/plotters/sequenceset_plotter.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/plotters/time_plotter.py` & `pymeos-1.2.0a1/pymeos/plotters/time_plotter.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/temporal/interpolation.py` & `pymeos-1.2.0a1/pymeos/temporal/interpolation.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/temporal/temporal.py` & `pymeos-1.2.0a1/pymeos/temporal/temporal.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/temporal/tinstant.py` & `pymeos-1.2.0a1/pymeos/temporal/tinstant.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/temporal/tsequence.py` & `pymeos-1.2.0a1/pymeos/temporal/tsequence.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/temporal/tsequenceset.py` & `pymeos-1.2.0a1/pymeos/temporal/tsequenceset.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/time/period.py` & `pymeos-1.2.0a1/pymeos/time/period.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/time/periodset.py` & `pymeos-1.2.0a1/pymeos/time/periodset.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/time/time.py` & `pymeos-1.2.0a1/pymeos/time/time.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos/time/timestampset.py` & `pymeos-1.2.0a1/pymeos/time/timestampset.py`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pymeos.egg-info/PKG-INFO` & `pymeos-1.2.0a1/pymeos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeos
-Version: 1.2.0a0
+Version: 1.2.0a1
 Summary: Python wrapper for the MEOS C Library.
 Author-email: Victor Divi <vdiviloper@gmail.com>, Zhicheng Luo <zhicheng.luo@ulb.be>, Krishna Chaitanya Bommakanti <bkchaitan94@gmail.com>
 License: PostgreSQL
 Project-URL: Homepage, https://github.com/MobilityDB/PyMEOS
 Project-URL: Bug Tracker, https://github.com/MobilityDB/PyMEOS/issues
 Project-URL: Changelog, https://github.com/MobilityDB/PyMEOS/blob/master/pymeos/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymeos-1.2.0a0/pymeos.egg-info/SOURCES.txt` & `pymeos-1.2.0a1/pymeos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymeos-1.2.0a0/pyproject.toml` & `pymeos-1.2.0a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pymeos"
-version = "1.2.0-alpha"
+version = "1.2.0-alpha.1"
 authors = [
     { name = "Victor Divi", email = "vdiviloper@gmail.com" },
     { name = "Zhicheng Luo", email = "zhicheng.luo@ulb.be" },
     { name = "Krishna Chaitanya Bommakanti", email = "bkchaitan94@gmail.com" },
 ]
 description = "Python wrapper for the MEOS C Library."
 classifiers = [
@@ -18,14 +18,15 @@
 readme = "README.md"
 license = { text = "PostgreSQL" }
 
 requires-python = ">=3.7"
 dependencies = [
     'pymeos-cffi==0.0.19',
     'python-dateutil',
+    'functools',
     'spans',
     'postgis',
     'shapely',
     'geopandas'
 ]
 
 [project.optional-dependencies]
```

