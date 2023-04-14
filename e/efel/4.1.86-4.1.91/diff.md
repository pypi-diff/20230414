# Comparing `tmp/efel-4.1.86.tar.gz` & `tmp/efel-4.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-4.1.86.tar", last modified: Wed Apr 12 09:25:59 2023, max compression
+gzip compressed data, was "efel-4.1.91.tar", last modified: Thu Apr 13 10:40:04 2023, max compression
```

## Comparing `efel-4.1.86.tar` & `efel-4.1.91.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:25:59.559762 efel-4.1.86/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-12 09:25:58.000000 efel-4.1.86/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-04-12 09:25:58.000000 efel-4.1.86/COPYING
--rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-04-12 09:25:58.000000 efel-4.1.86/COPYING.less
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-04-12 09:25:58.000000 efel-4.1.86/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-04-12 09:25:58.000000 efel-4.1.86/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-12 09:25:59.559762 efel-4.1.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-04-12 09:25:58.000000 efel-4.1.86/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:25:59.563763 efel-4.1.86/efel/
--rw-r--r--   0 runner    (1001) docker     (122)    12702 2023-04-12 09:25:58.000000 efel-4.1.86/efel/DependencyV5.txt
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-12 09:25:58.000000 efel-4.1.86/efel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-12 09:25:59.563763 efel-4.1.86/efel/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    18332 2023-04-12 09:25:58.000000 efel-4.1.86/efel/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:25:59.559762 efel-4.1.86/efel/cppcore/
--rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/DependencyTree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/DependencyTree.h
--rw-r--r--   0 runner    (1001) docker     (122)    14348 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/FillFptrTable.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/FillFptrTable.h
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/Global.h
--rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/LibV1.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/LibV1.h
--rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/LibV2.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/LibV2.h
--rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/LibV3.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/LibV3.h
--rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/LibV4.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/LibV4.h
--rw-r--r--   0 runner    (1001) docker     (122)   134268 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/LibV5.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15700 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/LibV5.h
--rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/Utils.h
--rw-r--r--   0 runner    (1001) docker     (122)    22200 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/cfeature.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/cfeature.h
--rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/cppcore.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/eFELLogger.h
--rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/efel.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/efel.h
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/mapoperations.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/mapoperations.h
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-12 09:25:58.000000 efel-4.1.86/efel/cppcore/types.h
--rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-04-12 09:25:58.000000 efel-4.1.86/efel/io.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:25:59.559762 efel-4.1.86/efel/pyfeatures/
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-12 09:25:58.000000 efel-4.1.86/efel/pyfeatures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10308 2023-04-12 09:25:58.000000 efel-4.1.86/efel/pyfeatures/pyfeatures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-12 09:25:58.000000 efel-4.1.86/efel/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 09:25:59.555762 efel-4.1.86/efel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-12 09:25:59.000000 efel-4.1.86/efel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-04-12 09:25:59.000000 efel-4.1.86/efel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 09:25:59.000000 efel-4.1.86/efel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-12 09:25:59.000000 efel-4.1.86/efel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-12 09:25:59.000000 efel-4.1.86/efel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-12 09:25:59.559762 efel-4.1.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-04-12 09:25:58.000000 efel-4.1.86/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-04-12 09:25:58.000000 efel-4.1.86/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 10:40:04.422554 efel-4.1.91/
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-13 10:40:01.000000 efel-4.1.91/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    35151 2023-04-13 10:40:01.000000 efel-4.1.91/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-04-13 10:40:01.000000 efel-4.1.91/COPYING.less
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-04-13 10:40:01.000000 efel-4.1.91/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-04-13 10:40:01.000000 efel-4.1.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-13 10:40:04.422554 efel-4.1.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7400 2023-04-13 10:40:01.000000 efel-4.1.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 10:40:04.422554 efel-4.1.91/efel/
+-rw-r--r--   0 runner    (1001) docker     (122)    12805 2023-04-13 10:40:01.000000 efel-4.1.91/efel/DependencyV5.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-13 10:40:01.000000 efel-4.1.91/efel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-13 10:40:04.422554 efel-4.1.91/efel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18462 2023-04-13 10:40:01.000000 efel-4.1.91/efel/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 10:40:04.422554 efel-4.1.91/efel/cppcore/
+-rw-r--r--   0 runner    (1001) docker     (122)     6902 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/DependencyTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/DependencyTree.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/FillFptrTable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/FillFptrTable.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/Global.h
+-rw-r--r--   0 runner    (1001) docker     (122)    69609 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV1.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV1.h
+-rw-r--r--   0 runner    (1001) docker     (122)    57446 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV2.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8364 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV2.h
+-rw-r--r--   0 runner    (1001) docker     (122)    40008 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV3.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4874 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV3.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3611 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV4.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV4.h
+-rw-r--r--   0 runner    (1001) docker     (122)   136351 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV5.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15913 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/LibV5.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3430 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/Utils.h
+-rw-r--r--   0 runner    (1001) docker     (122)    22270 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/cfeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/cfeature.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/cppcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/eFELLogger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3597 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/efel.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/efel.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/mapoperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/mapoperations.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-13 10:40:01.000000 efel-4.1.91/efel/cppcore/types.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10312 2023-04-13 10:40:01.000000 efel-4.1.91/efel/io.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 10:40:04.422554 efel-4.1.91/efel/pyfeatures/
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-13 10:40:01.000000 efel-4.1.91/efel/pyfeatures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10308 2023-04-13 10:40:01.000000 efel-4.1.91/efel/pyfeatures/pyfeatures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-04-13 10:40:01.000000 efel-4.1.91/efel/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 10:40:04.418554 efel-4.1.91/efel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-13 10:40:04.000000 efel-4.1.91/efel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-04-13 10:40:04.000000 efel-4.1.91/efel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 10:40:04.000000 efel-4.1.91/efel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-13 10:40:04.000000 efel-4.1.91/efel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-13 10:40:04.000000 efel-4.1.91/efel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-13 10:40:04.422554 efel-4.1.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-04-13 10:40:01.000000 efel-4.1.91/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69513 2023-04-13 10:40:01.000000 efel-4.1.91/versioneer.py
```

### Comparing `efel-4.1.86/COPYING` & `efel-4.1.91/COPYING`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/COPYING.less` & `efel-4.1.91/COPYING.less`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/LICENSE.txt` & `efel-4.1.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/PKG-INFO` & `efel-4.1.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.1.86
+Version: 4.1.91
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.1.86/README.md` & `efel-4.1.91/README.md`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/DependencyV5.txt` & `efel-4.1.91/efel/DependencyV5.txt`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 LibV5:current #LibV1:interpolate 
 LibV5:time #LibV1:interpolate 
 LibV5:steady_state_voltage_stimend #LibV1:interpolate 
 LibV5:voltage_base #LibV1:interpolate
 LibV5:current_base 
 LibV5:decay_time_constant_after_stim #LibV1:interpolate 
 LibV5:sag_time_constant #LibV1:minimum_voltage #LibV5:steady_state_voltage_stimend #LibV5:sag_amplitude #LibV1:interpolate
