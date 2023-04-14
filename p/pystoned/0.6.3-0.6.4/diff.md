# Comparing `tmp/pystoned-0.6.3.tar.gz` & `tmp/pystoned-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystoned-0.6.3.tar", last modified: Sat Apr  8 11:02:58 2023, max compression
+gzip compressed data, was "pystoned-0.6.4.tar", last modified: Fri Apr 14 13:50:02 2023, max compression
```

## Comparing `pystoned-0.6.3.tar` & `pystoned-0.6.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-08 11:02:58.123448 pystoned-0.6.3/
--rw-r--r--   0 dais2     (1000) dais2     (1000)    35149 2021-10-05 07:06:23.000000 pystoned-0.6.3/LICENSE
--rw-rw-r--   0 dais2     (1000) dais2     (1000)     2976 2023-04-08 11:02:58.123448 pystoned-0.6.3/PKG-INFO
--rw-r--r--   0 dais2     (1000) dais2     (1000)     2288 2023-01-28 14:01:26.000000 pystoned-0.6.3/README.md
-drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-08 11:02:58.119448 pystoned-0.6.3/pystoned/
--rw-r--r--   0 dais2     (1000) dais2     (1000)    13169 2023-02-25 14:32:21.000000 pystoned-0.6.3/pystoned/CNLS.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     8579 2023-04-07 08:10:12.000000 pystoned-0.6.3/pystoned/CNLSDDF.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     9784 2023-02-25 14:32:53.000000 pystoned-0.6.3/pystoned/CNLSG.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    15726 2023-02-25 14:33:03.000000 pystoned-0.6.3/pystoned/CQER.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     8122 2023-04-07 08:10:02.000000 pystoned-0.6.3/pystoned/CQERDDF.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    21380 2023-02-25 14:32:38.000000 pystoned-0.6.3/pystoned/CQERG.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     6613 2023-04-07 08:10:07.000000 pystoned-0.6.3/pystoned/CSVR.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    18111 2023-04-07 08:09:53.000000 pystoned-0.6.3/pystoned/DEA.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     5964 2023-04-07 08:09:49.000000 pystoned-0.6.3/pystoned/FDH.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     4816 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/ICNLS.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     2861 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/ICQER.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     9456 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/StoNED.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)      800 2023-01-31 11:34:44.000000 pystoned-0.6.3/pystoned/__init__.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     1473 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/constant.py
-drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-08 11:02:58.123448 pystoned-0.6.3/pystoned/data/
--rw-r--r--   0 dais2     (1000) dais2     (1000)     1429 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/data/41Firm.csv
--rw-r--r--   0 dais2     (1000) dais2     (1000)     7609 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/data/abatementCost.csv
--rw-r--r--   0 dais2     (1000) dais2     (1000)     3082 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/data/electricityFirms.csv
--rw-r--r--   0 dais2     (1000) dais2     (1000)    33693 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/data/riceProduction.csv
--rw-r--r--   0 dais2     (1000) dais2     (1000)     4733 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/dataset.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     2993 2023-04-08 10:42:52.000000 pystoned-0.6.3/pystoned/pCNLS.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     6357 2023-04-08 10:42:11.000000 pystoned-0.6.3/pystoned/pCQER.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     3250 2023-04-08 10:44:39.000000 pystoned-0.6.3/pystoned/pICQER.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     4548 2023-02-26 18:24:25.000000 pystoned-0.6.3/pystoned/plot.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     8256 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/sCQER.py
-drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-08 11:02:58.123448 pystoned-0.6.3/pystoned/utils/
--rw-r--r--   0 dais2     (1000) dais2     (1000)    11736 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/utils/CNLSG1.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    14915 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/utils/CNLSG2.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    12161 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/utils/CNLSZG1.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    15358 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/utils/CNLSZG2.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    13742 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/utils/CQERG1.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    16930 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/utils/CQERG2.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    14286 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/utils/CQERZG1.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    17619 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/utils/CQERZG2.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)      240 2023-01-28 13:53:33.000000 pystoned-0.6.3/pystoned/utils/__init__.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     1121 2023-02-25 14:26:26.000000 pystoned-0.6.3/pystoned/utils/interpolation.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)      960 2023-02-25 12:37:20.000000 pystoned-0.6.3/pystoned/utils/sweet.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     8684 2023-03-04 07:54:35.000000 pystoned-0.6.3/pystoned/utils/tools.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     1632 2023-04-07 23:03:08.000000 pystoned-0.6.3/pystoned/wCNLS.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)     3327 2023-04-07 23:03:03.000000 pystoned-0.6.3/pystoned/wCQER.py
--rw-r--r--   0 dais2     (1000) dais2     (1000)    11886 2023-04-07 23:04:51.000000 pystoned-0.6.3/pystoned/weakCNLS.py
-drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-08 11:02:58.123448 pystoned-0.6.3/pystoned.egg-info/
--rw-rw-r--   0 dais2     (1000) dais2     (1000)     2976 2023-04-08 11:02:58.000000 pystoned-0.6.3/pystoned.egg-info/PKG-INFO
--rw-rw-r--   0 dais2     (1000) dais2     (1000)     1075 2023-04-08 11:02:58.000000 pystoned-0.6.3/pystoned.egg-info/SOURCES.txt
--rw-rw-r--   0 dais2     (1000) dais2     (1000)        1 2023-04-08 11:02:58.000000 pystoned-0.6.3/pystoned.egg-info/dependency_links.txt
--rw-rw-r--   0 dais2     (1000) dais2     (1000)        1 2023-04-08 11:02:57.000000 pystoned-0.6.3/pystoned.egg-info/not-zip-safe
--rw-rw-r--   0 dais2     (1000) dais2     (1000)       86 2023-04-08 11:02:58.000000 pystoned-0.6.3/pystoned.egg-info/requires.txt
--rw-rw-r--   0 dais2     (1000) dais2     (1000)        9 2023-04-08 11:02:58.000000 pystoned-0.6.3/pystoned.egg-info/top_level.txt
--rw-rw-r--   0 dais2     (1000) dais2     (1000)       38 2023-04-08 11:02:58.123448 pystoned-0.6.3/setup.cfg
--rw-r--r--   0 dais2     (1000) dais2     (1000)     1345 2023-04-08 10:57:22.000000 pystoned-0.6.3/setup.py
+drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-14 13:50:02.637539 pystoned-0.6.4/
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    35149 2021-10-05 07:06:23.000000 pystoned-0.6.4/LICENSE
+-rw-rw-r--   0 dais2     (1000) dais2     (1000)     2976 2023-04-14 13:50:02.637539 pystoned-0.6.4/PKG-INFO
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     2288 2023-01-28 14:01:26.000000 pystoned-0.6.4/README.md
+drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-14 13:50:02.633539 pystoned-0.6.4/pystoned/
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    13360 2023-04-14 13:42:03.000000 pystoned-0.6.4/pystoned/CNLS.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     8579 2023-04-07 08:10:12.000000 pystoned-0.6.4/pystoned/CNLSDDF.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     9975 2023-04-14 13:44:39.000000 pystoned-0.6.4/pystoned/CNLSG.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    15915 2023-04-14 13:31:50.000000 pystoned-0.6.4/pystoned/CQER.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     8122 2023-04-07 08:10:02.000000 pystoned-0.6.4/pystoned/CQERDDF.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    21756 2023-04-14 13:40:58.000000 pystoned-0.6.4/pystoned/CQERG.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     6908 2023-04-14 13:36:31.000000 pystoned-0.6.4/pystoned/CSVR.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    18111 2023-04-07 08:09:53.000000 pystoned-0.6.4/pystoned/DEA.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     5964 2023-04-07 08:09:49.000000 pystoned-0.6.4/pystoned/FDH.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     4816 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/ICNLS.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     2861 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/ICQER.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     9456 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/StoNED.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)      800 2023-01-31 11:34:44.000000 pystoned-0.6.4/pystoned/__init__.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     1473 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/constant.py
+drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-14 13:50:02.633539 pystoned-0.6.4/pystoned/data/
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     1429 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/data/41Firm.csv
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     7609 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/data/abatementCost.csv
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     3082 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/data/electricityFirms.csv
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    33693 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/data/riceProduction.csv
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     4733 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/dataset.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     2993 2023-04-08 10:42:52.000000 pystoned-0.6.4/pystoned/pCNLS.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     6357 2023-04-08 10:42:11.000000 pystoned-0.6.4/pystoned/pCQER.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     3250 2023-04-08 10:44:39.000000 pystoned-0.6.4/pystoned/pICQER.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     4701 2023-04-14 13:15:21.000000 pystoned-0.6.4/pystoned/plot.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     8256 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/sCQER.py
+drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-14 13:50:02.637539 pystoned-0.6.4/pystoned/utils/
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    11736 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CNLSG1.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    14915 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CNLSG2.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    12161 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CNLSZG1.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    15358 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CNLSZG2.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    13742 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CQERG1.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    16930 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CQERG2.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    14286 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CQERZG1.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    17619 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/CQERZG2.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)      240 2023-01-28 13:53:33.000000 pystoned-0.6.4/pystoned/utils/__init__.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     1121 2023-04-14 10:56:02.000000 pystoned-0.6.4/pystoned/utils/interpolation.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)      960 2023-02-25 12:37:20.000000 pystoned-0.6.4/pystoned/utils/sweet.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     8684 2023-03-04 07:54:35.000000 pystoned-0.6.4/pystoned/utils/tools.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     1632 2023-04-07 23:03:08.000000 pystoned-0.6.4/pystoned/wCNLS.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     3327 2023-04-07 23:03:03.000000 pystoned-0.6.4/pystoned/wCQER.py
+-rw-r--r--   0 dais2     (1000) dais2     (1000)    11886 2023-04-07 23:04:51.000000 pystoned-0.6.4/pystoned/weakCNLS.py
+drwxrwxr-x   0 dais2     (1000) dais2     (1000)        0 2023-04-14 13:50:02.633539 pystoned-0.6.4/pystoned.egg-info/
+-rw-rw-r--   0 dais2     (1000) dais2     (1000)     2976 2023-04-14 13:50:02.000000 pystoned-0.6.4/pystoned.egg-info/PKG-INFO
+-rw-rw-r--   0 dais2     (1000) dais2     (1000)     1075 2023-04-14 13:50:02.000000 pystoned-0.6.4/pystoned.egg-info/SOURCES.txt
+-rw-rw-r--   0 dais2     (1000) dais2     (1000)        1 2023-04-14 13:50:02.000000 pystoned-0.6.4/pystoned.egg-info/dependency_links.txt
+-rw-rw-r--   0 dais2     (1000) dais2     (1000)        1 2023-04-14 13:49:08.000000 pystoned-0.6.4/pystoned.egg-info/not-zip-safe
+-rw-rw-r--   0 dais2     (1000) dais2     (1000)       86 2023-04-14 13:50:02.000000 pystoned-0.6.4/pystoned.egg-info/requires.txt
+-rw-rw-r--   0 dais2     (1000) dais2     (1000)        9 2023-04-14 13:50:02.000000 pystoned-0.6.4/pystoned.egg-info/top_level.txt
+-rw-rw-r--   0 dais2     (1000) dais2     (1000)       38 2023-04-14 13:50:02.637539 pystoned-0.6.4/setup.cfg
+-rw-r--r--   0 dais2     (1000) dais2     (1000)     1345 2023-04-14 12:21:31.000000 pystoned-0.6.4/setup.py
```

### Comparing `pystoned-0.6.3/LICENSE` & `pystoned-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/PKG-INFO` & `pystoned-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystoned
-Version: 0.6.3
+Version: 0.6.4
 Summary: A Python Package for Convex Regression and Frontier Estimation
 Home-page: https://github.com/ds2010/pyStoNED
 Download-URL: https://pypi.org/project/pystoned/
 Author: Sheng Dai, Yu-Hsueh Fang, Chia-Yen Lee, Timo Kuosmanen
 Author-email: sheng.dai@utu.fi
 License: GPLv3
 Keywords: StoNED,CNLS,CER,CQR,Z-variables,CNLSG
