# Comparing `tmp/newick-tree-builder-0.4.0.tar.gz` & `tmp/newick-tree-builder-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newick-tree-builder-0.4.0.tar", last modified: Fri Apr 14 12:14:35 2023, max compression
+gzip compressed data, was "newick-tree-builder-0.4.4.tar", last modified: Fri Apr 14 14:26:52 2023, max compression
```

## Comparing `newick-tree-builder-0.4.0.tar` & `newick-tree-builder-0.4.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 12:14:35.493594 newick-tree-builder-0.4.0/
--rw-r--r--   0 ba        (1000) ba        (1000)      724 2023-04-14 12:14:35.493594 newick-tree-builder-0.4.0/PKG-INFO
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 12:14:35.493594 newick-tree-builder-0.4.0/newick/
--rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-07 17:41:00.000000 newick-tree-builder-0.4.0/newick/__init__.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 12:14:35.493594 newick-tree-builder-0.4.0/newick/backend/
--rw-r--r--   0 ba        (1000) ba        (1000)       34 2023-04-08 12:27:05.000000 newick-tree-builder-0.4.0/newick/backend/__init__.py
--rw-r--r--   0 ba        (1000) ba        (1000)     1121 2023-04-07 19:57:05.000000 newick-tree-builder-0.4.0/newick/backend/nhx_util.py
--rw-r--r--   0 ba        (1000) ba        (1000)    25242 2023-04-14 11:09:02.000000 newick-tree-builder-0.4.0/newick/backend/node.py
--rw-r--r--   0 ba        (1000) ba        (1000)     2255 2023-04-14 10:06:26.000000 newick-tree-builder-0.4.0/newick/backend/path.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 12:14:35.493594 newick-tree-builder-0.4.0/newick/backend/test/
--rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-07 19:39:39.000000 newick-tree-builder-0.4.0/newick/backend/test/__init__.py
--rw-r--r--   0 ba        (1000) ba        (1000)      633 2023-04-12 14:37:56.000000 newick-tree-builder-0.4.0/newick/backend/test/test_nhx_util.py
--rw-r--r--   0 ba        (1000) ba        (1000)     3576 2023-04-14 09:39:53.000000 newick-tree-builder-0.4.0/newick/backend/test/test_node.py
--rw-r--r--   0 ba        (1000) ba        (1000)      833 2023-04-14 10:08:13.000000 newick-tree-builder-0.4.0/newick/backend/test/test_path.py
--rw-r--r--   0 ba        (1000) ba        (1000)     1884 2023-04-14 10:45:15.000000 newick-tree-builder-0.4.0/newick/backend/test/test_tree.py
--rw-r--r--   0 ba        (1000) ba        (1000)    13087 2023-04-14 11:02:21.000000 newick-tree-builder-0.4.0/newick/backend/tree.py
--rw-r--r--   0 ba        (1000) ba        (1000)      252 2023-04-08 12:32:42.000000 newick-tree-builder-0.4.0/newick/backend/util_funcs.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 12:14:35.493594 newick-tree-builder-0.4.0/newick/frontend/
--rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-11 18:09:04.000000 newick-tree-builder-0.4.0/newick/frontend/__init__.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 12:14:35.493594 newick-tree-builder-0.4.0/newick/frontend/test/
--rw-r--r--   0 ba        (1000) ba        (1000)       85 2023-04-14 11:10:34.000000 newick-tree-builder-0.4.0/newick/frontend/test/test_very_basic.py
--rw-r--r--   0 ba        (1000) ba        (1000)     1307 2023-04-14 11:36:16.000000 newick-tree-builder-0.4.0/newick/frontend/very_basic.py
-drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 12:14:35.493594 newick-tree-builder-0.4.0/newick_tree_builder.egg-info/
--rw-r--r--   0 ba        (1000) ba        (1000)      724 2023-04-14 12:14:35.000000 newick-tree-builder-0.4.0/newick_tree_builder.egg-info/PKG-INFO
--rw-r--r--   0 ba        (1000) ba        (1000)      665 2023-04-14 12:14:35.000000 newick-tree-builder-0.4.0/newick_tree_builder.egg-info/SOURCES.txt
--rw-r--r--   0 ba        (1000) ba        (1000)        1 2023-04-14 12:14:35.000000 newick-tree-builder-0.4.0/newick_tree_builder.egg-info/dependency_links.txt
--rw-r--r--   0 ba        (1000) ba        (1000)       24 2023-04-14 12:14:35.000000 newick-tree-builder-0.4.0/newick_tree_builder.egg-info/requires.txt
--rw-r--r--   0 ba        (1000) ba        (1000)        7 2023-04-14 12:14:35.000000 newick-tree-builder-0.4.0/newick_tree_builder.egg-info/top_level.txt
--rw-r--r--   0 ba        (1000) ba        (1000)     1001 2023-04-14 12:07:39.000000 newick-tree-builder-0.4.0/pyproject.toml
--rw-r--r--   0 ba        (1000) ba        (1000)       38 2023-04-14 12:14:35.493594 newick-tree-builder-0.4.0/setup.cfg
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:26:52.853594 newick-tree-builder-0.4.4/
+-rw-r--r--   0 ba        (1000) ba        (1000)      783 2023-04-14 14:26:52.853594 newick-tree-builder-0.4.4/PKG-INFO
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:26:52.843594 newick-tree-builder-0.4.4/newick/
+-rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-07 17:41:00.000000 newick-tree-builder-0.4.4/newick/__init__.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:26:52.843594 newick-tree-builder-0.4.4/newick/backend/
+-rw-r--r--   0 ba        (1000) ba        (1000)       34 2023-04-08 12:27:05.000000 newick-tree-builder-0.4.4/newick/backend/__init__.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     1103 2023-04-14 13:08:53.000000 newick-tree-builder-0.4.4/newick/backend/nhx_util.py
+-rw-r--r--   0 ba        (1000) ba        (1000)    25290 2023-04-14 14:02:54.000000 newick-tree-builder-0.4.4/newick/backend/node.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     2255 2023-04-14 10:06:26.000000 newick-tree-builder-0.4.4/newick/backend/path.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:26:52.853594 newick-tree-builder-0.4.4/newick/backend/test/
+-rw-r--r--   0 ba        (1000) ba        (1000)       32 2023-04-14 12:45:25.000000 newick-tree-builder-0.4.4/newick/backend/test/__init__.py
+-rw-r--r--   0 ba        (1000) ba        (1000)      619 2023-04-14 13:09:59.000000 newick-tree-builder-0.4.4/newick/backend/test/test_nhx_util.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     3576 2023-04-14 09:39:53.000000 newick-tree-builder-0.4.4/newick/backend/test/test_node.py
+-rw-r--r--   0 ba        (1000) ba        (1000)      833 2023-04-14 10:08:13.000000 newick-tree-builder-0.4.4/newick/backend/test/test_path.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     1884 2023-04-14 10:45:15.000000 newick-tree-builder-0.4.4/newick/backend/test/test_tree.py
+-rw-r--r--   0 ba        (1000) ba        (1000)    13087 2023-04-14 13:16:33.000000 newick-tree-builder-0.4.4/newick/backend/tree.py
+-rw-r--r--   0 ba        (1000) ba        (1000)      252 2023-04-08 12:32:42.000000 newick-tree-builder-0.4.4/newick/backend/util_funcs.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:26:52.853594 newick-tree-builder-0.4.4/newick/frontend/
+-rw-r--r--   0 ba        (1000) ba        (1000)        0 2023-04-11 18:09:04.000000 newick-tree-builder-0.4.4/newick/frontend/__init__.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:26:52.853594 newick-tree-builder-0.4.4/newick/frontend/test/
+-rw-r--r--   0 ba        (1000) ba        (1000)       32 2023-04-14 12:45:30.000000 newick-tree-builder-0.4.4/newick/frontend/test/__init__.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     2865 2023-04-14 14:22:50.000000 newick-tree-builder-0.4.4/newick/frontend/test/test_very_basic.py
+-rw-r--r--   0 ba        (1000) ba        (1000)     2434 2023-04-14 14:06:10.000000 newick-tree-builder-0.4.4/newick/frontend/very_basic.py
+drwxr-xr-x   0 ba        (1000) ba        (1000)        0 2023-04-14 14:26:52.853594 newick-tree-builder-0.4.4/newick_tree_builder.egg-info/
+-rw-r--r--   0 ba        (1000) ba        (1000)      783 2023-04-14 14:26:52.000000 newick-tree-builder-0.4.4/newick_tree_builder.egg-info/PKG-INFO
+-rw-r--r--   0 ba        (1000) ba        (1000)      698 2023-04-14 14:26:52.000000 newick-tree-builder-0.4.4/newick_tree_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)        1 2023-04-14 14:26:52.000000 newick-tree-builder-0.4.4/newick_tree_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)       24 2023-04-14 14:26:52.000000 newick-tree-builder-0.4.4/newick_tree_builder.egg-info/requires.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)        7 2023-04-14 14:26:52.000000 newick-tree-builder-0.4.4/newick_tree_builder.egg-info/top_level.txt
+-rw-r--r--   0 ba        (1000) ba        (1000)     1060 2023-04-14 14:26:13.000000 newick-tree-builder-0.4.4/pyproject.toml
+-rw-r--r--   0 ba        (1000) ba        (1000)       38 2023-04-14 14:26:52.853594 newick-tree-builder-0.4.4/setup.cfg
```

### Comparing `newick-tree-builder-0.4.0/PKG-INFO` & `newick-tree-builder-0.4.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: newick-tree-builder
-Version: 0.4.0
-Summary: small lib to generate newick trees.
+Version: 0.4.4
+Summary: Small lib to generate newick trees. Comes with NHX and rudimentary hybridization capabilities.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 Project-URL: Homepage, https://github.com/NiRit100/newick-tree-builder
 Keywords: biology,newick,newick-format,new hampshire,tree,graph-theory,x-nh
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `newick-tree-builder-0.4.0/newick/backend/nhx_util.py` & `newick-tree-builder-0.4.4/newick/backend/nhx_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 def generate_nhx(dict:dict, ext_head='&&NHX') -> str:
     if dict == None or len(dict) == 0:
-        return "[" + ext_head + "]"
+        return ""
     else:
         ret_elements = []
         for key in dict.keys():
             str_key = nhx_filter_str(str(key))
             str_val = nhx_filter_str(str(dict[key]))
             str_el = str_key + '=' + str_val
             ret_elements.append(str_el)
```