+LibV5:multiple_decay_time_constant_after_stim #LibV5:decay_time_constant_after_stim #LibV1:interpolate
 LibV5:maximum_voltage_from_voltagebase #LibV5:voltage_base #LibV1:maximum_voltage #LibV1:interpolate 
 LibV5:sag_amplitude #LibV1:minimum_voltage #LibV5:steady_state_voltage_stimend #LibV5:voltage_deflection_vb_ssse #LibV1:interpolate 
 LibV5:sag_ratio1 #LibV1:minimum_voltage #LibV5:sag_amplitude #LibV5:voltage_base #LibV1:interpolate 
 LibV5:sag_ratio2 #LibV1:minimum_voltage #LibV5:steady_state_voltage_stimend #LibV5:voltage_base #LibV1:interpolate 
 LibV5:AP_peak_upstroke     #LibV5:AP_begin_indices #LibV5:peak_indices #LibV1:interpolate
 LibV5:AP_peak_downstroke   #LibV5:min_AHP_indices #LibV5:peak_indices #LibV1:interpolate
 LibV5:min_between_peaks_indices 	    #LibV5:peak_indices #LibV1:interpolate
```

### Comparing `efel-4.1.86/efel/__init__.py` & `efel-4.1.91/efel/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/api.py` & `efel-4.1.91/efel/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,18 @@
 
     # First set some settings that are used by the feature extraction
 
     for setting_name, int_setting in list(_int_settings.items()):
         cppcore.setFeatureInt(setting_name, [int_setting])
 
     for setting_name, double_setting in list(_double_settings.items()):
-        cppcore.setFeatureDouble(setting_name, [double_setting])
+        if isinstance(double_setting, list):
+            cppcore.setFeatureDouble(setting_name, double_setting)
+        else:
+            cppcore.setFeatureDouble(setting_name, [double_setting])
 
     for setting_name, str_setting in list(_string_settings.items()):
         cppcore.setFeatureString(setting_name, str_setting)
 
 
 def setIntSetting(setting_name, new_value):
     """Set a certain integer setting to a new value"""
