# Comparing `tmp/aioWiserHeatAPI-1.3.1.tar.gz` & `tmp/aioWiserHeatAPI-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioWiserHeatAPI-1.3.1.tar", last modified: Wed Mar 22 18:37:09 2023, max compression
+gzip compressed data, was "aioWiserHeatAPI-1.3.2.tar", last modified: Fri Apr 14 17:03:43 2023, max compression
```

## Comparing `aioWiserHeatAPI-1.3.1.tar` & `aioWiserHeatAPI-1.3.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:37:09.511473 aioWiserHeatAPI-1.3.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-03-22 18:37:09.511473 aioWiserHeatAPI-1.3.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4092 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:37:09.507473 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/heating.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/heating_actuator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:37:09.511473 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/automations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/extra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/opentherm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/special_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/zigbee.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/hot_water.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/rest_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    24010 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/roomstat.py
--rw-r--r--   0 runner    (1001) docker     (123)    40806 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/shutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/smartplug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/smartvalve.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/ufh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/wiserhub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 18:37:09.511473 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-03-22 18:37:09.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-22 18:37:09.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 18:37:09.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-22 18:37:09.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-22 18:37:09.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-22 18:37:09.000000 aioWiserHeatAPI-1.3.1/aioWiserHeatAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-22 18:37:09.511473 aioWiserHeatAPI-1.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-03-22 18:36:59.000000 aioWiserHeatAPI-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:03:43.353615 aioWiserHeatAPI-1.3.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-14 17:03:43.353615 aioWiserHeatAPI-1.3.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4339 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:03:43.349615 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/heating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/heating_actuator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:03:43.353615 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/extra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/opentherm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/special_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/zigbee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/hot_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/rest_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24883 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/roomstat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40806 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/smartplug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/smartvalve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/ufh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/wiserhub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:03:43.349615 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 17:03:43.000000 aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 17:03:43.353615 aioWiserHeatAPI-1.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-04-14 17:03:33.000000 aioWiserHeatAPI-1.3.2/setup.py
```

### Comparing `aioWiserHeatAPI-1.3.1/LICENSE` & `aioWiserHeatAPI-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/PKG-INFO` & `aioWiserHeatAPI-1.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aioWiserHeatAPI
-Version: 1.3.1
+Version: 1.3.2
 Summary: An AsyncIO API for controlling the Drayton Wiser Heating system
 Home-page: https://github.com/msp1974/aioWiserHeatAPI
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Drayton Wiser Hub API Async v1.3.1
+# Drayton Wiser Hub API Async v1.3.2
 
 This repository contains a simple API which queries the Drayton Wiser Heating sysystem used in the UK.
 
 The API functionality provides the following functionality to control the wiser heating system for 1,2 and 3 channel heat hubs
 The API also supports Smart Plugs and initial basic functionality for Shutter and Lights
 
 ## Requirements
@@ -64,15 +64,22 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.3.2
+
+* Fixed issue ot maintaining some parameters after hub update
+* Improved handling of extra config json errors
+* Amended current_target_temp to use DisplayedSetPoint instead of CurrentSetPoint as this displays incorrectly in Eco mode
+
 ### 1.3.1
+
 * Away mode overrides passive mode functions
 
 ### 1.3.0
 
 * Rework passive mode functionality (may break previous code if using passive mode)
 
 ### 1.2.2
```

### Comparing `aioWiserHeatAPI-1.3.1/README.md` & `aioWiserHeatAPI-1.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Drayton Wiser Hub API Async v1.3.1
+# Drayton Wiser Hub API Async v1.3.2
 
 This repository contains a simple API which queries the Drayton Wiser Heating sysystem used in the UK.
 
 The API functionality provides the following functionality to control the wiser heating system for 1,2 and 3 channel heat hubs
 The API also supports Smart Plugs and initial basic functionality for Shutter and Lights
 
 ## Requirements
@@ -48,15 +48,22 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.3.2
+
+* Fixed issue ot maintaining some parameters after hub update
+* Improved handling of extra config json errors
+* Amended current_target_temp to use DisplayedSetPoint instead of CurrentSetPoint as this displays incorrectly in Eco mode
+
 ### 1.3.1
+
 * Away mode overrides passive mode functions
 
 ### 1.3.0
 
 * Rework passive mode functionality (may break previous code if using passive mode)
 
 ### 1.2.2
