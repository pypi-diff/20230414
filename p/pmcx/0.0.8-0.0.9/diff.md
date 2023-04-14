# Comparing `tmp/pmcx-0.0.8-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/pmcx-0.0.9-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3460003 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat  9861632 b- defN 23-Jan-22 05:50 pmcx.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat    10158 b- defN 23-Jan-22 05:50 pmcx-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jan-22 05:50 pmcx-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jan-22 05:50 pmcx-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      377 b- defN 23-Jan-22 05:50 pmcx-0.0.8.dist-info/RECORD
-5 files, 9872279 bytes uncompressed, 3459309 bytes compressed:  65.0%
+Zip file size: 3461176 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat  9862144 b- defN 23-Feb-05 15:17 _pmcx.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    10158 b- defN 23-Feb-05 15:17 pmcx-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Feb-05 15:17 pmcx-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Feb-05 15:17 pmcx-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      378 b- defN 23-Feb-05 15:17 pmcx-0.0.9.dist-info/RECORD
+5 files, 9872793 bytes uncompressed, 3460480 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: pmcx.pypy39-pp73-win_amd64.pyd
+Filename: _pmcx.pypy39-pp73-win_amd64.pyd
 Comment: 
 
-Filename: pmcx-0.0.8.dist-info/METADATA
+Filename: pmcx-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pmcx-0.0.8.dist-info/WHEEL
+Filename: pmcx-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pmcx-0.0.8.dist-info/top_level.txt
+Filename: pmcx-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pmcx-0.0.8.dist-info/RECORD
+Filename: pmcx-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pmcx-0.0.8.dist-info/METADATA` & `pmcx-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmcx
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python bindings for Monte Carlo eXtreme photon transport simulator
 Home-page: https://github.com/fangq/mcx
 Author: Matin Raayai Ardakani, Qianqian Fang
 Author-email: raayaiardakani.m@northeastern.edu, q.fang@neu.edu
 Maintainer: Qianqian Fang
 License: GPLv3+
 Download-URL: http://mcx.space
@@ -28,15 +28,15 @@
 ![](http://mcx.space/img/mcx18_banner.png)
 
 # PMCX - Python bindings for Monte Carlo eXtreme photon transport simulator
 
 - Copyright: (C) Matin Raayai Ardakani (2022-2023) <raayaiardakani.m at northeastern.edu> 
 and Qianqian Fang (2019-2023) <q.fang at neu.edu>
 - License: GNU Public License V3 or later
-- Version: 0.0.8
+- Version: 0.0.9
 - URL: https://pypi.org/project/pmcx/
 - Github: https://github.com/fangq/mcx
 
 [![Build Status](https://travis-ci.com/fangq/mcx.svg?branch=master)](https://travis-ci.com/fangq/mcx)
 
 This module provides a Python binding for Monte Carlo eXtreme (MCX).
 For other binaries, including the standalone executable and the MATLAB bindings, see [our website](http://mcx.space).
```

