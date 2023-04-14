# Comparing `tmp/raster-tools-0.1.2.tar.gz` & `tmp/raster-tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster-tools-0.1.2.tar", last modified: Fri Apr  7 23:46:37 2023, max compression
+gzip compressed data, was "raster-tools-0.1.3.tar", last modified: Fri Apr 14 00:14:01 2023, max compression
```

## Comparing `raster-tools-0.1.2.tar` & `raster-tools-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-07 23:46:37.268363 raster-tools-0.1.2/
--rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster-tools-0.1.2/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)      316 2022-08-26 20:44:14.000000 raster-tools-0.1.2/MANIFEST.in
--rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-07 23:46:37.268363 raster-tools-0.1.2/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2023-04-01 01:01:01.000000 raster-tools-0.1.2/README.md
--rw-r--r--   0 fred      (1000) fred      (1000)      273 2022-08-26 20:44:14.000000 raster-tools-0.1.2/pyproject.toml
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-07 23:46:37.264363 raster-tools-0.1.2/raster_tools/
--rw-rw-r--   0 fred      (1000) fred      (1000)      934 2023-01-25 21:30:15.000000 raster-tools-0.1.2/raster_tools/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)      383 2023-01-28 03:26:22.000000 raster-tools-0.1.2/raster_tools/_compat.py
--rw-rw-r--   0 fred      (1000) fred      (1000)       22 2023-04-07 23:45:46.000000 raster-tools-0.1.2/raster_tools/_version.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7664 2023-01-04 22:54:45.000000 raster-tools-0.1.2/raster_tools/batch.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6536 2023-02-01 01:11:45.000000 raster-tools-0.1.2/raster_tools/clipping.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9647 2023-03-29 17:25:11.000000 raster-tools-0.1.2/raster_tools/creation.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1286 2022-11-29 01:39:49.000000 raster-tools-0.1.2/raster_tools/dask_utils.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-07 23:46:37.264363 raster-tools-0.1.2/raster_tools/distance/
--rw-r--r--   0 fred      (1000) fred      (1000)      427 2022-08-26 20:44:16.000000 raster-tools-0.1.2/raster_tools/distance/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6777 2022-10-21 23:01:50.000000 raster-tools-0.1.2/raster_tools/distance/_heap.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    26495 2023-01-04 22:54:45.000000 raster-tools-0.1.2/raster_tools/distance/cost_distance.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    34820 2023-04-06 23:13:37.000000 raster-tools-0.1.2/raster_tools/distance/proximity.py
--rw-r--r--   0 fred      (1000) fred      (1000)     3240 2022-12-09 03:28:15.000000 raster-tools-0.1.2/raster_tools/dtypes.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20687 2023-03-03 21:13:40.000000 raster-tools-0.1.2/raster_tools/focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    35260 2023-01-04 22:54:45.000000 raster-tools-0.1.2/raster_tools/general.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7149 2023-01-04 22:54:45.000000 raster-tools-0.1.2/raster_tools/io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12275 2023-02-15 02:21:21.000000 raster-tools-0.1.2/raster_tools/line_stats.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2123 2022-10-22 00:44:28.000000 raster-tools-0.1.2/raster_tools/masking.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    46733 2023-04-07 23:46:08.000000 raster-tools-0.1.2/raster_tools/raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4076 2022-10-21 23:01:50.000000 raster-tools-0.1.2/raster_tools/stat_common.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    17964 2023-03-31 23:07:40.000000 raster-tools-0.1.2/raster_tools/surface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3163 2023-02-15 02:21:21.000000 raster-tools-0.1.2/raster_tools/utils.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    30306 2023-04-07 23:46:08.000000 raster-tools-0.1.2/raster_tools/vector.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20196 2023-04-06 21:19:23.000000 raster-tools-0.1.2/raster_tools/zonal.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-07 23:46:37.264363 raster-tools-0.1.2/raster_tools.egg-info/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-07 23:46:37.000000 raster-tools-0.1.2/raster_tools.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1774 2023-04-07 23:46:37.000000 raster-tools-0.1.2/raster_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2023-04-07 23:46:37.000000 raster-tools-0.1.2/raster_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-04-07 23:46:37.000000 raster-tools-0.1.2/raster_tools.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       13 2023-04-07 23:46:37.000000 raster-tools-0.1.2/raster_tools.egg-info/top_level.txt
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-07 23:46:37.264363 raster-tools-0.1.2/requirements/
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-01-25 21:30:15.000000 raster-tools-0.1.2/requirements/default.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2023-04-07 23:46:37.268363 raster-tools-0.1.2/setup.cfg
--rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2023-01-31 00:50:40.000000 raster-tools-0.1.2/setup.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-07 23:46:37.268363 raster-tools-0.1.2/tests/
--rw-rw-r--   0 fred      (1000) fred      (1000)     4072 2023-01-04 22:54:46.000000 raster-tools-0.1.2/tests/test_clipping.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7404 2023-01-04 22:54:46.000000 raster-tools-0.1.2/tests/test_distance.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1297 2022-08-26 20:44:16.000000 raster-tools-0.1.2/tests/test_distance__heap.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     8212 2023-04-06 23:11:34.000000 raster-tools-0.1.2/tests/test_distance_proximity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20233 2023-03-03 21:13:40.000000 raster-tools-0.1.2/tests/test_focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    22392 2023-02-01 19:59:47.000000 raster-tools-0.1.2/tests/test_general.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7288 2023-01-28 03:48:27.000000 raster-tools-0.1.2/tests/test_line_stats.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    55226 2023-02-16 01:34:06.000000 raster-tools-0.1.2/tests/test_raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4124 2022-08-26 20:44:16.000000 raster-tools-0.1.2/tests/test_stat_common.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5157 2023-02-15 02:21:21.000000 raster-tools-0.1.2/tests/test_surface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10830 2023-01-25 02:09:19.000000 raster-tools-0.1.2/tests/test_vector.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6903 2023-04-06 20:45:48.000000 raster-tools-0.1.2/tests/test_zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/
+-rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster-tools-0.1.3/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)      316 2022-08-26 20:44:14.000000 raster-tools-0.1.3/MANIFEST.in
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-14 00:14:01.282053 raster-tools-0.1.3/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2023-04-11 21:45:35.000000 raster-tools-0.1.3/README.md
+-rw-r--r--   0 fred      (1000) fred      (1000)      273 2022-08-26 20:44:14.000000 raster-tools-0.1.3/pyproject.toml
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/raster_tools/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      934 2023-01-25 21:30:15.000000 raster-tools-0.1.3/raster_tools/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)      383 2023-01-28 03:26:22.000000 raster-tools-0.1.3/raster_tools/_compat.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)       22 2023-04-14 00:12:51.000000 raster-tools-0.1.3/raster_tools/_version.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7664 2023-01-04 22:54:45.000000 raster-tools-0.1.3/raster_tools/batch.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6536 2023-02-01 01:11:45.000000 raster-tools-0.1.3/raster_tools/clipping.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9647 2023-03-29 17:25:11.000000 raster-tools-0.1.3/raster_tools/creation.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1286 2022-11-29 01:39:49.000000 raster-tools-0.1.3/raster_tools/dask_utils.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/raster_tools/distance/
+-rw-r--r--   0 fred      (1000) fred      (1000)      427 2022-08-26 20:44:16.000000 raster-tools-0.1.3/raster_tools/distance/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6777 2022-10-21 23:01:50.000000 raster-tools-0.1.3/raster_tools/distance/_heap.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    26495 2023-01-04 22:54:45.000000 raster-tools-0.1.3/raster_tools/distance/cost_distance.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    34940 2023-04-13 22:25:41.000000 raster-tools-0.1.3/raster_tools/distance/proximity.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3240 2022-12-09 03:28:15.000000 raster-tools-0.1.3/raster_tools/dtypes.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20687 2023-03-03 21:13:40.000000 raster-tools-0.1.3/raster_tools/focal.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    35261 2023-04-11 22:00:22.000000 raster-tools-0.1.3/raster_tools/general.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7149 2023-01-04 22:54:45.000000 raster-tools-0.1.3/raster_tools/io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12275 2023-02-15 02:21:21.000000 raster-tools-0.1.3/raster_tools/line_stats.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2123 2022-10-22 00:44:28.000000 raster-tools-0.1.3/raster_tools/masking.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    46873 2023-04-11 21:59:29.000000 raster-tools-0.1.3/raster_tools/raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4076 2022-10-21 23:01:50.000000 raster-tools-0.1.3/raster_tools/stat_common.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    17964 2023-03-31 23:07:40.000000 raster-tools-0.1.3/raster_tools/surface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3163 2023-02-15 02:21:21.000000 raster-tools-0.1.3/raster_tools/utils.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    26731 2023-04-14 00:13:27.000000 raster-tools-0.1.3/raster_tools/vector.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20196 2023-04-06 21:19:23.000000 raster-tools-0.1.3/raster_tools/zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/raster_tools.egg-info/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-14 00:14:01.000000 raster-tools-0.1.3/raster_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1774 2023-04-14 00:14:01.000000 raster-tools-0.1.3/raster_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)        1 2023-04-14 00:14:01.000000 raster-tools-0.1.3/raster_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-04-14 00:14:01.000000 raster-tools-0.1.3/raster_tools.egg-info/requires.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       13 2023-04-14 00:14:01.000000 raster-tools-0.1.3/raster_tools.egg-info/top_level.txt
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/requirements/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-01-25 21:30:15.000000 raster-tools-0.1.3/requirements/default.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       38 2023-04-14 00:14:01.282053 raster-tools-0.1.3/setup.cfg
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2023-01-31 00:50:40.000000 raster-tools-0.1.3/setup.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/tests/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4072 2023-01-04 22:54:46.000000 raster-tools-0.1.3/tests/test_clipping.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7404 2023-01-04 22:54:46.000000 raster-tools-0.1.3/tests/test_distance.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1297 2022-08-26 20:44:16.000000 raster-tools-0.1.3/tests/test_distance__heap.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8212 2023-04-14 00:09:55.000000 raster-tools-0.1.3/tests/test_distance_proximity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20233 2023-03-03 21:13:40.000000 raster-tools-0.1.3/tests/test_focal.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    22392 2023-02-01 19:59:47.000000 raster-tools-0.1.3/tests/test_general.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7288 2023-01-28 03:48:27.000000 raster-tools-0.1.3/tests/test_line_stats.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    55226 2023-02-16 01:34:06.000000 raster-tools-0.1.3/tests/test_raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4124 2022-08-26 20:44:16.000000 raster-tools-0.1.3/tests/test_stat_common.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5157 2023-02-15 02:21:21.000000 raster-tools-0.1.3/tests/test_surface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10830 2023-01-25 02:09:19.000000 raster-tools-0.1.3/tests/test_vector.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6903 2023-04-06 20:45:48.000000 raster-tools-0.1.3/tests/test_zonal.py
```

### Comparing `raster-tools-0.1.2/LICENSE` & `raster-tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/PKG-INFO` & `raster-tools-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `raster-tools-0.1.2/README.md` & `raster-tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/__init__.py` & `raster-tools-0.1.3/raster_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/batch.py` & `raster-tools-0.1.3/raster_tools/batch.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/clipping.py` & `raster-tools-0.1.3/raster_tools/clipping.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/creation.py` & `raster-tools-0.1.3/raster_tools/creation.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/dask_utils.py` & `raster-tools-0.1.3/raster_tools/dask_utils.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/distance/_heap.py` & `raster-tools-0.1.3/raster_tools/distance/_heap.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/distance/cost_distance.py` & `raster-tools-0.1.3/raster_tools/distance/cost_distance.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/distance/proximity.py` & `raster-tools-0.1.3/raster_tools/distance/proximity.py`

 * *Files 1% similar despite different names*

