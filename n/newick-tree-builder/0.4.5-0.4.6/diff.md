# Comparing `tmp/newick-tree-builder-0.4.5.tar.gz` & `tmp/newick-tree-builder-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newick-tree-builder-0.4.5.tar", last modified: Fri Apr 14 14:43:58 2023, max compression
+gzip compressed data, was "newick-tree-builder-0.4.6.tar", last modified: Fri Apr 14 14:58:56 2023, max compression
```

## Comparing `newick-tree-builder-0.4.5.tar` & `newick-tree-builder-0.4.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:43:58.653594 newick-tree-builder-0.4.5/
--rw-r--r--   0 ba        (1000) ba        (1000)      783 2023-04-14 14:43:58.653594 newick-tree-builder-0.4.5/PKG-INFO
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:43:58.653594 newick-tree-builder-0.4.5/newick/
--rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-07 17:41:00.000000 newick-tree-builder-0.4.5/newick/__init__.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:43:58.653594 newick-tree-builder-0.4.5/newick/backend/
--rw-r--r--   0 ba        (1000) ba        (1000)       34 2023-04-08 12:27:05.000000 newick-tree-builder-0.4.5/newick/backend/__init__.py
--rw-r--r--   0 ba        (1000) ba        (1000)     1103 2023-04-14 13:08:53.000000 newick-tree-builder-0.4.5/newick/backend/nhx_util.py
--rw-r--r--   0 ba        (1000) ba        (1000)    24895 2023-04-14 14:42:21.000000 newick-tree-builder-0.4.5/newick/backend/node.py
--rw-r--r--   0 ba        (1000) ba        (1000)     2255 2023-04-14 10:06:26.000000 newick-tree-builder-0.4.5/newick/backend/path.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:43:58.653594 newick-tree-builder-0.4.5/newick/backend/test/
--rw-r--r--   0 ba        (1000) ba        (1000)       32 2023-04-14 12:45:25.000000 newick-tree-builder-0.4.5/newick/backend/test/__init__.py
--rw-r--r--   0 ba        (1000) ba        (1000)      619 2023-04-14 13:09:59.000000 newick-tree-builder-0.4.5/newick/backend/test/test_nhx_util.py
--rw-r--r--   0 ba        (1000) ba        (1000)     3576 2023-04-14 09:39:53.000000 newick-tree-builder-0.4.5/newick/backend/test/test_node.py
--rw-r--r--   0 ba        (1000) ba        (1000)      833 2023-04-14 10:08:13.000000 newick-tree-builder-0.4.5/newick/backend/test/test_path.py
--rw-r--r--   0 ba        (1000) ba        (1000)     1884 2023-04-14 10:45:15.000000 newick-tree-builder-0.4.5/newick/backend/test/test_tree.py
--rw-r--r--   0 ba        (1000) ba        (1000)    13087 2023-04-14 13:16:33.000000 newick-tree-builder-0.4.5/newick/backend/tree.py
--rw-r--r--   0 ba        (1000) ba        (1000)      252 2023-04-08 12:32:42.000000 newick-tree-builder-0.4.5/newick/backend/util_funcs.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:43:58.653594 newick-tree-builder-0.4.5/newick/frontend/
--rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-11 18:09:04.000000 newick-tree-builder-0.4.5/newick/frontend/__init__.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:43:58.653594 newick-tree-builder-0.4.5/newick/frontend/test/
--rw-r--r--   0 ba        (1000) ba        (1000)       32 2023-04-14 12:45:30.000000 newick-tree-builder-0.4.5/newick/frontend/test/__init__.py
--rw-r--r--   0 ba        (1000) ba        (1000)     2865 2023-04-14 14:22:50.000000 newick-tree-builder-0.4.5/newick/frontend/test/test_very_basic.py
--rw-r--r--   0 ba        (1000) ba        (1000)     2434 2023-04-14 14:06:10.000000 newick-tree-builder-0.4.5/newick/frontend/very_basic.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:43:58.653594 newick-tree-builder-0.4.5/newick_tree_builder.egg-info/
--rw-r--r--   0 ba        (1000) ba        (1000)      783 2023-04-14 14:43:58.000000 newick-tree-builder-0.4.5/newick_tree_builder.egg-info/PKG-INFO
--rw-r--r--   0 ba        (1000) ba        (1000)      698 2023-04-14 14:43:58.000000 newick-tree-builder-0.4.5/newick_tree_builder.egg-info/SOURCES.txt
--rw-r--r--   0 ba        (1000) ba        (1000)        1 2023-04-14 14:43:58.000000 newick-tree-builder-0.4.5/newick_tree_builder.egg-info/dependency_links.txt
--rw-r--r--   0 ba        (1000) ba        (1000)       24 2023-04-14 14:43:58.000000 newick-tree-builder-0.4.5/newick_tree_builder.egg-info/requires.txt
--rw-r--r--   0 ba        (1000) ba        (1000)        7 2023-04-14 14:43:58.000000 newick-tree-builder-0.4.5/newick_tree_builder.egg-info/top_level.txt
--rw-r--r--   0 ba        (1000) ba        (1000)     1060 2023-04-14 14:43:53.000000 newick-tree-builder-0.4.5/pyproject.toml
--rw-r--r--   0 ba        (1000) ba        (1000)       38 2023-04-14 14:43:58.653594 newick-tree-builder-0.4.5/setup.cfg
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:58:56.343594 newick-tree-builder-0.4.6/
+-rw-r--r--   0 ba        (1000) ba        (1000)      783 2023-04-14 14:58:56.343594 newick-tree-builder-0.4.6/PKG-INFO
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:58:56.343594 newick-tree-builder-0.4.6/newick/
+-rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-07 17:41:00.000000 newick-tree-builder-0.4.6/newick/__init__.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:58:56.343594 newick-tree-builder-0.4.6/newick/backend/
+-rw-r--r--   0 ba        (1000) ba        (1000)       34 2023-04-08 12:27:05.000000 newick-tree-builder-0.4.6/newick/backend/__init__.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     1103 2023-04-14 13:08:53.000000 newick-tree-builder-0.4.6/newick/backend/nhx_util.py
+-rw-r--r--   0 ba        (1000) ba        (1000)    24871 2023-04-14 14:57:02.000000 newick-tree-builder-0.4.6/newick/backend/node.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     2255 2023-04-14 10:06:26.000000 newick-tree-builder-0.4.6/newick/backend/path.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:58:56.343594 newick-tree-builder-0.4.6/newick/backend/test/
+-rw-r--r--   0 ba        (1000) ba        (1000)       32 2023-04-14 12:45:25.000000 newick-tree-builder-0.4.6/newick/backend/test/__init__.py
+-rw-r--r--   0 ba        (1000) ba        (1000)      619 2023-04-14 13:09:59.000000 newick-tree-builder-0.4.6/newick/backend/test/test_nhx_util.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     3576 2023-04-14 09:39:53.000000 newick-tree-builder-0.4.6/newick/backend/test/test_node.py
+-rw-r--r--   0 ba        (1000) ba        (1000)      833 2023-04-14 10:08:13.000000 newick-tree-builder-0.4.6/newick/backend/test/test_path.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     1884 2023-04-14 10:45:15.000000 newick-tree-builder-0.4.6/newick/backend/test/test_tree.py
+-rw-r--r--   0 ba        (1000) ba        (1000)    13087 2023-04-14 13:16:33.000000 newick-tree-builder-0.4.6/newick/backend/tree.py
+-rw-r--r--   0 ba        (1000) ba        (1000)      252 2023-04-08 12:32:42.000000 newick-tree-builder-0.4.6/newick/backend/util_funcs.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:58:56.343594 newick-tree-builder-0.4.6/newick/frontend/
+-rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-11 18:09:04.000000 newick-tree-builder-0.4.6/newick/frontend/__init__.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:58:56.343594 newick-tree-builder-0.4.6/newick/frontend/test/
+-rw-r--r--   0 ba        (1000) ba        (1000)       32 2023-04-14 12:45:30.000000 newick-tree-builder-0.4.6/newick/frontend/test/__init__.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     2865 2023-04-14 14:22:50.000000 newick-tree-builder-0.4.6/newick/frontend/test/test_very_basic.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     2434 2023-04-14 14:06:10.000000 newick-tree-builder-0.4.6/newick/frontend/very_basic.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:58:56.343594 newick-tree-builder-0.4.6/newick_tree_builder.egg-info/
+-rw-r--r--   0 ba        (1000) ba        (1000)      783 2023-04-14 14:58:56.000000 newick-tree-builder-0.4.6/newick_tree_builder.egg-info/PKG-INFO
+-rw-r--r--   0 ba        (1000) ba        (1000)      698 2023-04-14 14:58:56.000000 newick-tree-builder-0.4.6/newick_tree_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)        1 2023-04-14 14:58:56.000000 newick-tree-builder-0.4.6/newick_tree_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)       24 2023-04-14 14:58:56.000000 newick-tree-builder-0.4.6/newick_tree_builder.egg-info/requires.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)        7 2023-04-14 14:58:56.000000 newick-tree-builder-0.4.6/newick_tree_builder.egg-info/top_level.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)     1060 2023-04-14 14:58:52.000000 newick-tree-builder-0.4.6/pyproject.toml
+-rw-r--r--   0 ba        (1000) ba        (1000)       38 2023-04-14 14:58:56.343594 newick-tree-builder-0.4.6/setup.cfg
```

### Comparing `newick-tree-builder-0.4.5/PKG-INFO` & `newick-tree-builder-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newick-tree-builder
-Version: 0.4.5
+Version: 0.4.6
 Summary: Small lib to generate newick trees. Comes with NHX and rudimentary hybridization capabilities.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 Project-URL: Homepage, https://github.com/NiRit100/newick-tree-builder
 Keywords: biology,newick,newick-format,new hampshire,tree,graph-theory,x-nh
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `newick-tree-builder-0.4.5/newick/backend/nhx_util.py` & `newick-tree-builder-0.4.6/newick/backend/nhx_util.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.5/newick/backend/node.py` & `newick-tree-builder-0.4.6/newick/backend/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,18 +47,17 @@
                 dict().
             children (list, optional): 
                 list of children nodes. Defaults to [].
                 Please avoid using this if possible.
         """
         
         # argument validation
-        if not isinstance(label, str):
-            if label == None:
-                label = ""
-            else:
+        if label == None:
+            label = ""
+        elif not isinstance(label, str):
                 label = str(label)
         if not isinstance(distance, float):
             distance = float(distance)
         if distance < 0:
             msg = \
                 """
                 Distance from parent node must be positive.
```

