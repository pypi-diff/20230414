# Comparing `tmp/SPLayout-0.4.3.tar.gz` & `tmp/SPLayout-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SPLayout-0.4.3.tar", last modified: Fri Feb 24 04:33:58 2023, max compression
+gzip compressed data, was "dist\SPLayout-0.4.4.tar", last modified: Fri Apr 14 12:44:47 2023, max compression
```

## Comparing `SPLayout-0.4.3.tar` & `SPLayout-0.4.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 04:33:58.000000 SPLayout-0.4.3/
--rw-rw-rw-   0        0        0     2146 2023-02-24 04:33:58.000000 SPLayout-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     2433 2023-02-23 14:51:36.000000 SPLayout-0.4.3/README.md
--rw-rw-rw-   0        0        0     1473 2023-02-23 14:51:44.000000 SPLayout-0.4.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-24 04:33:58.000000 SPLayout-0.4.3/SPLayout.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-02-24 04:33:58.000000 SPLayout-0.4.3/SPLayout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2023-02-24 04:33:58.000000 SPLayout-0.4.3/SPLayout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 04:33:58.000000 SPLayout-0.4.3/SPLayout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-02-24 04:33:58.000000 SPLayout-0.4.3/SPLayout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-24 04:33:58.000000 SPLayout-0.4.3/SPLayout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-24 04:33:58.000000 SPLayout-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-02-23 14:06:17.000000 SPLayout-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-24 04:33:58.000000 SPLayout-0.4.3/splayout/
--rw-rw-rw-   0        0        0     1987 2023-02-24 04:33:15.000000 SPLayout-0.4.3/splayout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 04:33:58.000000 SPLayout-0.4.3/splayout/adjointmethod/
--rw-rw-rw-   0        0        0      293 2023-02-24 04:21:26.000000 SPLayout-0.4.3/splayout/adjointmethod/__init__.py
--rw-rw-rw-   0        0        0    10984 2023-02-23 12:33:21.000000 SPLayout-0.4.3/splayout/adjointmethod/adjointshapeopt.py
--rw-rw-rw-   0        0        0    10647 2023-02-24 04:32:00.000000 SPLayout-0.4.3/splayout/adjointmethod/adjointtopologyopt.py
--rw-rw-rw-   0        0        0    10586 2023-02-23 12:35:47.000000 SPLayout-0.4.3/splayout/adjointmethod/shaperegion2d.py
--rw-rw-rw-   0        0        0    10652 2023-02-23 12:35:57.000000 SPLayout-0.4.3/splayout/adjointmethod/shaperegion3d.py
--rw-rw-rw-   0        0        0    11374 2023-02-23 12:36:38.000000 SPLayout-0.4.3/splayout/adjointmethod/topologyregion2d.py
--rw-rw-rw-   0        0        0    11149 2023-02-24 02:38:35.000000 SPLayout-0.4.3/splayout/adjointmethod/topologyregion3d.py
-drwxrwxrwx   0        0        0        0 2023-02-24 04:33:58.000000 SPLayout-0.4.3/splayout/algorithms/
--rw-rw-rw-   0        0        0      312 2023-02-23 13:06:11.000000 SPLayout-0.4.3/splayout/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5781 2022-01-04 05:22:28.000000 SPLayout-0.4.3/splayout/algorithms/binarybatalgorithm.py
--rw-rw-rw-   0        0        0     6360 2022-01-04 06:04:34.000000 SPLayout-0.4.3/splayout/algorithms/binarygeneticalgorithm.py
--rw-rw-rw-   0        0        0     5831 2022-01-04 06:03:59.000000 SPLayout-0.4.3/splayout/algorithms/binaryparticleswarmalgorithm.py
--rw-rw-rw-   0        0        0     4305 2023-02-23 12:22:49.000000 SPLayout-0.4.3/splayout/algorithms/directbinarysearchalgorithm.py
--rw-rw-rw-   0        0        0     7333 2023-02-23 11:24:29.000000 SPLayout-0.4.3/splayout/algorithms/particleswarmalgorithm.py
-drwxrwxrwx   0        0        0        0 2023-02-24 04:33:58.000000 SPLayout-0.4.3/splayout/components/
--rw-rw-rw-   0        0        0     3728 2023-02-23 12:38:12.000000 SPLayout-0.4.3/splayout/components/AEMDgrating.py
--rw-rw-rw-   0        0        0      714 2023-02-23 13:44:58.000000 SPLayout-0.4.3/splayout/components/__init__.py
--rw-rw-rw-   0        0        0     4403 2023-02-23 12:38:42.000000 SPLayout-0.4.3/splayout/components/bend.py
--rw-rw-rw-   0        0        0     9026 2023-02-23 12:39:10.000000 SPLayout-0.4.3/splayout/components/doubleconnector.py
--rw-rw-rw-   0        0        0     6092 2023-02-23 12:42:22.000000 SPLayout-0.4.3/splayout/components/filledpattern.py
--rw-rw-rw-   0        0        0    49359 2023-02-23 12:42:22.000000 SPLayout-0.4.3/splayout/components/microring.py
--rw-rw-rw-   0        0        0    21403 2023-02-23 12:42:22.000000 SPLayout-0.4.3/splayout/components/pixelsregion.py
--rw-rw-rw-   0        0        0     7433 2023-02-23 12:41:22.000000 SPLayout-0.4.3/splayout/components/polygon.py
--rw-rw-rw-   0        0        0    14219 2023-02-23 12:42:22.000000 SPLayout-0.4.3/splayout/components/quarbend.py
--rw-rw-rw-   0        0        0    18098 2023-02-23 12:42:22.000000 SPLayout-0.4.3/splayout/components/sbend.py
--rw-rw-rw-   0        0        0    13136 2023-02-23 12:41:22.000000 SPLayout-0.4.3/splayout/components/selfdefinecomponent.py
--rw-rw-rw-   0        0        0    28052 2023-02-23 12:43:30.000000 SPLayout-0.4.3/splayout/components/simpleasymmetricdirectionalcoupler.py
--rw-rw-rw-   0        0        0     7270 2023-02-23 12:41:22.000000 SPLayout-0.4.3/splayout/components/slowlyvaryingtaper.py
--rw-rw-rw-   0        0        0     6668 2023-02-23 14:27:24.000000 SPLayout-0.4.3/splayout/components/taper.py
--rw-rw-rw-   0        0        0     1269 2023-02-23 12:41:22.000000 SPLayout-0.4.3/splayout/components/text.py
--rw-rw-rw-   0        0        0     8908 2023-02-23 12:42:22.000000 SPLayout-0.4.3/splayout/components/waveguide.py
-drwxrwxrwx   0        0        0        0 2023-02-24 04:33:58.000000 SPLayout-0.4.3/splayout/lumericalcommun/
--rw-rw-rw-   0        0        0       72 2023-02-23 12:26:37.000000 SPLayout-0.4.3/splayout/lumericalcommun/__init__.py
--rw-rw-rw-   0        0        0    74794 2023-02-23 12:42:48.000000 SPLayout-0.4.3/splayout/lumericalcommun/fdtdapi.py
--rw-rw-rw-   0        0        0    44213 2023-02-23 12:42:48.000000 SPLayout-0.4.3/splayout/lumericalcommun/modeapi.py
-drwxrwxrwx   0        0        0        0 2023-02-24 04:33:58.000000 SPLayout-0.4.3/splayout/utils/
--rw-rw-rw-   0        0        0       20 2023-02-23 12:27:14.000000 SPLayout-0.4.3/splayout/utils/__init__.py
--rw-rw-rw-   0        0        0     7931 2023-02-23 12:43:16.000000 SPLayout-0.4.3/splayout/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/
+-rw-rw-rw-   0        0        0     2146 2023-04-14 12:44:47.000000 SPLayout-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2433 2023-02-23 14:51:36.000000 SPLayout-0.4.4/README.md
+-rw-rw-rw-   0        0        0     1473 2023-02-23 14:51:44.000000 SPLayout-0.4.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 12:44:47.000000 SPLayout-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-02-23 14:06:17.000000 SPLayout-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/
+-rw-rw-rw-   0        0        0     1987 2023-04-14 12:44:18.000000 SPLayout-0.4.4/splayout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/adjointmethod/
+-rw-rw-rw-   0        0        0      293 2023-02-24 04:21:26.000000 SPLayout-0.4.4/splayout/adjointmethod/__init__.py
+-rw-rw-rw-   0        0        0    10984 2023-02-23 12:33:21.000000 SPLayout-0.4.4/splayout/adjointmethod/adjointshapeopt.py
+-rw-rw-rw-   0        0        0    10647 2023-02-24 04:32:00.000000 SPLayout-0.4.4/splayout/adjointmethod/adjointtopologyopt.py
+-rw-rw-rw-   0        0        0    10586 2023-02-23 12:35:47.000000 SPLayout-0.4.4/splayout/adjointmethod/shaperegion2d.py
+-rw-rw-rw-   0        0        0    10652 2023-02-23 12:35:57.000000 SPLayout-0.4.4/splayout/adjointmethod/shaperegion3d.py
+-rw-rw-rw-   0        0        0    11374 2023-02-23 12:36:38.000000 SPLayout-0.4.4/splayout/adjointmethod/topologyregion2d.py
+-rw-rw-rw-   0        0        0    11149 2023-02-24 02:38:35.000000 SPLayout-0.4.4/splayout/adjointmethod/topologyregion3d.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/algorithms/
+-rw-rw-rw-   0        0        0      312 2023-02-23 13:06:11.000000 SPLayout-0.4.4/splayout/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5781 2022-01-04 05:22:28.000000 SPLayout-0.4.4/splayout/algorithms/binarybatalgorithm.py
+-rw-rw-rw-   0        0        0     6360 2022-01-04 06:04:34.000000 SPLayout-0.4.4/splayout/algorithms/binarygeneticalgorithm.py
+-rw-rw-rw-   0        0        0     5831 2022-01-04 06:03:59.000000 SPLayout-0.4.4/splayout/algorithms/binaryparticleswarmalgorithm.py
+-rw-rw-rw-   0        0        0     4305 2023-02-23 12:22:49.000000 SPLayout-0.4.4/splayout/algorithms/directbinarysearchalgorithm.py
+-rw-rw-rw-   0        0        0     7333 2023-02-23 11:24:29.000000 SPLayout-0.4.4/splayout/algorithms/particleswarmalgorithm.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/components/
+-rw-rw-rw-   0        0        0     3728 2023-02-23 12:38:12.000000 SPLayout-0.4.4/splayout/components/AEMDgrating.py
+-rw-rw-rw-   0        0        0      714 2023-02-23 13:44:58.000000 SPLayout-0.4.4/splayout/components/__init__.py
+-rw-rw-rw-   0        0        0     4403 2023-02-23 12:38:42.000000 SPLayout-0.4.4/splayout/components/bend.py
+-rw-rw-rw-   0        0        0     9026 2023-02-23 12:39:10.000000 SPLayout-0.4.4/splayout/components/doubleconnector.py
+-rw-rw-rw-   0        0        0     6092 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/filledpattern.py
+-rw-rw-rw-   0        0        0    49359 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/microring.py
+-rw-rw-rw-   0        0        0    21403 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/pixelsregion.py
+-rw-rw-rw-   0        0        0     7433 2023-02-23 12:41:22.000000 SPLayout-0.4.4/splayout/components/polygon.py
+-rw-rw-rw-   0        0        0    14219 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/quarbend.py
+-rw-rw-rw-   0        0        0    18098 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/sbend.py
+-rw-rw-rw-   0        0        0    13136 2023-02-23 12:41:22.000000 SPLayout-0.4.4/splayout/components/selfdefinecomponent.py
+-rw-rw-rw-   0        0        0    28052 2023-02-23 12:43:30.000000 SPLayout-0.4.4/splayout/components/simpleasymmetricdirectionalcoupler.py
+-rw-rw-rw-   0        0        0     7270 2023-02-23 12:41:22.000000 SPLayout-0.4.4/splayout/components/slowlyvaryingtaper.py
+-rw-rw-rw-   0        0        0     6668 2023-02-23 14:27:24.000000 SPLayout-0.4.4/splayout/components/taper.py
+-rw-rw-rw-   0        0        0     1269 2023-02-23 12:41:22.000000 SPLayout-0.4.4/splayout/components/text.py
+-rw-rw-rw-   0        0        0     8908 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/waveguide.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/lumericalcommun/
+-rw-rw-rw-   0        0        0       72 2023-02-23 12:26:37.000000 SPLayout-0.4.4/splayout/lumericalcommun/__init__.py
+-rw-rw-rw-   0        0        0    75510 2023-04-14 12:41:11.000000 SPLayout-0.4.4/splayout/lumericalcommun/fdtdapi.py
+-rw-rw-rw-   0        0        0    44213 2023-02-23 12:42:48.000000 SPLayout-0.4.4/splayout/lumericalcommun/modeapi.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/utils/
+-rw-rw-rw-   0        0        0       20 2023-02-23 12:27:14.000000 SPLayout-0.4.4/splayout/utils/__init__.py
+-rw-rw-rw-   0        0        0     7931 2023-02-23 12:43:16.000000 SPLayout-0.4.4/splayout/utils/utils.py
```

### Comparing `SPLayout-0.4.3/PKG-INFO` & `SPLayout-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: SPLayout
-Version: 0.4.3
+Version: 0.4.4
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License: UNKNOWN
 Description: SPLayout
         ========