```diff
@@ -897,16 +897,16 @@
     Compute the proximity, allocation, and direction for a given source raster.
 
     This function uses proximity analysis to compute the proximity, allocation,
     and direction rasters for a given source raster. See the individual
     functions for more details:
 
     * :func:`pa_proximity`
-    * :func:`pa_allocation`
     * :func:`pa_direction`
+    * :func:`pa_allocation`
 
     This is very similar to ESRI's Proximity Analysis tools.
 
     Parameters
     ----------
     raster : Raster, path str
         The input source raster. If `target_values` is not specified or empty,
@@ -942,47 +942,51 @@
             range [-90, 90] and longitude must be in the range [-180, 180].
     double_precision : bool
         If ``True``, distances will will be computed with 64-bit precision,
         otherwise 32-bit floats are used. Default is ``False``.
 
     Returns
     -------
-    Raster
+    proximity : Raster
+        The proximity raster.
+    direction : Raster
         The direction raster.
+    allocation : Raster
+        The allocation raster.
 
     References
     ----------
     * `ESRI: Proximity Analysis <https://desktop.arcgis.com/en/arcmap/latest/analyze/commonly-used-tools/proximity-analysis.htm>`_
     * `ESRI: Euclidean Distance <https://desktop.arcgis.com/en/arcmap/latest/tools/spatial-analyst-toolbox/euclidean-distance.htm>`_
     * `ESRI: Euclidean Allocation <https://desktop.arcgis.com/en/arcmap/latest/tools/spatial-analyst-toolbox/euclidean-allocation.htm>`_
     * `ESRI: Euclidean Direction <https://desktop.arcgis.com/en/arcmap/latest/tools/spatial-analyst-toolbox/euclidean-direction.htm>`_
     * `Taxicab Distance <https://en.wikipedia.org/wiki/Taxicab_geometry>`_
     * `Chebyshev Distance <https://en.wikipedia.org/wiki/Chebyshev_distance>`_
     * `Great-Circle Distance <https://en.wikipedia.org/wiki/Great-circle_distance>`_
 
     See also
     --------
