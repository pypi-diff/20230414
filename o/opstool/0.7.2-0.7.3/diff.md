# Comparing `tmp/opstool-0.7.2.tar.gz` & `tmp/opstool-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opstool-0.7.2.tar", last modified: Mon Apr  3 08:36:14 2023, max compression
+gzip compressed data, was "opstool-0.7.3.tar", last modified: Fri Apr 14 09:19:37 2023, max compression
```

## Comparing `opstool-0.7.2.tar` & `opstool-0.7.3.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 08:36:14.703420 opstool-0.7.2/
--rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.7.2/LICENCE.txt
--rw-rw-rw-   0        0        0     6415 2023-04-03 08:36:14.703420 opstool-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.7.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-03 08:36:14.703420 opstool-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-03 08:24:33.000000 opstool-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 08:36:14.672165 opstool-0.7.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-03 08:36:14.672165 opstool-0.7.2/src/opstool/
--rw-rw-rw-   0        0        0       23 2023-04-03 08:35:03.000000 opstool-0.7.2/src/opstool/__about__.py
--rw-rw-rw-   0        0        0      560 2023-03-30 08:46:47.000000 opstool-0.7.2/src/opstool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 08:36:14.687878 opstool-0.7.2/src/opstool/analysis/
--rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.7.2/src/opstool/analysis/__init__.py
--rw-rw-rw-   0        0        0    13381 2023-03-27 05:54:09.000000 opstool-0.7.2/src/opstool/analysis/_sec_analysis.py
--rw-rw-rw-   0        0        0    26992 2023-03-30 08:54:07.000000 opstool-0.7.2/src/opstool/analysis/_smart_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-03 08:36:14.687878 opstool-0.7.2/src/opstool/examples/
--rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.7.2/src/opstool/examples/ArchBridge.py
--rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.7.2/src/opstool/examples/ArchBridge2.py
--rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.7.2/src/opstool/examples/CableStayedBridge.py
--rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.7.2/src/opstool/examples/Dam.py
--rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.7.2/src/opstool/examples/DamBreak.py
--rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.7.2/src/opstool/examples/Frame3D.py
--rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.7.2/src/opstool/examples/Igloo.py
--rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.7.2/src/opstool/examples/Pier.py
--rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.7.2/src/opstool/examples/SDOF.py
--rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.7.2/src/opstool/examples/SuspensionBridge.py
--rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.7.2/src/opstool/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 08:36:14.687878 opstool-0.7.2/src/opstool/preprocessing/
--rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.7.2/src/opstool/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2895 2023-03-30 08:55:58.000000 opstool-0.7.2/src/opstool/preprocessing/geom_transf.py
--rw-rw-rw-   0        0        0     2493 2023-01-05 16:40:03.000000 opstool-0.7.2/src/opstool/preprocessing/load.py
-drwxrwxrwx   0        0        0        0 2023-04-03 08:36:14.703420 opstool-0.7.2/src/opstool/preprocessing/section/
--rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.7.2/src/opstool/preprocessing/section/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-02-02 07:11:35.000000 opstool-0.7.2/src/opstool/preprocessing/section/lib_sec_mesh.py
--rw-rw-rw-   0        0        0    56590 2023-04-03 08:34:27.000000 opstool-0.7.2/src/opstool/preprocessing/section/sec_mesh.py
--rw-rw-rw-   0        0        0    26259 2023-04-03 07:38:09.000000 opstool-0.7.2/src/opstool/preprocessing/section/var_sec_mesh.py
--rw-rw-rw-   0        0        0    53330 2023-03-30 08:56:24.000000 opstool-0.7.2/src/opstool/preprocessing/tcl2py.py
--rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.7.2/src/opstool/preprocessing/unit_system.py
--rw-rw-rw-   0        0        0     5537 2023-03-30 08:16:45.000000 opstool-0.7.2/src/opstool/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 08:36:14.703420 opstool-0.7.2/src/opstool/vis/
--rw-rw-rw-   0        0        0      383 2023-03-31 06:58:30.000000 opstool-0.7.2/src/opstool/vis/__init__.py
--rw-rw-rw-   0        0        0    28007 2023-04-03 07:01:49.000000 opstool-0.7.2/src/opstool/vis/_get_model_base.py
--rw-rw-rw-   0        0        0    92644 2023-04-02 10:48:07.000000 opstool-0.7.2/src/opstool/vis/_plotly_base.py
--rw-rw-rw-   0        0        0    54299 2023-04-03 07:58:18.000000 opstool-0.7.2/src/opstool/vis/_pyvista_base.py
--rw-rw-rw-   0        0        0    22925 2023-03-31 06:57:51.000000 opstool-0.7.2/src/opstool/vis/fiber_sec_vis.py
--rw-rw-rw-   0        0        0    32483 2023-04-03 07:55:07.000000 opstool-0.7.2/src/opstool/vis/get_model_data.py
--rw-rw-rw-   0        0        0    19962 2023-03-26 16:33:19.000000 opstool-0.7.2/src/opstool/vis/ops_vis_plotly.py
--rw-rw-rw-   0        0        0    20623 2023-04-03 07:58:18.000000 opstool-0.7.2/src/opstool/vis/ops_vis_pyvista.py
--rw-rw-rw-   0        0        0     9535 2023-03-30 09:08:16.000000 opstool-0.7.2/src/opstool/vis/save_tikz.py
-drwxrwxrwx   0        0        0        0 2023-04-03 08:36:14.687878 opstool-0.7.2/src/opstool.egg-info/
--rw-rw-rw-   0        0        0     6415 2023-04-03 08:36:14.000000 opstool-0.7.2/src/opstool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1427 2023-04-03 08:36:14.000000 opstool-0.7.2/src/opstool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 08:36:14.000000 opstool-0.7.2/src/opstool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-04-03 08:36:14.000000 opstool-0.7.2/src/opstool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-03 08:36:14.000000 opstool-0.7.2/src/opstool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.701786 opstool-0.7.3/
+-rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.7.3/LICENCE.txt
+-rw-rw-rw-   0        0        0     6415 2023-04-14 09:19:37.701786 opstool-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.7.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:19:37.701786 opstool-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-03 08:24:33.000000 opstool-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.672284 opstool-0.7.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.678043 opstool-0.7.3/src/opstool/
+-rw-rw-rw-   0        0        0       23 2023-04-14 08:52:08.000000 opstool-0.7.3/src/opstool/__about__.py
+-rw-rw-rw-   0        0        0      560 2023-03-30 08:46:47.000000 opstool-0.7.3/src/opstool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.682979 opstool-0.7.3/src/opstool/analysis/
+-rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.7.3/src/opstool/analysis/__init__.py
+-rw-rw-rw-   0        0        0    13381 2023-03-27 05:54:09.000000 opstool-0.7.3/src/opstool/analysis/_sec_analysis.py
+-rw-rw-rw-   0        0        0    32716 2023-04-14 09:17:06.000000 opstool-0.7.3/src/opstool/analysis/_smart_analyze.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.690699 opstool-0.7.3/src/opstool/examples/
+-rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.7.3/src/opstool/examples/ArchBridge.py
+-rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.7.3/src/opstool/examples/ArchBridge2.py
+-rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.7.3/src/opstool/examples/CableStayedBridge.py
+-rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.7.3/src/opstool/examples/Dam.py
+-rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.7.3/src/opstool/examples/DamBreak.py
+-rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.7.3/src/opstool/examples/Frame3D.py
+-rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.7.3/src/opstool/examples/Igloo.py
+-rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.7.3/src/opstool/examples/Pier.py
+-rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.7.3/src/opstool/examples/SDOF.py
+-rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.7.3/src/opstool/examples/SuspensionBridge.py
+-rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.7.3/src/opstool/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.692695 opstool-0.7.3/src/opstool/preprocessing/
+-rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.7.3/src/opstool/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2895 2023-03-30 08:55:58.000000 opstool-0.7.3/src/opstool/preprocessing/geom_transf.py
+-rw-rw-rw-   0        0        0     2493 2023-01-05 16:40:03.000000 opstool-0.7.3/src/opstool/preprocessing/load.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.695708 opstool-0.7.3/src/opstool/preprocessing/section/
+-rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.7.3/src/opstool/preprocessing/section/__init__.py
+-rw-rw-rw-   0        0        0     1396 2023-04-14 09:09:55.000000 opstool-0.7.3/src/opstool/preprocessing/section/lib_sec_mesh.py
+-rw-rw-rw-   0        0        0    56420 2023-04-14 09:13:37.000000 opstool-0.7.3/src/opstool/preprocessing/section/sec_mesh.py
+-rw-rw-rw-   0        0        0    26219 2023-04-14 09:14:18.000000 opstool-0.7.3/src/opstool/preprocessing/section/var_sec_mesh.py
+-rw-rw-rw-   0        0        0    53330 2023-03-30 08:56:24.000000 opstool-0.7.3/src/opstool/preprocessing/tcl2py.py
+-rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.7.3/src/opstool/preprocessing/unit_system.py
+-rw-rw-rw-   0        0        0     5547 2023-04-14 09:08:22.000000 opstool-0.7.3/src/opstool/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.701786 opstool-0.7.3/src/opstool/vis/
+-rw-rw-rw-   0        0        0      483 2023-04-14 08:10:34.000000 opstool-0.7.3/src/opstool/vis/__init__.py
+-rw-rw-rw-   0        0        0    28011 2023-04-14 08:54:12.000000 opstool-0.7.3/src/opstool/vis/_get_model_base.py
+-rw-rw-rw-   0        0        0    92757 2023-04-14 08:56:23.000000 opstool-0.7.3/src/opstool/vis/_plotly_base.py
+-rw-rw-rw-   0        0        0    55080 2023-04-14 08:59:00.000000 opstool-0.7.3/src/opstool/vis/_pyvista_base.py
+-rw-rw-rw-   0        0        0    22788 2023-04-14 09:02:37.000000 opstool-0.7.3/src/opstool/vis/fiber_sec_vis.py
+-rw-rw-rw-   0        0        0    32483 2023-04-14 09:04:43.000000 opstool-0.7.3/src/opstool/vis/get_model_data.py
+-rw-rw-rw-   0        0        0    19952 2023-04-14 09:05:35.000000 opstool-0.7.3/src/opstool/vis/ops_vis_plotly.py
+-rw-rw-rw-   0        0        0    20744 2023-04-14 09:06:18.000000 opstool-0.7.3/src/opstool/vis/ops_vis_pyvista.py
+-rw-rw-rw-   0        0        0     7508 2023-04-14 09:06:33.000000 opstool-0.7.3/src/opstool/vis/quick_plot.py
+-rw-rw-rw-   0        0        0     9535 2023-04-14 09:07:20.000000 opstool-0.7.3/src/opstool/vis/save_tikz.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.681032 opstool-0.7.3/src/opstool.egg-info/
+-rw-rw-rw-   0        0        0     6415 2023-04-14 09:19:37.000000 opstool-0.7.3/src/opstool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1457 2023-04-14 09:19:37.000000 opstool-0.7.3/src/opstool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:19:37.000000 opstool-0.7.3/src/opstool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-04-14 09:19:37.000000 opstool-0.7.3/src/opstool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 09:19:37.000000 opstool-0.7.3/src/opstool.egg-info/top_level.txt
```

### Comparing `opstool-0.7.2/LICENCE.txt` & `opstool-0.7.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/PKG-INFO` & `opstool-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.7.2
+Version: 0.7.3
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: OpenSees seismic visualization
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.7.2 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.7.3 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
 yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees seismic
 visualization Platform: any Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8.* Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
