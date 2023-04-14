# Comparing `tmp/carrier_api-1.9.0.tar.gz` & `tmp/carrier_api-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carrier_api-1.9.0.tar", last modified: Thu Mar 30 11:24:47 2023, max compression
+gzip compressed data, was "carrier_api-1.9.2.tar", last modified: Fri Apr 14 04:19:11 2023, max compression
```

## Comparing `carrier_api-1.9.0.tar` & `carrier_api-1.9.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:24:47.658915 carrier_api-1.9.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1066 2023-03-30 11:24:08.000000 carrier_api-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-30 11:24:47.658915 carrier_api-1.9.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      323 2023-03-30 11:24:08.000000 carrier_api-1.9.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-03-30 11:24:08.000000 carrier_api-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 11:24:47.658915 carrier_api-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-30 11:24:32.000000 carrier_api-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:24:47.654915 carrier_api-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:24:47.658915 carrier_api-1.9.0/src/carrier_api/
--rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-03-30 11:24:08.000000 carrier_api-1.9.0/src/carrier_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-03-30 11:24:08.000000 carrier_api-1.9.0/src/carrier_api/api_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-03-30 11:24:08.000000 carrier_api-1.9.0/src/carrier_api/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      616 2023-03-30 11:24:08.000000 carrier_api-1.9.0/src/carrier_api/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-03-30 11:24:08.000000 carrier_api-1.9.0/src/carrier_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-30 11:24:08.000000 carrier_api-1.9.0/src/carrier_api/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-03-30 11:24:08.000000 carrier_api-1.9.0/src/carrier_api/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-03-30 11:24:08.000000 carrier_api-1.9.0/src/carrier_api/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-30 11:24:08.000000 carrier_api-1.9.0/src/carrier_api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-30 11:24:08.000000 carrier_api-1.9.0/src/carrier_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:24:47.658915 carrier_api-1.9.0/src/carrier_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-30 11:24:47.000000 carrier_api-1.9.0/src/carrier_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-30 11:24:47.000000 carrier_api-1.9.0/src/carrier_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 11:24:47.000000 carrier_api-1.9.0/src/carrier_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-30 11:24:47.000000 carrier_api-1.9.0/src/carrier_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-30 11:24:47.000000 carrier_api-1.9.0/src/carrier_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:19:11.962215 carrier_api-1.9.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1066 2023-04-14 04:18:53.000000 carrier_api-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-14 04:19:11.962215 carrier_api-1.9.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1350 2023-04-14 04:18:53.000000 carrier_api-1.9.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-14 04:18:53.000000 carrier_api-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 04:19:11.962215 carrier_api-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-14 04:19:01.000000 carrier_api-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:19:11.962215 carrier_api-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:19:11.962215 carrier_api-1.9.2/src/carrier_api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/api_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      616 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:19:11.962215 carrier_api-1.9.2/src/carrier_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-14 04:19:11.000000 carrier_api-1.9.2/src/carrier_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 04:19:11.000000 carrier_api-1.9.2/src/carrier_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:19:11.000000 carrier_api-1.9.2/src/carrier_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 04:19:11.000000 carrier_api-1.9.2/src/carrier_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 04:19:11.000000 carrier_api-1.9.2/src/carrier_api.egg-info/top_level.txt
```

### Comparing `carrier_api-1.9.0/LICENSE` & `carrier_api-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.0/setup.py` & `carrier_api-1.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 LONG_DESCRIPTION = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = "1.9.0"
+VERSION = "1.9.2"
 
 # Setting up
 setup(
     name="carrier_api",
     version=VERSION,
     author="Brendan Dahl",
     author_email="dahl.brendan@gmail.com",
```

### Comparing `carrier_api-1.9.0/src/carrier_api/api_connection.py` & `carrier_api-1.9.2/src/carrier_api/api_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             if "error" in response_json:
                 _LOGGER.debug(response.content)
                 raise AuthError(response_json["error"]["message"])
             self.access_token = response.json()["result"]["accessToken"]
         return self.access_token
 
     def activate(self):
-        """request data refresh from api"""
+        """request data refresh from api."""
         url = f"{INFINITY_API_BASE_URL}/users/{self.username}/activateSystems"
         self._post(url)
 
     def get_systems(self) -> [System]:
         url = f"{INFINITY_API_BASE_URL}/users/{self.username}/locations"
         response_json = self._get(url)
         systems = []
```

### Comparing `carrier_api-1.9.0/src/carrier_api/config.py` & `carrier_api-1.9.2/src/carrier_api/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     def __repr__(self):
         builder = {
             "api_id": self.api_id,
             "name": self.name,
             "hold_activity": self.hold_activity,
             "hold": self.hold,
             "hold_until": self.hold_until,
-            "activities": list(map(lambda activity: activity.__repr__(), self.activities)),
+            "activities": [activity.__repr__() for activity in self.activities],
         }
         if self.hold_activity is not None:
             builder["hold_activity"] = self.hold_activity.value
         return builder
 
     def __str__(self):
         return str(self.__repr__())
@@ -121,14 +121,15 @@
         self.system = system
         self.refresh()
 
     def refresh(self):
         self.raw_config_json = self.system.api_connection.get_config(
             system_serial=self.system.serial
         )
+        _LOGGER.debug(f"raw_config_json:{self.raw_config_json}")
         self.temperature_unit = safely_get_json_value(self.raw_config_json, "cfgem")
         self.static_pressure = safely_get_json_value(self.raw_config_json, "staticPressure")
         self.mode = safely_get_json_value(self.raw_config_json, "mode")
         self.limit_min = safely_get_json_value(self.raw_config_json, "utilityEvent.minLimit", int)
         self.limit_max = safely_get_json_value(self.raw_config_json, "utilityEvent.maxLimit", int)
         self.time_stamp = isoparse(safely_get_json_value(self.raw_config_json, "timestamp"))
         vacation_json = {
@@ -148,12 +149,12 @@
         return {
             "temperature_unit": self.temperature_unit,
             "static_pressure": self.static_pressure,
             "mode": self.mode,
             "limit_min": self.limit_min,
             "limit_max": self.limit_max,
             "time_stamp": self.time_stamp.astimezone().strftime("%m/%d/%Y, %H:%M:%S %Z"),
-            "zones": list(map(lambda zone: zone.__repr__(), self.zones)),
+            "zones": [zone.__repr__() for zone in self.zones],
         }
 
     def __str__(self):
         return str(self.__repr__())
```

### Comparing `carrier_api-1.9.0/src/carrier_api/const.py` & `carrier_api-1.9.2/src/carrier_api/const.py`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.0/src/carrier_api/profile.py` & `carrier_api-1.9.2/src/carrier_api/profile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 
 from dateutil.parser import isoparse
 import datetime
-from dateutil import tz
 
 from .util import safely_get_json_value
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Profile:
@@ -28,14 +27,15 @@
         self.system = system
         self.refresh()
 
     def refresh(self):
         self.raw_profile_json = self.system.api_connection.get_profile(
             system_serial=self.system.serial
         )
+        _LOGGER.debug(f"raw_profile_json:{self.raw_profile_json}")
         self.model = safely_get_json_value(self.raw_profile_json, "model")
         self.brand = safely_get_json_value(self.raw_profile_json, "brand")
         self.firmware = safely_get_json_value(self.raw_profile_json, "firmware")
         self.indoor_model = safely_get_json_value(self.raw_profile_json, "indoorModel")
         self.indoor_serial = safely_get_json_value(self.raw_profile_json, "indoorSerial")
         self.outdoor_model = safely_get_json_value(self.raw_profile_json, "outdoorModel")
         self.outdoor_serial = self.raw_profile_json["outdoorSerial"]
```

### Comparing `carrier_api-1.9.0/src/carrier_api/status.py` & `carrier_api-1.9.2/src/carrier_api/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         self.system = system
         self.refresh()
 
     def refresh(self):
         self.raw_status_json = self.system.api_connection.get_status(
             system_serial=self.system.serial
         )
+        _LOGGER.debug(f"raw_status_json:{self.raw_status_json}")
         self.outdoor_temperature: float = safely_get_json_value(self.raw_status_json, "oat", float)
         self.mode: str = self.raw_status_json["mode"]
         self.temperature_unit: TemperatureUnits = TemperatureUnits(self.raw_status_json["cfgem"])
         self.filter_used: int = safely_get_json_value(self.raw_status_json, "filtrlvl", int)
         self.is_disconnected: bool = safely_get_json_value(self.raw_status_json, "isDisconnected", bool)
         self.airflow_cfm: int = safely_get_json_value(self.raw_status_json, "idu.cfm", int)
         self.outdoor_unit_operational_status: str = safely_get_json_value(self.raw_status_json, "odu.opstat")
@@ -107,12 +108,12 @@
             "temperature_unit": self.temperature_unit.value,
             "filter_used": self.filter_used,
             "is_disconnected": self.is_disconnected,
             "airflow_cfm": self.airflow_cfm,
             "outdoor_unit_operational_status": self.outdoor_unit_operational_status,
             "indoor_unit_operational_status": self.indoor_unit_operational_status,
             "time_stamp": self.time_stamp.astimezone().strftime("%m/%d/%Y, %H:%M:%S %Z"),
-            "zones": list(map(lambda zone: zone.__repr__(), self.zones)),
+            "zones": [zone.__repr__() for zone in self.zones],
         }
 
     def __str__(self):
         return str(self.__repr__())
```

### Comparing `carrier_api-1.9.0/src/carrier_api/stub.py` & `carrier_api-1.9.2/src/carrier_api/stub.py`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.0/src/carrier_api/system.py` & `carrier_api-1.9.2/src/carrier_api/system.py`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.0/src/carrier_api/util.py` & `carrier_api-1.9.2/src/carrier_api/util.py`

 * *Files identical despite different names*

