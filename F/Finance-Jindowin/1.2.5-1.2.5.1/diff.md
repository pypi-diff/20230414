# Comparing `tmp/Finance-Jindowin-1.2.5.tar.gz` & `tmp/Finance-Jindowin-1.2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Jindowin-1.2.5.tar", last modified: Mon Mar 27 12:04:34 2023, max compression
+gzip compressed data, was "dist/Finance-Jindowin-1.2.5.1.tar", last modified: Fri Apr 14 15:45:44 2023, max compression
```

## Comparing `Finance-Jindowin-1.2.5.tar` & `Finance-Jindowin-1.2.5.1.tar`

### file list

```diff
@@ -1,214 +1,213 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/Finance_Jindowin.egg-info/
--rw-r--r--   0 root         (0) root         (0)      166 2023-03-27 12:04:33.000000 Finance-Jindowin-1.2.5/Finance_Jindowin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5519 2023-03-27 12:04:33.000000 Finance-Jindowin-1.2.5/Finance_Jindowin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-03-27 12:04:33.000000 Finance-Jindowin-1.2.5/Finance_Jindowin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      243 2023-03-27 12:04:33.000000 Finance-Jindowin-1.2.5/Finance_Jindowin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-27 12:04:33.000000 Finance-Jindowin-1.2.5/Finance_Jindowin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-03-23 02:22:41.000000 Finance-Jindowin-1.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      166 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      416 2023-03-23 02:24:04.000000 Finance-Jindowin-1.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/
--rw-r--r--   0 root         (0) root         (0)     2921 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/
--rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/
--rw-r--r--   0 root         (0) root         (0)      101 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69155 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/db_factory.py
--rw-r--r--   0 root         (0) root         (0)     7326 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/kd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/kd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68482 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/kd/kd_engine.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/mg/
--rw-r--r--   0 root         (0) root         (0)      111 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/mg/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/mg/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/mg/kn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/mg/kn/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10552 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/mg/kn/kn_engine.py
--rw-r--r--   0 root         (0) root         (0)     6160 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/mg/mg_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/rf/
--rw-r--r--   0 root         (0) root         (0)     1209 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/rf/EVENT.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/rf/STOCK.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/rf/THEME.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/data/DataAPI/rf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/ExternalAPI/
--rw-r--r--   0 root         (0) root         (0)      191 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/data/ExternalAPI/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/data/ExternalAPI/datayes.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/data/ExternalAPI/ricequant.py
--rw-r--r--   0 root         (0) root         (0)      258 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/ExternalAPI/tushare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/
--rw-r--r--   0 root         (0) root         (0)      922 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/dummy.py
--rw-r--r--   0 root         (0) root         (0)      441 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/engine.py
--rw-r--r--   0 root         (0) root         (0)     7153 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/factors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/basic.py
--rw-r--r--   0 root         (0) root         (0)     3432 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/classify.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/factors.py
--rw-r--r--   0 root         (0) root         (0)     1775 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/index_market.py
--rw-r--r--   0 root         (0) root         (0)     1090 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/yields.py
--rw-r--r--   0 root         (0) root         (0)      733 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/index_component.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/index_market.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/__init__.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/factors.py
--rw-r--r--   0 root         (0) root         (0)     6640 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/industry.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/market_stock.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/pit.py
--rw-r--r--   0 root         (0) root         (0)    14724 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/risk_model.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/yields.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/universe.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/utilities.py
--rw-r--r--   0 root         (0) root         (0)     4888 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/yields.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)      134 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5/jdw/jdcw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5/jdw/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/kdutils/create_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/kdutils/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5/jdw/kdutils/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2403 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5/jdw/kdutils/data/mongodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/kdutils/division/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/kdutils/division/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/kdutils/division/decorator.py
--rw-r--r--   0 root         (0) root         (0)     4786 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/kdutils/division/export.py
--rw-r--r--   0 root         (0) root         (0)     7249 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5/jdw/kdutils/file_utils.py
--rw-r--r--   0 root         (0) root         (0)     5188 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5/jdw/kdutils/logger.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/kdutils/singleton.py
--rw-r--r--   0 root         (0) root         (0)      357 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5/jdw/kdutils/utils.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5/jdw/kdutils/warning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/
--rw-r--r--   0 root         (0) root         (0)      344 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/anode/
--rw-r--r--   0 root         (0) root         (0)      175 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/anode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10145 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/anode/axtell.py
--rw-r--r--   0 root         (0) root         (0)    13341 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/anode/conor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/deckard/
--rw-r--r--   0 root         (0) root         (0)       41 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/deckard/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/deckard/goslin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/
--rw-r--r--   0 root         (0) root         (0)     1754 2023-03-27 07:08:57.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/evolution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/evolution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20611 2023-03-27 03:26:05.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/evolution/base.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/evolution/futures.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/evolution/paramizer.py
--rw-r--r--   0 root         (0) root         (0)     2432 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/evolution/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/geneticist/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/geneticist/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11936 2023-03-27 03:00:31.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/geneticist/base.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/geneticist/futures.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/geneticist/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/mutation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/mutation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11224 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/mutation/base.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/mutation/futures.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/mutation/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:07.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/carnot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/carnot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15030 2023-03-27 06:29:45.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/carnot/base.py
--rw-r--r--   0 root         (0) root         (0)     1798 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/carnot/futures.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/carnot/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/dendall/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/dendall/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11683 2023-03-27 02:53:43.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/dendall/base.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/dendall/futures.py
--rw-r--r--   0 root         (0) root         (0)     5684 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/dendall/params.py
--rw-r--r--   0 root         (0) root         (0)     3415 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/dendall/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/futures/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/futures/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1862 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/futures/alpha.py
--rw-r--r--   0 root         (0) root         (0)    12715 2023-03-26 11:36:16.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/futures/daily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17309 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/base copy.py
--rw-r--r--   0 root         (0) root         (0)    11651 2023-03-27 09:16:53.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/base.py
--rw-r--r--   0 root         (0) root         (0)     1923 2023-03-27 09:05:33.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/futures.py
--rw-r--r--   0 root         (0) root         (0)    13919 2023-03-27 09:12:30.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/models.py
--rw-r--r--   0 root         (0) root         (0)     1875 2023-03-27 09:05:40.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/stock/
--rw-r--r--   0 root         (0) root         (0)       53 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/stock/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/stock/alpha.py
--rw-r--r--   0 root         (0) root         (0)    12004 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/stock/daily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/metrics/
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/metrics/base.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/metrics/futures.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/metrics/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/score/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9894 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/score/base.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/score/futures.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/score/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/
--rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/atl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/atl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/atl/engine.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/mg_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/ntn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/ntn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py
--rw-r--r--   0 root         (0) root         (0)     2952 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/operator_engine.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/irey/
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/irey/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8222 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/irey/kestle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/
--rw-r--r--   0 root         (0) root         (0)      116 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2240 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/base.py
--rw-r--r--   0 root         (0) root         (0)     5979 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/futures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/indicator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/indicator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2401 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/indicator/atr.py
--rw-r--r--   0 root         (0) root         (0)     3270 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/indicator/base.py
--rw-r--r--   0 root         (0) root         (0)     3435 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/indicator/date.py
--rw-r--r--   0 root         (0) root         (0)     3312 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/indicator/symbol_pd.py
--rw-r--r--   0 root         (0) root         (0)     4466 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5/jdw/mfc/lombard/stock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/neutron/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/neutron/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5540 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/neutron/analysis.py
--rw-r--r--   0 root         (0) root         (0)     6955 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/neutron/factory.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/neutron/strategy.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5/jdw/mfc/neutron/trader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/mfc/oss/
--rw-r--r--   0 root         (0) root         (0)       37 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5/jdw/mfc/oss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-03-23 02:23:09.000000 Finance-Jindowin-1.2.5/jdw/mfc/oss/aliyun.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/plot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/plot/STOCK/
--rw-r--r--   0 root         (0) root         (0)      212 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/STOCK/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/STOCK/detail.py
--rw-r--r--   0 root         (0) root         (0)     3793 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/STOCK/flow_money.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/STOCK/hkshshz.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/STOCK/sentiment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/jdw/plot/THEME/
--rw-r--r--   0 root         (0) root         (0)      369 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/THEME/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6599 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/THEME/brief.py
--rw-r--r--   0 root         (0) root         (0)     7396 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/THEME/detail.py
--rw-r--r--   0 root         (0) root         (0)     3836 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/THEME/flow_money.py
--rw-r--r--   0 root         (0) root         (0)     6347 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/THEME/hkshshz.py
--rw-r--r--   0 root         (0) root         (0)     7672 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/THEME/indicators.py
--rw-r--r--   0 root         (0) root         (0)     3123 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/THEME/returns.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/THEME/sentiment.py
--rw-r--r--   0 root         (0) root         (0)      612 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4200 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/returns.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5/jdw/plot/stock.py
--rw-r--r--   0 root         (0) root         (0)     6727 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5/jdw/to_pandas.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5/jdw/utils.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-27 12:04:15.000000 Finance-Jindowin-1.2.5/jdw/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/requirements/
--rw-r--r--   0 root         (0) root         (0)      242 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 12:04:34.000000 Finance-Jindowin-1.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2065 2023-03-23 02:22:41.000000 Finance-Jindowin-1.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      170 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5486 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-03-23 02:22:41.000000 Finance-Jindowin-1.2.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      170 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2023-03-23 02:24:04.000000 Finance-Jindowin-1.2.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/
+-rw-r--r--   0 root         (0) root         (0)      101 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69155 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/db_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2023-03-30 00:48:57.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/kd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/kd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68482 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/kd/kd_engine.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/kn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/kn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10552 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/kn/kn_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6160 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/mg_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/EVENT.py
+-rw-r--r--   0 root         (0) root         (0)      596 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/STOCK.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/THEME.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/ExternalAPI/
+-rw-r--r--   0 root         (0) root         (0)      191 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/data/ExternalAPI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/data/ExternalAPI/datayes.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/data/ExternalAPI/ricequant.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/ExternalAPI/tushare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/
+-rw-r--r--   0 root         (0) root         (0)      922 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/dummy.py
+-rw-r--r--   0 root         (0) root         (0)      441 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/engine.py
+-rw-r--r--   0 root         (0) root         (0)     8728 2023-04-02 00:54:37.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/factors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/basic.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/classify.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/factors.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/index_market.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/yields.py
+-rw-r--r--   0 root         (0) root         (0)      733 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/index_component.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/index_market.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/factors.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/industry.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/market_stock.py
+-rw-r--r--   0 root         (0) root         (0)    14724 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/risk_model.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-03-23 02:23:00.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/yields.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-03-23 02:23:01.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/universe.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     4888 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/yields.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      134 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/jdcw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/create_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/data/mongodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/division/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/division/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/division/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4786 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/division/export.py
+-rw-r--r--   0 root         (0) root         (0)     7249 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/file_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5188 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/logger.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/singleton.py
+-rw-r--r--   0 root         (0) root         (0)      357 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/utils.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/kdutils/warning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/anode/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/anode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10145 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/anode/axtell.py
+-rw-r--r--   0 root         (0) root         (0)    13341 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/anode/conor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/deckard/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/deckard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/deckard/goslin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-03-27 07:08:57.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20603 2023-04-06 15:20:32.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/base.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/futures.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/paramizer.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12110 2023-04-11 03:16:45.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/base.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/futures.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11224 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/base.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:05.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:07.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15382 2023-04-09 01:55:30.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/base.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-04-07 08:05:19.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-04-07 08:05:50.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11683 2023-03-27 02:53:43.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/base.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/futures.py
+-rw-r--r--   0 root         (0) root         (0)     5684 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/params.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/alpha.py
+-rw-r--r--   0 root         (0) root         (0)    12715 2023-03-26 11:36:16.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/daily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17309 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/base copy.py
+-rw-r--r--   0 root         (0) root         (0)    11936 2023-04-10 03:16:30.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/base.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-10 03:16:39.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/futures.py
+-rw-r--r--   0 root         (0) root         (0)    17300 2023-04-10 03:33:10.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/models.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-04-10 03:16:49.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/alpha.py
+-rw-r--r--   0 root         (0) root         (0)    12004 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/daily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/base.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9894 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/base.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/futures.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-03-23 02:23:06.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/
+-rw-r--r--   0 root         (0) root         (0)      120 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/atl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/atl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/atl/engine.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/mg_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/ntn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/ntn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/operator_engine.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/irey/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/irey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8222 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/irey/kestle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/
+-rw-r--r--   0 root         (0) root         (0)      116 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/base.py
+-rw-r--r--   0 root         (0) root         (0)     5979 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/futures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/atr.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/base.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/date.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/symbol_pd.py
+-rw-r--r--   0 root         (0) root         (0)     4466 2023-03-23 02:23:04.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/stock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     6955 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/factory.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/strategy.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-03-23 02:23:03.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/trader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/oss/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-03-23 02:23:08.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/oss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-03-23 02:23:09.000000 Finance-Jindowin-1.2.5.1/jdw/mfc/oss/aliyun.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/plot/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/detail.py
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/flow_money.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/hkshshz.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/sentiment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6599 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/brief.py
+-rw-r--r--   0 root         (0) root         (0)     7396 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/detail.py
+-rw-r--r--   0 root         (0) root         (0)     3836 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/flow_money.py
+-rw-r--r--   0 root         (0) root         (0)     6347 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/hkshshz.py
+-rw-r--r--   0 root         (0) root         (0)     7672 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/indicators.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/returns.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/THEME/sentiment.py
+-rw-r--r--   0 root         (0) root         (0)      612 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4200 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/returns.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-03-23 02:22:59.000000 Finance-Jindowin-1.2.5.1/jdw/plot/stock.py
+-rw-r--r--   0 root         (0) root         (0)     6727 2023-03-23 02:23:02.000000 Finance-Jindowin-1.2.5.1/jdw/to_pandas.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-03-23 02:22:58.000000 Finance-Jindowin-1.2.5.1/jdw/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-14 15:44:53.000000 Finance-Jindowin-1.2.5.1/jdw/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/requirements/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-03-27 02:16:13.000000 Finance-Jindowin-1.2.5.1/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 15:45:44.000000 Finance-Jindowin-1.2.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-03-23 02:22:41.000000 Finance-Jindowin-1.2.5.1/setup.py
```

### Comparing `Finance-Jindowin-1.2.5/Finance_Jindowin.egg-info/SOURCES.txt` & `Finance-Jindowin-1.2.5.1/Finance_Jindowin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 jdw/data/SurfaceAPI/futures/factors.py
 jdw/data/SurfaceAPI/futures/index_market.py
 jdw/data/SurfaceAPI/futures/yields.py
 jdw/data/SurfaceAPI/stock/__init__.py
 jdw/data/SurfaceAPI/stock/factors.py
 jdw/data/SurfaceAPI/stock/industry.py
 jdw/data/SurfaceAPI/stock/market_stock.py