```

### Comparing `opstool-0.7.2/README.md` & `opstool-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/setup.py` & `opstool-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/__init__.py` & `opstool-0.7.3/src/opstool/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/analysis/_sec_analysis.py` & `opstool-0.7.3/src/opstool/analysis/_sec_analysis.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/analysis/_smart_analyze.py` & `opstool-0.7.3/src/opstool/analysis/_smart_analyze.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import time
 
 import numpy as np
 import openseespy.opensees as ops
 from rich import print
+
 from ..utils import _get_random_color
 
 
 class SmartAnalyze:
     """
     The SmartAnalyze is a class to provide OpenSeesPy users a easier
     way to conduct analyses.
@@ -24,15 +25,15 @@
     ----------------------------------------------
 
     TEST RELATED:
     ++++++++++++++
     testType: str, default="EnergyIncr"
         Identical to the testType in OpenSees test command.
         Choices see http://opensees.berkeley.edu/wiki/index.php/Test_Command.
-    testTol: float, default=1.0e-12
+    testTol: float, default=1.0e-10
         The initial test tolerance set to the OpenSees test command.
         If tryLooseTestTol is set to True, the test tolerance can be loosen.
     testIterTimes: int, default=10
         The initial number of test iteration times.
         If tryAddTestTimes is set to True, the number of test times can be enlarged.
     testPrintFlag: int, default=0
         The test print flag in OpenSees Test command.
@@ -46,83 +47,104 @@
         If unconverge, the last norm of test will be compared to `normTol`.
         If the norm is smaller, the number of test times will be enlarged.
     testIterTimesMore: int, default=50
         Only useful when tryaddTestTimes is True.
         If unconverge and norm is ok, the test iteration times will be set to this number.
     tryLooseTestTol: bool, default=False
         If this is set to True, if unconverge at minimum step,
-        the test tolerance will be loosen to the number specified by `looseTestTolTo`.the step will be set back.
-    looseTestTolTo: float, default=1.0
+        the test tolerance will be loosen to the number specified by `looseTestTolTo`.
+        the step will be set back.
+    looseTestTolTo: float, default= 100 * initial test tolerance
         Only useful if tryLooseTestTol is True.
         If unconvergance at the min step, the test tolerance will be set to this value.
 
     ALGORITHM RELATED:
     +++++++++++++++++++++++
     tryAlterAlgoTypes: bool, default=False
         If True, different algorithm types specified
         in `algoTypes` will be tried during unconvergance.
         If False, the first algorithm type specified in `algoTypes`
         will be used.
-    algoTypes: list[int], default=[10, 20, 30, 40, 50]
+    algoTypes: list[int], default=[40, 10, 20, 30, 50, 60, 70, 90]
         A list of flags of the algorithms to be used during unconvergance.
         The integer flag is documented in the following section.
         Only useful when tryAlterAlgoTypes is True.
-        The first flag will be used by default.
+        The first flag will be used by default when tryAlterAlgoTypes is False.
         The algorithm command in the model will be ignored.
         If you need other algorithm, try a user-defined algorithm. See the following section.
-
-    STEP RELATED:
-    +++++++++++++++++++++++
-    initialStep: float, default=None
-        Specifying the initial Step length to conduct analysis.
-        If None, equal to `dt`.
-    relaxation: float, between 0 and 1, default=0.5
-        A factor that is multiplied by each time
-        the step length is shortened.
-    minStep: float, default=1.e-6
-        The step tolerance when shortening
-        the step length.
-        If step length is smaller than minStep, special ways to converge the model will be used
-        according to `try-` flags.
-
-    LOGGING RELATED:
-    +++++++++++++++++++
-    printPer: int, default=10
-        Print to the console every several trials.
-    debugMode: bool, default=False
-        Print as much information as possible.
+    UserAlgoArgs: list, 
+        User-defined algorithm parameters, 100 is required in algoTypes,
+        and the parameters must be included in the list, for example:
+        algoTypes = [10, 20, 100],
+        UserAlgoArgs = ["KrylovNewton", "-iterate", "initial", "-maxDim", 20]
 
     .. tip::
         Algorithm type flag reference
         +++++++++++++++++++++++++++++++
         * 0:  Linear
         * 1:  Linear -initial
-        * 2:  Linear -factorOnce
+        * 2:  Linear -secant
+        * 3:  Linear -factorOnce
+        * 4:  Linear -initial -factorOnce
+        * 5:  Linear -secant -factorOnce
         * 10:  Newton
         * 11:  Newton -initial
         * 12:  Newton -initialThenCurrent
+        * 13:  Newton -Secant
         * 20:  NewtonLineSearch
         * 21:  NewtonLineSearch -type Bisection
         * 22:  NewtonLineSearch -type Secant
         * 23:  NewtonLineSearch -type RegulaFalsi
+        * 24:  NewtonLineSearch -type LinearInterpolated
+        * 25:  NewtonLineSearch -type InitialInterpolated
         * 30:  ModifiedNewton
         * 31:  ModifiedNewton -initial
+        * 32:  ModifiedNewton -secant
         * 40:  KrylovNewton
         * 41:  KrylovNewton -iterate initial
         * 42:  KrylovNewton -increment initial
         * 43:  KrylovNewton -iterate initial -increment initial
-        * 44:  KrylovNewton -maxDim 6
+        * 44:  KrylovNewton -maxDim 10
+        * 45:  KrylovNewton -iterate initial -increment initial -maxDim 10
         * 50:  SecantNewton
         * 51:  SecantNewton -iterate initial
         * 52:  SecantNewton -increment initial
         * 53:  SecantNewton -iterate initial -increment initial
         * 60:  BFGS
+        * 61:  BFGS -initial
+        * 62:  BFGS -secant
         * 70:  Broyden
+        * 71:  Broyden -initial
+        * 72:  Broyden -secant
         * 80:  PeriodicNewton
-        * 90:  User-defined0
+        * 81:  PeriodicNewton -maxDim 10
+        * 90:  ExpressNewton
+        * 91:  ExpressNewton -InitialTangent
+        * 100:  User-defined0
+
+    STEP RELATED:
+    +++++++++++++++++++++++
+    initialStep: float, default=None
+        Specifying the initial Step length to conduct analysis.
+        If None, equal to `dt`.
+    relaxation: float, between 0 and 1, default=0.5
+        A factor that is multiplied by each time
+        the step length is shortened.
+    minStep: float, default=1.e-6
+        The step tolerance when shortening
+        the step length.
+        If step length is smaller than minStep, special ways to converge the model will be used
+        according to `try-` flags.
+
+    LOGGING RELATED:
+    +++++++++++++++++++
+    printPer: int, default=50
+        Print to the console every several trials.
+    debugMode: bool, default=False
+        Print as much information as possible.
 
     Examples
     ---------
     .. note::
         ``test()`` and ``algorithm()`` will run automatically in ``SmartAnalyze``,
         but commands such as ``integrator()`` must be defined outside ``SmartAnalyze``.
 
@@ -145,56 +167,60 @@
     >>> import opstool as opst
     >>> ops.constraints('Transformation')
     >>> ops.numberer('Plain')
     >>> ops.system('BandGeneral')
     >>> protocol=[1, -1, 1, -1, 0]
     >>> analysis = opst.SmartAnalyze(analysis_type="Static")
     >>> segs = analysis.static_split(protocol, 0.01)
+    >>> print(segs)
     >>> for seg in segs:
-    >>>     analysis.StaticAnalyze(1, 1, seg)
+    >>>     analysis.StaticAnalyze(1, 2, seg)  # node tag 1, dof 2
 
     Example 3: change control parameters
     ++++++++++++++++++++++++++++++++++++++
     >>> analysis = opst.SmartAnalyze(analysis_type="Transient",
-    >>>                              algoTypes=[20, 30],
+    >>>                              algoTypes=[40, 30, 20],
     >>>                              printPer=20,
     >>>                              tryAlterAlgoTypes=True,
     >>>                             )
     """
 
     def __init__(self, analysis_type="Transient", **kargs):
         if analysis_type not in ("Transient", "Static"):
             raise ValueError("analysis_type must Transient or Static!")
         # default
-        self.control = {'analysis': analysis_type, 'testType': "EnergyIncr", 'testTol': 1.0e-12,
+        self.control = {'analysis': analysis_type, 'testType': "EnergyIncr", 'testTol': 1.0e-10,
                         'testIterTimes': 10, 'testPrintFlag': 0, 'tryAddTestTimes': False,
                         'normTol': 1.0e3, 'testIterTimesMore': 50, 'tryLooseTestTol': False,
-                        'looseTestTolTo': 1.0, 'tryAlterAlgoTypes': False, 'algoTypes': [10, 20, 30, 40, 50],
+                        'looseTestTolTo': 1.0, 'tryAlterAlgoTypes': False,
+                        'algoTypes': [40, 10, 20, 30, 50, 60, 70, 90], "UserAlgoArgs": None,
                         'initialStep': None, 'relaxation': 0.5, 'minStep': 1.0e-6,
-                        'printPer': 10, 'debugMode': False}
+                        'printPer': 50, 'debugMode': False}
+        self.control['looseTestTolTo'] = 100 * self.control['testTol']
         for name in kargs.keys():
             if name not in self.control.keys():
                 raise ValueError(f"arg {name} error!")
         self.control.update(kargs)
         self.eps = 1.E-12
         self.logo = "[bold magenta]SmartAnalyze:[/bold magenta]"
 
         # initial test commands
         ops.test(self.control['testType'], self.control['testTol'],
                  self.control['testIterTimes'], self.control['testPrintFlag'])
-        self._setAlgorithm(self.control['algoTypes'][0])
+        self._setAlgorithm(self.control['algoTypes'][0], self.control["UserAlgoArgs"])
 
         self.current = {'startTime': time.time(), 'algoIndex': 0,
                         'testIterTimes': self.control['testIterTimes'],
                         'testTol': self.control['testTol'], 'counter': 0,
                         'progress': 0, 'segs': 0, 'step': 0.0,
                         'node': 0, 'dof': 0}
 
     def transient_split(self, npts: int):
         """Step Segmentation for Transient Analysis.
+        It is not necessary to use this method.
 
         Parameters
         ----------
         npts : int
             Total steps for transient analysis.
 
         Returns
@@ -202,14 +228,15 @@
         A list to loop.
         """
         self.current['segs'] = npts
         return list(range(1, npts + 1))
 
     def static_split(self, targets: list, maxStep: float = None):
         """Returns a sequence of substeps for static analysis, for use in outer analysis loops.
+        It is not necessary to use this method if you already have a load sequence.
 
         Parameters
         ----------
         targets: list
             A list of target displacements, the first element must be positive.
         maxStep: float, default=None
             The maximum step length in the displacement control.
@@ -217,22 +244,22 @@
 
         Returns
         -------
         segs: list
             A sequence of substeps for static analysis.
 
         """
