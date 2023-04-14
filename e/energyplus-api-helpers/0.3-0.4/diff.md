# Comparing `tmp/energyplus_api_helpers-0.3.tar.gz` & `tmp/energyplus_api_helpers-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_api_helpers-0.3.tar", last modified: Thu Mar  2 20:09:25 2023, max compression
+gzip compressed data, was "energyplus_api_helpers-0.4.tar", last modified: Fri Apr 14 15:22:46 2023, max compression
```

## Comparing `energyplus_api_helpers-0.3.tar` & `energyplus_api_helpers-0.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 20:09:24.998871 energyplus_api_helpers-0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-03-02 20:09:24.998871 energyplus_api_helpers-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 20:09:24.994871 energyplus_api_helpers-0.3/energyplus_api_helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 20:09:24.998871 energyplus_api_helpers-0.3/energyplus_api_helpers/demos/
--rw-r--r--   0 runner    (1001) docker     (122)      524 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/demos/01_simple_library_call.py
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/demos/02_threaded.py
--rw-r--r--   0 runner    (1001) docker     (122)     1121 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/demos/03_multiprocessed.py
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/demos/04_dynamic_terminal_output_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/demos/05_dynamic_terminal_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/demos/06_plot_e_plus.py
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/demos/07_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     3874 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/demos/08_server_advanced.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/energyplus_api_helpers/import_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 20:09:24.994871 energyplus_api_helpers-0.3/energyplus_api_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-03-02 20:09:24.000000 energyplus_api_helpers-0.3/energyplus_api_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-03-02 20:09:24.000000 energyplus_api_helpers-0.3/energyplus_api_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-02 20:09:24.000000 energyplus_api_helpers-0.3/energyplus_api_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-03-02 20:09:24.000000 energyplus_api_helpers-0.3/energyplus_api_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-02 20:09:24.000000 energyplus_api_helpers-0.3/energyplus_api_helpers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-02 20:09:24.998871 energyplus_api_helpers-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-03-02 20:09:13.000000 energyplus_api_helpers-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:22:46.424359 energyplus_api_helpers-0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-04-14 15:22:46.424359 energyplus_api_helpers-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:22:46.420359 energyplus_api_helpers-0.4/energyplus_api_helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:22:46.424359 energyplus_api_helpers-0.4/energyplus_api_helpers/demos/
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/demos/01_simple_library_call.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/demos/02_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1121 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/demos/03_multiprocessed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/demos/04_dynamic_terminal_output_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/demos/05_dynamic_terminal_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2939 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/demos/06_plot_e_plus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/demos/07_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3874 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/demos/08_server_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/energyplus_api_helpers/import_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:22:46.420359 energyplus_api_helpers-0.4/energyplus_api_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-04-14 15:22:46.000000 energyplus_api_helpers-0.4/energyplus_api_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-04-14 15:22:46.000000 energyplus_api_helpers-0.4/energyplus_api_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 15:22:46.000000 energyplus_api_helpers-0.4/energyplus_api_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-14 15:22:46.000000 energyplus_api_helpers-0.4/energyplus_api_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-14 15:22:46.000000 energyplus_api_helpers-0.4/energyplus_api_helpers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-14 15:22:46.424359 energyplus_api_helpers-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-04-14 15:22:34.000000 energyplus_api_helpers-0.4/setup.py
```

### Comparing `energyplus_api_helpers-0.3/PKG-INFO` & `energyplus_api_helpers-0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: energyplus_api_helpers
-Version: 0.3
+Version: 0.4
 Summary: A set of helper classes, functions and demos, for interacting with the EnergyPlus Python API
 Home-page: https://github.com/Myoldmopar/EnergyPlusAPIHelper
-Author: Edwin Lee
-Author-email: a@a.a
-License: UnlicensedForNow
+Author: Edwin Lee, for NREL, for the United States Department of Energy
+License: ModifiedBSD
 Description: # EnergyPlus API Helper Scripts
         
         This project is a small library of helper functionality and, more importantly, demo scripts, for interacting with the EnergyPlus API.
         The EnergyPlus Python API is not on PyPi (as of now), it simply comes with the EnergyPlus installation.
         This library makes that process a bit easier, and also offers a set of demos in the `energyplus_api_helpers/demos` folder.
         
         A super minimal example using the helper class here:
