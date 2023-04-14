# Comparing `tmp/quera-ahs-utils-0.3.1.tar.gz` & `tmp/quera-ahs-utils-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quera-ahs-utils-0.3.1.tar", last modified: Thu Apr  6 11:49:47 2023, max compression
+gzip compressed data, was "quera-ahs-utils-0.3.2.tar", last modified: Fri Apr 14 15:55:55 2023, max compression
```

## Comparing `quera-ahs-utils-0.3.1.tar` & `quera-ahs-utils-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:49:47.028128 quera-ahs-utils-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-06 11:49:47.028128 quera-ahs-utils-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-06 11:49:47.028128 quera-ahs-utils-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:49:47.024128 quera-ahs-utils-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:49:47.028128 quera-ahs-utils-0.3.1/src/quera_ahs_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:49:47.028128 quera-ahs-utils-0.3.1/src/quera_ahs_utils/quera_ir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/quera_ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/quera_ir/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/quera_ir/task_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils/quera_ir/task_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:49:47.028128 quera-ahs-utils-0.3.1/src/quera_ahs_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-06 11:49:47.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-06 11:49:47.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:49:47.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-06 11:49:47.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 11:49:47.000000 quera-ahs-utils-0.3.1/src/quera_ahs_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:49:47.028128 quera-ahs-utils-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/test/test_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/test/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/test/test_parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-06 11:48:51.000000 quera-ahs-utils-0.3.1/test/test_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.692035 quera-ahs-utils-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-14 15:55:55.692035 quera-ahs-utils-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-14 15:55:55.692035 quera-ahs-utils-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.688035 quera-ahs-utils-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.688035 quera-ahs-utils-0.3.2/src/quera_ahs_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.692035 quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/task_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/task_specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.688035 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-14 15:55:55.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 15:55:55.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:55:55.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 15:55:55.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 15:55:55.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.692035 quera-ahs-utils-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/test/test_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/test/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/test/test_parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/test/test_plotting.py
```

### Comparing `quera-ahs-utils-0.3.1/LICENSE` & `quera-ahs-utils-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/PKG-INFO` & `quera-ahs-utils-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
 Home-page: https://github.com/QuEraComputing/quera-ahs-utils
 Author: QuEra Computing Inc. + Braket Science Team
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
```

### Comparing `quera-ahs-utils-0.3.1/README.md` & `quera-ahs-utils-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/pyproject.toml` & `quera-ahs-utils-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quera-ahs-utils"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
 ]
 maintainers = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
```

### Comparing `quera-ahs-utils-0.3.1/setup.cfg` & `quera-ahs-utils-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/src/quera_ahs_utils/analysis.py` & `quera-ahs-utils-0.3.2/src/quera_ahs_utils/analysis.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/src/quera_ahs_utils/drive.py` & `quera-ahs-utils-0.3.2/src/quera_ahs_utils/drive.py`

 * *Files 5% similar despite different names*

```diff
@@ -291,34 +291,45 @@
     """            
     shift = shift_list[0]
     for sf in shift_list[1:]:
         shift = concatenate_shifts(shift, sf)
     return shift
 
 
-def slice_time_series(time_series: TimeSeries, first: float, last: float, piecewise_constant=False):
+def slice_time_series(time_series: TimeSeries, first: float, last: float, piecewise_constant=False, min_time_step: float = 0.0):
     """Obtain a sub-section of a TimeSeries between times `first` and `last`
 
         Args:
             time_series (TimeSeries): The time series to slice
             first (float): Lower bound of the slicing region
             last (float): Upper bound of the slicing region
             piecewise_constant (bool, optional): Flag to use piecewise constant interpolation to get 
                 end points of slice, otherwise use piecewise linear interpolation. Defaults to False.
+            min_time_step (float): Check if the slice will fall too close to the value the input time series.
+                default value is 0.
                 
         Returns:
             TimeSeries: The resulting time series after slicing. 
