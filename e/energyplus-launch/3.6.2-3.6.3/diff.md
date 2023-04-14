# Comparing `tmp/energyplus_launch-3.6.2.tar.gz` & `tmp/energyplus_launch-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_launch-3.6.2.tar", last modified: Wed Apr 12 21:08:44 2023, max compression
+gzip compressed data, was "energyplus_launch-3.6.3.tar", last modified: Fri Apr 14 15:30:34 2023, max compression
```

## Comparing `energyplus_launch-3.6.2.tar` & `energyplus_launch-3.6.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:44.361879 energyplus_launch-3.6.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-12 21:08:44.361879 energyplus_launch-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:44.357879 energyplus_launch-3.6.2/energyplus_launch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-12 21:08:44.000000 energyplus_launch-3.6.2/energyplus_launch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-12 21:08:44.000000 energyplus_launch-3.6.2/energyplus_launch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 21:08:44.000000 energyplus_launch-3.6.2/energyplus_launch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-12 21:08:44.000000 energyplus_launch-3.6.2/energyplus_launch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-12 21:08:44.000000 energyplus_launch-3.6.2/energyplus_launch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-12 21:08:44.000000 energyplus_launch-3.6.2/energyplus_launch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:44.357879 energyplus_launch-3.6.2/eplaunch/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:44.361879 energyplus_launch-3.6.2/eplaunch/interface/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/interface/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/interface/dialog_external_viewers.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/interface/dialog_generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/interface/dialog_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/interface/dialog_weather.py
--rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/interface/dialog_workflow_dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    68908 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/interface/frame_main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5813 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/interface/widget_dir_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/interface/widget_file_list.py
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/tk_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:44.361879 energyplus_launch-3.6.2/eplaunch/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/utilities/crossplatform.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/utilities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:44.361879 energyplus_launch-3.6.2/eplaunch/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:44.361879 energyplus_launch-3.6.2/eplaunch/workflows/default/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/workflows/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/workflows/default/file_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/workflows/default/idf_details.py
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/workflows/default/site_location.py
--rw-r--r--   0 runner    (1001) docker     (122)    10103 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/workflows/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/workflows/workflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/workflows/workflow_tester.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/eplaunch/workflows/workflow_thread.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-12 21:08:44.361879 energyplus_launch-3.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-04-12 21:08:39.000000 energyplus_launch-3.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.930502 energyplus_launch-3.6.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-14 15:30:34.930502 energyplus_launch-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.926502 energyplus_launch-3.6.3/energyplus_launch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3759 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-14 15:30:34.000000 energyplus_launch-3.6.3/energyplus_launch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.926502 energyplus_launch-3.6.3/eplaunch/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.926502 energyplus_launch-3.6.3/eplaunch/interface/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5989 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/dialog_external_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/dialog_generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/dialog_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4914 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/dialog_weather.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/dialog_workflow_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69368 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/frame_main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5748 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/widget_dir_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/interface/widget_file_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/tk_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.926502 energyplus_launch-3.6.3/eplaunch/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/utilities/crossplatform.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/utilities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.930502 energyplus_launch-3.6.3/eplaunch/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4817 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:34.930502 energyplus_launch-3.6.3/eplaunch/workflows/default/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/default/file_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3266 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/default/idf_details.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/default/site_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10103 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/workflow_tester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/eplaunch/workflows/workflow_thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-14 15:30:34.930502 energyplus_launch-3.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2063 2023-04-14 15:30:30.000000 energyplus_launch-3.6.3/setup.py
```

### Comparing `energyplus_launch-3.6.2/LICENSE` & `energyplus_launch-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/PKG-INFO` & `energyplus_launch-3.6.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_launch
-Version: 3.6.2
+Version: 3.6.3
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
@@ -39,9 +39,20 @@
         
         Basic development dependencies are installed with `pip install -r requirements.txt`.
         This cross platform GUI application is built around the tkinter framework, so no additional dependencies are needed for the GUI.
         The application can be run by executing the module as `python -m eplaunch` file.
         To run the unit test suite, simply execute `nosetests`.
         Unit test results will appear in the console, and coverage results will be in a `cover` directory.
         
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