-    pa_proximity, pa_allocation, pa_direction
+    pa_proximity, pa_direction, pa_allocation
 
     """  # noqa: E501
     prox = pa_proximity(
         raster=raster,
         target_values=target_values,
         distance_metric=distance_metric,
         max_distance=max_distance,
         double_precision=double_precision,
     )
-    alloc = pa_allocation(
+    direction = pa_direction(
         raster=raster,
         target_values=target_values,
         distance_metric=distance_metric,
         max_distance=max_distance,
         double_precision=double_precision,
     )
-    direction = pa_direction(
+    alloc = pa_allocation(
         raster=raster,
         target_values=target_values,
         distance_metric=distance_metric,
         max_distance=max_distance,
         double_precision=double_precision,
     )
-    return prox, alloc, direction
+    return prox, direction, alloc
```

### Comparing `raster-tools-0.1.2/raster_tools/dtypes.py` & `raster-tools-0.1.3/raster_tools/dtypes.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/focal.py` & `raster-tools-0.1.3/raster_tools/focal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/general.py` & `raster-tools-0.1.3/raster_tools/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
     The approach is based on ESRI's local function.
 
     Parameters
     ----------
     raster : Raster or path str
         Input Raster object or path string
     stype : str
-        Summarization type. Valid opition are mean, std, var, max, min,
+        Summarization type. Valid opitions are mean, std, var, max, min,
         maxband, minband, prod, sum, mode, median, unique, entropy, asm
 
     Returns
     -------
     Raster
         The resulting raster of values aggregated along the band dimension.
```

### Comparing `raster-tools-0.1.2/raster_tools/io.py` & `raster-tools-0.1.3/raster_tools/io.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/line_stats.py` & `raster-tools-0.1.3/raster_tools/line_stats.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/masking.py` & `raster-tools-0.1.3/raster_tools/masking.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/raster.py` & `raster-tools-0.1.3/raster_tools/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -602,15 +602,20 @@
         if _fast_path:
             self._ds = raster
         else:
             self._ds = get_raster_ds(raster)
 
     def __repr__(self):
         # TODO: implement
-        return repr(self._ds.raster)
+        crs = self.crs
+        masked = self._masked
+        return (
+            f"<raster_tools.Raster (crs='{crs}', masked={masked})>\n"
+            f"{repr(self._ds.raster)}"
+        )
 
     @property
     def null_value(self):
         """The raster's null value used to fill missing or invalid entries."""
         return self._ds.raster.rio.nodata
 
     @property
