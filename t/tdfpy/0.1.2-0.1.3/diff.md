# Comparing `tmp/tdfpy-0.1.2.tar.gz` & `tmp/tdfpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdfpy-0.1.2.tar", last modified: Sun Nov 20 23:06:46 2022, max compression
+gzip compressed data, was "tdfpy-0.1.3.tar", last modified: Thu Apr 13 22:18:39 2023, max compression
```

## Comparing `tdfpy-0.1.2.tar` & `tdfpy-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-11-20 23:06:46.076364 tdfpy-0.1.2/
--rw-rw-rw-   0        0        0      444 2022-11-20 23:06:46.076364 tdfpy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      728 2022-09-29 06:32:54.000000 tdfpy-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2022-11-20 23:06:46.076364 tdfpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      792 2022-11-20 22:48:11.000000 tdfpy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-20 23:06:46.060686 tdfpy-0.1.2/tdfpy/
--rw-rw-rw-   0        0        0       33 2022-09-29 01:16:01.000000 tdfpy-0.1.2/tdfpy/__init__.py
--rw-rw-rw-   0        0        0      809 2022-09-28 21:38:22.000000 tdfpy-0.1.2/tdfpy/constants.py
--rw-rw-rw-   0        0        0 13529648 2022-09-28 18:45:28.000000 tdfpy-0.1.2/tdfpy/libtimsdata.so
--rw-rw-rw-   0        0        0     3113 2022-09-29 06:07:39.000000 tdfpy-0.1.2/tdfpy/pandas_tdf.py
--rw-rw-rw-   0        0        0  2861288 2022-09-28 18:45:28.000000 tdfpy-0.1.2/tdfpy/timsdata.dll
--rw-rw-rw-   0        0        0    17699 2022-11-20 22:47:35.000000 tdfpy-0.1.2/tdfpy/timsdata.py
-drwxrwxrwx   0        0        0        0 2022-11-20 23:06:46.074253 tdfpy-0.1.2/tdfpy.egg-info/
--rw-rw-rw-   0        0        0      444 2022-11-20 23:06:46.000000 tdfpy-0.1.2/tdfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2022-11-20 23:06:46.000000 tdfpy-0.1.2/tdfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-20 23:06:46.000000 tdfpy-0.1.2/tdfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2022-11-20 23:06:46.000000 tdfpy-0.1.2/tdfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-11-20 23:06:46.000000 tdfpy-0.1.2/tdfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 22:18:39.463019 tdfpy-0.1.3/
+-rw-rw-rw-   0        0        0      444 2023-04-13 22:18:39.463019 tdfpy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      728 2022-09-29 06:32:54.000000 tdfpy-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 22:18:39.464012 tdfpy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-04-13 22:16:35.000000 tdfpy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:18:39.443880 tdfpy-0.1.3/tdfpy/
+-rw-rw-rw-   0        0        0       33 2022-09-29 01:16:01.000000 tdfpy-0.1.3/tdfpy/__init__.py
+-rw-rw-rw-   0        0        0      809 2022-09-28 21:38:22.000000 tdfpy-0.1.3/tdfpy/constants.py
+-rw-rw-rw-   0        0        0 13529648 2022-09-28 18:45:28.000000 tdfpy-0.1.3/tdfpy/libtimsdata.so
+-rw-rw-rw-   0        0        0     3176 2023-04-13 21:47:32.000000 tdfpy-0.1.3/tdfpy/pandas_tdf.py
+-rw-rw-rw-   0        0        0  2861288 2022-09-28 18:45:28.000000 tdfpy-0.1.3/tdfpy/timsdata.dll
+-rw-rw-rw-   0        0        0    18058 2023-04-13 21:52:04.000000 tdfpy-0.1.3/tdfpy/timsdata.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:18:39.459998 tdfpy-0.1.3/tdfpy.egg-info/
+-rw-rw-rw-   0        0        0      444 2023-04-13 22:18:39.000000 tdfpy-0.1.3/tdfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-04-13 22:18:39.000000 tdfpy-0.1.3/tdfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 22:18:39.000000 tdfpy-0.1.3/tdfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-13 22:18:39.000000 tdfpy-0.1.3/tdfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-13 22:18:39.000000 tdfpy-0.1.3/tdfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 22:18:39.462015 tdfpy-0.1.3/tests/
+-rw-rw-rw-   0        0        0     2422 2023-04-13 21:52:04.000000 tdfpy-0.1.3/tests/test_pandas_tdf.py
```

### Comparing `tdfpy-0.1.2/README.md` & `tdfpy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.2/tdfpy/constants.py` & `tdfpy-0.1.3/tdfpy/constants.py`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.2/tdfpy/libtimsdata.so` & `tdfpy-0.1.3/tdfpy/libtimsdata.so`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.2/tdfpy/pandas_tdf.py` & `tdfpy-0.1.3/tdfpy/pandas_tdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import sqlite3
+import logging
 from dataclasses import dataclass
