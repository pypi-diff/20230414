# Comparing `tmp/pyroscopegridding-0.0.1.tar.gz` & `tmp/pyroscopegridding-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroscopegridding-0.0.1.tar", last modified: Fri Apr 14 15:18:47 2023, max compression
+gzip compressed data, was "dist/pyroscopegridding-0.0.2.tar", last modified: Fri Apr 14 15:20:13 2023, max compression
```

## Comparing `pyroscopegridding-0.0.1.tar` & `pyroscopegridding-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:18:47.592259 pyroscopegridding-0.0.1/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 15:18:47.588025 pyroscopegridding-0.0.1/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.0.1/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:18:47.371321 pyroscopegridding-0.0.1/pyroscopegridding/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2022-02-04 10:40:28.000000 pyroscopegridding-0.0.1/pyroscopegridding/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     2636 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.1/pyroscopegridding/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10387 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.1/pyroscopegridding/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33637 2023-04-14 14:32:01.000000 pyroscopegridding-0.0.1/pyroscopegridding/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10462 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.1/pyroscopegridding/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26242 2023-04-14 15:03:08.000000 pyroscopegridding-0.0.1/pyroscopegridding/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9309 2023-04-14 14:25:01.000000 pyroscopegridding-0.0.1/pyroscopegridding/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.1/pyroscopegridding/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10932 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.1/pyroscopegridding/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     4779 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.1/pyroscopegridding/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:18:47.551430 pyroscopegridding-0.0.1/pyroscopegridding.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 15:18:46.000000 pyroscopegridding-0.0.1/pyroscopegridding.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-14 15:18:46.000000 pyroscopegridding-0.0.1/pyroscopegridding.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-14 15:18:46.000000 pyroscopegridding-0.0.1/pyroscopegridding.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       71 2023-04-14 15:18:46.000000 pyroscopegridding-0.0.1/pyroscopegridding.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       54 2023-04-14 15:18:46.000000 pyroscopegridding-0.0.1/pyroscopegridding.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-14 15:18:46.000000 pyroscopegridding-0.0.1/pyroscopegridding.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-14 15:18:47.594260 pyroscopegridding-0.0.1/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1763 2023-04-14 15:18:39.000000 pyroscopegridding-0.0.1/setup.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:20:13.579505 pyroscopegridding-0.0.2/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 15:20:13.572507 pyroscopegridding-0.0.2/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegridding-0.0.2/README.md
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:20:13.257817 pyroscopegridding-0.0.2/pyroscopegridding/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2022-02-04 10:40:28.000000 pyroscopegridding-0.0.2/pyroscopegridding/__init__.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     2636 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.2/pyroscopegridding/fileparser.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10387 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.2/pyroscopegridding/filter_data.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    33637 2023-04-14 14:32:01.000000 pyroscopegridding-0.0.2/pyroscopegridding/grid_ncf.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10462 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.2/pyroscopegridding/gridding.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26242 2023-04-14 15:03:08.000000 pyroscopegridding-0.0.2/pyroscopegridding/gtools.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9309 2023-04-14 14:25:01.000000 pyroscopegridding-0.0.2/pyroscopegridding/naming_conventions.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    14116 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.2/pyroscopegridding/sat_data_input.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10932 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.2/pyroscopegridding/solar_zenith.py
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     4779 2023-04-14 14:22:50.000000 pyroscopegridding-0.0.2/pyroscopegridding/time_conv.py
+drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-04-14 15:20:13.516664 pyroscopegridding-0.0.2/pyroscopegridding.egg-info/
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      773 2023-04-14 15:20:12.000000 pyroscopegridding-0.0.2/pyroscopegridding.egg-info/PKG-INFO
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      590 2023-04-14 15:20:12.000000 pyroscopegridding-0.0.2/pyroscopegridding.egg-info/SOURCES.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-04-14 15:20:12.000000 pyroscopegridding-0.0.2/pyroscopegridding.egg-info/dependency_links.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       71 2023-04-14 15:20:12.000000 pyroscopegridding-0.0.2/pyroscopegridding.egg-info/entry_points.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       49 2023-04-14 15:20:12.000000 pyroscopegridding-0.0.2/pyroscopegridding.egg-info/requires.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       18 2023-04-14 15:20:12.000000 pyroscopegridding-0.0.2/pyroscopegridding.egg-info/top_level.txt
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-04-14 15:20:13.580732 pyroscopegridding-0.0.2/setup.cfg
+-rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1764 2023-04-14 15:19:45.000000 pyroscopegridding-0.0.2/setup.py
```

### Comparing `pyroscopegridding-0.0.1/PKG-INFO` & `pyroscopegridding-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.0.1/README.md` & `pyroscopegridding-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding/fileparser.py` & `pyroscopegridding-0.0.2/pyroscopegridding/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding/filter_data.py` & `pyroscopegridding-0.0.2/pyroscopegridding/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding/grid_ncf.py` & `pyroscopegridding-0.0.2/pyroscopegridding/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding/gridding.py` & `pyroscopegridding-0.0.2/pyroscopegridding/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding/gtools.py` & `pyroscopegridding-0.0.2/pyroscopegridding/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding/naming_conventions.py` & `pyroscopegridding-0.0.2/pyroscopegridding/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding/sat_data_input.py` & `pyroscopegridding-0.0.2/pyroscopegridding/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding/solar_zenith.py` & `pyroscopegridding-0.0.2/pyroscopegridding/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding/time_conv.py` & `pyroscopegridding-0.0.2/pyroscopegridding/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding.egg-info/PKG-INFO` & `pyroscopegridding-0.0.2/pyroscopegridding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyroscopegridding
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: data fusion,satellite,L2,L3
```

### Comparing `pyroscopegridding-0.0.1/pyroscopegridding.egg-info/SOURCES.txt` & `pyroscopegridding-0.0.2/pyroscopegridding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegridding-0.0.1/setup.py` & `pyroscopegridding-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Data fusion package for satellite data transformation.'
 LONG_DESCRIPTION = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data.'
 
 # Setting up
 setup(
     name = 'pyroscopegridding',         # Package name
     packages = ['pyroscopegridding'],   
-    version = '0.0.1',      # Initial version
+    version = '0.0.2',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
     keywords = ['data fusion', 'satellite', 'L2', 'L3'],   # Keywords
     #packages = find_packages(),
@@ -22,15 +22,15 @@
         'console_scripts': [
             'pyroscopegridtools = pyroscopegridtools.gtools:main'
         ]
     },
     install_requires=[            
             'numpy',
             'joblib',
-            'cuda',
+            #'cuda',
             'netCDF4',
             'pyhdf',
             'pyyaml',
             'numba',
             'argparse'
         ],
     classifiers=[
```

