# Comparing `tmp/htrvx-0.0.8.tar.gz` & `tmp/htrvx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htrvx-0.0.8.tar", last modified: Tue Mar  1 09:35:55 2022, max compression
+gzip compressed data, was "htrvx-0.0.9.tar", last modified: Wed Mar  9 06:39:53 2022, max compression
```

## Comparing `htrvx-0.0.8.tar` & `htrvx-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-03-01 09:35:55.705409 htrvx-0.0.8/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    35149 2021-09-01 12:22:01.000000 htrvx-0.0.8/LICENSE
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       27 2021-09-01 12:52:29.000000 htrvx-0.0.8/MANIFEST.in
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4302 2022-03-01 09:35:55.705409 htrvx-0.0.8/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3093 2022-02-23 09:42:48.000000 htrvx-0.0.8/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-03-01 09:35:55.701409 htrvx-0.0.8/htrvx/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2022-02-10 15:08:34.000000 htrvx-0.0.8/htrvx/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1761 2022-02-10 15:08:34.000000 htrvx-0.0.8/htrvx/cli.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-03-01 09:35:55.705409 htrvx-0.0.8/htrvx/schemas/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1909 2022-02-23 09:42:48.000000 htrvx-0.0.8/htrvx/schemas/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    54422 2022-02-10 15:08:34.000000 htrvx-0.0.8/htrvx/schemas/alto4.xsd
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    85745 2022-02-10 15:08:34.000000 htrvx-0.0.8/htrvx/schemas/page2019.xsd
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     6712 2022-02-25 13:46:48.000000 htrvx-0.0.8/htrvx/testing.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     6886 2022-03-01 09:29:39.000000 htrvx-0.0.8/htrvx/zones.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-03-01 09:35:55.701409 htrvx-0.0.8/htrvx.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     4302 2022-03-01 09:35:55.000000 htrvx-0.0.8/htrvx.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      354 2022-03-01 09:35:55.000000 htrvx-0.0.8/htrvx.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2022-03-01 09:35:55.000000 htrvx-0.0.8/htrvx.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       41 2022-03-01 09:35:55.000000 htrvx-0.0.8/htrvx.egg-info/entry_points.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       25 2022-03-01 09:35:55.000000 htrvx-0.0.8/htrvx.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        6 2022-03-01 09:35:55.000000 htrvx-0.0.8/htrvx.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2022-03-01 09:35:55.705409 htrvx-0.0.8/setup.cfg
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3798 2022-03-01 09:35:34.000000 htrvx-0.0.8/setup.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-03-09 06:39:53.253427 htrvx-0.0.9/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    35149 2021-09-01 12:22:01.000000 htrvx-0.0.9/LICENSE
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       27 2021-09-01 12:52:29.000000 htrvx-0.0.9/MANIFEST.in
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4391 2022-03-09 06:39:53.253427 htrvx-0.0.9/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3150 2022-03-09 06:39:27.000000 htrvx-0.0.9/README.md
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-03-09 06:39:53.249426 htrvx-0.0.9/htrvx/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2022-02-10 15:08:34.000000 htrvx-0.0.9/htrvx/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1761 2022-02-10 15:08:34.000000 htrvx-0.0.9/htrvx/cli.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-03-09 06:39:53.249426 htrvx-0.0.9/htrvx/schemas/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     1909 2022-02-23 09:42:48.000000 htrvx-0.0.9/htrvx/schemas/__init__.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    54422 2022-02-10 15:08:34.000000 htrvx-0.0.9/htrvx/schemas/alto4.xsd
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)    85745 2022-02-10 15:08:34.000000 htrvx-0.0.9/htrvx/schemas/page2019.xsd
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6712 2022-02-25 13:46:48.000000 htrvx-0.0.9/htrvx/testing.py
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     6883 2022-03-09 06:39:27.000000 htrvx-0.0.9/htrvx/zones.py
+drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2022-03-09 06:39:53.249426 htrvx-0.0.9/htrvx.egg-info/
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     4391 2022-03-09 06:39:53.000000 htrvx-0.0.9/htrvx.egg-info/PKG-INFO
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)      354 2022-03-09 06:39:53.000000 htrvx-0.0.9/htrvx.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2022-03-09 06:39:53.000000 htrvx-0.0.9/htrvx.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       41 2022-03-09 06:39:53.000000 htrvx-0.0.9/htrvx.egg-info/entry_points.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       25 2022-03-09 06:39:53.000000 htrvx-0.0.9/htrvx.egg-info/requires.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)        6 2022-03-09 06:39:53.000000 htrvx-0.0.9/htrvx.egg-info/top_level.txt
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2022-03-09 06:39:53.253427 htrvx-0.0.9/setup.cfg
+-rw-rw-r--   0 thibault  (1000) thibault  (1000)     3798 2022-03-09 06:39:34.000000 htrvx-0.0.9/setup.py
```

### Comparing `htrvx-0.0.8/LICENSE` & `htrvx-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `htrvx-0.0.8/PKG-INFO` & `htrvx-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htrvx
-Version: 0.0.8
+Version: 0.0.9
 Summary: HTRVX, HTR Validation with XSD
 Home-page: https://github.com/htr-united/htrvx
 Author: Thibault Clérice & Ariane Pinche
 License: MIT
 Description: 
         <img src="./img/htrvx.png" width=300 align=right>
         
@@ -69,14 +69,18 @@
                 pip install htrvx
             - name: Run HTRVX
               run: |
                 htrvx --verbose --group --format alto --segmonto --xsd --check-empty --raise-empty UNIX/Path/to/**/your/*.xml
         
         ```
         