```

### Comparing `pystoned-0.6.3/README.md` & `pystoned-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/CNLS.py` & `pystoned-0.6.4/pystoned/CNLS.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pyomo.core.expr.numvalue import NumericValue
 import numpy as np
 import pandas as pd
 
 from .constant import CET_ADDI, CET_MULT, FUN_PROD, FUN_COST, OPT_DEFAULT, RTS_CRS, RTS_VRS, OPT_LOCAL
 from .utils import tools, interpolation
 
+
 class CNLS:
     """Convex Nonparametric Least Square (CNLS)
     """
 
     def __init__(self, y, x, z=None, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
         """CNLS model
 
@@ -300,8 +301,12 @@
         """Return the shifted constatnt(alpha) term by CCNLS"""
         tools.assert_optimized(self.optimization_status)
         return self.get_alpha() + np.amax(self.get_residual())
     
     def get_predict(self, x_test):
         """Return the estimated function in testing sample"""
         tools.assert_optimized(self.optimization_status)
-        return interpolation.interpolation(self.get_alpha(), self.get_beta(), x_test, fun=self.fun)
+        if self.rts == RTS_VRS:
+            alpha,  beta = self.get_alpha(), self.get_beta()
+        elif self.rts == RTS_CRS:
+            alpha, beta = np.zeros((self.get_beta()).shape[0]), self.get_beta()
+        return interpolation.interpolation(alpha, beta, x_test, fun=self.fun)
```

### Comparing `pystoned-0.6.3/pystoned/CNLSDDF.py` & `pystoned-0.6.4/pystoned/CNLSDDF.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/CNLSG.py` & `pystoned-0.6.4/pystoned/CNLSG.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,8 +208,12 @@
         """Return the number of blocks"""
         tools.assert_optimized(self.optimization_status)
         return self.count
 
     def get_predict(self, x_test):
         """Return the estimated function in testing sample"""
         tools.assert_optimized(self.optimization_status)
-        return interpolation.interpolation(self.get_alpha(), self.get_beta(), x_test, fun=self.fun)
+        if self.rts == RTS_VRS:
+            alpha,  beta = self.get_alpha(), self.get_beta()
+        elif self.rts == RTS_CRS:
+            alpha, beta = np.zeros((self.get_beta()).shape[0]), self.get_beta()
+        return interpolation.interpolation(alpha, beta, x_test, fun=self.fun)
```

### Comparing `pystoned-0.6.3/pystoned/CQER.py` & `pystoned-0.6.4/pystoned/CQER.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,15 +330,19 @@
         elif self.cet == CET_ADDI:
             frontier = np.asarray(self.y) - self.get_residual()
         return np.asarray(frontier)
     
     def get_predict(self, x_test):
         """Return the estimated function in testing sample"""
         tools.assert_optimized(self.optimization_status)
-        return interpolation.interpolation(self.get_alpha(), self.get_beta(), x_test, fun=self.fun)
+        if self.rts == RTS_VRS:
+            alpha,  beta = self.get_alpha(), self.get_beta()
+        elif self.rts == RTS_CRS:
+            alpha, beta = np.zeros((self.get_beta()).shape[0]), self.get_beta()
+        return interpolation.interpolation(alpha, beta, x_test, fun=self.fun)
 
 
 class CER(CQR):
     """Convex expectile regression (CER)
     """
 
     def __init__(self, y, x, tau, z=None, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
```

### Comparing `pystoned-0.6.3/pystoned/CQERDDF.py` & `pystoned-0.6.4/pystoned/CQERDDF.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/CQERG.py` & `pystoned-0.6.4/pystoned/CQERG.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,16 +232,20 @@
         """Return the number of blocks"""
         tools.assert_optimized(self.optimization_status)
         return self.count
 
     def get_predict(self, x_test):
         """Return the estimated function in testing sample"""
         tools.assert_optimized(self.optimization_status)
-        return interpolation.interpolation(self.get_alpha(), self.get_beta(), x_test, fun=self.fun)
-    
+        if self.rts == RTS_VRS:
+            alpha,  beta = self.get_alpha(), self.get_beta()
+        elif self.rts == RTS_CRS:
+            alpha, beta = np.zeros((self.get_beta()).shape[0]), self.get_beta()
+        return interpolation.interpolation(alpha, beta, x_test, fun=self.fun)
+
 
 class CERG:
     """Convex expectile regression (CER) with Genetic algorithm
     """
 
     def __init__(self, y, x, tau, z=None, cet=CET_ADDI, fun=FUN_PROD, rts=RTS_VRS):
         """CERG model
@@ -465,8 +469,12 @@
         """Return the number of blocks"""
         tools.assert_optimized(self.optimization_status)
         return self.count
 
     def get_predict(self, x_test):
         """Return the estimated function in testing sample"""
         tools.assert_optimized(self.optimization_status)
-        return interpolation.interpolation(self.get_alpha(), self.get_beta(), x_test, fun=self.fun)
+        if self.rts == RTS_VRS:
+            alpha,  beta = self.get_alpha(), self.get_beta()
+        elif self.rts == RTS_CRS:
+            alpha, beta = np.zeros((self.get_beta()).shape[0]), self.get_beta()
+        return interpolation.interpolation(alpha, beta, x_test, fun=self.fun)
```

### Comparing `pystoned-0.6.3/pystoned/CSVR.py` & `pystoned-0.6.4/pystoned/CSVR.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,7 +155,13 @@
         """Return beta value by array"""
         tools.assert_optimized(self.optimization_status)
         beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
                                                           list(self.__model__.beta[:, :].value))])
         beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
         beta = beta.pivot(index='Name', columns='Key', values='Value')
         return beta.to_numpy()