### Comparing `energyplus_launch-3.6.2/README.md` & `energyplus_launch-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/energyplus_launch.egg-info/PKG-INFO` & `energyplus_launch-3.6.3/energyplus_launch.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-launch
-Version: 3.6.2
+Version: 3.6.3
 Summary: Graphical Interface and Workflow Manager for EnergyPlus
 Home-page: https://github.com/NREL/EP-Launch
 Author: Jason Glazer and Edwin Lee for the United States Department of Energy
 License: ModifiedBSD
 Description: # EP-Launch3
         
         [![GitHub release](https://img.shields.io/github/release/nrel/ep-launch.svg?style=for-the-badge)](https://github.com/nrel/ep-launch/releases/latest)
@@ -39,9 +39,20 @@
         
         Basic development dependencies are installed with `pip install -r requirements.txt`.
         This cross platform GUI application is built around the tkinter framework, so no additional dependencies are needed for the GUI.
         The application can be run by executing the module as `python -m eplaunch` file.
         To run the unit test suite, simply execute `nosetests`.
         Unit test results will appear in the console, and coverage results will be in a `cover` directory.
         
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

### Comparing `energyplus_launch-3.6.2/energyplus_launch.egg-info/SOURCES.txt` & `energyplus_launch-3.6.3/energyplus_launch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/interface/config.py` & `energyplus_launch-3.6.3/eplaunch/interface/config.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/interface/dialog_external_viewers.py` & `energyplus_launch-3.6.3/eplaunch/interface/dialog_external_viewers.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/interface/dialog_generic.py` & `energyplus_launch-3.6.3/eplaunch/interface/dialog_generic.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/interface/dialog_output.py` & `energyplus_launch-3.6.3/eplaunch/interface/dialog_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,20 +38,17 @@
         self.after(20, self._size_window)
 
     def _size_window(self):
         current_height = max(self.winfo_height(), 440)
         self.geometry('%dx%d+%d+%d' % (500, current_height, self.x, self.y))
 
     def add_output(self, message: str):
-        fully_scrolled_down = self.text_output.yview()[1] == 1.0
         self.text_output.insert(END, message)
         self.text_output.insert(END, '\n')
-        if fully_scrolled_down:
-            self.text_output.see(END)
-        self.update()
+        self.text_output.see(END)
 
     def close(self):
         self.destroy()
 
 
 if __name__ == "__main__":
     root = Tk()
```

### Comparing `energyplus_launch-3.6.2/eplaunch/interface/dialog_weather.py` & `energyplus_launch-3.6.3/eplaunch/interface/dialog_weather.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/interface/dialog_workflow_dirs.py` & `energyplus_launch-3.6.3/eplaunch/interface/dialog_workflow_dirs.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/interface/frame_main.py` & `energyplus_launch-3.6.3/eplaunch/interface/frame_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 from json import dumps
 from mimetypes import guess_type
 from pathlib import Path
 from platform import system
 from queue import Queue
 
 from subprocess import Popen
-from tkinter import Tk, PhotoImage, StringVar, Menu, DISABLED, OptionMenu, Frame, Label, Button, NSEW, E, VERTICAL, \
-    SUNKEN, S, LEFT, BOTH, messagebox, END, BooleanVar, ACTIVE, LabelFrame, RIGHT, EW, NS, filedialog, \
+from tkinter import Tk, PhotoImage, StringVar, Menu, DISABLED, Frame, Label, NSEW, E, VERTICAL, \
+    SUNKEN, S, LEFT, BOTH, messagebox, END, BooleanVar, NORMAL, RIGHT, EW, NS, filedialog, \
     ALL, Listbox, Scrollbar, SINGLE, Variable, HORIZONTAL
-from tkinter.ttk import Combobox, PanedWindow as ttkPanedWindow
+from tkinter.ttk import Combobox, PanedWindow as ttkPanedWindow, OptionMenu, LabelFrame
+if system() == 'Darwin':
+    from tkmacosx import Button
+else:
+    from tkinter.ttk import Button
 from typing import Dict, List, Optional, Tuple
 from uuid import uuid4
 from webbrowser import open as open_web
 from plan_tools.runtime import fixup_taskbar_icon_on_windows
 
 from eplaunch import VERSION, DOCS_URL, NAME
 from eplaunch.interface.dialog_generic import TkGenericDialog
@@ -114,15 +118,15 @@
 
         # finally set the initial directory and update the file listing
         self.dir_tree.dir_list.refresh_listing(self.conf.directory)
         self._update_file_list()
 
         # set the minimum size and redraw the app
         self.minsize(1050, 400)
-        self.update()
+        self.update()  # one quick redraw should be fine here to get updated geometry
         self.dir_files_pw.sashpos(0, self.conf.dir_file_paned_window_sash_position)
         self.conf.list_group_paned_window_sash_position = min(
             self.conf.list_group_paned_window_sash_position, self.winfo_height() - 250
         )
         self.list_group_pw.sashpos(0, self.conf.list_group_paned_window_sash_position)
 
         # one time update of the status bar
@@ -234,43 +238,49 @@
         lf = LabelFrame(container, text="Workflow Selection")
         Label(lf, text="Context:", justify=RIGHT).grid(row=0, column=0, sticky=E, **self.pad)
         self.option_workflow_context = OptionMenu(lf, self._tk_var_workflow_context, '<context>')
         self.option_workflow_context.grid(row=0, column=1, sticky=EW, **self.pad)
         Label(lf, text="Workflow:", justify=RIGHT).grid(row=1, column=0, sticky=E, **self.pad)
         self.option_workflow_instance = OptionMenu(lf, self._tk_var_workflow_instance, '<instance>')
         self.option_workflow_instance.grid(row=1, column=1, sticky=EW, **self.pad)
+        lf.grid_rowconfigure(ALL, weight=1)
+        lf.grid_columnconfigure(ALL, weight=1)
         lf.grid(row=0, column=0, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Run Workflow on...")
-        Button(
-            lf, text=u"\U000025B6 Selected File(s)", command=self._run_workflow_on_selection
-        ).grid(row=0, column=0, sticky=EW, **self.pad)
-        Button(
-            lf, text=u"\U000025B6 Current Group", command=self._run_workflow_on_group
-        ).grid(row=1, column=0, sticky=EW, **self.pad)
+        b = Button(lf, text=u"\U000025B6 Selected File(s)", command=self._run_workflow_on_selection, state=NORMAL)
+        b.grid(row=0, column=0, sticky=EW, **self.pad)
+        b = Button(lf, text=u"\U000025B6 Current Group", command=self._run_workflow_on_group, state=NORMAL)
+        b.grid(row=1, column=0, sticky=EW, **self.pad)
+        lf.grid_rowconfigure(ALL, weight=1)
+        lf.grid_columnconfigure(ALL, weight=1)
         lf.grid(row=0, column=1, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Weather Selection")
         Label(lf, text="Recent: ", justify=RIGHT).grid(row=0, column=0, **self.pad)
         self.option_weather_recent = OptionMenu(lf, self._tk_var_weather_recent, '<weather>')
         self.option_weather_recent.grid(row=0, column=1, sticky=EW, **self.pad)
         self.button_weather_select = Button(
             lf, text=u"\U0001f325 Select Weather File...", command=self._open_weather_dialog
         )
         self.button_weather_select.grid(row=1, column=0, columnspan=2, sticky=EW, **self.pad)
+        lf.grid_rowconfigure(ALL, weight=1)
+        lf.grid_columnconfigure(ALL, weight=1)
         lf.grid(row=0, column=2, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Quicklinks")
         self.button_open_in_text = Button(
             lf, text=u"\U0001F5B9 Open File in Text Editor", command=self._open_text_editor, state=DISABLED
         )
         self.button_open_in_text.grid(row=0, column=0, columnspan=3, sticky=EW, **self.pad)
         Button(
-            lf, text=u"\U0001F5C0 Open Dir in File Browser", command=self._open_file_browser
+            lf, text=u"\U0001F5C0 Open Dir in File Browser", command=self._open_file_browser, state=NORMAL
         ).grid(row=1, column=0, columnspan=3, sticky=EW, **self.pad)
+        lf.grid_rowconfigure(ALL, weight=1)
+        lf.grid_columnconfigure(ALL, weight=1)
         lf.grid(row=0, column=3, sticky=NS, **self.pad)
 
         lf = LabelFrame(container, text="Open Outputs")
         sub_frame = Frame(lf)
         self.button_open_output_1 = Button(
             sub_frame, textvariable=self._tk_var_output_1, command=self._open_output_1, state=DISABLED
         )
@@ -728,15 +738,15 @@
                     if output_file_date < input_file_date:
                         return True
         return False
 
     def _callback_file_selection_changed(self, selected_file_names: List[str]) -> None:
         """This gets called back by the file listing widget when a selection changes"""
         self.conf.file_selection = selected_file_names
-        status = ACTIVE if len(self.conf.file_selection) > 0 else DISABLED
+        status = NORMAL if len(self.conf.file_selection) > 0 else DISABLED
         self.button_open_in_text['state'] = status
         self._refresh_output_suffix_buttons_based_on_selection()
 
     # endregion
 
     # region weather operations
 
@@ -756,21 +766,20 @@
             self._handler_weather_recent_option_changed(try_to_select)
         elif len(self.conf.weathers_recent) > 0:
             self._handler_weather_recent_option_changed(self.conf.weathers_recent[0])  # could persist in self.conf
 
     def _handler_weather_recent_option_changed(self, new_weather_path: Path):
         """This is called when the recent weather option menu changes value"""
         self._tk_var_weather_recent.set(str(new_weather_path.name))
-        selected_recent_weather_string = self._tk_var_weather_recent.get()
         for selected_file_name in self.conf.file_selection:
             cache = CacheFile(self.conf.directory)
             cache.add_config(
                 self.workflow_manager.current_workflow.name,
                 selected_file_name,
-                {'weather': selected_recent_weather_string}
+                {'weather': str(new_weather_path)}
             )
         self._update_file_list()
 
     def _open_weather_dialog(self) -> None:
         dialog_weather = TkWeatherDialog(self, list(self.conf.weathers_recent))
         self.wait_window(dialog_weather)
         if dialog_weather.exit_code == TkWeatherDialog.CLOSE_SIGNAL_CANCEL:
@@ -863,48 +872,48 @@
                 new_workflow = w
                 break
         if new_workflow is None:
             messagebox.showerror("There was an unexpected error updating the workflow list, suggest restarting app.")
         # assign the current workflow instance in the workflow manager
         self.workflow_manager.current_workflow = new_workflow
         # update the weather buttons accordingly depending on if the workflow uses weather inputs
-        self._set_weather_widget_state(ACTIVE if new_workflow.uses_weather else DISABLED)
+        self._set_weather_widget_state(NORMAL if new_workflow.uses_weather else DISABLED)
         # clear the output menu entirely, and set status conditionally
         self._repopulate_output_suffix_options()
         # now that the workflow has been set, repopulate the file list columns and the file list itself
         self._repopulate_control_list_columns()
         self._update_file_list()
 
     def _repopulate_output_suffix_options(self):
         sorted_suffixes = sorted(self.workflow_manager.current_workflow.output_suffixes)
         combobox_output_enabled = 'readonly' if len(sorted_suffixes) > 0 else 'disabled'
-        output_enabled = ACTIVE if len(sorted_suffixes) > 0 else DISABLED
+        output_enabled = NORMAL if len(sorted_suffixes) > 0 else DISABLED
         self.option_workflow_outputs.configure(state=combobox_output_enabled)
         self.button_open_output_file.configure(state=output_enabled)
 
         # rebuild the option menu if applicable
         current_selection = self._tk_var_output_suffix.get()
-        if output_enabled == ACTIVE:
+        if output_enabled == NORMAL:
             self.option_workflow_outputs['values'] = sorted_suffixes
             if current_selection not in sorted_suffixes:
                 self._tk_var_output_suffix.set(sorted_suffixes[0])
         else:
             self.option_workflow_outputs['values'] = []
             self._tk_var_output_suffix.set('')
         self.option_workflow_outputs.selection_clear()
         suffixes = self.workflow_manager.current_workflow.output_suffixes
-        self.button_open_output_1.configure(state=ACTIVE if len(suffixes) > 0 else DISABLED)
+        self.button_open_output_1.configure(state=NORMAL if len(suffixes) > 0 else DISABLED)
         self._tk_var_output_1.set(suffixes[0] if len(suffixes) > 0 else '--')
-        self.button_open_output_2.configure(state=ACTIVE if len(suffixes) > 1 else DISABLED)
+        self.button_open_output_2.configure(state=NORMAL if len(suffixes) > 1 else DISABLED)
         self._tk_var_output_2.set(suffixes[1] if len(suffixes) > 1 else '--')
-        self.button_open_output_3.configure(state=ACTIVE if len(suffixes) > 2 else DISABLED)
+        self.button_open_output_3.configure(state=NORMAL if len(suffixes) > 2 else DISABLED)
         self._tk_var_output_3.set(suffixes[2] if len(suffixes) > 2 else '--')
-        self.button_open_output_4.configure(state=ACTIVE if len(suffixes) > 3 else DISABLED)
+        self.button_open_output_4.configure(state=NORMAL if len(suffixes) > 3 else DISABLED)
         self._tk_var_output_4.set(suffixes[3] if len(suffixes) > 3 else '--')
-        self.button_open_output_5.configure(state=ACTIVE if len(suffixes) > 4 else DISABLED)
+        self.button_open_output_5.configure(state=NORMAL if len(suffixes) > 4 else DISABLED)
         self._tk_var_output_5.set(suffixes[4] if len(suffixes) > 4 else '--')
         self._refresh_output_suffix_buttons_based_on_selection()
 
     def suffixed_paths_exist(self, original_path: Path, new_suffix: str) -> Tuple[Optional[Path], Optional[Path]]:
         filename_no_ext = original_path.with_suffix('').name
         new_path = self.conf.directory / (filename_no_ext + new_suffix)
         eplus_sub_dir = f"EPLaunchRun_{filename_no_ext}"
@@ -923,15 +932,15 @@
                 original_path = self.conf.directory / f
                 new_path, eplus_path = self.suffixed_paths_exist(original_path, suffix_to_open)
                 if (new_path and new_path.exists()) or (eplus_path and eplus_path.exists()):
                     pass  # good
                 else:
                     all_files_have_this_suffix = False
                     break
-            button.configure(state=ACTIVE if all_files_have_this_suffix else DISABLED)
+            button.configure(state=NORMAL if all_files_have_this_suffix else DISABLED)
 
     def _refresh_output_suffix_buttons_based_on_selection(self):
         self._refresh_single_output_suffix_button(self._tk_var_output_1, self.button_open_output_1)
         self._refresh_single_output_suffix_button(self._tk_var_output_2, self.button_open_output_2)
         self._refresh_single_output_suffix_button(self._tk_var_output_3, self.button_open_output_3)
         self._refresh_single_output_suffix_button(self._tk_var_output_4, self.button_open_output_4)
         self._refresh_single_output_suffix_button(self._tk_var_output_5, self.button_open_output_5)
```

### Comparing `energyplus_launch-3.6.2/eplaunch/interface/widget_dir_list.py` & `energyplus_launch-3.6.3/eplaunch/interface/widget_dir_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,21 +55,19 @@
         # default double click behavior is to reset the root to the double-clicked folder
         if single_selected_item_id == self.root_node:
             return
         # values will only hold one extra item, the absolute path for that node
         clicked_node_path = item_contents['values'][0]
         self.refresh_listing(Path(clicked_node_path))
 
-    def reset_tree(self, redraw: bool = False):
+    def reset_tree(self):
         self.heading('#0', text="(Dir Path)", anchor='w', command=self.select_new_root)
         for item in self.directory_node_ids:
             self.delete(item)
         self.directory_node_ids.clear()
-        if redraw:
-            self.update()
 
     def select_new_root(self):
         response = filedialog.askdirectory()
         if not response:
             return
         p = Path(response)
         if p.exists():
@@ -92,15 +90,15 @@
                 new_id = self.insert(
                     self.root_node, 'end', text=str(p.name), open=False, values=(str(p),),
                     image=self.non_root_folder_image
                 )
                 self.directory_node_ids.append(new_id)
             # elif p.is_file() and not p.name.startswith('.') and not p.name.startswith('__'):
             #     print(f"Filename \"{p.name}\"; File path \"{str(p)}\"")
-        self.update()
+        # self.update()
         if new_path and self.callback_on_root_changed:
             self.callback_on_root_changed(new_path)
         self.selection_set(self.root_node)
 
 
 class DirListScrollableFrame(Frame):
     def __init__(
```

### Comparing `energyplus_launch-3.6.2/eplaunch/interface/widget_file_list.py` & `energyplus_launch-3.6.3/eplaunch/interface/widget_file_list.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/utilities/cache.py` & `energyplus_launch-3.6.3/eplaunch/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/utilities/crossplatform.py` & `energyplus_launch-3.6.3/eplaunch/utilities/crossplatform.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/utilities/version.py` & `energyplus_launch-3.6.3/eplaunch/utilities/version.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/workflows/base.py` & `energyplus_launch-3.6.3/eplaunch/workflows/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/workflows/default/file_details.py` & `energyplus_launch-3.6.3/eplaunch/workflows/default/file_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/workflows/default/idf_details.py` & `energyplus_launch-3.6.3/eplaunch/workflows/default/idf_details.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/workflows/default/site_location.py` & `energyplus_launch-3.6.3/eplaunch/workflows/default/site_location.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/workflows/manager.py` & `energyplus_launch-3.6.3/eplaunch/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/workflows/workflow.py` & `energyplus_launch-3.6.3/eplaunch/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/workflows/workflow_tester.py` & `energyplus_launch-3.6.3/eplaunch/workflows/workflow_tester.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/eplaunch/workflows/workflow_thread.py` & `energyplus_launch-3.6.3/eplaunch/workflows/workflow_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_launch-3.6.2/setup.py` & `energyplus_launch-3.6.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from eplaunch import NAME, VERSION
 
 
 readme_file = Path(__file__).parent.resolve() / 'README.md'
 readme_contents = readme_file.read_text()
 
-install_requires = ['PLAN-Tools>=0.5']
+install_requires = ['PLAN-Tools>=0.5', 'tkmacosx']
 if system() == 'Windows':
     install_requires.append('pypiwin32')
 
 setup(
     name=NAME,
     version=VERSION,
     description='Graphical Interface and Workflow Manager for EnergyPlus',
@@ -34,9 +34,28 @@
         'gui_scripts': [
             'energyplus_launch=eplaunch.tk_runner:main_gui',
         ],
         'console_scripts': [
             'energyplus_launch_configure=eplaunch.configure:configure_cli',
             'energyplus_launch_workflow_tester=eplaunch.workflows.workflow_tester:cli'
         ]
-    }
+    },
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Science/Research',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3 :: Only',
+        'Topic :: Scientific/Engineering',
+        'Topic :: Scientific/Engineering :: Physics',
+        'Topic :: Utilities',
+    ],
+    platforms=[
+        'Linux (Tested on Ubuntu)', 'MacOSX', 'Windows'
+    ],
+    keywords=[
+        'energyplus_launch', 'ep_launch',
+        'EnergyPlus', 'eplus', 'Energy+',
+        'Building Simulation', 'Whole Building Energy Simulation',
+        'Heat Transfer', 'HVAC', 'Modeling',
+    ]
 )
```

