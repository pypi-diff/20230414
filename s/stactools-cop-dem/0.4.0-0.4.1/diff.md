# Comparing `tmp/stactools-cop-dem-0.4.0.tar.gz` & `tmp/stactools-cop-dem-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-cop-dem-0.4.0.tar", last modified: Fri Apr 14 19:23:18 2023, max compression
+gzip compressed data, was "stactools-cop-dem-0.4.1.tar", last modified: Fri Apr 14 20:20:34 2023, max compression
```

## Comparing `stactools-cop-dem-0.4.0.tar` & `stactools-cop-dem-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.286964 stactools-cop-dem-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-14 19:23:18.286964 stactools-cop-dem-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-14 19:23:18.286964 stactools-cop-dem-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.278964 stactools-cop-dem-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.278964 stactools-cop-dem-0.4.0/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.282964 stactools-cop-dem-0.4.0/src/stactools/cop_dem/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/src/stactools/cop_dem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/src/stactools/cop_dem/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/src/stactools/cop_dem/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/src/stactools/cop_dem/stac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.286964 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-14 19:23:18.000000 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 19:23:18.000000 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:23:18.000000 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 19:23:18.000000 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 19:23:18.000000 stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:23:18.286964 stactools-cop-dem-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-14 19:23:01.000000 stactools-cop-dem-0.4.0/tests/test_stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:20:34.752169 stactools-cop-dem-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 20:20:13.000000 stactools-cop-dem-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-14 20:20:34.752169 stactools-cop-dem-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-14 20:20:13.000000 stactools-cop-dem-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 20:20:13.000000 stactools-cop-dem-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-14 20:20:34.756169 stactools-cop-dem-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:20:34.752169 stactools-cop-dem-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:20:34.752169 stactools-cop-dem-0.4.1/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:20:34.752169 stactools-cop-dem-0.4.1/src/stactools/cop_dem/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 20:20:13.000000 stactools-cop-dem-0.4.1/src/stactools/cop_dem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-14 20:20:13.000000 stactools-cop-dem-0.4.1/src/stactools/cop_dem/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-14 20:20:13.000000 stactools-cop-dem-0.4.1/src/stactools/cop_dem/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-14 20:20:13.000000 stactools-cop-dem-0.4.1/src/stactools/cop_dem/stac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:20:34.752169 stactools-cop-dem-0.4.1/src/stactools_cop_dem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-14 20:20:34.000000 stactools-cop-dem-0.4.1/src/stactools_cop_dem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 20:20:34.000000 stactools-cop-dem-0.4.1/src/stactools_cop_dem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:20:34.000000 stactools-cop-dem-0.4.1/src/stactools_cop_dem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 20:20:34.000000 stactools-cop-dem-0.4.1/src/stactools_cop_dem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 20:20:34.000000 stactools-cop-dem-0.4.1/src/stactools_cop_dem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:20:34.752169 stactools-cop-dem-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-14 20:20:13.000000 stactools-cop-dem-0.4.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-14 20:20:13.000000 stactools-cop-dem-0.4.1/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-04-14 20:20:13.000000 stactools-cop-dem-0.4.1/tests/test_stac.py
```

### Comparing `stactools-cop-dem-0.4.0/LICENSE` & `stactools-cop-dem-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.4.0/PKG-INFO` & `stactools-cop-dem-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-cop-dem
-Version: 0.4.0
+Version: 0.4.1
 Summary: stactools package for Copernicus Digital Elevation Model
 Home-page: https://github.com/stactools-packages/cop-dem
 Author: Justin Fisk
 Author-email: misterfisk@gmail.com
 Project-URL: Documentation, https://stactools-cop-dem.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stactools-packages/cop-dem/issues
 Keywords: stactools,pystac,catalog,STAC,Copernicus,dem,elevation,raster
```

### Comparing `stactools-cop-dem-0.4.0/README.md` & `stactools-cop-dem-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.4.0/setup.cfg` & `stactools-cop-dem-0.4.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 	Programming Language :: Python :: 3.11
 
 [options]
 package_dir = 
 	= src
 packages = find_namespace:
 install_requires = 
-	stactools[s3] >= 0.4.0
+	stactools[s3] >= 0.4.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `stactools-cop-dem-0.4.0/src/stactools/cop_dem/commands.py` & `stactools-cop-dem-0.4.1/src/stactools/cop_dem/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.4.0/src/stactools/cop_dem/constants.py` & `stactools-cop-dem-0.4.1/src/stactools/cop_dem/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.4.0/src/stactools/cop_dem/stac.py` & `stactools-cop-dem-0.4.1/src/stactools/cop_dem/stac.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,18 @@
 
     projection = ProjectionExtension.ext(item, add_if_missing=True)
     projection.epsg = co.COP_DEM_EPSG
     projection.transform = transform[0:6]
     projection.shape = shape
 
     centroid = make_shape(item.geometry).centroid
-    projection.centroid = {"lat": centroid.y, "lon": centroid.x}
+    projection.centroid = {
+        "lat": round(centroid.y, 1),
+        "lon": round(centroid.x, 1)
+    }
 
     grid = GridExtension.ext(item, add_if_missing=True)
     grid.code = f"CDEM-{northing}{easting}"
 
     return item
```

### Comparing `stactools-cop-dem-0.4.0/src/stactools_cop_dem.egg-info/PKG-INFO` & `stactools-cop-dem-0.4.1/src/stactools_cop_dem.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-cop-dem
-Version: 0.4.0
+Version: 0.4.1
 Summary: stactools package for Copernicus Digital Elevation Model
 Home-page: https://github.com/stactools-packages/cop-dem
 Author: Justin Fisk
 Author-email: misterfisk@gmail.com
 Project-URL: Documentation, https://stactools-cop-dem.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/stactools-packages/cop-dem/issues
 Keywords: stactools,pystac,catalog,STAC,Copernicus,dem,elevation,raster
```

### Comparing `stactools-cop-dem-0.4.0/tests/test_commands.py` & `stactools-cop-dem-0.4.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `stactools-cop-dem-0.4.0/tests/test_stac.py` & `stactools-cop-dem-0.4.1/tests/test_stac.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,16 +122,16 @@
         projection = ProjectionExtension.ext(item)
         self.assertEqual(projection.epsg, 4326)
         self.assertEqual(projection.shape, (1200, 800))
         self.assertEqual(list(projection.transform), [
             0.00125, 0.0, -115.000625, 0.0, -0.0008333333333333334,
             54.000416666666666
         ])
-        self.assertEqual(round(projection.centroid["lat"], 5), 53.50042)
-        self.assertEqual(round(projection.centroid["lon"], 5), -114.50062)
+        self.assertEqual(round(projection.centroid["lat"], 5), 53.5)
+        self.assertEqual(round(projection.centroid["lon"], 5), -114.5)
 
         grid = GridExtension.ext(item)
         self.assertEqual(grid.code, "CDEM-N53W115")
 
         handbook = item.get_single_link("handbook")
         self.assertIsNotNone(handbook)
         self.assertEqual(handbook.title, "Copernicus DEM User handbook")
```

