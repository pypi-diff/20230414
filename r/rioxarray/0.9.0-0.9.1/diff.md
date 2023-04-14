# Comparing `tmp/rioxarray-0.9.0.tar.gz` & `tmp/rioxarray-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rioxarray-0.9.0.tar", last modified: Wed Nov 24 14:47:46 2021, max compression
+gzip compressed data, was "rioxarray-0.9.1.tar", last modified: Tue Jan  4 19:55:27 2022, max compression
```

## Comparing `rioxarray-0.9.0.tar` & `rioxarray-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 snowal    (1000) snowal    (1000)        0 2021-11-24 14:47:46.078156 rioxarray-0.9.0/
--rw-rw-r--   0 snowal    (1000) snowal    (1000)    10214 2021-11-23 20:47:55.000000 rioxarray-0.9.0/AUTHORS.rst
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     3022 2021-10-18 18:36:13.000000 rioxarray-0.9.0/CONTRIBUTING.rst
--rw-rw-r--   0 snowal    (1000) snowal    (1000)    10802 2021-10-18 18:36:13.000000 rioxarray-0.9.0/LICENSE
--rw-rw-r--   0 snowal    (1000) snowal    (1000)      654 2021-10-18 18:36:13.000000 rioxarray-0.9.0/LICENSE_datacube
--rw-rw-r--   0 snowal    (1000) snowal    (1000)    10273 2021-10-18 18:36:13.000000 rioxarray-0.9.0/LICENSE_xarray
--rw-rw-r--   0 snowal    (1000) snowal    (1000)      218 2021-10-18 18:36:13.000000 rioxarray-0.9.0/MANIFEST.in
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     4785 2021-11-24 14:47:46.078156 rioxarray-0.9.0/PKG-INFO
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     3849 2021-11-23 20:47:55.000000 rioxarray-0.9.0/README.rst
--rw-rw-r--   0 snowal    (1000) snowal    (1000)      146 2021-10-18 18:36:13.000000 rioxarray-0.9.0/pyproject.toml
-drwxrwxr-x   0 snowal    (1000) snowal    (1000)        0 2021-11-24 14:47:46.078156 rioxarray-0.9.0/rioxarray/
--rw-rw-r--   0 snowal    (1000) snowal    (1000)      405 2021-10-18 18:36:13.000000 rioxarray-0.9.0/rioxarray/__init__.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)    31722 2021-10-18 18:36:13.000000 rioxarray-0.9.0/rioxarray/_io.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     2693 2021-10-18 18:36:13.000000 rioxarray-0.9.0/rioxarray/_options.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     2321 2021-10-18 18:36:13.000000 rioxarray-0.9.0/rioxarray/_show_versions.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)       46 2021-11-24 14:42:35.000000 rioxarray-0.9.0/rioxarray/_version.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     1122 2021-10-18 18:36:13.000000 rioxarray-0.9.0/rioxarray/crs.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     1230 2021-10-18 18:36:13.000000 rioxarray-0.9.0/rioxarray/exceptions.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     9270 2021-10-18 18:36:13.000000 rioxarray-0.9.0/rioxarray/merge.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)    35279 2021-11-23 20:53:58.000000 rioxarray-0.9.0/rioxarray/raster_array.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)    18930 2021-11-23 20:46:09.000000 rioxarray-0.9.0/rioxarray/raster_dataset.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     9733 2021-10-18 18:36:13.000000 rioxarray-0.9.0/rioxarray/raster_writer.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)    37542 2021-10-18 18:36:13.000000 rioxarray-0.9.0/rioxarray/rioxarray.py
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     2108 2021-10-18 18:36:13.000000 rioxarray-0.9.0/rioxarray/xarray_plugin.py
-drwxrwxr-x   0 snowal    (1000) snowal    (1000)        0 2021-11-24 14:47:46.078156 rioxarray-0.9.0/rioxarray.egg-info/
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     4785 2021-11-24 14:47:46.000000 rioxarray-0.9.0/rioxarray.egg-info/PKG-INFO
--rw-rw-r--   0 snowal    (1000) snowal    (1000)      649 2021-11-24 14:47:46.000000 rioxarray-0.9.0/rioxarray.egg-info/SOURCES.txt
--rw-rw-r--   0 snowal    (1000) snowal    (1000)        1 2021-11-24 14:47:46.000000 rioxarray-0.9.0/rioxarray.egg-info/dependency_links.txt
--rw-rw-r--   0 snowal    (1000) snowal    (1000)       70 2021-11-24 14:47:46.000000 rioxarray-0.9.0/rioxarray.egg-info/entry_points.txt
--rw-rw-r--   0 snowal    (1000) snowal    (1000)        1 2021-11-24 14:47:46.000000 rioxarray-0.9.0/rioxarray.egg-info/not-zip-safe
--rw-rw-r--   0 snowal    (1000) snowal    (1000)      447 2021-11-24 14:47:46.000000 rioxarray-0.9.0/rioxarray.egg-info/requires.txt
--rw-rw-r--   0 snowal    (1000) snowal    (1000)       10 2021-11-24 14:47:46.000000 rioxarray-0.9.0/rioxarray.egg-info/top_level.txt
--rw-rw-r--   0 snowal    (1000) snowal    (1000)       38 2021-11-24 14:47:46.078156 rioxarray-0.9.0/setup.cfg
--rw-rw-r--   0 snowal    (1000) snowal    (1000)     2333 2021-10-18 18:36:13.000000 rioxarray-0.9.0/setup.py
+drwxrwxr-x   0 snowal    (1000) snowal    (1000)        0 2022-01-04 19:55:27.087497 rioxarray-0.9.1/
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)    10214 2021-12-08 15:15:15.000000 rioxarray-0.9.1/AUTHORS.rst
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     3022 2021-12-08 15:15:15.000000 rioxarray-0.9.1/CONTRIBUTING.rst
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)    10802 2021-12-08 15:15:15.000000 rioxarray-0.9.1/LICENSE
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)      654 2021-12-08 15:15:15.000000 rioxarray-0.9.1/LICENSE_datacube
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)    10273 2021-12-08 15:15:15.000000 rioxarray-0.9.1/LICENSE_xarray
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)      218 2021-12-08 15:15:15.000000 rioxarray-0.9.1/MANIFEST.in
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     4785 2022-01-04 19:55:27.087497 rioxarray-0.9.1/PKG-INFO
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     3849 2021-12-08 15:15:15.000000 rioxarray-0.9.1/README.rst
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)      146 2021-12-08 15:15:15.000000 rioxarray-0.9.1/pyproject.toml
+drwxrwxr-x   0 snowal    (1000) snowal    (1000)        0 2022-01-04 19:55:27.083497 rioxarray-0.9.1/rioxarray/
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)      405 2021-12-08 15:15:15.000000 rioxarray-0.9.1/rioxarray/__init__.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)    31722 2022-01-04 17:10:01.000000 rioxarray-0.9.1/rioxarray/_io.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     2693 2021-12-08 15:15:15.000000 rioxarray-0.9.1/rioxarray/_options.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     2321 2021-12-08 15:15:15.000000 rioxarray-0.9.1/rioxarray/_show_versions.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)       46 2022-01-04 19:36:27.000000 rioxarray-0.9.1/rioxarray/_version.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     1122 2021-12-08 15:15:15.000000 rioxarray-0.9.1/rioxarray/crs.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     1230 2021-12-08 15:15:15.000000 rioxarray-0.9.1/rioxarray/exceptions.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     9270 2021-12-08 15:15:15.000000 rioxarray-0.9.1/rioxarray/merge.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)    36358 2022-01-04 19:35:47.000000 rioxarray-0.9.1/rioxarray/raster_array.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)    18930 2021-12-08 15:15:15.000000 rioxarray-0.9.1/rioxarray/raster_dataset.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     9733 2021-12-08 15:15:15.000000 rioxarray-0.9.1/rioxarray/raster_writer.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)    37542 2021-12-08 15:15:15.000000 rioxarray-0.9.1/rioxarray/rioxarray.py
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     2108 2021-12-08 15:15:15.000000 rioxarray-0.9.1/rioxarray/xarray_plugin.py
+drwxrwxr-x   0 snowal    (1000) snowal    (1000)        0 2022-01-04 19:55:27.087497 rioxarray-0.9.1/rioxarray.egg-info/
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     4785 2022-01-04 19:55:27.000000 rioxarray-0.9.1/rioxarray.egg-info/PKG-INFO
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)      649 2022-01-04 19:55:27.000000 rioxarray-0.9.1/rioxarray.egg-info/SOURCES.txt
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)        1 2022-01-04 19:55:27.000000 rioxarray-0.9.1/rioxarray.egg-info/dependency_links.txt
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)       70 2022-01-04 19:55:27.000000 rioxarray-0.9.1/rioxarray.egg-info/entry_points.txt
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)        1 2022-01-04 19:55:27.000000 rioxarray-0.9.1/rioxarray.egg-info/not-zip-safe
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)      447 2022-01-04 19:55:27.000000 rioxarray-0.9.1/rioxarray.egg-info/requires.txt
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)       10 2022-01-04 19:55:27.000000 rioxarray-0.9.1/rioxarray.egg-info/top_level.txt
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)       38 2022-01-04 19:55:27.087497 rioxarray-0.9.1/setup.cfg
+-rw-rw-r--   0 snowal    (1000) snowal    (1000)     2333 2021-12-08 15:15:15.000000 rioxarray-0.9.1/setup.py
```

### Comparing `rioxarray-0.9.0/AUTHORS.rst` & `rioxarray-0.9.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/CONTRIBUTING.rst` & `rioxarray-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/LICENSE` & `rioxarray-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/LICENSE_datacube` & `rioxarray-0.9.1/LICENSE_datacube`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/LICENSE_xarray` & `rioxarray-0.9.1/LICENSE_xarray`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/PKG-INFO` & `rioxarray-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rioxarray
-Version: 0.9.0
+Version: 0.9.1
 Summary: rasterio xarray extension.
 Home-page: https://github.com/corteva/rioxarray
 Author: rioxarray Contributors
 Author-email: alansnow21@gmail.com
 License: BSD license
 Keywords: rioxarray,xarray,rasterio
 Platform: UNKNOWN
