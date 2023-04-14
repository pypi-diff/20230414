# Comparing `tmp/MGSurvE-0.7.5.5.tar.gz` & `tmp/MGSurvE-0.8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-0.7.5.5.tar", last modified: Thu Mar  2 21:26:10 2023, max compression
+gzip compressed data, was "MGSurvE-0.8.0.1.tar", last modified: Fri Apr 14 20:37:36 2023, max compression
```

## Comparing `MGSurvE-0.7.5.5.tar` & `MGSurvE-0.8.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-03-02 21:26:10.991648 MGSurvE-0.7.5.5/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-04-07 16:28:31.000000 MGSurvE-0.7.5.5/LICENSE
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-03-02 21:26:10.987648 MGSurvE-0.7.5.5/MGSurvE/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      275 2022-04-21 22:03:09.000000 MGSurvE-0.7.5.5/MGSurvE/__init__.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       23 2023-03-02 21:26:10.000000 MGSurvE-0.7.5.5/MGSurvE/_version.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6881 2022-04-13 19:47:11.000000 MGSurvE-0.7.5.5/MGSurvE/auxiliary.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      604 2022-02-18 19:18:22.000000 MGSurvE-0.7.5.5/MGSurvE/colors.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1665 2022-04-07 16:28:31.000000 MGSurvE-0.7.5.5/MGSurvE/constants.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6379 2022-07-29 16:40:19.000000 MGSurvE-0.7.5.5/MGSurvE/kernels.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    21356 2022-08-10 16:42:54.000000 MGSurvE-0.7.5.5/MGSurvE/landscape.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4924 2022-03-21 16:18:35.000000 MGSurvE-0.7.5.5/MGSurvE/matrices.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1358 2022-02-18 19:21:24.000000 MGSurvE-0.7.5.5/MGSurvE/network.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    45037 2023-02-23 20:20:29.000000 MGSurvE-0.7.5.5/MGSurvE/optimization.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     9200 2022-05-13 21:20:28.000000 MGSurvE-0.7.5.5/MGSurvE/optimizationPSO.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    17399 2022-09-20 03:17:58.000000 MGSurvE-0.7.5.5/MGSurvE/plots.py
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6849 2023-03-02 20:49:07.000000 MGSurvE-0.7.5.5/MGSurvE/pointProcess.py
-drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-03-02 21:26:10.991648 MGSurvE-0.7.5.5/MGSurvE.egg-info/
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-03-02 21:26:10.000000 MGSurvE-0.7.5.5/MGSurvE.egg-info/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      451 2023-03-02 21:26:10.000000 MGSurvE-0.7.5.5/MGSurvE.egg-info/SOURCES.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-03-02 21:26:10.000000 MGSurvE-0.7.5.5/MGSurvE.egg-info/dependency_links.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      198 2023-03-02 21:26:10.000000 MGSurvE-0.7.5.5/MGSurvE.egg-info/requires.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        8 2023-03-02 21:26:10.000000 MGSurvE-0.7.5.5/MGSurvE.egg-info/top_level.txt
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-03-02 21:26:10.991648 MGSurvE-0.7.5.5/PKG-INFO
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4162 2022-05-20 22:12:07.000000 MGSurvE-0.7.5.5/README.md
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-03-02 21:26:10.991648 MGSurvE-0.7.5.5/setup.cfg
--rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1348 2023-03-02 20:35:36.000000 MGSurvE-0.7.5.5/setup.py
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-14 20:37:36.954342 MGSurvE-0.8.0.1/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    35149 2022-04-07 16:28:31.000000 MGSurvE-0.8.0.1/LICENSE
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-14 20:37:36.954342 MGSurvE-0.8.0.1/MGSurvE/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      275 2022-04-21 22:03:09.000000 MGSurvE-0.8.0.1/MGSurvE/__init__.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       23 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE/_version.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6881 2022-04-13 19:47:11.000000 MGSurvE-0.8.0.1/MGSurvE/auxiliary.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      604 2022-02-18 19:18:22.000000 MGSurvE-0.8.0.1/MGSurvE/colors.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1665 2022-04-07 16:28:31.000000 MGSurvE-0.8.0.1/MGSurvE/constants.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6409 2023-04-14 19:41:05.000000 MGSurvE-0.8.0.1/MGSurvE/kernels.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    21356 2022-08-10 16:42:54.000000 MGSurvE-0.8.0.1/MGSurvE/landscape.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4924 2022-03-21 16:18:35.000000 MGSurvE-0.8.0.1/MGSurvE/matrices.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1358 2022-02-18 19:21:24.000000 MGSurvE-0.8.0.1/MGSurvE/network.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    45037 2023-02-23 20:20:29.000000 MGSurvE-0.8.0.1/MGSurvE/optimization.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     9200 2022-05-13 21:20:28.000000 MGSurvE-0.8.0.1/MGSurvE/optimizationPSO.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)    17959 2023-04-14 20:32:16.000000 MGSurvE-0.8.0.1/MGSurvE/plots.py
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     6849 2023-03-02 20:49:07.000000 MGSurvE-0.8.0.1/MGSurvE/pointProcess.py
+drwxrwxr-x   0 chipdelmal  (1000) chipdelmal  (1000)        0 2023-04-14 20:37:36.954342 MGSurvE-0.8.0.1/MGSurvE.egg-info/
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE.egg-info/PKG-INFO
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      451 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE.egg-info/SOURCES.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        1 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE.egg-info/dependency_links.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)      214 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE.egg-info/requires.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)        8 2023-04-14 20:37:36.000000 MGSurvE-0.8.0.1/MGSurvE.egg-info/top_level.txt
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4596 2023-04-14 20:37:36.954342 MGSurvE-0.8.0.1/PKG-INFO
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     4162 2023-04-04 16:41:41.000000 MGSurvE-0.8.0.1/README.md
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)       38 2023-04-14 20:37:36.954342 MGSurvE-0.8.0.1/setup.cfg
+-rw-rw-r--   0 chipdelmal  (1000) chipdelmal  (1000)     1414 2023-03-29 20:42:31.000000 MGSurvE-0.8.0.1/setup.py
```

### Comparing `MGSurvE-0.7.5.5/LICENSE` & `MGSurvE-0.8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.7.5.5/MGSurvE/auxiliary.py` & `MGSurvE-0.8.0.1/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.7.5.5/MGSurvE/colors.py` & `MGSurvE-0.8.0.1/MGSurvE/colors.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.7.5.5/MGSurvE/constants.py` & `MGSurvE-0.8.0.1/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.7.5.5/MGSurvE/kernels.py` & `MGSurvE-0.8.0.1/MGSurvE/kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     prob = A*math.exp(expC)+epsilon
     return prob
 
 
 ###############################################################################
 # Auxiliary
 ###############################################################################
