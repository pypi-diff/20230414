# Comparing `tmp/aeolus-0.4.8.tar.gz` & `tmp/aeolus-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeolus-0.4.8.tar", last modified: Mon Jan 25 21:49:48 2021, max compression
+gzip compressed data, was "aeolus-0.4.9.tar", last modified: Mon Apr 12 13:13:39 2021, max compression
```

## Comparing `aeolus-0.4.8.tar` & `aeolus-0.4.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.748510 aeolus-0.4.8/
--rw-r--r--   0 ds591     (1000) ds591     (1000)     7652 2019-02-28 17:46:52.000000 aeolus-0.4.8/LICENSE
--rw-r--r--   0 ds591     (1000) ds591     (1000)      209 2020-10-13 09:19:31.000000 aeolus-0.4.8/MANIFEST.in
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     2506 2021-01-25 21:49:48.748510 aeolus-0.4.8/PKG-INFO
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     1164 2020-11-26 21:30:51.000000 aeolus-0.4.8/README.md
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.740510 aeolus-0.4.8/docs/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      605 2020-12-17 13:52:16.000000 aeolus-0.4.8/docs/Makefile
--rw-r--r--   0 ds591     (1000) ds591     (1000)      200 2020-12-17 14:32:21.000000 aeolus-0.4.8/docs/environment.yml
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.744510 aeolus-0.4.8/docs/source/
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.744510 aeolus-0.4.8/docs/source/_static/
--rw-r--r--   0 ds591     (1000) ds591     (1000)     4286 2020-01-03 17:53:42.000000 aeolus-0.4.8/docs/source/_static/favicon.ico
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.744510 aeolus-0.4.8/docs/source/api/
--rw-r--r--   0 ds591     (1000) ds591     (1000)     2060 2020-12-03 22:41:49.000000 aeolus-0.4.8/docs/source/api/calc.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      176 2020-01-02 13:49:09.000000 aeolus-0.4.8/docs/source/api/const.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1371 2020-12-03 19:56:03.000000 aeolus-0.4.8/docs/source/api/coord.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      147 2020-12-03 22:55:06.000000 aeolus-0.4.8/docs/source/api/core.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      558 2020-06-08 17:01:40.000000 aeolus-0.4.8/docs/source/api/index.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      123 2020-09-28 16:49:30.000000 aeolus-0.4.8/docs/source/api/io.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      191 2020-06-08 17:03:16.000000 aeolus-0.4.8/docs/source/api/model.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      415 2020-03-31 22:43:42.000000 aeolus-0.4.8/docs/source/api/plot.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)       53 2019-03-28 16:39:59.000000 aeolus-0.4.8/docs/source/api/region.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      301 2020-11-27 11:29:06.000000 aeolus-0.4.8/docs/source/api/subset.rst
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     4238 2021-01-25 21:49:43.000000 aeolus-0.4.8/docs/source/changelog.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)     7287 2020-06-08 18:59:17.000000 aeolus-0.4.8/docs/source/conf.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)      154 2019-02-28 18:01:29.000000 aeolus-0.4.8/docs/source/contributing.rst
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.744510 aeolus-0.4.8/docs/source/examples/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      305 2019-02-28 18:16:56.000000 aeolus-0.4.8/docs/source/examples/_index_header_rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      726 2020-05-03 14:58:16.000000 aeolus-0.4.8/docs/source/index.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)     2604 2020-11-25 15:56:20.000000 aeolus-0.4.8/docs/source/install.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      714 2020-11-26 17:54:26.000000 aeolus-0.4.8/pyproject.toml
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     1914 2021-01-25 21:49:48.748510 aeolus-0.4.8/setup.cfg
--rw-r--r--   0 ds591     (1000) ds591     (1000)      221 2020-10-13 09:13:58.000000 aeolus-0.4.8/setup.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.740510 aeolus-0.4.8/src/
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.748510 aeolus-0.4.8/src/aeolus/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      115 2019-02-28 18:19:47.000000 aeolus-0.4.8/src/aeolus/__init__.py
--rw-rw-r--   0 ds591     (1000) ds591     (1000)      497 2021-01-25 21:49:48.748510 aeolus-0.4.8/src/aeolus/_version.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.744510 aeolus-0.4.8/src/aeolus/calc/
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1980 2020-12-03 22:41:23.000000 aeolus-0.4.8/src/aeolus/calc/__init__.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     5359 2020-12-03 22:34:03.000000 aeolus-0.4.8/src/aeolus/calc/calculus.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)    22233 2021-01-25 21:35:05.000000 aeolus-0.4.8/src/aeolus/calc/diag.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     3595 2021-01-25 21:35:53.000000 aeolus-0.4.8/src/aeolus/calc/flux_h.py
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     3401 2021-01-25 21:27:45.000000 aeolus-0.4.8/src/aeolus/calc/meta.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     3115 2019-12-03 15:30:30.000000 aeolus-0.4.8/src/aeolus/calc/metpy.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     7889 2021-01-25 21:35:30.000000 aeolus-0.4.8/src/aeolus/calc/stats.py
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     3952 2020-12-03 20:29:28.000000 aeolus-0.4.8/src/aeolus/calc/tl.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.744510 aeolus-0.4.8/src/aeolus/const/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      161 2019-12-16 13:33:34.000000 aeolus-0.4.8/src/aeolus/const/__init__.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     5350 2020-05-18 10:52:37.000000 aeolus-0.4.8/src/aeolus/const/const.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.744510 aeolus-0.4.8/src/aeolus/const/store/
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1283 2020-05-19 20:47:52.000000 aeolus-0.4.8/src/aeolus/const/store/earth.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)      738 2020-09-09 19:58:06.000000 aeolus-0.4.8/src/aeolus/const/store/general.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1157 2020-05-01 06:22:57.000000 aeolus-0.4.8/src/aeolus/const/store/proxb.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1297 2020-05-18 10:58:39.000000 aeolus-0.4.8/src/aeolus/const/store/titan.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)      935 2020-01-06 13:38:56.000000 aeolus-0.4.8/src/aeolus/const/store/trap1d.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1158 2020-05-01 06:22:59.000000 aeolus-0.4.8/src/aeolus/const/store/trap1e.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)      934 2020-01-06 13:38:56.000000 aeolus-0.4.8/src/aeolus/const/store/trap1f.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)    32764 2021-01-25 21:37:45.000000 aeolus-0.4.8/src/aeolus/coord.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)    11775 2021-01-25 21:32:17.000000 aeolus-0.4.8/src/aeolus/core.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1294 2020-12-03 12:39:36.000000 aeolus-0.4.8/src/aeolus/exceptions.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1157 2020-09-28 16:48:41.000000 aeolus-0.4.8/src/aeolus/io.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.748510 aeolus-0.4.8/src/aeolus/model/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      128 2020-06-08 16:28:18.000000 aeolus-0.4.8/src/aeolus/model/__init__.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     2444 2020-09-30 15:52:59.000000 aeolus-0.4.8/src/aeolus/model/base.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     5733 2020-09-30 15:59:09.000000 aeolus-0.4.8/src/aeolus/model/um.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.748510 aeolus-0.4.8/src/aeolus/plot/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      503 2020-04-28 10:22:32.000000 aeolus-0.4.8/src/aeolus/plot/__init__.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     3505 2020-04-28 10:22:50.000000 aeolus-0.4.8/src/aeolus/plot/cart.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     5517 2021-01-25 21:37:58.000000 aeolus-0.4.8/src/aeolus/plot/cloud.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)    10102 2019-10-29 12:07:06.000000 aeolus-0.4.8/src/aeolus/plot/cm_custom.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1584 2020-03-31 22:41:52.000000 aeolus-0.4.8/src/aeolus/plot/mpl.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     4703 2020-10-26 15:46:11.000000 aeolus-0.4.8/src/aeolus/plot/pv.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1455 2019-10-29 12:08:29.000000 aeolus-0.4.8/src/aeolus/plot/text.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     6644 2020-07-02 14:12:26.000000 aeolus-0.4.8/src/aeolus/region.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     4127 2020-11-27 11:38:55.000000 aeolus-0.4.8/src/aeolus/subset.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.744510 aeolus-0.4.8/src/aeolus.egg-info/
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     2506 2021-01-25 21:49:48.000000 aeolus-0.4.8/src/aeolus.egg-info/PKG-INFO
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     1783 2021-01-25 21:49:48.000000 aeolus-0.4.8/src/aeolus.egg-info/SOURCES.txt
--rw-rw-r--   0 ds591     (1000) ds591     (1000)        1 2021-01-25 21:49:48.000000 aeolus-0.4.8/src/aeolus.egg-info/dependency_links.txt
--rw-rw-r--   0 ds591     (1000) ds591     (1000)        1 2021-01-25 21:49:48.000000 aeolus-0.4.8/src/aeolus.egg-info/not-zip-safe
--rw-rw-r--   0 ds591     (1000) ds591     (1000)       87 2021-01-25 21:49:48.000000 aeolus-0.4.8/src/aeolus.egg-info/requires.txt
--rw-rw-r--   0 ds591     (1000) ds591     (1000)        7 2021-01-25 21:49:48.000000 aeolus-0.4.8/src/aeolus.egg-info/top_level.txt
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.748510 aeolus-0.4.8/tests/
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-01-25 21:49:48.748510 aeolus-0.4.8/tests/data/
--rw-r--r--   0 ds591     (1000) ds591     (1000)       94 2019-11-04 10:21:23.000000 aeolus-0.4.8/tests/data/dummy.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1278 2020-08-28 21:13:15.000000 aeolus-0.4.8/tests/test_calc.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     2261 2019-11-04 12:32:32.000000 aeolus-0.4.8/tests/test_const.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1062 2020-04-28 10:44:10.000000 aeolus-0.4.8/tests/test_coord.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)      551 2019-11-21 10:24:28.000000 aeolus-0.4.8/tests/test_core.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)    68611 2019-02-28 18:05:47.000000 aeolus-0.4.8/versioneer.py
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.147147 aeolus-0.4.9/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     7652 2019-02-28 17:46:52.000000 aeolus-0.4.9/LICENSE
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      209 2020-10-13 09:19:31.000000 aeolus-0.4.9/MANIFEST.in
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)     2506 2021-04-12 13:13:39.147147 aeolus-0.4.9/PKG-INFO
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)     1164 2020-11-26 21:30:51.000000 aeolus-0.4.9/README.md
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.135147 aeolus-0.4.9/docs/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      605 2020-12-17 13:52:16.000000 aeolus-0.4.9/docs/Makefile
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      235 2021-04-12 11:12:49.000000 aeolus-0.4.9/docs/environment.yml
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.135147 aeolus-0.4.9/docs/source/
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.135147 aeolus-0.4.9/docs/source/_static/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     4286 2020-01-03 17:53:42.000000 aeolus-0.4.9/docs/source/_static/favicon.ico
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.139147 aeolus-0.4.9/docs/source/api/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     2222 2021-03-25 11:26:46.000000 aeolus-0.4.9/docs/source/api/calc.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      176 2020-01-02 13:49:09.000000 aeolus-0.4.9/docs/source/api/const.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1371 2020-12-03 19:56:03.000000 aeolus-0.4.9/docs/source/api/coord.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      147 2020-12-03 22:55:06.000000 aeolus-0.4.9/docs/source/api/core.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      558 2020-06-08 17:01:40.000000 aeolus-0.4.9/docs/source/api/index.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      123 2020-09-28 16:49:30.000000 aeolus-0.4.9/docs/source/api/io.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      191 2020-06-08 17:03:16.000000 aeolus-0.4.9/docs/source/api/model.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      415 2020-03-31 22:43:42.000000 aeolus-0.4.9/docs/source/api/plot.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)       53 2019-03-28 16:39:59.000000 aeolus-0.4.9/docs/source/api/region.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      301 2020-11-27 11:29:06.000000 aeolus-0.4.9/docs/source/api/subset.rst
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)     5179 2021-04-12 11:13:41.000000 aeolus-0.4.9/docs/source/changelog.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     7287 2021-01-26 09:58:23.000000 aeolus-0.4.9/docs/source/conf.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      154 2019-02-28 18:01:29.000000 aeolus-0.4.9/docs/source/contributing.rst
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.139147 aeolus-0.4.9/docs/source/examples/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      305 2019-02-28 18:16:56.000000 aeolus-0.4.9/docs/source/examples/_index_header_rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      726 2020-05-03 14:58:16.000000 aeolus-0.4.9/docs/source/index.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     2604 2020-11-25 15:56:20.000000 aeolus-0.4.9/docs/source/install.rst
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      714 2020-11-26 17:54:26.000000 aeolus-0.4.9/pyproject.toml
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)     1936 2021-04-12 13:13:39.147147 aeolus-0.4.9/setup.cfg
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      221 2020-10-13 09:13:58.000000 aeolus-0.4.9/setup.py
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.135147 aeolus-0.4.9/src/
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.147147 aeolus-0.4.9/src/aeolus/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      115 2019-02-28 18:19:47.000000 aeolus-0.4.9/src/aeolus/__init__.py
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)      497 2021-04-12 13:13:39.147147 aeolus-0.4.9/src/aeolus/_version.py
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.143147 aeolus-0.4.9/src/aeolus/calc/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     2188 2021-03-25 11:24:42.000000 aeolus-0.4.9/src/aeolus/calc/__init__.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     5359 2020-12-03 22:34:03.000000 aeolus-0.4.9/src/aeolus/calc/calculus.py
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)    27230 2021-03-29 11:18:53.000000 aeolus-0.4.9/src/aeolus/calc/diag.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     3509 2021-04-01 15:23:03.000000 aeolus-0.4.9/src/aeolus/calc/flux_h.py
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)     3618 2021-02-25 16:36:06.000000 aeolus-0.4.9/src/aeolus/calc/meta.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     3115 2019-12-03 15:30:30.000000 aeolus-0.4.9/src/aeolus/calc/metpy.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     9722 2021-04-01 15:36:37.000000 aeolus-0.4.9/src/aeolus/calc/stats.py
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)     3952 2020-12-03 20:29:28.000000 aeolus-0.4.9/src/aeolus/calc/tl.py
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.143147 aeolus-0.4.9/src/aeolus/const/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      215 2021-02-23 09:32:46.000000 aeolus-0.4.9/src/aeolus/const/__init__.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     6676 2021-04-01 15:37:01.000000 aeolus-0.4.9/src/aeolus/const/const.py
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.143147 aeolus-0.4.9/src/aeolus/const/store/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1283 2020-05-19 20:47:52.000000 aeolus-0.4.9/src/aeolus/const/store/earth.json
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      738 2020-09-09 19:58:06.000000 aeolus-0.4.9/src/aeolus/const/store/general.json
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1157 2020-05-01 06:22:57.000000 aeolus-0.4.9/src/aeolus/const/store/proxb.json
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1297 2020-05-18 10:58:39.000000 aeolus-0.4.9/src/aeolus/const/store/titan.json
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      935 2020-01-06 13:38:56.000000 aeolus-0.4.9/src/aeolus/const/store/trap1d.json
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1158 2020-05-01 06:22:59.000000 aeolus-0.4.9/src/aeolus/const/store/trap1e.json
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      934 2020-01-06 13:38:56.000000 aeolus-0.4.9/src/aeolus/const/store/trap1f.json
+-rw-r--r--   0 ds591     (1000) ds591     (1000)    32903 2021-04-01 15:37:45.000000 aeolus-0.4.9/src/aeolus/coord.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)    13489 2021-04-12 10:51:39.000000 aeolus-0.4.9/src/aeolus/core.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1410 2021-04-01 15:20:07.000000 aeolus-0.4.9/src/aeolus/exceptions.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     2535 2021-02-23 09:37:14.000000 aeolus-0.4.9/src/aeolus/io.py
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.143147 aeolus-0.4.9/src/aeolus/model/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      128 2020-06-08 16:28:18.000000 aeolus-0.4.9/src/aeolus/model/__init__.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     2545 2021-02-23 19:28:35.000000 aeolus-0.4.9/src/aeolus/model/base.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     5885 2021-02-23 19:28:14.000000 aeolus-0.4.9/src/aeolus/model/um.py
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.143147 aeolus-0.4.9/src/aeolus/plot/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      503 2020-04-28 10:22:32.000000 aeolus-0.4.9/src/aeolus/plot/__init__.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     3505 2020-04-28 10:22:50.000000 aeolus-0.4.9/src/aeolus/plot/cart.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     5517 2021-01-25 21:37:58.000000 aeolus-0.4.9/src/aeolus/plot/cloud.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)    10102 2019-10-29 12:07:06.000000 aeolus-0.4.9/src/aeolus/plot/cm_custom.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1788 2021-04-01 15:16:34.000000 aeolus-0.4.9/src/aeolus/plot/mpl.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     4654 2021-04-01 15:20:58.000000 aeolus-0.4.9/src/aeolus/plot/pv.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1455 2019-10-29 12:08:29.000000 aeolus-0.4.9/src/aeolus/plot/text.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     6644 2020-07-02 14:12:26.000000 aeolus-0.4.9/src/aeolus/region.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     4144 2021-03-31 14:01:54.000000 aeolus-0.4.9/src/aeolus/subset.py
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.139147 aeolus-0.4.9/src/aeolus.egg-info/
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)     2506 2021-04-12 13:13:39.000000 aeolus-0.4.9/src/aeolus.egg-info/PKG-INFO
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)     1783 2021-04-12 13:13:39.000000 aeolus-0.4.9/src/aeolus.egg-info/SOURCES.txt
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)        1 2021-04-12 13:13:39.000000 aeolus-0.4.9/src/aeolus.egg-info/dependency_links.txt
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)        1 2021-01-25 21:49:48.000000 aeolus-0.4.9/src/aeolus.egg-info/not-zip-safe
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)      108 2021-04-12 13:13:39.000000 aeolus-0.4.9/src/aeolus.egg-info/requires.txt
+-rw-rw-r--   0 ds591     (1000) ds591     (1000)        7 2021-04-12 13:13:39.000000 aeolus-0.4.9/src/aeolus.egg-info/top_level.txt
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.147147 aeolus-0.4.9/tests/
+drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.147147 aeolus-0.4.9/tests/data/
+-rw-r--r--   0 ds591     (1000) ds591     (1000)       94 2019-11-04 10:21:23.000000 aeolus-0.4.9/tests/data/dummy.json
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1278 2020-08-28 21:13:15.000000 aeolus-0.4.9/tests/test_calc.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1893 2021-02-25 16:18:02.000000 aeolus-0.4.9/tests/test_const.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)     1980 2021-02-25 16:15:37.000000 aeolus-0.4.9/tests/test_coord.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)      551 2019-11-21 10:24:28.000000 aeolus-0.4.9/tests/test_core.py
+-rw-r--r--   0 ds591     (1000) ds591     (1000)    68611 2019-02-28 18:05:47.000000 aeolus-0.4.9/versioneer.py
```

### Comparing `aeolus-0.4.8/LICENSE` & `aeolus-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/PKG-INFO` & `aeolus-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeolus
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python library for object-oriented analysis of atmospheric model output.
 Home-page: https://github.com/exoclim/aeolus
 Author: Denis Sergeev
 Author-email: dennis.sergeev@gmail.com
 Maintainer: aeolus developers
 Maintainer-email: dennis.sergeev@gmail.com
 License: LGPL-3.0