```

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/cli.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/cli.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/const.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/const.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/devices.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/devices.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/discovery.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/discovery.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/heating.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/heating.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/heating_actuator.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/heating_actuator.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/automations.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/automations.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 # If room is boosted do not override
                 if not room.is_boosted:
                     # Set target temp to heat passive room in increments of passive_temperature_increment (default 0.5)
                     target_temp = min(
                         round(
                             (
                                 room.current_temperature
-                                + room.passive_temperature_increment
+                                + self._wiser_rest_controller._api_parameters.passive_mode_increment
                             )
                             * 2
                         )
                         / 2,
                         (
                             room.schedule.current_setting
                             if room.mode == WiserHeatingModeEnum.auto.value
```

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/battery.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/battery.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/capabilities.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/capabilities.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/cloud.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/cloud.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/device.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/device.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/extra_config.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/extra_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,21 @@
             async with aiofiles.open(self._config_file, mode="r") as config_file:
                 try:
                     contents = await config_file.read()
                     if contents:
                         self._config = json.loads(contents)
                     config_file.close()
 
-                except (OSError, EOFError, TypeError, AttributeError) as ex:
+                except (
+                    OSError,
+                    EOFError,
+                    TypeError,
+                    AttributeError,
+                    json.JSONDecodeError,
+                ) as ex:
                     raise WiserExtraConfigError("Error loading extra config file")
         else:
             await self.async_update_config("Info", "Version", "1.0.0")
         return
 
     async def async_update_config(self, section: str, key: str, value):
         # If section doesn't exist
@@ -48,15 +54,21 @@
 
     async def async_write_config(self):
         # Write to config file
         async with aiofiles.open(self._config_file, mode="w") as config_file:
             try:
                 await config_file.write(json.dumps(self._config, indent=2))
                 config_file.close()
-            except (OSError, EOFError, TypeError, AttributeError) as ex:
+            except (
+                OSError,
+                EOFError,
+                TypeError,
+                AttributeError,
+                json.JSONDecodeError,
+            ) as ex:
                 raise WiserExtraConfigError("Error writing to extra config file")
 
     # @property
     def config(self, section: str = None, key: str = None):
         try:
             if section:
                 if key:
```

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/firmware.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/firmware.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/network.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/network.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/opentherm.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/opentherm.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/signal.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/signal.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/special_times.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/special_times.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/temp.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/temp.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/helpers/zigbee.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/helpers/zigbee.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/hot_water.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/hot_water.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/light.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/light.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/moments.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/moments.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/rest_controller.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/rest_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,41 @@
+from dataclasses import dataclass
 import json
 
 from aioWiserHeatAPI.helpers.extra_config import _WiserExtraConfig
 from . import _LOGGER
 
 from .const import (
     REST_TIMEOUT,
     WISERHUBDOMAIN,
     WISERHUBSCHEDULES,
     WiserUnitsEnum,
 )
 
 from .exceptions import (
+    WiserExtraConfigError,
     WiserHubAuthenticationError,
     WiserHubConnectionError,
     WiserHubRESTError,
 )
 
 import asyncio
 import aiohttp
 import enum
 import re
 
 from typing import Any, Optional, cast
 
+
+@dataclass
+class WiserAPIParams:
+    passive_mode_increment = 0.5
+    stored_manual_target_temperature_alt_source = "current"
+
+
 # Connection info class
 class _WiserConnectionInfo(object):
     def __init__(self):
         self.host = None
         self.secret = None
         self.port = None
         self.units = WiserUnitsEnum.metric
@@ -51,14 +60,15 @@
         self,
         session: Optional[aiohttp.ClientSession] = None,
         timeout: Optional[float] = REST_TIMEOUT,
         wiser_connection_info: Optional[_WiserConnectionInfo] = None,
     ):
 
         self._wiser_connection_info = wiser_connection_info
+        self._api_parameters = WiserAPIParams()
 
         if not session:
             session = aiohttp.ClientSession()
         self._session = session
         self._timeout = aiohttp.ClientTimeout(total=timeout)
         self._hub_name = None
         self._extra_config_file = None
@@ -163,18 +173,24 @@
             raise_for_endpoint_error=raise_for_endpoint_error,
         )
 
     async def _get_extra_config_data(self):
         # Load extra config file
 
         if self._extra_config_file:
-            self._extra_config = _WiserExtraConfig(
-                self._extra_config_file, self._hub_name.lower()
-            )
-            await self._extra_config.async_load_config()
+            try:
+                self._extra_config = _WiserExtraConfig(
+                    self._extra_config_file, self._hub_name.lower()
+                )
+                await self._extra_config.async_load_config()
+            except WiserExtraConfigError as ex:
+                _LOGGER.error(
+                    "Your config file is corrupted and needs to be fixed to maintain all the functionality of this integration."
+                )
+                self._extra_config = None
 
     async def _send_command(
         self,
         url: str,
         command_data: dict,
         method: WiserRestActionEnum = WiserRestActionEnum.PATCH,
     ):
```

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/room.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/room.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,15 @@
         self._default_extra_config = {
             "passive_mode": False,
             "min": 14,
             "max": 18,
         }
 
         self._boost_temperature_delta = DEFAULT_BOOST_DELTA