-def nSolveKernel(kernelDict, yVal, guess=0, latlon=False, R=6371):
+def nSolveKernel(kernelDict, yVal, guess=0, latlon=False, R=6371e3):
     '''Calculates the distance it takes for the kernel to match a given probability (yVar).
 
     Args:
         kernelDict (dict): Dictionary with the kernel info {'kernel', 'params'}.
         yVal (float): Probability for which we are solving the distance.
         guess (float): Initial guess for the distance.
 
@@ -184,15 +184,15 @@
         float: Distance for the probability value.
     '''
     # https://stackoverflow.com/questions/5644836/in-python-how-does-one-catch-warnings-as-if-they-were-exceptions
     (kFun, kPar) = (kernelDict['kernel'], kernelDict['params'])
     func = lambda delta : yVal-kFun(delta, **kPar)
     distance = fsolve(func, guess)
     if latlon:
-        dist = math.atan(distance[0]/R)
+        dist = distance[0] # math.atan(distance[0]/R)*(180/math.pi)
     else:
         dist = distance[0]
     # Negative radius patch ---------------------------------------------------
     if dist < 0:
         return 0
     else:
         return dist
```

### Comparing `MGSurvE-0.7.5.5/MGSurvE/landscape.py` & `MGSurvE-0.8.0.1/MGSurvE/landscape.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.7.5.5/MGSurvE/matrices.py` & `MGSurvE-0.8.0.1/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.7.5.5/MGSurvE/network.py` & `MGSurvE-0.8.0.1/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.7.5.5/MGSurvE/optimization.py` & `MGSurvE-0.8.0.1/MGSurvE/optimization.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.7.5.5/MGSurvE/optimizationPSO.py` & `MGSurvE-0.8.0.1/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.7.5.5/MGSurvE/plots.py` & `MGSurvE-0.8.0.1/MGSurvE/plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 '''
 
 import warnings
 import matplotlib
 from os import path
 from math import log
+import cartopy.crs as ccrs
+import shapely.geometry as sgeom
+from cartopy.geodesic import Geodesic
 import matplotlib.pyplot as plt
 import MGSurvE.constants as cst
 import networkx as nx
 from sklearn.preprocessing import normalize
 import numpy as np
 
 
@@ -90,15 +93,16 @@
 
 def plotTraps(
         fig, ax,
         trapsCoords, trapsTypes, trapsKernels, trapsFixed,
         colors=cst.TRP_COLS, marker="X",
         edgecolors=('w', 'k'), lws=(2, 0), ls=':',
         size=350, zorders=(25, -5), fill=True,
-        transform=None, 
+        transform=None, transparencyHex='DD',
+        latlon=False, proj=ccrs.PlateCarree(),
         **kwargs
     ):
     """ Plots the traps with the radii of effectiveness.
 
     Parameters:
         fig (matplotlib): Matplotlib fig object.
         ax (matplotlib): Matplotlib ax object.
@@ -115,39 +119,47 @@
         kwargs (dict): Matplotlib's plot-compliant kwargs.
     
     Returns:
         (fig, ax): Matplotlib (fig, ax) tuple.
 
     """
     (cNum, tNum) = (len(colors), len(trapsTypes))
-    # if (cNum-tNum) < 0:
-    #     raise Exception(
-    #         'Less colors ({}) than trap types ({})!'.format(cNum, tNum)
-    #     )
     for (i, trap) in enumerate(trapsCoords):
         tType = trapsTypes[i]
         (col, ec) = (colors[tType], edgecolors[0])
         if trapsFixed[i]:
             ec = edgecolors[1]
-        transp = 'DD'
+        transp = transparencyHex
         if not fill:
             transp = '00'
         ax.scatter(
             trap[0], trap[1], 
             marker=marker, color=col[:-2]+transp, 
             s=size, zorder=zorders[0],
             edgecolors=ec, linewidths=lws[0]
         )
-        for r in trapsKernels[tType]['radii']:
-            circle = plt.Circle(
-                (trap[0], trap[1]), r, 
-                color=col, fill=fill, ls=ls, 
-                lw=lws[1], zorder=zorders[1]
+        # Draw Circles
+        if latlon:
+            (gd, geoms) = (Geodesic(), [])
+            for r in trapsKernels[tType]['radii']:
+                cp = gd.circle(lon=trap[0], lat=trap[1], radius=r)
+                geoms.append(sgeom.Polygon(cp))
+            ax.add_geometries(
+                geoms, crs=ccrs.PlateCarree(), 
+                edgecolor='#00000000', color=col, 
+                zorder=zorders[1]
             )
-            ax.add_patch(circle)
+        else:
+            for r in trapsKernels[tType]['radii']:
+                circle = plt.Circle(
+                    (trap[0], trap[1]), r, 
+                    color=col, fill=fill, ls=ls, 
+                    lw=lws[1], zorder=zorders[1]
+                )
+                ax.add_patch(circle)
     return (fig, ax)
 
 
 def plotTrapsNetwork(
         fig, ax,
         transMtx, traps, sites,
         lineColor='#3d0e61', lineWidth=20, 
@@ -461,22 +473,23 @@
 
 def plotTrapsKernels(
         fig, ax, lnd,
         colors=cst.TRP_COLS, maxSca=5, alpha=.75,
         distRange=(0, 100), aspect=.3
     ):
     kers = lnd.trapsKernels
+    ktypes = list(lnd.trapsKernels.keys())
     # dMax = max(max([kers[i]['radii'] for i in range(len(kers))])) * maxSca
     dMax = distRange[1]
     # Generate figure
     for i in range(len(kers)):
         ker = kers[i]
         dists = np.arange(0, dMax+1, dMax/100)
         probs = [ker['kernel'](d, **ker['params']) for d in dists]
-        ax.plot(dists, probs, color=colors[i], lw=4, alpha=alpha)
+        ax.plot(dists, probs, color=colors[ktypes[i]], lw=4, alpha=alpha)
     ax.set_xlim(0, dMax)
     ax.set_ylim(0, 1)
     ax.set_aspect(aspect/ax.get_data_ratio())
     return (fig, ax)
 
 
 def plotsClearMemory():
```

### Comparing `MGSurvE-0.7.5.5/MGSurvE/pointProcess.py` & `MGSurvE-0.8.0.1/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-0.7.5.5/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-0.8.0.1/MGSurvE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 0.7.5.5
+Version: 0.8.0.1
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -45,14 +45,14 @@
 ![landscape](https://github.com/Chipdelmal/MGSurvE/raw/main/img/demo.jpg)
 
 # Authors and Funders
 
 <img src="https://raw.githubusercontent.com/Chipdelmal/pyMSync/master/media/pusheen.jpg" height="125px" align="middle"><img src="https://github.com/Chipdelmal/MGSurvE/blob/main/img/MGSurvE_Logo.png?raw=true" height="125px" align="middle"> <br><br>
 
 * Lead and Dev: [Héctor M. Sánchez C.](https://chipdelmal.github.io/blog/)
-* Active Devs: Elijah Bartolome, Lillian Weng, Ayden Salazar, Xingli Yu, Joanna Yoo, Topiltzin Hernandez
+* Former Devs: Elijah Bartolome, Lillian Weng, Ayden Salazar, Xingli Yu, Joanna Yoo, Topiltzin Hernandez
 * PIs: [David L. Smith](http://www.healthdata.org/about/david-smith), [John M. Marshall](https://publichealth.berkeley.edu/people/john-marshall/)
 
 <br>
 
 <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/berkeley.jpg" height="25px"> &nbsp; <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/IHME.jpg" height="25px"> &nbsp;  <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/IGI.png" height="25px"> &nbsp; <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/DARPA.jpg" height="25px"> &nbsp; <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/gates.jpg" height="25px">
```

### Comparing `MGSurvE-0.7.5.5/PKG-INFO` & `MGSurvE-0.8.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 0.7.5.5
+Version: 0.8.0.1
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -45,14 +45,14 @@
 ![landscape](https://github.com/Chipdelmal/MGSurvE/raw/main/img/demo.jpg)
 
 # Authors and Funders
 
 <img src="https://raw.githubusercontent.com/Chipdelmal/pyMSync/master/media/pusheen.jpg" height="125px" align="middle"><img src="https://github.com/Chipdelmal/MGSurvE/blob/main/img/MGSurvE_Logo.png?raw=true" height="125px" align="middle"> <br><br>
 
 * Lead and Dev: [Héctor M. Sánchez C.](https://chipdelmal.github.io/blog/)
-* Active Devs: Elijah Bartolome, Lillian Weng, Ayden Salazar, Xingli Yu, Joanna Yoo, Topiltzin Hernandez
+* Former Devs: Elijah Bartolome, Lillian Weng, Ayden Salazar, Xingli Yu, Joanna Yoo, Topiltzin Hernandez
 * PIs: [David L. Smith](http://www.healthdata.org/about/david-smith), [John M. Marshall](https://publichealth.berkeley.edu/people/john-marshall/)
 
 <br>
 
 <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/berkeley.jpg" height="25px"> &nbsp; <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/IHME.jpg" height="25px"> &nbsp;  <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/IGI.png" height="25px"> &nbsp; <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/DARPA.jpg" height="25px"> &nbsp; <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/gates.jpg" height="25px">
```

### Comparing `MGSurvE-0.7.5.5/README.md` & `MGSurvE-0.8.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,14 @@
 ![landscape](https://github.com/Chipdelmal/MGSurvE/raw/main/img/demo.jpg)
 
 # Authors and Funders
 
 <img src="https://raw.githubusercontent.com/Chipdelmal/pyMSync/master/media/pusheen.jpg" height="125px" align="middle"><img src="https://github.com/Chipdelmal/MGSurvE/blob/main/img/MGSurvE_Logo.png?raw=true" height="125px" align="middle"> <br><br>
 
 * Lead and Dev: [Héctor M. Sánchez C.](https://chipdelmal.github.io/blog/)
-* Active Devs: Elijah Bartolome, Lillian Weng, Ayden Salazar, Xingli Yu, Joanna Yoo, Topiltzin Hernandez
+* Former Devs: Elijah Bartolome, Lillian Weng, Ayden Salazar, Xingli Yu, Joanna Yoo, Topiltzin Hernandez
 * PIs: [David L. Smith](http://www.healthdata.org/about/david-smith), [John M. Marshall](https://publichealth.berkeley.edu/people/john-marshall/)
 
 <br>
 
 <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/berkeley.jpg" height="25px"> &nbsp; <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/IHME.jpg" height="25px"> &nbsp;  <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/IGI.png" height="25px"> &nbsp; <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/DARPA.jpg" height="25px"> &nbsp; <img src="https://github.com/Chipdelmal/MGSurvE/raw/main/img/gates.jpg" height="25px">
```

### Comparing `MGSurvE-0.7.5.5/setup.py` & `MGSurvE-0.8.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,25 @@
     author='Hector M. Sanchez C.',
     author_email='sanchez.hmsc@berkeley.edu',
     description="MGSurvE",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
-        'deap', 'numpy', 'scikit-learn', 'scipy', 'matplotlib', 'sympy',
+        'deap', 'numpy', 'scikit-learn', 'scipy', 'matplotlib==3.5.2', 'sympy',
         'ipython', 'jupyter', 'pandas', 'compress-pickle', 'dill', 
         'vincenty', 'haversine', 'networkx', 'pointpats', 'libpysal',
         'geopandas'
     ],
     extras_require={
-        'dev': ['pytest', 'twine', 'wheel', 'sphinx', 'sphinx_rtd_theme'],
+        'dev': [
+            'pytest', 'ipykernel'
+            'twine', 'wheel', 
+            'sphinx', 'sphinx_rtd_theme'
+        ],
     },
     license='GPLv3',
     classifiers=[
         'Programming Language :: Python :: 3.9',
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ]
```

