# Comparing `tmp/cbig_network_correspondence-0.0.6.tar.gz` & `tmp/cbig_network_correspondence-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbig_network_correspondence-0.0.6.tar", max compression
+gzip compressed data, was "cbig_network_correspondence-0.0.7.tar", max compression
```

## Comparing `cbig_network_correspondence-0.0.6.tar` & `cbig_network_correspondence-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3180 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/README.md
--rw-r--r--   0        0        0     2376 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      445 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/__init__.py
--rw-r--r--   0        0        0    10455 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/compute_overlap_with_atlases.py
--rw-r--r--   0        0        0     2189 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/grab_data_info.py
--rw-r--r--   0        0        0      429 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/load_example.py
--rw-r--r--   0        0        0        0 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/py.typed
--rw-r--r--   0        0        0     5442 2023-04-13 10:47:29.210388 cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/visualize_overlap_lib.py
--rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3180 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/README.md
+-rw-r--r--   0        0        0     2376 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      490 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/__init__.py
+-rw-r--r--   0        0        0    10455 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/compute_overlap_with_atlases.py
+-rw-r--r--   0        0        0     2189 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/grab_data_info.py
+-rw-r--r--   0        0        0      429 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/load_example.py
+-rw-r--r--   0        0        0        0 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/py.typed
+-rw-r--r--   0        0        0     5442 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/visualize_overlap_lib.py
+-rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.0.7/PKG-INFO
```

### Comparing `cbig_network_correspondence-0.0.6/README.md` & `cbig_network_correspondence-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.6/pyproject.toml` & `cbig_network_correspondence-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cbig_network_correspondence"
-version = "0.0.6"
+version = "0.0.7"
 description = "A toolbox for exploring network correspondence across atlases"
 authors = [
     "Ruby Kong <roo.cone@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/compute_overlap_with_atlases.py` & `cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/compute_overlap_with_atlases.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/grab_data_info.py` & `cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/grab_data_info.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.6/src/cbig_network_correspondence/visualize_overlap_lib.py` & `cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/visualize_overlap_lib.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.6/PKG-INFO` & `cbig_network_correspondence-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbig-network-correspondence
-Version: 0.0.6
+Version: 0.0.7
 Summary: A toolbox for exploring network correspondence across atlases
 Home-page: https://rubykong.github.io/cbig_network_correspondence
 License: MIT
 Author: Ruby Kong
 Author-email: roo.cone@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
```