-
 import pandas as pd
 
 from tdfpy.constants import TableNames
 
+logger = logging.getLogger(__name__)
+
 
-def convert_table_to_df(db:str, table_name:str) -> pd.DataFrame:
-    print(f'Fetching {table_name} from {db}')
+def convert_table_to_df(db: str, table_name: str) -> pd.DataFrame:
+    logger.debug(f'Fetching {table_name} from {db}')
     with sqlite3.connect(str(db)) as conn:
         df = pd.read_sql_query(f'SELECT * FROM {table_name}', conn)
         return df
 
 
 @dataclass
 class PandasTdf:
```

### Comparing `tdfpy-0.1.2/tdfpy/timsdata.dll` & `tdfpy-0.1.3/tdfpy/timsdata.dll`

 * *Files identical despite different names*

### Comparing `tdfpy-0.1.2/tdfpy/timsdata.py` & `tdfpy-0.1.3/tdfpy/timsdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,46 @@
+import logging
 from contextlib import contextmanager
 
 import numpy as np
 import sqlite3
 import os
 import sys
 from ctypes import *
 from enum import Enum
 
 from numpy import unicode
 
+logger = logging.getLogger(__name__)
+
+logger.debug(f'sys.platform: {sys.platform}')
 if sys.platform[:5] == "win32":
+    logger.debug('platform win32 selected')
+    data_dir = os.path.dirname(sys.modules["tdfpy"].__file__)
+    libname = 'timsdata.dll'
+    data_path = os.path.join(data_dir, libname)
+elif sys.platform[:5] == "win64":
+    logger.debug('platform: win64 selected')
     data_dir = os.path.dirname(sys.modules["tdfpy"].__file__)
     libname = 'timsdata.dll'
     data_path = os.path.join(data_dir, libname)
 elif sys.platform[:5] == "linux":
+    logger.debug('platform: linux selected')
     data_dir = os.path.dirname(sys.modules["linux64"].__file__)
     libname = 'libtimsdata.dll'
     data_path = os.path.join(data_dir, libname)
-
 else:
     raise Exception("Unsupported platform.")
 
+
+logger.debug(f'data_path: {data_path}')
 if os.path.exists(data_path):
     dll = cdll.LoadLibrary(data_path)
 else:
+    logger.debug(f'{data_path} does not exist, trying {libname}')
     dll = cdll.LoadLibrary(libname)
 
 dll.tims_open_v2.argtypes = [c_char_p, c_uint32, c_uint32]
 dll.tims_open_v2.restype = c_uint64
 dll.tims_close.argtypes = [c_uint64]
 dll.tims_close.restype = None
 dll.tims_get_last_error_string.argtypes = [c_char_p, c_uint32]
@@ -124,15 +137,15 @@
 # Convert CCS to 1/K0 for a given charge and mz
 def ccsToOneOverK0ToCCSforMz(ccs, charge, mz):
     return dll.tims_ccs_to_oneoverk0_for_mz(ccs, charge, mz)
 
 
 class PressureCompensationStrategy(Enum):
     NoPressureCompensation = 0
