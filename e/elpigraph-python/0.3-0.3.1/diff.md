# Comparing `tmp/elpigraph-python-0.3.tar.gz` & `tmp/elpigraph-python-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elpigraph-python-0.3.tar", last modified: Fri Apr 14 13:26:17 2023, max compression
+gzip compressed data, was "elpigraph-python-0.3.1.tar", last modified: Fri Apr 14 13:41:07 2023, max compression
```

## Comparing `elpigraph-python-0.3.tar` & `elpigraph-python-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:26:17.911716 elpigraph-python-0.3/
--rw-r--r--   0 jbac       (502) staff       (20)    35823 2023-04-13 10:16:31.000000 elpigraph-python-0.3/LICENSE
--rw-r--r--   0 jbac       (502) staff       (20)       26 2023-04-13 10:16:31.000000 elpigraph-python-0.3/MANIFEST.in
--rw-r--r--   0 jbac       (502) staff       (20)     2733 2023-04-14 13:26:17.911845 elpigraph-python-0.3/PKG-INFO
--rw-r--r--   0 jbac       (502) staff       (20)     2190 2023-04-13 10:16:31.000000 elpigraph-python-0.3/README.md
-drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:26:17.908226 elpigraph-python-0.3/elpigraph/
--rw-r--r--   0 jbac       (502) staff       (20)    37260 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/_AlterStructure.py
--rw-r--r--   0 jbac       (502) staff       (20)    23429 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/_BaseElPiWrapper.py
--rw-r--r--   0 jbac       (502) staff       (20)     1074 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/_EMAdjustment.py
--rw-r--r--   0 jbac       (502) staff       (20)      563 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/__init__.py
--rw-r--r--   0 jbac       (502) staff       (20)    36994 2023-04-14 13:20:01.000000 elpigraph-python-0.3/elpigraph/_graph_editing.py
--rw-r--r--   0 jbac       (502) staff       (20)    62370 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/_topologies.py
--rw-r--r--   0 jbac       (502) staff       (20)       21 2023-04-14 13:20:25.000000 elpigraph-python-0.3/elpigraph/_version.py
--rw-r--r--   0 jbac       (502) staff       (20)    78943 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/plot.py
-drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:26:17.910467 elpigraph-python-0.3/elpigraph/src/
--rw-r--r--   0 jbac       (502) staff       (20)    39106 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/src/BaseElPi.py
--rw-r--r--   0 jbac       (502) staff       (20)     6811 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/src/PCA.py
--rw-r--r--   0 jbac       (502) staff       (20)      184 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/src/__init__.py
--rw-r--r--   0 jbac       (502) staff       (20)    69252 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/src/core.py
--rw-r--r--   0 jbac       (502) staff       (20)    19376 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/src/distutils.py
--rw-r--r--   0 jbac       (502) staff       (20)    71100 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/src/grammar_operations.py
--rw-r--r--   0 jbac       (502) staff       (20)    16072 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/src/graphs.py
--rw-r--r--   0 jbac       (502) staff       (20)     9721 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/src/reporting.py
--rw-r--r--   0 jbac       (502) staff       (20)    32378 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/src/supervised.py
--rw-r--r--   0 jbac       (502) staff       (20)     3823 2023-04-13 10:16:31.000000 elpigraph-python-0.3/elpigraph/src/synthetic.py
--rw-r--r--   0 jbac       (502) staff       (20)    18040 2023-04-13 10:18:22.000000 elpigraph-python-0.3/elpigraph/utils.py
-drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:26:17.911558 elpigraph-python-0.3/elpigraph_python.egg-info/
--rw-r--r--   0 jbac       (502) staff       (20)     2733 2023-04-14 13:26:17.000000 elpigraph-python-0.3/elpigraph_python.egg-info/PKG-INFO
--rw-r--r--   0 jbac       (502) staff       (20)      787 2023-04-14 13:26:17.000000 elpigraph-python-0.3/elpigraph_python.egg-info/SOURCES.txt
--rw-r--r--   0 jbac       (502) staff       (20)        1 2023-04-14 13:26:17.000000 elpigraph-python-0.3/elpigraph_python.egg-info/dependency_links.txt
--rw-r--r--   0 jbac       (502) staff       (20)        1 2023-04-13 10:32:47.000000 elpigraph-python-0.3/elpigraph_python.egg-info/not-zip-safe
--rw-r--r--   0 jbac       (502) staff       (20)      225 2023-04-14 13:26:17.000000 elpigraph-python-0.3/elpigraph_python.egg-info/requires.txt
--rw-r--r--   0 jbac       (502) staff       (20)       10 2023-04-14 13:26:17.000000 elpigraph-python-0.3/elpigraph_python.egg-info/top_level.txt
--rw-r--r--   0 jbac       (502) staff       (20)      137 2023-04-13 10:16:31.000000 elpigraph-python-0.3/requirements.txt
--rw-r--r--   0 jbac       (502) staff       (20)      106 2023-04-14 13:26:17.912175 elpigraph-python-0.3/setup.cfg
--rw-r--r--   0 jbac       (502) staff       (20)     2580 2023-04-13 10:16:31.000000 elpigraph-python-0.3/setup.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:41:07.459532 elpigraph-python-0.3.1/
+-rw-r--r--   0 jbac       (502) staff       (20)    35823 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/LICENSE
+-rw-r--r--   0 jbac       (502) staff       (20)       26 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/MANIFEST.in
+-rw-r--r--   0 jbac       (502) staff       (20)     2735 2023-04-14 13:41:07.459633 elpigraph-python-0.3.1/PKG-INFO
+-rw-r--r--   0 jbac       (502) staff       (20)     2190 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/README.md
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:41:07.456675 elpigraph-python-0.3.1/elpigraph/
+-rw-r--r--   0 jbac       (502) staff       (20)    37260 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/_AlterStructure.py
+-rw-r--r--   0 jbac       (502) staff       (20)    23429 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/_BaseElPiWrapper.py
+-rw-r--r--   0 jbac       (502) staff       (20)     1074 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/_EMAdjustment.py
+-rw-r--r--   0 jbac       (502) staff       (20)      563 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/__init__.py
+-rw-r--r--   0 jbac       (502) staff       (20)    37001 2023-04-14 13:40:06.000000 elpigraph-python-0.3.1/elpigraph/_graph_editing.py
+-rw-r--r--   0 jbac       (502) staff       (20)    62370 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/_topologies.py
+-rw-r--r--   0 jbac       (502) staff       (20)       23 2023-04-14 13:40:43.000000 elpigraph-python-0.3.1/elpigraph/_version.py
+-rw-r--r--   0 jbac       (502) staff       (20)    78943 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/plot.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:41:07.458426 elpigraph-python-0.3.1/elpigraph/src/
+-rw-r--r--   0 jbac       (502) staff       (20)    39106 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/src/BaseElPi.py
+-rw-r--r--   0 jbac       (502) staff       (20)     6811 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/src/PCA.py
+-rw-r--r--   0 jbac       (502) staff       (20)      184 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/src/__init__.py
+-rw-r--r--   0 jbac       (502) staff       (20)    69252 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/src/core.py
+-rw-r--r--   0 jbac       (502) staff       (20)    19376 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/src/distutils.py
+-rw-r--r--   0 jbac       (502) staff       (20)    71100 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/src/grammar_operations.py
+-rw-r--r--   0 jbac       (502) staff       (20)    16072 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/src/graphs.py
+-rw-r--r--   0 jbac       (502) staff       (20)     9721 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/src/reporting.py
+-rw-r--r--   0 jbac       (502) staff       (20)    32378 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/src/supervised.py
+-rw-r--r--   0 jbac       (502) staff       (20)     3823 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/elpigraph/src/synthetic.py
+-rw-r--r--   0 jbac       (502) staff       (20)    18040 2023-04-13 10:18:22.000000 elpigraph-python-0.3.1/elpigraph/utils.py
+drwxr-xr-x   0 jbac       (502) staff       (20)        0 2023-04-14 13:41:07.459354 elpigraph-python-0.3.1/elpigraph_python.egg-info/
+-rw-r--r--   0 jbac       (502) staff       (20)     2735 2023-04-14 13:41:07.000000 elpigraph-python-0.3.1/elpigraph_python.egg-info/PKG-INFO
+-rw-r--r--   0 jbac       (502) staff       (20)      787 2023-04-14 13:41:07.000000 elpigraph-python-0.3.1/elpigraph_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jbac       (502) staff       (20)        1 2023-04-14 13:41:07.000000 elpigraph-python-0.3.1/elpigraph_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jbac       (502) staff       (20)        1 2023-04-13 10:32:47.000000 elpigraph-python-0.3.1/elpigraph_python.egg-info/not-zip-safe
+-rw-r--r--   0 jbac       (502) staff       (20)      225 2023-04-14 13:41:07.000000 elpigraph-python-0.3.1/elpigraph_python.egg-info/requires.txt
+-rw-r--r--   0 jbac       (502) staff       (20)       10 2023-04-14 13:41:07.000000 elpigraph-python-0.3.1/elpigraph_python.egg-info/top_level.txt
+-rw-r--r--   0 jbac       (502) staff       (20)      137 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/requirements.txt
+-rw-r--r--   0 jbac       (502) staff       (20)      106 2023-04-14 13:41:07.459961 elpigraph-python-0.3.1/setup.cfg
+-rw-r--r--   0 jbac       (502) staff       (20)     2580 2023-04-13 10:16:31.000000 elpigraph-python-0.3.1/setup.py
```

### Comparing `elpigraph-python-0.3/LICENSE` & `elpigraph-python-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/PKG-INFO` & `elpigraph-python-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elpigraph-python
-Version: 0.3
+Version: 0.3.1
 Home-page: https://github.com/j-bac/elpigraph-python
 Maintainer: Jonathan Bac
 Maintainer-email: 
 Project-URL: Bug Reports, https://github.com/j-bac/elpigraph-python/issues
 Project-URL: Source, https://github.com/j-bac/elpigraph-python/
 Keywords: machine_learning graphs dimension_reduction single_cell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elpigraph-python-0.3/README.md` & `elpigraph-python-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/_AlterStructure.py` & `elpigraph-python-0.3.1/elpigraph/_AlterStructure.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/_BaseElPiWrapper.py` & `elpigraph-python-0.3.1/elpigraph/_BaseElPiWrapper.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/_EMAdjustment.py` & `elpigraph-python-0.3.1/elpigraph/_EMAdjustment.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/__init__.py` & `elpigraph-python-0.3.1/elpigraph/__init__.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/_graph_editing.py` & `elpigraph-python-0.3.1/elpigraph/_graph_editing.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,17 +110,17 @@
 
     while not (multiline.is_simple):  # while intersections in graph
 
         # find an intersection, update edges, break, update graph
         for i, j in itertools.combinations(range(len(multiline.geoms)), 2):
             line1, line2 = multiline.geoms[i], multiline.geoms[j]
             if line1.intersects(line2):