-        targets = np.array(targets)
+        targets = np.atleast_1d(targets)
         if targets.ndim != 1:
             raise ValueError("targets must be 1D!")
         if len(targets) == 1 and maxStep is None:
             raise ValueError(
                 "When targets has only one element, maxStep must be passed in!")
         if targets[0] != 0.0:
-            targets = np.insert(targets, 0, 0)
+            targets = np.insert(targets, 0, 0.0)
         if maxStep is None:
             maxStep = targets[1] - targets[0]
         # calcuate whole distance; divide the whole process into segments.
         distance = 0
         segs = []
         for i in range(len(targets) - 1):
             section = targets[i + 1] - targets[i]
@@ -269,64 +296,69 @@
         Parameters
         ----------
         dt : float
             Time Step.
 
         Returns
         -------
-        None
+        Return 0 if successful, otherwise returns a negative number.
         """
         if self.control['analysis'] != "Transient":
-            raise ValueError("Transient! Please check parameter set!")
+            raise ValueError("Transient! Please check parameter input!")
         self.control['initialStep'] = dt
 
         ops.analysis(self.control['analysis'])
 
         ok = self._RecursiveAnalyze(self.control['initialStep'], 0, self.control['testIterTimes'],
                                     self.control['testTol'], self.control.copy(), self.current.copy())
         if ok < 0:
             color = _get_random_color()
             custime = f"[{color}]{self._get_time():.3f}[/{color}]"
             print(
                 f">>> {self.logo} Analyze failed. Time consumption: {custime} s.")
             return ok
 
         self.current['progress'] += 1
-
-        if self.control['debugMode']:
-            if self.current['segs'] is not None:
-                color = _get_random_color()
-                custime = f"[{color}]{100 * self.current['progress'] / self.current['segs']:.3f}[/{color}]"
-                print(f"*** {self.logo} progress {custime} %")
-
-        if self.current['progress'] == self.current['segs']:
+        self.current['counter'] += 1
+        if self.current['segs'] > 0:
+            color = _get_random_color()
+            if self.control['debugMode']:
+                value1 = f"[bold {color}]{100 * self.current['progress'] / self.current['segs']:.3f}[/bold {color}]"
+                value2 = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
+                print(f"* {self.logo} progress {value1} %. Time consumption: {value2} s.")
+            elif self.current['counter'] >= self.control['printPer']:
+                value1 = f"[bold {color}]{100 * self.current['progress'] / self.current['segs']:.3f}[/bold {color}]"
+                value2 = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
+                print(f"* {self.logo} progress {value1} %. Time consumption: {value2} s.")
+                self.current['counter'] = 0
+        if (self.current['segs'] > 0) and (self.current['progress'] >= self.current['segs']):
             color = _get_random_color()
             custime = f"[{color}]{self._get_time():.3f}[/{color}]"
             print(
                 f">>> {self.logo} [{color}]Successfully finished[/{color}]! Time consumption: {custime} s.")
             return 0
 
     def StaticAnalyze(self, node: int, dof: int, seg: float):
-        """Single Step Static Analysis.
+        """Single step static analysis and applies to displacement control only.
 
         Parameters
         ----------
         node : int
             The node tag in the displacement control.
         dof : int
             The dof in the displacement control.
         seg : float
             Each load step, i.e. each element returned by static_split.
 
         Returns
         -------
-        None
+        Return 0 if successful, otherwise returns a negative number.
         """
         if self.control['analysis'] != "Static":
-            raise ValueError("Static! Please check parameter set!")
+            raise ValueError("Static! Please check parameter input!")
         self.control['initialStep'] = seg
         self.current['node'] = node
         self.current['dof'] = dof
         self.current['step'] = seg
 
         ops.integrator('DisplacementControl', node, dof, seg)
         ops.analysis(self.control['analysis'])
@@ -334,28 +366,35 @@
         ok = self._RecursiveAnalyze(seg, 0, self.control['testIterTimes'], self.control['testTol'],
                                     self.control.copy(), self.current.copy())
         if ok < 0:
             color = _get_random_color()
             value = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
             print(
                 f">>> {self.logo} Analyze failed. Time consumption: {value} s.")
-            return ok
+            return -1
         self.current['progress'] += 1
-
-        if self.control['debugMode']:
+        self.current['counter'] += 1
+        if self.current['segs'] > 0:
             color = _get_random_color()
-            value = f"[bold {color}]{100 * self.current['progress'] / self.current['segs']:.2f}[/bold {color}]"
-            print(f"*** {self.logo} progress {value} %")
+            if self.control['debugMode']:
+                value1 = f"[bold {color}]{100 * self.current['progress'] / self.current['segs']:.3f}[/bold {color}]"
+                value2 = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
+                print(f"* {self.logo} progress {value1} %. Time consumption: {value2} s.")
+            elif self.current['counter'] >= self.control['printPer']:
+                value1 = f"[bold {color}]{100 * self.current['progress'] / self.current['segs']:.3f}[/bold {color}]"
+                value2 = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
+                print(f"* {self.logo} progress {value1} %. Time consumption: {value2} s.")
+                self.current['counter'] = 0
 
-        if self.current['progress'] == self.current['segs']:
+        if (self.current['segs'] > 0) and (self.current['progress'] >= self.current['segs']):
             color = _get_random_color()
             value = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
             print(
                 f">>> {self.logo} [{color}]Successfully finished[/{color}]! Time consumption: {value} s.")
-            return 0
+        return 0
 
     def _RecursiveAnalyze(self, step: float, algoIndex: int,
                           testIterTimes: int, testTol: float,
                           vcontrol: dict, vcurrent: dict):
         """RecursiveAnalyze.
 
         Parameters
@@ -379,39 +418,38 @@
         -------
         int
             Analysis flag, if < 0, analysis failed; elsewise = 0 success.
         """
 
         if vcontrol['debugMode']:
             color = _get_random_color()
-            values = f"[bold {color}]step=%.3e, algoI=%i, times=%i, tol=%.3e[/bold {color}]" % (
-                step, algoIndex, testIterTimes, testTol)
+            values = f"[bold {color}]step=%.3e, algoIndex=%i, testIterTimes=%i, testTol=%.3e[/bold {color}]" % (
+                step, vcontrol['algoTypes'][algoIndex], testIterTimes, testTol)
             print(f"*** {self.logo} Run Recursive: {values}\n")
 
         if algoIndex != vcurrent['algoIndex']:
             color = _get_random_color()
             values = f"[bold {color}]%i[/bold {color}]" % (
                 vcontrol['algoTypes'][algoIndex])
             print(f">>> {self.logo} Setting algorithm to {values}\n")
-            self._setAlgorithm(vcontrol['algoTypes'][algoIndex])
+            self._setAlgorithm(vcontrol['algoTypes'][algoIndex], self.control["UserAlgoArgs"])
             vcurrent['algoIndex'] = algoIndex
 
         if testIterTimes != vcurrent['testIterTimes'] or testTol != vcurrent['testTol']:
             if testIterTimes != vcurrent['testIterTimes']:
                 color = _get_random_color()
                 values = f"[bold {color}]%i[/bold {color}]" % testIterTimes
                 print(
                     f">>> {self.logo} Setting test iteration times to {values}\n")
                 vcurrent['testIterTimes'] = testIterTimes
             if testTol != vcurrent['testTol']:
                 color = _get_random_color()
                 print(
                     f">>> {self.logo} Setting test tolerance to [bold {color}]%f[/bold {color}]\n" % testTol)
                 vcurrent['testTol'] = testTol
-
             ops.test(vcontrol['testType'], testTol,
                      testIterTimes, vcontrol['testPrintFlag'])
         # static step size
         if vcontrol['analysis'] == 'Static' and vcurrent['step'] != step:
             color = _get_random_color()
             print(
                 f">>> {self.logo} Setting step to [bold {color}]%.3e[/bold {color}]\n" % step)
@@ -419,24 +457,15 @@
                            vcurrent['node'], vcurrent['dof'], step)
             vcurrent['step'] = step
         # trial analyze once
         if vcontrol['analysis'] == 'Static':
             ok = ops.analyze(1)
         else:
             ok = ops.analyze(1, step)
-        vcurrent['counter'] += 1
         if ok == 0:
-            if vcurrent['counter'] >= vcontrol['printPer']:
-                if vcurrent['segs'] is not None:
-                    color = _get_random_color()
-                    value1 = f"[bold {color}]{100 * vcurrent['progress'] / vcurrent['segs']:.2f}[/bold {color}]"
-                    value2 = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
-                    print(
-                        f"* {self.logo} progress {value1} %. Time consumption: {value2} s.")
-                vcurrent['counter'] = 0
             return 0
         # If not convergence, add test iteration times. Use current step, algorithm and test tolerance.
         if vcontrol['tryAddTestTimes'] and testIterTimes != vcontrol['testIterTimesMore']:
             norm = ops.testNorm()
             color = _get_random_color()
             if norm[-1] < vcontrol['normTol']:
                 print(f">>> {self.logo} Adding test times to [bold {color}]%i[/bold {color}].\n" % (
@@ -452,183 +481,258 @@
             algoIndex += 1
             color = _get_random_color()
             print(f">>> {self.logo} Setting algorithm to [bold {color}]%i[/bold {color}].\n" % (
                 vcontrol['algoTypes'][algoIndex]))
             return self._RecursiveAnalyze(step, algoIndex, testIterTimes, testTol, vcontrol, vcurrent)
 
         # If step length is too small, try add test tolerance. set algorithm and test iteration times back.
-        if np.abs(step) < 2 * vcontrol['minStep']:
+        # Split the current step into two steps.
+        stepNew = step * vcontrol['relaxation']
+        if 0 < stepNew < vcontrol['minStep']:
+            stepNew = vcontrol['minStep']
+        if 0 > stepNew > -vcontrol['minStep']:
+            stepNew = -vcontrol['minStep']
+        if np.abs(stepNew) < vcontrol['minStep']:
             color = _get_random_color()
             print(
-                f">>> {self.logo} current step [bold {color}]%.3e[/bold {color}] beyond the min step!\n" % step)
+                f">>> {self.logo} current step [bold {color}]%.3e[/bold {color}] beyond the min step!\n" % stepNew)
             if vcontrol['tryLooseTestTol'] and vcurrent['testTol'] != vcontrol['looseTestTolTo']:
                 print(
                     f"!!! {self.logo} Warning: [bold {color}]Loosing test tolerance[/bold {color}]\n")
                 return self._RecursiveAnalyze(step, 0, vcontrol['testIterTimes'],
                                               vcontrol['looseTestTolTo'], vcontrol, vcurrent)
             # Here, all methods have been tried. Return negative value.
             return -1
 
-        # Split the current step into two steps.
-        stepNew = step * vcontrol['relaxation']
-        if 0 < stepNew < vcontrol['minStep']:
-            stepNew = vcontrol['minStep']
-        if 0 > stepNew > -vcontrol['minStep']:
-            stepNew = -vcontrol['minStep']
-
         stepRest = step - stepNew
         color = _get_random_color()
         print(f">>> {self.logo} Dividing the current step [bold {color}]%.3e into %.3e and %.3e[/bold {color}]\n" % (
             step, stepNew, stepRest))
         ok = self._RecursiveAnalyze(
             stepNew, 0, testIterTimes, testTol, vcontrol, vcurrent)
         if ok < 0:
             return -1
         ok = self._RecursiveAnalyze(
             stepRest, 0, testIterTimes, testTol, vcontrol, vcurrent)
         if ok < 0:
             return -1
         return 0
 
-    def _setAlgorithm(self, algotype):
+    def _setAlgorithm(self, algotype, user_algo_args: list = None):
         color = _get_random_color()
 
         def case0():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]Linear ...[/bold {color}]")
             ops.algorithm('Linear')
 
         def case1():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]Linear -initial ...[/bold {color}]")
