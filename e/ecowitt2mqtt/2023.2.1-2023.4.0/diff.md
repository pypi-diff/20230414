# Comparing `tmp/ecowitt2mqtt-2023.2.1.tar.gz` & `tmp/ecowitt2mqtt-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecowitt2mqtt-2023.2.1.tar", max compression
+gzip compressed data, was "ecowitt2mqtt-2023.4.0.tar", max compression
```

## Comparing `ecowitt2mqtt-2023.2.1.tar` & `ecowitt2mqtt-2023.4.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0     1072 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/LICENSE
--rw-r--r--   0        0        0    31131 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/README.md
--rw-r--r--   0        0        0       39 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/__init__.py
--rw-r--r--   0        0        0    13841 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/__main__.py
--rw-r--r--   0        0        0       24 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/backports/__init__.py
--rw-r--r--   0        0        0     1735 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/backports/enum.py
--rw-r--r--   0        0        0    16656 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/config.py
--rw-r--r--   0        0        0    11058 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/const.py
--rw-r--r--   0        0        0     2308 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/core.py
--rw-r--r--   0        0        0    11872 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/data.py
--rw-r--r--   0        0        0      107 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/errors.py
--rw-r--r--   0        0        0       22 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/__init__.py
--rw-r--r--   0        0        0     6542 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/__init__.py
--rw-r--r--   0        0        0     4891 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/battery.py
--rw-r--r--   0        0        0     2301 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/humidity.py
--rw-r--r--   0        0        0     2438 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/illuminance.py
--rw-r--r--   0        0        0     1018 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/leak.py
--rw-r--r--   0        0        0     2013 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/lightning.py
--rw-r--r--   0        0        0      744 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/pollution.py
--rw-r--r--   0        0        0     2737 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/precipitation.py
--rw-r--r--   0        0        0     1364 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/pressure.py
--rw-r--r--   0        0        0    21443 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/temperature.py
--rw-r--r--   0        0        0     1333 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/time.py
--rw-r--r--   0        0        0     4610 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/uv.py
--rw-r--r--   0        0        0     9593 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/wind.py
--rw-r--r--   0        0        0     2167 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/config_validation.py
--rw-r--r--   0        0        0     1619 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/device.py
--rw-r--r--   0        0        0     1800 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/publisher/__init__.py
--rw-r--r--   0        0        0      716 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/publisher/factory.py
--rw-r--r--   0        0        0    18180 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/publisher/hass.py
--rw-r--r--   0        0        0     1114 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/publisher/topic.py
--rw-r--r--   0        0        0     4973 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/server.py
--rw-r--r--   0        0        0      348 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/typing.py
--rw-r--r--   0        0        0     7978 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/runtime.py
--rw-r--r--   0        0        0     1255 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/util/__init__.py
--rw-r--r--   0        0        0     7808 2023-02-24 15:46:12.643139 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/util/meteo.py
--rw-r--r--   0        0        0    13191 2023-02-24 15:46:12.647138 ecowitt2mqtt-2023.2.1/ecowitt2mqtt/util/unit_conversion.py
--rw-r--r--   0        0        0     4236 2023-02-24 15:46:12.647138 ecowitt2mqtt-2023.2.1/pyproject.toml
--rw-r--r--   0        0        0    33243 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.2.1/setup.py
--rw-r--r--   0        0        0    32767 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/LICENSE
+-rw-r--r--   0        0        0    31131 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/README.md
+-rw-r--r--   0        0        0       39 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/__init__.py
+-rw-r--r--   0        0        0    13841 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/__main__.py
+-rw-r--r--   0        0        0       24 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/backports/__init__.py
+-rw-r--r--   0        0        0     1735 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/backports/enum.py
+-rw-r--r--   0        0        0    16656 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/config.py
+-rw-r--r--   0        0        0    11058 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/const.py
+-rw-r--r--   0        0        0     2308 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/core.py
+-rw-r--r--   0        0        0    11872 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/data.py
+-rw-r--r--   0        0        0      107 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/errors.py
+-rw-r--r--   0        0        0       22 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/__init__.py
+-rw-r--r--   0        0        0     6598 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/__init__.py
+-rw-r--r--   0        0        0     4891 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/battery.py
+-rw-r--r--   0        0        0     2301 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/humidity.py
+-rw-r--r--   0        0        0     2438 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/illuminance.py
+-rw-r--r--   0        0        0     1018 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/leak.py
+-rw-r--r--   0        0        0     2013 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/lightning.py
+-rw-r--r--   0        0        0      744 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/pollution.py
+-rw-r--r--   0        0        0     2737 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/precipitation.py
+-rw-r--r--   0        0        0     1364 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/pressure.py
+-rw-r--r--   0        0        0    21443 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/temperature.py
+-rw-r--r--   0        0        0     1333 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/time.py
+-rw-r--r--   0        0        0     4610 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/uv.py
+-rw-r--r--   0        0        0     9593 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/wind.py
+-rw-r--r--   0        0        0     2167 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/config_validation.py
+-rw-r--r--   0        0        0     1619 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/device.py
+-rw-r--r--   0        0        0     1800 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/factory.py
+-rw-r--r--   0        0        0    18180 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/hass.py
+-rw-r--r--   0        0        0     1114 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/topic.py
+-rw-r--r--   0        0        0     4973 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/server.py
+-rw-r--r--   0        0        0      348 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/typing.py
+-rw-r--r--   0        0        0     7978 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/runtime.py
+-rw-r--r--   0        0        0     1255 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/__init__.py
+-rw-r--r--   0        0        0     7934 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/meteo.py
+-rw-r--r--   0        0        0    13191 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/unit_conversion.py
+-rw-r--r--   0        0        0     4041 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/pyproject.toml
+-rw-r--r--   0        0        0    32767 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.4.0/PKG-INFO
```

### Comparing `ecowitt2mqtt-2023.2.1/LICENSE` & `ecowitt2mqtt-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/README.md` & `ecowitt2mqtt-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/__main__.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/__main__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/backports/enum.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/backports/enum.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/config.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/config.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/const.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Define package constants."""
 import logging
 from typing import Final
 
 from ecowitt2mqtt.helpers.typing import UnitSystemType
 
-__version__ = "2023.02.1"
+__version__ = "2023.04.0"
 
 LOGGER = logging.getLogger(__package__)
 
 # Configuration keys:
 CONF_BATTERY_OVERRIDES: Final = "battery_override"
 CONF_CONFIG: Final = "config"
 CONF_DEFAULT_BATTERY_STRATEGY: Final = "default_battery_strategy"
```

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/core.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/core.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/data.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/data.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/__init__.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,24 +100,24 @@
             )
         ) is not None:
             return cast(str, override)
         if self._config.output_unit_system == UNIT_SYSTEM_IMPERIAL:
             return self.output_unit_imperial
         return self.output_unit_metric
 
-    def calculate_from_value(
+    def calculate_from_value(  # type: ignore[empty-body]
         self, value: PreCalculatedValueType
     ) -> CalculatedDataPoint:
         """Perform the calculation.
 
         Args:
             value: A pre-calculated value.
         """
 
-    def calculate_from_payload(
+    def calculate_from_payload(  # type: ignore[empty-body]
         self, payload: dict[str, PreCalculatedValueType]
     ) -> CalculatedDataPoint:
         """Perform the calculation.
 
         Args:
             payload: An Ecowitt data payload.
         """
```

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/battery.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/battery.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/humidity.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/humidity.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/illuminance.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/illuminance.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/leak.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/leak.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/lightning.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/lightning.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/pollution.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/pollution.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/precipitation.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/precipitation.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/pressure.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/pressure.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/temperature.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/temperature.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/time.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/time.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/uv.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/uv.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/calculator/wind.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/wind.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/config_validation.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/config_validation.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/device.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/device.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/publisher/__init__.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/publisher/factory.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/factory.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/publisher/hass.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/hass.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/publisher/topic.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/topic.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/helpers/server.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/server.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/runtime.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/runtime.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/util/__init__.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/util/meteo.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/meteo.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,37 +145,40 @@
         The index.
     """
     dew_point_obj = get_dew_point_meteocalc_object(
         temperature, relative_humidity, unit_system
     )
     temp_obj = get_temperature_meteocalc_object(temperature, unit_system)
 