```

### Comparing `efel-4.1.86/efel/cppcore/DependencyTree.cpp` & `efel-4.1.91/efel/cppcore/DependencyTree.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/DependencyTree.h` & `efel-4.1.91/efel/cppcore/DependencyTree.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/FillFptrTable.cpp` & `efel-4.1.91/efel/cppcore/FillFptrTable.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,16 @@
   FptrTableV5["time"] = &LibV5::time;
   FptrTableV5["steady_state_voltage_stimend"] =
       &LibV5::steady_state_voltage_stimend;
   FptrTableV5["voltage_base"] = &LibV5::voltage_base;
   FptrTableV5["current_base"] = &LibV5::current_base;
   FptrTableV5["decay_time_constant_after_stim"] =
       &LibV5::decay_time_constant_after_stim;
+  FptrTableV5["multiple_decay_time_constant_after_stim"] =
+      &LibV5::multiple_decay_time_constant_after_stim;
   FptrTableV5["sag_time_constant"] =
       &LibV5::sag_time_constant;
 
   FptrTableV5["ohmic_input_resistance_vb_ssse"] =
       &LibV5::ohmic_input_resistance_vb_ssse;
   FptrTableV5["voltage_deflection_vb_ssse"] =
       &LibV5::voltage_deflection_vb_ssse;
```

### Comparing `efel-4.1.86/efel/cppcore/FillFptrTable.h` & `efel-4.1.91/efel/cppcore/FillFptrTable.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/Global.h` & `efel-4.1.91/efel/cppcore/Global.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/LibV1.cpp` & `efel-4.1.91/efel/cppcore/LibV1.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/LibV1.h` & `efel-4.1.91/efel/cppcore/LibV1.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/LibV2.cpp` & `efel-4.1.91/efel/cppcore/LibV2.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/LibV2.h` & `efel-4.1.91/efel/cppcore/LibV2.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/LibV3.cpp` & `efel-4.1.91/efel/cppcore/LibV3.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/LibV3.h` & `efel-4.1.91/efel/cppcore/LibV3.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/LibV4.cpp` & `efel-4.1.91/efel/cppcore/LibV4.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/LibV4.h` & `efel-4.1.91/efel/cppcore/LibV4.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/LibV5.cpp` & `efel-4.1.91/efel/cppcore/LibV5.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -2572,14 +2572,79 @@
   dtcas.push_back(val);
   setVec(DoubleFeatureData, StringData, "decay_time_constant_after_stim",
                dtcas);
 
   return 1;
 }
 
+// Calculate the time constants after each step for a stimuli containing several
+// steps, as for example SpikeRec protocols
+int LibV5::multiple_decay_time_constant_after_stim(mapStr2intVec& IntFeatureData,
+                                             mapStr2doubleVec& DoubleFeatureData,
+                                             mapStr2Str& StringData) {
+  int retVal;
+  int nSize;
+
+  retVal = CheckInMap(DoubleFeatureData, StringData,
+                            "multiple_decay_time_constant_after_stim", nSize);
+  if (retVal) {
+    return nSize;
+  }
+
+  vector<double> voltages;
+  retVal = getVec(DoubleFeatureData, StringData, "V", voltages);
+  if (retVal < 0) return -1;
+
+  vector<double> times;
+  retVal = getVec(DoubleFeatureData, StringData, "T", times);
+  if (retVal < 0) return -1;
+
+  vector<double> vect;
+  retVal = getVec(DoubleFeatureData, StringData, "multi_stim_end", vect);
+  if (retVal < 0) return -1;
+  vector<double> stimsEnd = vect;
+
+  retVal = getVec(DoubleFeatureData, StringData, "multi_stim_start", vect);
+  if (retVal < 0) return -1;
+  vector<double> stimsStart = vect;
+
+  double decay_start_after_stim, decay_end_after_stim;
+  retVal = getVec(DoubleFeatureData, StringData, "decay_start_after_stim",
+                        vect);
+  if (retVal == 1) {
+    decay_start_after_stim = vect[0];
+  } else {
+    decay_start_after_stim = 1.0;
+  }
+
+  retVal =
+      getVec(DoubleFeatureData, StringData, "decay_end_after_stim", vect);
+  if (retVal == 1) {
+    decay_end_after_stim = vect[0];
+  } else {
+    decay_end_after_stim = 10.0;
+  }
+
+  // Call the decay_time_constant_after_stim for each set of stim_start
+  // and stim_end
+  double ret_dtcas;
+  vector<double> dtcas;
+  for (size_t i = 0; i < stimsStart.size(); i++) {
+      ret_dtcas = __decay_time_constant_after_stim(times, voltages,
+                 decay_start_after_stim, decay_end_after_stim, stimsStart[i],
+                 stimsEnd[i]);
+      dtcas.push_back(ret_dtcas);
+  }
+
+  setVec(DoubleFeatureData, StringData, "multiple_decay_time_constant_after_stim",
+             dtcas);
+
+  return 1;
+}
+
 // compute time constant for the decay from the sag to the steady_state_voltage
 // noisy data is expected, so no golden section search is used
 // because with noisy data, x>0 often gives a worse logarithmic fit
 static int __sag_time_constant(const vector<double>& times,
                             const vector<double>& voltage,
                             const double minimum_voltage,
                             const double steady_state_v,
```

### Comparing `efel-4.1.86/efel/cppcore/LibV5.h` & `efel-4.1.91/efel/cppcore/LibV5.h`

 * *Files 0% similar despite different names*

```diff
@@ -214,14 +214,17 @@
                  mapStr2Str& StringData);
 int current_base(mapStr2intVec& IntFeatureData,           
                  mapStr2doubleVec& DoubleFeatureData,             
                  mapStr2Str& StringData);
 int decay_time_constant_after_stim(mapStr2intVec& IntFeatureData,
                                    mapStr2doubleVec& DoubleFeatureData,
                                    mapStr2Str& StringData);
