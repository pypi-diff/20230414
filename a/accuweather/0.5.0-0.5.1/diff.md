# Comparing `tmp/accuweather-0.5.0.tar.gz` & `tmp/accuweather-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accuweather-0.5.0.tar", last modified: Fri Jan  6 17:11:46 2023, max compression
+gzip compressed data, was "accuweather-0.5.1.tar", last modified: Fri Apr 14 07:26:32 2023, max compression
```

## Comparing `accuweather-0.5.0.tar` & `accuweather-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 17:11:46.485556 accuweather-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-01-06 17:11:36.000000 accuweather-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-06 17:11:36.000000 accuweather-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-01-06 17:11:46.485556 accuweather-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-01-06 17:11:36.000000 accuweather-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 17:11:46.485556 accuweather-0.5.0/accuweather/
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-01-06 17:11:36.000000 accuweather-0.5.0/accuweather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-06 17:11:36.000000 accuweather-0.5.0/accuweather/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-06 17:11:36.000000 accuweather-0.5.0/accuweather/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 17:11:36.000000 accuweather-0.5.0/accuweather/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 17:11:46.485556 accuweather-0.5.0/accuweather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-01-06 17:11:46.000000 accuweather-0.5.0/accuweather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-06 17:11:46.000000 accuweather-0.5.0/accuweather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 17:11:46.000000 accuweather-0.5.0/accuweather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-06 17:11:46.000000 accuweather-0.5.0/accuweather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-06 17:11:46.000000 accuweather-0.5.0/accuweather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-06 17:11:36.000000 accuweather-0.5.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-06 17:11:36.000000 accuweather-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-01-06 17:11:46.489556 accuweather-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-01-06 17:11:36.000000 accuweather-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:26:32.193588 accuweather-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-04-14 07:26:16.000000 accuweather-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 07:26:16.000000 accuweather-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-14 07:26:32.193588 accuweather-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-14 07:26:16.000000 accuweather-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:26:32.193588 accuweather-0.5.1/accuweather/
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-14 07:26:16.000000 accuweather-0.5.1/accuweather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-14 07:26:16.000000 accuweather-0.5.1/accuweather/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 07:26:16.000000 accuweather-0.5.1/accuweather/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:26:16.000000 accuweather-0.5.1/accuweather/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:26:32.193588 accuweather-0.5.1/accuweather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-14 07:26:32.000000 accuweather-0.5.1/accuweather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 07:26:32.000000 accuweather-0.5.1/accuweather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:26:32.000000 accuweather-0.5.1/accuweather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 07:26:32.000000 accuweather-0.5.1/accuweather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 07:26:32.000000 accuweather-0.5.1/accuweather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-14 07:26:16.000000 accuweather-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-14 07:26:16.000000 accuweather-0.5.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 07:26:16.000000 accuweather-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 07:26:32.193588 accuweather-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-14 07:26:16.000000 accuweather-0.5.1/setup.py
```

### Comparing `accuweather-0.5.0/LICENSE` & `accuweather-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `accuweather-0.5.0/PKG-INFO` & `accuweather-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accuweather
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python wrapper for getting weather data from AccuWeather servers.
 Home-page: https://github.com/bieniu/accuweather
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,15 @@
 ## API key
 
 To generate API key go to https://developer.accuweather.com/user/register and after registration create an app.
 
 
 ## How to use package
 ```python
