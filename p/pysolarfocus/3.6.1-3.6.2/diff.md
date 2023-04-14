# Comparing `tmp/pysolarfocus-3.6.1.tar.gz` & `tmp/pysolarfocus-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysolarfocus-3.6.1.tar", max compression
+gzip compressed data, was "pysolarfocus-3.6.2.tar", max compression
```

## Comparing `pysolarfocus-3.6.1.tar` & `pysolarfocus-3.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-03-29 17:56:25.720715 pysolarfocus-3.6.1/LICENSE
--rw-r--r--   0        0        0     3182 2023-03-29 17:56:25.720715 pysolarfocus-3.6.1/README.md
--rw-r--r--   0        0        0      580 2023-03-29 17:56:25.720715 pysolarfocus-3.6.1/pyproject.toml
--rw-r--r--   0        0        0     5601 2023-03-29 17:56:25.720715 pysolarfocus-3.6.1/pysolarfocus/__init__.py
--rw-r--r--   0        0        0     3356 2023-03-29 17:56:25.720715 pysolarfocus-3.6.1/pysolarfocus/component_factory.py
--rw-r--r--   0        0        0        0 2023-03-29 17:56:25.720715 pysolarfocus-3.6.1/pysolarfocus/components/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 17:56:25.720715 pysolarfocus-3.6.1/pysolarfocus/components/base/__init__.py
--rw-r--r--   0        0        0     9390 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/base/component.py
--rw-r--r--   0        0        0     2840 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/base/data_value.py
--rw-r--r--   0        0        0      159 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/base/enums.py
--rw-r--r--   0        0        0      205 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/base/part.py
--rw-r--r--   0        0        0      784 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/base/performance_calculator.py
--rw-r--r--   0        0        0      133 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/base/register_slice.py
--rw-r--r--   0        0        0      872 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/boiler.py
--rw-r--r--   0        0        0     1474 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/buffer.py
--rw-r--r--   0        0        0      292 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/fresh_water_module.py
--rw-r--r--   0        0        0     2650 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/heat_pump.py
--rw-r--r--   0        0        0     1827 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/heating_circuit.py
--rw-r--r--   0        0        0     1877 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/pellets_boiler.py
--rw-r--r--   0        0        0      800 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/photovoltaic.py
--rw-r--r--   0        0        0     1054 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/components/solar.py
--rw-r--r--   0        0        0     2965 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/const.py
--rw-r--r--   0        0        0     4027 2023-03-29 17:56:25.724716 pysolarfocus-3.6.1/pysolarfocus/modbus_wrapper.py
--rw-r--r--   0        0        0     3880 1970-01-01 00:00:00.000000 pysolarfocus-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/LICENSE
+-rw-r--r--   0        0        0     3183 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/README.md
+-rw-r--r--   0        0        0      580 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5601 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/pysolarfocus/__init__.py
+-rw-r--r--   0        0        0     3495 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/pysolarfocus/component_factory.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:52:37.749417 pysolarfocus-3.6.2/pysolarfocus/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/__init__.py
+-rw-r--r--   0        0        0     9390 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/component.py
+-rw-r--r--   0        0        0     2840 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/data_value.py
+-rw-r--r--   0        0        0      159 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/enums.py
+-rw-r--r--   0        0        0      205 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/part.py
+-rw-r--r--   0        0        0      784 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/performance_calculator.py
+-rw-r--r--   0        0        0      133 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/base/register_slice.py
+-rw-r--r--   0        0        0      872 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/boiler.py
+-rw-r--r--   0        0        0     1474 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/buffer.py
+-rw-r--r--   0        0        0      292 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/fresh_water_module.py
+-rw-r--r--   0        0        0     2650 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/heat_pump.py
+-rw-r--r--   0        0        0     1827 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/heating_circuit.py
+-rw-r--r--   0        0        0     1877 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/pellets_boiler.py
+-rw-r--r--   0        0        0      800 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/photovoltaic.py
+-rw-r--r--   0        0        0     1054 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/components/solar.py
+-rw-r--r--   0        0        0     2965 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/const.py
+-rw-r--r--   0        0        0     4027 2023-04-14 13:52:37.753417 pysolarfocus-3.6.2/pysolarfocus/modbus_wrapper.py
+-rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 pysolarfocus-3.6.2/PKG-INFO
```

### Comparing `pysolarfocus-3.6.1/LICENSE` & `pysolarfocus-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/README.md` & `pysolarfocus-3.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,16 @@
 ## Changelog of API-Versions
 > **Note**
 > The API-Version of Solarfocus is independent of the versions of this library. Below list refers to to 
 > the Solarfocus versions. See [releases](https://github.com/LavermanJJ/pysolarfocus/releases)for the changelog
 > of this library.
 
 
-#### 23.040
+#### 23.020
 * Add fresh water module state.
 
 #### 23.010
 * Add biomass boiler pellet statistics.
 
 #### 22.090
 * Add biomass boiler sweep function control.
-* Allow input of external buffer values.
+* Allow input of external buffer values.
```

### Comparing `pysolarfocus-3.6.1/pyproject.toml` & `pysolarfocus-3.6.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysolarfocus"
-version = "3.6.1"
+version = "3.6.2"
 description = "Unofficial, local Solarfocus client"
 authors = ["Jeroen Laverman <jjlaverman@web.de>"]
 license = "Apache-2.0"
 homepage = "https://github.com/lavermanjj/pysolarfocus"
 repository = "https://github.com/lavermanjj/pysolarfocus"
 keywords = ["solarfocus", "api client"]
 include = ["LICENSE"]
```

### Comparing `pysolarfocus-3.6.1/pysolarfocus/__init__.py` & `pysolarfocus-3.6.2/pysolarfocus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Python client lib for Solarfocus"""
-__version__ = "3.6.1"
+__version__ = "3.6.2"
 
 from enum import Enum
 from packaging import version
 
 #Default port for modbus
 PORT = 502
```

### Comparing `pysolarfocus-3.6.1/pysolarfocus/component_factory.py` & `pysolarfocus-3.6.2/pysolarfocus/component_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,19 @@
     def buffer(self, system:Systems,count:int, api_version:ApiVersions)->list[Buffer]:
         input_addresses = list(range(1900,1900+(20*count),20))
         holding_addresses = -1
         if api_version.greater_or_equal(ApiVersions.V_22_090.value):
             holding_addresses = list(range(34000,34000+(50*count),50))
         buffers = []
         for i in range(count):
-            input,holding = input_addresses[i],holding_addresses[i]
+            input = input_addresses[i]
+            if api_version.greater_or_equal(ApiVersions.V_22_090.value):
+                holding = holding_addresses[i]
+            else:
+                holding = -1 
             if system == Systems.Therminator:
                 buffer = TherminatorBuffer(input)._initialize(self.__modbus_connector)
             else:
                 buffer = Buffer(input,holding,api_version=api_version)._initialize(self.__modbus_connector)
             buffers.append(buffer)
         return buffers
```

### Comparing `pysolarfocus-3.6.1/pysolarfocus/components/base/component.py` & `pysolarfocus-3.6.2/pysolarfocus/components/base/component.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/components/base/data_value.py` & `pysolarfocus-3.6.2/pysolarfocus/components/base/data_value.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/components/base/performance_calculator.py` & `pysolarfocus-3.6.2/pysolarfocus/components/base/performance_calculator.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/components/boiler.py` & `pysolarfocus-3.6.2/pysolarfocus/components/boiler.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/components/buffer.py` & `pysolarfocus-3.6.2/pysolarfocus/components/buffer.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/components/heat_pump.py` & `pysolarfocus-3.6.2/pysolarfocus/components/heat_pump.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/components/heating_circuit.py` & `pysolarfocus-3.6.2/pysolarfocus/components/heating_circuit.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/components/pellets_boiler.py` & `pysolarfocus-3.6.2/pysolarfocus/components/pellets_boiler.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/components/photovoltaic.py` & `pysolarfocus-3.6.2/pysolarfocus/components/photovoltaic.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/components/solar.py` & `pysolarfocus-3.6.2/pysolarfocus/components/solar.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/const.py` & `pysolarfocus-3.6.2/pysolarfocus/const.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/pysolarfocus/modbus_wrapper.py` & `pysolarfocus-3.6.2/pysolarfocus/modbus_wrapper.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.1/PKG-INFO` & `pysolarfocus-3.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysolarfocus
-Version: 3.6.1
+Version: 3.6.2
 Summary: Unofficial, local Solarfocus client
 Home-page: https://github.com/lavermanjj/pysolarfocus
 License: Apache-2.0
 Keywords: solarfocus,api client
 Author: Jeroen Laverman
 Author-email: jjlaverman@web.de
 Requires-Python: >=3.9,<4.0
@@ -97,16 +97,17 @@
 ## Changelog of API-Versions
 > **Note**
 > The API-Version of Solarfocus is independent of the versions of this library. Below list refers to to 
 > the Solarfocus versions. See [releases](https://github.com/LavermanJJ/pysolarfocus/releases)for the changelog
 > of this library.
 
 
-#### 23.040
+#### 23.020
 * Add fresh water module state.
 
 #### 23.010
 * Add biomass boiler pellet statistics.
 
 #### 22.090
 * Add biomass boiler sweep function control.
 * Allow input of external buffer values.
+
```