+
+    def get_predict(self, x_test):
+        """Return the estimated function in testing sample"""
+        tools.assert_optimized(self.optimization_status)
+        alpha, beta = self.get_alpha(), self.get_beta()
+        return interpolation.interpolation(alpha, beta, x_test, fun=self.fun)
```

### Comparing `pystoned-0.6.3/pystoned/DEA.py` & `pystoned-0.6.4/pystoned/DEA.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/FDH.py` & `pystoned-0.6.4/pystoned/FDH.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/ICNLS.py` & `pystoned-0.6.4/pystoned/ICNLS.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/ICQER.py` & `pystoned-0.6.4/pystoned/ICQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/StoNED.py` & `pystoned-0.6.4/pystoned/StoNED.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/__init__.py` & `pystoned-0.6.4/pystoned/__init__.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/constant.py` & `pystoned-0.6.4/pystoned/constant.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/data/41Firm.csv` & `pystoned-0.6.4/pystoned/data/41Firm.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/data/abatementCost.csv` & `pystoned-0.6.4/pystoned/data/abatementCost.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/data/electricityFirms.csv` & `pystoned-0.6.4/pystoned/data/electricityFirms.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/data/riceProduction.csv` & `pystoned-0.6.4/pystoned/data/riceProduction.csv`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/dataset.py` & `pystoned-0.6.4/pystoned/dataset.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/pCNLS.py` & `pystoned-0.6.4/pystoned/pCNLS.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/pCQER.py` & `pystoned-0.6.4/pystoned/pCQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/pICQER.py` & `pystoned-0.6.4/pystoned/pICQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/plot.py` & `pystoned-0.6.4/pystoned/plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # import dependencies
 import matplotlib.pyplot as plt
 import numpy as np
 from .utils import interpolation
-from .constant import FUN_PROD, FUN_COST, RED_MOM
+from .constant import FUN_PROD, FUN_COST, RED_MOM, RTS_VRS, RTS_CRS
 
 
 def plot2d(model, x_select=0, label_name="estimated function", fig_name=None, method=RED_MOM):
     """Plot 2d estimated function/frontier
 
     Args:
         model: The input model for plotting.
@@ -67,16 +67,18 @@
         fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.       
         fig_name (String, optional): The name of figure to save. Defaults to None.
         line_transparent (bool, optional): control the transparency of the lines. Defaults to False.
         pane_transparent (bool, optional): control the transparency of the pane. Defaults to False.
     """
     x = np.array(model.x).T
     y = np.array(model.y).T
-    alpha = model.get_alpha()
-    beta = model.get_beta()
+    if model.rts == RTS_VRS:
+        alpha, beta = model.get_alpha(), model.get_beta()
+    elif model.rts == RTS_CRS:
+        alpha, beta = np.zeros((model.get_beta()).shape[0]), model.get_beta()
     if y.ndim != 1:
         print("Plot with mutiple y is unavailable now.")
         return False
 
     fig = plt.figure()
     ax = fig.add_subplot(projection='3d')
     dp = ax.scatter(x[x_select_1], x[x_select_2], y, marker='.', s=10)
@@ -107,15 +109,15 @@
     for i in range(len(XX)):
         for j in range(len(XX)):
             ZZ[i, j] = interpolation.interpolation(alpha, beta,
                                                    x=np.array(
                                                        [XX[i, j], YY[i, j]], ndmin=2),
                                                    fun=model.fun)
 
-    fl = ax.plot_surface(XX, YY, ZZ, rstride=1, cstride=1, cmap='viridis',
+    ax.plot_surface(XX, YY, ZZ, rstride=1, cstride=1, cmap='viridis',
                          edgecolor='none', alpha=0.5)
 
     # add x, y, z label
     ax.set_xlabel("Input $x1$")
     ax.set_ylabel("Input $x2$")
     ax.set_zlabel("Output $y$", rotation=0)
```