+"""Example of usage."""
 import asyncio
 import logging
 
 from aiohttp import ClientError, ClientSession
 
 from accuweather import (
     AccuWeather,
@@ -55,14 +56,15 @@
 LOCATION_KEY = "268068"
 API_KEY = "xxxxx"
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 async def main():
+    """Run main function."""
     async with ClientSession() as websession:
         try:
             accuweather = AccuWeather(
                 API_KEY, websession, latitude=LATITUDE, longitude=LONGITUDE
             )
             current_conditions = await accuweather.async_get_current_conditions()
             forecast = await accuweather.async_get_forecast(metric=True)
@@ -82,15 +84,14 @@
             print(f"Forecast: {forecast}")
             print(f"Forecast hourly: {forecast_hourly}")
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
-
 ```
 
 [releases]: https://github.com/bieniu/accuweather/releases
 [releases-shield]: https://img.shields.io/github/release/bieniu/accuweather.svg?style=popout
 [pypi-releases]: https://pypi.org/project/accuweather/
 [pypi-statistics]: https://pepy.tech/project/accuweather
 [pypi-releases-shield]: https://img.shields.io/pypi/v/accuweather
```

### Comparing `accuweather-0.5.0/README.md` & `accuweather-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ## API key
 
 To generate API key go to https://developer.accuweather.com/user/register and after registration create an app.
 
 
 ## How to use package
 ```python
+"""Example of usage."""
 import asyncio
 import logging
 
 from aiohttp import ClientError, ClientSession
 
 from accuweather import (
     AccuWeather,
@@ -34,14 +35,15 @@
 LOCATION_KEY = "268068"
 API_KEY = "xxxxx"
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 async def main():
+    """Run main function."""
     async with ClientSession() as websession:
         try:
             accuweather = AccuWeather(
                 API_KEY, websession, latitude=LATITUDE, longitude=LONGITUDE
             )
             current_conditions = await accuweather.async_get_current_conditions()
             forecast = await accuweather.async_get_forecast(metric=True)
@@ -61,15 +63,14 @@
             print(f"Forecast: {forecast}")
             print(f"Forecast hourly: {forecast_hourly}")
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
-
 ```
 
 [releases]: https://github.com/bieniu/accuweather/releases
 [releases-shield]: https://img.shields.io/github/release/bieniu/accuweather.svg?style=popout
 [pypi-releases]: https://pypi.org/project/accuweather/
 [pypi-statistics]: https://pepy.tech/project/accuweather
 [pypi-releases-shield]: https://img.shields.io/pypi/v/accuweather
```

### Comparing `accuweather-0.5.0/accuweather/__init__.py` & `accuweather-0.5.1/accuweather/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Python wrapper for getting weather data from AccueWeather for Limited Trial."""
 
 from __future__ import annotations
 
 import logging
 from http import HTTPStatus
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import orjson
 from aiohttp import ClientSession
 
 from .const import (
     ATTR_CURRENT_CONDITIONS,
     ATTR_FORECAST_DAILY_5,
     ATTR_FORECAST_HOURLY_12,
     ATTR_GEOPOSITION,
     ENDPOINT,
     HTTP_HEADERS,
+    MAX_API_KEY_LENGTH,
+    MAX_LATITUDE,
+    MAX_LONGITUDE,
     REMOVE_FROM_CURRENT_CONDITION,
     REMOVE_FROM_FORECAST,
     REQUESTS_EXCEEDED,
     TEMPERATURES,
     URLS,
 )
 from .exceptions import (
@@ -31,30 +34,29 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AccuWeather:
     """Main class to perform AccuWeather API requests."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         api_key: str,
         session: ClientSession,
         latitude: float | None = None,
         longitude: float | None = None,
         location_key: str | None = None,
     ) -> None:
         """Initialize."""
         if not self._valid_api_key(api_key):
             raise InvalidApiKeyError(
                 "Your API Key must be a 32-character hexadecimal string"
             )
-        if not location_key:
-            if not self._valid_coordinates(latitude, longitude):
-                raise InvalidCoordinatesError("Your coordinates are invalid")
+        if not location_key and not self._valid_coordinates(latitude, longitude):
+            raise InvalidCoordinatesError("Your coordinates are invalid")
 
         self.latitude = latitude
         self.longitude = longitude
         self._api_key = api_key
         self._session = session
         self._location_key = location_key
         self._location_name: str | None = None
@@ -64,33 +66,32 @@
     def _valid_coordinates(
         latitude: float | int | None, longitude: float | int | None
     ) -> bool:
         """Return True if coordinates are valid."""
         if (
             isinstance(latitude, (int, float))
             and isinstance(longitude, (int, float))
-            and abs(latitude) <= 90
-            and abs(longitude) <= 180
+            and abs(latitude) <= MAX_LATITUDE
+            and abs(longitude) <= MAX_LONGITUDE
         ):
             return True
         return False
 
     @staticmethod
     def _valid_api_key(api_key: str) -> bool:
         """Return True if API key is valid."""
-        if isinstance(api_key, str) and len(api_key) == 32:
+        if isinstance(api_key, str) and len(api_key) == MAX_API_KEY_LENGTH:
             return True
 
         return False
 
     @staticmethod
     def _construct_url(arg: str, **kwargs: str) -> str:
         """Construct AccuWeather API URL."""
-        url = ENDPOINT + URLS[arg].format(**kwargs)
-        return url
+        return ENDPOINT + URLS[arg].format(**kwargs)
 
     @staticmethod
     def _clean_current_condition(
         data: dict[str, Any], to_remove: tuple[str, ...]
     ) -> dict[str, Any]:
         """Clean current condition API response."""
         return {key: data[key] for key in data if key not in to_remove}