-            ops.algorithm('Linear', True, False)
+            ops.algorithm('Linear', "-Initial")
 
         def case2():
             print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -secant ...[/bold {color}]")
+            ops.algorithm('Linear', "-Secant")
+
+        def case3():
+            print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]Linear -factorOnce ...[/bold {color}]")
-            ops.algorithm('Linear', False, True)
+            ops.algorithm('Linear', "-FactorOnce")
+
+        def case4():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -initial -factorOnce ...[/bold {color}]")
+            ops.algorithm('Linear', "-Initial", "-FactorOnce")
+
+        def case5():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -secant -factorOnce ...[/bold {color}]")
+            ops.algorithm('Linear', "-Secant", "-FactorOnce")
 
         def case10():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]Newton ...[/bold {color}]")
             ops.algorithm('Newton')
 
         def case11():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]Newton -initial ...[/bold {color}]")
-            ops.algorithm('Newton', False, True, False)
+            ops.algorithm('Newton', "-Initial")
 
         def case12():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]Newton -initialThenCurrent ...[/bold {color}]")
-            ops.algorithm('Newton', False, False, True)
+            ops.algorithm('Newton', "-intialThenCurrent")
+
+        def case13():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]Newton -Secant ...[/bold {color}]")
+            ops.algorithm('Newton', "-Secant")
 
         def case20():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]NewtonLineSearch ...[/bold {color}]")
             ops.algorithm('NewtonLineSearch')
 
         def case21():
             print(f"> {self.logo} Setting algorithm to "
                   f"[bold {color}]NewtonLineSearch -type Bisection ...[/bold {color}]")
-            ops.algorithm('NewtonLineSearch', True)
+            ops.algorithm('NewtonLineSearch', "-type", "Bisection")
 
         def case22():
             print(f"> {self.logo} Setting algorithm to "
                   f"[bold {color}]NewtonLineSearch -type Secant ...[/bold {color}]")
-            ops.algorithm('NewtonLineSearch', False, True)
+            ops.algorithm('NewtonLineSearch', "-type", "Secant")
 
         def case23():
             print(f"> {self.logo} Setting algorithm to "
                   f"[bold {color}]NewtonLineSearch -type RegulaFalsi ...[/bold {color}]")
-            ops.algorithm('NewtonLineSearch', False, False, True)
+            ops.algorithm('NewtonLineSearch', "-type", "RegulaFalsi")
+
+        def case24():
+            print(f"> {self.logo} Setting algorithm to "
+                  f"[bold {color}]NewtonLineSearch -type LinearInterpolated ...[/bold {color}]")
+            ops.algorithm('NewtonLineSearch', "-type", "LinearInterpolated")
+
+        def case25():
+            print(f"> {self.logo} Setting algorithm to "
+                  f"[bold {color}]NewtonLineSearch -type InitialInterpolated ...[/bold {color}]")
+            ops.algorithm('NewtonLineSearch', "-type", "InitialInterpolated")
 
         def case30():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]Modified Newton ...[/bold {color}]")
             ops.algorithm('ModifiedNewton')
 
         def case31():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]ModifiedNewton -initial ...[/bold {color}]")
-            ops.algorithm('ModifiedNewton', False, True)
+            ops.algorithm('ModifiedNewton', "-initial")
+
+        def case32():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]ModifiedNewton -secant ...[/bold {color}]")
+            ops.algorithm('ModifiedNewton', "-secant")
 
         def case40():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]KrylovNewton ...[/bold {color}]")
             ops.algorithm('KrylovNewton')
 
         def case41():
             print(f"> {self.logo} Setting algorithm to "
                   f"[bold {color}]KrylovNewton -iterate initial ...[/bold {color}]")
-            ops.algorithm('KrylovNewton', 'initial')
+            ops.algorithm('KrylovNewton', "-iterate", 'initial')
 
         def case42():
             print(f"> {self.logo} Setting algorithm to "
                   f"[bold {color}]KrylovNewton -increment initial ...[/bold {color}]")
-            ops.algorithm('KrylovNewton', 'current', 'initial')
+            ops.algorithm('KrylovNewton', "-increment", 'initial')
 
         def case43():
             print(f"> {self.logo} Setting algorithm to "
                   f"[bold {color}]KrylovNewton -iterate initial -increment initial ...[/bold {color}]")
-            ops.algorithm('KrylovNewton', 'initial', 'initial')
+            ops.algorithm('KrylovNewton', "-iterate", 'initial', "-increment", 'initial')
 
         def case44():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]KrylovNewton -maxDim 50[/bold {color}]")
-            ops.algorithm('KrylovNewton', 'current', 'current', 50)
+                f"> {self.logo} Setting algorithm to  [bold {color}]KrylovNewton -maxDim 10[/bold {color}]")
+            ops.algorithm('KrylovNewton', "-maxDim", 10)
 
         def case45():
             print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]KrylovNewton -iterate initial -increment initial -maxDim 50[/bold {color}]")
-            ops.algorithm('KrylovNewton', 'initial', 'initial', 50)
+                  f"[bold {color}]KrylovNewton -iterate initial -increment initial -maxDim 10[/bold {color}]")
+            ops.algorithm('KrylovNewton', "-iterate", 'initial', "-increment", 'initial', "-maxDim", 10)
 
         def case50():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]SecantNewton ...[/bold {color}]")
             ops.algorithm('SecantNewton')
 
         def case51():
             print(f"> {self.logo} Setting algorithm to "
                   f"[bold {color}]SecantNewton -iterate initial ...[/bold {color}]")
-            ops.algorithm('SecantNewton', 'initial')
+            ops.algorithm('SecantNewton', "-iterate", 'initial')
 
         def case52():
             print(f"> {self.logo} Setting algorithm to "
                   f"[bold {color}]SecantNewton -increment initial  ...[/bold {color}]")
-            ops.algorithm('SecantNewton', 'current', 'initial')
+            ops.algorithm('SecantNewton', "-increment", 'initial')
 
         def case53():
             print(f"> {self.logo} Setting algorithm to "
                   f"[bold {color}]SecantNewton -iterate initial -increment initial ...[/bold {color}]")
-            ops.algorithm('SecantNewton', 'initial', 'initial')
+            ops.algorithm('SecantNewton', "-iterate", 'initial', "-increment", 'initial')
 
         def case60():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]BFGS ...[/bold {color}]")
             ops.algorithm('BFGS')
 
+        def case61():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]BFGS -initial...[/bold {color}]")
+            ops.algorithm('BFGS', "-initial")
+
+        def case62():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]BFGS -secant ...[/bold {color}]")
+            ops.algorithm('BFGS', "-secant")
+
         def case70():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]Broyden ...[/bold {color}]")
             ops.algorithm('Broyden')
 
+        def case71():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]Broyden -initial ...[/bold {color}]")
+            ops.algorithm('Broyden', "-initial")
+
+        def case72():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]Broyden -secant ...[/bold {color}]")
+            ops.algorithm('Broyden', "-secant")
+
         def case80():
             print(
                 f"> {self.logo} Setting algorithm to  [bold {color}]PeriodicNewton ...[/bold {color}]")
             ops.algorithm('PeriodicNewton')
 
+        def case81():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]PeriodicNewton -maxDim, 10 ...[/bold {color}]")
+            ops.algorithm('PeriodicNewton', "-maxDim", 10)
+
         def case90():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]ExpressNewton ...[/bold {color}]")
+            ops.algorithm('ExpressNewton')
+
+        def case91():
+            print(
+                f"> {self.logo} Setting algorithm to  [bold {color}]ExpressNewton -InitialTangent ...[/bold {color}]")
+            ops.algorithm('ExpressNewton', "-InitialTangent")
+
+        def case100():
             # User algorithm0
-            pass
+            if user_algo_args is not None:
+                ops.algorithm(*user_algo_args)
 
         def default():
             raise ValueError("!!! SmartAnalyze: ERROR! WRONG Algorithm Type!")
 
-        switch = {0: case0, 1: case1, 2: case2, 10: case10, 11: case11, 12: case12,
-                  20: case20, 21: case21, 22: case22, 23: case23,
-                  30: case30, 31: case31,
+        switch = {0: case0, 1: case1, 2: case2, 3: case3, 4: case4, 5: case5,
+                  10: case10, 11: case11, 12: case12, 13: case13,
+                  20: case20, 21: case21, 22: case22, 23: case23, 24: case24, 25: case25,
+                  30: case30, 31: case31, 32: case32,
                   40: case40, 41: case41, 42: case42, 43: case43, 44: case44, 45: case45,
                   50: case50, 51: case51, 52: case52, 53: case53,
-                  60: case60, 70: case70, 80: case80, 90: case90}
+                  60: case60, 61: case61, 62: case62,
+                  70: case70, 71: case71, 72: case72,
+                  80: case80, 81: case81,
+                  90: case90, 91: case91,
+                  100: case100}
 
         switch.get(algotype, default)()