```

### Comparing `aeolus-0.4.8/README.md` & `aeolus-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/docs/Makefile` & `aeolus-0.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/docs/source/_static/favicon.ico` & `aeolus-0.4.9/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/docs/source/api/calc.rst` & `aeolus-0.4.9/docs/source/api/calc.rst`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 .. autofunction:: aeolus.calc.d_dz
 .. autofunction:: aeolus.calc.deriv
 .. autofunction:: aeolus.calc.div_h
 .. autofunction:: aeolus.calc.integrate
 
 Statistics
 ----------
+.. autofunction:: aeolus.calc.abs_coord_mean
 .. autofunction:: aeolus.calc.cumsum
 .. autofunction:: aeolus.calc.last_n_day_mean
 .. autofunction:: aeolus.calc.meridional_mean
 .. autofunction:: aeolus.calc.minmaxdiff
 .. autofunction:: aeolus.calc.normalize_cube
 .. autofunction:: aeolus.calc.region_mean_diff
 .. autofunction:: aeolus.calc.spatial
@@ -33,23 +34,25 @@
 .. autofunction:: aeolus.calc.bond_albedo
 .. autofunction:: aeolus.calc.dry_lapse_rate
 .. autofunction:: aeolus.calc.flux
 .. autofunction:: aeolus.calc.geopotential_height
 .. autofunction:: aeolus.calc.ghe_norm
 .. autofunction:: aeolus.calc.heat_redist_eff
 .. autofunction:: aeolus.calc.horiz_wind_cmpnts
+.. autofunction:: aeolus.calc.meridional_mass_streamfunction
 .. autofunction:: aeolus.calc.precip_sum
 .. autofunction:: aeolus.calc.sfc_net_energy
 .. autofunction:: aeolus.calc.sfc_water_balance
 .. autofunction:: aeolus.calc.superrotation_index
 .. autofunction:: aeolus.calc.toa_cloud_radiative_effect
 .. autofunction:: aeolus.calc.toa_eff_temp
 .. autofunction:: aeolus.calc.toa_net_energy
 .. autofunction:: aeolus.calc.water_path
 .. autofunction:: aeolus.calc.wind_speed
+.. autofunction:: aeolus.calc.zonal_mass_streamfunction
 
 Horizontal fluxes
 -----------------
 .. autofunction:: aeolus.calc.net_horizontal_flux_to_region 
 
 Tidally-locked coordinates
 --------------------------
```

### Comparing `aeolus-0.4.8/docs/source/api/coord.rst` & `aeolus-0.4.9/docs/source/api/coord.rst`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/docs/source/api/index.rst` & `aeolus-0.4.9/docs/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/docs/source/changelog.rst` & `aeolus-0.4.9/docs/source/changelog.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,39 @@
 Changelog
 =========
 
 .. default-role:: py:obj
 
+0.4.9
+-----
+
+:Date: 12 April 2021
+
+* Add cached-property as a dependency
+* Rename `AtmosFlow` to `AtmoSim` and create a base class `AtmoSimBase`
+* Add `extract()` method to `AtmoSimBase`
+* Add pressure coordinate to `DimConstr`
+* Refactor `Run` and prepare for its deprecation
+* Add `load_data()` to `io`
+* Move `add_planet_conf_to_cubes()` to the `const` module
+* Deprecate `ScalarCube`
+* Add new variable names to `um`
+* Refactor derived constants and add `planet_rotation_rate` to the recipes
+* Add an option not to broadcast the coordinate to the cube's shape in `coord_to_cube()`
+* Make `spatial()`, `time_mean()` and `vertical_mean()` return the input cube in case of `CoordinateCollapseError`
+* Add `abs_coord_mean()` to average data over latitudes symmetric around the equator
+* Add functions to calculate meridional and zonal streamfunctions
+* Improve docstrings
+* Add an example notebook for working with model names
+
+
 0.4.8
 -----
 
-:Date: TBA
+:Date: 25 January 2021
 
 * Adapt to iris v3.0
 * Add new meta decorators
 * Fix typos
 
 
 0.4.7
```

### Comparing `aeolus-0.4.8/docs/source/conf.py` & `aeolus-0.4.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import aeolus
 
 
 # -- Project information -----------------------------------------------------
 
 project = "aeolus"
