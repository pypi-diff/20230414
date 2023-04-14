# Comparing `tmp/satellite_weather_downloader-1.8.1.tar.gz` & `tmp/satellite_weather_downloader-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satellite_weather_downloader-1.8.1.tar", max compression
+gzip compressed data, was "satellite_weather_downloader-1.8.2.tar", max compression
```

## Comparing `satellite_weather_downloader-1.8.1.tar` & `satellite_weather_downloader-1.8.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-04-12 17:48:08.413393 satellite_weather_downloader-1.8.1/LICENSE
--rw-r--r--   0        0        0     3072 2023-04-12 17:48:08.413393 satellite_weather_downloader-1.8.1/README.md
--rw-r--r--   0        0        0     1862 2023-04-12 17:50:24.654929 satellite_weather_downloader-1.8.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/__init__.py
--rw-r--r--   0        0        0      190 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/__init__.py
--rw-r--r--   0        0        0     9715 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/extract_reanalysis.py
--rw-r--r--   0        0        0       52 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/reanalysis/__init__.py
--rw-r--r--   0        0        0    12112 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/reanalysis/api_vars.py
--rw-r--r--   0        0        0    16153 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/reanalysis/prompt.py
--rw-r--r--   0        0        0     2924 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/downloader/request.py
--rw-r--r--   0        0        0      296 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/__init__.py
--rw-r--r--   0        0        0       20 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/__init__.py
--rw-r--r--   0        0        0     1360 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas.py
--rw-r--r--   0        0        0       11 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.cst
--rw-r--r--   0        0        0     9413 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.dbf
--rw-r--r--   0        0        0      417 2023-04-12 17:48:08.417394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.prj
--rw-r--r--   0        0        0 11174984 2023-04-12 17:48:08.489394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.shp
--rw-r--r--   0        0        0      372 2023-04-12 17:48:08.489394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.shx
--rw-r--r--   0        0        0       77 2023-04-12 17:48:08.489394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/__init__.py
--rw-r--r--   0        0        0     4119 2023-04-12 17:48:08.489394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/extract_coordinates.py
--rw-r--r--   0        0        0     1351 2023-04-12 17:48:08.489394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/extract_latlons.py
--rw-r--r--   0        0        0  1175429 2023-04-12 17:48:08.493394 satellite_weather_downloader-1.8.1/satellite/weather/_brazil/municipios.json
--rw-r--r--   0        0        0       40 2023-04-12 17:48:08.493394 satellite_weather_downloader-1.8.1/satellite/weather/utils/__init__.py
--rw-r--r--   0        0        0     4871 2023-04-12 17:48:08.493394 satellite_weather_downloader-1.8.1/satellite/weather/utils/episem.py
--rw-r--r--   0        0        0    11908 2023-04-12 17:48:08.493394 satellite_weather_downloader-1.8.1/satellite/weather/xr_extensions.py
--rw-r--r--   0        0        0     4888 1970-01-01 00:00:00.000000 satellite_weather_downloader-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-14 17:09:47.313802 satellite_weather_downloader-1.8.2/LICENSE
+-rw-r--r--   0        0        0     3072 2023-04-14 17:09:47.313802 satellite_weather_downloader-1.8.2/README.md
+-rw-r--r--   0        0        0     1862 2023-04-14 17:11:54.347297 satellite_weather_downloader-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/__init__.py
+-rw-r--r--   0        0        0     9715 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/extract_reanalysis.py
+-rw-r--r--   0        0        0       52 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/reanalysis/__init__.py
+-rw-r--r--   0        0        0    12112 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/reanalysis/api_vars.py
+-rw-r--r--   0        0        0    16153 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/reanalysis/prompt.py
+-rw-r--r--   0        0        0     2924 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/downloader/request.py
+-rw-r--r--   0        0        0      296 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/__init__.py
+-rw-r--r--   0        0        0       20 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/__init__.py
+-rw-r--r--   0        0        0     1360 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas.py
+-rw-r--r--   0        0        0       11 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.cst
+-rw-r--r--   0        0        0     9413 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.dbf
+-rw-r--r--   0        0        0      417 2023-04-14 17:09:47.317803 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.prj
+-rw-r--r--   0        0        0 11174984 2023-04-14 17:09:47.389805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.shp
+-rw-r--r--   0        0        0      372 2023-04-14 17:09:47.389805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.shx
+-rw-r--r--   0        0        0       77 2023-04-14 17:09:47.389805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/__init__.py
+-rw-r--r--   0        0        0     4119 2023-04-14 17:09:47.389805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/extract_coordinates.py
+-rw-r--r--   0        0        0     1351 2023-04-14 17:09:47.389805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/extract_latlons.py
+-rw-r--r--   0        0        0  1175429 2023-04-14 17:09:47.393805 satellite_weather_downloader-1.8.2/satellite/weather/_brazil/municipios.json
+-rw-r--r--   0        0        0       40 2023-04-14 17:09:47.393805 satellite_weather_downloader-1.8.2/satellite/weather/utils/__init__.py
+-rw-r--r--   0        0        0     4871 2023-04-14 17:09:47.393805 satellite_weather_downloader-1.8.2/satellite/weather/utils/episem.py
+-rw-r--r--   0        0        0    13631 2023-04-14 17:09:47.393805 satellite_weather_downloader-1.8.2/satellite/weather/xr_extensions.py
+-rw-r--r--   0        0        0     4888 1970-01-01 00:00:00.000000 satellite_weather_downloader-1.8.2/PKG-INFO
```

### Comparing `satellite_weather_downloader-1.8.1/LICENSE` & `satellite_weather_downloader-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/README.md` & `satellite_weather_downloader-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/pyproject.toml` & `satellite_weather_downloader-1.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "satellite-weather-downloader"
-version = "1.8.1"  # changed by semantic-release
+version = "1.8.2"  # changed by semantic-release
 description = "The modules available in this package are designed to capture and proccess satellite data from Copernicus"
 readme = "README.md"
 authors = ["Luã Bida Vacaro <luabidaa@gmail.com>"]
 maintainers = ["Luã Bida Vacaro <luabidaa@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/osl-incubator/satellite-weather-downloader"
 homepage = "https://github.com/osl-incubator/satellite-weather-downloader"
```

### Comparing `satellite_weather_downloader-1.8.1/satellite/downloader/extract_reanalysis.py` & `satellite_weather_downloader-1.8.2/satellite/downloader/extract_reanalysis.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/downloader/reanalysis/api_vars.py` & `satellite_weather_downloader-1.8.2/satellite/downloader/reanalysis/api_vars.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/downloader/reanalysis/prompt.py` & `satellite_weather_downloader-1.8.2/satellite/downloader/reanalysis/prompt.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/downloader/request.py` & `satellite_weather_downloader-1.8.2/satellite/downloader/request.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas.py` & `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.dbf` & `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.dbf`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/DSEI/areas_dsei.shp` & `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/DSEI/areas_dsei.shp`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/extract_coordinates.py` & `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/extract_coordinates.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/extract_latlons.py` & `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/extract_latlons.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/weather/_brazil/municipios.json` & `satellite_weather_downloader-1.8.2/satellite/weather/_brazil/municipios.json`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/weather/utils/episem.py` & `satellite_weather_downloader-1.8.2/satellite/weather/utils/episem.py`

 * *Files identical despite different names*

### Comparing `satellite_weather_downloader-1.8.1/satellite/weather/xr_extensions.py` & `satellite_weather_downloader-1.8.2/satellite/weather/xr_extensions.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import metpy.calc as mpcalc
 import numpy as np
 import xarray as xr
 from loguru import logger
 from matplotlib.path import Path
 from metpy.units import units
 from shapely.geometry.polygon import Polygon
+from sqlalchemy import create_engine
 
 from . import _brazil
 
 xr.set_options(keep_attrs=True)
 
 
 @xr.register_dataset_accessor('copebr')
@@ -68,14 +69,41 @@
         num_geocodes = len(geocodes) if isinstance(geocodes, list) else 1
         max_workers = math.ceil((num_geocodes / 100))
         pool = ThreadPoolExecutor(max_workers=max_workers)
         return pool.submit(
             asyncio.run, self._final_dataframe(geocodes=geocodes, raw=raw)
         ).result()
 
+    def to_sql(
+        self,
+        geocodes: Union[list, int],
+        sql_uri: str,
+        tablename: str,
+        schema: str,
+        raw: bool = False,
+    ) -> None:
+        """ 
+        Reads the data for each geocode and insert the rows into the
+        database one by one, created by sqlalchemy engine with the URI.
+        This method is convenient to prevent the memory overhead when
+        executing with a large amount of geocodes.
+        """
+        geocodes = [geocodes] if isinstance(geocodes, int) else geocodes
+        for geocode in geocodes:
+            self._geocode_to_sql(
+                geocode=geocode,
+                sql_uri=sql_uri,
+                schema=schema,
+                tablename=tablename,
+                raw=raw,
+            )
+        logger.debug(
+            f'{len(geocodes)} geocodes updated on {schema}.{tablename}'
+        )
+
     def geocode_ds(self, geocode: int, raw: bool):
         return asyncio.run(self._geocode_ds(geocode, raw))
 
     async def _final_dataframe(self, geocodes: Union[list, int], raw=False):
         geocodes = [geocodes] if isinstance(geocodes, int) else geocodes
 
         tasks = []
@@ -110,19 +138,49 @@
                         but with an extra column with the geocode, in order
                         to differ the data when inserting into a database,
                         for instance.
         """
 
         ds = await self._geocode_ds(geocode, raw)
         df = dd.from_delayed(dask.delayed(ds.to_dataframe)())
+        del ds
         geocode = [geocode for g in range(len(df))]
         df = df.assign(geocodigo=da.from_array(geocode))
 
         return df
 
+    def _geocode_to_sql(
+        self,
+        geocode: int,
+        sql_uri: str,
+        schema: str,
+        tablename: str,
+        raw: bool,
+    ):
+        ds = asyncio.run(self._geocode_ds(geocode, raw))
+        df = ds.to_dataframe()
+        del ds
+        geocodes = [geocode for g in range(len(df))]
+        df = df.assign(geocodigo=geocodes)
+        df = df.reset_index(drop=False)
+        if raw:
+            df = df.rename(columns={'time': 'datetime'})
+        else:
+            df = df.rename(columns={'time': 'date'})
+
+        engine = create_engine(sql_uri)
+        with engine.connect() as conn:
+            df.to_sql(
+                name=tablename,
+                schema=schema,
+                con=conn,
+                if_exists='append',
+                index=False,
+            )
+
     async def _geocode_ds(self, geocode: int, raw=False):
         """
         This is the most important method of the extension. It will
         slice the dataset according to the geocode provided, do the
         math and the parse of the units to Br's format, and reduce by
         min, mean and max by day, if the `raw` is false.
         Attrs:
@@ -154,18 +212,16 @@
         gmin, gmean, gmax, gtot = await asyncio.gather(
             self._reduce_by(gb, np.min, 'min'),
             self._reduce_by(gb, np.mean, 'med'),
             self._reduce_by(gb, np.max, 'max'),
             self._reduce_by(gb, np.sum, 'tot'),
         )
 
-
         final_ds = xr.combine_by_coords(
-            [gmin, gmean, gmax, gtot.precip_tot], 
-            data_vars='all'
+            [gmin, gmean, gmax, gtot.precip_tot], data_vars='all'
         )
 
         return final_ds
 
     async def _get_latlons(self, geocode: int):
         """
         Extract Latitude and Longitude from a Brazilian's city
```

### Comparing `satellite_weather_downloader-1.8.1/PKG-INFO` & `satellite_weather_downloader-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satellite-weather-downloader
-Version: 1.8.1
+Version: 1.8.2
 Summary: The modules available in this package are designed to capture and proccess satellite data from Copernicus
 Home-page: https://github.com/osl-incubator/satellite-weather-downloader
 License: GNU GPL v3.0
 Author: Luã Bida Vacaro
 Author-email: luabidaa@gmail.com
 Maintainer: Luã Bida Vacaro
 Maintainer-email: luabidaa@gmail.com
```