-jdw/data/SurfaceAPI/stock/pit.py
 jdw/data/SurfaceAPI/stock/risk_model.py
 jdw/data/SurfaceAPI/stock/yields.py
 jdw/kdutils/__init__.py
 jdw/kdutils/create_id.py
 jdw/kdutils/file_utils.py
 jdw/kdutils/logger.py
 jdw/kdutils/singleton.py
```

### Comparing `Finance-Jindowin-1.2.5/jdw/__init__.py` & `Finance-Jindowin-1.2.5.1/jdw/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/db_factory.py` & `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/db_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/fetch_engine.py` & `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/fetch_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/kd/kd_engine.py` & `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/kd/kd_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/DataAPI/db/utilities.py` & `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/db/utilities.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/DataAPI/mg/fetch_engine.py` & `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/fetch_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/DataAPI/mg/kn/kn_engine.py` & `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/kn/kn_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/DataAPI/mg/mg_factory.py` & `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/mg/mg_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/DataAPI/rf/EVENT.py` & `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/EVENT.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/DataAPI/rf/STOCK.py` & `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/STOCK.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/DataAPI/rf/THEME.py` & `Finance-Jindowin-1.2.5.1/jdw/data/DataAPI/rf/THEME.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/__init__.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/dummy.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/dummy.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/factors.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/factors.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,14 +32,48 @@
                     break
 
         if to_keep:
             raise ValueError("factors in <{0}> can't be find".format(to_keep))
 
         return factor_cols
 