-copyright = "2020, the aeolus developers"  # noqa
+copyright = "2021, the aeolus developers"  # noqa
 author = "The aeolus developers"
 
 # The short X.Y version
 version = aeolus.__version__
 # The full version, including alpha/beta/rc tags
 release = version
```

### Comparing `aeolus-0.4.8/docs/source/index.rst` & `aeolus-0.4.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/docs/source/install.rst` & `aeolus-0.4.9/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/pyproject.toml` & `aeolus-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/setup.cfg` & `aeolus-0.4.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -33,17 +33,18 @@
 zip_safe = False
 package_dir = 
 	= src
 packages = find:
 include_package_data = True
 python_requires = >=3.7
 install_requires = 
+	cached_property>=1.5.1
 	matplotlib>=3.0
 	numpy>=1.17.0
-	scitools-iris>=2.4.0
+	scitools-iris>=3.0
 	latlon23>=1.0.7
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 test = pytest>=3.3
```

### Comparing `aeolus-0.4.8/src/aeolus/calc/__init__.py` & `aeolus-0.4.9/src/aeolus/calc/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,26 +7,30 @@
     bond_albedo,
     dry_lapse_rate,
     flux,
     geopotential_height,
     ghe_norm,
     heat_redist_eff,
     horiz_wind_cmpnts,
+    meridional_mass_streamfunction,
     precip_sum,
     sfc_net_energy,
     sfc_water_balance,
+    sigma_p,
     superrotation_index,
     toa_cloud_radiative_effect,
     toa_eff_temp,
     toa_net_energy,
     water_path,
     wind_speed,