+int multiple_decay_time_constant_after_stim(mapStr2intVec& IntFeatureData,
+                                      mapStr2doubleVec& DoubleFeatureData,
+                                      mapStr2Str& StringData);
 int sag_time_constant(mapStr2intVec& IntFeatureData,
                             mapStr2doubleVec& DoubleFeatureData,
                             mapStr2Str& StringData);
 int voltage_deflection_vb_ssse(mapStr2intVec& IntFeatureData,
                                    mapStr2doubleVec& DoubleFeatureData,
                                    mapStr2Str& StringData);
 int ohmic_input_resistance_vb_ssse(mapStr2intVec& IntFeatureData,
```

### Comparing `efel-4.1.86/efel/cppcore/Utils.cpp` & `efel-4.1.91/efel/cppcore/Utils.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/Utils.h` & `efel-4.1.91/efel/cppcore/Utils.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/cfeature.cpp` & `efel-4.1.91/efel/cppcore/cfeature.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,15 @@
   featuretypes["voltage"] = "double";
   featuretypes["current"] = "double";
   featuretypes["time"] = "double";
   featuretypes["steady_state_voltage_stimend"] = "double";
   featuretypes["voltage_base"] = "double";
   featuretypes["current_base"] = "double";
   featuretypes["decay_time_constant_after_stim"] = "double";
+  featuretypes["multiple_decay_time_constant_after_stim"] = "double";
   featuretypes["sag_time_constant"] = "double";
   featuretypes["maximum_voltage_from_voltagebase"] = "double";
   featuretypes["sag_amplitude"] = "double";
   featuretypes["sag_ratio1"] = "double";
   featuretypes["sag_ratio2"] = "double";
   featuretypes["AP_peak_upstroke"] = "double";
   featuretypes["AP_peak_downstroke"] = "double";
```

### Comparing `efel-4.1.86/efel/cppcore/cfeature.h` & `efel-4.1.91/efel/cppcore/cfeature.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/cppcore.cpp` & `efel-4.1.91/efel/cppcore/cppcore.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/eFELLogger.h` & `efel-4.1.91/efel/cppcore/eFELLogger.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/efel.cpp` & `efel-4.1.91/efel/cppcore/efel.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/efel.h` & `efel-4.1.91/efel/cppcore/efel.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/mapoperations.cpp` & `efel-4.1.91/efel/cppcore/mapoperations.cpp`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/mapoperations.h` & `efel-4.1.91/efel/cppcore/mapoperations.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/cppcore/types.h` & `efel-4.1.91/efel/cppcore/types.h`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/io.py` & `efel-4.1.91/efel/io.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/pyfeatures/__init__.py` & `efel-4.1.91/efel/pyfeatures/__init__.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/pyfeatures/pyfeatures.py` & `efel-4.1.91/efel/pyfeatures/pyfeatures.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel/settings.py` & `efel-4.1.91/efel/settings.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/efel.egg-info/PKG-INFO` & `efel-4.1.91/efel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efel
-Version: 4.1.86
+Version: 4.1.91
 Summary: Electrophys Feature Extract Library (eFEL)
 Home-page: https://github.com/BlueBrain/eFEL
 Author: BlueBrain Project, EPFL
 Maintainer: Werner Van Geit
 Maintainer-email: werner.vangeit@epfl.ch
 License: LGPLv3
 Keywords: feature,extraction,electrophysiology,BlueBrainProject
```

### Comparing `efel-4.1.86/efel.egg-info/SOURCES.txt` & `efel-4.1.91/efel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/setup.py` & `efel-4.1.91/setup.py`

 * *Files identical despite different names*

### Comparing `efel-4.1.86/versioneer.py` & `efel-4.1.91/versioneer.py`

 * *Files identical despite different names*

