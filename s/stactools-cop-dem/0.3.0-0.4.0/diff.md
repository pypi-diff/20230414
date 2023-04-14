# Comparing `tmp/stactools-cop-dem-0.3.0.tar.gz` & `tmp/stactools-cop-dem-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-cop-dem-0.3.0.tar", last modified: Mon Mar 27 13:51:28 2023, max compression
+gzip compressed data, was "stactools-cop-dem-0.4.0.tar", last modified: Fri Apr 14 19:23:18 2023, max compression
```

## Comparing `stactools-cop-dem-0.3.0.tar` & `stactools-cop-dem-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:51:28.114842 stactools-cop-dem-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-27 13:51:09.000000 stactools-cop-dem-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-03-27 13:51:28.114842 stactools-cop-dem-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-27 13:51:09.000000 stactools-cop-dem-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-27 13:51:09.000000 stactools-cop-dem-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-27 13:51:28.114842 stactools-cop-dem-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:51:28.110842 stactools-cop-dem-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:51:28.110842 stactools-cop-dem-0.3.0/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:51:28.114842 stactools-cop-dem-0.3.0/src/stactools/cop_dem/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-27 13:51:09.000000 stactools-cop-dem-0.3.0/src/stactools/cop_dem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-27 13:51:09.000000 stactools-cop-dem-0.3.0/src/stactools/cop_dem/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-03-27 13:51:09.000000 stactools-cop-dem-0.3.0/src/stactools/cop_dem/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-03-27 13:51:09.000000 stactools-cop-dem-0.3.0/src/stactools/cop_dem/stac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:51:28.114842 stactools-cop-dem-0.3.0/src/stactools_cop_dem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-03-27 13:51:28.000000 stactools-cop-dem-0.3.0/src/stactools_cop_dem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-27 13:51:28.000000 stactools-cop-dem-0.3.0/src/stactools_cop_dem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 13:51:28.000000 stactools-cop-dem-0.3.0/src/stactools_cop_dem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 13:51:28.000000 stactools-cop-dem-0.3.0/src/stactools_cop_dem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-27 13:51:28.000000 stactools-cop-dem-0.3.0/src/stactools_cop_dem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:51:28.114842 stactools-cop-dem-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 13:51:09.000000 stactools-cop-dem-0.3.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-27 13:51:09.000000 stactools-cop-dem-0.3.0/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-03-27 13:51:09.000000 stactools-cop-dem-0.3.0/tests/test_stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.286964 stactools-cop-dem-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-14 19:23:18.286964 stactools-cop-dem-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-14 19:23:18.286964 stactools-cop-dem-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.278964 stactools-cop-dem-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.278964 stactools-cop-dem-0.4.0/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.282964 stactools-cop-dem-0.4.0/src/stactools/cop_dem/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/src/stactools/cop_dem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/src/stactools/cop_dem/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/src/stactools/cop_dem/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/src/stactools/cop_dem/stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.286964 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-14 19:23:18.000000 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 19:23:18.000000 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:23:18.000000 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 19:23:18.000000 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 19:23:18.000000 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.286964 stactools-cop-dem-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/tests/test_stac.py
```

### Comparing `stactools-cop-dem-0.3.0/LICENSE` & `stactools-cop-dem-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.3.0/PKG-INFO` & `stactools-cop-dem-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-cop-dem
-Version: 0.3.0
+Version: 0.4.0
 Summary: stactools package for Copernicus Digital Elevation Model
 Home-page: https://github.com/stactools-packages/cop-dem
 Author: Justin Fisk
 Author-email: misterfisk@gmail.com
 Project-URL: Documentation, https://stactools-cop-dem.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stactools-packages/cop-dem/issues
 Keywords: stactools,pystac,catalog,STAC,Copernicus,dem,elevation,raster