-        self.stored_manual_target_temperature_alt_source = "current"
-        self.passive_temperature_increment = 0.5
+        # self.stored_manual_target_temperature_alt_source = "current"
 
         # Add device id to schedule
         if self._schedule:
             self.schedule._assignments.append({"id": self.id, "name": self.name})
 
     def _effective_heating_mode(self, mode: str, temp: float) -> str:
         if mode.casefold() == TEXT_MANUAL.casefold() and temp == TEMP_OFF:
@@ -94,18 +93,24 @@
                 "Wiser room - {} command successful - {}".format(
                     inspect.stack()[1].function, result
                 )
             )
             return True
         return False
 
-    async def _update_extra_config(self, key: str, value):
-        await self._wiser_rest_controller._extra_config.async_update_config(
-            "Rooms", str(self.id), {key: value}
-        )
+    async def _update_extra_config(self, key: str, value) -> bool:
+        if self._wiser_rest_controller._extra_config:
+            try:
+                await self._wiser_rest_controller._extra_config.async_update_config(
+                    "Rooms", str(self.id), {key: value}
+                )
+                return True
+            except Exception:
+                return False
+        return False
 
     @property
     def is_passive_mode(self) -> bool:
         return (
             True
             if self._enable_automations
             and self.passive_mode_enabled
@@ -144,30 +149,41 @@
             return self.schedule.current_setting
         else:
             if self._extra_config and "max" in self._extra_config:
                 return self._extra_config["max"]
             return self._default_extra_config["max"]
 
     async def set_passive_mode(self, enable: bool):
-        await self._update_extra_config("passive_mode", enable)
-
-        if not self.is_away_mode:
-            # Set to min of temp range when initialised
-            if enable and self.mode != WiserHeatingModeEnum.off.value:
-                await self.set_target_temperature(self.passive_mode_lower_temp)
-
-            # Set target temp back to last manual temp if in manual mode
-            if (not enable) and self.mode == WiserHeatingModeEnum.manual.value:
-                await self.set_target_temperature(self.stored_manual_target_temperature)
+        if await self._update_extra_config("passive_mode", enable):
+            if not self.is_away_mode:
+                # Set to min of temp range when initialised
+                if enable and self.mode != WiserHeatingModeEnum.off.value:
+                    await self.set_target_temperature(self.passive_mode_lower_temp)
+
+                # Set target temp back to last manual temp if in manual mode
+                if (not enable) and self.mode == WiserHeatingModeEnum.manual.value:
+                    await self.set_target_temperature(
+                        self.stored_manual_target_temperature
+                    )
+        else:
+            _LOGGER.error(
+                "Unable to set passive mode.  This maybe caused by an issue with your extra config file."
+            )
 
     async def set_passive_mode_lower_temp(self, temp):
-        await self._update_extra_config("min", temp)
+        if not await self._update_extra_config("min", temp):
+            _LOGGER.error(
+                "Unable to set passive lower temp.  This maybe caused by an issue with your extra config file."
+            )
 
     async def set_passive_mode_upper_temp(self, temp):
-        await self._update_extra_config("max", temp)
+        if not await self._update_extra_config("max", temp):
+            _LOGGER.error(
+                "Unable to set passive mode upper temp.  This maybe caused by an issue with your extra config file."
+            )
 
     @property
     def available_modes(self) -> list:
         """Get available heating modes"""
         return [mode.value for mode in WiserHeatingModeEnum]
 
     @property
@@ -218,15 +234,15 @@
     def control_direction(self) -> str:
         """Get room heating control direction Heat or Cool"""
         return self._data.get("ControlDirection", TEXT_UNKNOWN)
 
     @property
     def current_target_temperature(self) -> float:
         """Get current target temperature for the room"""
-        return tf._from_wiser_temp(self._data.get("CurrentSetPoint", TEMP_MINIMUM))
+        return tf._from_wiser_temp(self._data.get("DisplayedSetPoint", TEMP_MINIMUM))
 
     @property
     def current_temperature(self) -> float:
         """Get current temperature of the room"""
         return tf._from_wiser_temp(
             self._data.get("CalculatedTemperature", TEMP_MINIMUM), "current"
         )
@@ -453,18 +469,22 @@
         """Get list of smartvalve ids associated with room"""
         return sorted(self._data.get("SmartValveIds", []))
 
     @property
     def stored_manual_target_temperature(self) -> float:
         if self._extra_config and "manual_temp" in self._extra_config:
             return self._extra_config["manual_temp"]
-        elif self.stored_manual_target_temperature_alt_source == "current":
+        elif (
+            self._wiser_rest_controller._api_parameters.stored_manual_target_temperature_alt_source.lower()
+            == "current"
+        ):
             return self.current_temperature
         elif (
-            self.stored_manual_target_temperature_alt_source == "scheduled"
+            self._wiser_rest_controller._api_parameters.stored_manual_target_temperature_alt_source.lower()
+            == "scheduled"
             and self.schedule
         ):
             return self.scheduled_target_temperature
         return TEMP_MINIMUM
 
     @property
     def target_temperature_origin(self) -> str:
```

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/roomstat.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/roomstat.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/schedule.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/shutter.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/shutter.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/smartplug.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/smartplug.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/smartvalve.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/smartvalve.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/system.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/system.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/ufh.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/ufh.py`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI/wiserhub.py` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI/wiserhub.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 This API allows you to get information from and control your wiserhub.
 """
 
 # TODO: Keep objects and update instead of recreating on hub update
 # TODO: Update entity values after commend issued to get current values
 import asyncio
+from dataclasses import dataclass
 import aiohttp
 import pathlib
 from typing import Optional
 
 
 from . import _LOGGER, __VERSION__
 
@@ -231,14 +232,18 @@
         return False
 
     async def close_session(self):
         await self._wiser_rest_controller._session.close()
 
     # API properties
     @property
+    def api_parameters(self):
+        return self._wiser_rest_controller._api_parameters
+
+    @property
     def devices(self):
         """List of device entities attached to the Wiser Hub"""
         return self._devices
 
     @property
     def heating_channels(self):
         """List of heating channel entities on the Wiser Hub"""
```

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI.egg-info/PKG-INFO` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aioWiserHeatAPI
-Version: 1.3.1
+Version: 1.3.2
 Summary: An AsyncIO API for controlling the Drayton Wiser Heating system
 Home-page: https://github.com/msp1974/aioWiserHeatAPI
 Author: Mark Parker
 Author-email: msparker@sky.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Drayton Wiser Hub API Async v1.3.1
+# Drayton Wiser Hub API Async v1.3.2
 
 This repository contains a simple API which queries the Drayton Wiser Heating sysystem used in the UK.
 
 The API functionality provides the following functionality to control the wiser heating system for 1,2 and 3 channel heat hubs
 The API also supports Smart Plugs and initial basic functionality for Shutter and Lights
 
 ## Requirements
@@ -64,15 +64,22 @@
 
 ## 6. Documentation
 
 Documentation available in [info.md](https://github.com/msp1974/wiserHeatAPIv2/blob/master/docs/info.md) in the docs directory and within comments in the code
 
 ## Changelog
 
+### v1.3.2
+
+* Fixed issue ot maintaining some parameters after hub update
+* Improved handling of extra config json errors
+* Amended current_target_temp to use DisplayedSetPoint instead of CurrentSetPoint as this displays incorrectly in Eco mode
+
 ### 1.3.1
+
 * Away mode overrides passive mode functions
 
 ### 1.3.0
 
 * Rework passive mode functionality (may break previous code if using passive mode)
 
 ### 1.2.2
```

### Comparing `aioWiserHeatAPI-1.3.1/aioWiserHeatAPI.egg-info/SOURCES.txt` & `aioWiserHeatAPI-1.3.2/aioWiserHeatAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioWiserHeatAPI-1.3.1/setup.py` & `aioWiserHeatAPI-1.3.2/setup.py`

 * *Files identical despite different names*

