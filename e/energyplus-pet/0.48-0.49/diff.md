# Comparing `tmp/energyplus_pet-0.48.tar.gz` & `tmp/energyplus_pet-0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_pet-0.48.tar", last modified: Thu Apr  6 19:49:45 2023, max compression
+gzip compressed data, was "energyplus_pet-0.49.tar", last modified: Fri Apr 14 16:20:53 2023, max compression
```

## Comparing `energyplus_pet-0.48.tar` & `energyplus_pet-0.49.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:49:45.848356 energyplus_pet-0.48/
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-04-06 19:49:45.848356 energyplus_pet-0.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-06 19:49:20.000000 energyplus_pet-0.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:49:45.844356 energyplus_pet-0.48/energyplus_pet/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/configure.py
--rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/correction_factor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/data_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:49:45.848356 energyplus_pet-0.48/energyplus_pet/equipment/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/equipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13066 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/equipment/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/equipment/column_header.py
--rw-r--r--   0 runner    (1001) docker     (122)     2291 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/equipment/common_curves.py
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/equipment/equip_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/equipment/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    20165 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/equipment/wahp_cooling_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    15424 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/equipment/wahp_heating_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/equipment/wwhp_cooling_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/equipment/wwhp_heating_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:49:45.848356 energyplus_pet-0.48/energyplus_pet/forms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16776 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/base_data_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/basic_message_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     4170 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/catalog_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/comparison_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/constant_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)    22194 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/correction_detail_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     9698 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/correction_summary_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     6408 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/correction_summary_widget.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/header_preview.py
--rw-r--r--   0 runner    (1001) docker     (122)    31620 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/forms/main.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)    12745 2023-04-06 19:49:20.000000 energyplus_pet-0.48/energyplus_pet/units.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 19:49:45.844356 energyplus_pet-0.48/energyplus_pet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-04-06 19:49:45.000000 energyplus_pet-0.48/energyplus_pet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-04-06 19:49:45.000000 energyplus_pet-0.48/energyplus_pet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 19:49:45.000000 energyplus_pet-0.48/energyplus_pet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-06 19:49:45.000000 energyplus_pet-0.48/energyplus_pet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-06 19:49:45.000000 energyplus_pet-0.48/energyplus_pet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-06 19:49:45.000000 energyplus_pet-0.48/energyplus_pet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-06 19:49:45.848356 energyplus_pet-0.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-04-06 19:49:20.000000 energyplus_pet-0.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:53.488829 energyplus_pet-0.49/
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-14 16:20:25.000000 energyplus_pet-0.49/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-04-14 16:20:53.488829 energyplus_pet-0.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-14 16:20:25.000000 energyplus_pet-0.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:53.484829 energyplus_pet-0.49/energyplus_pet/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/configure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/correction_factor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:53.484829 energyplus_pet-0.49/energyplus_pet/equipment/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13066 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/column_header.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2291 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/common_curves.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/equip_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20165 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/wahp_cooling_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15424 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/wahp_heating_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/wwhp_cooling_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/equipment/wwhp_heating_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:53.488829 energyplus_pet-0.49/energyplus_pet/forms/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16776 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/base_data_form.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/basic_message_form.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4170 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/catalog_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/comparison_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/constant_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22194 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/correction_detail_form.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9698 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/correction_summary_form.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6408 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/correction_summary_widget.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/header_preview.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31620 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/forms/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12745 2023-04-14 16:20:25.000000 energyplus_pet-0.49/energyplus_pet/units.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:20:53.484829 energyplus_pet-0.49/energyplus_pet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-14 16:20:53.000000 energyplus_pet-0.49/energyplus_pet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-14 16:20:53.488829 energyplus_pet-0.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-04-14 16:20:25.000000 energyplus_pet-0.49/setup.py
```

### Comparing `energyplus_pet-0.48/README.md` & `energyplus_pet-0.49/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/correction_factor.py` & `energyplus_pet-0.49/energyplus_pet/correction_factor.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/data_manager.py` & `energyplus_pet-0.49/energyplus_pet/data_manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/equipment/base.py` & `energyplus_pet-0.49/energyplus_pet/equipment/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/equipment/column_header.py` & `energyplus_pet-0.49/energyplus_pet/equipment/column_header.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/equipment/common_curves.py` & `energyplus_pet-0.49/energyplus_pet/equipment/common_curves.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/equipment/equip_types.py` & `energyplus_pet-0.49/energyplus_pet/equipment/equip_types.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/equipment/manager.py` & `energyplus_pet-0.49/energyplus_pet/equipment/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/equipment/wahp_cooling_curve.py` & `energyplus_pet-0.49/energyplus_pet/equipment/wahp_cooling_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/equipment/wahp_heating_curve.py` & `energyplus_pet-0.49/energyplus_pet/equipment/wahp_heating_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/equipment/wwhp_cooling_curve.py` & `energyplus_pet-0.49/energyplus_pet/equipment/wwhp_cooling_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/equipment/wwhp_heating_curve.py` & `energyplus_pet-0.49/energyplus_pet/equipment/wwhp_heating_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/forms/base_data_form.py` & `energyplus_pet-0.49/energyplus_pet/forms/base_data_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/forms/basic_message_form.py` & `energyplus_pet-0.49/energyplus_pet/forms/basic_message_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/forms/catalog_plot.py` & `energyplus_pet-0.49/energyplus_pet/forms/catalog_plot.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/forms/comparison_plot.py` & `energyplus_pet-0.49/energyplus_pet/forms/comparison_plot.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/forms/constant_parameters.py` & `energyplus_pet-0.49/energyplus_pet/forms/constant_parameters.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/forms/correction_detail_form.py` & `energyplus_pet-0.49/energyplus_pet/forms/correction_detail_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/forms/correction_summary_form.py` & `energyplus_pet-0.49/energyplus_pet/forms/correction_summary_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/forms/correction_summary_widget.py` & `energyplus_pet-0.49/energyplus_pet/forms/correction_summary_widget.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/forms/header_preview.py` & `energyplus_pet-0.49/energyplus_pet/forms/header_preview.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/forms/main.py` & `energyplus_pet-0.49/energyplus_pet/forms/main.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet/units.py` & `energyplus_pet-0.49/energyplus_pet/units.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.48/energyplus_pet.egg-info/PKG-INFO` & `energyplus_pet-0.49/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
-Name: energyplus-pet
-Version: 0.48
+Name: energyplus_pet
+Version: 0.49
 Summary: Parameter Estimation Tools for Generating EnergyPlus Inputs from Raw Performance Data
 Home-page: https://github.com/Myoldmopar/EnergyPlusPet