```

### Comparing `stactools-cop-dem-0.3.0/README.md` & `stactools-cop-dem-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.3.0/setup.cfg` & `stactools-cop-dem-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.3.0/src/stactools/cop_dem/commands.py` & `stactools-cop-dem-0.4.0/src/stactools/cop_dem/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.3.0/src/stactools/cop_dem/constants.py` & `stactools-cop-dem-0.4.0/src/stactools/cop_dem/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.3.0/src/stactools/cop_dem/stac.py` & `stactools-cop-dem-0.4.0/src/stactools/cop_dem/stac.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,83 @@
 import os.path
 import re
 from typing import Optional
 
-from pystac import (CatalogType, Collection, Extent, Asset, Summaries,
-                    SpatialExtent, TemporalExtent)
+from pystac import (
+    CatalogType,
+    Collection,
+    Extent,
+    Asset,
+    Summaries,
+    SpatialExtent,
+    TemporalExtent,
+)
+from pystac.extensions.grid import GridExtension
 from pystac.extensions.projection import ProjectionExtension
 from pystac.extensions.item_assets import ItemAssetsExtension
 from pystac.extensions.raster import (
     DataType,
     RasterBand,
     RasterExtension,
     Sampling,
 )
 from pystac.media_type import MediaType
 
 import rasterio
-from shapely.geometry import mapping, box
+from shapely.geometry import mapping, box, shape as make_shape
 from pystac import Item
 
 from stactools.core.io import ReadHrefModifier
 from stactools.cop_dem import constants as co
 
 
-def create_item(href: str,
-                read_href_modifier: Optional[ReadHrefModifier] = None,
-                host: Optional[str] = None) -> Item:
+def create_item(
+    href: str,
+    read_href_modifier: Optional[ReadHrefModifier] = None,
+    host: Optional[str] = None,
+) -> Item:
     """Creates a STAC Item from a single tile of Copernicus DEM data."""
     if read_href_modifier:
         modified_href = read_href_modifier(href)
     else:
         modified_href = href
     with rasterio.open(modified_href) as dataset:
         if dataset.crs.to_epsg() != co.COP_DEM_EPSG:
             raise ValueError(f"Dataset {href} is not EPSG:{co.COP_DEM_EPSG}, "
                              "which is required for Copernicus DEM data")
         bbox = list(dataset.bounds)
         geometry = mapping(box(*bbox))
         transform = dataset.transform
         shape = dataset.shape
-        item = Item(id=os.path.splitext(os.path.basename(href))[0],
-                    geometry=geometry,
-                    bbox=bbox,
-                    datetime=co.COP_DEM_COLLECTION_START,
-                    properties={},
-                    stac_extensions=[])
+        item = Item(
+            id=os.path.splitext(os.path.basename(href))[0],
+            geometry=geometry,
+            bbox=bbox,
+            datetime=co.COP_DEM_COLLECTION_START,
+            properties={},
+            stac_extensions=[],
+        )
 
     # resolution in arc seconds (not meters!), which is and 30 for GLO-90 and 10 for GLO-30
-    p = re.compile(r'Copernicus_DSM_COG_(\d\d)_.*')
-    m = p.match(os.path.basename(href))
-    if m:
-        if m.group(1) == '30':
+    p = re.compile(
+        r"Copernicus_DSM_COG_(?P<res>\d{2})_(?P<northing>[NS]\d{2})_00_(?P<easting>[EW]\d{3})_00_DEM.*"  # noqa: E501
+    )
+    if m := p.match(os.path.basename(href)):
+        res = m.group("res")
+        if res == "30":
             gsd = 90
-        elif m.group(1) == '10':
+        elif res == "10":
             gsd = 30
         else:
-            raise ValueError("unknown resolution {}".format(m.group(1)))
+            raise ValueError(f"unknown resolution {res}")
+
+        northing = m.group("northing")
+        easting = m.group("easting")
     else:
