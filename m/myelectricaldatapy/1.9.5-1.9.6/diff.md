# Comparing `tmp/myelectricaldatapy-1.9.5.tar.gz` & `tmp/myelectricaldatapy-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myelectricaldatapy-1.9.5.tar", last modified: Wed Apr 12 06:09:54 2023, max compression
+gzip compressed data, was "myelectricaldatapy-1.9.6.tar", last modified: Fri Apr 14 06:38:39 2023, max compression
```

## Comparing `myelectricaldatapy-1.9.5.tar` & `myelectricaldatapy-1.9.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/myelectricaldatapy/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/myelectricaldata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/myelectricaldatapy/mypdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-12 06:09:54.000000 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-12 06:09:54.000000 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 06:09:54.000000 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 06:09:54.000000 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 06:09:54.000000 myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-12 06:09:53.000000 myelectricaldatapy-1.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:09:54.094538 myelectricaldatapy-1.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/tests/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-12 06:09:43.000000 myelectricaldatapy-1.9.5/tests/test_load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/myelectricaldatapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/myelectricaldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9535 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/myelectricaldatapy/mypdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-14 06:38:39.000000 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-14 06:38:39.000000 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:38:39.000000 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 06:38:39.000000 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 06:38:39.000000 myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-14 06:38:37.000000 myelectricaldatapy-1.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:38:39.456822 myelectricaldatapy-1.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51244 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/tests/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-14 06:38:30.000000 myelectricaldatapy-1.9.6/tests/test_load_data.py
```

### Comparing `myelectricaldatapy-1.9.5/LICENSE` & `myelectricaldatapy-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.5/PKG-INFO` & `myelectricaldatapy-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.5
+Version: 1.9.6
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.5/README.md` & `myelectricaldatapy-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.5/myelectricaldatapy/analytics.py` & `myelectricaldatapy-1.9.6/myelectricaldatapy/analytics.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.5/myelectricaldatapy/auth.py` & `myelectricaldatapy-1.9.6/myelectricaldatapy/auth.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.5/myelectricaldatapy/myelectricaldata.py` & `myelectricaldatapy-1.9.6/myelectricaldatapy/myelectricaldata.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.5/myelectricaldatapy/mypdl.py` & `myelectricaldatapy-1.9.6/myelectricaldatapy/mypdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Class for my PDL."""
 from __future__ import annotations
 
 import logging
-from datetime import date
 from datetime import datetime as dt
 from datetime import timedelta
 from typing import Any, Callable, Tuple
 
 import voluptuous as vol
 
 from myelectricaldatapy import Enedis
@@ -103,15 +102,14 @@
         self.access: dict[str, Any] = {}
         self.contract: dict[str, Any] = {}
         self.address: dict[str, Any] = {}
         self.tempo: dict[str, Any] = {}
         self.ecowatt: dict[str, Any] = {}
         self.max_power: dict[str, Any] = {}
         self._connected: bool = False
-        self._last_access: date | None = None
         self._params: dict[str, dict[str, Any]] = {PRODUCTION: {}, CONSUMPTION: {}}
 
     @property
     def is_connected(self) -> bool:
         """Connect state."""
         return self.access.get("valid", False) is True
 
@@ -164,83 +162,68 @@
                 cum_price=params.get(ATTR_CUM_PRICE, {}),
                 start_date=params.get(ATTR_START),
                 tempo=self.tempo,
             )
             stats.update({mode: resultat})
         return stats
 
-    async def async_update(
-        self,
-        modes: dict[str, Any] | None = None,
-        force_refresh: bool = False,
-    ) -> None:
+    async def async_update(self, modes: dict[str, Any] | None = None) -> None:
         """Update data.
 
         modes = {
             "consumption":{
                 "service":["daily_consumption" | "consumption_load_curve"],
                 start: [date],
                 end: [date]
             },
             "production":{
                 "service":["daily_production" | "production_load_curve"],
                 start: [date],
                 end: [date]
             }
         }
