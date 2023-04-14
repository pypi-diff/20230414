# Comparing `tmp/MGSurvE-0.8.0.1.tar.gz` & `tmp/MGSurvE-0.8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-0.8.0.1.tar", last modified: Fri Apr 14 20:37:36 2023, max compression
+gzip compressed data, was "MGSurvE-0.8.0.2.tar", last modified: Fri Apr 14 21:42:39 2023, max compression
```

## Comparing `MGSurvE-0.8.0.1.tar` & `MGSurvE-0.8.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-14 20:37:36.954342 MGSurvE-0.8.0.1/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-04-07 16:28:31.000000 MGSurvE-0.8.0.1/LICENSE
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-14 20:37:36.954342 MGSurvE-0.8.0.1/MGSurvE/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      275 2022-04-21 22:03:09.000000 MGSurvE-0.8.0.1/MGSurvE/__init__.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       23 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE/_version.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6881 2022-04-13 19:47:11.000000 MGSurvE-0.8.0.1/MGSurvE/auxiliary.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      604 2022-02-18 19:18:22.000000 MGSurvE-0.8.0.1/MGSurvE/colors.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1665 2022-04-07 16:28:31.000000 MGSurvE-0.8.0.1/MGSurvE/constants.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6409 2023-04-14 19:41:05.000000 MGSurvE-0.8.0.1/MGSurvE/kernels.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    21356 2022-08-10 16:42:54.000000 MGSurvE-0.8.0.1/MGSurvE/landscape.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4924 2022-03-21 16:18:35.000000 MGSurvE-0.8.0.1/MGSurvE/matrices.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1358 2022-02-18 19:21:24.000000 MGSurvE-0.8.0.1/MGSurvE/network.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    45037 2023-02-23 20:20:29.000000 MGSurvE-0.8.0.1/MGSurvE/optimization.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     9200 2022-05-13 21:20:28.000000 MGSurvE-0.8.0.1/MGSurvE/optimizationPSO.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    17959 2023-04-14 20:32:16.000000 MGSurvE-0.8.0.1/MGSurvE/plots.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6849 2023-03-02 20:49:07.000000 MGSurvE-0.8.0.1/MGSurvE/pointProcess.py
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-14 20:37:36.954342 MGSurvE-0.8.0.1/MGSurvE.egg-info/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE.egg-info/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      451 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE.egg-info/SOURCES.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE.egg-info/dependency_links.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      214 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE.egg-info/requires.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        8 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE.egg-info/top_level.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-04-14 20:37:36.954342 MGSurvE-0.8.0.1/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4162 2023-04-04 16:41:41.000000 MGSurvE-0.8.0.1/README.md
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-04-14 20:37:36.954342 MGSurvE-0.8.0.1/setup.cfg
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1414 2023-03-29 20:42:31.000000 MGSurvE-0.8.0.1/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-04-14 21:42:39.005117 MGSurvE-0.8.0.2/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/LICENSE
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-04-14 21:42:39.000588 MGSurvE-0.8.0.2/MGSurvE/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       23 2023-04-14 21:42:38.000000 MGSurvE-0.8.0.2/MGSurvE/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      604 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6409 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/kernels.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21356 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/landscape.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/matrices.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/network.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/optimization.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/optimizationPSO.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18224 2023-04-14 21:30:43.000000 MGSurvE-0.8.0.2/MGSurvE/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/MGSurvE/pointProcess.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-04-14 21:42:39.003203 MGSurvE-0.8.0.2/MGSurvE.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4596 2023-04-14 21:42:38.000000 MGSurvE-0.8.0.2/MGSurvE.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-04-14 21:42:38.000000 MGSurvE-0.8.0.2/MGSurvE.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-04-14 21:42:38.000000 MGSurvE-0.8.0.2/MGSurvE.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      214 2023-04-14 21:42:38.000000 MGSurvE-0.8.0.2/MGSurvE.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-04-14 21:42:38.000000 MGSurvE-0.8.0.2/MGSurvE.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4596 2023-04-14 21:42:39.004675 MGSurvE-0.8.0.2/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4162 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/README.md
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-04-14 21:42:39.005236 MGSurvE-0.8.0.2/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1414 2023-04-14 21:27:20.000000 MGSurvE-0.8.0.2/setup.py
```

### Comparing `MGSurvE-0.8.0.1/LICENSE` & `MGSurvE-0.8.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE/auxiliary.py` & `MGSurvE-0.8.0.2/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE/colors.py` & `MGSurvE-0.8.0.2/MGSurvE/colors.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE/constants.py` & `MGSurvE-0.8.0.2/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE/kernels.py` & `MGSurvE-0.8.0.2/MGSurvE/kernels.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE/landscape.py` & `MGSurvE-0.8.0.2/MGSurvE/landscape.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE/matrices.py` & `MGSurvE-0.8.0.2/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE/network.py` & `MGSurvE-0.8.0.2/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE/optimization.py` & `MGSurvE-0.8.0.2/MGSurvE/optimization.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE/optimizationPSO.py` & `MGSurvE-0.8.0.2/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE/plots.py` & `MGSurvE-0.8.0.2/MGSurvE/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 
 '''
 
 import warnings
 import matplotlib
 from os import path
 from math import log
-import cartopy.crs as ccrs
-import shapely.geometry as sgeom
-from cartopy.geodesic import Geodesic
 import matplotlib.pyplot as plt
 import MGSurvE.constants as cst
 import networkx as nx
 from sklearn.preprocessing import normalize
 import numpy as np
 
+try:
+    import cartopy.crs as ccrs
+    import shapely.geometry as sgeom
+    from cartopy.geodesic import Geodesic
+    CARTOPY = True
+except ImportError:
+    warnings.warn("Cartopy not installed. Lat/Long plots might be incorrect!")
+
 
 def plotSites(
         fig, ax, 
         sites, pTypes,
         markers=cst.MKRS, colors=cst.MCOL,
         size=350, edgecolors='w', linewidths=1.25,
         zorder=5, transform=None, **kwargs
@@ -94,15 +99,15 @@
 def plotTraps(
         fig, ax,
         trapsCoords, trapsTypes, trapsKernels, trapsFixed,
         colors=cst.TRP_COLS, marker="X",
         edgecolors=('w', 'k'), lws=(2, 0), ls=':',
         size=350, zorders=(25, -5), fill=True,
         transform=None, transparencyHex='DD',
-        latlon=False, proj=ccrs.PlateCarree(),
+        latlon=False, proj=None,
         **kwargs
     ):
     """ Plots the traps with the radii of effectiveness.
 
     Parameters:
         fig (matplotlib): Matplotlib fig object.
         ax (matplotlib): Matplotlib ax object.
@@ -134,24 +139,26 @@
         ax.scatter(
             trap[0], trap[1], 
             marker=marker, color=col[:-2]+transp, 
             s=size, zorder=zorders[0],
             edgecolors=ec, linewidths=lws[0]
         )
         # Draw Circles
-        if latlon:
+        if latlon and CARTOPY:
             (gd, geoms) = (Geodesic(), [])
             for r in trapsKernels[tType]['radii']:
                 cp = gd.circle(lon=trap[0], lat=trap[1], radius=r)
                 geoms.append(sgeom.Polygon(cp))
             ax.add_geometries(
                 geoms, crs=ccrs.PlateCarree(), 
                 edgecolor='#00000000', color=col, 
                 zorder=zorders[1]
             )
+        if latlon and not CARTOPY:
+            warnings.warn("Please install cartopy to plot the traps' radii of attractiveness!")
         else:
             for r in trapsKernels[tType]['radii']:
                 circle = plt.Circle(
                     (trap[0], trap[1]), r, 
                     color=col, fill=fill, ls=ls, 
                     lw=lws[1], zorder=zorders[1]
                 )
```

### Comparing `MGSurvE-0.8.0.1/MGSurvE/pointProcess.py` & `MGSurvE-0.8.0.2/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-0.8.0.2/MGSurvE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 0.8.0.1
+Version: 0.8.0.2
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-0.8.0.1/PKG-INFO` & `MGSurvE-0.8.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 0.8.0.1
+Version: 0.8.0.2
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-0.8.0.1/README.md` & `MGSurvE-0.8.0.2/README.md`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.8.0.1/setup.py` & `MGSurvE-0.8.0.2/setup.py`

 * *Files identical despite different names*