```

### Comparing `opstool-0.7.2/src/opstool/examples/ArchBridge.py` & `opstool-0.7.3/src/opstool/examples/ArchBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/examples/ArchBridge2.py` & `opstool-0.7.3/src/opstool/examples/ArchBridge2.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/examples/CableStayedBridge.py` & `opstool-0.7.3/src/opstool/examples/CableStayedBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/examples/Dam.py` & `opstool-0.7.3/src/opstool/examples/Dam.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/examples/DamBreak.py` & `opstool-0.7.3/src/opstool/examples/DamBreak.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/examples/Frame3D.py` & `opstool-0.7.3/src/opstool/examples/Frame3D.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/examples/Igloo.py` & `opstool-0.7.3/src/opstool/examples/Igloo.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/examples/Pier.py` & `opstool-0.7.3/src/opstool/examples/Pier.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/examples/SDOF.py` & `opstool-0.7.3/src/opstool/examples/SDOF.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/examples/SuspensionBridge.py` & `opstool-0.7.3/src/opstool/examples/SuspensionBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/preprocessing/__init__.py` & `opstool-0.7.3/src/opstool/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/preprocessing/geom_transf.py` & `opstool-0.7.3/src/opstool/preprocessing/geom_transf.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/preprocessing/load.py` & `opstool-0.7.3/src/opstool/preprocessing/load.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/preprocessing/section/__init__.py` & `opstool-0.7.3/src/opstool/preprocessing/section/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/preprocessing/section/lib_sec_mesh.py` & `opstool-0.7.3/src/opstool/preprocessing/section/lib_sec_mesh.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/preprocessing/section/sec_mesh.py` & `opstool-0.7.3/src/opstool/preprocessing/section/sec_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,30 +54,30 @@
         # * section geo props
         self.sec_props = dict()
         self.frame_sec_props = dict()
 
         self.color_map = dict()
         self.is_centring = False
 
-    def assign_group(self, group: dict[str, any]):
+    def assign_group(self, group: dict):
         """Assign the group dict for each mesh.
 
         Parameters
         ------------
-        group : dict
+        group : dict[str, any]
             A dict of name as key, geometry obj as value.
 
         Returns
         ----------
         instance
         """
         self.group_map = group
         return self
 
-    def assign_mesh_size(self, mesh_size: dict[str, float]):
+    def assign_mesh_size(self, mesh_size: dict):
         """Assign the mesh size dict for each mesh.
 
         Parameters
         ------------
         mesh_size : dict[str, float]
             A dict of name as key, mesh size as value.
 
@@ -91,15 +91,15 @@
             if name not in self.group_map.keys():
                 raise ValueError(
                     f"{name} is not specified in the assign_group function!"
                 )
         self.mesh_size_map = mesh_size
         return self
 
-    def assign_ops_matTag(self, mat_tag: dict[str, int]):
+    def assign_ops_matTag(self, mat_tag: dict):
         """Assign the mesh size dict for each mesh.
 
         Parameters
         --------------
         mat_tag : dict[str, int]
             A dict of name as key, opensees matTag previous defined as value.
 
@@ -113,15 +113,15 @@
             if name not in self.group_map.keys():
                 raise ValueError(
                     f"{name} is not specified in the assign_group function!"
                 )
         self.mat_ops_map = mat_tag
         return self
 
-    def assign_group_color(self, colors):
+    def assign_group_color(self, colors: dict):
         """Assign the color dict to plot the section.
 
         Parameters
         -------------
         colors : dict[str, str]
             A dict of name as key, color as value.
         """
@@ -1065,15 +1065,15 @@
     """
 
     def __init__(self) -> None:
         self.rebar_data = []
 
     def add_rebar_line(
             self,
-            points: list[list[float, float]],
+            points: list,
             dia: float,
             gap: float = 0.1,
             n: int = None,
             closure: bool = False,
             matTag: int = None,
             color: str = "black",
             group_name: str = None,
@@ -1119,15 +1119,15 @@
         data = dict(
             rebar_xy=rebar_xy, color=color, name=group_name, dia=dia, matTag=matTag
         )
         self.rebar_data.append(data)
 
     def add_rebar_circle(
             self,
-            xo: list[float, float],
+            xo: list,
             radius: float,
             dia: float,
             gap: float = 0.1,
             n: int = None,
             angle1: float = 0.0,
             angle2: float = 360,
             matTag: int = None,
@@ -1238,16 +1238,16 @@
         yield_strength=yield_strength,
         density=density,
         color=color,
     )
 
 
 def add_polygon(
-        outline: list[list[float, float]],
-        holes: list[list[list[float, float]]] = None,
+        outline: list,
+        holes: list = None,
         material=None,
 ):
     """Add polygon plane geom obj.
 
     Parameters
     ----------
     outline : list[list[float, float]]
@@ -1268,15 +1268,15 @@
         material_ = material
     ply = Polygon(outline, holes)
     geometry = Geometry(geom=ply, material=material_)
     return geometry
 
 
 def add_circle(
-        xo: list[float, float],
+        xo: list,
         radius: float,
         holes=None,
         angle1=0.0,
         angle2=360,
         n_sub=40,
         material=None,
 ):
@@ -1334,15 +1334,15 @@
         y_new.extend(np.linspace(y1, y2, n, endpoint=True)[:-1].tolist())
     x_new.append(x[-1])
     y_new.append(y[-1])
     new_line = np.column_stack((x_new, y_new))
     return new_line
 
 
-def offset(points: list[list[float, float]], d: float):
+def offset(points: list, d: float):
     """Offsets closed polygons, same as :py:func:`opstool.preprocessing.poly_offset`
 
     Parameters
     ----------
     points  : list[list[float, float]]
         A list containing the coordinate points, [(x1, y1),(x2, y2),...,(xn.yn)].
     d : float
@@ -1361,15 +1361,15 @@
     >>> outlines4 = opst.offset(outlines3, d=0.1)
     """
     ply = Polygon(points)
     ply_off = ply.buffer(-d, cap_style=3, join_style=2)
     return list(ply_off.exterior.coords)
 
 
-def poly_offset(points: list[list[float, float]], d: float):
+def poly_offset(points: list, d: float):
     """Offsets closed polygons, same as :py:func:`opstool.preprocessing.offset`
 
     Parameters
     ----------
     points  : list[list[float, float]]
         A list containing the coordinate points, [(x1, y1),(x2, y2),...,(xn.yn)].
     d : float
@@ -1378,15 +1378,15 @@
     Returns
     -------
     coords: list[[float, float]]
     """
     return offset(points=points, d=d)
 
 
-def line_offset(points: list[list[float, float]], d: float):
+def line_offset(points: list, d: float):
     """Offset a distance from a non-closed line ring on its right or its left side.
 
     Parameters
     ----------
     points  : list[list[float, float]]
         A list containing the coordinate points, [(x1, y1),(x2, y2),...,(xn.yn)].
     d : float
```

### Comparing `opstool-0.7.2/src/opstool/preprocessing/section/var_sec_mesh.py` & `opstool-0.7.3/src/opstool/preprocessing/section/var_sec_mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import pyvista as pv
 # from sectionproperties.pre.geometry import Geometry
 from shapely import LineString
 
 pv.set_plot_theme("document")
 
 
-def var_line_string(pointsi: list[list[float, float]],
-                    pointsj: list[list[float, float]],
+def var_line_string(pointsi: list,
+                    pointsj: list,
                     path: list, n_sec: float = 2,
                     loc_sec: list | None = None,
                     closure: bool = False,
                     y_degree: int = 1, y_sym_plane: str = "j-0",
                     z_degree: int = 2, z_sym_plane: str = "j-0"):
     """Returns the varied line string.
```

### Comparing `opstool-0.7.2/src/opstool/preprocessing/tcl2py.py` & `opstool-0.7.3/src/opstool/preprocessing/tcl2py.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/preprocessing/unit_system.py` & `opstool-0.7.3/src/opstool/preprocessing/unit_system.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool/utils.py` & `opstool-0.7.3/src/opstool/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,22 @@
               26: (5, 6), 27: (5, 6), 28: (5, 6), 29: (5, 6), 30: (5, 6),
               31: (6, 6), 32: (6, 6), 33: (6, 6), 34: (6, 6), 35: (6, 6),
               36: (6, 6), 37: (6, 7), 38: (6, 7), 39: (6, 7), 40: (6, 7),
               41: (6, 7), 42: (6, 7), 43: (7, 7), 44: (7, 7), 45: (7, 7),
               46: (7, 7), 47: (7, 7), 48: (7, 7), 49: (7, 7)}
 
 
-def check_file(file_name: str, file_type: Union[str, list[str], tuple[str]]):
+def check_file(file_name: str, file_type: Union[str, list, tuple]):
     """Check file type.
 
     Parameters
     ----------
     file_name: str
         The file to be checked.
-    file_type: str
+    file_type: Union[str, list, tuple]
         The target file type.
 
     Returns
     -------
     None
     """
     if file_name:
```

### Comparing `opstool-0.7.2/src/opstool/vis/_get_model_base.py` & `opstool-0.7.3/src/opstool/vis/_get_model_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import triangle as tr
 import openseespy.opensees as ops
+import triangle as tr
 
+from ..preprocessing.section.sec_mesh import SecMesh
 from ..utils import (ELE_TAG_PFEM, ELE_TAG_Beam, ELE_TAG_Brick, ELE_TAG_Link,
                      ELE_TAG_Plane, ELE_TAG_Tetrahedron, ELE_TAG_Truss)
-from ..preprocessing.section.sec_mesh import SecMesh
 
 
 def get_node_coords():
     node_tags = ops.getNodeTags()
     num_node = len(node_tags)
     node_coords = np.zeros((num_node, 3))
     node_index = dict()  # key: nodeTag, value: index in Node_Coords
@@ -473,16 +473,16 @@
     cells["beam"] = beam_cells
     cells["beam_tags"] = beam_cells_tags
     cells["other_line"] = other_line_cells
     cells["other_line_tags"] = other_line_cells_tags
     cells["line_sec_ext"] = ext_cells
     cells["line_sec_int"] = int_cells
     cells["line_sec"] = sec_cells
-    for key, value in cells.items():
-        cells[key] = np.array(value)
+    # for key, value in cells.items():
+    #     cells[key] = np.array(value)
     return model_info, cells
 
 
 def get_node_react(fixed_nodes):
     reacts = []
     for tag in fixed_nodes:
         fixeddofs = ops.getFixedDOFs(tag)
```

### Comparing `opstool-0.7.2/src/opstool/vis/_plotly_base.py` & `opstool-0.7.3/src/opstool/vis/_plotly_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,16 @@
         grp1 = f["ModelInfo"]
         for name in grp1.keys():
             model_info[name] = grp1[name][...]
         grp2 = f["Cell"]
         for name in grp2.keys():
             cells[name] = grp2[name][...]
     for name, value in cells.items():
-        cells[name] = _reshape_cell(value)
+        if "_tags" not in name:
+            cells[name] = _reshape_cell(value)
     fig = _plot_model(obj, model_info, cells,
                       show_node_label=show_node_label,
                       show_ele_label=show_ele_label,
                       show_local_crd=show_local_crd,
                       show_fix_node=show_fix_node,
                       show_constrain_dof=show_constrain_dof,
                       label_size=label_size,
@@ -164,15 +165,15 @@
                 show_node_label: bool = False,
                 show_ele_label: bool = False,
                 show_local_crd: bool = False,
                 show_fix_node: bool = True,
                 show_constrain_dof: bool = False,
                 label_size: float = 8,
                 show_outline: bool = True,
-                opacity: float = 1.0,):
+                opacity: float = 1.0, ):
     fig = go.Figure()
     plotter = []
     points_no_deform = model_info["coord_no_deform"]
     # >>> face plot
     face_cells = [cells["plane"], cells["tetrahedron"], cells["brick"]]
     face_cells_tags = [cells["plane_tags"],
                        cells["tetrahedron_tags"], cells["brick_tags"]]