-        raise ValueError("unable to parse {}".format(href))
+        raise ValueError(f"unable to parse {href}")
 
     item.add_links(co.COP_DEM_LINKS)
     item.common_metadata.platform = co.COP_DEM_PLATFORM
     item.common_metadata.gsd = gsd
 
     if host and host not in co.COP_DEM_HOST.keys():
         raise ValueError(
@@ -77,27 +94,35 @@
     data_asset = Asset(
         href=href,
         title="Data",
         description=None,
         media_type=MediaType.COG,
         roles=["data"],
     )
-    data_bands = RasterBand.create(sampling=Sampling.POINT,
-                                   data_type=DataType.FLOAT32,
-                                   spatial_resolution=gsd,
-                                   unit="meter")
+    data_bands = RasterBand.create(
+        sampling=Sampling.POINT,
+        data_type=DataType.FLOAT32,
+        spatial_resolution=gsd,
+        unit="meter",
+    )
 
     item.add_asset("data", data_asset)
     RasterExtension.ext(data_asset, add_if_missing=True).bands = [data_bands]
 
     projection = ProjectionExtension.ext(item, add_if_missing=True)
     projection.epsg = co.COP_DEM_EPSG
     projection.transform = transform[0:6]
     projection.shape = shape
 
+    centroid = make_shape(item.geometry).centroid
+    projection.centroid = {"lat": centroid.y, "lon": centroid.x}
+
+    grid = GridExtension.ext(item, add_if_missing=True)
+    grid.code = f"CDEM-{northing}{easting}"
+
     return item
 
 
 def create_collection(product: str, host: Optional[str] = None) -> Collection:
     """Create a STAC Collection
 
     This function includes logic to extract all relevant metadata from
@@ -138,30 +163,33 @@
             f"Invalid host: {host}. Must be one of {list(co.COP_DEM_HOST.keys())}"
         )
     if host and (host_provider := co.COP_DEM_HOST.get(host)):
         providers = [*co.COP_DEM_PROVIDERS, host_provider]
     else:
         providers = co.COP_DEM_PROVIDERS
 
-    collection = Collection(id=f"cop-dem-{product.lower()}",
-                            title=f"Copernicus DEM {product.upper()}",
-                            description=co.COP_DEM_DESCRIPTION,
-                            license="proprietary",
-                            keywords=co.COP_DEM_KEYWORDS,
-                            catalog_type=CatalogType.RELATIVE_PUBLISHED,
-                            summaries=Summaries(summaries),
-                            extent=Extent(
-                                SpatialExtent(co.COP_DEM_SPATIAL_EXTENT),
-                                TemporalExtent([co.COP_DEM_TEMPORAL_EXTENT])),
-                            providers=providers,
-                            stac_extensions=[
-                                ItemAssetsExtension.get_schema_uri(),
-                                ProjectionExtension.get_schema_uri(),
-                                RasterExtension.get_schema_uri(),
-                            ])
+    collection = Collection(
+        id=f"cop-dem-{product.lower()}",
+        title=f"Copernicus DEM {product.upper()}",
+        description=co.COP_DEM_DESCRIPTION,
+        license="proprietary",
+        keywords=co.COP_DEM_KEYWORDS,
+        catalog_type=CatalogType.RELATIVE_PUBLISHED,
+        summaries=Summaries(summaries),
+        extent=Extent(
+            SpatialExtent(co.COP_DEM_SPATIAL_EXTENT),
+            TemporalExtent([co.COP_DEM_TEMPORAL_EXTENT]),
+        ),
+        providers=providers,
+        stac_extensions=[
+            ItemAssetsExtension.get_schema_uri(),
+            ProjectionExtension.get_schema_uri(),
+            RasterExtension.get_schema_uri(),
+        ],
+    )
 
     collection.add_links(co.COP_DEM_LINKS)
 
     assets = ItemAssetsExtension.ext(collection, add_if_missing=True)
     assets.item_assets = co.COP_DEM_ASSETS
 
     return collection
```

### Comparing `stactools-cop-dem-0.3.0/src/stactools_cop_dem.egg-info/PKG-INFO` & `stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-cop-dem
-Version: 0.3.0
+Version: 0.4.0
 Summary: stactools package for Copernicus Digital Elevation Model
 Home-page: https://github.com/stactools-packages/cop-dem
 Author: Justin Fisk
 Author-email: misterfisk@gmail.com
 Project-URL: Documentation, https://stactools-cop-dem.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stactools-packages/cop-dem/issues
 Keywords: stactools,pystac,catalog,STAC,Copernicus,dem,elevation,raster
```

### Comparing `stactools-cop-dem-0.3.0/tests/test_commands.py` & `stactools-cop-dem-0.4.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.3.0/tests/test_stac.py` & `stactools-cop-dem-0.4.0/tests/test_stac.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 from unittest import TestCase
 
 from pystac import Provider, MediaType
+from pystac.extensions.grid import GridExtension
 from pystac.extensions.projection import ProjectionExtension
 from pystac.extensions.raster import RasterExtension
 from pystac.provider import ProviderRole
 
 from stactools.cop_dem import stac
 
 from tests import test_data
@@ -56,14 +57,17 @@
         self.assertEqual(projection.epsg, 4326)
         self.assertEqual(projection.shape, (3600, 2400))
         self.assertEqual(list(projection.transform), [
             0.00041666666666666664, 0.0, -115.00020833333333, 0.0,
             -0.0002777777777777778, 54.00013888888889
         ])
 
+        grid = GridExtension.ext(item)
+        self.assertEqual(grid.code, "CDEM-N53W115")
+
         handbook = item.get_single_link("handbook")
         self.assertIsNotNone(handbook)
         self.assertEqual(handbook.title, "Copernicus DEM User handbook")
         self.assertEqual(handbook.rel, "handbook")
         self.assertEqual(
             handbook.href,
             "https://object.cloud.sdsc.edu/v1/AUTH_opentopography/www/metadata"
@@ -73,14 +77,15 @@
         data = item.assets["data"]
         self.assertEqual(data.href, self.glo30_path)
         self.assertEqual(data.title, "Data")
         self.assertIsNone(data.description)
         self.assertEqual(data.media_type, MediaType.COG)
         self.assertEqual(data.roles, ["data"])
 
+        self.assertTrue(GridExtension.has_extension(item))
         self.assertTrue(ProjectionExtension.has_extension(item))
         self.assertTrue(RasterExtension.has_extension(item))
 
         item.validate()  # raises STACValidationError if not
 
     def test_create_glo90_item(self):
         item = stac.create_item(self.glo90_path)
@@ -117,14 +122,19 @@
         projection = ProjectionExtension.ext(item)
         self.assertEqual(projection.epsg, 4326)
         self.assertEqual(projection.shape, (1200, 800))
         self.assertEqual(list(projection.transform), [
             0.00125, 0.0, -115.000625, 0.0, -0.0008333333333333334,
             54.000416666666666
         ])
+        self.assertEqual(round(projection.centroid["lat"], 5), 53.50042)
+        self.assertEqual(round(projection.centroid["lon"], 5), -114.50062)
+
+        grid = GridExtension.ext(item)
+        self.assertEqual(grid.code, "CDEM-N53W115")
 
         handbook = item.get_single_link("handbook")
         self.assertIsNotNone(handbook)
         self.assertEqual(handbook.title, "Copernicus DEM User handbook")
         self.assertEqual(handbook.rel, "handbook")
         self.assertEqual(
             handbook.href,
@@ -137,14 +147,15 @@
         self.assertEqual(data.title, "Data")
         self.assertIsNone(data.description)
         self.assertEqual(data.media_type, MediaType.COG)
         self.assertEqual(data.roles, ["data"])
 
         self.assertTrue(ProjectionExtension.has_extension(item))
         self.assertTrue(RasterExtension.has_extension(item))
+        self.assertTrue(GridExtension.has_extension(item))
 
         item.validate()  # raises STACValidationError if not
 
     def test_create_item_with_read_href_modifier(self):
         done = False
 
         def do_it(href):
```