### Comparing `pystoned-0.6.3/pystoned/sCQER.py` & `pystoned-0.6.4/pystoned/sCQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/CNLSG1.py` & `pystoned-0.6.4/pystoned/utils/CNLSG1.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/CNLSG2.py` & `pystoned-0.6.4/pystoned/utils/CNLSG2.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/CNLSZG1.py` & `pystoned-0.6.4/pystoned/utils/CNLSZG1.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/CNLSZG2.py` & `pystoned-0.6.4/pystoned/utils/CNLSZG2.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/CQERG1.py` & `pystoned-0.6.4/pystoned/utils/CQERG1.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/CQERG2.py` & `pystoned-0.6.4/pystoned/utils/CQERG2.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/CQERZG1.py` & `pystoned-0.6.4/pystoned/utils/CQERZG1.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/CQERZG2.py` & `pystoned-0.6.4/pystoned/utils/CQERZG2.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/interpolation.py` & `pystoned-0.6.4/pystoned/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/sweet.py` & `pystoned-0.6.4/pystoned/utils/sweet.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/utils/tools.py` & `pystoned-0.6.4/pystoned/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/wCNLS.py` & `pystoned-0.6.4/pystoned/wCNLS.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/wCQER.py` & `pystoned-0.6.4/pystoned/wCQER.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned/weakCNLS.py` & `pystoned-0.6.4/pystoned/weakCNLS.py`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/pystoned.egg-info/PKG-INFO` & `pystoned-0.6.4/pystoned.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystoned
-Version: 0.6.3
+Version: 0.6.4
 Summary: A Python Package for Convex Regression and Frontier Estimation
 Home-page: https://github.com/ds2010/pyStoNED
 Download-URL: https://pypi.org/project/pystoned/
 Author: Sheng Dai, Yu-Hsueh Fang, Chia-Yen Lee, Timo Kuosmanen
 Author-email: sheng.dai@utu.fi
 License: GPLv3
 Keywords: StoNED,CNLS,CER,CQR,Z-variables,CNLSG
```

### Comparing `pystoned-0.6.3/pystoned.egg-info/SOURCES.txt` & `pystoned-0.6.4/pystoned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystoned-0.6.3/setup.py` & `pystoned-0.6.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='pystoned',
-    version='0.6.3',
+    version='0.6.4',
     description='A Python Package for Convex Regression and Frontier Estimation',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GPLv3',
     packages=find_packages(),
     author='Sheng Dai, Yu-Hsueh Fang, Chia-Yen Lee, Timo Kuosmanen',
     author_email='sheng.dai@utu.fi',
```