-    return round(
-        temp_obj.c
-        + (
-            0.5555
-            * (
-                (
-                    6.11
-                    * math.exp(
-                        5417.7530
-                        * (
-                            (1 / 273.16)
-                            - (
-                                1
-                                / TemperatureConverter.convert(
-                                    dew_point_obj.c, TEMP_CELSIUS, TEMP_KELVIN
+    return cast(
+        int,
+        round(
+            temp_obj.c
+            + (
+                0.5555
+                * (
+                    (
+                        6.11
+                        * math.exp(
+                            5417.7530
+                            * (
+                                (1 / 273.16)
+                                - (
+                                    1
+                                    / TemperatureConverter.convert(
+                                        dew_point_obj.c, TEMP_CELSIUS, TEMP_KELVIN
+                                    )
                                 )
                             )
                         )
                     )
+                    - 10
                 )
-                - 10
             )
-        )
+        ),
     )
 
 
 def get_relative_strain_index(
     temperature: float, relative_humidity: float, unit_system: UnitSystemType
 ) -> float:
     """Get a simmer index meteocalc object.
```

### Comparing `ecowitt2mqtt-2023.2.1/ecowitt2mqtt/util/unit_conversion.py` & `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.2.1/pyproject.toml` & `ecowitt2mqtt-2023.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry]
 name = "ecowitt2mqtt"
-version = "2023.02.1"
+version = "2023.04.0"
 description = "A small web server to send data from Ecowitt devices to an MQTT Broker"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/ecowitt2mqtt"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -59,50 +59,42 @@
 ]
 
 [tool.poetry.dependencies]
 "ruamel.yaml" = "^0.17.21"
 aiohttp = "^3.8.1"
 asyncio-mqtt = ">=0.12.1"
 colorlog = "^6.6.0"
-fastapi = ">=0.89.1,<0.93.0"
+fastapi = ">=0.89.1,<0.96.0"
 meteocalc = "^1.1.0"
 python = "^3.9.0"
-python-multipart = "^0.0.5"
+python-multipart = ">=0.0.5,<0.0.7"
 rapidfuzz = "^2.13.0"
 uvicorn = ">=0.19.0"
 uvloop = "^0.17.0"
 voluptuous = "^0.13.1"
 
 [tool.poetry.group.dev.dependencies]
 aresponses = "^2.1.6"
 bandit = "^1.7.4"
-black = "^22.10.0"
+black = ">=22.10,<24.0"
 blacken-docs = "^1.12.1"
 codespell = "^2.2.2"
-coverage = {version = "^6.5", extras = ["toml"]}
+coverage = {version = ">=6.5,<8.0", extras = ["toml"]}
 darglint = "^1.8.1"
-flake8 = "^4.0.1"
-flake8-bandit = "^3.0.0"
-flake8-bugbear = "^22.10.27"
-flake8-builtins = "^2.0.0"
-flake8-comprehensions = "^3.10.0"
-flake8-docstrings = "^1.5.0"
-flake8-eradicate = "^1.4.0"
-flake8-markdown = "^0.3.0"
-flake8-simplify = "^0.19.3"
 isort = "^5.10.1"
-mypy = "^0.982"
-pre-commit = "^2.20.0"
+mypy = "^1.2.0"
+pre-commit = ">=2.20,<4.0"
 pre-commit-hooks = "^4.3.0"
 pylint = "^2.15.5"
 pytest = "^7.2.0"
 pytest-aiohttp = "^1.0.0"
-pytest-asyncio = "^0.20.1"
+pytest-asyncio = ">=0.20.1,<0.22.0"
 pytest-cov = "^4.0.0"
 pyupgrade = "^3.1.0"
+ruff = "^0.0.261"
 safety = "^2.3.1"
 typing-extensions = "^4.4.0"
 vulture = "^2.6"
 yamllint = "^1.28.0"
 
 [tool.poetry.scripts]
 ecowitt2mqtt = "ecowitt2mqtt.__main__:main"
```

### Comparing `ecowitt2mqtt-2023.2.1/setup.py` & `ecowitt2mqtt-2023.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,868 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ecowitt2mqtt
+Version: 2023.4.0
+Summary: A small web server to send data from Ecowitt devices to an MQTT Broker
+Home-page: https://github.com/bachya/ecowitt2mqtt
+License: MIT
+Author: Aaron Bach
+Author-email: bachya1208@gmail.com
+Requires-Python: >=3.9.0,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: asyncio-mqtt (>=0.12.1)
+Requires-Dist: colorlog (>=6.6.0,<7.0.0)
+Requires-Dist: fastapi (>=0.89.1,<0.96.0)
+Requires-Dist: meteocalc (>=1.1.0,<2.0.0)
+Requires-Dist: python-multipart (>=0.0.5,<0.0.7)
+Requires-Dist: rapidfuzz (>=2.13.0,<3.0.0)
+Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: uvicorn (>=0.19.0)
+Requires-Dist: uvloop (>=0.17.0,<0.18.0)
+Requires-Dist: voluptuous (>=0.13.1,<0.14.0)
+Project-URL: Bug Tracker, https://github.com/bachya/ecowitt2mqtt/issues
+Project-URL: Changelog, https://github.com/bachya/ecowitt2mqtt/releases
+Project-URL: Repository, https://github.com/bachya/ecowitt2mqtt
+Description-Content-Type: text/markdown
 
-packages = \
-['ecowitt2mqtt',
- 'ecowitt2mqtt.backports',
- 'ecowitt2mqtt.helpers',
- 'ecowitt2mqtt.helpers.calculator',
- 'ecowitt2mqtt.helpers.publisher',
- 'ecowitt2mqtt.util']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.8.1,<4.0.0',
- 'asyncio-mqtt>=0.12.1',
- 'colorlog>=6.6.0,<7.0.0',
- 'fastapi>=0.89.1,<0.93.0',
- 'meteocalc>=1.1.0,<2.0.0',
- 'python-multipart>=0.0.5,<0.0.6',
- 'rapidfuzz>=2.13.0,<3.0.0',
- 'ruamel.yaml>=0.17.21,<0.18.0',
- 'uvicorn>=0.19.0',
- 'uvloop>=0.17.0,<0.18.0',
- 'voluptuous>=0.13.1,<0.14.0']
-
-entry_points = \
-{'console_scripts': ['ecowitt2mqtt = ecowitt2mqtt.__main__:main']}
-
-setup_kwargs = {
-    'name': 'ecowitt2mqtt',
-    'version': '2023.2.1',
-    'description': 'A small web server to send data from Ecowitt devices to an MQTT Broker',
-    'long_description': '![ecowitt2mqtt][logo]\n\n[![CI][ci-badge]][ci]\n[![PyPI][pypi-badge]][pypi]\n[![Docker Hub][docker-hub-badge]][docker-hub]\n[![Version][version-badge]][version]\n[![License][license-badge]][license]\n[![Code Coverage][codecov-badge]][codecov]\n[![Maintainability][maintainability-badge]][maintainability]\n\n<a href="https://www.buymeacoffee.com/bachya1208P" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>\n\n`ecowitt2mqtt` is a small CLI/web server that can receive data from Fine Offset weather\nstations (and their numerous white-labeled counterparts, like Ecowitt and\nAmbient Weather), adjust that data in numerous ways, and send it on to one or more\nMQTT brokers.\n\n- [Installation](#installation)\n- [Python Versions](#python-versions)\n- [Disclaimer](#disclaimer)\n- [Supported Brands](#supported-brands)\n- [Quick Start](#quick-start)\n- [Configuration](#configuration)\n  - [Command Line Options](#command-line-options)\n  - [Environment Variables](#environment-variables)\n  - [Configuration File](#configuration-file)\n  - [Merging Configuration Options](#merging-configuration-options)\n  - [Input Data Formats](#input-data-formats)\n- [Advanced Usage](#advanced-usage)\n  - [Calculated Sensors](#calculated-sensors)\n  - [Battery Configurations](#battery-configurations)\n  - [Unit Systems](#unit-systems)\n  - [Raw Data](#raw-data)\n  - [Home Assistant](#home-assistant)\n  - [Running in the Background](#running-in-the-background)\n  - [Docker](#docker)\n- [Diagnostics](#diagnostics)\n- [Contributing](#contributing)\n\n# Installation\n\n```bash\npip install ecowitt2mqtt\n```\n\n# Python Versions\n\n`ecowitt2mqtt` is currently supported on:\n\n- Python 3.9\n- Python 3.10\n- Python 3.11\n\n# Disclaimer\n\nThe datapoints within this library and documentation constitute estimates and are\nintended to help informed decision making. They should not replace analysis, advice, or\ndiagnosis from trained professionals. Use this data at your own discretion.\n\n# Supported Brands\n\nDespite the name of the library, `ecowitt2mqtt` should support any weather station/gateway\nthat is produced by [Fine Offset](https://www.foshk.com/). This includes brands that\nwhite-label Fine Offset equipment, such as:\n\n- [Ambient Weather][ambient-weather] (U.S.)\n- [Ecowitt][ecowitt] (China, Hong Kong)\n- [Froggit][froggit] (Germany)\n\n...and many others. For more information on how these brands relate to one another, see\nthis forum post: https://www.wxforum.net/index.php?topic=40730.0\n\nAlthough there are some small differences between how these various branded devices are\nconfigured, `ecowitt2mqtt` endeavors to incorporate them all with minimal effort on the\nuser\'s part.\n\n# Quick Start\n\nFirst, install `ecowitt2mqtt` via `pip`:\n\n```bash\n$ pip install ecowitt2mqtt\n```\n\nNext, if you haven\'t already, install the appropriate mobile app to configure your\ndevice. For example:\n\n- Ambient Weather: awnet ([iOS][awnet-ios]/[Android][awnet-google-play])\n- Ecowitt: WS View ([iOS][ws-view-ios]/[Android][ws-view-google-play])\n\nFind the appropriate location in the mobile app to configure a customized upload target\nfor the station\'s data. This will differ depending on the app, but in general, you\nshould select your device and find a screen entitled "Upload" (or similar).\n\n![The "Upload" screen in the awnet app][awnet-upload-screen]\n![The "Upload" screen in the WS View app][ws-view-upload-screen]\n\nFill out the form with the appropriate values and tap `Save`:\n\n- `Protocol Type Same As`: pick the label that matches your brand (e.g., `Ecowitt` for\n  Ecowitt devices)\n- `Server IP / Hostname`: the IP address/hostname of the device running `ecowitt2mqtt`\n- `Path`: `/data/report/` (the default path used by most mobile apps)\n- `Port`: `8080` (the default port on which `ecowitt2mqtt` is served)\n- `Upload Interval`: 16 (a reasonable short number of seconds between publishes)\n\nThen, on the machine where you installed `ecowitt2mqtt`, run it:\n\n```bash\n$ ecowitt2mqtt \\\n    --mqtt-broker=192.168.1.101 \\\n    --mqtt-username=user \\\n    --mqtt-password=password \\\n    --mqtt-topic=ecowitt2mqtt/device_1\n    --input-data-format=ecowitt\n```\n\nWithin the `Upload Interval`, data should begin to appear in the MQTT broker.\n\n# Configuration\n\n`ecowitt2mqtt` can be configured via command line options, environment variables, or a\n(YAML or JSON) config file.\n\n## Command Line Options\n\n```\nusage: ecowitt2mqtt [-h] [--version]\n                    [--battery-override BATTERY_OVERRIDE] [-c config]\n                    [--default-battery-strategy default_battery_strategy]\n                    [--diagnostics] [--disable-calculated-data]\n                    [-e endpoint] [--hass-discovery]\n                    [--hass-discovery-prefix hass_discovery_prefix]\n                    [--hass-entity-id-prefix hass_entity_id_prefix]\n                    [--input-data-format input_data_format]\n                    [--input-unit-system input_unit_system]\n                    [-b mqtt_broker] [-p mqtt_password]\n                    [--mqtt-port mqtt_port] [--mqtt-retain]\n                    [--mqtt-tls] [-t mqtt_topic] [-u mqtt_username]\n                    [--output-unit-system output_unit_system]\n                    [--output-unit-accumulated-precipitation output_unit_accumulated_precipitation]\n                    [--output-unit-distance output_unit_distance]\n                    [--output-unit-humidity output_unit_humidity]\n                    [--output-unit-illuminance output_unit_illuminance]\n                    [--output-unit-precipitation-rate output_unit_precipitation_rate]\n                    [--output-unit-pressure output_unit_pressure]\n                    [--output-unit-speed output_unit_speed]\n                    [--output-unit-temperature output_unit_temperature]\n                    [--port port] [--precision precision] [--raw-data]\n                    [-v]\n\nSend data from an Ecowitt gateway to an MQTT broker\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --version             show program\'s version number and exit\n  --battery-override BATTERY_OVERRIDE\n                        A battery configuration override (format:\n                        key,value)\n  -c config, --config config\n                        A path to a YAML or JSON config file\n  --default-battery-strategy default_battery_strategy\n                        The default battery config strategy to use\n                        (default: boolean)\n  --diagnostics         Output diagnostics\n  --disable-calculated-data\n                        Disable the output of calculated sensors\n  -e endpoint, --endpoint endpoint\n                        The relative endpoint/path to serve\n                        ecowitt2mqtt on (default: /data/report)\n  --hass-discovery      Publish data in the Home Assistant MQTT\n                        Discovery format\n  --hass-discovery-prefix hass_discovery_prefix\n                        The Home Assistant MQTT Discovery topic prefix\n                        to use (default: homeassistant)\n  --hass-entity-id-prefix hass_entity_id_prefix\n                        The prefix to use for Home Assistant entity IDs\n  --input-data-format input_data_format\n                        The input data format used by the gateway\n                        (default: ecowitt)\n  --input-unit-system input_unit_system\n                        The input unit system used by the gateway\n                        (default: imperial)\n  -b mqtt_broker, --mqtt-broker mqtt_broker\n                        The hostname or IP address of an MQTT broker\n  -p mqtt_password, --mqtt-password mqtt_password\n                        A valid password for the MQTT broker\n  --mqtt-port mqtt_port\n                        The listenting port of the MQTT broker\n                        (default: 1883)\n  --mqtt-retain         Instruct the MQTT broker to retain messages\n  --mqtt-tls            Enable MQTT over TLS\n  -t mqtt_topic, --mqtt-topic mqtt_topic\n                        The MQTT topic to publish device data to\n  -u mqtt_username, --mqtt-username mqtt_username\n                        A valid username for the MQTT broker\n  --output-unit-system output_unit_system\n                        The output unit system used by the gateway\n                        (default: imperial)\n  --output-unit-accumulated-precipitation output_unit_accumulated_precipitation\n                        The output unit to use for accumulated\n                        precipitation data points (default: the default\n                        used by the output unit system)\n  --output-unit-distance output_unit_distance\n                        The output unit to use for distance data points\n                        (default: the default used by the output unit\n                        system)\n  --output-unit-humidity output_unit_humidity\n                        The output unit to use for humidity data points\n                        (default: the default used by the output unit\n                        system)\n  --output-unit-illuminance output_unit_illuminance\n                        The output unit to use for illuminance data\n                        points (default: the default used by the output\n                        unit system)\n  --output-unit-precipitation-rate output_unit_precipitation_rate\n                        The output unit to use for precipitation rate\n                        data points (default: the default used by the\n                        output unit system)\n  --output-unit-pressure output_unit_pressure\n                        The output unit to use for pressure data points\n                        (default: the default used by the output unit\n                        system)\n  --output-unit-speed output_unit_speed\n                        The output unit to use for speed data points\n                        (default: the default used by the output unit\n                        system)\n  --output-unit-temperature output_unit_temperature\n                        The output unit to use for temperature data\n                        points (default: the default used by the output\n                        unit system)\n  --port port           The port to serve ecowitt2mqtt on (default:\n                        8080)\n  --precision precision\n                        The precision to output data points at\n                        (default: no limit)\n  --raw-data            Return raw data (don\'t attempt to translate any\n                        values)\n  -v, --verbose         Increase verbosity of logged output\n```\n\n## Environment Variables\n\n- `ECOWITT2MQTT_BATTERY_OVERRIDE`: a semicolon-delimited list of key=value battery\n  overrides (default: `numeric`)\n- `ECOWITT2MQTT_CONFIG`: a path to a YAML or JSON config file (default: `None`)\n- `ECOWITT2MQTT_DEFAULT_BATTERY_STRATEGY`: the default battery config strategy to use\n  (default: `boolean`)\n- `ECOWITT2MQTT_DIAGNOSTICS`: whether to output diagnostics (default: `false`)\n- `ECOWITT2MQTT_DISABLE_CALCULATED_DATA`: whether to disable the output of calculated\n  sensors (default: `false`)\n- `ECOWITT2MQTT_ENDPOINT`: the relative endpoint/path to serve ecowitt2mqtt on (default:\n  `/data/report`)\n- `ECOWITT2MQTT_HASS_DISCOVERY_PREFIX`: the Home Assistant discovery prefix to use\n  (default: `homeassistant`)\n- `ECOWITT2MQTT_HASS_DISCOVERY`: publish data in the Home Assistant MQTT Discovery format\n  (default: `false`)\n- `ECOWITT2MQTT_HASS_ENTITY_ID_PREFIX`: the prefix to use for Home Assistant entity IDs\n  (default: `""`)\n- `ECOWITT2MQTT_INPUT_DATA_FORMAT`: the input data format used by the gateway (default:\n  `ecowitt`)\n- `ECOWITT2MQTT_INPUT_UNIT_SYSTEM`: the input unit system used by the device (default:\n  `imperial`)\n- `ECOWITT2MQTT_MQTT_BROKER`: the hostname or IP address of an MQTT broker\n- `ECOWITT2MQTT_MQTT_PASSWORD`: a valid password for the MQTT broker\n- `ECOWITT2MQTT_MQTT_PORT`: the listenting port of the MQTT broker (default: `1883`)\n- `ECOWITT2MQTT_MQTT_RETAIN`: whether to instruct the MQTT broker to retain messages\n  (default: `false`)\n- `ECOWITT2MQTT_MQTT_TLS`: publish data via MQTT over TLS (default: `false`)\n- `ECOWITT2MQTT_MQTT_TOPIC`: the MQTT topic to publish device data to\n- `ECOWITT2MQTT_MQTT_USERNAME`: a valid username for the MQTT broker\n- `ECOWITT2MQTT_OUTPUT_UNIT_SYSTEM`: the unit system to use in output (default: `imperial`)\n- `ECOWITT2MQTT_OUTPUT_UNIT_TEMPERATURE`: the output unit to use for temperature data\n  points (default: the default used by the output unit system)\n- `ECOWITT2MQTT_PORT`: the port to serve ecowitt2mqtt on (default: `8080`)\n- `ECOWITT2MQTT_PRECISION`: the precision to output data points at (default: no limit)\n- `ECOWITT2MQTT_RAW_DATA`: return raw data (don\'t attempt to translate any values)\n  (default: `false`)\n- `ECOWITT2MQTT_VERBOSE`: increase verbosity of logged output (default: `false`)\n\n## Configuration File\n\nThe configuration file can be formatted as either YAML:\n\n```yaml\n---\nbattery_override:\n  battery_key1: boolean\ndefault_battery_strategy: numeric\ndiagnostics: false\ndisable_calculated_data: false\nendpoint: /data/report\nhass_discovery: false\nhass_discovery_prefix: homeassistant\nhass_entity_id_prefix: test_prefix\ninput_data_format: ecowitt\ninput_unit_system: imperial\nmqtt_broker: 127.0.0.1\nmqtt_password: password\nmqtt_port: 1883\nmqtt_retain: false\nmqtt_tls: false\nmqtt_topic: Test\nmqtt_username: user\noutput_unit_system: imperial\nport: 8080\nraw_data: false\nverbose: false\n```\n\n...or JSON\n\n```json\n{\n  "battery_override": {\n    "battery_key1": "boolean"\n  },\n  "default_battery_strategy": "numeric",\n  "diagnostics": false,\n  "disable_calculated_data": false,\n  "endpoint": "/data/report",\n  "hass_discovery": false,\n  "hass_discovery_prefix": "homeassistant",\n  "hass_entity_id_prefix": "test_prefix"\n  "input_data_format": "ecowitt",\n  "input_unit_system": "imperial",\n  "mqtt_broker": "127.0.0.1",\n  "mqtt_password": "password",\n  "mqtt_port": 1883,\n  "mqtt_retain": true,\n  "mqtt_tls": false,\n  "mqtt_topic": "Test",\n  "mqtt_username": "user",\n  "output_unit_system": "imperial",\n  "port": 8080,\n  "raw_data": false,\n  "verbose": false\n}\n```\n\n...and makes use of the same config options available to the CLI.\n\n### Multiple Gateways\n\nWhen using the configuration file, it is possible to define specific configuration\nparameters for multiple Ecowitt gateways. This is useful if different gateways should\npublish to different MQTT brokers, in different formats, etc.\n\nFirst, you must determine the unique ID for each gateway. This can be observed in the\nlogs when `verbose` is enabled – look for the `PASSKEY` value that the gateway has:\n\n```\nReceived data from the Ecowitt device: {\'PASSKEY\': \'abcde12345\', ...}\n```\n\nThen, in the configuration file, simply add a `gateways` key that contains a mapping of\nany of the existing configuration options (except for `--verbose` and `--diagnostics`,\nwhich can only be defined once and are applied to _every_ configuration). Options that\nremain at the root level of the file are treated as defaults.\n\nFor example, this YAML configuration file:\n\n```yaml\n---\nmqtt_broker: 127.0.0.1\nmqtt_password: password\nmqtt_topic: Test\nmqtt_username: user\n\ngateways:\n  abcde12345:\n    hass_discovery: true\n```\n\n...defines two gateway definitions:\n\n- One that publishes to the `Test` topic on an MQTT broker at `127.0.0.1`\n- One (with a `PASSKEY` of `abcde12345`) that publishes to the same broker, but in Home\n  Assistant MQTT Discovery format.\n\nIn another example, this JSON configuration file:\n\n```json\n{\n  "mqtt_broker": "127.0.0.1",\n  "mqtt_password": "password",\n  "mqtt_port": 1883,\n  "mqtt_topic": "Test",\n  "mqtt_username": "user",\n  "gateways": {\n    "abcde12345": {\n      "mqtt_broker": "192.168.1.100",\n      "mqtt_retain": true,\n      "output_unit_system": "metric"\n    }\n  }\n}\n```\n\n...defines two gateway definitions:\n\n- One that publishes to the `Test` topic on an MQTT broker at `127.0.0.1`\n- One (with a `PASSKEY` of `abcde12345`) that publishes to a different broker\n  (`192.168.1.100`), outputs the data in metric, and retains the data on the broker\n\n## Merging Configuration Options\n\nWhen parsing configuration options, `ecowitt2mqtt` looks at the configuration sources in\nthe following order:\n\n1. Configuration File (Specific Gateway)\n2. Configuration File (Defaults)\n3. Environment Variables\n4. CLI Options\n\nThis allows you to mix and match sources – for instance, you might have "defaults" in\nthe configuration file and override them via environment variables.\n\n## Input Data Formats\n\n`ecowitt2mqtt` currently supports the following input data formats:\n\n- `ambient_weather`\n- `ecowitt`\n\nProvide the correct one to `---input-data-format` based on which device brand you use.\n\n# Advanced Usage\n\n## Calculated Sensors\n\nIn addition to the data coming from a gateway, `ecowitt2mqtt` will automatically deduce\nand published several additional, calculated data points if the requisite underlying\ndata exists:\n\n- **[Absolute Humidity][absolute-humidity]:** the actual volume of water vapor in the\n  air\n- **[Beaufort Scale][beaufort-scale]:** the empirical measure that relates wind speed to\n  observed conditions at sea or on land\n- **[Dew Point][dew-point]:** the temperature to which air must be cooled to become\n  saturated with water vapor, assuming constant air pressure and water content\n- **[Feels Like][heat-index]:** how hot or how cold the air feels to the human body when\n  factoring in variables such as relative humidity, wind speeds, the amount of sunshine,\n  etc.\n- **[Frost Point][frost-point]:** the temperature below 32°F (0°C) at which moisture in\n  the air will condense as a layer of frost on exposed surfaces that are also at a\n  temperature below the frost point\n- **[Frost Risk][frost-point]:** how likely the formation of frost is (based on the\n  `frostpoint`)\n- **[Heat Index][heat-index]:** how hot the air feels to the human body when factoring\n  in relative humidity (applicable when the apparent temperature is higher than the air\n  temperature)\n- **[Humidex][humidex]:** an index number used by Canadian meteorologists to describe\n  how hot the weather feels to the average person, by combining the effect of heat and\n  humidity\n- **[Humidex Perception][humidex]:** a human-friendly interpretation of the Humidex\n- **Relative Strain Index:** a measure of discomfort resulting from the combined effect\n  of temperature and humidity (applicable to heat stress of manual workers under shelter\n  at various metabolic rates)\n- **Relative Strain Index Perception:** a human-friendly interpretation of the Relative\n  Strain Index\n- **[Safe Exposure Times][safe-exposure-times]:** how long different skin types can be\n  in the sun (unprotected) before burning begins according to the\n  [Fitzpatrick Scale][fitzpatrick-scale]\n- **Solar Radiation (%):** the percentage of detected solar radiation illuminance as\n  perceived by the human eye\n- **[Simmer Index][simmer-index]:** an alternative to heat index that describes how how\n  the air feels to the human body in relatively dry environments\n- **[Simmer Zone][simmer-index]:** a human-friendly interpretation of the Simmer Index\n- **[Thermal Perception][dew-point]:** a human-friendly interpretation of the Dew Point\n- **[Wind Chill][wind-chill]:** how cold the air feels to the human body when factoring\n  in relative humidity, wind speed, etc. (applicable when the apparent temperature is\n  lower than the air temperature)\n\n(Special thanks to the excellent [`thermal_comfort` library][thermal-comfort-library] for\ninspiration on many of these.)\n\nIf you would prefer to not have these sensors calculated and published, you can utilize\nthe `--disable-calculated-data` configuration option.\n\n## Battery Configurations\n\nEcowitt devices report battery levels in three different formats:\n\n- `boolean`: `0` represents `OFF` (i.e., the battery is in normal condition) and `1` represents\n  `ON` (i.e., the battery is low).\n- `numeric`: the raw numeric value is interpreted as the number of volts remaining in the\n  battery.\n- `percentage`: the raw numeric value is interpreted as the percentage of voltage\n  remaining the battery.\n\n`ecowitt2mqtt` provides three mechanisms to handle this complexity:\n\n1. A built-in mapping of all currently known battery types to their assumed strategy\n2. A default battery strategy for unknown battery types\n3. User-defined battery strategy overrides\n\n### Built-in Mapping\n\n`ecowitt2mqtt` contains an internal mapping that should automatically transform all\nknown battery types into their correct format.\n\n### Default Battery Strategy\n\nBy using the `--default-battery-strategy` configuration parameter, users can specify how\nunknown battery types should be treated by default.\n\n### Battery Overrides\n\nIndividual batteries can be overridden and given a new strategy. How this is\naccomplished differs slightly based on the configuration method used:\n\n- Command Line Options: provide one or more `--battery-override "batt1=boolean"` options\n- Environment Variables: provide a `ECOWITT2MQTT_BATTERY_OVERRIDE` variable that is a\n  semicolon-delimited pair of "key=value" strings (e.g.,\n  `ECOWITT2MQTT_BATTERY_OVERRIDE="batt1=boolean;batt2=numeric"`)\n- Config File: include a dictionary of key/value pairs in either YAML or JSON format\n\nThese overrides work on both known and unknown battery types; that said, if you should\nfind the need to override a known battery type because `ecowitt2mqtt` has an incorrect\ninternal interpretation, submit an issue to get it corrected!\n\n### Example\n\nIn this example, a user mostly has batteries that should be treated as `boolean`, but\nalso has one – `wh60_batt1` – that should be treated as numeric.\n\n#### Command Line Options\n\n```\n$ ecowitt2mqtt --default-battery-strategy boolean --battery-override="wh60_batt1=numeric"\n```\n\n#### Environment Variables\n\n```\n$ ECOWITT2MQTT_DEFAULT_BATTERY_STRATEGY=boolean \\\n  ECOWITT2MQTT_BATTERY_OVERRIDE="wh60_batt1=numeric" \\\n  ecowitt2mqtt\n```\n\n#### Config File\n\nIn YAML:\n\n```yaml\n---\ndefault_battery_strategy: boolean\nbattery_override:\n  wh60_batt1: numeric\n```\n\n...or JSON\n\n```json\n{\n  "default_battery_strategy": "boolean",\n  "battery_override": {\n    "wh60_batt1": "numeric"\n  }\n}\n```\n\n## Unit Systems\n\n### Input and Output\n\n`ecowitt2mqtt` allows you to specify both the input and output unit systems for a device\nvia the `--input-unit-system` and `--output-unit-system` config options, respectively.\nThese are fairly self-explanatory, but take care to use an `--input-unit-system` that is\nconsistent with what your device provides (otherwise, your data will be very "off").\n\n### Overriding Units for Data Categories\n\nIf you wish, you can change the unit for individual data categories. For example, let\'s\nsay you wanted to use metric for the output unit system, but wanted to represent all\ntemperature data points in Kelvin – you would provide `--output-unit-system=metric` and\n`--output-unit-temperature=K` as config options. As expected, the value is properly\nconverted to the new unit.\n\n#### Accumulated Precipitation\n\nConfig Option: `--output-unit-accumulated-precipitation`\n\n- `in`\n- `mm`\n\n#### Absolute Humidity\n\nConfig Option: `--output-unit-humidity`\n\n- `g/m³`\n- `lbs/ft³`\n\n#### Illuminance\n\nConfig Option: `--output-unit-illuminance`\n\n- `fc`\n- `kfc`\n- `klx`\n- `lx`\n- `W/m²`\n\n#### Precipitation Rate\n\nConfig Option: `--output-unit-precipitation-rate`\n\n- `in/h`\n- `mm/h`\n\n#### Pressure\n\nConfig Option: `--output-unit-pressure`\n\n- `bar`\n- `cbar`\n- `hPa`\n- `inHg`\n- `kPa`\n- `mbar`\n- `mmHg`\n- `Pa`\n- `psi`\n\n#### Speed\n\nConfig Option: `--output-unit-speed`\n\n- `ft/s`\n- `in/d`\n- `in/h`\n- `km/h`\n- `kn`\n- `m/s`\n- `mph`\n- `mm/d`\n\n#### Temperature\n\nConfig Option: `--output-unit-temperature`\n\n- `°C`\n- `°F`\n- `K`\n\n## Raw Data\n\nIn some cases, it may be preferable to prevent `ecowitt2mqtt` from doing any data\ntranslation (converting values to a new unit system, changing binary values – such as\nmight be used by a battery – into "friendly" values, etc.). Passing the `--raw-data` flag\nwill accomplish this: data will flow directly from the Ecowitt device to the MQTT broker\nas-is.\n\nNote that the `--raw-data` flag supersedes any that might cause data translation (such as\n`--input-unit-system` or `--output-unit-system`).\n\n## Home Assistant\n\n### MQTT Discovery\n\n[Home Assistant][home-assistant] users can quickly add entities from an Ecowitt device\nby using [MQTT Discovery][home-assistant-mqtt-discovery]. Once Home Assistant is\nconfigured to accept MQTT Discovery, `ecowitt2mqtt` simply needs the `--hass-discovery`\nflag:\n\n```bash\n$ ecowitt2mqtt \\\n    --mqtt-broker=192.168.1.101 \\\n    --mqtt-username=user \\\n    --mqtt-password=password \\\n    --hass-discovery\n```\n\n### Custom Entity ID Prefix\n\nYou can provide a custom prefix for all Home Assistant entities via the\n`--hass-entity-id-prefix` config parameter.\n\n### Home Assistant OS Add-on\n\nHome Assistant OS users can install the official `ecowitt2mqtt` add-on by clicking the\nlink below:\n\n[![Home Assistant Add-on][home-assistant-addon-badge]][home-assistant-addon]\n\n## Running in the Background\n\n`ecowitt2mqtt` doesn\'t, itself, provide any sort of daemonization mechanism. The suggested\nroute is to use a different application.\n\n### `supervisord`\n\nAn example `supervisord` configuration file might look like this:\n\n```\n[supervisord]\nnodaemon=true\nloglevel=info\nuser=root\n\n[program:ecowitt2mqtt]\ncommand=ecowitt2mqtt --mqtt-broker=192.168.1.101 --mqtt-username=user --mqtt-password=password\nstdout_logfile=/dev/stdout\nstdout_logfile_maxbytes=0\nredirect_stderr=true\n```\n\n### `systemd`\n\nAn example `systemd` service file in `/etc/systemd/system` might look like this:\n\n```\n[Unit]\nDescription=ECOWITT2MQTT daemon\nAfter=network.target\n\n[Service]\nType=simple\nExecStart=ecowitt2mqtt --mqtt-broker=192.168.1.101 --mqtt-username=user --mqtt-password=password\nExecReload=kill -HUP $MAINPID\nKillMode=process\nRestart=on-failure\nRestartSec=5s\n\n[Install]\nWantedBy=multi-user.target\n```\n\nTo enable the service:\n\n```bash\n$ systemctl enable ecowitt2mqtt\n```\n\n## Docker\n\nThe library is available via a Docker image from both [Docker Hub][docker-hub] and\n[ghcr.io][ghcr]. It is configured by using the same environment variables listed\n[above](#environment-variables).\n\nRunning the image is straightforward:\n\n```\ndocker run -it \\\n    -e ECOWITT2MQTT_MQTT_BROKER=192.168.1.101 \\\n    -e ECOWITT2MQTT_MQTT_USERNAME=user \\\n    -e ECOWITT2MQTT_MQTT_PASSWORD=password \\\n    -p 8080:8080 \\\n    bachya/ecowitt2mqtt:latest\n```\n\nNote the value of the `-p` flag: you must expose the port defined by the `PORT`\nenvironment variable. In the example above, the default port (`8080`) is used and is\nexposed via the same port on the host.\n\n[`docker-compose`][docker-compose] users can find an example configuration file at\n[`docker-compose.dev.yml`](docker-compose.dev.yml). Note that this is intended to be a dev\nenvironment for quickly testing the repo itself; in production, you should refer to one\nof the published images.\n\n# Diagnostics\n\nYou may run `ecowitt2mqtt` in diagnostics mode by providing the `--diagnostics` flag. In\nthis mode, the app will wait until it receives and publishes a single payload, then\nexit. This allows users to collect a small-but-complete payload for use in testing,\ndebugging, and issue reporting.\n\n# Contributing\n\nThanks to all of [our contributors][contributors] so far!\n\n1. [Check for open features/bugs][issues] or [initiate a discussion on one][new-issue].\n2. [Fork the repository][fork].\n3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`\n4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`\n5. Install the dev environment: `script/setup`\n6. Code your new feature or bug fix on a new branch.\n7. Write tests that cover your new functionality.\n8. Run tests and ensure 100% code coverage: `poetry run pytest --cov ecowitt2mqtt tests`\n9. Update `README.md` with any new documentation.\n10. Submit a pull request!\n\n[absolute-humidity]: https://en.wikipedia.org/wiki/Humidity#Absolute_humidity\n[ambient-weather]: https://ambientweather.com/\n[awnet-google-play]: https://play.google.com/store/apps/details?id=com.dtston.ambienttoolplus&hl=en_US&gl=US\n[awnet-ios]: https://apps.apple.com/us/app/awnet/id1341994564\n[awnet-upload-screen]: resources/awnet-upload-screen.jpeg?raw=true\n[beaufort-scale]: https://en.wikipedia.org/wiki/Beaufort_scale\n[ci-badge]: https://github.com/bachya/ecowitt2mqtt/workflows/CI/badge.svg\n[ci]: https://github.com/bachya/ecowitt2mqtt/actions\n[codecov-badge]: https://codecov.io/gh/bachya/ecowitt2mqtt/branch/dev/graph/badge.svg\n[codecov]: https://codecov.io/gh/bachya/ecowitt2mqtt\n[coffee-image]: https://cdn.buymeacoffee.com/buttons/default-orange.png\n[coffee]: https://www.buymeacoffee.com/bachya1208P\n[contributors]: https://github.com/bachya/ecowitt2mqtt/graphs/contributors\n[dew-point]: https://en.wikipedia.org/wiki/Dew_point\n[docker-compose]: https://docs.docker.com/compose/\n[docker-hub-badge]: https://img.shields.io/docker/pulls/bachya/ecowitt2mqtt\n[docker-hub]: https://hub.docker.com/r/bachya/ecowitt2mqtt\n[ecowitt]: https://www.ecowitt.com/\n[fitzpatrick-scale]: https://en.wikipedia.org/wiki/Fitzpatrick_scale\n[fork]: https://github.com/bachya/ecowitt2mqtt/fork\n[froggit]: https://www.froggit.de/Weather-Station/\n[frost-point]: https://en.wikipedia.org/wiki/Dew_point#Frost_point\n[ghcr]: https://ghcr.io/bachya/ecowitt2mqtt\n[heat-index]: https://en.wikipedia.org/wiki/Heat_index\n[home-assistant-addon-badge]: https://my.home-assistant.io/badges/supervisor_addon.svg\n[home-assistant-addon]: https://my.home-assistant.io/redirect/supervisor_addon/?addon=c35f0383_ecowitt2mqtt&repository_url=https%3A%2F%2Fgithub.com%2Fbachya%2Fhome-assistant-addons\n[home-assistant-mqtt-discovery]: https://www.home-assistant.io/docs/mqtt/discovery/\n[home-assistant]: https://home-assistant.io\n[humidex]: https://en.wikipedia.org/wiki/Humidex\n[issues]: https://github.com/bachya/ecowitt2mqtt/issues\n[license-badge]: https://img.shields.io/pypi/l/ecowitt2mqtt.svg\n[license]: https://github.com/bachya/ecowitt2mqtt/blob/main/LICENSE\n[logo]: resources/logo-full.png\n[maintainability-badge]: https://api.codeclimate.com/v1/badges/a03c9e96f19a3dc37f98/maintainability\n[maintainability]: https://codeclimate.com/github/bachya/ecowitt2mqtt/maintainability\n[new-issue]: https://github.com/bachya/ecowitt2mqtt/issues/new\n[pypi-badge]: https://img.shields.io/pypi/v/ecowitt2mqtt.svg\n[pypi]: https://pypi.python.org/pypi/ecowitt2mqtt\n[safe-exposure-times]: https://www.openuv.io/kb/skin-types-safe-exposure-time-calculation/\n[simmer-index]: http://summersimmer.com/ssi_page2.htm\n[thermal-comfort-library]: https://github.com/dolezsa/thermal_comfort\n[version-badge]: https://img.shields.io/pypi/pyversions/ecowitt2mqtt.svg\n[version]: https://pypi.python.org/pypi/ecowitt2mqtt\n[wind-chill]: https://en.wikipedia.org/wiki/Wind_chill\n[ws-view-google-play]: https://play.google.com/store/apps/details?id=com.ost.wsview&gl=US\n[ws-view-ios]: https://apps.apple.com/us/app/ws-view/id1362944193\n[ws-view-upload-screen]: resources/ws-view-upload-screen.jpeg?raw=true\n',
-    'author': 'Aaron Bach',
-    'author_email': 'bachya1208@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/bachya/ecowitt2mqtt',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9.0,<4.0.0',
+![ecowitt2mqtt][logo]
+
+[![CI][ci-badge]][ci]
+[![PyPI][pypi-badge]][pypi]
+[![Docker Hub][docker-hub-badge]][docker-hub]
+[![Version][version-badge]][version]
+[![License][license-badge]][license]
+[![Code Coverage][codecov-badge]][codecov]
+[![Maintainability][maintainability-badge]][maintainability]
+
+<a href="https://www.buymeacoffee.com/bachya1208P" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+
+`ecowitt2mqtt` is a small CLI/web server that can receive data from Fine Offset weather
+stations (and their numerous white-labeled counterparts, like Ecowitt and
+Ambient Weather), adjust that data in numerous ways, and send it on to one or more
+MQTT brokers.
+
+- [Installation](#installation)
+- [Python Versions](#python-versions)
+- [Disclaimer](#disclaimer)
+- [Supported Brands](#supported-brands)
+- [Quick Start](#quick-start)
+- [Configuration](#configuration)
+  - [Command Line Options](#command-line-options)
+  - [Environment Variables](#environment-variables)
+  - [Configuration File](#configuration-file)
+  - [Merging Configuration Options](#merging-configuration-options)
+  - [Input Data Formats](#input-data-formats)
+- [Advanced Usage](#advanced-usage)
+  - [Calculated Sensors](#calculated-sensors)
+  - [Battery Configurations](#battery-configurations)
+  - [Unit Systems](#unit-systems)
+  - [Raw Data](#raw-data)
+  - [Home Assistant](#home-assistant)
+  - [Running in the Background](#running-in-the-background)
+  - [Docker](#docker)
+- [Diagnostics](#diagnostics)
+- [Contributing](#contributing)
+
+# Installation
+
+```bash
+pip install ecowitt2mqtt
+```
+
+# Python Versions
+
+`ecowitt2mqtt` is currently supported on:
+
+- Python 3.9
+- Python 3.10
+- Python 3.11
+
+# Disclaimer
+
+The datapoints within this library and documentation constitute estimates and are
+intended to help informed decision making. They should not replace analysis, advice, or
+diagnosis from trained professionals. Use this data at your own discretion.
+
+# Supported Brands
+
+Despite the name of the library, `ecowitt2mqtt` should support any weather station/gateway
+that is produced by [Fine Offset](https://www.foshk.com/). This includes brands that
+white-label Fine Offset equipment, such as:
+
+- [Ambient Weather][ambient-weather] (U.S.)
+- [Ecowitt][ecowitt] (China, Hong Kong)
+- [Froggit][froggit] (Germany)
+
+...and many others. For more information on how these brands relate to one another, see
+this forum post: https://www.wxforum.net/index.php?topic=40730.0
+
+Although there are some small differences between how these various branded devices are
+configured, `ecowitt2mqtt` endeavors to incorporate them all with minimal effort on the
+user's part.
+
+# Quick Start
+
+First, install `ecowitt2mqtt` via `pip`:
+
+```bash
+$ pip install ecowitt2mqtt
+```
+
+Next, if you haven't already, install the appropriate mobile app to configure your
+device. For example:
+
+- Ambient Weather: awnet ([iOS][awnet-ios]/[Android][awnet-google-play])
+- Ecowitt: WS View ([iOS][ws-view-ios]/[Android][ws-view-google-play])
+
+Find the appropriate location in the mobile app to configure a customized upload target
+for the station's data. This will differ depending on the app, but in general, you
+should select your device and find a screen entitled "Upload" (or similar).
+
+![The "Upload" screen in the awnet app][awnet-upload-screen]
+![The "Upload" screen in the WS View app][ws-view-upload-screen]
+
+Fill out the form with the appropriate values and tap `Save`:
+
+- `Protocol Type Same As`: pick the label that matches your brand (e.g., `Ecowitt` for
+  Ecowitt devices)
+- `Server IP / Hostname`: the IP address/hostname of the device running `ecowitt2mqtt`
+- `Path`: `/data/report/` (the default path used by most mobile apps)
+- `Port`: `8080` (the default port on which `ecowitt2mqtt` is served)
+- `Upload Interval`: 16 (a reasonable short number of seconds between publishes)
+
+Then, on the machine where you installed `ecowitt2mqtt`, run it:
+
+```bash
+$ ecowitt2mqtt \
+    --mqtt-broker=192.168.1.101 \
+    --mqtt-username=user \
+    --mqtt-password=password \
+    --mqtt-topic=ecowitt2mqtt/device_1
+    --input-data-format=ecowitt
+```
+
+Within the `Upload Interval`, data should begin to appear in the MQTT broker.
+
+# Configuration
+
+`ecowitt2mqtt` can be configured via command line options, environment variables, or a
+(YAML or JSON) config file.
+
+## Command Line Options
+
+```
+usage: ecowitt2mqtt [-h] [--version]
+                    [--battery-override BATTERY_OVERRIDE] [-c config]
+                    [--default-battery-strategy default_battery_strategy]
+                    [--diagnostics] [--disable-calculated-data]
+                    [-e endpoint] [--hass-discovery]
+                    [--hass-discovery-prefix hass_discovery_prefix]
+                    [--hass-entity-id-prefix hass_entity_id_prefix]
+                    [--input-data-format input_data_format]
+                    [--input-unit-system input_unit_system]
+                    [-b mqtt_broker] [-p mqtt_password]
+                    [--mqtt-port mqtt_port] [--mqtt-retain]
+                    [--mqtt-tls] [-t mqtt_topic] [-u mqtt_username]
+                    [--output-unit-system output_unit_system]
+                    [--output-unit-accumulated-precipitation output_unit_accumulated_precipitation]
+                    [--output-unit-distance output_unit_distance]
+                    [--output-unit-humidity output_unit_humidity]
+                    [--output-unit-illuminance output_unit_illuminance]
+                    [--output-unit-precipitation-rate output_unit_precipitation_rate]
+                    [--output-unit-pressure output_unit_pressure]
+                    [--output-unit-speed output_unit_speed]
+                    [--output-unit-temperature output_unit_temperature]
+                    [--port port] [--precision precision] [--raw-data]
+                    [-v]
+
+Send data from an Ecowitt gateway to an MQTT broker
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --version             show program's version number and exit
+  --battery-override BATTERY_OVERRIDE
+                        A battery configuration override (format:
+                        key,value)
+  -c config, --config config
+                        A path to a YAML or JSON config file
+  --default-battery-strategy default_battery_strategy
+                        The default battery config strategy to use
+                        (default: boolean)
+  --diagnostics         Output diagnostics
+  --disable-calculated-data
+                        Disable the output of calculated sensors
+  -e endpoint, --endpoint endpoint
+                        The relative endpoint/path to serve
+                        ecowitt2mqtt on (default: /data/report)
+  --hass-discovery      Publish data in the Home Assistant MQTT
+                        Discovery format
+  --hass-discovery-prefix hass_discovery_prefix
+                        The Home Assistant MQTT Discovery topic prefix
+                        to use (default: homeassistant)
+  --hass-entity-id-prefix hass_entity_id_prefix
+                        The prefix to use for Home Assistant entity IDs
+  --input-data-format input_data_format
+                        The input data format used by the gateway
+                        (default: ecowitt)
+  --input-unit-system input_unit_system
+                        The input unit system used by the gateway
+                        (default: imperial)
+  -b mqtt_broker, --mqtt-broker mqtt_broker
+                        The hostname or IP address of an MQTT broker
+  -p mqtt_password, --mqtt-password mqtt_password
+                        A valid password for the MQTT broker
+  --mqtt-port mqtt_port
+                        The listenting port of the MQTT broker
+                        (default: 1883)
+  --mqtt-retain         Instruct the MQTT broker to retain messages
+  --mqtt-tls            Enable MQTT over TLS
+  -t mqtt_topic, --mqtt-topic mqtt_topic
+                        The MQTT topic to publish device data to
+  -u mqtt_username, --mqtt-username mqtt_username
+                        A valid username for the MQTT broker
+  --output-unit-system output_unit_system
+                        The output unit system used by the gateway
+                        (default: imperial)
+  --output-unit-accumulated-precipitation output_unit_accumulated_precipitation
+                        The output unit to use for accumulated
+                        precipitation data points (default: the default
+                        used by the output unit system)
+  --output-unit-distance output_unit_distance
+                        The output unit to use for distance data points
+                        (default: the default used by the output unit
+                        system)
+  --output-unit-humidity output_unit_humidity
+                        The output unit to use for humidity data points
+                        (default: the default used by the output unit
+                        system)
+  --output-unit-illuminance output_unit_illuminance
+                        The output unit to use for illuminance data
+                        points (default: the default used by the output
+                        unit system)
+  --output-unit-precipitation-rate output_unit_precipitation_rate
+                        The output unit to use for precipitation rate
+                        data points (default: the default used by the
+                        output unit system)
+  --output-unit-pressure output_unit_pressure
+                        The output unit to use for pressure data points
+                        (default: the default used by the output unit
+                        system)
+  --output-unit-speed output_unit_speed
+                        The output unit to use for speed data points
+                        (default: the default used by the output unit
+                        system)
+  --output-unit-temperature output_unit_temperature
+                        The output unit to use for temperature data
+                        points (default: the default used by the output
+                        unit system)
+  --port port           The port to serve ecowitt2mqtt on (default:
+                        8080)
+  --precision precision
+                        The precision to output data points at
+                        (default: no limit)
+  --raw-data            Return raw data (don't attempt to translate any
+                        values)
+  -v, --verbose         Increase verbosity of logged output
+```
+
+## Environment Variables
+
+- `ECOWITT2MQTT_BATTERY_OVERRIDE`: a semicolon-delimited list of key=value battery
+  overrides (default: `numeric`)
+- `ECOWITT2MQTT_CONFIG`: a path to a YAML or JSON config file (default: `None`)
+- `ECOWITT2MQTT_DEFAULT_BATTERY_STRATEGY`: the default battery config strategy to use
+  (default: `boolean`)
+- `ECOWITT2MQTT_DIAGNOSTICS`: whether to output diagnostics (default: `false`)
+- `ECOWITT2MQTT_DISABLE_CALCULATED_DATA`: whether to disable the output of calculated
+  sensors (default: `false`)
+- `ECOWITT2MQTT_ENDPOINT`: the relative endpoint/path to serve ecowitt2mqtt on (default:
+  `/data/report`)
+- `ECOWITT2MQTT_HASS_DISCOVERY_PREFIX`: the Home Assistant discovery prefix to use
+  (default: `homeassistant`)
+- `ECOWITT2MQTT_HASS_DISCOVERY`: publish data in the Home Assistant MQTT Discovery format
+  (default: `false`)
+- `ECOWITT2MQTT_HASS_ENTITY_ID_PREFIX`: the prefix to use for Home Assistant entity IDs
+  (default: `""`)
+- `ECOWITT2MQTT_INPUT_DATA_FORMAT`: the input data format used by the gateway (default:
+  `ecowitt`)
+- `ECOWITT2MQTT_INPUT_UNIT_SYSTEM`: the input unit system used by the device (default:
+  `imperial`)
+- `ECOWITT2MQTT_MQTT_BROKER`: the hostname or IP address of an MQTT broker
+- `ECOWITT2MQTT_MQTT_PASSWORD`: a valid password for the MQTT broker
+- `ECOWITT2MQTT_MQTT_PORT`: the listenting port of the MQTT broker (default: `1883`)
+- `ECOWITT2MQTT_MQTT_RETAIN`: whether to instruct the MQTT broker to retain messages
+  (default: `false`)
+- `ECOWITT2MQTT_MQTT_TLS`: publish data via MQTT over TLS (default: `false`)
+- `ECOWITT2MQTT_MQTT_TOPIC`: the MQTT topic to publish device data to
+- `ECOWITT2MQTT_MQTT_USERNAME`: a valid username for the MQTT broker
+- `ECOWITT2MQTT_OUTPUT_UNIT_SYSTEM`: the unit system to use in output (default: `imperial`)
+- `ECOWITT2MQTT_OUTPUT_UNIT_TEMPERATURE`: the output unit to use for temperature data
+  points (default: the default used by the output unit system)
+- `ECOWITT2MQTT_PORT`: the port to serve ecowitt2mqtt on (default: `8080`)
+- `ECOWITT2MQTT_PRECISION`: the precision to output data points at (default: no limit)
+- `ECOWITT2MQTT_RAW_DATA`: return raw data (don't attempt to translate any values)
+  (default: `false`)
+- `ECOWITT2MQTT_VERBOSE`: increase verbosity of logged output (default: `false`)
+
+## Configuration File
+
+The configuration file can be formatted as either YAML:
+
+```yaml
+---
+battery_override:
+  battery_key1: boolean
+default_battery_strategy: numeric
+diagnostics: false
+disable_calculated_data: false
+endpoint: /data/report
+hass_discovery: false
+hass_discovery_prefix: homeassistant
+hass_entity_id_prefix: test_prefix
+input_data_format: ecowitt
+input_unit_system: imperial
+mqtt_broker: 127.0.0.1
+mqtt_password: password
+mqtt_port: 1883
+mqtt_retain: false
+mqtt_tls: false
+mqtt_topic: Test
+mqtt_username: user
+output_unit_system: imperial
+port: 8080
+raw_data: false
+verbose: false
+```
+
+...or JSON
+
+```json
+{
+  "battery_override": {
+    "battery_key1": "boolean"
+  },
+  "default_battery_strategy": "numeric",
+  "diagnostics": false,
+  "disable_calculated_data": false,
+  "endpoint": "/data/report",
+  "hass_discovery": false,
+  "hass_discovery_prefix": "homeassistant",
+  "hass_entity_id_prefix": "test_prefix"
+  "input_data_format": "ecowitt",
+  "input_unit_system": "imperial",
+  "mqtt_broker": "127.0.0.1",
+  "mqtt_password": "password",
+  "mqtt_port": 1883,
+  "mqtt_retain": true,
+  "mqtt_tls": false,
+  "mqtt_topic": "Test",
+  "mqtt_username": "user",
+  "output_unit_system": "imperial",
+  "port": 8080,
+  "raw_data": false,
+  "verbose": false
+}
+```
+
+...and makes use of the same config options available to the CLI.
+
+### Multiple Gateways
+
+When using the configuration file, it is possible to define specific configuration
+parameters for multiple Ecowitt gateways. This is useful if different gateways should
+publish to different MQTT brokers, in different formats, etc.
+
+First, you must determine the unique ID for each gateway. This can be observed in the
+logs when `verbose` is enabled – look for the `PASSKEY` value that the gateway has:
+
+```
+Received data from the Ecowitt device: {'PASSKEY': 'abcde12345', ...}
+```
+
+Then, in the configuration file, simply add a `gateways` key that contains a mapping of
+any of the existing configuration options (except for `--verbose` and `--diagnostics`,
+which can only be defined once and are applied to _every_ configuration). Options that
+remain at the root level of the file are treated as defaults.
+
+For example, this YAML configuration file:
+
+```yaml
+---
+mqtt_broker: 127.0.0.1
+mqtt_password: password
+mqtt_topic: Test
+mqtt_username: user
+
+gateways:
+  abcde12345:
+    hass_discovery: true
+```
+
+...defines two gateway definitions:
+
+- One that publishes to the `Test` topic on an MQTT broker at `127.0.0.1`
+- One (with a `PASSKEY` of `abcde12345`) that publishes to the same broker, but in Home
+  Assistant MQTT Discovery format.
+
+In another example, this JSON configuration file:
+
+```json
+{
+  "mqtt_broker": "127.0.0.1",
+  "mqtt_password": "password",
+  "mqtt_port": 1883,
+  "mqtt_topic": "Test",
+  "mqtt_username": "user",
+  "gateways": {
+    "abcde12345": {
+      "mqtt_broker": "192.168.1.100",
+      "mqtt_retain": true,
+      "output_unit_system": "metric"
+    }
+  }
+}
+```
+
+...defines two gateway definitions:
+
+- One that publishes to the `Test` topic on an MQTT broker at `127.0.0.1`
+- One (with a `PASSKEY` of `abcde12345`) that publishes to a different broker
+  (`192.168.1.100`), outputs the data in metric, and retains the data on the broker
+
+## Merging Configuration Options
+
+When parsing configuration options, `ecowitt2mqtt` looks at the configuration sources in
+the following order:
+
+1. Configuration File (Specific Gateway)
+2. Configuration File (Defaults)
+3. Environment Variables
+4. CLI Options
+
+This allows you to mix and match sources – for instance, you might have "defaults" in
+the configuration file and override them via environment variables.
+
+## Input Data Formats
+
+`ecowitt2mqtt` currently supports the following input data formats:
+
+- `ambient_weather`
+- `ecowitt`
+
+Provide the correct one to `---input-data-format` based on which device brand you use.
+
+# Advanced Usage
+
+## Calculated Sensors
+
+In addition to the data coming from a gateway, `ecowitt2mqtt` will automatically deduce
+and published several additional, calculated data points if the requisite underlying
+data exists:
+
+- **[Absolute Humidity][absolute-humidity]:** the actual volume of water vapor in the
+  air
+- **[Beaufort Scale][beaufort-scale]:** the empirical measure that relates wind speed to
+  observed conditions at sea or on land
+- **[Dew Point][dew-point]:** the temperature to which air must be cooled to become
+  saturated with water vapor, assuming constant air pressure and water content
+- **[Feels Like][heat-index]:** how hot or how cold the air feels to the human body when
+  factoring in variables such as relative humidity, wind speeds, the amount of sunshine,
+  etc.
+- **[Frost Point][frost-point]:** the temperature below 32°F (0°C) at which moisture in
+  the air will condense as a layer of frost on exposed surfaces that are also at a
+  temperature below the frost point
+- **[Frost Risk][frost-point]:** how likely the formation of frost is (based on the
+  `frostpoint`)
+- **[Heat Index][heat-index]:** how hot the air feels to the human body when factoring
+  in relative humidity (applicable when the apparent temperature is higher than the air
+  temperature)
+- **[Humidex][humidex]:** an index number used by Canadian meteorologists to describe
+  how hot the weather feels to the average person, by combining the effect of heat and
+  humidity
+- **[Humidex Perception][humidex]:** a human-friendly interpretation of the Humidex
+- **Relative Strain Index:** a measure of discomfort resulting from the combined effect
+  of temperature and humidity (applicable to heat stress of manual workers under shelter
+  at various metabolic rates)
+- **Relative Strain Index Perception:** a human-friendly interpretation of the Relative
+  Strain Index
+- **[Safe Exposure Times][safe-exposure-times]:** how long different skin types can be
+  in the sun (unprotected) before burning begins according to the
+  [Fitzpatrick Scale][fitzpatrick-scale]
+- **Solar Radiation (%):** the percentage of detected solar radiation illuminance as
+  perceived by the human eye
+- **[Simmer Index][simmer-index]:** an alternative to heat index that describes how how
+  the air feels to the human body in relatively dry environments
+- **[Simmer Zone][simmer-index]:** a human-friendly interpretation of the Simmer Index
+- **[Thermal Perception][dew-point]:** a human-friendly interpretation of the Dew Point
+- **[Wind Chill][wind-chill]:** how cold the air feels to the human body when factoring
+  in relative humidity, wind speed, etc. (applicable when the apparent temperature is
+  lower than the air temperature)
+
+(Special thanks to the excellent [`thermal_comfort` library][thermal-comfort-library] for
+inspiration on many of these.)
+
+If you would prefer to not have these sensors calculated and published, you can utilize
+the `--disable-calculated-data` configuration option.
+
+## Battery Configurations
+
+Ecowitt devices report battery levels in three different formats:
+
+- `boolean`: `0` represents `OFF` (i.e., the battery is in normal condition) and `1` represents
+  `ON` (i.e., the battery is low).
+- `numeric`: the raw numeric value is interpreted as the number of volts remaining in the
+  battery.
+- `percentage`: the raw numeric value is interpreted as the percentage of voltage
+  remaining the battery.
+
+`ecowitt2mqtt` provides three mechanisms to handle this complexity:
+
+1. A built-in mapping of all currently known battery types to their assumed strategy
+2. A default battery strategy for unknown battery types
+3. User-defined battery strategy overrides
+
+### Built-in Mapping
+
+`ecowitt2mqtt` contains an internal mapping that should automatically transform all
+known battery types into their correct format.
+
+### Default Battery Strategy
+
+By using the `--default-battery-strategy` configuration parameter, users can specify how
+unknown battery types should be treated by default.
+
+### Battery Overrides
+
+Individual batteries can be overridden and given a new strategy. How this is
+accomplished differs slightly based on the configuration method used:
+
+- Command Line Options: provide one or more `--battery-override "batt1=boolean"` options
+- Environment Variables: provide a `ECOWITT2MQTT_BATTERY_OVERRIDE` variable that is a
+  semicolon-delimited pair of "key=value" strings (e.g.,
+  `ECOWITT2MQTT_BATTERY_OVERRIDE="batt1=boolean;batt2=numeric"`)
+- Config File: include a dictionary of key/value pairs in either YAML or JSON format
+
+These overrides work on both known and unknown battery types; that said, if you should
+find the need to override a known battery type because `ecowitt2mqtt` has an incorrect
+internal interpretation, submit an issue to get it corrected!
+
+### Example
+
+In this example, a user mostly has batteries that should be treated as `boolean`, but
+also has one – `wh60_batt1` – that should be treated as numeric.
+
+#### Command Line Options
+
+```
+$ ecowitt2mqtt --default-battery-strategy boolean --battery-override="wh60_batt1=numeric"
+```
+
+#### Environment Variables
+
+```
+$ ECOWITT2MQTT_DEFAULT_BATTERY_STRATEGY=boolean \
+  ECOWITT2MQTT_BATTERY_OVERRIDE="wh60_batt1=numeric" \
+  ecowitt2mqtt
+```
+
+#### Config File
+
+In YAML:
+
+```yaml
+---
+default_battery_strategy: boolean
+battery_override:
+  wh60_batt1: numeric
+```
+
+...or JSON
+
+```json
+{
+  "default_battery_strategy": "boolean",
+  "battery_override": {
+    "wh60_batt1": "numeric"
+  }
 }
+```
+
+## Unit Systems
+
+### Input and Output
+
+`ecowitt2mqtt` allows you to specify both the input and output unit systems for a device
+via the `--input-unit-system` and `--output-unit-system` config options, respectively.
+These are fairly self-explanatory, but take care to use an `--input-unit-system` that is
+consistent with what your device provides (otherwise, your data will be very "off").
+
+### Overriding Units for Data Categories
+
+If you wish, you can change the unit for individual data categories. For example, let's
+say you wanted to use metric for the output unit system, but wanted to represent all
+temperature data points in Kelvin – you would provide `--output-unit-system=metric` and
+`--output-unit-temperature=K` as config options. As expected, the value is properly
+converted to the new unit.
+
+#### Accumulated Precipitation
+
+Config Option: `--output-unit-accumulated-precipitation`
+
+- `in`
+- `mm`
+
+#### Absolute Humidity
+
+Config Option: `--output-unit-humidity`
+
+- `g/m³`
+- `lbs/ft³`
+
+#### Illuminance
+
+Config Option: `--output-unit-illuminance`
+
+- `fc`
+- `kfc`
+- `klx`
+- `lx`
+- `W/m²`
+
+#### Precipitation Rate
+
+Config Option: `--output-unit-precipitation-rate`
+
+- `in/h`
+- `mm/h`
+
+#### Pressure
+
+Config Option: `--output-unit-pressure`
+
+- `bar`
+- `cbar`
+- `hPa`
+- `inHg`
+- `kPa`
+- `mbar`
+- `mmHg`
+- `Pa`
+- `psi`
+
+#### Speed
+
+Config Option: `--output-unit-speed`
+
+- `ft/s`
+- `in/d`
+- `in/h`
+- `km/h`
+- `kn`
+- `m/s`
+- `mph`
+- `mm/d`
+
+#### Temperature
+
+Config Option: `--output-unit-temperature`
+
+- `°C`
+- `°F`
+- `K`
+
+## Raw Data
+
+In some cases, it may be preferable to prevent `ecowitt2mqtt` from doing any data
+translation (converting values to a new unit system, changing binary values – such as
+might be used by a battery – into "friendly" values, etc.). Passing the `--raw-data` flag
+will accomplish this: data will flow directly from the Ecowitt device to the MQTT broker
+as-is.
+
+Note that the `--raw-data` flag supersedes any that might cause data translation (such as
+`--input-unit-system` or `--output-unit-system`).
+
+## Home Assistant
+
+### MQTT Discovery
+
+[Home Assistant][home-assistant] users can quickly add entities from an Ecowitt device
+by using [MQTT Discovery][home-assistant-mqtt-discovery]. Once Home Assistant is
+configured to accept MQTT Discovery, `ecowitt2mqtt` simply needs the `--hass-discovery`
+flag:
+
+```bash
+$ ecowitt2mqtt \
+    --mqtt-broker=192.168.1.101 \
+    --mqtt-username=user \
+    --mqtt-password=password \
+    --hass-discovery
+```
+
+### Custom Entity ID Prefix
+
+You can provide a custom prefix for all Home Assistant entities via the
+`--hass-entity-id-prefix` config parameter.
+
+### Home Assistant OS Add-on
+
+Home Assistant OS users can install the official `ecowitt2mqtt` add-on by clicking the
+link below:
+
+[![Home Assistant Add-on][home-assistant-addon-badge]][home-assistant-addon]
+
+## Running in the Background
+
+`ecowitt2mqtt` doesn't, itself, provide any sort of daemonization mechanism. The suggested
+route is to use a different application.
+
+### `supervisord`
+
+An example `supervisord` configuration file might look like this:
+
+```
+[supervisord]
+nodaemon=true
+loglevel=info
+user=root
+
+[program:ecowitt2mqtt]
+command=ecowitt2mqtt --mqtt-broker=192.168.1.101 --mqtt-username=user --mqtt-password=password
+stdout_logfile=/dev/stdout
+stdout_logfile_maxbytes=0
+redirect_stderr=true
+```
+
+### `systemd`
+
+An example `systemd` service file in `/etc/systemd/system` might look like this:
+
+```
+[Unit]
+Description=ECOWITT2MQTT daemon
+After=network.target
+
+[Service]
+Type=simple
+ExecStart=ecowitt2mqtt --mqtt-broker=192.168.1.101 --mqtt-username=user --mqtt-password=password
+ExecReload=kill -HUP $MAINPID
+KillMode=process
+Restart=on-failure
+RestartSec=5s
+
+[Install]
+WantedBy=multi-user.target
+```
+
+To enable the service:
+
+```bash
+$ systemctl enable ecowitt2mqtt
+```
+
+## Docker
+
+The library is available via a Docker image from both [Docker Hub][docker-hub] and
+[ghcr.io][ghcr]. It is configured by using the same environment variables listed
+[above](#environment-variables).
+
+Running the image is straightforward:
+
+```
+docker run -it \
+    -e ECOWITT2MQTT_MQTT_BROKER=192.168.1.101 \
+    -e ECOWITT2MQTT_MQTT_USERNAME=user \
+    -e ECOWITT2MQTT_MQTT_PASSWORD=password \
+    -p 8080:8080 \
+    bachya/ecowitt2mqtt:latest
+```
+
+Note the value of the `-p` flag: you must expose the port defined by the `PORT`
+environment variable. In the example above, the default port (`8080`) is used and is
+exposed via the same port on the host.
+
+[`docker-compose`][docker-compose] users can find an example configuration file at
+[`docker-compose.dev.yml`](docker-compose.dev.yml). Note that this is intended to be a dev
+environment for quickly testing the repo itself; in production, you should refer to one
+of the published images.
+
+# Diagnostics
+
+You may run `ecowitt2mqtt` in diagnostics mode by providing the `--diagnostics` flag. In
+this mode, the app will wait until it receives and publishes a single payload, then
+exit. This allows users to collect a small-but-complete payload for use in testing,
+debugging, and issue reporting.
+
+# Contributing
+
+Thanks to all of [our contributors][contributors] so far!
+
+1. [Check for open features/bugs][issues] or [initiate a discussion on one][new-issue].
+2. [Fork the repository][fork].
+3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`
+4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`
+5. Install the dev environment: `script/setup`
+6. Code your new feature or bug fix on a new branch.
+7. Write tests that cover your new functionality.
+8. Run tests and ensure 100% code coverage: `poetry run pytest --cov ecowitt2mqtt tests`
+9. Update `README.md` with any new documentation.
+10. Submit a pull request!
 
+[absolute-humidity]: https://en.wikipedia.org/wiki/Humidity#Absolute_humidity
+[ambient-weather]: https://ambientweather.com/
+[awnet-google-play]: https://play.google.com/store/apps/details?id=com.dtston.ambienttoolplus&hl=en_US&gl=US
+[awnet-ios]: https://apps.apple.com/us/app/awnet/id1341994564
+[awnet-upload-screen]: resources/awnet-upload-screen.jpeg?raw=true
+[beaufort-scale]: https://en.wikipedia.org/wiki/Beaufort_scale
+[ci-badge]: https://github.com/bachya/ecowitt2mqtt/workflows/CI/badge.svg
+[ci]: https://github.com/bachya/ecowitt2mqtt/actions
+[codecov-badge]: https://codecov.io/gh/bachya/ecowitt2mqtt/branch/dev/graph/badge.svg
+[codecov]: https://codecov.io/gh/bachya/ecowitt2mqtt
+[coffee-image]: https://cdn.buymeacoffee.com/buttons/default-orange.png
+[coffee]: https://www.buymeacoffee.com/bachya1208P
+[contributors]: https://github.com/bachya/ecowitt2mqtt/graphs/contributors
+[dew-point]: https://en.wikipedia.org/wiki/Dew_point
+[docker-compose]: https://docs.docker.com/compose/
+[docker-hub-badge]: https://img.shields.io/docker/pulls/bachya/ecowitt2mqtt
+[docker-hub]: https://hub.docker.com/r/bachya/ecowitt2mqtt
+[ecowitt]: https://www.ecowitt.com/
+[fitzpatrick-scale]: https://en.wikipedia.org/wiki/Fitzpatrick_scale
+[fork]: https://github.com/bachya/ecowitt2mqtt/fork
+[froggit]: https://www.froggit.de/Weather-Station/
+[frost-point]: https://en.wikipedia.org/wiki/Dew_point#Frost_point
+[ghcr]: https://ghcr.io/bachya/ecowitt2mqtt
+[heat-index]: https://en.wikipedia.org/wiki/Heat_index
+[home-assistant-addon-badge]: https://my.home-assistant.io/badges/supervisor_addon.svg
+[home-assistant-addon]: https://my.home-assistant.io/redirect/supervisor_addon/?addon=c35f0383_ecowitt2mqtt&repository_url=https%3A%2F%2Fgithub.com%2Fbachya%2Fhome-assistant-addons
+[home-assistant-mqtt-discovery]: https://www.home-assistant.io/docs/mqtt/discovery/
+[home-assistant]: https://home-assistant.io
+[humidex]: https://en.wikipedia.org/wiki/Humidex
+[issues]: https://github.com/bachya/ecowitt2mqtt/issues
+[license-badge]: https://img.shields.io/pypi/l/ecowitt2mqtt.svg
+[license]: https://github.com/bachya/ecowitt2mqtt/blob/main/LICENSE
+[logo]: resources/logo-full.png
+[maintainability-badge]: https://api.codeclimate.com/v1/badges/a03c9e96f19a3dc37f98/maintainability
+[maintainability]: https://codeclimate.com/github/bachya/ecowitt2mqtt/maintainability
+[new-issue]: https://github.com/bachya/ecowitt2mqtt/issues/new
+[pypi-badge]: https://img.shields.io/pypi/v/ecowitt2mqtt.svg
+[pypi]: https://pypi.python.org/pypi/ecowitt2mqtt
+[safe-exposure-times]: https://www.openuv.io/kb/skin-types-safe-exposure-time-calculation/
+[simmer-index]: http://summersimmer.com/ssi_page2.htm
+[thermal-comfort-library]: https://github.com/dolezsa/thermal_comfort
+[version-badge]: https://img.shields.io/pypi/pyversions/ecowitt2mqtt.svg
+[version]: https://pypi.python.org/pypi/ecowitt2mqtt
+[wind-chill]: https://en.wikipedia.org/wiki/Wind_chill
+[ws-view-google-play]: https://play.google.com/store/apps/details?id=com.ost.wsview&gl=US
+[ws-view-ios]: https://apps.apple.com/us/app/ws-view/id1362944193
+[ws-view-upload-screen]: resources/ws-view-upload-screen.jpeg?raw=true
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,420 +1,403 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['ecowitt2mqtt', 'ecowitt2mqtt.backports', 'ecowitt2mqtt.helpers',
-'ecowitt2mqtt.helpers.calculator', 'ecowitt2mqtt.helpers.publisher',
-'ecowitt2mqtt.util'] package_data = \ {'': ['*']} install_requires = \
-['aiohttp>=3.8.1,<4.0.0', 'asyncio-mqtt>=0.12.1', 'colorlog>=6.6.0,<7.0.0',
-'fastapi>=0.89.1,<0.93.0', 'meteocalc>=1.1.0,<2.0.0', 'python-
-multipart>=0.0.5,<0.0.6', 'rapidfuzz>=2.13.0,<3.0.0',
-'ruamel.yaml>=0.17.21,<0.18.0', 'uvicorn>=0.19.0', 'uvloop>=0.17.0,<0.18.0',
-'voluptuous>=0.13.1,<0.14.0'] entry_points = \ {'console_scripts':
-['ecowitt2mqtt = ecowitt2mqtt.__main__:main']} setup_kwargs = { 'name':
-'ecowitt2mqtt', 'version': '2023.2.1', 'description': 'A small web server to
-send data from Ecowitt devices to an MQTT Broker', 'long_description': '!
-[ecowitt2mqtt][logo]\n\n[![CI][ci-badge]][ci]\n[![PyPI][pypi-badge]][pypi]\n[!
-[Docker Hub][docker-hub-badge]][docker-hub]\n[![Version][version-badge]]
-[version]\n[![License][license-badge]][license]\n[![Code Coverage][codecov-
-badge]][codecov]\n[![Maintainability][maintainability-badge]]
-[maintainability]\n\n[Buy_Me_A_Coffee]\n\n`ecowitt2mqtt` is a small CLI/web
-server that can receive data from Fine Offset weather\nstations (and their
-numerous white-labeled counterparts, like Ecowitt and\nAmbient Weather), adjust
-that data in numerous ways, and send it on to one or more\nMQTT brokers.\n\n-
-[Installation](#installation)\n- [Python Versions](#python-versions)\n-
-[Disclaimer](#disclaimer)\n- [Supported Brands](#supported-brands)\n- [Quick
-Start](#quick-start)\n- [Configuration](#configuration)\n - [Command Line
-Options](#command-line-options)\n - [Environment Variables](#environment-
-variables)\n - [Configuration File](#configuration-file)\n - [Merging
-Configuration Options](#merging-configuration-options)\n - [Input Data Formats]
-(#input-data-formats)\n- [Advanced Usage](#advanced-usage)\n - [Calculated
-Sensors](#calculated-sensors)\n - [Battery Configurations](#battery-
-configurations)\n - [Unit Systems](#unit-systems)\n - [Raw Data](#raw-data)\n -
-[Home Assistant](#home-assistant)\n - [Running in the Background](#running-in-
-the-background)\n - [Docker](#docker)\n- [Diagnostics](#diagnostics)\n-
-[Contributing](#contributing)\n\n# Installation\n\n```bash\npip install
-ecowitt2mqtt\n```\n\n# Python Versions\n\n`ecowitt2mqtt` is currently supported
-on:\n\n- Python 3.9\n- Python 3.10\n- Python 3.11\n\n# Disclaimer\n\nThe
-datapoints within this library and documentation constitute estimates and
-are\nintended to help informed decision making. They should not replace
-analysis, advice, or\ndiagnosis from trained professionals. Use this data at
-your own discretion.\n\n# Supported Brands\n\nDespite the name of the library,
-`ecowitt2mqtt` should support any weather station/gateway\nthat is produced by
-[Fine Offset](https://www.foshk.com/). This includes brands that\nwhite-label
-Fine Offset equipment, such as:\n\n- [Ambient Weather][ambient-weather]
-(U.S.)\n- [Ecowitt][ecowitt] (China, Hong Kong)\n- [Froggit][froggit]
-(Germany)\n\n...and many others. For more information on how these brands
-relate to one another, see\nthis forum post: https://www.wxforum.net/
-index.php?topic=40730.0\n\nAlthough there are some small differences between
-how these various branded devices are\nconfigured, `ecowitt2mqtt` endeavors to
-incorporate them all with minimal effort on the\nuser\'s part.\n\n# Quick
-Start\n\nFirst, install `ecowitt2mqtt` via `pip`:\n\n```bash\n$ pip install
-ecowitt2mqtt\n```\n\nNext, if you haven\'t already, install the appropriate
-mobile app to configure your\ndevice. For example:\n\n- Ambient Weather: awnet
-([iOS][awnet-ios]/[Android][awnet-google-play])\n- Ecowitt: WS View ([iOS][ws-
-view-ios]/[Android][ws-view-google-play])\n\nFind the appropriate location in
-the mobile app to configure a customized upload target\nfor the station\'s
-data. This will differ depending on the app, but in general, you\nshould select
-your device and find a screen entitled "Upload" (or similar).\n\n![The "Upload"
-screen in the awnet app][awnet-upload-screen]\n![The "Upload" screen in the WS
-View app][ws-view-upload-screen]\n\nFill out the form with the appropriate
-values and tap `Save`:\n\n- `Protocol Type Same As`: pick the label that
-matches your brand (e.g., `Ecowitt` for\n Ecowitt devices)\n- `Server IP /
-Hostname`: the IP address/hostname of the device running `ecowitt2mqtt`\n-
-`Path`: `/data/report/` (the default path used by most mobile apps)\n- `Port`:
-`8080` (the default port on which `ecowitt2mqtt` is served)\n- `Upload
-Interval`: 16 (a reasonable short number of seconds between publishes)\n\nThen,
-on the machine where you installed `ecowitt2mqtt`, run it:\n\n```bash\n$
-ecowitt2mqtt \\\n --mqtt-broker=192.168.1.101 \\\n --mqtt-username=user \\\n --
-mqtt-password=password \\\n --mqtt-topic=ecowitt2mqtt/device_1\n --input-data-
-format=ecowitt\n```\n\nWithin the `Upload Interval`, data should begin to
-appear in the MQTT broker.\n\n# Configuration\n\n`ecowitt2mqtt` can be
-configured via command line options, environment variables, or a\n(YAML or
-JSON) config file.\n\n## Command Line Options\n\n```\nusage: ecowitt2mqtt [-h]
-[--version]\n [--battery-override BATTERY_OVERRIDE] [-c config]\n [--default-
-battery-strategy default_battery_strategy]\n [--diagnostics] [--disable-
-calculated-data]\n [-e endpoint] [--hass-discovery]\n [--hass-discovery-prefix
-hass_discovery_prefix]\n [--hass-entity-id-prefix hass_entity_id_prefix]\n [--
-input-data-format input_data_format]\n [--input-unit-system
-input_unit_system]\n [-b mqtt_broker] [-p mqtt_password]\n [--mqtt-port
-mqtt_port] [--mqtt-retain]\n [--mqtt-tls] [-t mqtt_topic] [-u mqtt_username]\n
-[--output-unit-system output_unit_system]\n [--output-unit-accumulated-
-precipitation output_unit_accumulated_precipitation]\n [--output-unit-distance
-output_unit_distance]\n [--output-unit-humidity output_unit_humidity]\n [--
-output-unit-illuminance output_unit_illuminance]\n [--output-unit-
-precipitation-rate output_unit_precipitation_rate]\n [--output-unit-pressure
-output_unit_pressure]\n [--output-unit-speed output_unit_speed]\n [--output-
-unit-temperature output_unit_temperature]\n [--port port] [--precision
-precision] [--raw-data]\n [-v]\n\nSend data from an Ecowitt gateway to an MQTT
-broker\n\noptional arguments:\n -h, --help show this help message and exit\n --
-version show program\'s version number and exit\n --battery-override
-BATTERY_OVERRIDE\n A battery configuration override (format:\n key,value)\n -
-c config, --config config\n A path to a YAML or JSON config file\n --default-
-battery-strategy default_battery_strategy\n The default battery config strategy
-to use\n (default: boolean)\n --diagnostics Output diagnostics\n --disable-
-calculated-data\n Disable the output of calculated sensors\n -e endpoint, --
-endpoint endpoint\n The relative endpoint/path to serve\n ecowitt2mqtt on
-(default: /data/report)\n --hass-discovery Publish data in the Home Assistant
-MQTT\n Discovery format\n --hass-discovery-prefix hass_discovery_prefix\n The
-Home Assistant MQTT Discovery topic prefix\n to use (default: homeassistant)\n
---hass-entity-id-prefix hass_entity_id_prefix\n The prefix to use for Home
-Assistant entity IDs\n --input-data-format input_data_format\n The input data
-format used by the gateway\n (default: ecowitt)\n --input-unit-system
-input_unit_system\n The input unit system used by the gateway\n (default:
-imperial)\n -b mqtt_broker, --mqtt-broker mqtt_broker\n The hostname or IP
-address of an MQTT broker\n -p mqtt_password, --mqtt-password mqtt_password\n A
-valid password for the MQTT broker\n --mqtt-port mqtt_port\n The listenting
-port of the MQTT broker\n (default: 1883)\n --mqtt-retain Instruct the MQTT
-broker to retain messages\n --mqtt-tls Enable MQTT over TLS\n -t mqtt_topic, --
-mqtt-topic mqtt_topic\n The MQTT topic to publish device data to\n -
-u mqtt_username, --mqtt-username mqtt_username\n A valid username for the MQTT
-broker\n --output-unit-system output_unit_system\n The output unit system used
-by the gateway\n (default: imperial)\n --output-unit-accumulated-precipitation
-output_unit_accumulated_precipitation\n The output unit to use for
-accumulated\n precipitation data points (default: the default\n used by the
-output unit system)\n --output-unit-distance output_unit_distance\n The output
-unit to use for distance data points\n (default: the default used by the output
-unit\n system)\n --output-unit-humidity output_unit_humidity\n The output unit
-to use for humidity data points\n (default: the default used by the output
-unit\n system)\n --output-unit-illuminance output_unit_illuminance\n The output
-unit to use for illuminance data\n points (default: the default used by the
-output\n unit system)\n --output-unit-precipitation-rate
-output_unit_precipitation_rate\n The output unit to use for precipitation
-rate\n data points (default: the default used by the\n output unit system)\n --
-output-unit-pressure output_unit_pressure\n The output unit to use for pressure
-data points\n (default: the default used by the output unit\n system)\n --
-output-unit-speed output_unit_speed\n The output unit to use for speed data
-points\n (default: the default used by the output unit\n system)\n --output-
-unit-temperature output_unit_temperature\n The output unit to use for
-temperature data\n points (default: the default used by the output\n unit
-system)\n --port port The port to serve ecowitt2mqtt on (default:\n 8080)\n --
-precision precision\n The precision to output data points at\n (default: no
-limit)\n --raw-data Return raw data (don\'t attempt to translate any\n
-values)\n -v, --verbose Increase verbosity of logged output\n```\n\n##
-Environment Variables\n\n- `ECOWITT2MQTT_BATTERY_OVERRIDE`: a semicolon-
-delimited list of key=value battery\n overrides (default: `numeric`)\n-
-`ECOWITT2MQTT_CONFIG`: a path to a YAML or JSON config file (default:
-`None`)\n- `ECOWITT2MQTT_DEFAULT_BATTERY_STRATEGY`: the default battery config
-strategy to use\n (default: `boolean`)\n- `ECOWITT2MQTT_DIAGNOSTICS`: whether
-to output diagnostics (default: `false`)\n-
-`ECOWITT2MQTT_DISABLE_CALCULATED_DATA`: whether to disable the output of
-calculated\n sensors (default: `false`)\n- `ECOWITT2MQTT_ENDPOINT`: the
-relative endpoint/path to serve ecowitt2mqtt on (default:\n `/data/report`)\n-
-`ECOWITT2MQTT_HASS_DISCOVERY_PREFIX`: the Home Assistant discovery prefix to
-use\n (default: `homeassistant`)\n- `ECOWITT2MQTT_HASS_DISCOVERY`: publish data
-in the Home Assistant MQTT Discovery format\n (default: `false`)\n-
-`ECOWITT2MQTT_HASS_ENTITY_ID_PREFIX`: the prefix to use for Home Assistant
-entity IDs\n (default: `""`)\n- `ECOWITT2MQTT_INPUT_DATA_FORMAT`: the input
-data format used by the gateway (default:\n `ecowitt`)\n-
-`ECOWITT2MQTT_INPUT_UNIT_SYSTEM`: the input unit system used by the device
-(default:\n `imperial`)\n- `ECOWITT2MQTT_MQTT_BROKER`: the hostname or IP
-address of an MQTT broker\n- `ECOWITT2MQTT_MQTT_PASSWORD`: a valid password for
-the MQTT broker\n- `ECOWITT2MQTT_MQTT_PORT`: the listenting port of the MQTT
-broker (default: `1883`)\n- `ECOWITT2MQTT_MQTT_RETAIN`: whether to instruct the
-MQTT broker to retain messages\n (default: `false`)\n- `ECOWITT2MQTT_MQTT_TLS`:
-publish data via MQTT over TLS (default: `false`)\n- `ECOWITT2MQTT_MQTT_TOPIC`:
-the MQTT topic to publish device data to\n- `ECOWITT2MQTT_MQTT_USERNAME`: a
-valid username for the MQTT broker\n- `ECOWITT2MQTT_OUTPUT_UNIT_SYSTEM`: the
-unit system to use in output (default: `imperial`)\n-
-`ECOWITT2MQTT_OUTPUT_UNIT_TEMPERATURE`: the output unit to use for temperature
-data\n points (default: the default used by the output unit system)\n-
-`ECOWITT2MQTT_PORT`: the port to serve ecowitt2mqtt on (default: `8080`)\n-
-`ECOWITT2MQTT_PRECISION`: the precision to output data points at (default: no
-limit)\n- `ECOWITT2MQTT_RAW_DATA`: return raw data (don\'t attempt to translate
-any values)\n (default: `false`)\n- `ECOWITT2MQTT_VERBOSE`: increase verbosity
-of logged output (default: `false`)\n\n## Configuration File\n\nThe
-configuration file can be formatted as either YAML:\n\n```yaml\n---
-\nbattery_override:\n battery_key1: boolean\ndefault_battery_strategy:
-numeric\ndiagnostics: false\ndisable_calculated_data: false\nendpoint: /data/
-report\nhass_discovery: false\nhass_discovery_prefix:
-homeassistant\nhass_entity_id_prefix: test_prefix\ninput_data_format:
-ecowitt\ninput_unit_system: imperial\nmqtt_broker: 127.0.0.1\nmqtt_password:
-password\nmqtt_port: 1883\nmqtt_retain: false\nmqtt_tls: false\nmqtt_topic:
-Test\nmqtt_username: user\noutput_unit_system: imperial\nport: 8080\nraw_data:
-false\nverbose: false\n```\n\n...or JSON\n\n```json\n{\n "battery_override":
-{\n "battery_key1": "boolean"\n },\n "default_battery_strategy": "numeric",\n
-"diagnostics": false,\n "disable_calculated_data": false,\n "endpoint": "/data/
-report",\n "hass_discovery": false,\n "hass_discovery_prefix":
-"homeassistant",\n "hass_entity_id_prefix": "test_prefix"\n
-"input_data_format": "ecowitt",\n "input_unit_system": "imperial",\n
-"mqtt_broker": "127.0.0.1",\n "mqtt_password": "password",\n "mqtt_port":
-1883,\n "mqtt_retain": true,\n "mqtt_tls": false,\n "mqtt_topic": "Test",\n
-"mqtt_username": "user",\n "output_unit_system": "imperial",\n "port": 8080,\n
-"raw_data": false,\n "verbose": false\n}\n```\n\n...and makes use of the same
-config options available to the CLI.\n\n### Multiple Gateways\n\nWhen using the
-configuration file, it is possible to define specific configuration\nparameters
-for multiple Ecowitt gateways. This is useful if different gateways
-should\npublish to different MQTT brokers, in different formats, etc.\n\nFirst,
-you must determine the unique ID for each gateway. This can be observed in
-the\nlogs when `verbose` is enabled â look for the `PASSKEY` value that the
-gateway has:\n\n```\nReceived data from the Ecowitt device: {\'PASSKEY\':
-\'abcde12345\', ...}\n```\n\nThen, in the configuration file, simply add a
-`gateways` key that contains a mapping of\nany of the existing configuration
-options (except for `--verbose` and `--diagnostics`,\nwhich can only be defined
-once and are applied to _every_ configuration). Options that\nremain at the
-root level of the file are treated as defaults.\n\nFor example, this YAML
-configuration file:\n\n```yaml\n---\nmqtt_broker: 127.0.0.1\nmqtt_password:
-password\nmqtt_topic: Test\nmqtt_username: user\n\ngateways:\n abcde12345:\n
-hass_discovery: true\n```\n\n...defines two gateway definitions:\n\n- One that
-publishes to the `Test` topic on an MQTT broker at `127.0.0.1`\n- One (with a
-`PASSKEY` of `abcde12345`) that publishes to the same broker, but in Home\n
-Assistant MQTT Discovery format.\n\nIn another example, this JSON configuration
-file:\n\n```json\n{\n "mqtt_broker": "127.0.0.1",\n "mqtt_password":
-"password",\n "mqtt_port": 1883,\n "mqtt_topic": "Test",\n "mqtt_username":
-"user",\n "gateways": {\n "abcde12345": {\n "mqtt_broker": "192.168.1.100",\n
-"mqtt_retain": true,\n "output_unit_system": "metric"\n }\n
-}\n}\n```\n\n...defines two gateway definitions:\n\n- One that publishes to the
-`Test` topic on an MQTT broker at `127.0.0.1`\n- One (with a `PASSKEY` of
-`abcde12345`) that publishes to a different broker\n (`192.168.1.100`), outputs
-the data in metric, and retains the data on the broker\n\n## Merging
-Configuration Options\n\nWhen parsing configuration options, `ecowitt2mqtt`
-looks at the configuration sources in\nthe following order:\n\n1. Configuration
-File (Specific Gateway)\n2. Configuration File (Defaults)\n3. Environment
-Variables\n4. CLI Options\n\nThis allows you to mix and match sources â for
-instance, you might have "defaults" in\nthe configuration file and override
-them via environment variables.\n\n## Input Data Formats\n\n`ecowitt2mqtt`
-currently supports the following input data formats:\n\n- `ambient_weather`\n-
-`ecowitt`\n\nProvide the correct one to `---input-data-format` based on which
-device brand you use.\n\n# Advanced Usage\n\n## Calculated Sensors\n\nIn
-addition to the data coming from a gateway, `ecowitt2mqtt` will automatically
-deduce\nand published several additional, calculated data points if the
-requisite underlying\ndata exists:\n\n- **[Absolute Humidity][absolute-
-humidity]:** the actual volume of water vapor in the\n air\n- **[Beaufort
-Scale][beaufort-scale]:** the empirical measure that relates wind speed to\n
-observed conditions at sea or on land\n- **[Dew Point][dew-point]:** the
-temperature to which air must be cooled to become\n saturated with water vapor,
-assuming constant air pressure and water content\n- **[Feels Like][heat-index]:
-** how hot or how cold the air feels to the human body when\n factoring in
-variables such as relative humidity, wind speeds, the amount of sunshine,\n
-etc.\n- **[Frost Point][frost-point]:** the temperature below 32Â°F (0Â°C) at
-which moisture in\n the air will condense as a layer of frost on exposed
-surfaces that are also at a\n temperature below the frost point\n- **[Frost
-Risk][frost-point]:** how likely the formation of frost is (based on the\n
-`frostpoint`)\n- **[Heat Index][heat-index]:** how hot the air feels to the
-human body when factoring\n in relative humidity (applicable when the apparent
-temperature is higher than the air\n temperature)\n- **[Humidex][humidex]:** an
-index number used by Canadian meteorologists to describe\n how hot the weather
-feels to the average person, by combining the effect of heat and\n humidity\n-
-**[Humidex Perception][humidex]:** a human-friendly interpretation of the
-Humidex\n- **Relative Strain Index:** a measure of discomfort resulting from
-the combined effect\n of temperature and humidity (applicable to heat stress of
-manual workers under shelter\n at various metabolic rates)\n- **Relative Strain
-Index Perception:** a human-friendly interpretation of the Relative\n Strain
-Index\n- **[Safe Exposure Times][safe-exposure-times]:** how long different
-skin types can be\n in the sun (unprotected) before burning begins according to
-the\n [Fitzpatrick Scale][fitzpatrick-scale]\n- **Solar Radiation (%):** the
-percentage of detected solar radiation illuminance as\n perceived by the human
-eye\n- **[Simmer Index][simmer-index]:** an alternative to heat index that
-describes how how\n the air feels to the human body in relatively dry
-environments\n- **[Simmer Zone][simmer-index]:** a human-friendly
-interpretation of the Simmer Index\n- **[Thermal Perception][dew-point]:** a
-human-friendly interpretation of the Dew Point\n- **[Wind Chill][wind-chill]:**
-how cold the air feels to the human body when factoring\n in relative humidity,
-wind speed, etc. (applicable when the apparent temperature is\n lower than the
-air temperature)\n\n(Special thanks to the excellent [`thermal_comfort`
-library][thermal-comfort-library] for\ninspiration on many of these.)\n\nIf you
-would prefer to not have these sensors calculated and published, you can
-utilize\nthe `--disable-calculated-data` configuration option.\n\n## Battery
-Configurations\n\nEcowitt devices report battery levels in three different
-formats:\n\n- `boolean`: `0` represents `OFF` (i.e., the battery is in normal
-condition) and `1` represents\n `ON` (i.e., the battery is low).\n- `numeric`:
-the raw numeric value is interpreted as the number of volts remaining in the\n
-battery.\n- `percentage`: the raw numeric value is interpreted as the
-percentage of voltage\n remaining the battery.\n\n`ecowitt2mqtt` provides three
-mechanisms to handle this complexity:\n\n1. A built-in mapping of all currently
-known battery types to their assumed strategy\n2. A default battery strategy
-for unknown battery types\n3. User-defined battery strategy overrides\n\n###
-Built-in Mapping\n\n`ecowitt2mqtt` contains an internal mapping that should
-automatically transform all\nknown battery types into their correct
-format.\n\n### Default Battery Strategy\n\nBy using the `--default-battery-
-strategy` configuration parameter, users can specify how\nunknown battery types
-should be treated by default.\n\n### Battery Overrides\n\nIndividual batteries
-can be overridden and given a new strategy. How this is\naccomplished differs
-slightly based on the configuration method used:\n\n- Command Line Options:
-provide one or more `--battery-override "batt1=boolean"` options\n- Environment
-Variables: provide a `ECOWITT2MQTT_BATTERY_OVERRIDE` variable that is a\n
-semicolon-delimited pair of "key=value" strings (e.g.,\n
-`ECOWITT2MQTT_BATTERY_OVERRIDE="batt1=boolean;batt2=numeric"`)\n- Config File:
-include a dictionary of key/value pairs in either YAML or JSON format\n\nThese
+Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2023.4.0 Summary: A small web
+server to send data from Ecowitt devices to an MQTT Broker Home-page: https://
+github.com/bachya/ecowitt2mqtt License: MIT Author: Aaron Bach Author-email:
+bachya1208@gmail.com Requires-Python: >=3.9.0,<4.0.0 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-Dist: asyncio-mqtt (>=0.12.1)
+Requires-Dist: colorlog (>=6.6.0,<7.0.0) Requires-Dist: fastapi
+(>=0.89.1,<0.96.0) Requires-Dist: meteocalc (>=1.1.0,<2.0.0) Requires-Dist:
+python-multipart (>=0.0.5,<0.0.7) Requires-Dist: rapidfuzz (>=2.13.0,<3.0.0)
+Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0) Requires-Dist: uvicorn
+(>=0.19.0) Requires-Dist: uvloop (>=0.17.0,<0.18.0) Requires-Dist: voluptuous
+(>=0.13.1,<0.14.0) Project-URL: Bug Tracker, https://github.com/bachya/
+ecowitt2mqtt/issues Project-URL: Changelog, https://github.com/bachya/
+ecowitt2mqtt/releases Project-URL: Repository, https://github.com/bachya/
+ecowitt2mqtt Description-Content-Type: text/markdown ![ecowitt2mqtt][logo] [!
+[CI][ci-badge]][ci] [![PyPI][pypi-badge]][pypi] [![Docker Hub][docker-hub-
+badge]][docker-hub] [![Version][version-badge]][version] [![License][license-
+badge]][license] [![Code Coverage][codecov-badge]][codecov] [![Maintainability]
+[maintainability-badge]][maintainability] [Buy_Me_A_Coffee] `ecowitt2mqtt` is a
+small CLI/web server that can receive data from Fine Offset weather stations
+(and their numerous white-labeled counterparts, like Ecowitt and Ambient
+Weather), adjust that data in numerous ways, and send it on to one or more MQTT
+brokers. - [Installation](#installation) - [Python Versions](#python-versions)
+- [Disclaimer](#disclaimer) - [Supported Brands](#supported-brands) - [Quick
+Start](#quick-start) - [Configuration](#configuration) - [Command Line Options]
+(#command-line-options) - [Environment Variables](#environment-variables) -
+[Configuration File](#configuration-file) - [Merging Configuration Options]
+(#merging-configuration-options) - [Input Data Formats](#input-data-formats) -
+[Advanced Usage](#advanced-usage) - [Calculated Sensors](#calculated-sensors) -
+[Battery Configurations](#battery-configurations) - [Unit Systems](#unit-
+systems) - [Raw Data](#raw-data) - [Home Assistant](#home-assistant) - [Running
+in the Background](#running-in-the-background) - [Docker](#docker) -
+[Diagnostics](#diagnostics) - [Contributing](#contributing) # Installation
+```bash pip install ecowitt2mqtt ``` # Python Versions `ecowitt2mqtt` is
+currently supported on: - Python 3.9 - Python 3.10 - Python 3.11 # Disclaimer
+The datapoints within this library and documentation constitute estimates and
+are intended to help informed decision making. They should not replace
+analysis, advice, or diagnosis from trained professionals. Use this data at
+your own discretion. # Supported Brands Despite the name of the library,
+`ecowitt2mqtt` should support any weather station/gateway that is produced by
+[Fine Offset](https://www.foshk.com/). This includes brands that white-label
+Fine Offset equipment, such as: - [Ambient Weather][ambient-weather] (U.S.) -
+[Ecowitt][ecowitt] (China, Hong Kong) - [Froggit][froggit] (Germany) ...and
+many others. For more information on how these brands relate to one another,
+see this forum post: https://www.wxforum.net/index.php?topic=40730.0 Although
+there are some small differences between how these various branded devices are
+configured, `ecowitt2mqtt` endeavors to incorporate them all with minimal
+effort on the user's part. # Quick Start First, install `ecowitt2mqtt` via
+`pip`: ```bash $ pip install ecowitt2mqtt ``` Next, if you haven't already,
+install the appropriate mobile app to configure your device. For example: -
+Ambient Weather: awnet ([iOS][awnet-ios]/[Android][awnet-google-play]) -
+Ecowitt: WS View ([iOS][ws-view-ios]/[Android][ws-view-google-play]) Find the
+appropriate location in the mobile app to configure a customized upload target
+for the station's data. This will differ depending on the app, but in general,
+you should select your device and find a screen entitled "Upload" (or similar).
+![The "Upload" screen in the awnet app][awnet-upload-screen] ![The "Upload"
+screen in the WS View app][ws-view-upload-screen] Fill out the form with the
+appropriate values and tap `Save`: - `Protocol Type Same As`: pick the label
+that matches your brand (e.g., `Ecowitt` for Ecowitt devices) - `Server IP /
+Hostname`: the IP address/hostname of the device running `ecowitt2mqtt` -
+`Path`: `/data/report/` (the default path used by most mobile apps) - `Port`:
+`8080` (the default port on which `ecowitt2mqtt` is served) - `Upload
+Interval`: 16 (a reasonable short number of seconds between publishes) Then, on
+the machine where you installed `ecowitt2mqtt`, run it: ```bash $ ecowitt2mqtt
+\ --mqtt-broker=192.168.1.101 \ --mqtt-username=user \ --mqtt-password=password
+\ --mqtt-topic=ecowitt2mqtt/device_1 --input-data-format=ecowitt ``` Within the
+`Upload Interval`, data should begin to appear in the MQTT broker. #
+Configuration `ecowitt2mqtt` can be configured via command line options,
+environment variables, or a (YAML or JSON) config file. ## Command Line Options
+``` usage: ecowitt2mqtt [-h] [--version] [--battery-override BATTERY_OVERRIDE]
+[-c config] [--default-battery-strategy default_battery_strategy] [--
+diagnostics] [--disable-calculated-data] [-e endpoint] [--hass-discovery] [--
+hass-discovery-prefix hass_discovery_prefix] [--hass-entity-id-prefix
+hass_entity_id_prefix] [--input-data-format input_data_format] [--input-unit-
+system input_unit_system] [-b mqtt_broker] [-p mqtt_password] [--mqtt-port
+mqtt_port] [--mqtt-retain] [--mqtt-tls] [-t mqtt_topic] [-u mqtt_username] [--
+output-unit-system output_unit_system] [--output-unit-accumulated-precipitation
+output_unit_accumulated_precipitation] [--output-unit-distance
+output_unit_distance] [--output-unit-humidity output_unit_humidity] [--output-
+unit-illuminance output_unit_illuminance] [--output-unit-precipitation-rate
+output_unit_precipitation_rate] [--output-unit-pressure output_unit_pressure]
+[--output-unit-speed output_unit_speed] [--output-unit-temperature
+output_unit_temperature] [--port port] [--precision precision] [--raw-data] [-
+v] Send data from an Ecowitt gateway to an MQTT broker optional arguments: -h,
+--help show this help message and exit --version show program's version number
+and exit --battery-override BATTERY_OVERRIDE A battery configuration override
+(format: key,value) -c config, --config config A path to a YAML or JSON config
+file --default-battery-strategy default_battery_strategy The default battery
+config strategy to use (default: boolean) --diagnostics Output diagnostics --
+disable-calculated-data Disable the output of calculated sensors -e endpoint, -
+-endpoint endpoint The relative endpoint/path to serve ecowitt2mqtt on
+(default: /data/report) --hass-discovery Publish data in the Home Assistant
+MQTT Discovery format --hass-discovery-prefix hass_discovery_prefix The Home
+Assistant MQTT Discovery topic prefix to use (default: homeassistant) --hass-
+entity-id-prefix hass_entity_id_prefix The prefix to use for Home Assistant
+entity IDs --input-data-format input_data_format The input data format used by
+the gateway (default: ecowitt) --input-unit-system input_unit_system The input
+unit system used by the gateway (default: imperial) -b mqtt_broker, --mqtt-
+broker mqtt_broker The hostname or IP address of an MQTT broker -
+p mqtt_password, --mqtt-password mqtt_password A valid password for the MQTT
+broker --mqtt-port mqtt_port The listenting port of the MQTT broker (default:
+1883) --mqtt-retain Instruct the MQTT broker to retain messages --mqtt-tls
+Enable MQTT over TLS -t mqtt_topic, --mqtt-topic mqtt_topic The MQTT topic to
+publish device data to -u mqtt_username, --mqtt-username mqtt_username A valid
+username for the MQTT broker --output-unit-system output_unit_system The output
+unit system used by the gateway (default: imperial) --output-unit-accumulated-
+precipitation output_unit_accumulated_precipitation The output unit to use for
+accumulated precipitation data points (default: the default used by the output
+unit system) --output-unit-distance output_unit_distance The output unit to use
+for distance data points (default: the default used by the output unit system)
+--output-unit-humidity output_unit_humidity The output unit to use for humidity
+data points (default: the default used by the output unit system) --output-
+unit-illuminance output_unit_illuminance The output unit to use for illuminance
+data points (default: the default used by the output unit system) --output-
+unit-precipitation-rate output_unit_precipitation_rate The output unit to use
+for precipitation rate data points (default: the default used by the output
+unit system) --output-unit-pressure output_unit_pressure The output unit to use
+for pressure data points (default: the default used by the output unit system)
+--output-unit-speed output_unit_speed The output unit to use for speed data
+points (default: the default used by the output unit system) --output-unit-
+temperature output_unit_temperature The output unit to use for temperature data
+points (default: the default used by the output unit system) --port port The
+port to serve ecowitt2mqtt on (default: 8080) --precision precision The
+precision to output data points at (default: no limit) --raw-data Return raw
+data (don't attempt to translate any values) -v, --verbose Increase verbosity
+of logged output ``` ## Environment Variables -
+`ECOWITT2MQTT_BATTERY_OVERRIDE`: a semicolon-delimited list of key=value
+battery overrides (default: `numeric`) - `ECOWITT2MQTT_CONFIG`: a path to a
+YAML or JSON config file (default: `None`) -
+`ECOWITT2MQTT_DEFAULT_BATTERY_STRATEGY`: the default battery config strategy to
+use (default: `boolean`) - `ECOWITT2MQTT_DIAGNOSTICS`: whether to output
+diagnostics (default: `false`) - `ECOWITT2MQTT_DISABLE_CALCULATED_DATA`:
+whether to disable the output of calculated sensors (default: `false`) -
+`ECOWITT2MQTT_ENDPOINT`: the relative endpoint/path to serve ecowitt2mqtt on
+(default: `/data/report`) - `ECOWITT2MQTT_HASS_DISCOVERY_PREFIX`: the Home
+Assistant discovery prefix to use (default: `homeassistant`) -
+`ECOWITT2MQTT_HASS_DISCOVERY`: publish data in the Home Assistant MQTT
+Discovery format (default: `false`) - `ECOWITT2MQTT_HASS_ENTITY_ID_PREFIX`: the
+prefix to use for Home Assistant entity IDs (default: `""`) -
+`ECOWITT2MQTT_INPUT_DATA_FORMAT`: the input data format used by the gateway
+(default: `ecowitt`) - `ECOWITT2MQTT_INPUT_UNIT_SYSTEM`: the input unit system
+used by the device (default: `imperial`) - `ECOWITT2MQTT_MQTT_BROKER`: the
+hostname or IP address of an MQTT broker - `ECOWITT2MQTT_MQTT_PASSWORD`: a
+valid password for the MQTT broker - `ECOWITT2MQTT_MQTT_PORT`: the listenting
+port of the MQTT broker (default: `1883`) - `ECOWITT2MQTT_MQTT_RETAIN`: whether
+to instruct the MQTT broker to retain messages (default: `false`) -
+`ECOWITT2MQTT_MQTT_TLS`: publish data via MQTT over TLS (default: `false`) -
+`ECOWITT2MQTT_MQTT_TOPIC`: the MQTT topic to publish device data to -
+`ECOWITT2MQTT_MQTT_USERNAME`: a valid username for the MQTT broker -
+`ECOWITT2MQTT_OUTPUT_UNIT_SYSTEM`: the unit system to use in output (default:
+`imperial`) - `ECOWITT2MQTT_OUTPUT_UNIT_TEMPERATURE`: the output unit to use
+for temperature data points (default: the default used by the output unit
+system) - `ECOWITT2MQTT_PORT`: the port to serve ecowitt2mqtt on (default:
+`8080`) - `ECOWITT2MQTT_PRECISION`: the precision to output data points at
+(default: no limit) - `ECOWITT2MQTT_RAW_DATA`: return raw data (don't attempt
+to translate any values) (default: `false`) - `ECOWITT2MQTT_VERBOSE`: increase
+verbosity of logged output (default: `false`) ## Configuration File The
+configuration file can be formatted as either YAML: ```yaml --
+- battery_override: battery_key1: boolean default_battery_strategy: numeric
+diagnostics: false disable_calculated_data: false endpoint: /data/report
+hass_discovery: false hass_discovery_prefix: homeassistant
+hass_entity_id_prefix: test_prefix input_data_format: ecowitt
+input_unit_system: imperial mqtt_broker: 127.0.0.1 mqtt_password: password
+mqtt_port: 1883 mqtt_retain: false mqtt_tls: false mqtt_topic: Test
+mqtt_username: user output_unit_system: imperial port: 8080 raw_data: false
+verbose: false ``` ...or JSON ```json { "battery_override": { "battery_key1":
+"boolean" }, "default_battery_strategy": "numeric", "diagnostics": false,
+"disable_calculated_data": false, "endpoint": "/data/report", "hass_discovery":
+false, "hass_discovery_prefix": "homeassistant", "hass_entity_id_prefix":
+"test_prefix" "input_data_format": "ecowitt", "input_unit_system": "imperial",
+"mqtt_broker": "127.0.0.1", "mqtt_password": "password", "mqtt_port": 1883,
+"mqtt_retain": true, "mqtt_tls": false, "mqtt_topic": "Test", "mqtt_username":
+"user", "output_unit_system": "imperial", "port": 8080, "raw_data": false,
+"verbose": false } ``` ...and makes use of the same config options available to
+the CLI. ### Multiple Gateways When using the configuration file, it is
+possible to define specific configuration parameters for multiple Ecowitt
+gateways. This is useful if different gateways should publish to different MQTT
+brokers, in different formats, etc. First, you must determine the unique ID for
+each gateway. This can be observed in the logs when `verbose` is enabled â
+look for the `PASSKEY` value that the gateway has: ``` Received data from the
+Ecowitt device: {'PASSKEY': 'abcde12345', ...} ``` Then, in the configuration
+file, simply add a `gateways` key that contains a mapping of any of the
+existing configuration options (except for `--verbose` and `--diagnostics`,
+which can only be defined once and are applied to _every_ configuration).
+Options that remain at the root level of the file are treated as defaults. For
+example, this YAML configuration file: ```yaml --- mqtt_broker: 127.0.0.1
+mqtt_password: password mqtt_topic: Test mqtt_username: user gateways:
+abcde12345: hass_discovery: true ``` ...defines two gateway definitions: - One
+that publishes to the `Test` topic on an MQTT broker at `127.0.0.1` - One (with
+a `PASSKEY` of `abcde12345`) that publishes to the same broker, but in Home
+Assistant MQTT Discovery format. In another example, this JSON configuration
+file: ```json { "mqtt_broker": "127.0.0.1", "mqtt_password": "password",
+"mqtt_port": 1883, "mqtt_topic": "Test", "mqtt_username": "user", "gateways":
+{ "abcde12345": { "mqtt_broker": "192.168.1.100", "mqtt_retain": true,
+"output_unit_system": "metric" } } } ``` ...defines two gateway definitions: -
+One that publishes to the `Test` topic on an MQTT broker at `127.0.0.1` - One
+(with a `PASSKEY` of `abcde12345`) that publishes to a different broker
+(`192.168.1.100`), outputs the data in metric, and retains the data on the
+broker ## Merging Configuration Options When parsing configuration options,
+`ecowitt2mqtt` looks at the configuration sources in the following order: 1.
+Configuration File (Specific Gateway) 2. Configuration File (Defaults) 3.
+Environment Variables 4. CLI Options This allows you to mix and match sources
+â for instance, you might have "defaults" in the configuration file and
+override them via environment variables. ## Input Data Formats `ecowitt2mqtt`
+currently supports the following input data formats: - `ambient_weather` -
+`ecowitt` Provide the correct one to `---input-data-format` based on which
+device brand you use. # Advanced Usage ## Calculated Sensors In addition to the
+data coming from a gateway, `ecowitt2mqtt` will automatically deduce and
+published several additional, calculated data points if the requisite
+underlying data exists: - **[Absolute Humidity][absolute-humidity]:** the
+actual volume of water vapor in the air - **[Beaufort Scale][beaufort-scale]:**
+the empirical measure that relates wind speed to observed conditions at sea or
+on land - **[Dew Point][dew-point]:** the temperature to which air must be
+cooled to become saturated with water vapor, assuming constant air pressure and
+water content - **[Feels Like][heat-index]:** how hot or how cold the air feels
+to the human body when factoring in variables such as relative humidity, wind
+speeds, the amount of sunshine, etc. - **[Frost Point][frost-point]:** the
+temperature below 32Â°F (0Â°C) at which moisture in the air will condense as a
+layer of frost on exposed surfaces that are also at a temperature below the
+frost point - **[Frost Risk][frost-point]:** how likely the formation of frost
+is (based on the `frostpoint`) - **[Heat Index][heat-index]:** how hot the air
+feels to the human body when factoring in relative humidity (applicable when
+the apparent temperature is higher than the air temperature) - **[Humidex]
+[humidex]:** an index number used by Canadian meteorologists to describe how
+hot the weather feels to the average person, by combining the effect of heat
+and humidity - **[Humidex Perception][humidex]:** a human-friendly
+interpretation of the Humidex - **Relative Strain Index:** a measure of
+discomfort resulting from the combined effect of temperature and humidity
+(applicable to heat stress of manual workers under shelter at various metabolic
+rates) - **Relative Strain Index Perception:** a human-friendly interpretation
+of the Relative Strain Index - **[Safe Exposure Times][safe-exposure-times]:**
+how long different skin types can be in the sun (unprotected) before burning
+begins according to the [Fitzpatrick Scale][fitzpatrick-scale] - **Solar
+Radiation (%):** the percentage of detected solar radiation illuminance as
+perceived by the human eye - **[Simmer Index][simmer-index]:** an alternative
+to heat index that describes how how the air feels to the human body in
+relatively dry environments - **[Simmer Zone][simmer-index]:** a human-friendly
+interpretation of the Simmer Index - **[Thermal Perception][dew-point]:** a
+human-friendly interpretation of the Dew Point - **[Wind Chill][wind-chill]:**
+how cold the air feels to the human body when factoring in relative humidity,
+wind speed, etc. (applicable when the apparent temperature is lower than the
+air temperature) (Special thanks to the excellent [`thermal_comfort` library]
+[thermal-comfort-library] for inspiration on many of these.) If you would
+prefer to not have these sensors calculated and published, you can utilize the
+`--disable-calculated-data` configuration option. ## Battery Configurations
+Ecowitt devices report battery levels in three different formats: - `boolean`:
+`0` represents `OFF` (i.e., the battery is in normal condition) and `1`
+represents `ON` (i.e., the battery is low). - `numeric`: the raw numeric value
+is interpreted as the number of volts remaining in the battery. - `percentage`:
+the raw numeric value is interpreted as the percentage of voltage remaining the
+battery. `ecowitt2mqtt` provides three mechanisms to handle this complexity: 1.
+A built-in mapping of all currently known battery types to their assumed
+strategy 2. A default battery strategy for unknown battery types 3. User-
+defined battery strategy overrides ### Built-in Mapping `ecowitt2mqtt` contains
+an internal mapping that should automatically transform all known battery types
+into their correct format. ### Default Battery Strategy By using the `--
+default-battery-strategy` configuration parameter, users can specify how
+unknown battery types should be treated by default. ### Battery Overrides
+Individual batteries can be overridden and given a new strategy. How this is
+accomplished differs slightly based on the configuration method used: - Command
+Line Options: provide one or more `--battery-override "batt1=boolean"` options
+- Environment Variables: provide a `ECOWITT2MQTT_BATTERY_OVERRIDE` variable
+that is a semicolon-delimited pair of "key=value" strings (e.g.,
+`ECOWITT2MQTT_BATTERY_OVERRIDE="batt1=boolean;batt2=numeric"`) - Config File:
+include a dictionary of key/value pairs in either YAML or JSON format These
 overrides work on both known and unknown battery types; that said, if you
-should\nfind the need to override a known battery type because `ecowitt2mqtt`
-has an incorrect\ninternal interpretation, submit an issue to get it
-corrected!\n\n### Example\n\nIn this example, a user mostly has batteries that
-should be treated as `boolean`, but\nalso has one â `wh60_batt1` â that
-should be treated as numeric.\n\n#### Command Line Options\n\n```\n$
-ecowitt2mqtt --default-battery-strategy boolean --battery-
-override="wh60_batt1=numeric"\n```\n\n#### Environment Variables\n\n```\n$
-ECOWITT2MQTT_DEFAULT_BATTERY_STRATEGY=boolean \\\n
-ECOWITT2MQTT_BATTERY_OVERRIDE="wh60_batt1=numeric" \\\n
-ecowitt2mqtt\n```\n\n#### Config File\n\nIn YAML:\n\n```yaml\n---
-\ndefault_battery_strategy: boolean\nbattery_override:\n wh60_batt1:
-numeric\n```\n\n...or JSON\n\n```json\n{\n "default_battery_strategy":
-"boolean",\n "battery_override": {\n "wh60_batt1": "numeric"\n }\n}\n```\n\n##
-Unit Systems\n\n### Input and Output\n\n`ecowitt2mqtt` allows you to specify
-both the input and output unit systems for a device\nvia the `--input-unit-
-system` and `--output-unit-system` config options, respectively.\nThese are
-fairly self-explanatory, but take care to use an `--input-unit-system` that
-is\nconsistent with what your device provides (otherwise, your data will be
-very "off").\n\n### Overriding Units for Data Categories\n\nIf you wish, you
-can change the unit for individual data categories. For example, let\'s\nsay
-you wanted to use metric for the output unit system, but wanted to represent
-all\ntemperature data points in Kelvin â you would provide `--output-unit-
-system=metric` and\n`--output-unit-temperature=K` as config options. As
-expected, the value is properly\nconverted to the new unit.\n\n#### Accumulated
-Precipitation\n\nConfig Option: `--output-unit-accumulated-precipitation`\n\n-
-`in`\n- `mm`\n\n#### Absolute Humidity\n\nConfig Option: `--output-unit-
-humidity`\n\n- `g/mÂ³`\n- `lbs/ftÂ³`\n\n#### Illuminance\n\nConfig Option: `--
-output-unit-illuminance`\n\n- `fc`\n- `kfc`\n- `klx`\n- `lx`\n- `W/mÂ²`\n\n####
-Precipitation Rate\n\nConfig Option: `--output-unit-precipitation-rate`\n\n-
-`in/h`\n- `mm/h`\n\n#### Pressure\n\nConfig Option: `--output-unit-
-pressure`\n\n- `bar`\n- `cbar`\n- `hPa`\n- `inHg`\n- `kPa`\n- `mbar`\n-
-`mmHg`\n- `Pa`\n- `psi`\n\n#### Speed\n\nConfig Option: `--output-unit-
-speed`\n\n- `ft/s`\n- `in/d`\n- `in/h`\n- `km/h`\n- `kn`\n- `m/s`\n- `mph`\n-
-`mm/d`\n\n#### Temperature\n\nConfig Option: `--output-unit-temperature`\n\n-
-`Â°C`\n- `Â°F`\n- `K`\n\n## Raw Data\n\nIn some cases, it may be preferable to
-prevent `ecowitt2mqtt` from doing any data\ntranslation (converting values to a
-new unit system, changing binary values â such as\nmight be used by a battery
-â into "friendly" values, etc.). Passing the `--raw-data` flag\nwill
-accomplish this: data will flow directly from the Ecowitt device to the MQTT
-broker\nas-is.\n\nNote that the `--raw-data` flag supersedes any that might
-cause data translation (such as\n`--input-unit-system` or `--output-unit-
-system`).\n\n## Home Assistant\n\n### MQTT Discovery\n\n[Home Assistant][home-
-assistant] users can quickly add entities from an Ecowitt device\nby using
-[MQTT Discovery][home-assistant-mqtt-discovery]. Once Home Assistant
-is\nconfigured to accept MQTT Discovery, `ecowitt2mqtt` simply needs the `--
-hass-discovery`\nflag:\n\n```bash\n$ ecowitt2mqtt \\\n --mqtt-
-broker=192.168.1.101 \\\n --mqtt-username=user \\\n --mqtt-password=password
-\\\n --hass-discovery\n```\n\n### Custom Entity ID Prefix\n\nYou can provide a
-custom prefix for all Home Assistant entities via the\n`--hass-entity-id-
-prefix` config parameter.\n\n### Home Assistant OS Add-on\n\nHome Assistant OS
-users can install the official `ecowitt2mqtt` add-on by clicking the\nlink
-below:\n\n[![Home Assistant Add-on][home-assistant-addon-badge]][home-
-assistant-addon]\n\n## Running in the Background\n\n`ecowitt2mqtt` doesn\'t,
-itself, provide any sort of daemonization mechanism. The suggested\nroute is to
-use a different application.\n\n### `supervisord`\n\nAn example `supervisord`
-configuration file might look like this:\n\n```\n
-[supervisord]\nnodaemon=true\nloglevel=info\nuser=root\n\n[program:
-ecowitt2mqtt]\ncommand=ecowitt2mqtt --mqtt-broker=192.168.1.101 --mqtt-
-username=user --mqtt-password=password\nstdout_logfile=/dev/
-stdout\nstdout_logfile_maxbytes=0\nredirect_stderr=true\n```\n\n###
-`systemd`\n\nAn example `systemd` service file in `/etc/systemd/system` might
-look like this:\n\n```\n[Unit]\nDescription=ECOWITT2MQTT
-daemon\nAfter=network.target\n\n[Service]\nType=simple\nExecStart=ecowitt2mqtt
---mqtt-broker=192.168.1.101 --mqtt-username=user --mqtt-
-password=password\nExecReload=kill -HUP $MAINPID\nKillMode=process\nRestart=on-
-failure\nRestartSec=5s\n\n[Install]\nWantedBy=multi-user.target\n```\n\nTo
-enable the service:\n\n```bash\n$ systemctl enable ecowitt2mqtt\n```\n\n##
-Docker\n\nThe library is available via a Docker image from both [Docker Hub]
-[docker-hub] and\n[ghcr.io][ghcr]. It is configured by using the same
-environment variables listed\n[above](#environment-variables).\n\nRunning the
-image is straightforward:\n\n```\ndocker run -it \\\n -
-e ECOWITT2MQTT_MQTT_BROKER=192.168.1.101 \\\n -
-e ECOWITT2MQTT_MQTT_USERNAME=user \\\n -e ECOWITT2MQTT_MQTT_PASSWORD=password
-\\\n -p 8080:8080 \\\n bachya/ecowitt2mqtt:latest\n```\n\nNote the value of the
-`-p` flag: you must expose the port defined by the `PORT`\nenvironment
-variable. In the example above, the default port (`8080`) is used and
-is\nexposed via the same port on the host.\n\n[`docker-compose`][docker-
-compose] users can find an example configuration file at\n[`docker-
-compose.dev.yml`](docker-compose.dev.yml). Note that this is intended to be a
-dev\nenvironment for quickly testing the repo itself; in production, you should
-refer to one\nof the published images.\n\n# Diagnostics\n\nYou may run
-`ecowitt2mqtt` in diagnostics mode by providing the `--diagnostics` flag.
-In\nthis mode, the app will wait until it receives and publishes a single
-payload, then\nexit. This allows users to collect a small-but-complete payload
-for use in testing,\ndebugging, and issue reporting.\n\n#
-Contributing\n\nThanks to all of [our contributors][contributors] so far!\n\n1.
-[Check for open features/bugs][issues] or [initiate a discussion on one][new-
-issue].\n2. [Fork the repository][fork].\n3. (_optional, but highly
-recommended_) Create a virtual environment: `python3 -m venv .venv`\n4.
-(_optional, but highly recommended_) Enter the virtual environment: `source
-./.venv/bin/activate`\n5. Install the dev environment: `script/setup`\n6. Code
-your new feature or bug fix on a new branch.\n7. Write tests that cover your
-new functionality.\n8. Run tests and ensure 100% code coverage: `poetry run
-pytest --cov ecowitt2mqtt tests`\n9. Update `README.md` with any new
-documentation.\n10. Submit a pull request!\n\n[absolute-humidity]: https://
-en.wikipedia.org/wiki/Humidity#Absolute_humidity\n[ambient-weather]: https://
-ambientweather.com/\n[awnet-google-play]: https://play.google.com/store/apps/
-details?id=com.dtston.ambienttoolplus&hl=en_US&gl=US\n[awnet-ios]: https://
-apps.apple.com/us/app/awnet/id1341994564\n[awnet-upload-screen]: resources/
-awnet-upload-screen.jpeg?raw=true\n[beaufort-scale]: https://en.wikipedia.org/
-wiki/Beaufort_scale\n[ci-badge]: https://github.com/bachya/ecowitt2mqtt/
-workflows/CI/badge.svg\n[ci]: https://github.com/bachya/ecowitt2mqtt/actions\n
+should find the need to override a known battery type because `ecowitt2mqtt`
+has an incorrect internal interpretation, submit an issue to get it corrected!
+### Example In this example, a user mostly has batteries that should be treated
+as `boolean`, but also has one â `wh60_batt1` â that should be treated as
+numeric. #### Command Line Options ``` $ ecowitt2mqtt --default-battery-
+strategy boolean --battery-override="wh60_batt1=numeric" ``` #### Environment
+Variables ``` $ ECOWITT2MQTT_DEFAULT_BATTERY_STRATEGY=boolean \
+ECOWITT2MQTT_BATTERY_OVERRIDE="wh60_batt1=numeric" \ ecowitt2mqtt ``` ####
+Config File In YAML: ```yaml --- default_battery_strategy: boolean
+battery_override: wh60_batt1: numeric ``` ...or JSON ```json
+{ "default_battery_strategy": "boolean", "battery_override": { "wh60_batt1":
+"numeric" } } ``` ## Unit Systems ### Input and Output `ecowitt2mqtt` allows
+you to specify both the input and output unit systems for a device via the `--
+input-unit-system` and `--output-unit-system` config options, respectively.
+These are fairly self-explanatory, but take care to use an `--input-unit-
+system` that is consistent with what your device provides (otherwise, your data
+will be very "off"). ### Overriding Units for Data Categories If you wish, you
+can change the unit for individual data categories. For example, let's say you
+wanted to use metric for the output unit system, but wanted to represent all
+temperature data points in Kelvin â you would provide `--output-unit-
+system=metric` and `--output-unit-temperature=K` as config options. As
+expected, the value is properly converted to the new unit. #### Accumulated
+Precipitation Config Option: `--output-unit-accumulated-precipitation` - `in` -
+`mm` #### Absolute Humidity Config Option: `--output-unit-humidity` - `g/mÂ³` -
+`lbs/ftÂ³` #### Illuminance Config Option: `--output-unit-illuminance` - `fc` -
+`kfc` - `klx` - `lx` - `W/mÂ²` #### Precipitation Rate Config Option: `--
+output-unit-precipitation-rate` - `in/h` - `mm/h` #### Pressure Config Option:
+`--output-unit-pressure` - `bar` - `cbar` - `hPa` - `inHg` - `kPa` - `mbar` -
+`mmHg` - `Pa` - `psi` #### Speed Config Option: `--output-unit-speed` - `ft/s`
+- `in/d` - `in/h` - `km/h` - `kn` - `m/s` - `mph` - `mm/d` #### Temperature
+Config Option: `--output-unit-temperature` - `Â°C` - `Â°F` - `K` ## Raw Data In
+some cases, it may be preferable to prevent `ecowitt2mqtt` from doing any data
+translation (converting values to a new unit system, changing binary values â
+such as might be used by a battery â into "friendly" values, etc.). Passing
+the `--raw-data` flag will accomplish this: data will flow directly from the
+Ecowitt device to the MQTT broker as-is. Note that the `--raw-data` flag
+supersedes any that might cause data translation (such as `--input-unit-system`
+or `--output-unit-system`). ## Home Assistant ### MQTT Discovery [Home
+Assistant][home-assistant] users can quickly add entities from an Ecowitt
+device by using [MQTT Discovery][home-assistant-mqtt-discovery]. Once Home
+Assistant is configured to accept MQTT Discovery, `ecowitt2mqtt` simply needs
+the `--hass-discovery` flag: ```bash $ ecowitt2mqtt \ --mqtt-
+broker=192.168.1.101 \ --mqtt-username=user \ --mqtt-password=password \ --
+hass-discovery ``` ### Custom Entity ID Prefix You can provide a custom prefix
+for all Home Assistant entities via the `--hass-entity-id-prefix` config
+parameter. ### Home Assistant OS Add-on Home Assistant OS users can install the
+official `ecowitt2mqtt` add-on by clicking the link below: [![Home Assistant
+Add-on][home-assistant-addon-badge]][home-assistant-addon] ## Running in the
+Background `ecowitt2mqtt` doesn't, itself, provide any sort of daemonization
+mechanism. The suggested route is to use a different application. ###
+`supervisord` An example `supervisord` configuration file might look like this:
+``` [supervisord] nodaemon=true loglevel=info user=root [program:ecowitt2mqtt]
+command=ecowitt2mqtt --mqtt-broker=192.168.1.101 --mqtt-username=user --mqtt-
+password=password stdout_logfile=/dev/stdout stdout_logfile_maxbytes=0
+redirect_stderr=true ``` ### `systemd` An example `systemd` service file in `/
+etc/systemd/system` might look like this: ``` [Unit] Description=ECOWITT2MQTT
+daemon After=network.target [Service] Type=simple ExecStart=ecowitt2mqtt --
+mqtt-broker=192.168.1.101 --mqtt-username=user --mqtt-password=password
+ExecReload=kill -HUP $MAINPID KillMode=process Restart=on-failure RestartSec=5s
+[Install] WantedBy=multi-user.target ``` To enable the service: ```bash $
+systemctl enable ecowitt2mqtt ``` ## Docker The library is available via a
+Docker image from both [Docker Hub][docker-hub] and [ghcr.io][ghcr]. It is
+configured by using the same environment variables listed [above](#environment-
+variables). Running the image is straightforward: ``` docker run -it \ -
+e ECOWITT2MQTT_MQTT_BROKER=192.168.1.101 \ -e ECOWITT2MQTT_MQTT_USERNAME=user \
+-e ECOWITT2MQTT_MQTT_PASSWORD=password \ -p 8080:8080 \ bachya/ecowitt2mqtt:
+latest ``` Note the value of the `-p` flag: you must expose the port defined by
+the `PORT` environment variable. In the example above, the default port
+(`8080`) is used and is exposed via the same port on the host. [`docker-
+compose`][docker-compose] users can find an example configuration file at
+[`docker-compose.dev.yml`](docker-compose.dev.yml). Note that this is intended
+to be a dev environment for quickly testing the repo itself; in production, you
+should refer to one of the published images. # Diagnostics You may run
+`ecowitt2mqtt` in diagnostics mode by providing the `--diagnostics` flag. In
+this mode, the app will wait until it receives and publishes a single payload,
+then exit. This allows users to collect a small-but-complete payload for use in
+testing, debugging, and issue reporting. # Contributing Thanks to all of [our
+contributors][contributors] so far! 1. [Check for open features/bugs][issues]
+or [initiate a discussion on one][new-issue]. 2. [Fork the repository][fork].
+3. (_optional, but highly recommended_) Create a virtual environment: `python3
+-m venv .venv` 4. (_optional, but highly recommended_) Enter the virtual
+environment: `source ./.venv/bin/activate` 5. Install the dev environment:
+`script/setup` 6. Code your new feature or bug fix on a new branch. 7. Write
+tests that cover your new functionality. 8. Run tests and ensure 100% code
+coverage: `poetry run pytest --cov ecowitt2mqtt tests` 9. Update `README.md`
+with any new documentation. 10. Submit a pull request! [absolute-humidity]:
+https://en.wikipedia.org/wiki/Humidity#Absolute_humidity [ambient-weather]:
+https://ambientweather.com/ [awnet-google-play]: https://play.google.com/store/
+apps/details?id=com.dtston.ambienttoolplus&hl=en_US&gl=US [awnet-ios]: https://
+apps.apple.com/us/app/awnet/id1341994564 [awnet-upload-screen]: resources/
+awnet-upload-screen.jpeg?raw=true [beaufort-scale]: https://en.wikipedia.org/
+wiki/Beaufort_scale [ci-badge]: https://github.com/bachya/ecowitt2mqtt/
+workflows/CI/badge.svg [ci]: https://github.com/bachya/ecowitt2mqtt/actions
 [codecov-badge]: https://codecov.io/gh/bachya/ecowitt2mqtt/branch/dev/graph/
-badge.svg\n[codecov]: https://codecov.io/gh/bachya/ecowitt2mqtt\n[coffee-
-image]: https://cdn.buymeacoffee.com/buttons/default-orange.png\n[coffee]:
-https://www.buymeacoffee.com/bachya1208P\n[contributors]: https://github.com/
-bachya/ecowitt2mqtt/graphs/contributors\n[dew-point]: https://en.wikipedia.org/
-wiki/Dew_point\n[docker-compose]: https://docs.docker.com/compose/\n[docker-
-hub-badge]: https://img.shields.io/docker/pulls/bachya/ecowitt2mqtt\n[docker-
-hub]: https://hub.docker.com/r/bachya/ecowitt2mqtt\n[ecowitt]: https://
-www.ecowitt.com/\n[fitzpatrick-scale]: https://en.wikipedia.org/wiki/
-Fitzpatrick_scale\n[fork]: https://github.com/bachya/ecowitt2mqtt/fork\n
-[froggit]: https://www.froggit.de/Weather-Station/\n[frost-point]: https://
-en.wikipedia.org/wiki/Dew_point#Frost_point\n[ghcr]: https://ghcr.io/bachya/
-ecowitt2mqtt\n[heat-index]: https://en.wikipedia.org/wiki/Heat_index\n[home-
+badge.svg [codecov]: https://codecov.io/gh/bachya/ecowitt2mqtt [coffee-image]:
+https://cdn.buymeacoffee.com/buttons/default-orange.png [coffee]: https://
+www.buymeacoffee.com/bachya1208P [contributors]: https://github.com/bachya/
+ecowitt2mqtt/graphs/contributors [dew-point]: https://en.wikipedia.org/wiki/
+Dew_point [docker-compose]: https://docs.docker.com/compose/ [docker-hub-
+badge]: https://img.shields.io/docker/pulls/bachya/ecowitt2mqtt [docker-hub]:
+https://hub.docker.com/r/bachya/ecowitt2mqtt [ecowitt]: https://
+www.ecowitt.com/ [fitzpatrick-scale]: https://en.wikipedia.org/wiki/
+Fitzpatrick_scale [fork]: https://github.com/bachya/ecowitt2mqtt/fork
+[froggit]: https://www.froggit.de/Weather-Station/ [frost-point]: https://
+en.wikipedia.org/wiki/Dew_point#Frost_point [ghcr]: https://ghcr.io/bachya/
+ecowitt2mqtt [heat-index]: https://en.wikipedia.org/wiki/Heat_index [home-
 assistant-addon-badge]: https://my.home-assistant.io/badges/
-supervisor_addon.svg\n[home-assistant-addon]: https://my.home-assistant.io/
+supervisor_addon.svg [home-assistant-addon]: https://my.home-assistant.io/
 redirect/supervisor_addon/
 ?addon=c35f0383_ecowitt2mqtt&repository_url=https%3A%2F%2Fgithub.com%2Fbachya%2Fhome-
-assistant-addons\n[home-assistant-mqtt-discovery]: https://www.home-
-assistant.io/docs/mqtt/discovery/\n[home-assistant]: https://home-
-assistant.io\n[humidex]: https://en.wikipedia.org/wiki/Humidex\n[issues]:
-https://github.com/bachya/ecowitt2mqtt/issues\n[license-badge]: https://
-img.shields.io/pypi/l/ecowitt2mqtt.svg\n[license]: https://github.com/bachya/
-ecowitt2mqtt/blob/main/LICENSE\n[logo]: resources/logo-full.png\n
-[maintainability-badge]: https://api.codeclimate.com/v1/badges/
-a03c9e96f19a3dc37f98/maintainability\n[maintainability]: https://
-codeclimate.com/github/bachya/ecowitt2mqtt/maintainability\n[new-issue]: https:
-//github.com/bachya/ecowitt2mqtt/issues/new\n[pypi-badge]: https://
-img.shields.io/pypi/v/ecowitt2mqtt.svg\n[pypi]: https://pypi.python.org/pypi/
-ecowitt2mqtt\n[safe-exposure-times]: https://www.openuv.io/kb/skin-types-safe-
-exposure-time-calculation/\n[simmer-index]: http://summersimmer.com/
-ssi_page2.htm\n[thermal-comfort-library]: https://github.com/dolezsa/
-thermal_comfort\n[version-badge]: https://img.shields.io/pypi/pyversions/
-ecowitt2mqtt.svg\n[version]: https://pypi.python.org/pypi/ecowitt2mqtt\n[wind-
-chill]: https://en.wikipedia.org/wiki/Wind_chill\n[ws-view-google-play]: https:
-//play.google.com/store/apps/details?id=com.ost.wsview&gl=US\n[ws-view-ios]:
-https://apps.apple.com/us/app/ws-view/id1362944193\n[ws-view-upload-screen]:
-resources/ws-view-upload-screen.jpeg?raw=true\n', 'author': 'Aaron Bach',
-'author_email': 'bachya1208@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/bachya/ecowitt2mqtt',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'entry_points': entry_points, 'python_requires':
-'>=3.9.0,<4.0.0', } setup(**setup_kwargs)
+assistant-addons [home-assistant-mqtt-discovery]: https://www.home-
+assistant.io/docs/mqtt/discovery/ [home-assistant]: https://home-assistant.io
+[humidex]: https://en.wikipedia.org/wiki/Humidex [issues]: https://github.com/
+bachya/ecowitt2mqtt/issues [license-badge]: https://img.shields.io/pypi/l/
+ecowitt2mqtt.svg [license]: https://github.com/bachya/ecowitt2mqtt/blob/main/
+LICENSE [logo]: resources/logo-full.png [maintainability-badge]: https://
+api.codeclimate.com/v1/badges/a03c9e96f19a3dc37f98/maintainability
+[maintainability]: https://codeclimate.com/github/bachya/ecowitt2mqtt/
+maintainability [new-issue]: https://github.com/bachya/ecowitt2mqtt/issues/new
+[pypi-badge]: https://img.shields.io/pypi/v/ecowitt2mqtt.svg [pypi]: https://
+pypi.python.org/pypi/ecowitt2mqtt [safe-exposure-times]: https://www.openuv.io/
+kb/skin-types-safe-exposure-time-calculation/ [simmer-index]: http://
+summersimmer.com/ssi_page2.htm [thermal-comfort-library]: https://github.com/
+dolezsa/thermal_comfort [version-badge]: https://img.shields.io/pypi/
+pyversions/ecowitt2mqtt.svg [version]: https://pypi.python.org/pypi/
+ecowitt2mqtt [wind-chill]: https://en.wikipedia.org/wiki/Wind_chill [ws-view-
+google-play]: https://play.google.com/store/apps/
+details?id=com.ost.wsview&gl=US [ws-view-ios]: https://apps.apple.com/us/app/
+ws-view/id1362944193 [ws-view-upload-screen]: resources/ws-view-upload-
+screen.jpeg?raw=true
```

