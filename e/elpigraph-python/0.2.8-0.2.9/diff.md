# Comparing `tmp/elpigraph-python-0.2.8.tar.gz` & `tmp/elpigraph-python-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elpigraph-python-0.2.8.tar", last modified: Thu Apr 13 10:32:47 2023, max compression
+gzip compressed data, was "elpigraph-python-0.2.9.tar", last modified: Fri Apr 14 13:08:29 2023, max compression
```

## Comparing `elpigraph-python-0.2.8.tar` & `elpigraph-python-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-13 10:32:47.923720 elpigraph-python-0.2.8/
--rw-r--r--   0 jbac       (502) staff       (20)    35823 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/LICENSE
--rw-r--r--   0 jbac       (502) staff       (20)       26 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/MANIFEST.in
--rw-r--r--   0 jbac       (502) staff       (20)     2735 2023-04-13 10:32:47.923808 elpigraph-python-0.2.8/PKG-INFO
--rw-r--r--   0 jbac       (502) staff       (20)     2190 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/README.md
-drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-13 10:32:47.920682 elpigraph-python-0.2.8/elpigraph/
--rw-r--r--   0 jbac       (502) staff       (20)    37260 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/_AlterStructure.py
--rw-r--r--   0 jbac       (502) staff       (20)    23429 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/_BaseElPiWrapper.py
--rw-r--r--   0 jbac       (502) staff       (20)     1074 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/_EMAdjustment.py
--rw-r--r--   0 jbac       (502) staff       (20)      563 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/__init__.py
--rw-r--r--   0 jbac       (502) staff       (20)    36962 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/_graph_editing.py
--rw-r--r--   0 jbac       (502) staff       (20)    62370 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/_topologies.py
--rw-r--r--   0 jbac       (502) staff       (20)       23 2023-04-13 10:19:41.000000 elpigraph-python-0.2.8/elpigraph/_version.py
--rw-r--r--   0 jbac       (502) staff       (20)    78943 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/plot.py
-drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-13 10:32:47.922574 elpigraph-python-0.2.8/elpigraph/src/
--rw-r--r--   0 jbac       (502) staff       (20)    39106 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/BaseElPi.py
--rw-r--r--   0 jbac       (502) staff       (20)     6811 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/PCA.py
--rw-r--r--   0 jbac       (502) staff       (20)      184 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/__init__.py
--rw-r--r--   0 jbac       (502) staff       (20)    69252 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/core.py
--rw-r--r--   0 jbac       (502) staff       (20)    19376 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/distutils.py
--rw-r--r--   0 jbac       (502) staff       (20)    71100 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/grammar_operations.py
--rw-r--r--   0 jbac       (502) staff       (20)    16072 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/graphs.py
--rw-r--r--   0 jbac       (502) staff       (20)     9721 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/reporting.py
--rw-r--r--   0 jbac       (502) staff       (20)    32378 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/supervised.py
--rw-r--r--   0 jbac       (502) staff       (20)     3823 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/elpigraph/src/synthetic.py
--rw-r--r--   0 jbac       (502) staff       (20)    18040 2023-04-13 10:18:22.000000 elpigraph-python-0.2.8/elpigraph/utils.py
-drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-13 10:32:47.923573 elpigraph-python-0.2.8/elpigraph_python.egg-info/
--rw-r--r--   0 jbac       (502) staff       (20)     2735 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/PKG-INFO
--rw-r--r--   0 jbac       (502) staff       (20)      787 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/SOURCES.txt
--rw-r--r--   0 jbac       (502) staff       (20)        1 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/dependency_links.txt
--rw-r--r--   0 jbac       (502) staff       (20)        1 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/not-zip-safe
--rw-r--r--   0 jbac       (502) staff       (20)      225 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/requires.txt
--rw-r--r--   0 jbac       (502) staff       (20)       10 2023-04-13 10:32:47.000000 elpigraph-python-0.2.8/elpigraph_python.egg-info/top_level.txt
--rw-r--r--   0 jbac       (502) staff       (20)      137 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/requirements.txt
--rw-r--r--   0 jbac       (502) staff       (20)      106 2023-04-13 10:32:47.924130 elpigraph-python-0.2.8/setup.cfg
--rw-r--r--   0 jbac       (502) staff       (20)     2580 2023-04-13 10:16:31.000000 elpigraph-python-0.2.8/setup.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:08:28.995315 elpigraph-python-0.2.9/
+-rw-r--r--   0 jbac       (502) staff       (20)    35823 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/LICENSE
+-rw-r--r--   0 jbac       (502) staff       (20)       26 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/MANIFEST.in
+-rw-r--r--   0 jbac       (502) staff       (20)     2735 2023-04-14 13:08:28.995431 elpigraph-python-0.2.9/PKG-INFO
+-rw-r--r--   0 jbac       (502) staff       (20)     2190 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/README.md
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:08:28.990455 elpigraph-python-0.2.9/elpigraph/
+-rw-r--r--   0 jbac       (502) staff       (20)    37260 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/_AlterStructure.py
+-rw-r--r--   0 jbac       (502) staff       (20)    23429 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/_BaseElPiWrapper.py
+-rw-r--r--   0 jbac       (502) staff       (20)     1074 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/_EMAdjustment.py
+-rw-r--r--   0 jbac       (502) staff       (20)      563 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/__init__.py
+-rw-r--r--   0 jbac       (502) staff       (20)    36968 2023-04-14 13:07:23.000000 elpigraph-python-0.2.9/elpigraph/_graph_editing.py
+-rw-r--r--   0 jbac       (502) staff       (20)    62370 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/_topologies.py
+-rw-r--r--   0 jbac       (502) staff       (20)       23 2023-04-14 13:07:35.000000 elpigraph-python-0.2.9/elpigraph/_version.py
+-rw-r--r--   0 jbac       (502) staff       (20)    78943 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/plot.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:08:28.993966 elpigraph-python-0.2.9/elpigraph/src/
+-rw-r--r--   0 jbac       (502) staff       (20)    39106 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/src/BaseElPi.py
+-rw-r--r--   0 jbac       (502) staff       (20)     6811 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/src/PCA.py
+-rw-r--r--   0 jbac       (502) staff       (20)      184 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/src/__init__.py
+-rw-r--r--   0 jbac       (502) staff       (20)    69252 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/src/core.py
+-rw-r--r--   0 jbac       (502) staff       (20)    19376 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/src/distutils.py
+-rw-r--r--   0 jbac       (502) staff       (20)    71100 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/src/grammar_operations.py
+-rw-r--r--   0 jbac       (502) staff       (20)    16072 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/src/graphs.py
+-rw-r--r--   0 jbac       (502) staff       (20)     9721 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/src/reporting.py
+-rw-r--r--   0 jbac       (502) staff       (20)    32378 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/src/supervised.py
+-rw-r--r--   0 jbac       (502) staff       (20)     3823 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/elpigraph/src/synthetic.py
+-rw-r--r--   0 jbac       (502) staff       (20)    18040 2023-04-13 10:18:22.000000 elpigraph-python-0.2.9/elpigraph/utils.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:08:28.995154 elpigraph-python-0.2.9/elpigraph_python.egg-info/
+-rw-r--r--   0 jbac       (502) staff       (20)     2735 2023-04-14 13:08:28.000000 elpigraph-python-0.2.9/elpigraph_python.egg-info/PKG-INFO
+-rw-r--r--   0 jbac       (502) staff       (20)      787 2023-04-14 13:08:28.000000 elpigraph-python-0.2.9/elpigraph_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jbac       (502) staff       (20)        1 2023-04-14 13:08:28.000000 elpigraph-python-0.2.9/elpigraph_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jbac       (502) staff       (20)        1 2023-04-13 10:32:47.000000 elpigraph-python-0.2.9/elpigraph_python.egg-info/not-zip-safe
+-rw-r--r--   0 jbac       (502) staff       (20)      225 2023-04-14 13:08:28.000000 elpigraph-python-0.2.9/elpigraph_python.egg-info/requires.txt
+-rw-r--r--   0 jbac       (502) staff       (20)       10 2023-04-14 13:08:28.000000 elpigraph-python-0.2.9/elpigraph_python.egg-info/top_level.txt
+-rw-r--r--   0 jbac       (502) staff       (20)      137 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/requirements.txt
+-rw-r--r--   0 jbac       (502) staff       (20)      106 2023-04-14 13:08:28.995831 elpigraph-python-0.2.9/setup.cfg
+-rw-r--r--   0 jbac       (502) staff       (20)     2580 2023-04-13 10:16:31.000000 elpigraph-python-0.2.9/setup.py
```

### Comparing `elpigraph-python-0.2.8/LICENSE` & `elpigraph-python-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/PKG-INFO` & `elpigraph-python-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elpigraph-python
-Version: 0.2.8
+Version: 0.2.9
 Home-page: https://github.com/j-bac/elpigraph-python
 Maintainer: Jonathan Bac
 Maintainer-email: 
 Project-URL: Bug Reports, https://github.com/j-bac/elpigraph-python/issues
 Project-URL: Source, https://github.com/j-bac/elpigraph-python/
 Keywords: machine_learning graphs dimension_reduction single_cell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elpigraph-python-0.2.8/README.md` & `elpigraph-python-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/_AlterStructure.py` & `elpigraph-python-0.2.9/elpigraph/_AlterStructure.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/_BaseElPiWrapper.py` & `elpigraph-python-0.2.9/elpigraph/_BaseElPiWrapper.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/_EMAdjustment.py` & `elpigraph-python-0.2.9/elpigraph/_EMAdjustment.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/__init__.py` & `elpigraph-python-0.2.9/elpigraph/__init__.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/_graph_editing.py` & `elpigraph-python-0.2.9/elpigraph/_graph_editing.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     lnodep = new_nodep.tolist()
     new_edges = edges.tolist()
     multiline = MultiLineString([LineString(new_nodep[e]) for e in new_edges])
 
     while not (multiline.is_simple):  # while intersections in graph
 
         # find an intersection, update edges, break, update graph