```

### Comparing `SPLayout-0.4.3/README.md` & `SPLayout-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/README.rst` & `SPLayout-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/SPLayout.egg-info/PKG-INFO` & `SPLayout-0.4.4/SPLayout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: SPLayout
-Version: 0.4.3
+Version: 0.4.4
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License: UNKNOWN
 Description: SPLayout
         ========
```

### Comparing `SPLayout-0.4.3/SPLayout.egg-info/SOURCES.txt` & `SPLayout-0.4.4/SPLayout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/setup.py` & `SPLayout-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/__init__.py` & `SPLayout-0.4.4/splayout/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 ## Submodules
 from . import utils
 from . import components
 from . import algorithms
 from . import lumericalcommun
 from . import adjointmethod
```

### Comparing `SPLayout-0.4.3/splayout/adjointmethod/adjointshapeopt.py` & `SPLayout-0.4.4/splayout/adjointmethod/adjointshapeopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/adjointmethod/adjointtopologyopt.py` & `SPLayout-0.4.4/splayout/adjointmethod/adjointtopologyopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/adjointmethod/shaperegion2d.py` & `SPLayout-0.4.4/splayout/adjointmethod/shaperegion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/adjointmethod/shaperegion3d.py` & `SPLayout-0.4.4/splayout/adjointmethod/shaperegion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/adjointmethod/topologyregion2d.py` & `SPLayout-0.4.4/splayout/adjointmethod/topologyregion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/adjointmethod/topologyregion3d.py` & `SPLayout-0.4.4/splayout/adjointmethod/topologyregion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/algorithms/binarybatalgorithm.py` & `SPLayout-0.4.4/splayout/algorithms/binarybatalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/algorithms/binarygeneticalgorithm.py` & `SPLayout-0.4.4/splayout/algorithms/binarygeneticalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/algorithms/binaryparticleswarmalgorithm.py` & `SPLayout-0.4.4/splayout/algorithms/binaryparticleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/algorithms/directbinarysearchalgorithm.py` & `SPLayout-0.4.4/splayout/algorithms/directbinarysearchalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/algorithms/particleswarmalgorithm.py` & `SPLayout-0.4.4/splayout/algorithms/particleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/AEMDgrating.py` & `SPLayout-0.4.4/splayout/components/AEMDgrating.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/__init__.py` & `SPLayout-0.4.4/splayout/components/__init__.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/bend.py` & `SPLayout-0.4.4/splayout/components/bend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/doubleconnector.py` & `SPLayout-0.4.4/splayout/components/doubleconnector.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/filledpattern.py` & `SPLayout-0.4.4/splayout/components/filledpattern.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/microring.py` & `SPLayout-0.4.4/splayout/components/microring.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/pixelsregion.py` & `SPLayout-0.4.4/splayout/components/pixelsregion.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/polygon.py` & `SPLayout-0.4.4/splayout/components/polygon.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/quarbend.py` & `SPLayout-0.4.4/splayout/components/quarbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/sbend.py` & `SPLayout-0.4.4/splayout/components/sbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/selfdefinecomponent.py` & `SPLayout-0.4.4/splayout/components/selfdefinecomponent.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/simpleasymmetricdirectionalcoupler.py` & `SPLayout-0.4.4/splayout/components/simpleasymmetricdirectionalcoupler.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/slowlyvaryingtaper.py` & `SPLayout-0.4.4/splayout/components/slowlyvaryingtaper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/taper.py` & `SPLayout-0.4.4/splayout/components/taper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/text.py` & `SPLayout-0.4.4/splayout/components/text.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/components/waveguide.py` & `SPLayout-0.4.4/splayout/components/waveguide.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/lumericalcommun/fdtdapi.py` & `SPLayout-0.4.4/splayout/lumericalcommun/fdtdapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,17 @@
         -----
         This function should be called after setting a source.
         """
         self.fdtd.eval("select(\"" + source_name + "\");")
         self.fdtd.eval("set(\"phase\"," +  "%.6f"%(phase) + ");")
 
 
-    def add_fdtd_region(self,bottom_left_corner_point,top_right_corner_point,simulation_time=5000,background_index=1.444,mesh_order =2,dimension=3,height = 1, z_min = None, z_max = None, z_symmetric = 0, y_antisymmetric = 0, y_periodic = 0, pml_layers = 8):
+    def add_fdtd_region(self,bottom_left_corner_point,top_right_corner_point,simulation_time=5000, background_material = None,
+                        background_index=1.444,mesh_order =2,dimension=3,height = 1, z_min = None,
+                        z_max = None, z_symmetric = 0, y_antisymmetric = 0, y_periodic = 0, pml_layers = 8):
         """
         Add simulation region in Lumerical FDTD.
 
         Parameters
         ----------
         bottom_left_corner_point : Point
             Lower left corner of the region.
