# Comparing `tmp/ariston-0.13.0.tar.gz` & `tmp/ariston-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ariston-0.13.0.tar", last modified: Wed Mar 29 19:56:52 2023, max compression
+gzip compressed data, was "ariston-0.13.1.tar", last modified: Fri Apr 14 17:56:55 2023, max compression
```

## Comparing `ariston-0.13.0.tar` & `ariston-0.13.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-03-29 19:56:41.895026 ariston-0.13.0/LICENSE
--rw-r--r--   0        0        0     3495 2023-03-29 19:56:41.895026 ariston-0.13.0/README.md
--rw-r--r--   0        0        0     5933 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/__init__.py
--rw-r--r--   0        0        0    23504 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/ariston_api.py
--rw-r--r--   0        0        0    13991 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/const.py
--rw-r--r--   0        0        0    12513 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/device.py
--rw-r--r--   0        0        0     3455 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/evo_device.py
--rw-r--r--   0        0        0     1090 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/evo_lydos_device.py
--rw-r--r--   0        0        0    30035 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/galevo_device.py
--rw-r--r--   0        0        0     1487 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/lux_device.py
--rw-r--r--   0        0        0     3172 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/lydos_hybrid_device.py
--rw-r--r--   0        0        0     9836 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/nuos_split_device.py
--rw-r--r--   0        0        0     7118 2023-03-29 19:56:41.895026 ariston-0.13.0/ariston/velis_device.py
--rw-r--r--   0        0        0      361 2023-03-29 19:56:41.895026 ariston-0.13.0/pyproject.toml
--rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 ariston-0.13.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-14 17:56:45.872999 ariston-0.13.1/LICENSE
+-rw-r--r--   0        0        0     3495 2023-04-14 17:56:45.872999 ariston-0.13.1/README.md
+-rw-r--r--   0        0        0     5933 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/__init__.py
+-rw-r--r--   0        0        0    23504 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/ariston_api.py
+-rw-r--r--   0        0        0    13991 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/const.py
+-rw-r--r--   0        0        0    12513 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/device.py
+-rw-r--r--   0        0        0     3766 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/evo_device.py
+-rw-r--r--   0        0        0     1090 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/evo_lydos_device.py
+-rw-r--r--   0        0        0    30516 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/galevo_device.py
+-rw-r--r--   0        0        0     1487 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/lux_device.py
+-rw-r--r--   0        0        0     3172 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/lydos_hybrid_device.py
+-rw-r--r--   0        0        0     9836 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/nuos_split_device.py
+-rw-r--r--   0        0        0     7118 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/velis_device.py
+-rw-r--r--   0        0        0      361 2023-04-14 17:56:45.872999 ariston-0.13.1/pyproject.toml
+-rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 ariston-0.13.1/PKG-INFO
```

### Comparing `ariston-0.13.0/LICENSE` & `ariston-0.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/README.md` & `ariston-0.13.1/README.md`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/ariston/__init__.py` & `ariston-0.13.1/ariston/__init__.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/ariston/ariston_api.py` & `ariston-0.13.1/ariston/ariston_api.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/ariston/const.py` & `ariston-0.13.1/ariston/const.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/ariston/device.py` & `ariston-0.13.1/ariston/device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/ariston/evo_device.py` & `ariston-0.13.1/ariston/evo_device.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Evo device class for Ariston module."""
 from __future__ import annotations
 
 import logging
+from datetime import datetime
 from typing import Optional
 
 from .const import (
     EvoPlantMode,
     EvoDeviceProperties,
     MedDeviceSettings,
     PlantData,
@@ -45,14 +46,22 @@
     def get_water_heater_eco_value(self) -> Optional[int]:
         """Get water heater eco value"""
         return self.data.get(EvoDeviceProperties.ECO, None)
 
     def get_rm_tm_value(self) -> Optional[str]:
         """Get remaining time value"""
         return self.data.get(EvoDeviceProperties.RM_TM, None)
+    
+    def get_rm_tm_in_minutes(self) -> int:
+        """Get remaining time value in minutes"""
+        rm_tm = self.get_rm_tm_value()
+        if rm_tm is None:
+            return -1
+        time = datetime.strptime(rm_tm, "%H:%M:%S")
+        return time.hour * 60 + time.minute
 
     def get_water_heater_maximum_setpoint_temperature_minimum(self) -> Optional[float]:
         """Get water heater maximum setpoint temperature minimum"""
         return self.plant_settings.get(
             MedDeviceSettings.MED_MAX_SETPOINT_TEMPERATURE_MIN, None
         )
```

### Comparing `ariston-0.13.0/ariston/evo_lydos_device.py` & `ariston-0.13.1/ariston/evo_lydos_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/ariston/galevo_device.py` & `ariston-0.13.1/ariston/galevo_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,14 +279,18 @@
     def get_ch_flow_temp_unit(self) -> str:
         """Get central heating flow temperature unit"""
         return self._get_item_by_id(DeviceProperties.CH_FLOW_TEMP, PropertyType.UNIT)
 
     def get_is_flame_on_value(self) -> bool:
         """Get is flame on value"""
         return self._get_item_by_id(DeviceProperties.IS_FLAME_ON, PropertyType.VALUE)
+        
+    def get_is_heating_pump_on_value(self) -> bool:                              
+        """Get is heating pump on value"""                                           
+        return self._get_item_by_id(DeviceProperties.IS_HEATING_PUMP_ON, PropertyType.VALUE)
 
     def get_holiday_mode_value(self) -> bool:
         """Get holiday mode on value"""
         return self._get_item_by_id(DeviceProperties.HOLIDAY, PropertyType.VALUE)
 
     def get_zone_mode(self, zone: int) -> ZoneMode:
         """Get zone mode on value"""
@@ -326,18 +330,22 @@
 
     def get_plant_mode_opt_texts(self) -> list[str]:
         """Get plant mode on option texts"""
         return self._get_item_by_id(DeviceProperties.PLANT_MODE, PropertyType.OPT_TEXTS)
 
     def get_plant_mode_text(self) -> str:
         """Get plant mode on option texts"""
-        index = self.get_plant_mode_options().index(self.get_plant_mode())
-        return self._get_item_by_id(
-            DeviceProperties.PLANT_MODE, PropertyType.OPT_TEXTS
-        )[index]
+        current_plant_mode = self.get_plant_mode().value
+        plant_mode_options = self.get_plant_mode_options()
+        if current_plant_mode in plant_mode_options:
+            index = plant_mode_options.index(current_plant_mode)
+            return self._get_item_by_id(
+                DeviceProperties.PLANT_MODE, PropertyType.OPT_TEXTS
+            )[index]
+        return PlantMode.UNDEFINED.name
 
     def get_measured_temp_unit(self, zone: int) -> str:
         """Get zone measured temp unit"""
         return self._get_item_by_id(
             ThermostatProperties.ZONE_MEASURED_TEMP, PropertyType.UNIT, zone
         )
```

### Comparing `ariston-0.13.0/ariston/lux_device.py` & `ariston-0.13.1/ariston/lux_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/ariston/lydos_hybrid_device.py` & `ariston-0.13.1/ariston/lydos_hybrid_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/ariston/nuos_split_device.py` & `ariston-0.13.1/ariston/nuos_split_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/ariston/velis_device.py` & `ariston-0.13.1/ariston/velis_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.0/PKG-INFO` & `ariston-0.13.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariston
-Version: 0.13.0
+Version: 0.13.1
 Summary: Ariston module
 Author-email: Tamás Füstös <fustom@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: requests
```