-        for i, j in itertools.combinations(range(len(multiline)), 2):
+        for i, j in itertools.combinations(range(len(multiline.geoms)), 2):
             line1, line2 = multiline[i], multiline[j]
             if line1.intersects(line2):
                 if list(np.array(line1.intersection(line2))) not in lnodep:
                     new_nodep = np.append(
                         new_nodep, np.array(line1.intersection(line2))[None], axis=0,
                     )
                     intersects_idx = [list(new_edges[i]), list(new_edges[j])]
```

### Comparing `elpigraph-python-0.2.8/elpigraph/_topologies.py` & `elpigraph-python-0.2.9/elpigraph/_topologies.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/plot.py` & `elpigraph-python-0.2.9/elpigraph/plot.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/src/BaseElPi.py` & `elpigraph-python-0.2.9/elpigraph/src/BaseElPi.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/src/PCA.py` & `elpigraph-python-0.2.9/elpigraph/src/PCA.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/src/core.py` & `elpigraph-python-0.2.9/elpigraph/src/core.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/src/distutils.py` & `elpigraph-python-0.2.9/elpigraph/src/distutils.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/src/grammar_operations.py` & `elpigraph-python-0.2.9/elpigraph/src/grammar_operations.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/src/graphs.py` & `elpigraph-python-0.2.9/elpigraph/src/graphs.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/src/reporting.py` & `elpigraph-python-0.2.9/elpigraph/src/reporting.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/src/supervised.py` & `elpigraph-python-0.2.9/elpigraph/src/supervised.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/src/synthetic.py` & `elpigraph-python-0.2.9/elpigraph/src/synthetic.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph/utils.py` & `elpigraph-python-0.2.9/elpigraph/utils.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/elpigraph_python.egg-info/PKG-INFO` & `elpigraph-python-0.2.9/elpigraph_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elpigraph-python
-Version: 0.2.8
+Version: 0.2.9
 Home-page: https://github.com/j-bac/elpigraph-python
 Maintainer: Jonathan Bac
 Maintainer-email: 
 Project-URL: Bug Reports, https://github.com/j-bac/elpigraph-python/issues
 Project-URL: Source, https://github.com/j-bac/elpigraph-python/
 Keywords: machine_learning graphs dimension_reduction single_cell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elpigraph-python-0.2.8/elpigraph_python.egg-info/SOURCES.txt` & `elpigraph-python-0.2.9/elpigraph_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.2.8/setup.py` & `elpigraph-python-0.2.9/setup.py`

 * *Files identical despite different names*