@@ -620,15 +625,15 @@
     @property
     def xdata(self):
         """The underlying :class:`xarray.DataArray` (read only)"""
         return self._ds.raster
 
     @property
     def data(self):
-        """The underlying dask array of data (read only)"""
+        """The underlying dask array of data"""
         return self._ds.raster.data
 
     @property
     def values(self):
         """
         The raw internal raster as a numpy array.
```

### Comparing `raster-tools-0.1.2/raster_tools/stat_common.py` & `raster-tools-0.1.3/raster_tools/stat_common.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/surface.py` & `raster-tools-0.1.3/raster_tools/surface.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/utils.py` & `raster-tools-0.1.3/raster_tools/utils.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools/vector.py` & `raster-tools-0.1.3/raster_tools/vector.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import dask.array as da
 import dask.dataframe as dd
 import dask_geopandas as dgpd
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import rasterio as rio
-import shapely
 import xarray as xr
 from dask.delayed import delayed
 from packaging import version
 from rasterio.enums import MergeAlg
 from rasterio.env import GDALVersion
 from rasterio.features import rasterize as rio_rasterize
 
@@ -228,33 +227,14 @@
         return result
     elif _is_series(src) or _is_frame(src):
         return Vector(src)
     else:
         raise TypeError("Invalid vector input")
 
 
-def get_vector_frame(src):
-    if isinstance(src, Vector):
-        return src.data
-    elif is_str(src):
-        result = open_vectors(src)
-        if not isinstance(result, Vector):
-            # More than one layer was found
-            raise ValueError("Input source must only have 1 layer")
-        return result.data
-    elif _is_series(src) or _is_frame(src):
-        if _is_series(src):
-            src = src.to_frame("geometry")
-        if dask.is_dask_collection(src):
-            return src
-        return dgpd.from_geopandas(src, npartitions=1)
-    else:
-        raise TypeError("Invalid vector input")
-
-
 def _get_len_from_divisions(divs):
     # This should never overcount but may undercount by 1 because
     # dask.dataframe special cases the last division when creating a dataframe.
     #
     # NOTE: Dask dataframes have a divisions property. This is a tuple of
     # locations along the index where partitions start and stop. It looks like
     # this: (0, 10, 20, 29) for a dataframe with 3 divisions and 30 elements.
@@ -440,28 +420,16 @@
     result = result.rio.write_nodata(fill)
     return result
 
 
 def _geoms_to_raster_mask(xc, yc, geoms, all_touched=True, block_info=None):
     xc = xc.ravel()
     yc = yc.ravel()
-    shape = (yc.size, xc.size)
-    cell_size = max(np.diff(xc).max(), np.diff(yc).max())
-    chunk_bbox = shapely.geometry.box(
-        xc.min(), yc.min(), xc.max(), yc.max()
-    ).buffer(cell_size)
-    geoms_bbox = shapely.geometry.box(*geoms.total_bounds)
-    if not shapely.intersects(chunk_bbox, geoms_bbox):
-        return np.zeros(shape, dtype="uint8")
-
-    geoms = geoms.clip(chunk_bbox)
-    if not len(geoms):
-        return np.zeros(shape, dtype="uint8")
-
     # Convert geoms into a boolean (0/1) array using xc and yc for gridding.
+    shape = (yc.size, xc.size)
     transform = xr.DataArray(
         da.zeros(shape), coords=(yc, xc), dims=("y", "x")
     ).rio.transform()
     # Use a MemoryFile to avoid writing to disk
     with rio.io.MemoryFile() as memfile, rio.open(
         memfile,
         mode="w+",
@@ -490,100 +458,24 @@
             yc,
             geoms=part,
             all_touched=all_touched,
             chunks=like.data.chunks[1:],
             meta=np.array((), dtype=I8),
         )
         parts.append(data)
-    data = da.stack(parts, axis=0).any(axis=0, keepdims=True).astype("uint8")
+    data = da.stack(parts, axis=0).max(axis=0, keepdims=True)
     x = like.x
     y = like.y
     xrs = xr.DataArray(data, coords=([1], y, x), dims=like.xdata.dims)
     if like.crs is not None:
         xrs = xrs.rio.write_crs(like.crs)
     xrs = xrs.rio.write_nodata(0)
     return xrs
 
 
-def rasterize(gdf, like, field=None, all_touched=True):
-    """Convert vector data to a raster.
-
-    Parameters
-    ----------
-    like : Raster
-        A to use for grid and CRS information. The resulting raster will be
-        on the same grid as `like`.
-    field : str, optional
-        The name of a field to use for fill values when rasterizing the
-        vector features.
-    all_touched : bool, optional
-        If ``True``, grid cells that the vector touches will be burned in.
-        If False, only cells with a center point inside of the vector
-        perimeter will be burned in.
-
-    Returns
-    -------
-    Raster
-        The resulting raster. The result will have a single band. Each
-        vector shape is assigned a 1-based integer value equal to its order
-        in the original vector collection. This integer value is what is
-        burned in at the corresponding grid cells. The dtype of the result
-        will be the minimum, unsigned integer type that can fit the ID
-        values. The null value is 0.
-
-    """
-    like = get_raster(like)
-    if field is not None:
-        if not is_str(field):
-            raise TypeError("Field must be a string")
-        if field not in gdf:
-            raise ValueError(f"Invalid field name: {repr(field)}")
-        dtype = gdf.dtypes.to_dict()[field]
-        if not is_int(dtype) and not is_float(dtype):
-            raise ValueError("The specified field must be a scalar data type")
-
-    xrs = _vector_to_raster_dask(
-        gdf.to_crs(like.crs),
-        gdf.size,
-        xlike=like.xdata,
-        field=field,
-        all_touched=all_touched,
-    )
-    return Raster(xrs)
-
-
-def rasterize_mask(gdf, like, all_touched=True):
-    """Convert vector data to a raster mask.
-
-    Parameters
-    ----------
-    like : Raster
-        A to use for grid and CRS information. The resulting raster will be
-        on the same grid as `like`.
-    all_touched : bool, optional
-        If ``True``, grid cells that the vector touches will be burned in.
-        If False, only cells with a center point inside of the vector
-        perimeter will be burned in.
-
-    Returns
-    -------
-    Raster
-        The resulting raster. The result will have a single band. All cells
-        that fall under the vector data are masked with ``1``. The null
-        value is 0.
-
-    """
-    like = get_raster(like)
-
-    xrs = _vector_to_raster_mask(
-        gdf.to_crs(like.crs).geometry, like, all_touched=all_touched
-    )
-    return Raster(xrs)
-
-
 def _normalize_geo_data(geo):
     if not _is_series(geo) and not _is_frame(geo):
         raise TypeError(
             "Invalid data type. Must be some type GeoDataFrame or"
             f" GeoSeries. Got {type(geo)}."
         )
     if _is_series(geo):
```

### Comparing `raster-tools-0.1.2/raster_tools/zonal.py` & `raster-tools-0.1.3/raster_tools/zonal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/raster_tools.egg-info/PKG-INFO` & `raster-tools-0.1.3/raster_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `raster-tools-0.1.2/raster_tools.egg-info/SOURCES.txt` & `raster-tools-0.1.3/raster_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/setup.py` & `raster-tools-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_clipping.py` & `raster-tools-0.1.3/tests/test_clipping.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_distance.py` & `raster-tools-0.1.3/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_distance__heap.py` & `raster-tools-0.1.3/tests/test_distance__heap.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_distance_proximity.py` & `raster-tools-0.1.3/tests/test_distance_proximity.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 )
 
 
 @pytest.mark.parametrize("src", [esri_src, esri_src.astype("uint8")])
 def test_proximity_analysis_esri_example(src):
     src = Raster(src).set_null_value(0)
 
-    prox, alloc, dirn = prx.proximity_analysis(src)
+    prox, dirn, alloc = prx.proximity_analysis(src)
 
     assert np.allclose(prox, esri_euc_prox)
     assert np.allclose(alloc, esri_euc_alloc)
     assert np.allclose(dirn, esri_euc_dir)
     assert prox.dtype == F32
     assert prox.xdata.compute().dtype == F32
     assert alloc.dtype == src.dtype
@@ -92,15 +92,15 @@
     prox_truth = esri_euc_prox.copy()
     prox_truth[mask] = prox.null_value
     alloc_truth = esri_euc_alloc.copy()
     alloc_truth[mask] = alloc.null_value
     dir_truth = esri_euc_dir.copy()
     dir_truth[mask] = dirn.null_value
 
-    prox, alloc, dirn = prx.proximity_analysis(src, max_distance=3)
+    prox, dirn, alloc = prx.proximity_analysis(src, max_distance=3)
 
     assert np.allclose(prox, prox_truth)
     assert np.allclose(prox.mask.compute(), mask)
     assert np.allclose(alloc, alloc_truth)
     assert np.allclose(alloc.mask.compute(), mask)
     assert np.allclose(dirn, dir_truth)
     assert np.allclose(dirn.mask.compute(), mask)
@@ -222,15 +222,15 @@
 )
 @pytest.mark.parametrize("src", srcs)
 def test_proximity_metric(src, metric, truth_func, max_distance):
     data = src.values[0]
     x = src.x
     y = src.y
 
-    rprox, ralloc, rdirn = prx.proximity_analysis(
+    rprox, rdirn, ralloc = prx.proximity_analysis(
         src, distance_metric=metric, max_distance=max_distance
     )
     tprox, talloc, tdirn = apply_metric(
         data,
         x,
         y,
         truth_func,
@@ -253,26 +253,26 @@
 def test_proximity_great_circle():
     tprox = Raster("tests/data/raster/prox_haversine_proximity.tif")
     talloc = Raster("tests/data/raster/prox_haversine_allocation.tif")
     tdirn = Raster("tests/data/raster/prox_haversine_direction.tif")
 
     src = Raster("tests/data/raster/prox_src.tif")
 
-    rprox, ralloc, rdirn = prx.proximity_analysis(
+    rprox, rdirn, ralloc = prx.proximity_analysis(
         src, distance_metric="haversine"
     )
     assert np.allclose(rprox, tprox)
     assert np.allclose(ralloc, talloc)
     assert np.allclose(rdirn, tdirn)
 
     max_dist = 1.5e6
     mask = tprox.values > max_dist
     tprox.xdata.data = da.where(mask, tprox.null_value, tprox.data)
     talloc.xdata.data = da.where(mask, talloc.null_value, talloc.data)
     tdirn.xdata.data = da.where(mask, tdirn.null_value, tdirn.data)
 
-    rprox, ralloc, rdirn = prx.proximity_analysis(
+    rprox, rdirn, ralloc = prx.proximity_analysis(
         src, distance_metric="haversine", max_distance=max_dist
     )
     assert np.allclose(rprox, tprox)
     assert np.allclose(ralloc, talloc)
     assert np.allclose(rdirn, tdirn)
```

### Comparing `raster-tools-0.1.2/tests/test_focal.py` & `raster-tools-0.1.3/tests/test_focal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_general.py` & `raster-tools-0.1.3/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_line_stats.py` & `raster-tools-0.1.3/tests/test_line_stats.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_raster.py` & `raster-tools-0.1.3/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_stat_common.py` & `raster-tools-0.1.3/tests/test_stat_common.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_surface.py` & `raster-tools-0.1.3/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_vector.py` & `raster-tools-0.1.3/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.2/tests/test_zonal.py` & `raster-tools-0.1.3/tests/test_zonal.py`

 * *Files identical despite different names*