+    def category(self, universe, category, start_date, end_date, columns=None):
+        factor_model = self._engine.table_model(category)
+        if columns is not None:
+            cols = [factor_model.trade_date, factor_model.code]
+            for col in columns:
+                cols.append(factor_model.__dict__[col])
+        else:
+            cols = [factor_model]
+
+        if isinstance(universe, Universe):
+            cond = universe._query_statements(start_date, end_date)
+            universe_model = universe._table_model
+            big_table = join(
+                factor_model, universe_model,
+                and_(factor_model.trade_date == universe_model.trade_date,
+                     factor_model.code == universe_model.code,
+                     factor_model.flag == 1, cond))
+            query = select(cols).select_from(big_table)\
+            .order_by(factor_model.trade_date, factor_model.code)
+        else:
+            query = select(cols).where(
+                and_(factor_model.trade_date.between(start_date, end_date),
+                     factor_model.code.in_(universe))).order_by(
+                         factor_model.trade_date, factor_model.code)
+        df = pd.read_sql(query, self._engine.client())
+        if 'id' in df.columns:
+            df.drop('id', axis=1, inplace=True)
+        if 'flag' in df.columns:
+            df.drop('flag', axis=1, inplace=True)
+        if 'timestamp' in df.columns:
+            df.drop('timestamp', axis=1, inplace=True)
+        df.replace([-np.inf, np.inf], np.nan, inplace=True)
+        return df
+
     def fetch(self, universe, start_date, end_date, columns):
         if isinstance(columns, Transformer):
             transformer = columns
         else:
             transformer = Transformer(columns)
         dependency = transformer.dependency
         universe_model = universe._table_model if isinstance(
```

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/basic.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/classify.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/classify.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/index_market.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/index_market.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/futures/yields.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/futures/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/index_component.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/index_component.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/index_market.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/index_market.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/industry.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/industry.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/market_stock.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/market_stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/risk_model.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/risk_model.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/stock/yields.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/stock/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/universe.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/universe.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/utilities.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/utilities.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/data/SurfaceAPI/yields.py` & `Finance-Jindowin-1.2.5.1/jdw/data/SurfaceAPI/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/kdutils/create_id.py` & `Finance-Jindowin-1.2.5.1/jdw/kdutils/create_id.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/kdutils/data/mongodb.py` & `Finance-Jindowin-1.2.5.1/jdw/kdutils/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/kdutils/division/decorator.py` & `Finance-Jindowin-1.2.5.1/jdw/kdutils/division/decorator.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/kdutils/division/export.py` & `Finance-Jindowin-1.2.5.1/jdw/kdutils/division/export.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/kdutils/file_utils.py` & `Finance-Jindowin-1.2.5.1/jdw/kdutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/kdutils/logger.py` & `Finance-Jindowin-1.2.5.1/jdw/kdutils/logger.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/anode/axtell.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/anode/axtell.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/anode/conor.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/anode/conor.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/deckard/goslin.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/deckard/goslin.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/__init__.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/evolution/base.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,15 +411,15 @@
         return dummy_data
 
     def prepare_data(self, begin_date=None, end_date=None):
         yields_data = self.fetch_yields(
             begin_date=begin_date,
             end_date=end_date,
             universe=self._universe_class(u_name=self._universe))
-        
+
         factors_data = self.factors_data(
             begin_date=begin_date,
             end_date=end_date,
             factor_name=self._transformer.dependency,
             universe=self._universe_class(u_name=self._universe))
 
         industry_data = self.fetch_industry(
```

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/evolution/futures.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/evolution/paramizer.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/paramizer.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/evolution/stock.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/evolution/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/geneticist/base.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,23 +240,25 @@
         init_config('hoist_mutation', 0.1, configure)  # 突变异率
         init_config('point_replace', 0.1, configure)  # 点交换率
         init_config('rootid', str(int(time.time())), configure)  # 节点
         init_config('convergence', 0.002, configure)  # 每一代收敛预设停止值
 
     def calculate_result(self, total_data, configure, custom_params=None):
         operators_sets = custom_transformer(self._operators)
+        self.create_configure(configure)
         kwargs = custom_params if isinstance(custom_params, dict) else {}
-        kwargs['evaluate'] = configure['evaluate']
-        kwargs['method'] = configure['method']
         kwargs['horizon'] = self._horizon
         kwargs['offset'] = self._offset
         kwargs['universe'] = self._universe
         kwargs['hold'] = self._horizon
-
-        self.create_configure(configure)
+        kwargs['evaluate'] = configure['evaluate']
+        kwargs['method'] = configure['method']
+        kwargs['tournament_size'] = configure['tournament_size']
+        kwargs['standard_score'] = configure['standard_score']
+        kwargs['rootid'] = configure['rootid']
         configure['custom_params'] = kwargs
         gentic = self.create_gentic(operators_sets, configure)
         gentic.train(total_data=total_data)
         return self._evolution_sets if self._callback_save is None else None
 
     def run(self, begin_date, end_date, configure, custom_params=None):
         total_data = self.prepare_data(begin_date=begin_date,
```

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/geneticist/futures.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/geneticist/stock.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/geneticist/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/mutation/base.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/mutation/futures.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/catalyst/mutation/stock.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/catalyst/mutation/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/carnot/base.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-import hashlib, copy, json
+import hashlib, copy, json, pdb
 import numpy as np
 import pandas as pd
 from ultron.tradingday import *
 from ultron.optimize.model.modelbase import load_module
 from ultron.factor.data.transformer import Transformer
 from ultron.factor.data.processing import factor_processing
 from ultron.factor.data.winsorize import winsorize_normal
@@ -287,22 +287,28 @@
             index = (date_label >= start) & (date_label <= end)
             base_model = copy.deepcopy(alpha_model)
             train_data = total_data.set_index(
                 'trade_date').loc[index].reset_index()
             train_data = train_data.sort_values(by=['trade_date', 'code'])
             ne_x = train_data[self._alpha_model.formulas.names].values
 
-            codes = train_data.code
+            #codes = train_data.code
+            kd_logger.info("start predict {} model".format(d))
+            index = train_data.set_index(['trade_date', 'code']).index
             X = pd.DataFrame(
                 ne_x, columns=self._alpha_model.formulas.names).fillna(0)
             y = pd.DataFrame(base_model.predict(X).flatten(),
-                             index=codes,
+                             index=index,
                              columns=[self._factor_name])
+            # 获取最新一期
+            y = y.reset_index().sort_values(
+                by=['trade_date', 'code']).drop_duplicates(subset=['code'],
+                                                           keep='last')
             y['trade_date'] = d
-            res.append(y.reset_index().set_index(['trade_date', 'code']))
+            res.append(y.set_index(['trade_date', 'code']))
         return pd.concat(res, axis=0)
 
     def generate_models(self, begin_date, end_date):
         start_date = advanceDateByCalendar(
             'china.sse', begin_date,
             "-{}b".format(self._batch + self._freq + 1),
             BizDayConventions.Following)
```

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/carnot/futures.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/futures.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # -*- coding: utf-8 -*-
-from jdw.mfc.entropy.gravity.carnot.base import Base
+from jdw.mfc.entropy.gravity.mixture.base import Base
 from jdw.data.SurfaceAPI.futures.factors import FutFactors
 from jdw.data.SurfaceAPI.universe import FutUniverse
 from jdw.data.SurfaceAPI.futures.yields import FutYields
 from jdw.data.SurfaceAPI.futures.classify import FutClassify
 
 
-class FuturesCarnot(Base):
+class FuturesMixture(Base):
 
     def __init__(self,
-                 model_name,
-                 model_params,
-                 features,
-                 factors_normal=True,
-                 horizon=1,
+                 model_name=None,
+                 model_params=None,
+                 model_sets=[],
                  batch=1,
                  freq=1,
-                 offset=0,
+                 horizon=1,
+                 offset=1,
+                 stacking=False,
+                 factors_normal=True,
                  industry_name='kh',
                  industry_level=1,
-                 yield_name='ret',
+                 yield_name='returns',
                  universe=None):
-        super(FuturesCarnot, self).__init__(factor_class=FutFactors,
-                                            universe_class=FutUniverse,
-                                            yields_class=FutYields,
-                                            industry_class=FutClassify,
-                                            model_name=model_name,
-                                            model_params=model_params,
-                                            features=features,
-                                            factors_normal=factors_normal,
-                                            batch=batch,
-                                            freq=freq,
-                                            offset=offset,
-                                            horizon=horizon,
-                                            industry_name=industry_name,
-                                            industry_level=industry_level,
-                                            yield_name=yield_name,
-                                            universe=universe)
+        super(FuturesMixture, self).__init__(factor_class=FutFactors,
+                                             universe_class=FutUniverse,
+                                             yields_class=FutYields,
+                                             industry_class=FutClassify,
+                                             model_name=model_name,
+                                             model_params=model_params,
+                                             model_sets=model_sets,
+                                             batch=batch,
+                                             freq=freq,
+                                             horizon=horizon,
+                                             offset=offset,
+                                             stacking=stacking,
+                                             factors_normal=factors_normal,
+                                             industry_name=industry_name,
+                                             industry_level=industry_level,
+                                             yield_name=yield_name,
+                                             universe=universe)
```

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/carnot/stock.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/stock.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
                  model_params,
                  features,
                  factors_normal=True,
                  horizon=1,
                  batch=1,
                  freq=1,
                  offset=0,
+                 factor_name=None,
                  industry_name='sw',
                  industry_level=1,
                  yield_name='ret',
                  universe=None):
         super(StockCarnot, self).__init__(factor_class=StkFactors,
                                           universe_class=StkUniverse,
                                           yields_class=StkYields,
@@ -29,11 +30,12 @@
                                           model_params=model_params,
                                           features=features,
                                           factors_normal=factors_normal,
                                           batch=batch,
                                           freq=freq,
                                           offset=offset,
                                           horizon=horizon,
+                                          factor_name=factor_name,
                                           industry_name=industry_name,
                                           industry_level=industry_level,
                                           yield_name=yield_name,
                                           universe=universe)
```

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/dendall/base.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/dendall/futures.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/dendall/params.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/params.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/dendall/stock.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/dendall/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/futures/alpha.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/alpha.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/futures/daily.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/futures/daily.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/base copy.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/base copy.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/base.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 class Base(object):
 
     def __init__(self,
                  factor_class,
                  universe_class,
                  yields_class,
                  industry_class,
-                 model_name,
-                 model_params,
-                 model_sets,
+                 model_name=None,
+                 model_params=None,
+                 model_sets=[],
                  batch=1,
                  freq=1,
                  horizon=1,
                  offset=1,
                  stacking=False,
                  factors_normal=True,
                  industry_name='sw',
@@ -40,22 +40,24 @@
         self._industry_class = industry_class
         self._universe_class = universe_class
         self._industry_name = industry_name
         self._industry_level = industry_level
         self._universe = universe
         self._factors_normal = factors_normal
         self._yield_name = yield_name
-        self._integrated_model = IntegratedModel(model_name=model_name,
-                                                 model_params=model_params,
-                                                 model_sets=model_sets,
-                                                 batch=batch,
-                                                 freq=freq,
-                                                 horizon=horizon,
-                                                 offset=offset,
-                                                 stacking=stacking)
+        self._integrated_model = None
+        if model_name is not None:
+            self._integrated_model = IntegratedModel(model_name=model_name,
+                                                     model_params=model_params,
+                                                     model_sets=model_sets,
+                                                     batch=batch,
+                                                     freq=freq,
+                                                     horizon=horizon,
+                                                     offset=offset,
+                                                     stacking=stacking)
 
     def initialize_params(self):
         kd_logger.info("initialize params")
         max_horizon = self._integrated_model.max_params(
             'horizon') + self._integrated_model._horizon
         max_offset = self._integrated_model.max_params(
             'offset') + self._integrated_model._offset
@@ -150,15 +152,14 @@
 
     def factors_normal(self, factors_data, factors_columns):
         kd_logger.info("start factors normal")
         new_factors = factor_processing(
             factors_data[factors_columns].values,
             pre_process=[winsorize_normal, standardize],
             groups=factors_data['trade_date'].values)
-
         factors_data = pd.DataFrame(new_factors,
                                     columns=factors_columns,
                                     index=factors_data.set_index(
                                         ['trade_date', 'code']).index)
         factors_data = factors_data.reset_index()
         factors_data = factors_data.sort_values(by=['trade_date', 'code'])
         return factors_data
@@ -166,19 +167,17 @@
     def prepare_data(self, begin_date, end_date, formulas, is_train=True):
         if is_train:
             yields_data = self.fetch_yields(
                 begin_date=begin_date,
                 end_date=end_date,
                 universe=self._universe_class(u_name=self._universe))
 
-        dependency = list(
-            itertools.chain.from_iterable([x.dependency for x in formulas]))
+        dependency = self._integrated_model.dependency()
 
-        factors_columns = list(
-            itertools.chain.from_iterable([x.names for x in formulas]))
+        factors_columns = self._integrated_model.features()
 
         factors_data = self.factors_data(
             begin_date=begin_date,
             end_date=end_date,
             factor_name=dependency,
             universe=self._universe_class(u_name=self._universe))
 
@@ -188,34 +187,41 @@
             universe=self._universe_class(u_name=self._universe))
 
         factors_data = self.industry_fillna(
             industry_data=industry_data, factors_data=factors_data).fillna(0)
         factors_data = factors_data.sort_values(by=['trade_date', 'code'])
         ### 因子换算
         factors_data = factors_data.sort_values(by=['trade_date', 'code'])
+        '''
         res = []
         for exp in formulas:
             formula_data = exp.transform(
                 'code', factors_data.set_index('trade_date')).reset_index()
             res.append(formula_data.set_index(['trade_date', 'code']))
         factors_data = pd.concat(res, axis=1).reset_index()
+        '''
+        factors_data = formulas.transform(
+            'code', factors_data.set_index('trade_date')).reset_index()
         ### 行业中位数填充
         if self._factors_normal:
             if is_train:
                 total_data = factors_data.merge(yields_data,
                                                 on=['trade_date', 'code'])
                 total_data = self.factors_normal(
                     total_data, factors_columns + ['nxt1_ret'])
             else:
                 total_data = factors_data
                 total_data = self.factors_normal(total_data, factors_columns)
         return total_data
 
-    def save(self):
-        return self._integrated_model.save()
+    def dump_models(self):
+        return self._integrated_model.dump_models()
+
+    def load_models(self, desc):
+        self._integrated_model = IntegratedModel.mixture_clf_load(desc)
 
     def generate_models(self, begin_date, end_date):
         max_offset, max_horizon, max_batch, max_freq = self.initialize_params()
         start_date = advanceDateByCalendar(
             'china.sse', begin_date,
             "-{}b".format(max_horizon + max_offset + 1),
             BizDayConventions.Following)
```

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/futures.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/stock.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # -*- coding: utf-8 -*-
 from jdw.mfc.entropy.gravity.mixture.base import Base
-from jdw.data.SurfaceAPI.futures.factors import FutFactors
-from jdw.data.SurfaceAPI.universe import FutUniverse
-from jdw.data.SurfaceAPI.futures.yields import FutYields
-from jdw.data.SurfaceAPI.futures.classify import FutClassify
+from jdw.data.SurfaceAPI.stock.factors import StkFactors
+from jdw.data.SurfaceAPI.universe import StkUniverse
+from jdw.data.SurfaceAPI.stock.yields import StkYields
+from jdw.data.SurfaceAPI.stock.industry import Industry
 
 
-class FuturesMixture(Base):
+class StockMixture(Base):
 
     def __init__(self,
-                 model_name,
-                 model_params,
-                 model_sets,
+                 model_name=None,
+                 model_params=None,
+                 model_sets=[],
                  batch=1,
                  freq=1,
                  horizon=1,
                  offset=1,
                  stacking=False,
                  factors_normal=True,
-                 industry_name='kh',
+                 industry_name='sw',
                  industry_level=1,
                  yield_name='returns',
                  universe=None):
-        super(FuturesMixture, self).__init__(factor_class=FutFactors,
-                                             universe_class=FutUniverse,
-                                             yields_class=FutYields,
-                                             industry_class=FutClassify,
-                                             model_name=model_name,
-                                             model_params=model_params,
-                                             model_sets=model_sets,
-                                             batch=batch,
-                                             freq=freq,
-                                             horizon=horizon,
-                                             offset=offset,
-                                             stacking=stacking,
-                                             factors_normal=factors_normal,
-                                             industry_name=industry_name,
-                                             industry_level=industry_level,
-                                             yield_name=yield_name,
-                                             universe=universe)
+        super(StockMixture, self).__init__(factor_class=StkFactors,
+                                           universe_class=StkUniverse,
+                                           yields_class=StkYields,
+                                           industry_class=Industry,
+                                           model_name=model_name,
+                                           model_params=model_params,
+                                           model_sets=model_sets,
+                                           batch=batch,
+                                           freq=freq,
+                                           horizon=horizon,
+                                           offset=offset,
+                                           stacking=stacking,
+                                           factors_normal=factors_normal,
+                                           industry_name=industry_name,
+                                           industry_level=industry_level,
+                                           yield_name=yield_name,
+                                           universe=universe)
```

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/models.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/mixture/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # -*- coding: utf-8 -*-
 import copy, hashlib, json, pdb, itertools
 import pandas as pd
 from ultron.tradingday import *
+from ultron.sentry.Analysis.SecurityValueHolders import SecurityValueHolder
 from ultron.optimize.model.treemodel import StackingRegressor
 from ultron.optimize.model.modelbase import load_module
-from ultron.factor.utilities import encode
+from ultron.factor.utilities import encode, decode
+from ultron.factor.data.transformer import Transformer
 from jdw.kdutils.create_id import create_id
 from jdw.kdutils.logger import kd_logger
 
 
 class ModelTuple(object):
 
     def __init__(self, features, model_name, params, batch, freq, horizon,
                  offset):
         alpha_model = load_module(model_name)(features=features, **params)
         s = hashlib.md5(
             json.dumps({
                 'name': model_name,
                 'feature': alpha_model.formulas.names,
-                'params': params
+                'params': params,
+                'batch': batch,
+                'freq': freq,
+                'horizon': horizon,
+                'offset': offset
             }).encode(encoding="utf-8")).hexdigest()
         self.id = create_id(original=s, digit=10)
         self.alpha_model = alpha_model
         self.features = features
         self.model_name = model_name
         self.params = params
         self.batch = batch
@@ -30,55 +36,116 @@
         self.horizon = horizon
         self.offset = offset
         self.train_models = []
 
 
 class IntegratedModel(object):
 
+    @classmethod
+    def mixture_clf_dump(cls, total_data, begin_date, end_date, model_name,
+                         model_params, model_sets, batch, freq, horizon,
+                         offset, stacking):
+        integrated_model = cls(model_name=model_name,
+                               model_params=model_params,
+                               model_sets=model_sets,
+                               batch=batch,
+                               freq=freq,
+                               horizon=horizon,
+                               offset=offset,
+                               stacking=stacking)
+        integrated_model.generate_models(total_data=total_data,
+                                         begin_date=begin_date,
+                                         end_date=end_date)
+        return integrated_model.save_models()
+
+    @classmethod
+    def mixture_clf_load(cls, desc):
+        model_desc = decode(desc)
+        base_model = decode(model_desc['base_model'])
+        model_sets = model_desc['model_sets']
+        sets = []
+        for model in model_sets:
+            sets.append(decode(model))
+        stacking = model_desc['stacking']
+        integrated_model = cls(model_name=base_model['name'],
+                               model_params=base_model['params'],
+                               model_sets=model_sets,
+                               batch=base_model['batch'],
+                               freq=base_model['freq'],
+                               horizon=base_model['horizon'],
+                               offset=base_model['offset'],
+                               stacking=stacking,
+                               alpha_models={
+                                   'models': base_model['models'],
+                                   'id': base_model['id']
+                               })
+        return integrated_model
+
     def __init__(self,
                  model_name,
                  model_params,
                  model_sets,
                  batch=1,
                  freq=1,
                  horizon=1,
                  offset=1,
-                 stacking=False):
+                 stacking=False,
+                 alpha_models=None):
         self._model_name = model_name
         self._model_params = model_params
         self._batch = batch
         self._freq = freq
         self._horizon = horizon
         self._offset = offset
         self._model_sets = self.initialize_models(model_sets)
         self._stacking = stacking
+        self._alpha_models = alpha_models
 
     def initialize_models(self, model_sets):
         kd_logger.info("initialize models")
         return [
             ModelTuple(features=x['features'],
                        model_name=x['model_name'],
                        params=x['params'],
                        batch=x['batch'],
                        freq=x['freq'],
                        horizon=x['horizon'],
                        offset=x['offset']) for x in model_sets
         ]
 
     def formulas(self):
-        return [x.alpha_model.formulas for x in self._model_sets]
+        features = [x.features for x in self._model_sets]
+        features = list(itertools.chain.from_iterable(features))
+        formulas = []
+        names = []
+        for f in features:
+            if isinstance(f, str) and f not in names:
+                formulas.append(f)
+                names.append(f)
+            elif isinstance(f, SecurityValueHolder):
+                formulas.append(f)
+        return Transformer(formulas)
 
     def features(self):
         return list(
             set(
                 list(
                     itertools.chain.from_iterable([
                         x.alpha_model.formulas.names for x in self._model_sets
                     ]))))
 
+    def dependency(self):
+        return list(
+            set(
+                list(
+                    itertools.chain.from_iterable([
+                        x.alpha_model.formulas.dependency
+                        for x in self._model_sets
+                    ]))))
+
     def max_params(self, name):
         return max([x.__getattribute__(name) for x in self._model_sets])
 
     def create_model(self, total_data, name, mid, alpha_model, batch, freq,
                      begin_date, end_date):
         models = {}
         date_label = pd.DatetimeIndex(total_data.trade_date).to_pydatetime()
@@ -212,22 +279,22 @@
         s = hashlib.md5(
             json.dumps({
                 'name': self._model_name,
                 'feature': alpha_model.formulas.names,
                 'params': self._model_params
             }).encode(encoding="utf-8")).hexdigest()
         mid = create_id(original=s, digit=10)
-        self._alpha_model = self.create_model(total_data=factors_data,
-                                              name=self._model_name,
-                                              mid=mid,
-                                              alpha_model=alpha_model,
-                                              batch=self._batch,
-                                              freq=self._freq,
-                                              begin_date=begin_date,
-                                              end_date=end_date)
+        self._alpha_models = self.create_model(total_data=factors_data,
+                                               name=self._model_name,
+                                               mid=mid,
+                                               alpha_model=alpha_model,
+                                               batch=self._batch,
+                                               freq=self._freq,
+                                               begin_date=begin_date,
+                                               end_date=end_date)
 
     def create_factors(self, total_data, begin_date, end_date):
         res = []
         for model_tuple in self._model_sets:
             new_factors = self.predict(
                 mid=model_tuple.id,
                 total_data=total_data[
@@ -254,30 +321,48 @@
             json.dumps({
                 'name': self._model_name,
                 'feature': alpha_model.formulas.names,
                 'params': self._model_params
             }).encode(encoding="utf-8")).hexdigest()
         mid = create_id(original=s, digit=10)
 
-        self._alpha_model = self.create_model(total_data=total_data,
-                                              name=self._model_name,
-                                              mid=mid,
-                                              alpha_model=model,
-                                              batch=self._batch,
-                                              freq=self._freq,
-                                              begin_date=begin_date,
-                                              end_date=end_date)
+        self._alpha_models = self.create_model(total_data=total_data,
+                                               name=self._model_name,
+                                               mid=mid,
+                                               alpha_model=model,
+                                               batch=self._batch,
+                                               freq=self._freq,
+                                               begin_date=begin_date,
+                                               end_date=end_date)
 
-    def save(self):
+    def dump_models(self):
         res = []
         if not self._stacking:
             for model in self._model_sets:
-                rs = {'model': model.train_models, 'id': model.id}
+                rs = {'model': encode(model), 'id': model.id}
                 res.append(rs)
-        desc = {'model_sets': res, 'base': self._alpha_model['models']}
+        desc = {
+            'model_sets':
+            res,
+            'base_model':
+            encode({
+                'name': self._model_name,
+                'params': self._model_params,
+                'batch': self._batch,
+                'freq': self._freq,
+                'horizon': self._horizon,
+                'offset': self._offset,
+                'models': self._alpha_models['models'],
+                'id': self._alpha_models['id']
+            }),
+            'stacking':
+            self._stacking,
+            'version':
+            1.0
+        }
         return encode(desc)
 
     def generate_models(self, total_data, begin_date, end_date):
         kd_logger.info("generate models")
         if not self._stacking:
             self.train_models(total_data=total_data,
                               begin_date=begin_date,
@@ -300,24 +385,24 @@
 
     def generate_predict(self, total_data, begin_date, end_date):
         kd_logger.info("generate predict")
         if not self._stacking:
             factors_data = self.create_factors(total_data=total_data,
                                                begin_date=begin_date,
                                                end_date=end_date)
-            new_factors = self.predict(mid=self._alpha_model['id'],
+            new_factors = self.predict(mid=self._alpha_models['id'],
                                        total_data=factors_data.reset_index(),
-                                       models=self._alpha_model['models'],
+                                       models=self._alpha_models['models'],
                                        freq=self._freq,
                                        batch=self._batch,
                                        begin_date=begin_date,
                                        end_date=end_date)
         else:
-            new_factors = self.predict(mid=self._alpha_model['id'],
+            new_factors = self.predict(mid=self._alpha_models['id'],
                                        total_data=total_data,
-                                       models=self._alpha_model['models'],
+                                       models=self._alpha_models['models'],
                                        freq=self._freq,
                                        batch=self._batch,
                                        begin_date=begin_date,
                                        end_date=end_date)
 
         return new_factors
```

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/mixture/stock.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/carnot/futures.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # -*- coding: utf-8 -*-
-from jdw.mfc.entropy.gravity.mixture.base import Base
-from jdw.data.SurfaceAPI.stock.factors import StkFactors
-from jdw.data.SurfaceAPI.universe import StkUniverse
-from jdw.data.SurfaceAPI.stock.yields import StkYields
-from jdw.data.SurfaceAPI.stock.industry import Industry
+from jdw.mfc.entropy.gravity.carnot.base import Base
+from jdw.data.SurfaceAPI.futures.factors import FutFactors
+from jdw.data.SurfaceAPI.universe import FutUniverse
+from jdw.data.SurfaceAPI.futures.yields import FutYields
+from jdw.data.SurfaceAPI.futures.classify import FutClassify
 
 
-class StockMixture(Base):
+class FuturesCarnot(Base):
 
     def __init__(self,
                  model_name,
                  model_params,
-                 model_sets,
+                 features,
+                 factors_normal=True,
+                 horizon=1,
                  batch=1,
                  freq=1,
-                 horizon=1,
-                 offset=1,
-                 stacking=False,
-                 factors_normal=True,
-                 industry_name='sw',
+                 offset=0,
+                 factor_name=None,
+                 industry_name='kh',
                  industry_level=1,
-                 yield_name='returns',
+                 yield_name='ret',
                  universe=None):
-        super(StockMixture, self).__init__(factor_class=StkFactors,
-                                           universe_class=StkUniverse,
-                                           yields_class=StkYields,
-                                           industry_class=Industry,
-                                           model_name=model_name,
-                                           model_params=model_params,
-                                           model_sets=model_sets,
-                                           batch=batch,
-                                           freq=freq,
-                                           horizon=horizon,
-                                           offset=offset,
-                                           stacking=stacking,
-                                           factors_normal=factors_normal,
-                                           industry_name=industry_name,
-                                           industry_level=industry_level,
-                                           yield_name=yield_name,
-                                           universe=universe)
+        super(FuturesCarnot, self).__init__(factor_class=FutFactors,
+                                            universe_class=FutUniverse,
+                                            yields_class=FutYields,
+                                            industry_class=FutClassify,
+                                            model_name=model_name,
+                                            model_params=model_params,
+                                            features=features,
+                                            factors_normal=factors_normal,
+                                            batch=batch,
+                                            freq=freq,
+                                            offset=offset,
+                                            horizon=horizon,
+                                            factor_name=factor_name,
+                                            industry_name=industry_name,
+                                            industry_level=industry_level,
+                                            yield_name=yield_name,
+                                            universe=universe)
```

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/stock/alpha.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/alpha.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/gravity/stock/daily.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/gravity/stock/daily.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/metrics/base.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/metrics/futures.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/metrics/stock.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/metrics/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/score/base.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/score/futures.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/entropy/pascal/score/stock.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/entropy/pascal/score/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/atl/engine.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/atl/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/mg_factory.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/mg_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/ntn/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/experimental/DataAPI/mg/operator_engine.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/experimental/DataAPI/mg/operator_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/irey/kestle.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/irey/kestle.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/lombard/base.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/lombard/futures.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/futures.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/lombard/indicator/atr.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/atr.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/lombard/indicator/base.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/lombard/indicator/date.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/date.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/lombard/indicator/symbol_pd.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/indicator/symbol_pd.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/lombard/stock.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/lombard/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/neutron/analysis.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/analysis.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/neutron/factory.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/neutron/strategy.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/strategy.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/neutron/trader.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/neutron/trader.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/mfc/oss/aliyun.py` & `Finance-Jindowin-1.2.5.1/jdw/mfc/oss/aliyun.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/STOCK/detail.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/detail.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/STOCK/flow_money.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/flow_money.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/STOCK/hkshshz.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/hkshshz.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/STOCK/sentiment.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/STOCK/sentiment.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/THEME/brief.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/brief.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/THEME/detail.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/detail.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/THEME/flow_money.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/flow_money.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/THEME/hkshshz.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/hkshshz.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/THEME/indicators.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/indicators.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/THEME/returns.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/returns.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/THEME/sentiment.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/THEME/sentiment.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/__init__.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/returns.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/returns.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/plot/stock.py` & `Finance-Jindowin-1.2.5.1/jdw/plot/stock.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/to_pandas.py` & `Finance-Jindowin-1.2.5.1/jdw/to_pandas.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/jdw/utils.py` & `Finance-Jindowin-1.2.5.1/jdw/utils.py`

 * *Files identical despite different names*

### Comparing `Finance-Jindowin-1.2.5/setup.py` & `Finance-Jindowin-1.2.5.1/setup.py`

 * *Files identical despite different names*

