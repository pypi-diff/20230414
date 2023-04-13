# Comparing `tmp/tdfpy-0.1.5.tar.gz` & `tmp/tdfpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdfpy-0.1.5.tar", last modified: Thu Apr 13 22:27:15 2023, max compression
+gzip compressed data, was "tdfpy-0.1.6.tar", last modified: Thu Apr 13 22:36:04 2023, max compression
```

## Comparing `tdfpy-0.1.5.tar` & `tdfpy-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 22:27:15.678462 tdfpy-0.1.5/
--rw-rw-rw-   0        0        0      444 2023-04-13 22:27:15.677456 tdfpy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      728 2022-09-29 06:32:54.000000 tdfpy-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 22:27:15.678462 tdfpy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-04-13 22:26:52.000000 tdfpy-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:27:15.664905 tdfpy-0.1.5/tdfpy/
--rw-rw-rw-   0        0        0       33 2022-09-29 01:16:01.000000 tdfpy-0.1.5/tdfpy/__init__.py
--rw-rw-rw-   0        0        0      809 2022-09-28 21:38:22.000000 tdfpy-0.1.5/tdfpy/constants.py
--rw-rw-rw-   0        0        0 13529648 2022-09-28 18:45:28.000000 tdfpy-0.1.5/tdfpy/libtimsdata.so
--rw-rw-rw-   0        0        0     3176 2023-04-13 21:47:32.000000 tdfpy-0.1.5/tdfpy/pandas_tdf.py
--rw-rw-rw-   0        0        0  2861288 2022-09-28 18:45:28.000000 tdfpy-0.1.5/tdfpy/timsdata.dll
--rw-rw-rw-   0        0        0    18058 2023-04-13 21:52:04.000000 tdfpy-0.1.5/tdfpy/timsdata.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:27:15.676456 tdfpy-0.1.5/tdfpy.egg-info/
--rw-rw-rw-   0        0        0      444 2023-04-13 22:27:15.000000 tdfpy-0.1.5/tdfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-04-13 22:27:15.000000 tdfpy-0.1.5/tdfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 22:27:15.000000 tdfpy-0.1.5/tdfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-13 22:27:15.000000 tdfpy-0.1.5/tdfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 22:27:15.000000 tdfpy-0.1.5/tdfpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 22:27:15.677456 tdfpy-0.1.5/tests/
--rw-rw-rw-   0        0        0     2422 2023-04-13 21:52:04.000000 tdfpy-0.1.5/tests/test_pandas_tdf.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:36:04.819662 tdfpy-0.1.6/
+-rw-rw-rw-   0        0        0      444 2023-04-13 22:36:04.818663 tdfpy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      728 2022-09-29 06:32:54.000000 tdfpy-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 22:36:04.819662 tdfpy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-04-13 22:35:35.000000 tdfpy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:36:04.803662 tdfpy-0.1.6/tdfpy/
+-rw-rw-rw-   0        0        0       33 2022-09-29 01:16:01.000000 tdfpy-0.1.6/tdfpy/__init__.py
+-rw-rw-rw-   0        0        0      809 2022-09-28 21:38:22.000000 tdfpy-0.1.6/tdfpy/constants.py
+-rw-rw-rw-   0        0        0 13529648 2022-09-28 18:45:28.000000 tdfpy-0.1.6/tdfpy/libtimsdata.so
+-rw-rw-rw-   0        0        0     3176 2023-04-13 21:47:32.000000 tdfpy-0.1.6/tdfpy/pandas_tdf.py
+-rw-rw-rw-   0        0        0  2861288 2022-09-28 18:45:28.000000 tdfpy-0.1.6/tdfpy/timsdata.dll
+-rw-rw-rw-   0        0        0    17796 2023-04-13 22:34:53.000000 tdfpy-0.1.6/tdfpy/timsdata.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:36:04.815662 tdfpy-0.1.6/tdfpy.egg-info/
+-rw-rw-rw-   0        0        0      444 2023-04-13 22:36:04.000000 tdfpy-0.1.6/tdfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-04-13 22:36:04.000000 tdfpy-0.1.6/tdfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 22:36:04.000000 tdfpy-0.1.6/tdfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-13 22:36:04.000000 tdfpy-0.1.6/tdfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 22:36:04.000000 tdfpy-0.1.6/tdfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 22:36:04.818663 tdfpy-0.1.6/tests/
+-rw-rw-rw-   0        0        0     2418 2023-04-13 22:31:01.000000 tdfpy-0.1.6/tests/test_pandas_tdf.py
+-rw-rw-rw-   0        0        0      269 2023-04-13 22:33:37.000000 tdfpy-0.1.6/tests/test_timsdata.py
```

### Comparing `tdfpy-0.1.5/README.md` & `tdfpy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.5/setup.py` & `tdfpy-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 setup(
     name='tdfpy',
-    version='0.1.5',
+    version='0.1.6',
     description='Pip package to work with bruker tdf and tdf_bin files',
     url='https://github.com/pgarrett-scripps/tdfpy',
     author='Patrick Garrett',
     author_email='pgarrett@scripps.edu',
     license='MIT',
     packages=['tdfpy'],
     package_dir={'tdfpy': 'tdfpy'},
     include_package_data=True,
     package_data={'tdfpy': ['timsdata.dll', 'libtimsdata.so']},
-    install_requires=['pandas~=2.0.0',
-                      'numpy~=1.24.2',
+    install_requires=['numpy~=1.24.2',
+                      'pandas~=2.0.0',
                       ],
 
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3.10',
```

### Comparing `tdfpy-0.1.5/tdfpy/constants.py` & `tdfpy-0.1.6/tdfpy/constants.py`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.5/tdfpy/libtimsdata.so` & `tdfpy-0.1.6/tdfpy/libtimsdata.so`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.5/tdfpy/pandas_tdf.py` & `tdfpy-0.1.6/tdfpy/pandas_tdf.py`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.5/tdfpy/timsdata.dll` & `tdfpy-0.1.6/tdfpy/timsdata.dll`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.5/tdfpy/timsdata.py` & `tdfpy-0.1.6/tdfpy/timsdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import numpy as np
 import sqlite3
 import os
 import sys
 from ctypes import *
 from enum import Enum
 
-from numpy import unicode
-
 logger = logging.getLogger(__name__)
 
 logger.debug(f'sys.platform: {sys.platform}')
 if sys.platform[:5] == "win32":
     logger.debug('platform win32 selected')
     data_dir = os.path.dirname(sys.modules["tdfpy"].__file__)
     libname = 'timsdata.dll'
@@ -145,20 +143,16 @@
     PerFramePressureCompensation = 2
 
 
 class TimsData:
     def __init__(self, analysis_directory, use_recalibrated_state=False,
                  pressure_compensation_strategy=PressureCompensationStrategy.NoPressureCompensation):
 
-        if sys.version_info.major == 2:
-            if not isinstance(analysis_directory, unicode):
-                raise ValueError("analysis_directory must be a Unicode string.")
-        if sys.version_info.major == 3:
-            if not isinstance(analysis_directory, str):
-                raise ValueError("analysis_directory must be a string.")
+        if not isinstance(analysis_directory, str):
+            raise ValueError("analysis_directory must be a string.")
 
         self.dll = dll
 
         self.handle = self.dll.tims_open_v2(
             analysis_directory.encode('utf-8'),
             1 if use_recalibrated_state else 0,
             pressure_compensation_strategy.value)
```

### Comparing `tdfpy-0.1.5/tests/test_pandas_tdf.py` & `tdfpy-0.1.6/tests/test_pandas_tdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 
 from tdfpy.pandas_tdf import PandasTdf
 
 TDF_PATH = r'200ngHeLaPASEF_1min.d\analysis.tdf'
 
 
-class TestStringMethods(unittest.TestCase):
+class TestPandasTDF(unittest.TestCase):
     pd_tdf = PandasTdf(TDF_PATH)
 
     def test_calibration_info(self):
         self.assertTrue(isinstance(self.pd_tdf.calibration_info, pd.DataFrame))
 
     def test_dia_frame_msms_info(self):
         self.assertTrue(isinstance(self.pd_tdf.dia_frame_msms_info, pd.DataFrame))
```