### Comparing `newick-tree-builder-0.4.5/newick/backend/path.py` & `newick-tree-builder-0.4.6/newick/backend/path.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.5/newick/backend/test/test_nhx_util.py` & `newick-tree-builder-0.4.6/newick/backend/test/test_nhx_util.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.5/newick/backend/test/test_node.py` & `newick-tree-builder-0.4.6/newick/backend/test/test_node.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.5/newick/backend/test/test_path.py` & `newick-tree-builder-0.4.6/newick/backend/test/test_path.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.5/newick/backend/test/test_tree.py` & `newick-tree-builder-0.4.6/newick/backend/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.5/newick/backend/tree.py` & `newick-tree-builder-0.4.6/newick/backend/tree.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.5/newick/frontend/test/test_very_basic.py` & `newick-tree-builder-0.4.6/newick/frontend/test/test_very_basic.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.5/newick/frontend/very_basic.py` & `newick-tree-builder-0.4.6/newick/frontend/very_basic.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.5/newick_tree_builder.egg-info/PKG-INFO` & `newick-tree-builder-0.4.6/newick_tree_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newick-tree-builder
-Version: 0.4.5
+Version: 0.4.6
 Summary: Small lib to generate newick trees. Comes with NHX and rudimentary hybridization capabilities.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 Project-URL: Homepage, https://github.com/NiRit100/newick-tree-builder
 Keywords: biology,newick,newick-format,new hampshire,tree,graph-theory,x-nh
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `newick-tree-builder-0.4.5/newick_tree_builder.egg-info/SOURCES.txt` & `newick-tree-builder-0.4.6/newick_tree_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.5/pyproject.toml` & `newick-tree-builder-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "newick-tree-builder"
-version = "0.4.5"
+version = "0.4.6"
 description = "Small lib to generate newick trees. Comes with NHX and rudimentary hybridization capabilities."
 authors = [{ name = "Nico Rittinghaus", email = "nico@ritti.ng" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