-        If the update succeeds, the next one can only be done on the next day
-        at least that force_refresh is true
         """
-        self.access = await self._api.async_valid_access(self.pdl)
-        if (
-            force_refresh is False
-            and self._last_access is not None
-            and self._last_access == dt.now().date()
-        ):
-            return
-
-        start = dt.now() - timedelta(days=730)
-        end = dt.now()
+        start = dt.now() - timedelta(days=1095)
+        end = dt.now() + timedelta(days=1)
         funcs: dict[str, Callable[..., Any]] = {
             DAILY_PROD: self._api.async_get_daily_production,
             DETAIL_PROD: self._api.async_get_details_production,
             DAILY_CONSUM: self._api.async_get_daily_consumption,
             DETAIL_CONSUM: self._api.async_get_details_consumption,
         }
 
+        self.access = await self._api.async_valid_access(self.pdl)
         self.contract = await self._api.async_get_contract(self.pdl)
         self.address = await self._api.async_get_address(self.pdl)
         if self._ecowatt_subs:
-            self.ecowatt = await self._api.async_get_ecowatt(
-                start, end + timedelta(days=1)
-            )
+            self.ecowatt = await self._api.async_get_ecowatt(start, end)
         if self._maxpower_subs:
             self.max_power = await self._api.async_get_max_power(self.pdl, start, end)
         if modes:
             try:
                 validate = MODES_SCH(modes)
             except vol.Error as error:
                 _LOGGER.error("The format is incorrect. (%s)", error)
             else:
                 for mode, params in validate.items():
                     service = params.get(ATTR_SERVICE)
                     days = 370 if service in [DAILY_PROD, DAILY_CONSUM] else 7
                     func = funcs[params.get(ATTR_SERVICE)]
-                    start = (
+                    dt_start = (
                         params.get(ATTR_START)
                         if params.get(ATTR_START)
                         else dt.now() - timedelta(days=days)
                     )
-                    end = params.get(ATTR_END) if params.get(ATTR_END) else dt.now()
-                    dataset = await func(self.pdl, start, end)
-                    self._params[mode].update({"dataset": dataset, ATTR_START: start})
+                    dt_end = params.get(ATTR_END) if params.get(ATTR_END) else end
+                    dataset = await func(self.pdl, dt_start, dt_end)
+                    self._params[mode].update(
+                        {"dataset": dataset, ATTR_START: dt_start}
+                    )
                     if service in [DAILY_CONSUM, DETAIL_CONSUM] and self._tempo_subs:
-                        self.tempo = await self._api.async_get_tempo(start, end)
-
-        self._last_access = dt.now().date()
+                        self.tempo = await self._api.async_get_tempo(dt_start, dt_end)
 
     def tempo_subscription(self, activate: bool = False) -> None:
         """Enable or Disable Tempo Subscription."""
         self._off_subs = False
         self._tempo_subs = activate is True
 
     def offpeak_subscription(self, activate: bool = False) -> None:
```

### Comparing `myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/PKG-INFO` & `myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myelectricaldatapy
-Version: 1.9.5
+Version: 1.9.6
 Summary: Fetch Linky data from myelectricaldata.fr
 Home-page: https://github.com/cyr-ius/myelectricaldatapy/tree/master/myelectricaldatapy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: enedis,linky,async,myelectricaldata
 Classifier: Programming Language :: Python
```

### Comparing `myelectricaldatapy-1.9.5/myelectricaldatapy.egg-info/SOURCES.txt` & `myelectricaldatapy-1.9.6/myelectricaldatapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.5/pyproject.toml` & `myelectricaldatapy-1.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.5/setup.py` & `myelectricaldatapy-1.9.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="myelectricaldatapy",
-    version="1.9.5",
+    version="1.9.6",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Fetch Linky data from myelectricaldata.fr",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "pandas==1.4.3", "voluptuous>=0.13.1"],
```

### Comparing `myelectricaldatapy-1.9.5/tests/consts.py` & `myelectricaldatapy-1.9.6/tests/consts.py`

 * *Files identical despite different names*

### Comparing `myelectricaldatapy-1.9.5/tests/test_analytics.py` & `myelectricaldatapy-1.9.6/tests/test_analytics.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     assert resultat[0]["value"] == 1.296
 
     dataset = DS_DAILY
     modes = {"consumption": {"service": "daily_consumption"}}
     with patch.object(
         myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
     ):
-        await api.async_update(modes=modes, force_refresh=True)
+        await api.async_update(modes=modes)
         resultat = api.stats["consumption"]
 
     assert resultat[0]["notes"] == "standard"
     assert resultat[0]["value"] == 42.045
 
 
 @freeze_time("2023-03-01")
@@ -69,15 +69,15 @@
     assert round(resultat[0]["price"], 2) == 0.22
 
     dataset = DS_DAILY
     modes = {"consumption": {"service": "daily_consumption"}}
     with patch.object(
         myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
     ):
-        await api.async_update(modes=modes, force_refresh=True)
+        await api.async_update(modes=modes)
         resultat = api.stats["consumption"]
 
     assert resultat[0]["notes"] == "standard"
     assert round(resultat[0]["price"], 2) == 7.15
 
 
 @freeze_time("2023-03-01")
@@ -202,15 +202,15 @@
 
     sum_value_1 = resultat1[26]["sum_value"] + resultat1[77]["sum_value"]
     assert round(sum_value, 3) == round(sum_value_1, 3)
     dataset = DS_COMPARE
     with patch.object(
         myelectricaldatapy.auth.EnedisAuth, "request", return_value=dataset
     ):
-        await api.async_update(modes=modes, force_refresh=True)
+        await api.async_update(modes=modes)
         resultat2 = api.stats["consumption"]
     assert round(sum_value, 3) == resultat2[2]["sum_value"]
     print(resultat2)
 
 
 @freeze_time("2023-03-01")
 @pytest.mark.asyncio
```

### Comparing `myelectricaldatapy-1.9.5/tests/test_load_data.py` & `myelectricaldatapy-1.9.6/tests/test_load_data.py`

 * *Files identical despite different names*