@@ -38,9 +37,20 @@
         
         [![PyPIRelease](https://github.com/Myoldmopar/EnergyPlusAPIDemos/actions/workflows/release.yml/badge.svg)](https://github.com/Myoldmopar/EnergyPlusAPIDemos/actions/workflows/release.yml)
         
         When a release is tagged, a GitHub Action workflow will create a Python wheel and upload it to the PyPi server.
         
         To install into an existing Python environment, execute `pip install energyplus_api_helpers`
         
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

### Comparing `energyplus_api_helpers-0.3/README.md` & `energyplus_api_helpers-0.4/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_api_helpers-0.3/energyplus_api_helpers/demos/01_simple_library_call.py` & `energyplus_api_helpers-0.4/energyplus_api_helpers/demos/01_simple_library_call.py`

 * *Files identical despite different names*

### Comparing `energyplus_api_helpers-0.3/energyplus_api_helpers/demos/02_threaded.py` & `energyplus_api_helpers-0.4/energyplus_api_helpers/demos/02_threaded.py`

 * *Files identical despite different names*

### Comparing `energyplus_api_helpers-0.3/energyplus_api_helpers/demos/03_multiprocessed.py` & `energyplus_api_helpers-0.4/energyplus_api_helpers/demos/03_multiprocessed.py`

 * *Files identical despite different names*

### Comparing `energyplus_api_helpers-0.3/energyplus_api_helpers/demos/04_dynamic_terminal_output_progress.py` & `energyplus_api_helpers-0.4/energyplus_api_helpers/demos/04_dynamic_terminal_output_progress.py`

 * *Files identical despite different names*

### Comparing `energyplus_api_helpers-0.3/energyplus_api_helpers/demos/05_dynamic_terminal_output.py` & `energyplus_api_helpers-0.4/energyplus_api_helpers/demos/05_dynamic_terminal_output.py`

 * *Files identical despite different names*

### Comparing `energyplus_api_helpers-0.3/energyplus_api_helpers/demos/06_plot_e_plus.py` & `energyplus_api_helpers-0.4/energyplus_api_helpers/demos/06_plot_e_plus.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.hl.set_xdata(self.x)
         self.hl.set_ydata(self.y_outdoor)
         self.h2.set_xdata(self.x)
         self.h2.set_ydata(self.y_zone)
         self.ax.relim()
         self.ax.autoscale_view()
         plt.draw()
-        plt.pause(0.00001)
+        plt.pause(0.000001)
 
 
 class EnergyPlusManager:
     def __init__(self):
         self.e = EPlusAPIHelper(Path('/eplus/installs/EnergyPlus-22-2-0'))
         self.api = self.e.get_api_instance()
         self.got_handles = False
```

### Comparing `energyplus_api_helpers-0.3/energyplus_api_helpers/demos/07_server.py` & `energyplus_api_helpers-0.4/energyplus_api_helpers/demos/07_server.py`

 * *Files identical despite different names*

### Comparing `energyplus_api_helpers-0.3/energyplus_api_helpers/demos/08_server_advanced.py` & `energyplus_api_helpers-0.4/energyplus_api_helpers/demos/08_server_advanced.py`

 * *Files identical despite different names*

### Comparing `energyplus_api_helpers-0.3/energyplus_api_helpers/import_helper.py` & `energyplus_api_helpers-0.4/energyplus_api_helpers/import_helper.py`

 * *Files identical despite different names*

### Comparing `energyplus_api_helpers-0.3/energyplus_api_helpers.egg-info/SOURCES.txt` & `energyplus_api_helpers-0.4/energyplus_api_helpers.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.py
 energyplus_api_helpers/__init__.py
 energyplus_api_helpers/import_helper.py
 energyplus_api_helpers.egg-info/PKG-INFO
 energyplus_api_helpers.egg-info/SOURCES.txt
 energyplus_api_helpers.egg-info/dependency_links.txt
```