### Comparing `newick-tree-builder-0.4.0/newick/backend/node.py` & `newick-tree-builder-0.4.4/newick/backend/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,17 @@
                 Whether or not to count this duplication.
         """
         # count duplicates
         if count:
             self._dupcount += 1
         # copy additional information
         s_ao = self.get_additional_info()
-        for k, v in other.get_additional_info():
+        o_ao = other.get_additional_info()
+        for k in o_ao.keys():
+            v = o_ao[k]
             if k in s_ao.keys():
                 if s_ao[k] != v:
                     if isinstance(v, set) and isinstance(s_ao[k], set):
                         s_ao[k] = s_ao[k].union(v)
                     elif isinstance(v, list) and isinstance(s_ao[k], list):
                         s_ao[k].extend(v)
                     else:
```

### Comparing `newick-tree-builder-0.4.0/newick/backend/path.py` & `newick-tree-builder-0.4.4/newick/backend/path.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.0/newick/backend/test/test_nhx_util.py` & `newick-tree-builder-0.4.4/newick/backend/test/test_nhx_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from newick.backend.nhx_util import *
 
 def test_generate_nhx_null():
-    assert generate_nhx(None) == "[&&NHX]"
+    assert generate_nhx(None) == ""
     
 def test_generate_nhx_empty():
-    assert generate_nhx(dict()) == "[&&NHX]"
+    assert generate_nhx(dict()) == ""
     
 def test_generate_nhx_alphanum():
     dct = {"A":1, "Bonn": None, 52: True}
     assert generate_nhx(dct) == "[&&NHX:A=1:Bonn=None:52=True]"
 
 def test_generate_nhx_othersym():
     dct = {"A=C":1, "B:nn": "B(er)lin", "new\n-line": "s p a c e"}
```

### Comparing `newick-tree-builder-0.4.0/newick/backend/test/test_node.py` & `newick-tree-builder-0.4.4/newick/backend/test/test_node.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.0/newick/backend/test/test_path.py` & `newick-tree-builder-0.4.4/newick/backend/test/test_path.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.0/newick/backend/test/test_tree.py` & `newick-tree-builder-0.4.4/newick/backend/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.0/newick/backend/tree.py` & `newick-tree-builder-0.4.4/newick/backend/tree.py`

 * *Files identical despite different names*

### Comparing `newick-tree-builder-0.4.0/newick_tree_builder.egg-info/PKG-INFO` & `newick-tree-builder-0.4.4/newick_tree_builder.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: newick-tree-builder
-Version: 0.4.0
-Summary: small lib to generate newick trees.
+Version: 0.4.4
+Summary: Small lib to generate newick trees. Comes with NHX and rudimentary hybridization capabilities.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 Project-URL: Homepage, https://github.com/NiRit100/newick-tree-builder
 Keywords: biology,newick,newick-format,new hampshire,tree,graph-theory,x-nh
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `newick-tree-builder-0.4.0/newick_tree_builder.egg-info/SOURCES.txt` & `newick-tree-builder-0.4.4/newick_tree_builder.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 newick/backend/test/__init__.py
 newick/backend/test/test_nhx_util.py
 newick/backend/test/test_node.py
 newick/backend/test/test_path.py
 newick/backend/test/test_tree.py
 newick/frontend/__init__.py
 newick/frontend/very_basic.py
+newick/frontend/test/__init__.py
 newick/frontend/test/test_very_basic.py
 newick_tree_builder.egg-info/PKG-INFO
 newick_tree_builder.egg-info/SOURCES.txt
 newick_tree_builder.egg-info/dependency_links.txt
 newick_tree_builder.egg-info/requires.txt
 newick_tree_builder.egg-info/top_level.txt
```

### Comparing `newick-tree-builder-0.4.0/pyproject.toml` & `newick-tree-builder-0.4.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "newick-tree-builder"
-version = "0.4.0"
-description = "small lib to generate newick trees."
+version = "0.4.4"
+description = "Small lib to generate newick trees. Comes with NHX and rudimentary hybridization capabilities."
 authors = [{ name = "Nico Rittinghaus", email = "nico@ritti.ng" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
```