-    AnalyisGlobalPressureCompensation = 1
+    AnalysisGlobalPressureCompensation = 1
     PerFramePressureCompensation = 2
 
 
 class TimsData:
     def __init__(self, analysis_directory, use_recalibrated_state=False,
                  pressure_compensation_strategy=PressureCompensationStrategy.NoPressureCompensation):
 
@@ -296,15 +309,15 @@
 
         if rc == 0:
             _throwLastTimsDataError(self.dll)
 
         return result
 
     # read some "quasi profile" MS/MS spectra for a given list of precursors; returns a dict mapping
-    # 'precursor_id' to the profil arrays (intensity_values).
+    # 'precursor_id' to the profile arrays (intensity_values).
     def readPasefProfileMsMs(self, precursor_list):
         precursors_for_dll = np.array(precursor_list, dtype=np.int64)
 
         result = {}
 
         @MSMS_PROFILE_SPECTRUM_FUNCTOR
         def callback_for_dll(precursor_id, num_points, intensity_values):
@@ -317,15 +330,15 @@
 
         if rc == 0:
             _throwLastTimsDataError(self.dll)
 
         return result
 
     # read "quasi profile" MS/MS spectra for a given frame; returns a dict mapping
-    # 'precursor_id' to the profil arrays (intensity_values).
+    # 'precursor_id' to the profile arrays (intensity_values).
     def readPasefProfileMsMsForFrame(self, frame_id):
         result = {}
 
         @MSMS_PROFILE_SPECTRUM_FUNCTOR
         def callback_for_dll(precursor_id, num_points, intensity_values):
             result[precursor_id] = intensity_values[0:num_points]
 
@@ -368,15 +381,15 @@
 
         if rc == 0:
             _throwLastTimsDataError(self.dll)
 
         return result
 
     # read "quasi profile" spectra for a tims frame;
-    # returns the profil array (intensity_values).
+    # returns the profile array (intensity_values).
     def extractProfileForFrame(self, frame_id, scan_begin, scan_end):
         result = None
 
         @MSMS_PROFILE_SPECTRUM_FUNCTOR
         def callback_for_dll(precursor_id, num_points, intensity_values):
             nonlocal result
             result = intensity_values[0:num_points]
@@ -398,44 +411,42 @@
         """Efficiently extract several MS1-only extracted-ion chromatograms.
 
         The argument 'jobs' defines which chromatograms are to be extracted; it must be an iterator
         (generator) object producing a stream of ChromatogramJob objects. The jobs must be produced
         in the order of ascending 'time_begin'.
 
         The function 'trace_sink' is called for each extracted trace with three arguments: job ID,
-        numpy array of frame IDs ("x axis"), numpy array of chromatogram values ("y axis").
+        numpy array of frame IDs ("x-axis"), numpy array of chromatogram values ("y-axis").
 
         For more information, see the documentation of the C-language API of the timsdata DLL.
 
         """
 
         @CHROMATOGRAM_JOB_GENERATOR
         def wrap_gen(job, user_data):
             try:
                 job[0] = next(jobs)
                 return 1
             except StopIteration:
                 return 2
             except Exception as e:
-                # TODO: instead of printing this here, let extractChromatograms throw this
-                print("extractChromatograms: generator produced exception ", e)
+                logger.error("extractChromatograms: generator produced exception ", e)
                 return 0
 
         @CHROMATOGRAM_TRACE_SINK
         def wrap_sink(job_id, num_points, frame_ids, values, user_data):
             try:
                 trace_sink(
                     job_id,
                     np.array(frame_ids[0:num_points], dtype=np.int64),
                     np.array(values[0:num_points], dtype=np.uint64)
                 )
                 return 1
             except Exception as e:
-                # TODO: instead of printing this here, let extractChromatograms throw this
-                print("extractChromatograms: sink produced exception ", e)
+                logger.error("extractChromatograms: sink produced exception ", e)
                 return 0
 
         unused_user_data = 0
         rc = self.dll.tims_extract_chromatograms(self.handle, wrap_gen, wrap_sink, unused_user_data)
 
         if rc == 0:
             _throwLastTimsDataError(self.dll)
```