+            
+        Raises: ValueError
+            When the sliced time series will have a time-step smaller than `min_time_step`. 
     """
     times = np.array(time_series.times())    
     values = np.array(time_series.values())
     
     assert first < last
     assert first >= 0
     assert last <= times[-1]
     
+    if np.any((times[times > first] - first) < min_time_step):
+        raise ValueError("first time step too close to existing time-point.")
+    
+    if np.any((times[times > last] - last) < min_time_step):
+        raise ValueError("first time step too close to existing time-point.")
+    
     first_index = np.searchsorted(times,first)
     last_index = np.searchsorted(times,last)
 
     first_value = get_time_series_value(time_series, first, piecewise_constant=piecewise_constant)
     last_value  = get_time_series_value(time_series, last, piecewise_constant=piecewise_constant)
 
     new_time_series = TimeSeries()
@@ -330,43 +341,43 @@
     for time,value in zip(inter_times,inter_values):
         new_time_series.put(time-first,value)
         
     new_time_series.put((last-first),last_value)
     
     return new_time_series
 
-def slice_drive(drive: DrivingField, first: float, last: float) -> DrivingField:
+def slice_drive(drive: DrivingField, first: float, last: float, min_time_step: float=0.0) -> DrivingField:
     """Obtain a sub-section of a driving field between times `first` and `last`
 
         Args:
             drive (DrivingField): The driving field object to be sliced. 
             first (float): Lower bound of the slice. 
             last (float): Upper bound of the slice.
 
         Returns:
             DrivingField: The resulting driving field after slicing
     """
     return DrivingField(
-        amplitude=slice_time_series(drive.amplitude.time_series, first, last),
-        detuning=slice_time_series(drive.detuning.time_series, first, last),
-        phase=slice_time_series(drive.phase.time_series, first, last, piecewise_constant=True)
+        amplitude=slice_time_series(drive.amplitude.time_series, first, last, min_time_step=min_time_step),
+        detuning=slice_time_series(drive.detuning.time_series, first, last, min_time_step=min_time_step),
+        phase=slice_time_series(drive.phase.time_series, first, last, piecewise_constant=True, min_time_step=min_time_step)
     )
     
-def slice_shift(shift: ShiftingField, first: float, last: float) -> ShiftingField:
+def slice_shift(shift: ShiftingField, first: float, last: float, min_time_step: float = 0.0) -> ShiftingField:
     """Obtain a sub-section of shifting field begin times `first` and `last`
 
     Args:
         shift (ShiftingField): The shifting field object to be sliced
         first (float): Lower bound of the slice. 
         last (float): Upper bound of the slice. 
 
     Returns:
         ShiftingField: The resulting shifting field after slicing. 
     """
-    new_time_series = slice_time_series(shift.magnitude.time_series, first, last)
+    new_time_series = slice_time_series(shift.magnitude.time_series, first, last, min_time_step=min_time_step)
     return ShiftingField(Field(new_time_series, shift.magnitude.pattern))
 
 
 def adiabatic_drive(
         t_ramp_up: float,
         t_ramp_down: float,
         t_sweep: float,
```

### Comparing `quera-ahs-utils-0.3.1/src/quera_ahs_utils/ir.py` & `quera-ahs-utils-0.3.2/src/quera_ahs_utils/ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/src/quera_ahs_utils/parallelize.py` & `quera-ahs-utils-0.3.2/src/quera_ahs_utils/parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/src/quera_ahs_utils/plotting.py` & `quera-ahs-utils-0.3.2/src/quera_ahs_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/src/quera_ahs_utils/quera_ir/capabilities.py` & `quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/capabilities.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/src/quera_ahs_utils/quera_ir/task_results.py` & `quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/task_results.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/src/quera_ahs_utils/quera_ir/task_specification.py` & `quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/task_specification.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/src/quera_ahs_utils.egg-info/PKG-INFO` & `quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.3.1
+Version: 0.3.2
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
 Home-page: https://github.com/QuEraComputing/quera-ahs-utils
 Author: QuEra Computing Inc. + Braket Science Team
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
```

### Comparing `quera-ahs-utils-0.3.1/src/quera_ahs_utils.egg-info/SOURCES.txt` & `quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/test/test_drive.py` & `quera-ahs-utils-0.3.2/test/test_drive.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/test/test_ir.py` & `quera-ahs-utils-0.3.2/test/test_ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/test/test_parallelize.py` & `quera-ahs-utils-0.3.2/test/test_parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.1/test/test_plotting.py` & `quera-ahs-utils-0.3.2/test/test_plotting.py`

 * *Files identical despite different names*