+        ---
+        
+        Logo by [Alix Chagué](https://alix-tz.github.io).
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `htrvx-0.0.8/README.md` & `htrvx-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,7 +60,11 @@
         python -m pip install --upgrade pip
         pip install htrvx
     - name: Run HTRVX
       run: |
         htrvx --verbose --group --format alto --segmonto --xsd --check-empty --raise-empty UNIX/Path/to/**/your/*.xml
 
 ```
+
+---
+
+Logo by [Alix Chagué](https://alix-tz.github.io).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `htrvx-0.0.8/htrvx/cli.py` & `htrvx-0.0.9/htrvx/cli.py`

 * *Files identical despite different names*

### Comparing `htrvx-0.0.8/htrvx/schemas/__init__.py` & `htrvx-0.0.9/htrvx/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `htrvx-0.0.8/htrvx/schemas/alto4.xsd` & `htrvx-0.0.9/htrvx/schemas/alto4.xsd`

 * *Files identical despite different names*

### Comparing `htrvx-0.0.8/htrvx/schemas/page2019.xsd` & `htrvx-0.0.9/htrvx/schemas/page2019.xsd`

 * *Files identical despite different names*

### Comparing `htrvx-0.0.8/htrvx/testing.py` & `htrvx-0.0.9/htrvx/testing.py`

 * *Files identical despite different names*

### Comparing `htrvx-0.0.8/htrvx/zones.py` & `htrvx-0.0.9/htrvx/zones.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from typing import Dict, Optional, Union, Iterable, Tuple, List
 from dataclasses import dataclass
 import lxml.etree as ET
 
 SegmontoZones = frozenset(["CustomZone",
                            "DamageZone",
-                           "DecorationZone",
+                           "GraphicZone",
                            "DigitizationArtefactZone",
                            "DropCapitalZone",
                            "MainZone",
                            "MarginTextZone",
                            "MusicZone",
                            "NumberingZone",
                            "QuireMarksZone",
```

### Comparing `htrvx-0.0.8/htrvx.egg-info/PKG-INFO` & `htrvx-0.0.9/htrvx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htrvx
-Version: 0.0.8
+Version: 0.0.9
 Summary: HTRVX, HTR Validation with XSD
 Home-page: https://github.com/htr-united/htrvx
 Author: Thibault Clérice & Ariane Pinche
 License: MIT
 Description: 
         <img src="./img/htrvx.png" width=300 align=right>
         
@@ -69,14 +69,18 @@
                 pip install htrvx
             - name: Run HTRVX
               run: |
                 htrvx --verbose --group --format alto --segmonto --xsd --check-empty --raise-empty UNIX/Path/to/**/your/*.xml
         
         ```
         
+        ---
+        
+        Logo by [Alix Chagué](https://alix-tz.github.io).
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `htrvx-0.0.8/setup.py` & `htrvx-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Package meta-data.
 NAME = 'htrvx'
 DESCRIPTION = 'HTRVX, HTR Validation with XSD'
 URL = 'https://github.com/htr-united/htrvx'
 AUTHOR = 'Thibault Clérice & Ariane Pinche'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