-                if list(np.array(line1.intersection(line2).coords)) not in lnodep:
+                if np.array(line1.intersection(line2).coords).flatten().tolist() not in lnodep:
                     new_nodep = np.append(
-                        new_nodep, np.array(line1.intersection(line2).coords)[None], axis=0,
+                        new_nodep, np.array(line1.intersection(line2).coords), axis=0,
                     )
                     intersects_idx = [list(new_edges[i]), list(new_edges[j])]
                     new_edges.pop(new_edges.index(intersects_idx[0]))
                     new_edges.pop(new_edges.index(intersects_idx[1]))
 
                     for n in np.array(intersects_idx).flatten():
                         new_edges.append([n, len(new_nodep) - 1])
```

### Comparing `elpigraph-python-0.3/elpigraph/_topologies.py` & `elpigraph-python-0.3.1/elpigraph/_topologies.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/plot.py` & `elpigraph-python-0.3.1/elpigraph/plot.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/src/BaseElPi.py` & `elpigraph-python-0.3.1/elpigraph/src/BaseElPi.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/src/PCA.py` & `elpigraph-python-0.3.1/elpigraph/src/PCA.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/src/core.py` & `elpigraph-python-0.3.1/elpigraph/src/core.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/src/distutils.py` & `elpigraph-python-0.3.1/elpigraph/src/distutils.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/src/grammar_operations.py` & `elpigraph-python-0.3.1/elpigraph/src/grammar_operations.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/src/graphs.py` & `elpigraph-python-0.3.1/elpigraph/src/graphs.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/src/reporting.py` & `elpigraph-python-0.3.1/elpigraph/src/reporting.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/src/supervised.py` & `elpigraph-python-0.3.1/elpigraph/src/supervised.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/src/synthetic.py` & `elpigraph-python-0.3.1/elpigraph/src/synthetic.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph/utils.py` & `elpigraph-python-0.3.1/elpigraph/utils.py`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/elpigraph_python.egg-info/PKG-INFO` & `elpigraph-python-0.3.1/elpigraph_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elpigraph-python
-Version: 0.3
+Version: 0.3.1
 Home-page: https://github.com/j-bac/elpigraph-python
 Maintainer: Jonathan Bac
 Maintainer-email: 
 Project-URL: Bug Reports, https://github.com/j-bac/elpigraph-python/issues
 Project-URL: Source, https://github.com/j-bac/elpigraph-python/
 Keywords: machine_learning graphs dimension_reduction single_cell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `elpigraph-python-0.3/elpigraph_python.egg-info/SOURCES.txt` & `elpigraph-python-0.3.1/elpigraph_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elpigraph-python-0.3/setup.py` & `elpigraph-python-0.3.1/setup.py`

 * *Files identical despite different names*