+    zonal_mass_streamfunction,
 )
 from .flux_h import horizontal_fluxes_through_region_boundaries, net_horizontal_flux_to_region
 from .stats import (
+    abs_coord_mean,
     cumsum,
     last_n_day_mean,
     meridional_mean,
     minmaxdiff,
     normalize_cube,
     region_mean_diff,
     spatial,
@@ -39,14 +43,15 @@
 from .tl import (
     regrid_to_rotated_pole_coordinates,
     regrid_to_tidally_locked_coordinates,
     rotate_winds_to_tidally_locked_coordinates,
 )
 
 __all__ = (
+    "abs_coord_mean",
     "air_density",
     "air_potential_temperature",
     "air_temperature",
     "bond_albedo",
     "cumsum",
     "d_dx",
     "d_dy",
@@ -58,32 +63,35 @@
     "geopotential_height",
     "ghe_norm",
     "heat_redist_eff",
     "horiz_wind_cmpnts",
     "horizontal_fluxes_through_region_boundaries",
     "integrate",
     "last_n_day_mean",
+    "meridional_mass_streamfunction",
     "meridional_mean",
     "minmaxdiff",
     "net_horizontal_flux_to_region",
     "normalize_cube",
     "precip_sum",
     "region_mean_diff",
     "region_mean_diff",
     "regrid_to_rotated_pole_coordinates",
     "regrid_to_tidally_locked_coordinates",
     "rotate_winds_to_tidally_locked_coordinates",
     "sfc_net_energy",
     "sfc_water_balance",
+    "sigma_p",
     "spatial",
     "spatial_mean",
     "spatial_quartiles",
     "superrotation_index",
     "time_mean",
     "toa_cloud_radiative_effect",
     "toa_eff_temp",
     "toa_net_energy",
     "vertical_mean",
     "water_path",
     "wind_speed",
+    "zonal_mass_streamfunction",
     "zonal_mean",
 )
```

### Comparing `aeolus-0.4.8/src/aeolus/calc/calculus.py` & `aeolus-0.4.9/src/aeolus/calc/calculus.py`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/calc/diag.py` & `aeolus-0.4.9/src/aeolus/calc/diag.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Some commonly used diagnostics in atmospheric science."""
 from cf_units import Unit
 
 from iris.analysis.calculus import _coord_cos
-from iris.analysis.maths import add, multiply
+from iris.analysis.maths import add, apply_ufunc, multiply
 from iris.exceptions import ConstraintMismatchError as ConMisErr
+from iris.util import reverse
 
 import numpy as np
 
 from .calculus import d_dz, integrate
 from .meta import const_from_attrs, update_metadata
-from .stats import spatial_mean
+from .stats import cumsum, spatial_mean, time_mean, zonal_mean
 from ..const import init_const
-from ..const.const import ScalarCube
 from ..coord import coord_to_cube, ensure_bounds, regrid_3d
 from ..exceptions import ArgumentError, MissingCubeError
 from ..model import um
 from ..subset import _dim_constr
 
 
 __all__ = (
@@ -25,36 +25,47 @@
     "bond_albedo",
     "dry_lapse_rate",
     "flux",
     "geopotential_height",
     "ghe_norm",
     "heat_redist_eff",
     "horiz_wind_cmpnts",
+    "meridional_mass_streamfunction",
     "precip_sum",
     "sfc_net_energy",
     "sfc_water_balance",
+    "sigma_p",
     "toa_cloud_radiative_effect",
     "toa_eff_temp",
     "toa_net_energy",
     "water_path",
     "wind_speed",
+    "zonal_mass_streamfunction",
 )
 
 
 def _precip_name_mapping(model=um):
     """Generate lists of variable names for `precip_sum()`."""
     return {
         "total": [model.ls_rain, model.ls_snow, model.cv_rain, model.cv_snow],
         "conv": [model.cv_rain, model.cv_snow],
         "stra": [model.ls_rain, model.ls_snow],
         "rain": [model.ls_rain, model.cv_rain],
         "snow": [model.ls_snow, model.cv_snow],
     }
 
 
+@update_metadata(name="cos_lat", units="1")
+def lat_cos(cube, model=um):
+    """Convert the latitude coordinate to a cube and apply cosine to it."""
+    lat_cube = coord_to_cube(cube, model.y, broadcast=False)
+    lat_cos_cube = apply_ufunc(np.cos, apply_ufunc(np.deg2rad, lat_cube))
+    return lat_cos_cube
+
+
 @update_metadata(units="K")
 def air_temperature(cubelist, const=None, model=um):
     """
     Get the real temperature from the given cube list.
 
     If not present, it is attempted to calculate it from other variables,
     Exner pressure or air pressure, and potential temperature.
@@ -84,15 +95,15 @@
 
         if len(cubelist.extract(model.exner)) == 1:
             exner = cubelist.extract_cube(model.exner)
         elif len(cubelist.extract(model.pres)) == 1:
             if const is None:
                 const = thta.attributes["planet_conf"]
             pres = cubelist.extract_cube(model.pres)
-            exner = (pres / const.reference_surface_pressure.asc) ** (
+            exner = (pres / const.reference_surface_pressure) ** (
                 const.dry_air_gas_constant / const.dry_air_spec_heat_press
             ).data
         else:
             raise MissingCubeError(f"Unable to get air temperature from {cubelist}")
         temp = thta * exner
         temp.rename(model.temp)
         return temp
@@ -131,15 +142,15 @@
 
         if len(cubelist.extract(model.exner)) == 1:
             exner = cubelist.extract_cube(model.exner)
         elif len(cubelist.extract(model.pres)) == 1:
             if const is None:
                 const = temp.attributes["planet_conf"]
             pres = cubelist.extract_cube(model.pres)
-            exner = (pres / const.reference_surface_pressure.asc) ** (
+            exner = (pres / const.reference_surface_pressure) ** (
                 const.dry_air_gas_constant / const.dry_air_spec_heat_press
             ).data
         else:
             raise MissingCubeError(f"Unable to get air potential temperature from {cubelist}")
         thta = temp / exner
         thta.rename(model.thta)
         thta.convert_units("K")
@@ -172,15 +183,15 @@
         return cubelist.extract_cube(model.dens)
     except ConMisErr:
         try:
             temp = cubelist.extract_cube(model.temp)
             pres = cubelist.extract_cube(model.pres)
             if const is None:
                 const = pres.attributes["planet_conf"]
-            rho = pres / (const.dry_air_gas_constant.asc * temp)
+            rho = pres / (const.dry_air_gas_constant * temp)
             rho.rename(model.dens)
             return rho
         except ConMisErr:
             _msg = f"Unable to get variables from\n{cubelist}\nto calculate air density"
             raise MissingCubeError(_msg)
 
 
@@ -209,15 +220,15 @@
     try:
         return cubelist.extract_cube(model.ghgt)
     except ConMisErr:
         try:
             cube_w_height = cubelist.extract(_dim_constr(model.z, strict=False))[0]
             if const is None:
                 const = cube_w_height.attributes["planet_conf"]
-            g_hgt = coord_to_cube(cube_w_height, model.z) * const.gravity.asc
+            g_hgt = coord_to_cube(cube_w_height, model.z) * const.gravity
             g_hgt.attributes = {k: v for k, v in cube_w_height.attributes.items() if k != "STASH"}
             ensure_bounds(g_hgt, [model.z])
             g_hgt.rename(model.ghgt)
             return g_hgt
         except ConMisErr:
             _msg = f"No cubes in \n{cubelist}\nwith {model.z} as a coordinate."
             raise MissingCubeError(_msg)
@@ -371,36 +382,36 @@
     Calculate domain-average precipitation minus evaporation.
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         Input list of cubes.
     const: aeolus.const.const.ConstContainer, optional
-        Must have a `ScalarCube` of `condensible_density` as an attribute.
+        Must have a scalar cube of `condensible_density` as an attribute.
         If not given, attempt is made to retrieve it from cube attributes.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     iris.cube.Cube
         Cube of total surface downward water flux (P-E).
     """
     try:
         evap = cubelist.extract_cube(model.sfc_evap)
     except ConMisErr:
         try:
             lhf = cubelist.extract_cube(model.sfc_lhf)
-            evap = lhf / const.condensible_heat_vaporization.asc
-            evap /= const.condensible_density.asc
+            evap = lhf / const.condensible_heat_vaporization
+            evap /= const.condensible_density
         except (KeyError, ConMisErr):
             raise MissingCubeError(f"Cannot retrieve evaporation from\n{cubelist}")
     try:
         precip = cubelist.extract_cube(model.ppn)
-        precip /= const.condensible_density.asc
+        precip /= const.condensible_density
     except ConMisErr:
         precip = precip_sum(cubelist, ptype="total", const=const, model=model)
     precip.convert_units("mm h-1")
     evap.convert_units("mm h-1")
     net = precip - evap
     return net
 
@@ -413,15 +424,15 @@
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         Input list of cubes.
     ptype: str, optional
         Precipitation type (total|stra|conv|rain|snow).
     const: aeolus.const.const.ConstContainer, optional
-        Must have a `ScalarCube` of `condensible_density` as an attribute.
+        Must have a scalar cube of `condensible_density` as an attribute.
         If not given, attempt to retrieve it from cube attributes.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     iris.cube.Cube
@@ -438,15 +449,15 @@
     precip = 0.0
     for varname in varnames:
         try:
             cube = cubelist.extract_cube(varname)
             precip += cube
         except ConMisErr:
             pass
-    precip /= const.condensible_density.asc
+    precip /= const.condensible_density
     precip.convert_units("mm day^-1")
     precip.rename(f"{ptype}_precip_rate")
     return precip
 
 
 @update_metadata(name="heat_redistribution_efficiency", units="1")
 def heat_redist_eff(cubelist, region_a, region_b, model=um):
@@ -494,47 +505,43 @@
     Returns
     -------
     iris.cube.Cube
         Cube of :math:`T_{eff}`.
     """
     toa_olr = cubelist.extract_cube(model.toa_olr)
     sbc = init_const().stefan_boltzmann
-    try:
-        t_eff = (toa_olr / sbc) ** 0.25
-    except ValueError:
-        t_eff = (toa_olr / sbc.asc) ** 0.25
+    t_eff = (toa_olr / sbc) ** 0.25
     return t_eff
 
 
 @update_metadata(name="normalised_greenhouse_effect_parameter", units="1")
 def ghe_norm(cubelist, model=um):
     r"""
     Normalised greenhouse effect parameter.
 
     .. math::
-        GHE = 1 - \left(\frac{T_{eff}}{T_{sfc}}\right)^{1/4}
+        GHE = 1 - \left(\frac{T_{eff}}{T_{sfc}}\right)^4
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         Input list of cubes.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     iris.cube.Cube
-        Cube of greenhouse effect parameter with collapsed spatial dimensions.
+        Cube of greenhouse effect parameter.
     """
-    t_sfc = spatial_mean(cubelist.extract_cube(um.t_sfc))
+    t_sfc = cubelist.extract_cube(model.t_sfc)
     t_eff = toa_eff_temp(cubelist, model=model)
-    one = t_eff.copy(data=np.ones(t_eff.shape))
-    one.units = "1"
-    gh_norm = one - (t_eff / t_sfc) ** 4
-    return gh_norm
+    out = (t_eff / t_sfc) ** 4
+    out = out.copy(data=1 - out.data)
+    return out
 
 
 @const_from_attrs
 @update_metadata(name="bond_albedo", units="1")
 def bond_albedo(cubelist, const=None, model=um):
     r"""
     Bold albedo.
@@ -543,30 +550,27 @@
         4 \frac{OSR_{TOA}}{S_{0}}
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         Input list of cubes.
     const: aeolus.const.const.ConstContainer, optional
-        Must have a `ScalarCube` of `condensible_density` as an attribute.
+        Must have a scalar cube of `solar_constant` as an attribute.
         If not given, attempt to retrieve it from cube attributes.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     iris.cube.Cube
         Cube of bond albedo.
     """
     toa_osr = cubelist.extract_cube(model.toa_osr)
     sc = const.solar_constant
-    try:
-        b_alb = 4 * toa_osr / sc
-    except ValueError:
-        b_alb = 4 * toa_osr / sc.asc
+    b_alb = 4 * toa_osr / sc
     return b_alb
 
 
 @update_metadata(units="kg m-2")
 def water_path(cubelist, kind="water_vapour", model=um):
     r"""
     Water vapour or condensate path, i.e. a vertical integral of a water phase.
@@ -664,14 +668,17 @@
 
         m = a cos\phi(\Omega a cos\phi + u)
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         List of cubes containing a cube of zonal velocity (u).
+    const: aeolus.const.const.ConstContainer, optional
+        Constainer with the relevant planetary constants.
+        If not given, attempt is made to retrieve it from cube attributes.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     s_idx: iris.cube.Cube
         Cubes of superrotation index.
@@ -682,16 +689,15 @@
     """
     # Zonal velocity
     u = cubelist.extract_cube(model.u)
     # Radius of the planet
     r = const.radius
     r.convert_units("m")
     # Rotation rate
-    omega = ScalarCube.from_cube((const.day / (2 * np.pi)) ** (-1))
-    omega.convert_units("s-1")
+    omega = const.planet_rotation_rate
 
     lat_coord = u.coord(model.y).copy()
     lat_dim = u.coord_dims(model.y)[0]
     lat_coord.convert_units("radians")
     lat_cos_coord = _coord_cos(lat_coord)
 
     # Calculate intermediate terms
@@ -701,15 +707,15 @@
     r_coslat.units = Unit("m")
     inner_sum = add(u, omega_r_coslat, dim=lat_dim)
 
     # Calculate axial component of specific absolute angular momentum
     ang_mom = multiply(inner_sum, r_coslat, dim=lat_dim)
 
     # Final index
-    s_idx = ang_mom / omega.asc / r.asc / r.asc
+    s_idx = ang_mom / omega / (r ** 2)
     s_idx.convert_units("1")
     s_idx = s_idx.copy(data=s_idx.data - 1)
     return s_idx
 
 
 @update_metadata(name="wind_speed", units="m s-1")
 def wind_speed(*components):
@@ -722,7 +728,145 @@
         Cubes of u, v, w wind components.
 
     .. math::
         \sqrt{u^2 + v^2 + w^2}
     """
     out = sum(cube ** 2 for cube in components) ** 0.5
     return out
+
+
+@const_from_attrs
+@update_metadata(name="atmosphere_hybrid_sigma_pressure_coordinate", units="1")
+def sigma_p(cubelist, const=None, model=um):
+    r"""
+    Calculate sigma (normalised pressure coordinate) from a cube of pressure.
+
+    .. math::
+        \sigma = p / p_{sfc}
+
+    Parameters
+    ----------
+    cubelist: iris.cube.CubeList
+        Input list of cubes.
+    const: aeolus.const.const.ConstContainer, optional
+        Must have a cube of reference (surface) pressure as an attribute.
+        If not given, attempt to retrieve it from cube attributes.
+    model: aeolus.model.Model, optional
+        Model class with relevant variable names.
+    """
+    pres_cube = time_mean(spatial_mean(cubelist.extract_cube(model.pres)))
+    pres_cube.convert_units("Pa")
+    return pres_cube / const.reference_surface_pressure
+
+
+@const_from_attrs
+@update_metadata(name="zonal_mass_streamfunction", units="kg s^-1")
+def zonal_mass_streamfunction(cubelist, const=None, model=um):
+    r"""
+    Calculate mean zonal mass streamfunction.
+
+    .. math::
+        \Psi_Z = 2\pi a \int_{z_{sfc}}^{z_{top}}\overline{\rho}^* \overline{u}^* dz
+
+    References
+    ----------
+    Haqq-Misra & Kopparapu (2015), eq. 5;
+    Hartmann (1994), Global Physical Climatology, eq. 6.21
+
+    Examples
+    --------
+    >>> lat_band_constr = iris.Constraint(
+        latitude=lambda x: -30 <= x.point <= 30, longitude=lambda x: True
+    )
+    >>> mzsf = zonal_mass_streamfunction(cubes.extract(lat_band_constr))
+    """
+    streamf_const = 2 * np.pi * const.radius
+
+    u = cubelist.extract_cube(model.u)
+    u_tm = time_mean(u, model=model)
+    u = -1 * (u_tm - zonal_mean(u_tm, model=model))
+
+    if u.coord(axis="z").units.is_convertible("m"):
+        rho = cubelist.extract_cube(model.dens).copy()
+        rho = time_mean(rho, model=model)
+        rho.coord(model.z).bounds = None
+        u.coord(model.z).bounds = None
+        integrand = u * rho
+        # integrand = reverse(integrand, model.z)
+        # print(integrand.coord(um.z))
+        res = cumsum(integrand, "z", axis_weights=True, model=model)
+        # res = cumsum(integrand, "z", axis_weights=True, model=model)
+        # res = reverse(res, model.z)
+
+    elif u.coord(axis="z").units.is_convertible("Pa"):
+        integrand = u
+        res = cumsum(integrand, "z", axis_weights=True, model=model)
+        res /= const.gravity
+
+    res *= streamf_const
+    return res
+
+
+@const_from_attrs
+@update_metadata(name="meridional_mass_streamfunction", units="kg s^-1")
+def meridional_mass_streamfunction(cubelist, const=None, model=um):
+    r"""
+    Calculate the mean meridional mass streamfunction.
+
+    * In height coordinates
+
+    .. math::
+        \Psi_M = - 2\pi cos\phi a \int_{z_{sfc}}^{z_{top}}\overline{\rho v} dz
+
+    * In pressure coordinates
+
+    .. math::
+        \Psi_M = 2\pi cos\phi a \int_{0}^{p_{sfc}}\overline{\rho v} dp / g
+
+    Parameters
+    ----------
+    cubelist: iris.cube.CubeList
+        Input cubelist.
+    const: aeolus.const.const.ConstContainer, optional
+        If not given, constants are attempted to be retrieved from
+        attributes of a cube in the cube list.
+    model: aeolus.model.Model, optional
+        Model class with relevant variable names.
+
+    Returns
+    -------
+    iris.cube.Cube
+        Cube with collapsed spatial dimensions.
+
+    References
+    ----------
+    Haqq-Misra & Kopparapu (2015), eq. 4;
+    Vallis (2017)
+
+    Examples
+    --------
+    >>> from aeolus.calc import meridional_mass_streamfunction, time_mean
+    >>> from aeolus.const import init_const
+    >>> from aeolus.model import um
+    >>> earth_constants = init_const("earth")
+    >>> cubes = iris.cube.CubeList([time_mean(cube) for cube in input_cubes])
+    >>> mmsf = meridional_mass_streamfunction(cubes, const=earth_constants, model=um)
+    """
+    v = cubelist.extract_cube(model.v)
+    v = zonal_mean(v, model=model)
+    if v.coord(model.z).units.is_convertible("m"):
+        rho = zonal_mean(cubelist.extract_cube(model.dens), model=model)
+        rho.coord(model.z).bounds = None
+        v.coord(model.z).bounds = None
+        # Reverse the coordinate to start from the model top (where p=0 or z=z_top)
+        # TODO: check if the coordinate is ascending or descending
+        integrand = reverse(v * rho, model.z)
+        res = -1 * cumsum(integrand, "z", axis_weights=True, model=model)
+        # Reverse the result back
+        res = reverse(res, model.z)
+    elif v.coord(model.z).units.is_convertible("Pa"):
+        res = cumsum(v, "z", axis_weights=True, model=model)
+        res /= const.gravity
+    # Calculate the constant: 2 pi cos\phi a
+    streamf_const = 2 * np.pi * const.radius * lat_cos(res, model=model)
+    res *= streamf_const
+    return res
```

### Comparing `aeolus-0.4.8/src/aeolus/calc/flux_h.py` & `aeolus-0.4.9/src/aeolus/calc/flux_h.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # -*- coding: utf-8 -*-
 """Integrated fluxes."""
-import warnings
-
 import iris
 
 import numpy as np
 
 from ..const import get_planet_radius
 from ..coord import nearest_coord_value, vertical_cross_section_area
-from ..exceptions import AeolusWarning
+from ..exceptions import _warn
 from ..model import um
 
 
 __all__ = ("horizontal_fluxes_through_region_boundaries", "net_horizontal_flux_to_region")
 
 
 def horizontal_fluxes_through_region_boundaries(
@@ -28,18 +26,17 @@
 
     total_h_fluxes = iris.cube.CubeList()
     for bound in region:
         this_coord = bound["coord"]
         other_coord, (other_min, other_max) = region._perpendicular_side_limits(bound["name"])
         nearest = nearest_coord_value(scalar_cube, this_coord, bound["value"])
         if abs(nearest - bound["value"]) >= warn_thresh:
-            warnings.warn(
+            _warn(
                 f"Nearest value is {np.round(nearest - bound['value'], 2)} deg away"
                 f" from the given value of {this_coord}",
-                AeolusWarning,
             )
         vcross_cnstr = iris.Constraint(**{this_coord: nearest})
         vcross_cnstr &= vertical_constraint
 
         if other_max >= other_min:
             vcross_cnstr &= iris.Constraint(**{other_coord: lambda x: other_min <= x <= other_max})
             cube = scalar_cube.extract(vcross_cnstr)
@@ -73,17 +70,15 @@
         u,
         v,
         r_planet=r_planet,
         vertical_constraint=vertical_constraint,
         model=model,
     )
     net_flux = (
-        total_h_fluxes.extract_cube(
-            iris.Constraint(cube_func=lambda x: "through_west" in x.name())
-        )
+        total_h_fluxes.extract_cube(iris.Constraint(cube_func=lambda x: "through_west" in x.name()))
         - total_h_fluxes.extract_cube(
             iris.Constraint(cube_func=lambda x: "through_east" in x.name())
         )
         + total_h_fluxes.extract_cube(
             iris.Constraint(cube_func=lambda x: "through_south" in x.name())
         )
         - total_h_fluxes.extract_cube(
```

### Comparing `aeolus-0.4.8/src/aeolus/calc/meta.py` & `aeolus-0.4.9/src/aeolus/calc/meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,22 +78,30 @@
         cube_out.cell_methods = cell_methods
         return cube_out
 
     return wrapper
 
 
 def update_metadata(name=None, units=None, attrs=None):
-    """Update metadata of a cube returned by a function."""
+    """
+    Update metadata of a cube returned by a function.
+
+    If units are "unknown", the units are reset to the given units,
+    otherwise `convert_units()` is used.
+    """
 
     def _update(cube):
         """Update name, convert units and update attributes."""
         if isinstance(name, str):
             cube.rename(name)
         if isinstance(units, (str, cf_units.Unit)):
-            cube.convert_units(units)
+            if cube.units == "unknown":
+                cube.units = units
+            else:
+                cube.convert_units(units)
         if isinstance(attrs, dict):
             cube.attributes.update(attrs)
 
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             # Call the decorated function
```

### Comparing `aeolus-0.4.8/src/aeolus/calc/metpy.py` & `aeolus-0.4.9/src/aeolus/calc/metpy.py`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/calc/stats.py` & `aeolus-0.4.9/src/aeolus/calc/stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Statistical functions."""
-from warnings import warn
-
 import iris
+from iris.exceptions import CoordinateCollapseError as CoColErr
+from iris.exceptions import CoordinateNotFoundError as CoNotFound
 from iris.util import broadcast_to_shape
 
 import numpy as np
 
 from .calculus import integrate
-from ..coord import area_weights_cube, ensure_bounds
-from ..exceptions import AeolusWarning
+from ..coord import area_weights_cube, coord_to_cube, ensure_bounds
+from ..exceptions import ArgumentError, _warn
 from ..model import um
 from ..subset import extract_last_n_days
 
 
 __all__ = (
+    "abs_coord_mean",
     "cumsum",
     "last_n_day_mean",
     "meridional_mean",
     "minmaxdiff",
     "normalize_cube",
     "region_mean_diff",
     "spatial",
@@ -25,14 +26,51 @@
     "spatial_quartiles",
     "time_mean",
     "vertical_mean",
     "zonal_mean",
 )
 
 
+def abs_coord_mean(cube, coord):
+    """
+    Calculate cube's average over absolute values of a coordinate.
+
+    For example, applying this to a cube with N latitudes ranging
+    from SP to NP returns a cube with (N+1)//2 latitudes.
+
+    Parameters
+    ----------
+    cube: iris.cube.Cube
+        Cube with the specified coordinate.
+    coord: str or iris.coords.Coord
+        Coordinate to apply abs().
+
+    Returns
+    -------
+    iris.cube.Cube
+        Cube with a reduced dimension.
+    """
+    sign_lat = iris.analysis.maths.apply_ufunc(np.sign, coord_to_cube(cube, coord, broadcast=False))
+    sign_cube = sign_lat * cube
+    _coord = sign_cube.coord(coord)
+    _coord_dim = sign_cube.coord_dims(_coord)
+    abs_coord = iris.coords.AuxCoord.from_coord(_coord)
+    abs_coord.rename(f"abs_{abs_coord.name()}")
+    abs_coord.points = np.abs(_coord.points)
+    abs_coord.bounds = np.abs(_coord.bounds)
+    sign_cube.add_aux_coord(abs_coord, data_dims=_coord_dim)
+    out = sign_cube.aggregated_by(abs_coord, iris.analysis.MEAN)
+    out.remove_coord(_coord)
+    out.rename(cube.name())
+    out.units = cube.units
+    iris.util.promote_aux_coord_to_dim_coord(out, abs_coord.name())
+    out.coord(abs_coord).rename(_coord.name())
+    return out
+
+
 def cumsum(cube, axis, axis_weights=False, model=um):
     """
     Cumulative sum of a cube.
 
     Parameters
     ----------
     cube: iris.cube.Cube
@@ -47,15 +85,15 @@
     Returns
     -------
     iris.cube.Cube
         Cube of cumulative sums with the same dimensions as the input cube.
     """
     try:
         c = cube.coord(getattr(model, axis)).copy()
-    except (AttributeError, iris.exceptions.CoordinateNotFoundError):
+    except (AttributeError, CoNotFound):
         c = cube.coord(axis=axis).copy()
     dim = cube.coord_dims(c)
     if axis_weights:
         if not c.has_bounds():
             c.guess_bounds()
         weights = broadcast_to_shape(c.bounds[:, 1] - c.bounds[:, 0], cube.shape, dim)
         data = cube.data * weights
@@ -195,33 +233,45 @@
     coords = (model.y, model.x)
     flag = all(cube.coord(c).has_bounds() for c in coords)
     aggregator = getattr(iris.analysis, aggr.upper())
     if flag and isinstance(aggregator, iris.analysis.WeightedAggregator):
         kw = {"weights": area_weights_cube(cube, normalize=True).data}
     else:
         kw = {}
-    return cube.collapsed(coords, aggregator, **kw)
+    try:
+        out = cube.collapsed(coords, aggregator, **kw)
+    except CoColErr as e:
+        _warn(f"Caught exception in spatial():\n{e}")
+        # out = iris.util.squeeze(cube)
+        out = cube
+    return out
 
 
 def spatial_mean(cube, model=um):
     """Shortcut for spatial(cube, "mean")."""
     return spatial(cube, "mean", model=model)
 
 
 def spatial_quartiles(cube, model=um):
     """Calculate quartiles over horizontal coordinates."""
-    warn("No weights are applied!", AeolusWarning)
+    _warn("No weights are applied!")
     q25 = cube.collapsed((model.y, model.x), iris.analysis.PERCENTILE, percent=25)
     q75 = cube.collapsed((model.y, model.x), iris.analysis.PERCENTILE, percent=75)
     return q25, q75
 
 
 def time_mean(cube, model=um):
     """Time average of a cube."""
-    return cube.collapsed(model.t, iris.analysis.MEAN)
+    try:
+        out = cube.collapsed(model.t, iris.analysis.MEAN)
+    except CoColErr as e:
+        _warn(f"Caught exception in time_mean():\n{e}")
+        # out = iris.util.squeeze(cube)
+        out = cube
+    return out
 
 
 def vertical_mean(cube, weight_by=None, model=um):
     """
     Vertical mean of a cube with optional weighting.
 
     Parameters
@@ -235,14 +285,17 @@
 
     Returns
     -------
     iris.cube.Cube
         Collapsed cube.
     """
     coord = model.z
+    if len(cube.coord_dims(coord)) == 0:
+        _warn(f"The {repr(coord)} does not describe any dimension in {repr(cube)}.")
+        return cube
     if weight_by is None:
         vmean = cube.collapsed(coord, iris.analysis.MEAN)
     else:
         if isinstance(weight_by, (str, iris.coords.Coord)):
             weights = broadcast_to_shape(
                 cube.coord(weight_by).points.squeeze(), cube.shape, cube.coord_dims(weight_by)
             )
@@ -251,15 +304,15 @@
             a_copy = cube.copy()
             b_copy = weight_by.copy()
             a_copy.coord(coord).bounds = None
             b_copy.coord(coord).bounds = None
             prod = b_copy * a_copy
             vmean = integrate(prod, coord) / integrate(weight_by, coord)
         else:
-            raise ValueError(f"unrecognised type of weight_by: {type(weight_by)}")
+            raise ArgumentError(f"Unrecognised type of weight_by: {type(weight_by)}")
     vmean.rename(f"vertical_mean_of_{cube.name()}")
     return vmean
 
 
 def zonal_mean(cube, model=um):
     """
     Calculate cube's zonal average.
```

### Comparing `aeolus-0.4.8/src/aeolus/calc/tl.py` & `aeolus-0.4.9/src/aeolus/calc/tl.py`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/const/const.py` & `aeolus-0.4.9/src/aeolus/const/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,52 @@
 # -*- coding: utf-8 -*-
 """Main interface to the physical constants store."""
 import json
 from dataclasses import make_dataclass
 from pathlib import Path
-from warnings import warn
 
 import iris
 
 import numpy as np
 
-from ..exceptions import AeolusWarning, ArgumentError, LoadError
+from ..exceptions import ArgumentError, LoadError, _warn
 
 
-__all__ = ("init_const", "get_planet_radius")
+__all__ = ("add_planet_conf_to_cubes", "get_planet_radius", "init_const")
 
 CONST_DIR = Path(__file__).parent / "store"
 
+DERIVED_CONST = {
+    "dry_air_gas_constant": (
+        lambda slf: slf.molar_gas_constant / slf.dry_air_molecular_weight,
+        "J kg-1 K-1",
+    ),
+    "molecular_weight_ratio": (
+        lambda slf: slf.condensible_molecular_weight / slf.dry_air_molecular_weight,
+        "1",
+    ),
+    "poisson_exponent": (
+        lambda slf: slf.dry_air_gas_constant / slf.dry_air_spec_heat_press,
+        "1",
+    ),
+    "planet_rotation_rate": (lambda slf: (slf.day / (2 * np.pi)) ** (-1), "s-1"),
+}
+
 
 class ScalarCube(iris.cube.Cube):
     """Cube without coordinates."""
 
+    def __init__(self, *args, **kw):
+        """Initialise aeolus.const.const.ScalarCube."""
+        _warn(
+            "ScalarCube is deprecated and will be removed in the next release. "
+            "Use iris.cube.Cube instead.",
+        )
+        super(ScalarCube, self).__init__(*args, **kw)
+
     def __repr__(self):
         """Repr of this class."""
         return f"<ScalarCube of {self.long_name} [{self.units}]>"
 
     def __deepcopy__(self, memo):
         """Deep copy of a scalar cube."""
         return self.from_cube(self._deepcopy(memo))
@@ -59,31 +82,26 @@
         self._convert_to_iris_cubes()
         self._derive_const()
 
     def _convert_to_iris_cubes(self):
         """Loop through fields and convert each of them to `iris.cube.Cube`."""
         for name in self.__dataclass_fields__:
             _field = getattr(self, name)
-            cube = ScalarCube(
+            cube = iris.cube.Cube(
                 data=_field.get("value"), units=_field.get("units", 1), long_name=name
             )
             object.__setattr__(self, name, cube)
 
     def _derive_const(self):
         """Not fully implemented yet."""
-        derivatives = {
-            "dry_air_gas_constant": lambda slf: slf.molar_gas_constant
-            / slf.dry_air_molecular_weight,
-            "molecular_weight_ratio": lambda slf: slf.condensible_molecular_weight
-            / slf.dry_air_molecular_weight,
-            "poisson_exponent": lambda slf: slf.dry_air_gas_constant / slf.dry_air_spec_heat_press,
-        }
-        for name, func in derivatives.items():
+        for name, recipe in DERIVED_CONST.items():
+            func, units = recipe
             try:
-                cube = ScalarCube.from_cube(func(self))
+                cube = func(self)
+                cube.convert_units(units)
                 cube.rename(name)
                 object.__setattr__(self, name, cube)
             except AttributeError:
                 pass
 
 
 def _read_const_file(name, directory=CONST_DIR):
@@ -136,15 +154,19 @@
     else:
         kw = {"directory": directory}
     # transform the list of dictionaries into a dictionary
     const_dict = _read_const_file("general")  # TODO: make this more flexible?
     if name != "general":
         const_dict.update(_read_const_file(name, **kw))
     kls = make_dataclass(
-        cls_name, fields=[*const_dict.keys()], bases=(ConstContainer,), frozen=True, repr=False
+        cls_name,
+        fields=[*const_dict.keys()],
+        bases=(ConstContainer,),
+        frozen=True,
+        repr=False,
     )
     return kls(**const_dict)
 
 
 def get_planet_radius(cube, default=iris.fileformats.pp.EARTH_RADIUS):
     """Get planet radius in metres from cube attributes or coordinate system."""
     cs = cube.coord_system("CoordSystem")
@@ -152,10 +174,32 @@
         r = cs.semi_major_axis
     else:
         try:
             r = cube.attributes["planet_conf"].radius.copy()
             r.convert_units("m")
             r = float(r.data)
         except (KeyError, LoadError):
-            warn("Using default radius", AeolusWarning)
+            _warn("Using default radius")
             r = default
     return r
+
+
+def add_planet_conf_to_cubes(cubelist, const):
+    """
+    Add constants container to the cube attributes and replace its coordinate system.
+
+    Parameters
+    ----------
+    cubelist: iris.cube.CubeList
+        List of cubes containing a cube of zonal velocity (u).
+    const: aeolus.const.const.ConstContainer, optional
+        Constainer with the relevant planetary constants.
+    """
+    const.radius.convert_units("m")
+    _coord_system = iris.coord_systems.GeogCS(semi_major_axis=const.radius.data)
+    for cube in cubelist:
+        # add constants to cube attributes
+        cube.attributes["planet_conf"] = const
+        for coord in cube.coords():
+            if coord.coord_system:
+                # Replace coordinate system with the planet radius given in `self.const`
+                coord.coord_system = _coord_system
```

### Comparing `aeolus-0.4.8/src/aeolus/const/store/earth.json` & `aeolus-0.4.9/src/aeolus/const/store/earth.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/const/store/general.json` & `aeolus-0.4.9/src/aeolus/const/store/general.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/const/store/proxb.json` & `aeolus-0.4.9/src/aeolus/const/store/proxb.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/const/store/titan.json` & `aeolus-0.4.9/src/aeolus/const/store/titan.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/const/store/trap1d.json` & `aeolus-0.4.9/src/aeolus/const/store/trap1d.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/const/store/trap1e.json` & `aeolus-0.4.9/src/aeolus/const/store/trap1e.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/const/store/trap1f.json` & `aeolus-0.4.9/src/aeolus/const/store/trap1f.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/coord.py` & `aeolus-0.4.9/src/aeolus/coord.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 """Functionality related to coordinates of cubes."""
 from datetime import timedelta
-from warnings import warn
 
 from cartopy.util import add_cyclic_point
 
 import iris
 from iris.analysis.cartography import wrap_lons
 from iris.coord_categorisation import _months_in_season, add_categorised_coord
 from iris.exceptions import CoordinateNotFoundError as CoNotFound
 from iris.experimental import stratify
 from iris.util import broadcast_to_shape, guess_coord_axis, is_regular
 
 import numpy as np
 
 from .const import get_planet_radius
-from .exceptions import AeolusWarning, ArgumentError, BadCoordinateError, NotFoundError
+from .exceptions import ArgumentError, BadCoordinateError, NotFoundError, _warn
 from .model import um
 
 
 __all__ = (
     "CoordContainer",
     "add_binned_coord",
     "add_cyclic_point_to_cube",
@@ -80,15 +79,15 @@
     See Also
     --------
     aeolus.coord._cell_centres
     """
     assert points.ndim == 1, "Only 1D points are allowed"
     diffs = np.diff(points)
     if not np.allclose(diffs, diffs[0]):
-        warn("_cell_bounds() is supposed to work only for uniformly spaced points", AeolusWarning)
+        _warn("_cell_bounds() is supposed to work only for uniformly spaced points")
     delta = diffs[0] * bound_position
     bounds = np.concatenate([[points[0] - delta], points + delta])
     return bounds
 
 
 def _cell_centres(bounds, bound_position=0.5):
     """
@@ -472,49 +471,51 @@
         )
     else:
         new_cube = iris.cube.Cube(data=_data, units=units)
     new_cube.rename(f"{prefix}delta_{_coord.name()}")
     return new_cube
 
 
-def coord_to_cube(cube, coord):
+def coord_to_cube(cube, coord, broadcast=True):
     """
-    Convert coordinate points to a cube of the same dimension as the given cube.
+    Convert coordinate points to a cube with the same dimensions.
 
     Parameters
     ----------
     cube: iris.cube.Cube
         Cube containing the coordinate to be broadcast.
     coord: str or iris.coords.Coord
         Coordinate to be broadcast.
+    broadcast: bool, optional
+        Broadcast the coordinate points to the shape of the cube.
 
     Returns
     -------
     iris.cube.Cube
         Cube of broadcast coordinate.
     """
     if isinstance(coord, str):
         _coord = cube.coord(coord)
     else:
         _coord = coord
+    kw = {
+        "units": _coord.units,
+        "long_name": _coord.long_name,
+        "standard_name": _coord.standard_name,
+        "var_name": _coord.var_name,
+    }
     dim_map = cube.coord_dims(_coord.name())
     _data = _coord.points
-    if len(dim_map) > 0:
+    if len(dim_map) > 0 and broadcast:
         _data = broadcast_to_shape(_data, cube.shape, dim_map)
         dc = [(c.copy(), cube.coord_dims(c)) for c in cube.dim_coords]
         ac = [(c.copy(), cube.coord_dims(c)) for c in cube.aux_coords]
-        new_cube = iris.cube.Cube(
-            data=_data,
-            units=_coord.units,
-            long_name=_coord.name(),
-            dim_coords_and_dims=dc,
-            aux_coords_and_dims=ac,
-        )
+        new_cube = iris.cube.Cube(data=_data, dim_coords_and_dims=dc, aux_coords_and_dims=ac, **kw)
     else:
-        new_cube = iris.cube.Cube(data=_data, standard_name=_coord.name(), units=_coord.units)
+        new_cube = iris.cube.Cube(data=_data, dim_coords_and_dims=[(_coord.copy(), 0)], **kw)
     return new_cube
 
 
 def ensure_bounds(cube, coords=("x", "y"), model=um):
     """Auto-generate bounds for cube coordinates."""
     for coord in coords:
         try:
@@ -826,15 +827,15 @@
     coord = cube.coord(coord_name)
     i = coord.nearest_neighbour_index(val)
     return coord.points[i]
 
 
 def not_equal_coord_axes(cube1, cube2):
     """Given 2 cubes, return axes of unequal dimensional coordinates."""
-    coord_comp = iris.analysis.coord_comparison(cube1, cube2)
+    coord_comp = iris.analysis._dimensional_metadata_comparison(cube1, cube2)
     neq_dim_coords = set(coord_comp["not_equal"]).intersection(set(coord_comp["dimensioned"]))
     dims = []
     for coord_pair in neq_dim_coords:
         for coord in coord_pair:
             dims.append(iris.util.guess_coord_axis(coord))
     return set(filter(None, dims))
```

### Comparing `aeolus-0.4.8/src/aeolus/core.py` & `aeolus-0.4.9/src/aeolus/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Core submodule of aeolus package."""
-from pathlib import Path
-from warnings import warn
+from cached_property import cached_property
 
 import iris
 from iris.exceptions import ConstraintMismatchError as ConMisErr
 
 from .calc import diag
 from .calc.meta import copy_doc
-from .const import init_const
+from .const import add_planet_conf_to_cubes, init_const
 from .coord import CoordContainer
-from .exceptions import AeolusWarning, ArgumentError
+from .exceptions import _warn
+from .io import load_data, save_cubelist
 from .model import um
 from .region import Region
 from .subset import DimConstr
 
 __all__ = (
-    "AtmosFlow",
+    "AtmoSim",
+    "AtmoSimBase",
     "Run",
 )
 
 
-class AtmosFlow:
+class AtmoSimBase:
     """
-    Atmospheric Flow.
+    Base class for creating atmospheric model simulation classes in aeolus.
 
     Used to store and calculate atmospheric fields from gridded model output.
-    Derived quantities are stored as cached properties to save computational
-    time.
+    Derived quantities are stored as cached properties to save computational time.
 
-    Uses spherical coordinates.
+    Assumes the data are in spherical coordinates on a regular longitude-latitude grid.
 
     Attributes
     ----------
     name: str
         The run's name.
     description: str
         A description of the run.
@@ -48,38 +48,42 @@
         name="",
         description="",
         planet="",
         const_dir=None,
         model=um,
         model_type=None,
         timestep=None,
-        processed=False,
+        vert_coord=None,
     ):
         """
-        Instantiate an `AtmosFlow` object.
+        Instantiate an `AtmoSimBase` object.
 
         Parameters
         ----------
         cubes: iris.cube.CubeList
             Atmospheric fields.
         name: str, optional
-            The name of this `AtmosFlow`.
+            The name or label of this `AtmoSim`.
         description: str, optional
             This is not used internally; it is solely for the user's information.
         planet: str, optional
             Planet configuration. This is used to get appropriate physical constants.
             If not given, Earth physical constants are initialised.
         const_dir: pathlib.Path, optional
             Path to a folder with files containing constants for a specific planet.
         model: aeolus.model.Model, optional
             Model class with relevant coordinate and variable names.
         model_type: str, optional
             Type of the model run, global or LAM.
         timestep: int, optional
             Model time step in s.
+        vert_coord: str, optional
+            Character identificator for the type of the model's vertical coordinate.
+            "z" - data on "level_height"
+            "p" - data on pressure levels
 
         See also
         --------
         aeolus.const.init_const, aeolus.core.Run
         """
         self._cubes = cubes
         self.name = name
@@ -93,112 +97,191 @@
         self.model = model
         self.dim_constr = DimConstr(model=self.model)
 
         # If the model is global or LAM (nested) and what its driving model is
         self.model_type = model_type
         self.timestep = timestep
 
-        # Common coordinates
-        self.coord = CoordContainer(self._cubes)
+        # Domain
+        try:
+            cube_yx = self._cubes.extract(self.dim_constr.relax.yx)[0]
+            self.domain = Region.from_cube(cube_yx, name=f"{name}_domain", shift_lons=True)
+        except IndexError:
+            _warn("Initialised without a domain.")
 
         # Variables as attributes
-        self.assign_fields()
+        self._assign_fields()
+
+        # Common coordinates
+        dim_seq = ["tyx", "yx"]
+        self.vert_coord = vert_coord
+        # TODO: make it more flexible
+        if self.vert_coord == "z":
+            self.coord = CoordContainer(self._cubes.extract(self.dim_constr.relax.z))
+        elif self.vert_coord == "p":
+            self.coord = CoordContainer(self._cubes.extract(self.dim_constr.relax.p))
+        else:
+            self.coord = CoordContainer(self._cubes.extract(self.dim_constr.relax.yx))
+
+        if self.vert_coord is not None:
+            dim_seq += [f"t{self.vert_coord}yx", f"{self.vert_coord}yx"]
+        for seq in dim_seq:
+            try:
+                setattr(
+                    self,
+                    f"_ref_{seq}",
+                    self._cubes.extract(getattr(self.dim_constr.strict, seq))[0],
+                )
+            except IndexError:
+                pass
+
+    @classmethod
+    def from_parent_class(cls, obj):
+        """Dynamically inherit from a similar class."""
+        new_obj = cls(
+            cubes=obj._cubes,
+            name=obj.name,
+            description=obj.description,
+            planet=obj.planet,
+            const_dir=obj.const_dir,
+            model=obj.model,
+            model_type=obj.model_type,
+            timestep=obj.timestep,
+            vert_coord=obj.vert_coord,
+        )
+        return new_obj
 
     def __getitem__(self, key):
         """Redirect self[key] to self.key."""
         return self.__getattribute__(key)
 
     def _assign_fields(self):
         """Assign input cubelist items as attributes of this class."""
+        self.vars = []
         kwargs = {}
         for key in self.model.__dataclass_fields__:
             try:
                 kwargs[key] = self._cubes.extract_cube(getattr(self.model, key))
+                self.vars.append(key)
             except ConMisErr:
                 pass
         self.__dict__.update(**kwargs)
         del kwargs, key
 
     def _update_planet(self, planet="", const_dir=None):
         """Add or update planetary constants."""
         self.planet = planet
-        self.const = init_const(planet, directory=const_dir)
+        self.const_dir = const_dir
+        self.const = init_const(self.planet, directory=self.const_dir)
         try:
             self.const.radius.convert_units("m")
             self._coord_system = iris.coord_systems.GeogCS(semi_major_axis=self.const.radius.data)
         except AttributeError:
             self._coord_system = None
-            warn("Run initialised without a coordinate system.", AeolusWarning)
+            _warn("Run initialised without a coordinate system.")
 
     def _add_planet_conf_to_cubes(self):
-        """Add or update planetary constants container to cube attributes within `self.proc`."""
-        for cube in self._cubes:
-            # add constants to cube attributes
-            cube.attributes["planet_conf"] = self.const
-            for coord in cube.coords():
-                if coord.coord_system:
-                    # Replace coordinate system with the planet radius given in `self.const`
-                    coord.coord_system = self._coord_system
+        """Add or update planetary constants container to cube attributes."""
+        add_planet_conf_to_cubes(self._cubes, self.const)
+
+    def extract(self, constraints):
+        """
+        Subset `AtmoSim` using iris constraints.
+
+        Parameters
+        ----------
+        constraints: iris.Constraint or iterable of constraints
+            A single constraint or an iterable.
+        """
+        new_obj = self.__class__(
+            cubes=self._cubes.extract(constraints),
+            name=self.name,
+            description=self.description,
+            planet=self.planet,
+            const_dir=self.const_dir,
+            model=self.model,
+            model_type=self.model_type,
+            timestep=self.timestep,
+            vert_coord=self.vert_coord,
+        )
+        return new_obj
 
-    @property
+
+class AtmoSim(AtmoSimBase):
+    """
+    Main class for dealing with a atmospheric model simulation output in aeolus.
+
+    Used to store and calculate atmospheric fields from gridded model output.
+    Derived quantities are stored as cached properties to save computational time.
+    """
+
+    @cached_property
+    @copy_doc(diag.wind_speed)
+    def sigma_p(self):
+        # TODO: pass the cube only?
+        return diag.sigma_p(self._cubes, const=self.const, model=self.model)
+
+    @cached_property
     @copy_doc(diag.wind_speed)
     def wind_speed(self):
         cmpnts = []
         for cmpnt_key in ["u", "v", "w"]:
             try:
                 cmpnts.append(self[cmpnt_key])
             except AttributeError:
                 pass
         return diag.wind_speed(*cmpnts)
 
+    @cached_property
+    @copy_doc(diag.toa_net_energy)
+    def toa_net_energy(self):
+        return diag.toa_net_energy(self._cubes, model=self.model)
+
+    @cached_property
+    @copy_doc(diag.sfc_water_balance)
+    def sfc_water_balance(self):
+        return diag.sfc_water_balance(self._cubes, const=self.const, model=self.model)
+
 
 class Run:
     """
     A single model 'run', i.e. simulation.
 
     Attributes
     ----------
     name: str
         The run's name.
-    description: str
-        A description of the run.
     const: aeolus.const.ConstContainer
         Physical constants used in calculations for this run.
     model: aeolus.model.Model, optional
         Model class with relevant coordinate names.
     """
 
-    attr_keys = ["name", "description", "planet", "model_type", "timestep", "parent", "children"]
+    attr_keys = ["name", "planet", "model_type", "timestep"]
 
     def __init__(
         self,
         files=None,
         name="",
-        description="",
         planet="",
         const_dir=None,
         model=um,
         model_type=None,
         timestep=None,
-        parent=None,
-        children=None,
         processed=False,
     ):
         """
         Instantiate a `Run` object.
 
         Parameters
         ----------
         files: str or pathlib.Path, optional
             Wildcard for loading files.
         name: str, optional
             The run's name.
-        description: str, optional
-            A description of the model. This is not used internally by
-            aeolus; it is solely for the user's information.
         planet: str, optional
             Planet configuration. This is used to get appropriate physical constants.
             If not given, Earth physical constants are initialised.
         const_dir: pathlib.Path, optional
             Path to a folder with JSON files containing constants for a specific planet.
         model: aeolus.model.Model, optional
             Model class with relevant coordinate and variable names.
@@ -213,92 +296,81 @@
         processed: bool, optional
             If True, data from `files` is assigned to `proc` attribute.
 
         See also
         --------
         aeolus.const.init_const
         """
+        _warn(
+            "Run is deprecated and will be removed in the next release. "
+            "Use iris.cube.CubeList instead."
+        )
         self.name = name
-        self.description = description
 
         # Planetary constants
         self._update_planet(planet=planet, const_dir=const_dir)
 
         # Model-specific names of variables and coordinates
         self.model = model
         self.dim_constr = DimConstr(model=self.model)
 
         # If the model is global or LAM (nested) and what its driving model is
         self.model_type = model_type
         self.timestep = timestep
-        self.parent = parent
-        self.children = children
         self.processed = processed
 
         if files:
             self.load_data(files)
             try:
                 if self.processed:
                     cube_yx = self.proc.extract(self.dim_constr.relax.yx)[0]
                 else:
                     cube_yx = self.raw.extract(self.dim_constr.relax.yx)[0]
                 self.domain = Region.from_cube(cube_yx, name=f"{name}_domain", shift_lons=True)
             except IndexError:
-                warn("Run initialised without a domain.")
+                _warn("Run initialised without a domain.")
         else:
-            warn("Run initialised without input files")
+            _warn("Run initialised without input files")
 
     def load_data(self, files):
         """Load cubes."""
-        if isinstance(files, (list, set, tuple)):
-            fnames = [str(i) for i in files]
-        elif isinstance(files, (str, Path)):
-            fnames = str(files)
-        else:
-            raise ArgumentError(f"Input type {type(files)} is not allowed.")
         if self.processed:
-            self.proc = iris.load(fnames)
+            self.proc = load_data(files)
             self._add_planet_conf_to_cubes()
         else:
-            self.raw = iris.load(fnames)
+            self.raw = load_data(files)
 
     def _update_planet(self, planet="", const_dir=None):
         """Add or update planetary constants."""
         self.planet = planet
         self.const = init_const(planet, directory=const_dir)
         try:
             self.const.radius.convert_units("m")
             self._coord_system = iris.coord_systems.GeogCS(semi_major_axis=self.const.radius.data)
         except AttributeError:
             self._coord_system = None
-            warn("Run initialised without a coordinate system.", AeolusWarning)
+            _warn("Run initialised without a coordinate system.")
 
     def _add_planet_conf_to_cubes(self):
-        """Add or update planetary constants container to cube attributes within `self.proc`."""
-        for cube in self.proc:
-            # add constants to cube attributes
-            cube.attributes["planet_conf"] = self.const
-            for coord in cube.coords():
-                if coord.coord_system:
-                    # Replace coordinate system with the planet radius given in `self.const`
-                    coord.coord_system = self._coord_system
+        """Add or update planetary constants container to cube attributes."""
+        add_planet_conf_to_cubes(self._cubes, self.const)
 
     def proc_data(self, func=None, **func_args):
         """
         Post-process data for easier analysis and store it in `self.proc` attribute.
 
         Parameters
         ----------
         func: callable
             Function that takes `iris.cube.CubeList` as its first argument.
         **func_args: dict-like, optional
             Keyword arguments passed to `func`.
         """
         if self.processed:
-            warn("Run's data is already processed. Skipping.", AeolusWarning)
+            _warn("Run's data is already processed. Skipping.")
         else:
             self.proc = iris.cube.CubeList()
             if callable(func):
                 self.proc = func(self.raw, **func_args)
             self._add_planet_conf_to_cubes()
             self.processed = True
 
@@ -313,36 +385,21 @@
             and appends new cubes to it (and does not return anything).
         **func_args: dict-like, optional
             Keyword arguments passed to `func`.
         """
         if callable(func):
             func(self.proc, **func_args)
 
-    def to_netcdf(self, path):
+    def to_file(self, path):
         """
-        Save `proc` cubelist to a netCDF file with appropriate metadata.
+        Save `proc` cubelist to a file with appropriate metadata.
 
         Parameters
         ----------
         path: str or pathlib.Path
             File path.
         """
         run_attrs = {}
         for key in self.attr_keys:
             if getattr(self, key):
                 run_attrs[key] = str(getattr(self, key))
-        # Remove planet_conf attribute before saving
-        out = iris.cube.CubeList()
-        old_attrs = {}
-        for cube in self.proc:
-            old_attrs[cube.name()] = cube.attributes.copy()
-            new_attrs = {**cube.attributes, **run_attrs}
-            try:
-                new_attrs.pop("planet_conf")
-            except KeyError:
-                pass
-            cube.attributes = new_attrs
-            out.append(cube)
-        iris.save(out, str(path))
-        # Restore original attributes
-        for cube in self.proc:
-            cube.attributes = old_attrs[cube.name()]
+        save_cubelist(self.proc, path, **run_attrs)
```

### Comparing `aeolus-0.4.8/src/aeolus/exceptions.py` & `aeolus-0.4.9/src/aeolus/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # -*- coding: utf-8 -*-
 """Exceptions specific to aeolus package."""
+from warnings import warn
+
+
+def _warn(msg):
+    """Raise an aeolus-related warning."""
+    warn(msg, AeolusWarning)
 
 
 class AeolusWarning(UserWarning):
     """Base class for warnings in aeolus package."""
 
     pass
```

### Comparing `aeolus-0.4.8/src/aeolus/io.py` & `aeolus-0.4.9/src/aeolus/io.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 """Input and output functionality."""
-import f90nml
+from pathlib import Path
 
 import iris
 
 import numpy as np
 
+from .exceptions import ArgumentError
 
-__all__ = ("load_multidir", "load_vert_lev")
+
+__all__ = ("load_data", "load_multidir", "load_vert_lev", "save_cubelist")
+
+
+def load_data(files):
+    """Wrap `iris.load` to deal with `pathlib.Path` objects."""
+    if isinstance(files, (list, set, tuple)):
+        fnames = [str(i) for i in files]
+    elif isinstance(files, (str, Path)):
+        fnames = str(files)
+    else:
+        raise ArgumentError(f"Input type {type(files)} is not allowed.")
+    return iris.load(fnames)
 
 
 def load_multidir(path_mask, labels, label_name="run"):
     """Load cubelists from multiple directories and merge."""
     joint_cl = iris.cube.CubeList()
     for label in labels:
         cl = iris.load(str(path_mask).format(label))
@@ -33,11 +46,44 @@
         What levels to return: "theta" or "rho".
 
     Returns
     -------
     levs: numpy.array
         Array of height levels.
     """
-    with path_to_file as nml_file:
+    import f90nml  # noqa
+
+    with path_to_file.open("r") as nml_file:
         nml = f90nml.read(nml_file)
         levs = np.array(nml["vertlevs"][f"eta_{lev_type}"]) * nml["vertlevs"]["z_top_of_model"]
     return levs
+
+
+def save_cubelist(cubelist, path, **aux_attrs):
+    """
+    Save a cubelist w/o the `planet_conf` container to a file.
+
+    Parameters
+    ----------
+    cubelist: iris.cube.CubeList
+        Cube list to write to disk.
+    path: str or pathlib.Path
+        File path.
+    aux_attrs: dict, optional
+        Dictionary of additional attributes to save with the cubes.
+    """
+    # Remove planet_conf attribute before saving
+    out = iris.cube.CubeList()
+    old_attrs = []
+    for cube in cubelist:
+        old_attrs.append(cube.attributes.copy())
+        new_attrs = {**cube.attributes, **aux_attrs}
+        try:
+            new_attrs.pop("planet_conf")
+        except KeyError:
+            pass
+        cube.attributes = new_attrs
+        out.append(cube)
+    iris.save(out, str(path))
+    # Restore original attributes
+    for cube, attrs in zip(cubelist, old_attrs):
+        cube.attributes = attrs
```

### Comparing `aeolus-0.4.8/src/aeolus/model/base.py` & `aeolus-0.4.9/src/aeolus/model/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     # Coordinates
     t: str = None  # time
     fcst_ref: str = None  # forecast reference
     fcst_prd: str = None  # forecast period
     z: str = None  # height
     lev: str = None  # level number
     s: str = None  # sigma
+    d: str = None  # depth
+    p: str = None  # pressure level
     y: str = None  # latitude
     x: str = None  # longitude
     # Variables
     # Main
     u: str = None
     v: str = None
     w: str = None
@@ -89,12 +91,14 @@
     dq_sw: str = None
     dq_lw: str = None
     dq_lsppn: str = None
     dq_bl: str = None
     dq_cv: str = None
     dq_lscld: str = None
     dq_adv: str = None
+    # Soil
+    soil_moist: str = None
 
     def __repr__(self):
         """Override the repr method of the dataclass."""
         size = len([_ for _, v in self.__dataclass_fields__.items() if v.name is not None])
         return f"{self.__class__}({size} fields)"
```

### Comparing `aeolus-0.4.8/src/aeolus/model/um.py` & `aeolus-0.4.9/src/aeolus/model/um.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     # Coordinates
     t="time",
     fcst_ref="forecast_reference_time",
     fcst_prd="forecast_period",
     z="level_height",
     lev="model_level_number",
     s="sigma",
+    d="depth",
+    p="air_pressure",
     y="latitude",
     x="longitude",
     # Variables
     u="x_wind",
     v="y_wind",
     w="upward_air_velocity",
     pres="air_pressure",
@@ -78,24 +80,27 @@
     dq_sw="change_over_time_in_specific_humidity_due_to_shortwave_heating",
     dq_lw="change_over_time_in_specific_humidity_due_to_longwave_heating",
     dq_lsppn="change_over_time_in_specific_humidity_due_to_stratiform_precipitation",
     dq_bl="change_over_time_in_specific_humidity_due_to_boundary_layer_mixing",
     dq_cv="change_over_time_in_specific_humidity_due_to_convection",
     dq_lscld="m01s09i182",
     dq_adv="change_over_time_in_specific_humidity_due_to_advection",
+    soil_moist="moisture_content_of_soil_layer",
 )
 
 um_stash = Model(
     # Coordinates
     t="time",
     fcst_ref="forecast_reference_time",
     fcst_prd="forecast_period",
     z="level_height",
     lev="model_level_number",
     s="sigma",
+    d="depth",
+    p="air_pressure",
     y="latitude",
     x="longitude",
     # Variables
     u="m01s00i002",
     v="m01s00i003",
     w="m01s00i150",
     pres="m01s00i408",
@@ -155,8 +160,9 @@
     dq_sw="m01s01i182",
     dq_lw="m01s02i182",
     dq_lsppn="m01s04i182",
     dq_bl="m01s03i182",
     dq_cv="m01s05i182",
     dq_lscld="m01s09i182",
     dq_adv="m01s12i182",
+    soil_moist="m01s08i223",
 )
```

### Comparing `aeolus-0.4.8/src/aeolus/plot/cart.py` & `aeolus-0.4.9/src/aeolus/plot/cart.py`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/plot/cloud.py` & `aeolus-0.4.9/src/aeolus/plot/cloud.py`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/plot/cm_custom.py` & `aeolus-0.4.9/src/aeolus/plot/cm_custom.py`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/plot/mpl.py` & `aeolus-0.4.9/src/aeolus/plot/mpl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """Matplotlib-related utilities."""
 import matplotlib.colors as mcolors
 from matplotlib.lines import Line2D
 
 import numpy as np
 
+from ..exceptions import _warn
+
+
 __all__ = ("MidpointNormalize", "add_custom_legend")
 
 
 class MidpointNormalize(mcolors.Normalize):
     """Normalise data around a midpoint."""
 
     def __init__(self, vmin=None, vmax=None, midpoint=None, clip=False):  # noqa
+        _warn(
+            "MidpointNormalize is deprecated and will be removed in the next release. "
+            "Use matplotlib.colors.CenteredNorm instead."
+        )
         self.midpoint = midpoint
         mcolors.Normalize.__init__(self, vmin, vmax, clip)
 
     def __call__(self, value, clip=None):  # noqa
         # Ignoring masked values and all kinds of edge cases
         x, y = [self.vmin, self.midpoint, self.vmax], [0, 0.5, 1]
         return np.ma.masked_array(np.interp(value, x, y))
```

### Comparing `aeolus-0.4.8/src/aeolus/plot/pv.py` & `aeolus-0.4.9/src/aeolus/plot/pv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Prepare data in spherical coordinates for pyvista plotting."""
-from warnings import warn
-
 import numpy as np
 
 from pyvista import grid_from_sph_coords, transform_vectors_sph_to_cart
 
 from ..coord import _cell_bounds
-from ..exceptions import AeolusWarning
+from ..exceptions import _warn
 from ..model import um
 
 
 __all__ = ("grid_for_scalar_cube_sph", "grid_for_vector_cubes_sph")
 
 
 def grid_for_scalar_cube_sph(cube, z_scale=1, z_offset=0, grid=None, label="scalar3d", model=um):
@@ -48,15 +46,15 @@
             levels = np.array([0])
         levels = z_scale * levels + z_offset
 
         grid = grid_from_sph_coords(lons, lats, levels)
 
     # Add data arras to grid
     if label in grid.cell_arrays:
-        warn(f"Label '{label}' exists in {grid}", AeolusWarning)
+        _warn(f"Label '{label}' exists in {grid}")
     grid.cell_arrays[label] = np.array(cube.data).swapaxes(-2, -1).ravel("C")
     return grid
 
 
 def grid_for_vector_cubes_sph(
     u,
     v,
```

### Comparing `aeolus-0.4.8/src/aeolus/plot/text.py` & `aeolus-0.4.9/src/aeolus/plot/text.py`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/region.py` & `aeolus-0.4.9/src/aeolus/region.py`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/src/aeolus/subset.py` & `aeolus-0.4.9/src/aeolus/subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,35 +90,37 @@
 class DimConstr:
     """
     Container for strict or relaxed dimensional constraints.
 
     Examples
     --------
     Extract cubes that have y and x dimensional coordinates (among others):
+
     >>> dc = DimConstr()
     >>> cubelist.extract(dc.relax.yx)
 
     Extract cubes that only have model levels, y and x dimensions:
+
     >>> dc = DimConstr()
     >>> cubelist.extract(dc.strict.myx)
     """
 
     def __init__(self, model=um):
         """
         Initialise DimConstr.
 
         Parameters
         ----------
         model: aeolus.model.Model, optional
             Model class with relevant coordinate names.
         """
-        abbr_aliases = {"t": "t", "z": "z", "m": "lev", "y": "y", "x": "x"}
+        abbr_aliases = {"t": "t", "z": "z", "m": "lev", "p": "p", "y": "y", "x": "x"}
         for mode in ["strict", "relax"]:
             attrs = {}
-            for key in ("z", "m"):
+            for key in ("z", "m", "p"):
                 for n in range(1, 5):
                     for seq in combinations(["t", key, "y", "x"], n):
                         model_seq = [abbr_aliases[letter] for letter in seq]
                         attrs["".join(seq)] = _dim_constr(
                             *[getattr(model, i) for i in model_seq], strict=(mode == "strict")
                         )
             setattr(self, mode, _ModeDimConstr(**attrs))
```

### Comparing `aeolus-0.4.8/src/aeolus.egg-info/PKG-INFO` & `aeolus-0.4.9/src/aeolus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeolus
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python library for object-oriented analysis of atmospheric model output.
 Home-page: https://github.com/exoclim/aeolus
 Author: Denis Sergeev
 Author-email: dennis.sergeev@gmail.com
 Maintainer: aeolus developers
 Maintainer-email: dennis.sergeev@gmail.com
 License: LGPL-3.0
```

### Comparing `aeolus-0.4.8/src/aeolus.egg-info/SOURCES.txt` & `aeolus-0.4.9/src/aeolus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/tests/test_calc.py` & `aeolus-0.4.9/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/tests/test_const.py` & `aeolus-0.4.9/tests/test_const.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def test_init_const_general():
     """Test init_const function w/o arguments."""
     cnsts = const.init_const()
     assert str(cnsts).startswith("GeneralConstants")
     assert isinstance(cnsts, const.const.ConstContainer)
     for key in cnsts.__dataclass_fields__.keys():
         attr = getattr(cnsts, key)
-        assert isinstance(attr, const.const.ScalarCube)
+        assert isinstance(attr, iris.cube.Cube)
         assert attr.ndim == 0  # XXX could be relaxed
     key = "stefan_boltzmann"
     assert key in cnsts.__dataclass_fields__
     cube = getattr(cnsts, key)
     assert cube.units == "W m-2 K-4"
     npt.assert_allclose(cube.data, 5.670367e-08)
 
@@ -55,17 +55,7 @@
         assert isinstance(attr, iris.cube.Cube)
         assert attr.ndim == 0  # XXX could be relaxed
     key = "my_constant"
     assert key in cnsts.__dataclass_fields__
     cube = getattr(cnsts, key)
     assert cube.units == "m s-1"
     npt.assert_allclose(cube.data, 123)
-
-
-def test_scalarcube():
-    """Test ScalarCube."""
-    name = "physical_constant"
-    cube = iris.cube.Cube(data=-123.456, units="m", long_name=name)
-    scube = const.const.ScalarCube.from_cube(cube)
-    assert isinstance(scube.asc, iris.coords.AuxCoord)
-    npt.assert_allclose(scube.data, scube.asc.points.squeeze())
-    assert scube.asc.long_name == name
```

### Comparing `aeolus-0.4.8/tests/test_coord.py` & `aeolus-0.4.9/tests/test_coord.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Test coord submodule."""
 from aeolus import coord
 
+import iris
+
 import numpy as np
 import numpy.testing as npt
 
 
 def test_cell_centres():
     """Test cell_centres."""
     arr = np.array([-1, 0, 1, 2])
@@ -28,7 +30,30 @@
 
 
 def test__is_longitude_global():
     """Test _is_longitude_global."""
     assert coord._is_longitude_global(np.arange(0, 360, 2.5))
     assert coord._is_longitude_global(np.linspace(-180, 180, 10))
     assert not coord._is_longitude_global(np.arange(0, 180, 2.5))
+
+
+def test_coord_to_cube():
+    """Test coord_to_cube."""
+    xc = iris.coords.DimCoord([-1, 2, 3], units="m", standard_name="longitude")
+    yc = iris.coords.DimCoord([10, 30, 50, 70], units="m", standard_name="latitude")
+    zc = iris.coords.DimCoord([1000, 500], units="hPa", standard_name="air_pressure")
+    arr = np.arange(24).reshape((2, 4, 3))
+    cube = iris.cube.Cube(
+        data=arr,
+        dim_coords_and_dims=[i[::-1] for i in [*enumerate((zc, yc, xc))]],
+        standard_name="x_wind",
+        units="m/s",
+    )
+    cc_bc = coord.coord_to_cube(cube, "longitude")
+    assert cc_bc.ndim == 3
+    assert cc_bc.coord("latitude") == cube.coord("latitude")
+    cc = coord.coord_to_cube(cube, "longitude", broadcast=False)
+    assert cc.ndim == 1
+    assert cc.shape == xc.shape
+    assert cc.standard_name == "longitude"
+    assert cc.units == "m"
+    npt.assert_allclose(cc.data, xc.points)
```

### Comparing `aeolus-0.4.8/tests/test_core.py` & `aeolus-0.4.9/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.8/versioneer.py` & `aeolus-0.4.9/versioneer.py`

 * *Files identical despite different names*