@@ -189,21 +190,21 @@
             x, y, z = [face_line_points[:, j] for j in range(3)]
             plotter.append(go.Scatter3d(x=x, y=y, z=z,
                                         line=dict(color="black",
                                                   width=obj.line_width / 2),
                                         mode="lines", name=names[ii],
                                         connectgaps=False, hoverinfo="skip"))
             x, y, z = [face_mid_points[:, j] for j in range(3)]
+            labels_ = [f"tag: {kk}" for kk in face_cells_tags[ii]]  # hover label
             plotter.append(
                 go.Scatter3d(x=x, y=y, z=z,
                              marker=dict(size=obj.point_size, color=face_colors[ii],
                                          symbol='circle-open'),
                              mode="markers", name=names[ii],
-                             customdata=face_cells_tags[ii],
-                             hovertemplate='<b>tag: %{customdata}</b>'))
+                             hovertemplate='<b>%{text}</b>', text=labels_, ))
     # >>> line plot
     line_cells = [cells["truss"], cells["link"],
                   cells["beam"], cells["other_line"]]
     line_cells_tags = [cells["truss_tags"], cells["link_tags"],
                        cells["beam_tags"], cells["other_line_tags"]]
     line_colors = [obj.color_truss, obj.color_link,
                    obj.color_line, obj.color_line]
@@ -216,21 +217,22 @@
                 points_no_deform, line_cells[i])
             x, y, z = line_points[:, 0], line_points[:, 1], line_points[:, 2]
             plotter.append(go.Scatter3d(x=x, y=y, z=z,
                                         line=dict(
                                             color=line_colors[i], width=line_widths[i]),
                                         mode="lines", name=names[i],
                                         connectgaps=False, hoverinfo="skip"))
-            x, y, z = [line_mid_points[:, j] for j in range(3)]  # hover label
+            x, y, z = [line_mid_points[:, j] for j in range(3)]
+            labels_ = [f"tag: {kk}" for kk in line_cells_tags[i]]  # hover label
             plotter.append(go.Scatter3d(x=x, y=y, z=z,
                                         marker=dict(size=obj.point_size, color=line_colors[i],
                                                     symbol='circle-open'),
                                         mode="markers", name=names[i],
-                                        customdata=line_cells_tags[i],
-                                        hovertemplate='<b>tag: %{customdata}</b>'))
+                                        hovertemplate='<b>%{text}</b>',
+                                        text=labels_, ))
     # point plot
     node_labels = [str(i) for i in model_info["NodeTags"]]
     x, y, z = [points_no_deform[:, j] for j in range(3)]
     plotter.append(go.Scatter3d(x=x, y=y, z=z,
                                 marker=dict(size=obj.point_size,
                                             color=obj.color_point),
                                 mode="markers", name="Node", customdata=node_labels,
@@ -439,15 +441,15 @@
                                                   size=12),
                                     mode="text", name="constraint dofs")
             plotter.append(txt_plot)
 
 
 def _eigen_vis(
         obj,
-        mode_tags: list[int],
+        mode_tags: list,
         input_file: str = 'EigenData.hdf5',
         subplots: bool = False,
         alpha: float = None,
         show_outline: bool = False,
         show_origin: bool = False,
         opacity: float = 1.0,
         show_face_line: bool = True,
@@ -869,15 +871,15 @@
                                   hovertemplate='%{customdata}')
         fig.add_trace(point_plot)
         if show_values:
             labels = [f"{fi:.3E}" for fi in f]
             txt_plot = go.Scatter3d(x=x, y=y, z=z, text=labels,
                                     textfont=dict(color="#6e750e",
                                                   size=10),
-                                    mode="text", hoverinfo='skip',)
+                                    mode="text", hoverinfo='skip', )
             fig.add_trace(txt_plot)
         # max min point plot
         labels = [
             f"<b>tag: {NodeTags[idx]}</b><br>{direction}: {f[idx]:.3E}" for idx in [idxmax, idxmin]]
         point_plot2 = go.Scatter3d(x=x[[idxmax, idxmin]], y=y[[idxmax, idxmin]], z=z[[idxmax, idxmin]],
                                    marker=dict(size=obj.point_size * 1.25,
                                                color=obj.color_point,
@@ -892,15 +894,15 @@
             line_ends[i] = node_coords[i] - \
                 np.array(axis_dict[direct]) * \
                 max_bound / 30 * np.sign(f[i])
         line_points = []
         line_cells = []
         for point1, point2 in zip(node_coords, line_ends):
             line_points.extend([point2, point1])
-            line_cells.extend([2, len(line_points)-2, len(line_points)-1])
+            line_cells.extend([2, len(line_points) - 2, len(line_points) - 1])
         line_cells = np.reshape(line_cells, (-1, 3))
         line_plot = _generate_line_mesh(points=line_points, cells=line_cells,
                                         line_width=obj.line_width * 2, color=color_dict[direct])
         fig.add_traces(line_plot)
         arrow_plot = _creat_arrows(points=line_points, cells=line_cells,
                                    color=color_dict[direct])
         fig.add_traces(arrow_plot)
@@ -955,15 +957,15 @@
             title=dict(font=dict(family="courier", color='black', size=25),
                        text=f"<b>OpenSeesPy Node Reactions View</b>"
                        ),
             sliders=sliders,
         )
     else:  # a sing step
         idx = np.argmax([np.max(np.abs(react[:, reactidx_dict[direct]]))
-                        for react in node_react_steps])
+                         for react in node_react_steps])
         creat_plot(idx)
         f = node_react_steps[idx][:, reactidx_dict[direct]]
         idxmax, idxmin = np.argmax(f), np.argmin(f)
         txt = (f"<b>OpenSeesPy Node Reactions View</b>"
                f"<br>Step {i + 1} {direction}"
                f"<br>max={f[idxmax]:.3E} | nodeTag={NodeTags[idxmax]}"
                f"<br>min={f[idxmin]:.3E} | nodeTag={NodeTags[idxmin]}")
@@ -1427,15 +1429,15 @@
         pio.write_html(fig, file=save_html, auto_open=True)
     if obj.notebook:
         fig.show()
 
 
 def _frame_resp_vis(obj,
                     input_file: str = "BeamRespStepData-1.hdf5",
-                    ele_tags: list[int] = None,
+                    ele_tags: list = None,
                     slider: bool = False,
                     response: str = "Mz",
                     show_values=True,
                     alpha: float = None,
                     opacity: float = 1,
                     save_html: str = "FrameRespVis"
                     ):
@@ -2099,20 +2101,20 @@
                   anchor_tip=True):
     points = np.array(points)
     cells = np.array(cells)
     x, y, z = points[:, 0], points[:, 1], points[:, 2]
     x_, y_, z_ = [], [], []
     u, v, w = [], [], []
     for p in cells:
-        x_.append(x[p[1]] + arrow_starting_ratio*(x[p[2]] - x[p[1]]))
-        y_.append(y[p[1]] + arrow_starting_ratio*(y[p[2]] - y[p[1]]))
-        z_.append(z[p[1]] + arrow_starting_ratio*(z[p[2]] - z[p[1]]))
-        u.append(arrow_tip_ratio*(x[p[2]] - x[p[1]]))
-        v.append(arrow_tip_ratio*(y[p[2]] - y[p[1]]))
-        w.append(arrow_tip_ratio*(z[p[2]] - z[p[1]]))
+        x_.append(x[p[1]] + arrow_starting_ratio * (x[p[2]] - x[p[1]]))
+        y_.append(y[p[1]] + arrow_starting_ratio * (y[p[2]] - y[p[1]]))
+        z_.append(z[p[1]] + arrow_starting_ratio * (z[p[2]] - z[p[1]]))
+        u.append(arrow_tip_ratio * (x[p[2]] - x[p[1]]))
+        v.append(arrow_tip_ratio * (y[p[2]] - y[p[1]]))
+        w.append(arrow_tip_ratio * (z[p[2]] - z[p[1]]))
     arrow_plot = []
     for i in range(len(cells)):
         if anchor_tip:
             arrow_plot.append(go.Cone(x=[x_[i]], y=[y_[i]], z=[z_[i]],
                                       u=[u[i]], v=[v[i]], w=[w[i]],
                                       sizemode="absolute",
                                       anchor='tip', hoverinfo='skip',
```

### Comparing `opstool-0.7.2/src/opstool/vis/_pyvista_base.py` & `opstool-0.7.3/src/opstool/vis/_pyvista_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+
 import h5py
 import numpy as np
 import pyvista as pv
 
 from ..utils import check_file, shape_dict
 
 
@@ -28,15 +29,15 @@
         grp1 = f["ModelInfo"]
         for name in grp1.keys():
             model_info[name] = grp1[name][...]
         grp2 = f["Cell"]
         for name in grp2.keys():
             cells[name] = grp2[name][...]
 
-    plotter = pv.Plotter(notebook=obj.notebook)
+    plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
     _plot_model(obj, plotter, model_info, cells, opacity)
 
     txt = f"OpenSees 3D View\nNum. of Node:{model_info['num_node']}\nNum. of Ele:{model_info['num_ele']}"
     plotter.add_text(txt, position="upper_right", font_size=10, font="courier")
     if show_outline:
         if np.max(model_info["model_dims"]) <= 2:
             show_zaxis = False
@@ -69,14 +70,15 @@
     _show_mp_constraint(obj, plotter, model_info, show_constrain_dof)
     plotter.add_axes()
     plotter.view_isometric()
     if np.max(model_info["model_dims"]) <= 2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
+    plotter.enable_anti_aliasing('msaa')
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _show_mp_constraint(obj, plotter, model_info, show_dofs):
     points = model_info["ConstrainedCoords"]
     cells = model_info["ConstrainedCells"]
@@ -96,26 +98,36 @@
 def _show_beam_sec(plotter, model_info, cells, paras):
     ext_points = model_info["line_sec_ext_points"]
     int_points = model_info["line_sec_int_points"]
     sec_points = model_info["line_sec_points"]
     ext_cells = cells["line_sec_ext"]
     int_cells = cells["line_sec_int"]
     sec_cells = cells["line_sec"]
+    if paras['texture']:
+        texture = pv.read_texture(paras['texture'])
+    else:
+        texture = None
     if len(ext_cells) > 0:
         ext = _generate_mesh(ext_points, ext_cells, kind='face')
+        if texture is not None:
+            ext.texture_map_to_plane(inplace=True)
         plotter.add_mesh(ext, show_edges=False, color=paras['color'],
-                         opacity=paras['opacity'], texture=paras['texture'])
+                         opacity=paras['opacity'], texture=texture)
     if len(int_cells) > 0:
         intt = _generate_mesh(int_points, int_cells, kind='face')
+        if texture is not None:
+            intt.texture_map_to_plane(inplace=True)
         plotter.add_mesh(intt, show_edges=False, color=paras['color'],
-                         opacity=paras['opacity'], texture=paras['texture'])
+                         opacity=paras['opacity'], texture=texture)
     if len(sec_cells) > 0:
         sec = _generate_mesh(sec_points, sec_cells, kind='face')