@@ -102,27 +103,25 @@
         """Parse and clean daily forecast API response."""
         parsed_data = [
             {key: value for key, value in item.items() if key not in to_remove}
             for item in data["DailyForecasts"]
         ]
 
         for day in parsed_data:
-            # For some forecast days, the AccuWeather API does not provide an Ozone value.
+            # For some forecast days, the API does not provide an Ozone value.
             day.setdefault("Ozone", {})
             day["Ozone"].setdefault("Value")
             day["Ozone"].setdefault("Category")
 
             for item in day["AirAndPollen"]:
                 if item["Name"] == "AirQuality":
                     day[item["Type"]] = item
-                    day[item["Type"]].pop("Name")
-                    day[item["Type"]].pop("Type")
-                else:
-                    day[item["Name"]] = item
-                    day[item["Name"]].pop("Name")
+                day[item["Name"]] = item
+                day[item["Name"]]["Category"] = day[item["Name"]]["Category"].lower()
+                day[item["Name"]].pop("Name")
             day.pop("AirAndPollen")
 
             for temp in TEMPERATURES:
                 day[f"{temp}Min"] = day[temp]["Minimum"]
                 day[f"{temp}Max"] = day[temp]["Maximum"]
                 day.pop(temp)
 
@@ -136,35 +135,36 @@
         return parsed_data
 
     @staticmethod
     def _parse_forecast_hourly(
         data: list[dict[str, Any]], to_remove: tuple[str, ...]
     ) -> list[dict[str, Any]]:
         """Parse and clean hourly forecast API response."""
