# Comparing `tmp/spatialcsv-0.0.7.tar.gz` & `tmp/spatialcsv-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialcsv-0.0.7.tar", last modified: Thu Apr 13 14:25:35 2023, max compression
+gzip compressed data, was "spatialcsv-0.0.8.tar", last modified: Thu Apr 13 23:18:26 2023, max compression
```

## Comparing `spatialcsv-0.0.7.tar` & `spatialcsv-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 14:25:35.402030 spatialcsv-0.0.7/
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1560 2023-04-02 12:42:12.000000 spatialcsv-0.0.7/LICENSE
--rw-r--r--   0 thomer    (1000) thomer    (1000)      122 2023-04-02 12:42:12.000000 spatialcsv-0.0.7/MANIFEST.in
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1484 2023-04-13 14:25:35.402030 spatialcsv-0.0.7/PKG-INFO
--rw-r--r--   0 thomer    (1000) thomer    (1000)      672 2023-04-12 23:58:14.000000 spatialcsv-0.0.7/README.md
--rw-r--r--   0 thomer    (1000) thomer    (1000)       38 2023-04-13 01:16:34.000000 spatialcsv-0.0.7/requirements.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)      393 2023-04-13 14:25:35.405363 spatialcsv-0.0.7/setup.cfg
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1908 2023-04-13 14:25:30.000000 spatialcsv-0.0.7/setup.py
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 14:25:35.402030 spatialcsv-0.0.7/spatialcsv/
--rw-r--r--   0 thomer    (1000) thomer    (1000)      150 2023-04-13 14:25:30.000000 spatialcsv-0.0.7/spatialcsv/__init__.py
--rw-r--r--   0 thomer    (1000) thomer    (1000)      445 2023-04-02 12:42:12.000000 spatialcsv-0.0.7/spatialcsv/cli.py
--rw-r--r--   0 thomer    (1000) thomer    (1000)     8239 2023-04-13 11:56:16.000000 spatialcsv-0.0.7/spatialcsv/spatialcsv.py
--rw-r--r--   0 thomer    (1000) thomer    (1000)      986 2023-04-13 14:20:34.000000 spatialcsv-0.0.7/spatialcsv/spatialfolium.py
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 14:25:35.402030 spatialcsv-0.0.7/spatialcsv.egg-info/
--rw-r--r--   0 thomer    (1000) thomer    (1000)     1484 2023-04-13 14:25:35.000000 spatialcsv-0.0.7/spatialcsv.egg-info/PKG-INFO
--rw-r--r--   0 thomer    (1000) thomer    (1000)      423 2023-04-13 14:25:35.000000 spatialcsv-0.0.7/spatialcsv.egg-info/SOURCES.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)       39 2023-04-13 14:25:35.000000 spatialcsv-0.0.7/spatialcsv.egg-info/dependency_links.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)       51 2023-04-13 14:25:35.000000 spatialcsv-0.0.7/spatialcsv.egg-info/entry_points.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)        1 2023-04-02 12:46:06.000000 spatialcsv-0.0.7/spatialcsv.egg-info/not-zip-safe
--rw-r--r--   0 thomer    (1000) thomer    (1000)       38 2023-04-13 14:25:35.000000 spatialcsv-0.0.7/spatialcsv.egg-info/requires.txt
--rw-r--r--   0 thomer    (1000) thomer    (1000)       11 2023-04-13 14:25:35.000000 spatialcsv-0.0.7/spatialcsv.egg-info/top_level.txt
-drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 14:25:35.402030 spatialcsv-0.0.7/tests/
--rw-r--r--   0 thomer    (1000) thomer    (1000)      402 2023-04-02 12:42:12.000000 spatialcsv-0.0.7/tests/test_spatialcsv.py
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1560 2023-04-02 12:42:12.000000 spatialcsv-0.0.8/LICENSE
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      122 2023-04-02 12:42:12.000000 spatialcsv-0.0.8/MANIFEST.in
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1484 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/PKG-INFO
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      672 2023-04-12 23:58:14.000000 spatialcsv-0.0.8/README.md
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       38 2023-04-13 01:16:34.000000 spatialcsv-0.0.8/requirements.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      393 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/setup.cfg
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1908 2023-04-13 23:17:49.000000 spatialcsv-0.0.8/setup.py
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/spatialcsv/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      150 2023-04-13 23:17:49.000000 spatialcsv-0.0.8/spatialcsv/__init__.py
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      445 2023-04-02 12:42:12.000000 spatialcsv-0.0.8/spatialcsv/cli.py
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     8782 2023-04-13 14:55:32.000000 spatialcsv-0.0.8/spatialcsv/spatialcsv.py
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      986 2023-04-13 14:20:34.000000 spatialcsv-0.0.8/spatialcsv/spatialfolium.py
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/spatialcsv.egg-info/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)     1484 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/PKG-INFO
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      423 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/SOURCES.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       39 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/dependency_links.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       51 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/entry_points.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)        1 2023-04-02 12:46:06.000000 spatialcsv-0.0.8/spatialcsv.egg-info/not-zip-safe
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       38 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/requires.txt
+-rw-r--r--   0 thomer    (1000) thomer    (1000)       11 2023-04-13 23:18:26.000000 spatialcsv-0.0.8/spatialcsv.egg-info/top_level.txt
+drwxr-xr-x   0 thomer    (1000) thomer    (1000)        0 2023-04-13 23:18:26.562468 spatialcsv-0.0.8/tests/
+-rw-r--r--   0 thomer    (1000) thomer    (1000)      402 2023-04-02 12:42:12.000000 spatialcsv-0.0.8/tests/test_spatialcsv.py
```

### Comparing `spatialcsv-0.0.7/LICENSE` & `spatialcsv-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialcsv-0.0.7/PKG-INFO` & `spatialcsv-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialcsv
-Version: 0.0.7
+Version: 0.0.8
 Summary: Easily add location points to a map from a csv
 Home-page: https://github.com/TJHomer/spatialcsv
 Author: Tracy Homer
 Author-email: thomer@mac.com
 License: GNU General Public License v3
 Keywords: spatialcsv
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `spatialcsv-0.0.7/README.md` & `spatialcsv-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `spatialcsv-0.0.7/setup.py` & `spatialcsv-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,10 +54,10 @@
     keywords='spatialcsv',
     name='spatialcsv',
     packages=find_packages(include=['spatialcsv', 'spatialcsv.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/TJHomer/spatialcsv',
-    version='0.0.7',
+    version='0.0.8',
     zip_safe=False,
 )
```

### Comparing `spatialcsv-0.0.7/spatialcsv/spatialcsv.py` & `spatialcsv-0.0.8/spatialcsv/spatialcsv.py`

 * *Files 7% similar despite different names*

```diff
@@ -240,22 +240,41 @@
         """
         import geopandas as gpd
         gdf = gpd.read_file(data)
         geojson = gdf.__geo_interface__
         self.add_geojson(geojson, name=name, **kwargs)
 
 
-    def add_geojson(self, data, **kwargs):
-        """Adds a GeoJSON layer to the map.
+    def add_geodf(self, data, name='GeoDataFrame', **kwargs)
+        """Adds a GeoDataFrame to the map
+        
+        Args:
+            data: geodataframe instance
+        """
+        geodf = ipyleaflet.GeoData(data=data, name=name, **kwargs)
+        self.add_layer(geodf)
+
+
+    def add_vector(self, data, name, **kwarags):
+        """Adds a vector layer to the map.
+        Can be GeoJson, shapefile, GeoDataFrame, etc
 
         Args:
-            data (dict): The GeoJSON data.
-            kwargs: Keyword arguments to pass to the GeoJSON layer.
+            data: the vector data
+            name: the type of data. example: 'GeoJson', 'Shapefile', 'GeoDataFrame'
+            kwargs: Keyword arguments to pass to the layer.
         """
-        import json
+        if name == "GeoJson":
+            self.add_geojson(self, data, name, **kwargs)
+        elif name == "Shapefile":
+            self.add_shp(self, data, name, **kwargs)
+        elif name == "GeoDataFrame":
+            self.add_geodf(self, data, name, **kwargs)
+        else:
+            print("This type of vector is not supported yet.")
+        
+
+
+
 
-        if isinstance(data, str):
-            with open(data, "r") as f:
-                data = json.load(f)
 
-        geojson = ipyleaflet.GeoJSON(data=data, **kwargs)
-        self.add_layer(geojson)
+
```

### Comparing `spatialcsv-0.0.7/spatialcsv/spatialfolium.py` & `spatialcsv-0.0.8/spatialcsv/spatialfolium.py`

 * *Files identical despite different names*

### Comparing `spatialcsv-0.0.7/spatialcsv.egg-info/PKG-INFO` & `spatialcsv-0.0.8/spatialcsv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialcsv
-Version: 0.0.7
+Version: 0.0.8
 Summary: Easily add location points to a map from a csv
 Home-page: https://github.com/TJHomer/spatialcsv
 Author: Tracy Homer
 Author-email: thomer@mac.com
 License: GNU General Public License v3
 Keywords: spatialcsv
 Classifier: Development Status :: 2 - Pre-Alpha
```