-Author: Edwin Lee
-Author-email: a@a.a
-License: UnlicensedForNow
+Author: Edwin Lee, for NREL, for United States Department of Energy
+License: ModifiedBSD
 Description: # EnergyPlus "PET"
         
         This project is a cross platform Python (Tk) GUI and tool kit for generating EnergyPlus inputs from component performance data. 
         
         ## Code Quality
         
         [![Flake8](https://github.com/Myoldmopar/EnergyPlusPET/actions/workflows/flake8.yml/badge.svg)](https://github.com/Myoldmopar/EnergyPlusPET/actions/workflows/flake8.yml)
@@ -29,9 +28,20 @@
         
         [![PyPIRelease](https://github.com/Myoldmopar/EnergyPlusPET/actions/workflows/release.yml/badge.svg)](https://github.com/Myoldmopar/EnergyPlusPET/actions/workflows/release.yml)
         
         When a release is tagged, a GitHub Action workflow will create a Python wheel and upload it to the PyPi server.
         
         To install into an existing Python environment, execute `pip install energyplus_pet`
         
-Platform: UNKNOWN
+Keywords: energyplus_launch,ep_launch,EnergyPlus,eplus,Energy+,Building Simulation,Whole Building Energy Simulation,Heat Transfer,HVAC,Modeling
+Platform: Linux (Tested on Ubuntu)
+Platform: MacOSX
+Platform: Windows
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `energyplus_pet-0.48/energyplus_pet.egg-info/SOURCES.txt` & `energyplus_pet-0.49/energyplus_pet.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.cfg
 setup.py
 energyplus_pet/__init__.py
 energyplus_pet/__main__.py
 energyplus_pet/configure.py
 energyplus_pet/correction_factor.py
```