+        if texture is not None:
+            sec.texture_map_to_plane(inplace=True)
         plotter.add_mesh(sec, show_edges=False, color=paras['color'],
-                         opacity=paras['opacity'], texture=paras['texture'])
+                         opacity=paras['opacity'], texture=texture)
 
 
 def _show_beam_local_axes(plotter, model_info):
     beam_xlocal = model_info["beam_xlocal"]
     beam_ylocal = model_info["beam_ylocal"]
     beam_zlocal = model_info["beam_zlocal"]
     beam_midpoints = model_info["beam_midpoints"]
@@ -246,15 +258,15 @@
                          render_lines_as_tubes=False, line_width=2)
     else:
         warnings.warn("Model has no fix nodes!")
 
 
 def _eigen_vis(
         obj,
-        mode_tags: list[int],
+        mode_tags: list,
         input_file: str = 'EigenData.hdf5',
         subplots: bool = False,
         link_views: bool = True,
         alpha: float = None,
         show_outline: bool = False,
         show_origin: bool = False,
         opacity: float = 1.0,
@@ -287,21 +299,21 @@
             )
         shape = shape_dict[modej - modei + 1]
         subplot_titles = []
         for i, idx in enumerate(range(modei, modej + 1)):
             txt = "Mode {}: T = {:.3f} s".format(idx, 1 / f[idx - 1])
             subplot_titles.append(txt)
 
-        plotter = pv.Plotter(notebook=obj.notebook, shape=shape)
+        plotter = pv.Plotter(notebook=obj.notebook, shape=shape, line_smoothing=True)
         for i, idx in enumerate(range(modei, modej + 1)):
             eigen_vec = eigenvector[idx - 1]
             if alpha is None:
                 value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
                 alpha_ = (
-                        eigen_data["max_bound"] / obj.bound_fact / value_
+                    eigen_data["max_bound"] / obj.bound_fact / value_
                 )
             else:
                 alpha_ = alpha
             eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
             scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
 
             idxi = int(np.ceil((i + 1) / shape[1]) - 1)
@@ -327,15 +339,15 @@
 
             # plotter.add_scalar_bar(color='#000000', n_labels=10, label_font_size=8)
             # txt = 'Mode {}\nf = {:.3f} Hz\nT = {:.3f} s'.format(i + 1, f[i], 1 / f[i])
             txt = "Mode {} T = {:.3f} s".format(idx, 1 / f[idx - 1])
             plotter.add_text(
                 txt,
                 position="upper_right",
-                font_size=10,
+                font_size=15,
                 # color="black",
                 font="courier",
             )
             if show_outline:
                 plotter.show_bounds(
                     grid=False,
                     location="outer",
@@ -345,23 +357,23 @@
                     font_size=10,
                 )
             plotter.add_axes(color="black")
         if link_views:
             plotter.link_views()
     # !slide style
     else:
-        plotter = pv.Plotter(notebook=obj.notebook)
+        plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
         def create_mesh(value):
             step = int(round(value)) - 1
             eigen_vec = eigenvector[step]
             if alpha is None:
                 value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
                 alpha_ = (
-                        eigen_data["max_bound"] / obj.bound_fact / value_
+                    eigen_data["max_bound"] / obj.bound_fact / value_
                 )
             else:
                 alpha_ = alpha
             eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
             scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
             cmin = np.min(scalars)
             cmax = np.max(scalars)
@@ -384,15 +396,15 @@
             plotter.add_scalar_bar(
                 fmt="%.3e", n_labels=10, label_font_size=12
             )
 
             # txt = 'Mode {}\nf = {:.3f} Hz\nT = {:.3f} s'.format(mode_tag, f_, 1 / f_)
             txt = "Mode {}\nT = {:.3f} s".format(step + 1, 1 / f[step])
             plotter.add_text(
-                txt, position="upper_left", font_size=12, font="courier"
+                txt, position="upper_left", font_size=15, font="courier"
             )
             if show_outline:
                 plotter.show_bounds(
                     grid=False,
                     location="outer",
                     bounds=eigen_data["bound"],
                     show_zaxis=True,
@@ -415,14 +427,15 @@
             tube_width=0.01,
         )
     plotter.view_isometric()
     if np.max(eigen_data["model_dims"]) <= 2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