@@ -507,14 +509,15 @@
             Whether set anti-symmetric in y-axis (default: 0).
         y_periodic : Bool or Int
             Whether set periodic in y-axis (default: 0).
 
         Notes
         -----
         If z_min and z_max are specified, the height property will be invalid.
+        If background_material is specified, the background_index will be invalid.
         """
         self.fdtd.eval("addfdtd;")
         self.fdtd.eval("set(\"dimension\"," + str(dimension-1) + ");")
         position = (bottom_left_corner_point + top_right_corner_point)/2
         x_span = abs(bottom_left_corner_point.x - top_right_corner_point.x)
         y_span = abs(bottom_left_corner_point.y - top_right_corner_point.y)
         self.fdtd.eval("set(\"x\"," +  "%.6f"%(position.x) + "e-6);")
@@ -524,15 +527,24 @@
         self.fdtd.eval("set(\"z\",0);")
         if (type(z_min) != type(None) and type(z_max) != type(None)):
             self.fdtd.eval("set(\"z min\"," + "%.6f" % (z_min) + "e-6);")
             self.fdtd.eval("set(\"z max\"," + "%.6f" % (z_max) + "e-6);")
         else:
             self.fdtd.eval("set(\"z span\"," + "%.6f" % (height) + "e-6);")
         self.fdtd.eval("set(\"simulation time\"," + str(simulation_time) + "e-15);")
-        self.fdtd.eval("set(\"index\"," +  str(background_index) + ");")
+        if not(background_material is None):
+            if type(background_material) == str:
+                self.fdtd.eval("set(\"background material\",\"" + background_material + "\");")
+            elif type(background_material) == float:
+                self.fdtd.eval("set(\"background material\",\"" + "<Object defined dielectric>" + "\");")
+                self.fdtd.eval("set(\"index\"," + str(background_material) + ");")
+            else:
+                raise Exception("Wrong background_material specification!")
+        else:
+            self.fdtd.eval("set(\"index\"," +  str(background_index) + ");")
         self.fdtd.eval("set(\"mesh accuracy\"," + str(mesh_order) + ");")
         self.fdtd.eval("set(\"pml layers\"," +str(pml_layers) +");")
 
         if (dimension == 3 and z_symmetric == 1):
             self.fdtd.eval("set(\"z min bc\", \"Symmetric\");")
 
         if (y_antisymmetric == 1):
```

### Comparing `SPLayout-0.4.3/splayout/lumericalcommun/modeapi.py` & `SPLayout-0.4.4/splayout/lumericalcommun/modeapi.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.3/splayout/utils/utils.py` & `SPLayout-0.4.4/splayout/utils/utils.py`

 * *Files identical despite different names*