```

### Comparing `rioxarray-0.9.0/README.rst` & `rioxarray-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray/_io.py` & `rioxarray-0.9.1/rioxarray/_io.py`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray/_options.py` & `rioxarray-0.9.1/rioxarray/_options.py`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray/_show_versions.py` & `rioxarray-0.9.1/rioxarray/_show_versions.py`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray/crs.py` & `rioxarray-0.9.1/rioxarray/crs.py`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray/exceptions.py` & `rioxarray-0.9.1/rioxarray/exceptions.py`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray/merge.py` & `rioxarray-0.9.1/rioxarray/merge.py`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray/raster_array.py` & `rioxarray-0.9.1/rioxarray/raster_array.py`

 * *Files 5% similar despite different names*

```diff
@@ -483,21 +483,41 @@
 
         Returns
         --------
         :obj:`xarray.DataArray`:
             Contains the data from the src_data_array, reprojected to match
             match_data_array.
         """
-        return self.reproject(
+        reprojected_data_array = self.reproject(
             match_data_array.rio.crs,
             transform=match_data_array.rio.transform(recalc=True),
             shape=match_data_array.rio.shape,
             resampling=resampling,
             **reproject_kwargs,
         )
+        # hack to resolve: https://github.com/corteva/rioxarray/issues/298
+        # may be resolved in the future by flexible indexes:
+        # https://github.com/pydata/xarray/pull/4489#issuecomment-831809607
+        x_attrs = reprojected_data_array[reprojected_data_array.rio.x_dim].attrs.copy()
+        y_attrs = reprojected_data_array[reprojected_data_array.rio.y_dim].attrs.copy()
+        # ensure coords the same
+        reprojected_data_array = reprojected_data_array.assign_coords(
+            {
+                reprojected_data_array.rio.x_dim: match_data_array[
+                    match_data_array.rio.x_dim
+                ].values.copy(),
+                reprojected_data_array.rio.y_dim: match_data_array[
+                    match_data_array.rio.y_dim
+                ].values.copy(),
+            }
+        )
+        # ensure attributes copied
+        reprojected_data_array[reprojected_data_array.rio.x_dim].attrs = x_attrs
+        reprojected_data_array[reprojected_data_array.rio.y_dim].attrs = y_attrs
+        return reprojected_data_array
 
     def pad_xy(self, minx, miny, maxx, maxy, constant_values):
         """Pad the array to x,y bounds.
 
         .. versionadded:: 0.0.29
 
         Parameters
```

### Comparing `rioxarray-0.9.0/rioxarray/raster_dataset.py` & `rioxarray-0.9.1/rioxarray/raster_dataset.py`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray/raster_writer.py` & `rioxarray-0.9.1/rioxarray/raster_writer.py`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray/rioxarray.py` & `rioxarray-0.9.1/rioxarray/rioxarray.py`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray/xarray_plugin.py` & `rioxarray-0.9.1/rioxarray/xarray_plugin.py`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/rioxarray.egg-info/PKG-INFO` & `rioxarray-0.9.1/rioxarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rioxarray
-Version: 0.9.0
+Version: 0.9.1
 Summary: rasterio xarray extension.
 Home-page: https://github.com/corteva/rioxarray
 Author: rioxarray Contributors
 Author-email: alansnow21@gmail.com
 License: BSD license
 Keywords: rioxarray,xarray,rasterio
 Platform: UNKNOWN
```

### Comparing `rioxarray-0.9.0/rioxarray.egg-info/SOURCES.txt` & `rioxarray-0.9.1/rioxarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rioxarray-0.9.0/setup.py` & `rioxarray-0.9.1/setup.py`

 * *Files identical despite different names*

