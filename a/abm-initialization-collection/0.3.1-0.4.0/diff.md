# Comparing `tmp/abm_initialization_collection-0.3.1.tar.gz` & `tmp/abm_initialization_collection-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abm_initialization_collection-0.3.1.tar", max compression
+gzip compressed data, was "abm_initialization_collection-0.4.0.tar", max compression
```

## Comparing `abm_initialization_collection-0.3.1.tar` & `abm_initialization_collection-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1519 2023-03-30 19:21:42.099904 abm_initialization_collection-0.3.1/LICENSE
--rw-r--r--   0        0        0      916 2023-03-30 19:21:42.099904 abm_initialization_collection-0.3.1/README.md
--rw-r--r--   0        0        0     1964 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/__main__.py
--rw-r--r--   0        0        0      257 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/coordinate/__init__.py
--rw-r--r--   0        0        0      783 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py
--rw-r--r--   0        0        0     3061 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/coordinate/make_grid_coordinates.py
--rw-r--r--   0        0        0      411 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/image/__init__.py
--rw-r--r--   0        0        0     4099 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/image/create_voronoi_image.py
--rw-r--r--   0        0        0      407 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/image/get_image_bounds.py
--rw-r--r--   0        0        0     3181 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/image/plot_contact_sheet.py
--rw-r--r--   0        0        0      874 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/image/select_fov_images.py
--rw-r--r--   0        0        0        0 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/py.typed
--rw-r--r--   0        0        0      778 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/__init__.py
--rw-r--r--   0        0        0      453 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/exclude_selected_ids.py
--rw-r--r--   0        0        0      715 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/get_image_samples.py
--rw-r--r--   0        0        0     2724 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/get_sample_indices.py
--rw-r--r--   0        0        0      449 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/include_selected_ids.py
--rw-r--r--   0        0        0     1812 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/remove_edge_regions.py
--rw-r--r--   0        0        0     6170 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/remove_unconnected_regions.py
--rw-r--r--   0        0        0     1453 2023-03-30 19:21:42.103904 abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/scale_sample_coordinates.py
--rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 abm_initialization_collection-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/LICENSE
+-rw-r--r--   0        0        0      916 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/README.md
+-rw-r--r--   0        0        0     1964 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/__main__.py
+-rw-r--r--   0        0        0      257 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/coordinate/__init__.py
+-rw-r--r--   0        0        0      783 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py
+-rw-r--r--   0        0        0     3061 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/coordinate/make_grid_coordinates.py
+-rw-r--r--   0        0        0      411 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/image/__init__.py
+-rw-r--r--   0        0        0     4099 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/image/create_voronoi_image.py
+-rw-r--r--   0        0        0      407 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/image/get_image_bounds.py
+-rw-r--r--   0        0        0     3181 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/image/plot_contact_sheet.py
+-rw-r--r--   0        0        0     1131 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/image/select_fov_images.py
+-rw-r--r--   0        0        0        0 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/py.typed
+-rw-r--r--   0        0        0      778 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/__init__.py
+-rw-r--r--   0        0        0      453 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/exclude_selected_ids.py
+-rw-r--r--   0        0        0      715 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/get_image_samples.py
+-rw-r--r--   0        0        0     2724 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/get_sample_indices.py
+-rw-r--r--   0        0        0      449 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/include_selected_ids.py
+-rw-r--r--   0        0        0     1812 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/remove_edge_regions.py
+-rw-r--r--   0        0        0     6170 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/remove_unconnected_regions.py
+-rw-r--r--   0        0        0     1453 2023-04-14 15:51:19.645270 abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/scale_sample_coordinates.py
+-rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 abm_initialization_collection-0.4.0/PKG-INFO
```

### Comparing `abm_initialization_collection-0.3.1/LICENSE` & `abm_initialization_collection-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/README.md` & `abm_initialization_collection-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/pyproject.toml` & `abm_initialization_collection-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abm-initialization-collection"
-version = "0.3.1"
+version = "0.4.0"
 description = "Collection of tasks for initializing abm simulations."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `abm_initialization_collection-0.3.1/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py` & `abm_initialization_collection-0.4.0/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/src/abm_initialization_collection/coordinate/make_grid_coordinates.py` & `abm_initialization_collection-0.4.0/src/abm_initialization_collection/coordinate/make_grid_coordinates.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/src/abm_initialization_collection/image/create_voronoi_image.py` & `abm_initialization_collection-0.4.0/src/abm_initialization_collection/image/create_voronoi_image.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/src/abm_initialization_collection/image/plot_contact_sheet.py` & `abm_initialization_collection-0.4.0/src/abm_initialization_collection/image/plot_contact_sheet.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/__init__.py` & `abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/get_image_samples.py` & `abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/get_image_samples.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/get_sample_indices.py` & `abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/get_sample_indices.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/remove_edge_regions.py` & `abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/remove_edge_regions.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/remove_unconnected_regions.py` & `abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/remove_unconnected_regions.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/src/abm_initialization_collection/sample/scale_sample_coordinates.py` & `abm_initialization_collection-0.4.0/src/abm_initialization_collection/sample/scale_sample_coordinates.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.3.1/PKG-INFO` & `abm_initialization_collection-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abm-initialization-collection
-Version: 0.3.1
+Version: 0.4.0
 Summary: Collection of tasks for initializing abm simulations.
 License: BSD-3-Clause
 Author: Jessica S. Yu
 Author-email: jesyu@uw.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

