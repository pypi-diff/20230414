# Comparing `tmp/pysolarfocus-3.6.2.tar.gz` & `tmp/pysolarfocus-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysolarfocus-3.6.2.tar", max compression
+gzip compressed data, was "pysolarfocus-3.6.3.tar", max compression
```

## Comparing `pysolarfocus-3.6.2.tar` & `pysolarfocus-3.6.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/LICENSE
--rw-r--r--   0        0        0     3183 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/README.md
--rw-r--r--   0        0        0      580 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/pyproject.toml
--rw-r--r--   0        0        0     5601 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/pysolarfocus/__init__.py
--rw-r--r--   0        0        0     3495 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/pysolarfocus/component_factory.py
--rw-r--r--   0        0        0        0 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/pysolarfocus/components/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/__init__.py
--rw-r--r--   0        0        0     9390 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/component.py
--rw-r--r--   0        0        0     2840 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/data_value.py
--rw-r--r--   0        0        0      159 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/enums.py
--rw-r--r--   0        0        0      205 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/part.py
--rw-r--r--   0        0        0      784 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/performance_calculator.py
--rw-r--r--   0        0        0      133 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/register_slice.py
--rw-r--r--   0        0        0      872 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/boiler.py
--rw-r--r--   0        0        0     1474 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/buffer.py
--rw-r--r--   0        0        0      292 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/fresh_water_module.py
--rw-r--r--   0        0        0     2650 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/heat_pump.py
--rw-r--r--   0        0        0     1827 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/heating_circuit.py
--rw-r--r--   0        0        0     1877 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/pellets_boiler.py
--rw-r--r--   0        0        0      800 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/photovoltaic.py
--rw-r--r--   0        0        0     1054 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/solar.py
--rw-r--r--   0        0        0     2965 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/const.py
--rw-r--r--   0        0        0     4027 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/modbus_wrapper.py
--rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 pysolarfocus-3.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/LICENSE
+-rw-r--r--   0        0        0     3183 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/README.md
+-rw-r--r--   0        0        0      580 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5469 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/__init__.py
+-rw-r--r--   0        0        0     3495 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/component_factory.py
+-rw-r--r--   0        0        0        0 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/__init__.py
+-rw-r--r--   0        0        0     9390 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/component.py
+-rw-r--r--   0        0        0     2840 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/data_value.py
+-rw-r--r--   0        0        0      159 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/enums.py
+-rw-r--r--   0        0        0      205 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/part.py
+-rw-r--r--   0        0        0      784 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/performance_calculator.py
+-rw-r--r--   0        0        0      133 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/register_slice.py
+-rw-r--r--   0        0        0      872 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/boiler.py
+-rw-r--r--   0        0        0     1474 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/buffer.py
+-rw-r--r--   0        0        0      292 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/fresh_water_module.py
+-rw-r--r--   0        0        0     2650 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/heat_pump.py
+-rw-r--r--   0        0        0     1827 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/heating_circuit.py
+-rw-r--r--   0        0        0     1877 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/pellets_boiler.py
+-rw-r--r--   0        0        0      800 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/photovoltaic.py
+-rw-r--r--   0        0        0     1054 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/solar.py
+-rw-r--r--   0        0        0     2965 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/const.py
+-rw-r--r--   0        0        0     4027 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/modbus_wrapper.py
+-rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 pysolarfocus-3.6.3/PKG-INFO
```

### Comparing `pysolarfocus-3.6.2/LICENSE` & `pysolarfocus-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/README.md` & `pysolarfocus-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pyproject.toml` & `pysolarfocus-3.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "pysolarfocus"
-version = "3.6.2"
+version = "3.6.3"
 description = "Unofficial, local Solarfocus client"
 authors = ["Jeroen Laverman <jjlaverman@web.de>"]
 license = "Apache-2.0"
 homepage = "https://github.com/lavermanjj/pysolarfocus"
 repository = "https://github.com/lavermanjj/pysolarfocus"
 keywords = ["solarfocus", "api client"]
 include = ["LICENSE"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pymodbus = "2.5.3"
+pymodbus = "3.2.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pysolarfocus-3.6.2/pysolarfocus/__init__.py` & `pysolarfocus-3.6.3/pysolarfocus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Python client lib for Solarfocus"""
-__version__ = "3.6.2"
+__version__ = "3.6.3"
 
 from enum import Enum
 from packaging import version
 
 #Default port for modbus
 PORT = 502
 
@@ -85,15 +85,15 @@
         return self.__conn.connect()
 
     @property
     def is_connected(self)->bool:
         """Check if connection is established"""
         return self.__conn.is_connected
     
-    def update(self):
+    def update(self) -> bool:
         """Read values from Heating System"""
         if (
             self.update_heating()
             and self.update_buffer()
             and self.update_boiler()
             and self.update_heatpump()
             and self.update_photovoltaic()
@@ -131,27 +131,23 @@
             for fresh_water_module in self.fresh_water_modules:
                 if not fresh_water_module.update():
                     return False
         return True
 
     def update_heatpump(self) -> bool:
         """Read values from Heating System"""
-        if self._system is Systems.Vampair:
-            return self.heatpump.update()
-        return True
+        return self.heatpump.update()
 
     def update_photovoltaic(self) -> bool:
         """Read values from Heating System"""
         return self.photovoltaic.update()
 
     def update_pelletsboiler(self) -> bool:
         """Read values from Pellets boiler"""
-        if self._system is Systems.Therminator:
-            return self.pelletsboiler.update()
-        return True
+        return self.pelletsboiler.update()
     
     def update_solar(self) -> bool:
         """Read values from Solar"""
         return self.solar.update()
     
     
     def __repr__(self) -> str:
```

### Comparing `pysolarfocus-3.6.2/pysolarfocus/component_factory.py` & `pysolarfocus-3.6.3/pysolarfocus/component_factory.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/components/base/component.py` & `pysolarfocus-3.6.3/pysolarfocus/components/base/component.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/components/base/data_value.py` & `pysolarfocus-3.6.3/pysolarfocus/components/base/data_value.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/components/base/performance_calculator.py` & `pysolarfocus-3.6.3/pysolarfocus/components/base/performance_calculator.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/components/boiler.py` & `pysolarfocus-3.6.3/pysolarfocus/components/boiler.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/components/buffer.py` & `pysolarfocus-3.6.3/pysolarfocus/components/buffer.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/components/heat_pump.py` & `pysolarfocus-3.6.3/pysolarfocus/components/heat_pump.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/components/heating_circuit.py` & `pysolarfocus-3.6.3/pysolarfocus/components/heating_circuit.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/components/pellets_boiler.py` & `pysolarfocus-3.6.3/pysolarfocus/components/pellets_boiler.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/components/photovoltaic.py` & `pysolarfocus-3.6.3/pysolarfocus/components/photovoltaic.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/components/solar.py` & `pysolarfocus-3.6.3/pysolarfocus/components/solar.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/const.py` & `pysolarfocus-3.6.3/pysolarfocus/const.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/pysolarfocus/modbus_wrapper.py` & `pysolarfocus-3.6.3/pysolarfocus/modbus_wrapper.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.2/PKG-INFO` & `pysolarfocus-3.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pysolarfocus
-Version: 3.6.2
+Version: 3.6.3
 Summary: Unofficial, local Solarfocus client
 Home-page: https://github.com/lavermanjj/pysolarfocus
 License: Apache-2.0
 Keywords: solarfocus,api client
 Author: Jeroen Laverman
 Author-email: jjlaverman@web.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pymodbus (==2.5.3)
+Requires-Dist: pymodbus (==3.2.2)
 Project-URL: Repository, https://github.com/lavermanjj/pysolarfocus
 Description-Content-Type: text/markdown
 
 # pysolarfocus: Python Client for Solarfocus eco<sup>_manager-touch_</sup>
 
 Python client library to interact with heating systems of [Solarfocus](https://www.solarfocus.com/) (eco<sup>_manager-touch_</sup> and thermi<sup>nator</sup> II) via Modbus TCP. This library has been developed for the integration into [Home-Assistant](https://www.home-assistant.io/) via a [custom integration](https://github.com/LavermanJJ/home-assistant-solarfocus), but can be used indepdently.
```