-        parsed_data = [
+        return [
             {key: value for key, value in item.items() if key not in to_remove}
             for item in data
         ]
-        return parsed_data
 
     async def _async_get_data(self, url: str) -> Any:
         """Retrieve data from AccuWeather API."""
         async with self._session.get(url, headers=HTTP_HEADERS) as resp:
             if resp.status == HTTPStatus.UNAUTHORIZED.value:
                 raise InvalidApiKeyError("Invalid API key")
+
             if resp.status != HTTPStatus.OK.value:
-                # pylint: disable=no-member
                 error_text = orjson.loads(await resp.text())
                 if error_text["Message"] == REQUESTS_EXCEEDED:
                     raise RequestsExceededError(
                         "The allowed number of requests has been exceeded"
                     )
                 raise ApiError(f"Invalid response from AccuWeather API: {resp.status}")
+
             _LOGGER.debug("Data retrieved from %s, status: %s", url, resp.status)
             data = await resp.json()
+
         if resp.headers["RateLimit-Remaining"].isdigit():
             self._requests_remaining = int(resp.headers["RateLimit-Remaining"])
 
         if "hourly" in url:
             return data
 
         return data if isinstance(data, dict) else data[0]
@@ -181,28 +181,34 @@
         self._location_key = data["Key"]
         self._location_name = data["LocalizedName"]
 
     async def async_get_current_conditions(self) -> dict[str, Any]:
         """Retrieve current conditions data from AccuWeather."""
         if not self._location_key:
             await self.async_get_location()
-        assert self._location_key is not None
+
+        if TYPE_CHECKING:
+            assert self._location_key is not None  # noqa: S101
+
         url = self._construct_url(
             ATTR_CURRENT_CONDITIONS,
             api_key=self._api_key,
             location_key=self._location_key,
         )
         data = await self._async_get_data(url)
         return self._clean_current_condition(data, REMOVE_FROM_CURRENT_CONDITION)
 
     async def async_get_forecast(self, metric: bool = True) -> list[dict[str, Any]]:
         """Retrieve daily forecast data from AccuWeather."""
         if not self._location_key:
             await self.async_get_location()
-        assert self._location_key is not None
+
+        if TYPE_CHECKING:
+            assert self._location_key is not None  # noqa: S101
+
         url = self._construct_url(
             ATTR_FORECAST_DAILY_5,
             api_key=self._api_key,
             location_key=self._location_key,
             metric=str(metric),
         )
         data = await self._async_get_data(url)
@@ -210,15 +216,18 @@
 
     async def async_get_forecast_hourly(
         self, metric: bool = True
     ) -> list[dict[str, Any]]:
         """Retrieve hourly forecast data from AccuWeather."""
         if not self._location_key:
             await self.async_get_location()
-        assert self._location_key is not None
+
+        if TYPE_CHECKING:
+            assert self._location_key is not None  # noqa: S101
+
         url = self._construct_url(
             ATTR_FORECAST_HOURLY_12,
             api_key=self._api_key,
             location_key=self._location_key,
             metric=str(metric),
         )
         data = await self._async_get_data(url)
```

### Comparing `accuweather-0.5.0/accuweather/const.py` & `accuweather-0.5.1/accuweather/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from __future__ import annotations
 
 ATTR_CURRENT_CONDITIONS: str = "currentconditions"
 ATTR_FORECAST_DAILY_5: str = "forecasts"
 ATTR_FORECAST_HOURLY_12: str = "forecasts_hourly"
 ATTR_GEOPOSITION: str = "geoposition"
 
+MAX_API_KEY_LENGTH = 32
+MAX_LATITUDE = 90
+MAX_LONGITUDE = 180
+
 ENDPOINT: str = "https://dataservice.accuweather.com/"
 HTTP_HEADERS: dict[str, str] = {"Content-Encoding": "gzip"}
 REQUESTS_EXCEEDED: str = "The allowed number of requests has been exceeded."
 
 REMOVE_FROM_CURRENT_CONDITION: tuple[str, ...] = (
     "LocalObservationDateTime",
     "EpochTime",
@@ -24,10 +28,10 @@
     "Temperature",
     "RealFeelTemperature",
     "RealFeelTemperatureShade",
 )
 URLS: dict[str, str] = {
     ATTR_GEOPOSITION: "locations/v1/cities/geoposition/search?apikey={api_key}&q={lat}%2C{lon}",
     ATTR_CURRENT_CONDITIONS: "currentconditions/v1/{location_key}?apikey={api_key}&details=true",
-    ATTR_FORECAST_DAILY_5: "forecasts/v1/daily/5day/{location_key}?apikey={api_key}&details=true&metric={metric}",  # pylint: disable=line-too-long
-    ATTR_FORECAST_HOURLY_12: "forecasts/v1/hourly/12hour/{location_key}?apikey={api_key}&details=true&metric={metric}",  # pylint: disable=line-too-long
+    ATTR_FORECAST_DAILY_5: "forecasts/v1/daily/5day/{location_key}?apikey={api_key}&details=true&metric={metric}",
+    ATTR_FORECAST_HOURLY_12: "forecasts/v1/hourly/12hour/{location_key}?apikey={api_key}&details=true&metric={metric}",
 }
```

### Comparing `accuweather-0.5.0/accuweather/exceptions.py` & `accuweather-0.5.1/accuweather/exceptions.py`

 * *Files identical despite different names*

### Comparing `accuweather-0.5.0/accuweather.egg-info/PKG-INFO` & `accuweather-0.5.1/accuweather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accuweather
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python wrapper for getting weather data from AccuWeather servers.
 Home-page: https://github.com/bieniu/accuweather
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,15 @@
 ## API key
 
 To generate API key go to https://developer.accuweather.com/user/register and after registration create an app.
 
 
 ## How to use package
 ```python
+"""Example of usage."""
 import asyncio
 import logging
 
 from aiohttp import ClientError, ClientSession
 
 from accuweather import (
     AccuWeather,
@@ -55,14 +56,15 @@
 LOCATION_KEY = "268068"
 API_KEY = "xxxxx"
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 async def main():
+    """Run main function."""
     async with ClientSession() as websession:
         try:
             accuweather = AccuWeather(
                 API_KEY, websession, latitude=LATITUDE, longitude=LONGITUDE
             )
             current_conditions = await accuweather.async_get_current_conditions()
             forecast = await accuweather.async_get_forecast(metric=True)
@@ -82,15 +84,14 @@
             print(f"Forecast: {forecast}")
             print(f"Forecast hourly: {forecast_hourly}")
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
-
 ```
 
 [releases]: https://github.com/bieniu/accuweather/releases
 [releases-shield]: https://img.shields.io/github/release/bieniu/accuweather.svg?style=popout
 [pypi-releases]: https://pypi.org/project/accuweather/
 [pypi-statistics]: https://pepy.tech/project/accuweather
 [pypi-releases-shield]: https://img.shields.io/pypi/v/accuweather
```

### Comparing `accuweather-0.5.0/setup.py` & `accuweather-0.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Setup module for accuweather."""
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.5.0"
+VERSION = "0.5.1"
+
+with open("requirements.txt", encoding="utf-8") as file:
+    requirements = file.read().splitlines()
 
 setup(
     name="accuweather",
     version=VERSION,
     author="Maciej Bieniek",
     description="Python wrapper for getting weather data from AccuWeather servers.",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/bieniu/accuweather",
     license="Apache-2.0 License",
     packages=["accuweather"],
     package_data={"accuweather": ["py.typed"]},
     python_requires=">=3.9",
-    install_requires=list(
-        val.strip() for val in open("requirements.txt", encoding="utf-8")
-    ),
+    install_requires=requirements,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
```