+    plotter.enable_anti_aliasing('msaa')
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _eigen_anim(
         obj,
         mode_tag: int = 1,
@@ -448,31 +461,31 @@
     if mode_tag > num_mode_tag:
         raise ValueError("Insufficient number of modes in open file")
     eigen_vec = eigenvector[mode_tag - 1]
     f_ = f[mode_tag - 1]
     if alpha is None:
         value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
         alpha_ = (
-                eigen_data["max_bound"] / obj.bound_fact / value_
+            eigen_data["max_bound"] / obj.bound_fact / value_
         )
     else:
         alpha_ = alpha
     eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
     anti_eigen_points = eigen_data["coord_no_deform"] - eigen_vec * alpha_
     scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
     plt_points = [anti_eigen_points,
                   eigen_data["coord_no_deform"], eigen_points]
     # -----------------------------------------------------------------------------
     # start plot
-    plotter = pv.Plotter(notebook=obj.notebook)
+    plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
     if alpha is None:
         value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
         alpha_ = (
-                eigen_data["max_bound"] / obj.bound_fact / value_
+            eigen_data["max_bound"] / obj.bound_fact / value_
         )
     else:
         alpha_ = alpha
     eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
     anti_eigen_points = eigen_data["coord_no_deform"] - eigen_vec * alpha_
     scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
     point_plot, line_plot, face_plot = _generate_all_mesh(plotter,
@@ -494,15 +507,15 @@
         fmt="%.3E", n_labels=10, label_font_size=12
     )
 
     plotter.add_text(
         "Mode {}\nf = {:.3f} Hz\nT = {:.3f} s".format(
             mode_tag, f_, 1 / f_),
         position="upper_right",
-        font_size=12,
+        font_size=15,
         # color="black",
         font="courier",
     )
     if show_outline:
         plotter.show_bounds(
             grid=False,
             location="outer",
@@ -547,14 +560,15 @@
             plotter.update_coordinates(
                 points, mesh=face_plot, render=render)
         plotter.update_scalar_bar_range(
             clim=[np.min(xyz_eigen), np.max(xyz_eigen)], name=None
         )
         plotter.write_frame()
     # ----------------------------------------------------------------------------------
+    plotter.enable_anti_aliasing('msaa')
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _react_vis(obj,
                input_file: str = "NodeReactionStepData-1.hdf5",
                slider: bool = False,
@@ -588,15 +602,15 @@
     color_dict = dict(fx="#d20962", fy="#f47721", fz="#7ac143",
                       mx="#00a78e", my="#00bce4", mz="#7d3f98")
     if D2:
         reactidx_dict = dict(fx=0, fy=1, fz=None, mx=None, my=None, mz=2)
     else:
         reactidx_dict = dict(fx=0, fy=1, fz=2, mx=3, my=4, mz=5)
 
-    plotter = pv.Plotter(notebook=obj.notebook)
+    plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
     def create_mesh(value):
         step = int(round(value)) - 1
         f = node_react_steps[step][:, reactidx_dict[direct]]
         idxmax, idxmin = np.argmax(f), np.argmin(f)
         plotter.clear_actors()  # !!!!!!
         # point plot
@@ -682,14 +696,15 @@
                          for react in node_react_steps])
         create_mesh(idx + 1)
     plotter.view_isometric()
     if D2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
+    plotter.enable_anti_aliasing('msaa')
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _deform_vis(
         obj,
         input_file: str = "NodeRespStepData-1.hdf5",
@@ -768,15 +783,15 @@
         else:
             alpha_ = alpha
     else:
         alpha_ = 0
     # ------------------------------------------------------------------------
     # Start plot
     # -------------------------------------------------------------------------
-    plotter = pv.Plotter(notebook=obj.notebook)
+    plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
     def create_mesh(value):
         step = int(round(value)) - 1
         if model_update:
             node_nodeform_coords = model_info_steps["coord_no_deform"][step]
             bounds = model_info_steps["bound"][step]
             lines_cells = cell_steps["all_lines"][step]
@@ -868,14 +883,15 @@
     else:  # plot a single step
         create_mesh(max_step + 1)
     plotter.view_isometric()
     if np.max(model_dims) <= 2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
+    plotter.enable_anti_aliasing('msaa')
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _deform_anim(
         obj,
         input_file: str = "NodeRespStepData-1.hdf5",
@@ -947,15 +963,15 @@
             alpha_ = max_bound / obj.bound_fact / value
         else:
             alpha_ = alpha
     else:
         alpha_ = 0
     # -----------------------------------------------------------------------------
     # start plot
-    plotter = pv.Plotter(notebook=obj.notebook)
+    plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
     def creat_mesh(step):
         if model_update:
             node_nodeform_coords = model_info_steps["coord_no_deform"][step]
             bounds = model_info_steps["bound"][step]
             lines_cells = cell_steps["all_lines"][step]
             faces_cells = cell_steps["all_faces"][step]
@@ -1029,21 +1045,22 @@
         plotter.open_movie(save_fig, framerate=framerate)
     # plotter.write_frame()  # write initial data
     for step in range(num_steps):
         _ = creat_mesh(step)
         plotter.write_frame()
 
     # ----------------------------------------------------------------------------------
+    plotter.enable_anti_aliasing('msaa')
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _frame_resp_vis(obj,
                     input_file: str = "BeamRespStepData-1.hdf5",
-                    ele_tags: list[int] = None,
+                    ele_tags: list = None,
                     slider: bool = False,
                     response: str = "Mz",
                     show_values=True,
                     alpha: float = None,
                     opacity: float = 1,
                     save_fig: str = "FrameRespVis.svg"
                     ):
@@ -1124,15 +1141,15 @@
         alpha_ = max_bound / maxv / obj.bound_fact
     else:
         alpha_ = alpha
 
     # ------------------------------------------------------------------------
     # start plot
     # -------------------------------------------------------------------------
-    plotter = pv.Plotter(notebook=obj.notebook)
+    plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
     def create_mesh(value):
         step = int(round(value)) - 1
         local_forces = local_forces_step[step]
         local_forces_scale = local_forces * alpha_
         # add force face cells
         # TODO if values symbol versa, need trangle
@@ -1253,14 +1270,15 @@
     else:  # plot a single step
         create_mesh(maxstep + 1)
     plotter.view_isometric()
     if np.max(np.abs(beam_node_coords[:, -1])) < 1e-5:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
+    plotter.enable_anti_aliasing('msaa')
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _generate_mesh(points, cells, kind="line"):
     """
     generate the mesh from the points and cells
```

### Comparing `opstool-0.7.2/src/opstool/vis/fiber_sec_vis.py` & `opstool-0.7.3/src/opstool/vis/fiber_sec_vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 
 import h5py
 import numpy as np
 import matplotlib
 import matplotlib.animation as animation
 import matplotlib.pyplot as plt
-from typing import Union
 from ..utils import shape_dict
 
 
 class FiberSecVis:
     """
     A class to vis the fiber section responses in OpenSeesPy.
 
@@ -95,15 +94,15 @@
                         self.lw, self.cmap, self.opacity, mat_color)
         plt.show()
 
     def _get_fiber_data(self,
                         key: str,
                         step: int = None,
                         show_variable: str = "strain",
-                        show_mats: Union[int, list[int], tuple[int]] = None,
+                        show_mats=None,
                         ):
 
         if key not in self.key_names:
             raise ValueError("ele_tag and sec_tag not in set_fiber_secs()!")
         fiber_step_data = self.fiber_sec_step_data[key]
         fiber_step_data = np.array(fiber_step_data)
 
@@ -160,15 +159,15 @@
         areas = fiber_data[:, 2]
         return fiber_data, step_, matidx, vmin, vmax, ylocs, zlocs, areas
 
     def resp_vis(self,
                  ele_tag: int, sec_tag: int,
                  step: int = None,
                  show_variable: str = "strain",
-                 show_mats: Union[int, list[int], tuple[int]] = None,
+                 show_mats=None,
                  ):
         """fiber section response vis.
 
         Parameters
         -----------
         ele_tag: int
             The element tag to which the section is to be displayed.
@@ -252,15 +251,15 @@
         plt.tight_layout()
         plt.show()
 
     def animation(self,
                   output_file: str,
                   ele_tag: int, sec_tag: int,
                   show_variable: str = "strain",
-                  show_mats: Union[int, list[int], tuple[int]] = None,
+                  show_mats=None,
                   framerate: int = 24,
                   ):
         """fiber section response animation.
 
         Parameters
         ----------
         output_file: str
```

### Comparing `opstool-0.7.2/src/opstool/vis/get_model_data.py` & `opstool-0.7.3/src/opstool/vis/get_model_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 
     def get_node_react_step(self,
                             dynamic: bool = False,
                             rayleigh: bool = False,
                             num_steps: int = 10000000000000,
                             total_time: float = 10000000000000,
                             stop_cond: bool = False,
-                            save_file: str | bool = "NodeReactionStepData-1.hdf5", ):
+                            save_file: Union[str, bool] = "NodeReactionStepData-1.hdf5", ):
         """Get one step the node reactions data.
 
         Parameters
         ----------
         dynamic : bool, optional, by default False
             If True, include dynamic effects.
         rayleigh : bool, optional, by default False
@@ -330,15 +330,15 @@
                 grp.create_dataset(
                     f"step{i + 1}", data=self.node_react_steps[i])
 
     def get_node_resp_step(self,
                            num_steps: int = 10000000000000,
                            total_time: float = 10000000000000,
                            stop_cond: bool = False,
-                           save_file: str | bool = "NodeRespStepData-1.hdf5",
+                           save_file: Union[str, bool] = "NodeRespStepData-1.hdf5",
                            model_update: bool = False):
         """Get the node response data one step.
 
         .. note::
             You need to call this function at each analysis step in OpenSees.
             The advantage is that you can modify the iterative algorithm at
             each analysis step to facilitate convergence.
@@ -448,15 +448,15 @@
                 for i in range(n):
                     subgrp.create_dataset(f"step{i + 1}", data=value[i])
 
     def get_frame_resp_step(self,
                             num_steps: int = 10000000000000,
                             total_time: float = 10000000000000,
                             stop_cond: bool = False,
-                            save_file: str | bool = "BeamRespStepData-1.hdf5"
+                            save_file: Union[str, bool] = "BeamRespStepData-1.hdf5"
                             ):
         """Get the response data one step.
 
         .. note::
             You need to call this function at each analysis step in OpenSees.
             The advantage is that you can modify the iterative algorithm at
             each analysis step to facilitate convergence.
@@ -523,15 +523,15 @@
             for name, value in self.beam_infos.items():
                 grp1.create_dataset(name, data=value)
             for name, value in self.beam_resp_step.items():
                 subgrp = grp2.create_group(name)
                 for i in range(n):
                     subgrp.create_dataset(f"step{i + 1}", data=value[i])
 
-    def get_fiber_data(self, ele_sec: list[tuple[int, int]], save_file: str | bool = 'FiberData.hdf5'):
+    def get_fiber_data(self, ele_sec: list, save_file: Union[str, bool] = 'FiberData.hdf5'):
         """Get data from the section assigned by parameter ele_sec.
 
         Parameters
         ----------
         ele_sec: list[tuple[int, int]]
             A list or tuple composed of element tag and sectag.
             e.g., [(ele1, sec1), (ele2, sec2), ... , (elen, secn)],
@@ -571,15 +571,15 @@
             print(
                 f"Fiber section data saved in [bold {next(self.colors_cycle)}]{output_filename}[/] !")
 
     def get_fiber_resp_step(self,
                             num_steps: int = 10000000000000,
                             total_time: float = 10000000000000,
                             stop_cond: bool = False,
-                            save_file: str | bool = "FiberRespStepData-1.hdf5"):
+                            save_file: Union[str, bool] = "FiberRespStepData-1.hdf5"):
         """Get analysis results data for fiber section one step.
 
         Parameters
         ----------
         num_steps: int, default=10000000000000
             Total number of steps, set to determine when to save data.
         total_time: float, default=10000000000000
@@ -709,15 +709,15 @@
             self._save_fiber_resp_step(filename, "a")
         if reset_state:
             self.reset_steps_state()
         print(
             f"All responses data saved in [bold {next(self.colors_cycle)}]{filename}[/] !")
 
 
-def _get_fiber_sec_data(ele_tag: int, sec_tag: int = 1) -> ArrayLike:
+def _get_fiber_sec_data(ele_tag: int, sec_tag: int = 1):
     """Get the fiber sec data for a beam element.
 
     Parameters
     ----------
     ele_tag: int
         The element tag to which the section is to be displayed.
     sec_tag: int
```

### Comparing `opstool-0.7.2/src/opstool/vis/ops_vis_plotly.py` & `opstool-0.7.3/src/opstool/vis/ops_vis_plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                    show_outline=show_outline,
                    opacity=opacity,
                    save_html=save_html
                    )
 
     def eigen_vis(
         self,
-        mode_tags: list[int],
+        mode_tags: list,
         input_file: str = 'EigenData.hdf5',
         subplots: bool = False,
         alpha: float = None,
         show_outline: bool = False,
         show_origin: bool = False,
         opacity: float = 1.0,
         show_face_line: bool = True,
@@ -426,15 +426,15 @@
                      show_face_line=show_face_line,
                      save_html=save_html,
                      model_update=model_update
                      )
 
     def frame_resp_vis(self,
                        input_file: str = "BeamRespStepData-1.hdf5",
-                       ele_tags: list[int] = None,
+                       ele_tags: list = None,
                        slider: bool = False,
                        response: str = "Mz",
                        show_values=True,
                        alpha: float = None,
                        opacity: float = 1,
                        save_html: str = "FrameRespVis"
                        ):
```

### Comparing `opstool-0.7.2/src/opstool/vis/ops_vis_pyvista.py` & `opstool-0.7.3/src/opstool/vis/ops_vis_pyvista.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         # ------------------------------
         self.point_size = point_size
         self.line_width = line_width
         self.title = "opstool"
         # Initialize the color dict
         colors = dict(
             point="#580f41",
-            line="#037ef3",
+            line="#0504aa",
             face="#00c16e",
             solid="#0cb9c1",
             truss="#7552cc",
             link="#01ff07",
             constraint="#00ffff",
         )
         if colors_dict is not None:
@@ -120,16 +120,18 @@
             Whether to display the fix nodes.
         show_constrain_dof: bool, default=False
             Whether to display labels for constrained degrees of freedom.
         show_beam_sec: bool default = False
             Whether to render the 3d section of beam or truss elements.
             If True, the Arg `beam_sec` in :py:meth:`opstool.vis.GetFEMdata.get_model_data`
             must be assigned in advance.
-        beam_sec_paras: dict = None,
+        beam_sec_paras: dict defalut = None,
             A dict to control beam section render, optional key: color, opacity, texture.
+            For texture, you can pass an image file with color=None,
+            if texture is None, it will be ignored.
         label_size: float, default=8
             The foontsize of node and ele label.
         show_outline: bool, default=True
             Whether to show the axis frame.
         opacity: float, default=1.0
             Plane and solid element transparency.
         save_fig: str, default='ModelVis.svg'
@@ -160,15 +162,15 @@
                    show_outline=show_outline,
                    opacity=opacity,
                    save_fig=save_fig
                    )
 
     def eigen_vis(
         self,
-        mode_tags: list[int],
+        mode_tags: list,
         input_file: str = 'EigenData.hdf5',
         subplots: bool = False,
         link_views: bool = True,
         alpha: float = None,
         show_outline: bool = False,
         show_origin: bool = False,
         opacity: float = 1.0,
@@ -468,15 +470,15 @@
             show_face_line=show_face_line,
             save_fig=save_fig,
             model_update=model_update
         )
 
     def frame_resp_vis(self,
                        input_file: str = "BeamRespStepData-1.hdf5",
-                       ele_tags: list[int] = None,
+                       ele_tags: list = None,
                        slider: bool = False,
                        response: str = "Mz",
                        show_values=True,
                        alpha: float = None,
                        opacity: float = 1,
                        save_fig: str = "FrameRespVis.svg"
                        ):
```

### Comparing `opstool-0.7.2/src/opstool/vis/save_tikz.py` & `opstool-0.7.3/src/opstool/vis/save_tikz.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.2/src/opstool.egg-info/PKG-INFO` & `opstool-0.7.3/src/opstool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.7.2
+Version: 0.7.3
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
 Keywords: OpenSees seismic visualization
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.7.2 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.7.3 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
 yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees seismic
 visualization Platform: any Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8.* Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
```

### Comparing `opstool-0.7.2/src/opstool.egg-info/SOURCES.txt` & `opstool-0.7.3/src/opstool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 src/opstool/vis/_get_model_base.py
 src/opstool/vis/_plotly_base.py
 src/opstool/vis/_pyvista_base.py
 src/opstool/vis/fiber_sec_vis.py
 src/opstool/vis/get_model_data.py
 src/opstool/vis/ops_vis_plotly.py
 src/opstool/vis/ops_vis_pyvista.py
+src/opstool/vis/quick_plot.py
 src/opstool/vis/save_tikz.py
```

