# Comparing `tmp/osm_annotation-0.1.8.tar.gz` & `tmp/osm_annotation-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\jixin\Documents\Bitbucket\osm_annotation\dist\.tmp-uty8t4nd\osm_annotation-0.1.8.tar", last modified: Tue Feb  7 13:51:47 2023, max compression
+gzip compressed data, was "osm_annotation-0.1.9.tar", last modified: Fri Apr 14 18:36:12 2023, max compression
```

## Comparing `osm_annotation-0.1.8.tar` & `osm_annotation-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 13:51:47.855276 osm_annotation-0.1.8/
--rw-rw-rw-   0        0        0     1083 2023-01-28 16:56:13.000000 osm_annotation-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       27 2023-01-30 20:11:31.000000 osm_annotation-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7032 2023-02-07 13:51:47.855276 osm_annotation-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     6372 2023-02-07 13:51:44.000000 osm_annotation-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-07 13:51:47.837276 osm_annotation-0.1.8/osm_annotation/
--rw-rw-rw-   0        0        0        0 2023-01-28 16:56:32.000000 osm_annotation-0.1.8/osm_annotation/__init__.py
--rw-rw-rw-   0        0        0    19872 2023-01-30 20:14:44.000000 osm_annotation-0.1.8/osm_annotation/geofabrik_database.py
-drwxrwxrwx   0        0        0        0 2023-02-07 13:51:47.853235 osm_annotation-0.1.8/osm_annotation/label_map/
--rw-rw-rw-   0        0        0     6528 2023-01-28 20:54:39.000000 osm_annotation-0.1.8/osm_annotation/label_map/osm_label_hierarchy.csv
--rw-rw-rw-   0        0        0     6570 2023-01-29 15:49:48.000000 osm_annotation-0.1.8/osm_annotation/label_map/osm_label_hierarchy_clean.csv
--rw-rw-rw-   0        0        0    12601 2023-01-30 14:57:47.000000 osm_annotation-0.1.8/osm_annotation/semantic_annotation.py
-drwxrwxrwx   0        0        0        0 2023-02-07 13:51:47.847267 osm_annotation-0.1.8/osm_annotation.egg-info/
--rw-rw-rw-   0        0        0     7032 2023-02-07 13:51:47.000000 osm_annotation-0.1.8/osm_annotation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-02-07 13:51:47.000000 osm_annotation-0.1.8/osm_annotation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 13:51:47.000000 osm_annotation-0.1.8/osm_annotation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-02-07 13:51:47.000000 osm_annotation-0.1.8/osm_annotation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      137 2023-01-30 19:56:26.000000 osm_annotation-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      764 2023-02-07 13:51:47.857235 osm_annotation-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1016 2023-02-07 13:51:36.000000 osm_annotation-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:36:12.625673 osm_annotation-0.1.9/
+-rw-rw-rw-   0        0        0     1083 2023-04-14 13:03:19.000000 osm_annotation-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-04-14 13:03:19.000000 osm_annotation-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7488 2023-04-14 18:36:12.625673 osm_annotation-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6828 2023-04-14 13:08:48.000000 osm_annotation-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 18:36:12.617672 osm_annotation-0.1.9/osm_annotation/
+-rw-rw-rw-   0        0        0        0 2023-04-14 13:03:19.000000 osm_annotation-0.1.9/osm_annotation/__init__.py
+-rw-rw-rw-   0        0        0    20704 2023-04-14 14:00:35.000000 osm_annotation-0.1.9/osm_annotation/geofabrik_database.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:36:12.625673 osm_annotation-0.1.9/osm_annotation/label_map/
+-rw-rw-rw-   0        0        0     6646 2023-04-14 13:03:19.000000 osm_annotation-0.1.9/osm_annotation/label_map/osm_label_hierarchy.csv
+-rw-rw-rw-   0        0        0     6570 2023-04-14 13:03:19.000000 osm_annotation-0.1.9/osm_annotation/label_map/osm_label_hierarchy_clean.csv
+-rw-rw-rw-   0        0        0    13796 2023-04-14 14:17:48.000000 osm_annotation-0.1.9/osm_annotation/semantic_annotation.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:36:12.622673 osm_annotation-0.1.9/osm_annotation.egg-info/
+-rw-rw-rw-   0        0        0     7488 2023-04-14 18:36:12.000000 osm_annotation-0.1.9/osm_annotation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-04-14 18:36:12.000000 osm_annotation-0.1.9/osm_annotation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 18:36:12.000000 osm_annotation-0.1.9/osm_annotation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 18:36:12.000000 osm_annotation-0.1.9/osm_annotation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      139 2023-04-14 18:36:09.000000 osm_annotation-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      764 2023-04-14 18:36:12.627673 osm_annotation-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2023-04-14 14:19:18.000000 osm_annotation-0.1.9/setup.py
```

### Comparing `osm_annotation-0.1.8/LICENSE` & `osm_annotation-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `osm_annotation-0.1.8/PKG-INFO` & `osm_annotation-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm_annotation
-Version: 0.1.8
+Version: 0.1.9
 Summary: An easy-to-use Python package that annotate location data with semantic labels from OpenStreetMap
 Home-page: https://bitbucket.org/mhealthresearchgroup/osm_annotation/src/main/
 Author: Jixin Li
 Author-email: li.jix@northeastern.edu
 Project-URL: Bug Tracker, https://bitbucket.org/mhealthresearchgroup/osm_annotation/issues?status=new&status=open
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,27 +12,27 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # location_annotation_with_openstreetmap
 This is an easy-to-use Python package for annotating location data with OpenStreetMap Point-of-interest tags. It provides a solution for researchers to adding additional layer of context information to location data at large scale in an automatic way. For example, the input can be pairs of coordinates (lat, lon), and the output are types of places of the input locations, such as "gym", "restaurant", "university", "office", etc. Annotation using this package incurs no cost when this package downloads and uses free POI data from [Geofabrik](https://www.geofabrik.de/) that reflect daily changes from [OpenStreetMap](https://en.wikipedia.org/wiki/OpenStreetMap). For questions about this package, please leave an [issue](https://bitbucket.org/mhealthresearchgroup/osm_annotation/issues?status=new&status=open) or contact the [author](mailto:li.jix@northeastern.edu).
 
-### Author and Credits
-Jixin Li, mHealth research group@Northeastern University  
-
-This package integrates the geodf and dist functions from the GPS2space package (https://gps2space.readthedocs.io/en/latest/).  
-
-A paper is in submission. If you use this package, please cite it as below.  
-> Li, Jixin. (2023). osm_annotation (version 0.1.8) [Python package]. https://bitbucket.org/mhealthresearchgroup/osm_annotation/src/main/
-
-
 ### Two general steps
 **1. Download and create a geofabrik POI database in local system**  
 **2. Annotate location data using the POI database**  
 
+## Contact
+- Author: Jixin Li @ [mHealth research group](https://www.mhealthgroup.org/)
+- For questions about this package, please leave an [issue](https://bitbucket.org/mhealthresearchgroup/osm_annotation/issues?status=new&status=open&is_spam=!spam).
+  
+## Citation
+- This repository is a part of journal paper submission that is currently under review. Full citation information will come soon. In the meanwhile, please cite as below:
+> Jixin Li. 2023. location_annotation_with_openstreetmap (osm_annotation). https://bitbucket.org/mhealthresearchgroup/osm_annotation/src/main/ 
+- This package also integrates the geodf and dist functions from the GPS2space package (https://gps2space.readthedocs.io/en/latest/).
+
 ## Dependencies
 - geopandas
 - fiona
 - gps2space
 - tqdm
 - Python >= 3.7
 
@@ -76,59 +76,72 @@
 ```python
 # coordinates of Fenway Park in Boston
 centroid_latitude = 42.34653831212525
 centroid_longitude = -71.09724395926423
 semantic_annotator.annotate_single_point(centroid_latitude, centroid_longitude)
 ```
 
-Returned result is a json file with
-- matched_labels: semantic label matched with the query point
-- min_distance: the distance from the query point to the matched POI, in meters
-- distances_to_pois: distance to other types of POIs
-> {'matched_labels': 'recreational;outdoor;pitch (polygon)',
- 'min_distance': 6.169761255410299,
- 'distances_to_pois': {'busines;busines;company (polygon)': 326501.593160387,
-  'busines;busines;convention_center (polygon)': 2682942.101031607,
-  'busines;busines;factory (polygon)': 3612.955363467255,
-  'busines;busines;industrial (polygon)': 486.88772114370636,
-  'busines;busines;office (polygon)': 932.2980449124797,
-  'commercial;food;bakery (point)': 738.1374807550822,
-> ...
-> }
+Returned result is a json file with  
+    - matched_labels: semantic label matched with the query point  
+    - min_distance: the distance from the query point to the matched POI, in meters  
+    - distances_to_pois: distance to other types of POIs  
+    
+```json
+   {  
+    'matched_labels': 'recreational;outdoor;pitch (polygon)',  
+    'min_distance': 6.169761255410299,  
+    'distances_to_pois': {  
+        'busines;busines;company (polygon)': 326501.593160387,  
+        'busines;busines;convention_center (polygon)': 2682942.101031607,  
+        'busines;busines;factory (polygon)': 3612.955363467255,  
+        'busines;busines;industrial (polygon)': 486.88772114370636,  
+        'busines;busines;office (polygon)': 932.2980449124797,  
+        'commercial;food;bakery (point)': 738.1374807550822,  
+        ...
+   }
+```
 
 
 ### Example of Method 2
 ```python
 # bounding box (NW corner,NE corner, SE corner, SW corner) of Museum of Fine Arts in Boston
 lat_list = [42.33969558839377, 42.34039653732734, 42.339235761638996, 42.33847311473655]
 lon_list = [-71.09563225696323, -71.09348529667446, -71.09270768730832, -71.0948470612041]
 semantic_annotator.annotate_single_shape(lat_list, lon_list)
 ```
 
-Returned result is a json file with
-- matched_labels: semantic labels matched with the query shape
-- point_labels: semantic labels of point POI matched with the query shape
-- poly_labels: semantic labels of polygon POI matched with the query shape
+Returned result is a json file with  
+- matched_labels: semantic labels matched with the query shape  
+- point_labels: semantic labels of point POI matched with the query shape  
+- poly_labels: semantic labels of polygon POI matched with the query shape  
 - matched_geometries: geometries of POIs matched with the query shape
-> {'matched_labels': ['commercial;food;cafe (point)',
-  'commercial;shopping;shop (point)',
-  'commercial;leisure;museum (polygon)',
-  'service;transportation;parking (polygon)',
-  'recreational;outdoor;nature (polygon)'],
- 'point_labels': ['commercial;food;cafe (point)',
-  'commercial;shopping;shop (point)'],
- 'poly_labels': ['commercial;leisure;museum (polygon)',
-  'recreational;outdoor;nature (polygon)',
-  'service;transportation;parking (polygon)'],
- 'matched_geometries': [<shapely.geometry.point.Point at 0x2b8b25338410>,
-  <shapely.geometry.polygon.Polygon at 0x2b8b25353b10>,
-  <shapely.geometry.point.Point at 0x2b8b253415d0>,
-  <shapely.geometry.polygon.Polygon at 0x2b8b250b0910>,
-  <shapely.geometry.polygon.Polygon at 0x2b8b25331690>]}
 
+```json
+   {
+    'matched_labels': 
+       ['commercial;food;cafe (point)',
+       'commercial;shopping;shop (point)',
+       'commercial;leisure;museum (polygon)',
+       'service;transportation;parking (polygon)',
+       'recreational;outdoor;nature (polygon)'],
+    'point_labels': 
+       ['commercial;food;cafe (point)',
+       'commercial;shopping;shop (point)'],
+    'poly_labels': 
+       ['commercial;leisure;museum (polygon)',
+       'recreational;outdoor;nature (polygon)',
+       'service;transportation;parking (polygon)'],
+    'matched_geometries': 
+        [<shapely.geometry.point.Point at 0x2b8b25338410>,
+        <shapely.geometry.polygon.Polygon at 0x2b8b25353b10>,
+        <shapely.geometry.point.Point at 0x2b8b253415d0>,
+        <shapely.geometry.polygon.Polygon at 0x2b8b250b0910>,
+        <shapely.geometry.polygon.Polygon at 0x2b8b25331690>]
+   }
+```
 
 
 ### Example of Method 3
 ```python
 # library, cafe, gym, and train station around the Northeastern University campus
 locations = [[42.33833,-71.08795], # library
              [42.33909,-71.08758], # cafe
@@ -138,8 +151,8 @@
 semantic_annotator.annotate_batch_points(dataframe = location_dataframe, latitude_colname = 'latitude', longitude_colname = 'longitude')
 ```
 
 Returned result is a dataframe with
 - matched_labels: semantic labels matched with the query points
 - min_distance: the distance from the query point to the matched POI, in meters
 
-![alt text](https://github.com/rexli999/location_annotation_with_openstreetmap/blob/main/batch_results.png "batch result")
+![Batch_result](batch_results.png)
```

### Comparing `osm_annotation-0.1.8/README.md` & `osm_annotation-0.1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # location_annotation_with_openstreetmap
 This is an easy-to-use Python package for annotating location data with OpenStreetMap Point-of-interest tags. It provides a solution for researchers to adding additional layer of context information to location data at large scale in an automatic way. For example, the input can be pairs of coordinates (lat, lon), and the output are types of places of the input locations, such as "gym", "restaurant", "university", "office", etc. Annotation using this package incurs no cost when this package downloads and uses free POI data from [Geofabrik](https://www.geofabrik.de/) that reflect daily changes from [OpenStreetMap](https://en.wikipedia.org/wiki/OpenStreetMap). For questions about this package, please leave an [issue](https://bitbucket.org/mhealthresearchgroup/osm_annotation/issues?status=new&status=open) or contact the [author](mailto:li.jix@northeastern.edu).
 
-### Author and Credits
-Jixin Li, mHealth research group@Northeastern University  
-
-This package integrates the geodf and dist functions from the GPS2space package (https://gps2space.readthedocs.io/en/latest/).  
-
-A paper is in submission. If you use this package, please cite it as below.  
-> Li, Jixin. (2023). osm_annotation (version 0.1.8) [Python package]. https://bitbucket.org/mhealthresearchgroup/osm_annotation/src/main/
-
-
 ### Two general steps
 **1. Download and create a geofabrik POI database in local system**  
 **2. Annotate location data using the POI database**  
 
+## Contact
+- Author: Jixin Li @ [mHealth research group](https://www.mhealthgroup.org/)
+- For questions about this package, please leave an [issue](https://bitbucket.org/mhealthresearchgroup/osm_annotation/issues?status=new&status=open&is_spam=!spam).
+  
+## Citation
+- This repository is a part of journal paper submission that is currently under review. Full citation information will come soon. In the meanwhile, please cite as below:
+> Jixin Li. 2023. location_annotation_with_openstreetmap (osm_annotation). https://bitbucket.org/mhealthresearchgroup/osm_annotation/src/main/ 
+- This package also integrates the geodf and dist functions from the GPS2space package (https://gps2space.readthedocs.io/en/latest/).
+
 ## Dependencies
 - geopandas
 - fiona
 - gps2space
 - tqdm
 - Python >= 3.7
 
@@ -61,59 +61,72 @@
 ```python
 # coordinates of Fenway Park in Boston
 centroid_latitude = 42.34653831212525
 centroid_longitude = -71.09724395926423
 semantic_annotator.annotate_single_point(centroid_latitude, centroid_longitude)
 ```
 
-Returned result is a json file with
-- matched_labels: semantic label matched with the query point
-- min_distance: the distance from the query point to the matched POI, in meters
-- distances_to_pois: distance to other types of POIs
-> {'matched_labels': 'recreational;outdoor;pitch (polygon)',
- 'min_distance': 6.169761255410299,
- 'distances_to_pois': {'busines;busines;company (polygon)': 326501.593160387,
-  'busines;busines;convention_center (polygon)': 2682942.101031607,
-  'busines;busines;factory (polygon)': 3612.955363467255,
-  'busines;busines;industrial (polygon)': 486.88772114370636,
-  'busines;busines;office (polygon)': 932.2980449124797,
-  'commercial;food;bakery (point)': 738.1374807550822,
-> ...
-> }
+Returned result is a json file with  
+    - matched_labels: semantic label matched with the query point  
+    - min_distance: the distance from the query point to the matched POI, in meters  
+    - distances_to_pois: distance to other types of POIs  
+    
+```json
+   {  
+    'matched_labels': 'recreational;outdoor;pitch (polygon)',  
+    'min_distance': 6.169761255410299,  
+    'distances_to_pois': {  
+        'busines;busines;company (polygon)': 326501.593160387,  
+        'busines;busines;convention_center (polygon)': 2682942.101031607,  
+        'busines;busines;factory (polygon)': 3612.955363467255,  
+        'busines;busines;industrial (polygon)': 486.88772114370636,  
+        'busines;busines;office (polygon)': 932.2980449124797,  
+        'commercial;food;bakery (point)': 738.1374807550822,  
+        ...
+   }
+```
 
 
 ### Example of Method 2
 ```python
 # bounding box (NW corner,NE corner, SE corner, SW corner) of Museum of Fine Arts in Boston
 lat_list = [42.33969558839377, 42.34039653732734, 42.339235761638996, 42.33847311473655]
 lon_list = [-71.09563225696323, -71.09348529667446, -71.09270768730832, -71.0948470612041]
 semantic_annotator.annotate_single_shape(lat_list, lon_list)
 ```
 
-Returned result is a json file with
-- matched_labels: semantic labels matched with the query shape
-- point_labels: semantic labels of point POI matched with the query shape
-- poly_labels: semantic labels of polygon POI matched with the query shape
+Returned result is a json file with  
+- matched_labels: semantic labels matched with the query shape  
+- point_labels: semantic labels of point POI matched with the query shape  
+- poly_labels: semantic labels of polygon POI matched with the query shape  
 - matched_geometries: geometries of POIs matched with the query shape
-> {'matched_labels': ['commercial;food;cafe (point)',
-  'commercial;shopping;shop (point)',
-  'commercial;leisure;museum (polygon)',
-  'service;transportation;parking (polygon)',
-  'recreational;outdoor;nature (polygon)'],
- 'point_labels': ['commercial;food;cafe (point)',
-  'commercial;shopping;shop (point)'],
- 'poly_labels': ['commercial;leisure;museum (polygon)',
-  'recreational;outdoor;nature (polygon)',
-  'service;transportation;parking (polygon)'],
- 'matched_geometries': [<shapely.geometry.point.Point at 0x2b8b25338410>,
-  <shapely.geometry.polygon.Polygon at 0x2b8b25353b10>,
-  <shapely.geometry.point.Point at 0x2b8b253415d0>,
-  <shapely.geometry.polygon.Polygon at 0x2b8b250b0910>,
-  <shapely.geometry.polygon.Polygon at 0x2b8b25331690>]}
 
+```json
+   {
+    'matched_labels': 
+       ['commercial;food;cafe (point)',
+       'commercial;shopping;shop (point)',
+       'commercial;leisure;museum (polygon)',
+       'service;transportation;parking (polygon)',
+       'recreational;outdoor;nature (polygon)'],
+    'point_labels': 
+       ['commercial;food;cafe (point)',
+       'commercial;shopping;shop (point)'],
+    'poly_labels': 
+       ['commercial;leisure;museum (polygon)',
+       'recreational;outdoor;nature (polygon)',
+       'service;transportation;parking (polygon)'],
+    'matched_geometries': 
+        [<shapely.geometry.point.Point at 0x2b8b25338410>,
+        <shapely.geometry.polygon.Polygon at 0x2b8b25353b10>,
+        <shapely.geometry.point.Point at 0x2b8b253415d0>,
+        <shapely.geometry.polygon.Polygon at 0x2b8b250b0910>,
+        <shapely.geometry.polygon.Polygon at 0x2b8b25331690>]
+   }
+```
 
 
 ### Example of Method 3
 ```python
 # library, cafe, gym, and train station around the Northeastern University campus
 locations = [[42.33833,-71.08795], # library
              [42.33909,-71.08758], # cafe
@@ -123,8 +136,8 @@
 semantic_annotator.annotate_batch_points(dataframe = location_dataframe, latitude_colname = 'latitude', longitude_colname = 'longitude')
 ```
 
 Returned result is a dataframe with
 - matched_labels: semantic labels matched with the query points
 - min_distance: the distance from the query point to the matched POI, in meters
 
-![alt text](https://github.com/rexli999/location_annotation_with_openstreetmap/blob/main/batch_results.png "batch result")
+![Batch_result](batch_results.png)
```

### Comparing `osm_annotation-0.1.8/osm_annotation/geofabrik_database.py` & `osm_annotation-0.1.9/osm_annotation/geofabrik_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -334,28 +334,38 @@
 
     end_time = time.time()
     print("End:  all state shapefiles have been extracted and reorganized.")
     print("Total runtime is {} min".format((end_time - start_time) / 60))
     print("")
     return
 
+def _save_shp_file(df, df_folder_path, lvl3, suffix, shp_break_row_num):
+    shp_break_num = len(df) // shp_break_row_num + 1
+    df_split = np.array_split(df, shp_break_num)
+
+    for i in range(shp_break_num):
+        df_save_path = os.path.join(df_folder_path, lvl3 + str(i+1) + suffix)
+        df_split[i].to_file(df_save_path)
+    return
 
 def _rearrange_shapefiles(organized_data_folder_path, combined_data_folder_path):
     """combine files for states and layers.
 
     Parameters:
        global variables
     Returns:
        None
     """
 
     print("======================================================================================================")
     print("Start rearrange shapefiles (last step, this process may take about 3 hours)")
     start_time = time.time()
     start = 0
+    shp_break_row_num = 10000000
+
     for lvl1 in tqdm(os.listdir(organized_data_folder_path)):
         print(lvl1)
         lvl1_path = os.path.join(organized_data_folder_path, lvl1)
         for lvl2 in os.listdir(lvl1_path):
             print("  " + lvl2)
             lvl2_path = os.path.join(lvl1_path, lvl2)
             for lvl3 in os.listdir(lvl2_path):
@@ -384,28 +394,32 @@
                         if df_line.shape[0] > 0:
                             df_point = df_point[df_point['geo_type'] == shapely.geometry.point.Point]
                             df_line.reset_index(inplace=True, drop=True)
                             df_point.reset_index(inplace=True, drop=True)
                             df_point = df_point.drop('geo_type', 1)
                             df_line = df_line.drop('geo_type', 1)
                             if df_point.shape[0] > 0:
-                                df_point.to_file(df_point_path)
-                            df_line.to_file(df_line_path)
+                                _save_shp_file(df_point, df_folder_path, lvl3, "_point.shp", shp_break_row_num)
+                                # df_point.to_file(df_point_path)
+                            # df_line.to_file(df_line_path)
+                            _save_shp_file(df_line, df_folder_path, lvl3, "_line.shp", shp_break_row_num)
                         else:
                             df_point = df_point.drop('geo_type', 1)
                             df_point.reset_index(inplace=True, drop=True)
-                            df_point.to_file(df_point_path)
+                            # df_point.to_file(df_point_path)
+                            _save_shp_file(df_point, df_folder_path, lvl3, "_point.shp", shp_break_row_num)
 
                 if not os.path.exists(df_polygon_path):
                     for target_file in glob(os.path.join(lvl3_path, "*polygon.shp")):
                         shpfile_df = gpd.read_file(target_file)
                         df_polygon = df_polygon.append(shpfile_df)
                     if df_polygon.shape[0] > 0:
                         df_polygon.reset_index(inplace=True, drop=True)
-                        df_polygon.to_file(df_polygon_path)
+                        # df_polygon.to_file(df_polygon_path)
+                        _save_shp_file(df_polygon, df_folder_path, lvl3, "_polygon.shp", shp_break_row_num)
 
     end_time = time.time()
     print("Runtime of the program is {} min".format((end_time - start_time) / 60))
 
 
 def build(database_folder_path):
     """builds a local database of Geofabrik shapefiles in designated folder path.
```

### Comparing `osm_annotation-0.1.8/osm_annotation/label_map/osm_label_hierarchy.csv` & `osm_annotation-0.1.9/osm_annotation/label_map/osm_label_hierarchy.csv`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-Level 1,Level 2,Level 3,Synonyms,,,,,,,,,,,,,,,,,,,,,,,,
-Residential,,,,,,,,,,,,,,,,,,,,,,,,,,,
-,Residential,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,apartment,apartments,studio,,,,,,,,,,,,,,,,,,,,,,,
-,,dormitory,dorm,fraternity house,fraternity,,,,,,,,,,,,,,,,,,,,,,
-,,house,House,Carriage_House,deckhouse,semidetached_house,townhouse,condominiums,Condos,condominum,affordable housing,,,,,,,,,,,,,,,,
-,,residential,bungalow,cabin,hut,lodge,mansion,mobile_home,residence,,,,,,,,,,,,,,,,,,
-,,Home,,,,,,,,,,,,,,,,,,,,,,,,,
-Service,,,,,,,,,,,,,,,,,,,,,,,,,,,
-,Education,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,college,college_building,,,,,,,,,,,,,,,,,,,,,,,,
-,,childcare,childcare facility,Day Care,,,,,,,,,,,,,,,,,,,,,,,
-,,Preschool,,,,,,,,,,,,,,,,,,,,,,,,,
-,,kindergarten,,,,,,,,,,,,,,,,,,,,,,,,,
-,,school,High School,music_school,classroom,,,,,,,,,,,,,,,,,,,,,,
-,,library,university library,,,,,,,,,,,,,,,,,,,,,,,,
-,,university,,,,,,,,,,,,,,,,,,,,,,,,,
-,,education,academic,academic_building,,,,,,,,,,,,,,,,,,,,,,,
-,Health,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,clinic,,,,,,,,,,,,,,,,,,,,,,,,,
-,,dentist,Dentist_Office,,,,,,,,,,,,,,,,,,,,,,,,
-,,doctor,doctors,,,,,,,,,,,,,,,,,,,,,,,,
-,,hospital,,,,,,,,,,,,,,,,,,,,,,,,,
-,,pharmacy,,,,,,,,,,,,,,,,,,,,,,,,,
-,,Health_Center,,,,,,,,,,,,,,,,,,,,,,,,,
-,,nursing_home,,,,,,,,,,,,,,,,,,,,,,,,,
-,,medical,,,,,,,,,,,,,,,,,,,,,,,,,
-,,health,healthcare,,,,,,,,,,,,,,,,,,,,,,,,
-,,mental_health_clinic,,,,,,,,,,,,,,,,,,,,,,,,,
-,Religious,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,buddhist,christian,christian_anglican,christian_catholic,christian_evangelical,christian_lutheran,christian_methodist,christian_orthodox,christian_protestant,hindu,jewish,muslim,muslim_shia,muslim_sunni,sikh,taoist,cathedral,chapel,church,monastery,mosque,religion,presbytery,religious,,
-,Transportation,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,transportation,,,,,,,,,,,,,,,,,,,,,,,,,
-,,airport,airfield,helipad,apron,,,,,,,,,,,,,,,,,,,,,,
-,,bus_station,bus_stop,,,,,,,,,,,,,,,,,,,,,,,,
-,,train_station,railway_station,railway_halt,tram_stop,subway_entrance,,,,,,,,,,,,,,,,,,,,,
-,,car_rental,car_sharing,,,,,,,,,,,,,,,,,,,,,,,,
-,,taxi,taxi_rank,,,,,,,,,,,,,,,,,,,,,,,,
-,,ferry_terminal,,,,,,,,,,,,,,,,,,,,,,,,,
-,,fuel,service,Gas_Station,,,,,,,,,,,,,,,,,,,,,,,
-,,parking,garage,garages,parking_multistorey,parking_underground,vending_parking,parking_site,parking_lot,car_park,parking_structure,parking_space,,,,,,,,,,,,,,,
-,,parking_bicycle,,,,,,,,,,,,,,,,,,,,,,,,,
-,Finance,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,bank,,,,,,,,,,,,,,,,,,,,,,,,,
-,,atm,,,,,,,,,,,,,,,,,,,,,,,,,
-,Other,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,government,Government,courthouse,embassy,municipal,town_hall,,,,,,,,,,,,,,,,,,,,
-,,police,Police Station,,,,,,,,,,,,,,,,,,,,,,,,
-,,post_office,post_box,Post_Office,US_Post_Office,,,,,,,,,,,,,,,,,,,,,,
-,,community_centre,community_center,,,,,,,,,,,,,,,,,,,,,,,,
-,,fire_station,Fire_Department,fire_department,,,,,,,,,,,,,,,,,,,,,,,
-,,prison,Jail_House,jail,,,,,,,,,,,,,,,,,,,,,,,
-,,telephone,,,,,,,,,,,,,,,,,,,,,,,,,
-,,public_building,,,,,,,,,,,,,,,,,,,,,,,,,
-Commercial,,,,,,,,,,,,,,,,,,,,,,,,,,,
-,Leisure,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,cinema,,,,,,,,,,,,,,,,,,,,,,,,,
-,,bar,pub,nightclub,,,,,,,,,,,,,,,,,,,,,,,
-,,theatre,theater,concert_hall,,,,,,,,,,,,,,,,,,,,,,,
-,,theme_park,,,,,,,,,,,,,,,,,,,,,,,,,
-,,zoo,,,,,,,,,,,,,,,,,,,,,,,,,
-,,museum,arts_centre,arts_center,,,,,,,,,,,,,,,,,,,,,,,
-,,casino,,,,,,,,,,,,,,,,,,,,,,,,,
-,Shopping,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,kiosk,newsagent,vending_machine,vending_cigarette,vending_any,,,,,,,,,,,,,,,,,,,,,
-,,shop,clothes,shoe_shop,outdoor_shop,bicycle_shop,bookshop,car_dealership,computer_shop,furniture_shop,gift_shop,jeweller,mobile_phone_shop,sports_shop,stationery,toy_shop,video_shop,store,retail,optician,garden_centre,general,florist,chemist,retail_store,Store,shopping
-,,supermarket,butcher,convenience,greengrocer,grocery_store,Grocery,,,,,,,,,,,,,,,,,,,,
-,,mall,department_store,market_place,shopping_center,,,,,,,,,,,,,,,,,,,,,,
-,Food,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,beverages,biergarten,,,,,,,,,,,,,,,,,,,,,,,,
-,,deli,,,,,,,,,,,,,,,,,,,,,,,,,
-,,restaurant,food_court,,,,,,,,,,,,,,,,,,,,,,,,
-,,cafe,coffee shop,,,,,,,,,,,,,,,,,,,,,,,,
-,,bakery,,,,,,,,,,,,,,,,,,,,,,,,,
-,,fast_food,,,,,,,,,,,,,,,,,,,,,,,,,
-,,food_and_drink,food,,,,,,,,,,,,,,,,,,,,,,,,
-,Lifestyle,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,laundry,,,,,,,,,,,,,,,,,,,,,,,,,
-,,beauty_shop,hairdresser,,,,,,,,,,,,,,,,,,,,,,,,
-,,car_wash,car_repair,,,,,,,,,,,,,,,,,,,,,,,,
-,,hotel,hostel,motel,bed_and_breakfast,guesthouse,chalet,inn,,,,,,,,,,,,,,,,,,,
-,,recycling,recycling_clothes,recycling_glass,recycling_metal,recycling_paper,,,,,,,,,,,,,,,,,,,,,
-,,stadium,,,,,,,,,,,,,,,,,,,,,,,,,
-,,veterinary,,,,,,,,,,,,,,,,,,,,,,,,,
-,,travel_agent,,,,,,,,,,,,,,,,,,,,,,,,,
-,other,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,commercial,commercial;greenhous,commercial;yes,,,,,,,,,,,,,,,,,,,,,,,
-Business,,,,,,,,,,,,,,,,,,,,,,,,,,,
-,Business,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,industrial,,,,,,,,,,,,,,,,,,,,,,,,,
-,,office,,,,,,,,,,,,,,,,,,,,,,,,,
-,,company,,,,,,,,,,,,,,,,,,,,,,,,,
-,,factory,quarry,power_station,,,,,,,,,,,,,,,,,,,,,,,
-,,convention_center,convention_centre,conference_center,,,,,,,,,,,,,,,,,,,,,,,
-Recreational,,,,,,,,,,,,,,,,,,,,,,,,,,,
-,Indoor,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,sports_centre,Sports House,sports_complex,sports_hall,recreational_center,Gymnasium,Gym,,,,,,,,,,,,,,,,,,,
-,,swimming_pool,,,,,,,,,,,,,,,,,,,,,,,,,
-,Outdoor,,,,,,,,,,,,,,,,,,,,,,,,,,
-,,nature,beach,cave_entrance,cliff,glacier,peak,spring,tree,volcano,nature_reserve,forest,meadow,orchard,vineyard,scrub,grass,national_park,basin,,,,,,,,
-,,water,waterfall,reservoir,river,dock,glacier,wetland,,,,,,,,,,,,,,,,,,,
-,,park,allotments,recreation_ground,village_green,,,,,,,,,,,,,,,,,,,,,,
-,,farm,farmland,farmyard,,,,,,,,,,,,,,,,,,,,,,,
-,,bicycle_rental,,,,,,,,,,,,,,,,,,,,,,,,,
-,,golf_course,,,,,,,,,,,,,,,,,,,,,,,,,
-,,dog_park,,,,,,,,,,,,,,,,,,,,,,,,,
-,,ice_rink,Ice_Skating_Rink,,,,,,,,,,,,,,,,,,,,,,,,
-,,picnic_site,,,,,,,,,,,,,,,,,,,,,,,,,
-,,pitch,,,,,,,,,,,,,,,,,,,,,,,,,
-,,playground,Playground,,,,,,,,,,,,,,,,,,,,,,,,
-,,track,,,,,,,,,,,,,,,,,,,,,,,,,
-,,viewpoint,observation_tower,,,,,,,,,,,,,,,,,,,,,,,,
-,,attraction,monument,memorial,castle,ruins,archaeological,battlefield,fort,aerialway_station,,,,,,,,,,,,,,,,,
-,,hunting_stand,,,,,,,,,,,,,,,,,,,,,,,,,
-,,graveyard,cemetery,,,,,,,,,,,,,,,,,,,,,,,,
-,,tennis_court,,,,,,,,,,,,,,,,,,,,,,,,,
-,,shelter,alpine_hut,,,,,,,,,,,,,,,,,,,,,,,,
-,,camp_site,caravan_site,,,,,,,,,,,,,,,,,,,,,,,,
+Level 1,Level 2,Level 3,Synonyms,,,,,,,,,,,,,,,,,,,,,,,,
+Residential,,,,,,,,,,,,,,,,,,,,,,,,,,,
+,Residential,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,apartment,apartments,studio,,,,,,,,,,,,,,,,,,,,,,,
+,,dormitory,dorm,fraternity house,fraternity,,,,,,,,,,,,,,,,,,,,,,
+,,house,House,Carriage_House,deckhouse,semidetached_house,townhouse,condominiums,Condos,condominum,affordable housing,,,,,,,,,,,,,,,,
+,,residential,bungalow,cabin,hut,lodge,mansion,mobile_home,residence,,,,,,,,,,,,,,,,,,
+,,Home,,,,,,,,,,,,,,,,,,,,,,,,,
+Service,,,,,,,,,,,,,,,,,,,,,,,,,,,
+,Education,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,college,college_building,,,,,,,,,,,,,,,,,,,,,,,,
+,,childcare,childcare facility,Day Care,,,,,,,,,,,,,,,,,,,,,,,
+,,Preschool,,,,,,,,,,,,,,,,,,,,,,,,,
+,,kindergarten,,,,,,,,,,,,,,,,,,,,,,,,,
+,,school,High School,music_school,classroom,,,,,,,,,,,,,,,,,,,,,,
+,,library,university library,,,,,,,,,,,,,,,,,,,,,,,,
+,,university,,,,,,,,,,,,,,,,,,,,,,,,,
+,,education,academic,academic_building,,,,,,,,,,,,,,,,,,,,,,,
+,Health,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,clinic,,,,,,,,,,,,,,,,,,,,,,,,,
+,,dentist,Dentist_Office,,,,,,,,,,,,,,,,,,,,,,,,
+,,doctor,doctors,,,,,,,,,,,,,,,,,,,,,,,,
+,,hospital,,,,,,,,,,,,,,,,,,,,,,,,,
+,,pharmacy,,,,,,,,,,,,,,,,,,,,,,,,,
+,,Health_Center,,,,,,,,,,,,,,,,,,,,,,,,,
+,,nursing_home,,,,,,,,,,,,,,,,,,,,,,,,,
+,,medical,,,,,,,,,,,,,,,,,,,,,,,,,
+,,health,healthcare,,,,,,,,,,,,,,,,,,,,,,,,
+,,mental_health_clinic,,,,,,,,,,,,,,,,,,,,,,,,,
+,Religious,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,buddhist,christian,christian_anglican,christian_catholic,christian_evangelical,christian_lutheran,christian_methodist,christian_orthodox,christian_protestant,hindu,jewish,muslim,muslim_shia,muslim_sunni,sikh,taoist,cathedral,chapel,church,monastery,mosque,religion,presbytery,religious,,
+,Transportation,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,transportation,,,,,,,,,,,,,,,,,,,,,,,,,
+,,airport,airfield,helipad,apron,,,,,,,,,,,,,,,,,,,,,,
+,,bus_station,bus_stop,,,,,,,,,,,,,,,,,,,,,,,,
+,,train_station,railway_station,railway_halt,tram_stop,subway_entrance,,,,,,,,,,,,,,,,,,,,,
+,,car_rental,car_sharing,,,,,,,,,,,,,,,,,,,,,,,,
+,,taxi,taxi_rank,,,,,,,,,,,,,,,,,,,,,,,,
+,,ferry_terminal,,,,,,,,,,,,,,,,,,,,,,,,,
+,,fuel,service,Gas_Station,,,,,,,,,,,,,,,,,,,,,,,
+,,parking,garage,garages,parking_multistorey,parking_underground,vending_parking,parking_site,parking_lot,car_park,parking_structure,parking_space,,,,,,,,,,,,,,,
+,,parking_bicycle,,,,,,,,,,,,,,,,,,,,,,,,,
+,Finance,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,bank,,,,,,,,,,,,,,,,,,,,,,,,,
+,,atm,,,,,,,,,,,,,,,,,,,,,,,,,
+,Other,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,government,Government,courthouse,embassy,municipal,town_hall,,,,,,,,,,,,,,,,,,,,
+,,police,Police Station,,,,,,,,,,,,,,,,,,,,,,,,
+,,post_office,post_box,Post_Office,US_Post_Office,,,,,,,,,,,,,,,,,,,,,,
+,,community_centre,community_center,,,,,,,,,,,,,,,,,,,,,,,,
+,,fire_station,Fire_Department,fire_department,,,,,,,,,,,,,,,,,,,,,,,
+,,prison,Jail_House,jail,,,,,,,,,,,,,,,,,,,,,,,
+,,telephone,,,,,,,,,,,,,,,,,,,,,,,,,
+,,public_building,,,,,,,,,,,,,,,,,,,,,,,,,
+Commercial,,,,,,,,,,,,,,,,,,,,,,,,,,,
+,Leisure,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,cinema,,,,,,,,,,,,,,,,,,,,,,,,,
+,,bar,pub,nightclub,,,,,,,,,,,,,,,,,,,,,,,
+,,theatre,theater,concert_hall,,,,,,,,,,,,,,,,,,,,,,,
+,,theme_park,,,,,,,,,,,,,,,,,,,,,,,,,
+,,zoo,,,,,,,,,,,,,,,,,,,,,,,,,
+,,museum,arts_centre,arts_center,,,,,,,,,,,,,,,,,,,,,,,
+,,casino,,,,,,,,,,,,,,,,,,,,,,,,,
+,Shopping,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,kiosk,newsagent,vending_machine,vending_cigarette,vending_any,,,,,,,,,,,,,,,,,,,,,
+,,shop,clothes,shoe_shop,outdoor_shop,bicycle_shop,bookshop,car_dealership,computer_shop,furniture_shop,gift_shop,jeweller,mobile_phone_shop,sports_shop,stationery,toy_shop,video_shop,store,retail,optician,garden_centre,general,florist,chemist,retail_store,Store,shopping
+,,supermarket,butcher,convenience,greengrocer,grocery_store,Grocery,,,,,,,,,,,,,,,,,,,,
+,,mall,department_store,market_place,shopping_center,,,,,,,,,,,,,,,,,,,,,,
+,Food,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,beverages,biergarten,,,,,,,,,,,,,,,,,,,,,,,,
+,,deli,,,,,,,,,,,,,,,,,,,,,,,,,
+,,restaurant,food_court,,,,,,,,,,,,,,,,,,,,,,,,
+,,cafe,coffee shop,,,,,,,,,,,,,,,,,,,,,,,,
+,,bakery,,,,,,,,,,,,,,,,,,,,,,,,,
+,,fast_food,,,,,,,,,,,,,,,,,,,,,,,,,
+,,food_and_drink,food,,,,,,,,,,,,,,,,,,,,,,,,
+,Lifestyle,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,laundry,,,,,,,,,,,,,,,,,,,,,,,,,
+,,beauty_shop,hairdresser,,,,,,,,,,,,,,,,,,,,,,,,
+,,car_wash,car_repair,,,,,,,,,,,,,,,,,,,,,,,,
+,,hotel,hostel,motel,bed_and_breakfast,guesthouse,chalet,inn,,,,,,,,,,,,,,,,,,,
+,,recycling,recycling_clothes,recycling_glass,recycling_metal,recycling_paper,,,,,,,,,,,,,,,,,,,,,
+,,stadium,,,,,,,,,,,,,,,,,,,,,,,,,
+,,veterinary,,,,,,,,,,,,,,,,,,,,,,,,,
+,,travel_agent,,,,,,,,,,,,,,,,,,,,,,,,,
+,other,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,commercial,commercial;greenhous,commercial;yes,,,,,,,,,,,,,,,,,,,,,,,
+Business,,,,,,,,,,,,,,,,,,,,,,,,,,,
+,Business,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,industrial,,,,,,,,,,,,,,,,,,,,,,,,,
+,,office,,,,,,,,,,,,,,,,,,,,,,,,,
+,,company,,,,,,,,,,,,,,,,,,,,,,,,,
+,,factory,quarry,power_station,,,,,,,,,,,,,,,,,,,,,,,
+,,convention_center,convention_centre,conference_center,,,,,,,,,,,,,,,,,,,,,,,
+Recreational,,,,,,,,,,,,,,,,,,,,,,,,,,,
+,Indoor,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,sports_centre,Sports House,sports_complex,sports_hall,recreational_center,Gymnasium,Gym,,,,,,,,,,,,,,,,,,,
+,,swimming_pool,,,,,,,,,,,,,,,,,,,,,,,,,
+,Outdoor,,,,,,,,,,,,,,,,,,,,,,,,,,
+,,nature,beach,cave_entrance,cliff,glacier,peak,spring,tree,volcano,nature_reserve,forest,meadow,orchard,vineyard,scrub,grass,national_park,basin,,,,,,,,
+,,water,waterfall,reservoir,river,dock,glacier,wetland,,,,,,,,,,,,,,,,,,,
+,,park,allotments,recreation_ground,village_green,,,,,,,,,,,,,,,,,,,,,,
+,,farm,farmland,farmyard,,,,,,,,,,,,,,,,,,,,,,,
+,,bicycle_rental,,,,,,,,,,,,,,,,,,,,,,,,,
+,,golf_course,,,,,,,,,,,,,,,,,,,,,,,,,
+,,dog_park,,,,,,,,,,,,,,,,,,,,,,,,,
+,,ice_rink,Ice_Skating_Rink,,,,,,,,,,,,,,,,,,,,,,,,
+,,picnic_site,,,,,,,,,,,,,,,,,,,,,,,,,
+,,pitch,,,,,,,,,,,,,,,,,,,,,,,,,
+,,playground,Playground,,,,,,,,,,,,,,,,,,,,,,,,
+,,track,,,,,,,,,,,,,,,,,,,,,,,,,
+,,viewpoint,observation_tower,,,,,,,,,,,,,,,,,,,,,,,,
+,,attraction,monument,memorial,castle,ruins,archaeological,battlefield,fort,aerialway_station,,,,,,,,,,,,,,,,,
+,,hunting_stand,,,,,,,,,,,,,,,,,,,,,,,,,
+,,graveyard,cemetery,,,,,,,,,,,,,,,,,,,,,,,,
+,,tennis_court,,,,,,,,,,,,,,,,,,,,,,,,,
+,,shelter,alpine_hut,,,,,,,,,,,,,,,,,,,,,,,,
+,,camp_site,caravan_site,,,,,,,,,,,,,,,,,,,,,,,,
 ,,tourism,tourist_info,tourist_map,tourist_board,tourist_guidepost,,,,,,,,,,,,,,,,,,,,,
```

### Comparing `osm_annotation-0.1.8/osm_annotation/label_map/osm_label_hierarchy_clean.csv` & `osm_annotation-0.1.9/osm_annotation/label_map/osm_label_hierarchy_clean.csv`

 * *Files identical despite different names*

### Comparing `osm_annotation-0.1.8/osm_annotation/semantic_annotation.py` & `osm_annotation-0.1.9/osm_annotation/semantic_annotation.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,27 +67,32 @@
                 lvl2_path = lvl1_path + os.sep + lvl2_label
                 for lvl3_label in os.listdir(lvl2_path):
                     # print("    Level 3 : "+lvl3_label)
                     lvl3_path = lvl2_path + os.sep + lvl3_label
 
                     finding_list_point = list(glob(os.path.join(lvl3_path, "*_point.shp")))
                     if len(finding_list_point) > 0:
-                        point_shp_path = finding_list_point[0]
-                        gdf_landmark = gpd.read_file(point_shp_path)
+                        gdf_landmark = pd.DataFrame()
+                        for point_shp_path in finding_list_point:
+                            gdf_landmark = gdf_landmark.append(gpd.read_file(point_shp_path))
+                            gdf_landmark.reset_index(inplace=True, drop=True)
 
                         nearest_POI = dist.dist_to_point(cluster_centroid_point, gdf_landmark, proj=2163)
                         distance = list(nearest_POI['dist2point'])[0]
                         distance_list.append(distance)
                         osm_label_list.append("{};{};{} (point)".format(lvl1_label, lvl2_label, lvl3_label))
 
                     finding_list_poly = list(glob(os.path.join(lvl3_path, "*_polygon.shp")))
                     if len(finding_list_poly) > 0:
-                        poly_shp_path = finding_list_poly[0]
+                        gdf_landmark = pd.DataFrame()
+                        for poly_shp_path in finding_list_poly:
+                            gdf_landmark = gdf_landmark.append(gpd.read_file(poly_shp_path))
+                            gdf_landmark.reset_index(inplace=True, drop=True)
 
-                        gdf_landmark = gpd.read_file(poly_shp_path)
+                        # gdf_landmark = gpd.read_file(poly_shp_path)
                         gdf_landmark = gdf_landmark.to_crs('epsg:2163')
                         gdf_landmark.geometry = gdf_landmark.geometry.centroid
 
                         nearest_POI = dist.dist_to_point(cluster_centroid_point, gdf_landmark, proj=2163)
                         distance = list(nearest_POI['dist2point'])[0]
                         distance_list.append(distance)
                         osm_label_list.append("{};{};{} (polygon)".format(lvl1_label, lvl2_label, lvl3_label))
@@ -139,35 +144,41 @@
                 lvl2_path = lvl1_path + os.sep + lvl2_label
                 for lvl3_label in os.listdir(lvl2_path):
                     # print("    Level 3 : "+lvl3_label)
                     lvl3_path = lvl2_path + os.sep + lvl3_label
 
                     finding_list_point = list(glob(os.path.join(lvl3_path, "*_point.shp")))
                     if len(finding_list_point) > 0:
-                        point_shp_path = finding_list_point[0]
-                        gdf_landmark_point = fiona.open(point_shp_path)
+                        for point_shp_path in finding_list_point:
+                            gdf_landmark_point = fiona.open(point_shp_path)
 
-                        for next_shp in gdf_landmark_point:
-                            geo = shape(next_shp['geometry'])
-                            if cluster_poly.contains(geo):  # polygon contains a point landmark
-                                point_label_list.append("{};{};{} (point)".format(lvl1_label, lvl2_label, lvl3_label))
-                                geo_list.append(geo)
-                                break
+                            for next_shp in gdf_landmark_point:
+                                geo = shape(next_shp['geometry'])
+                                if cluster_poly.contains(geo):  # polygon contains a point landmark
+                                    point_label_list.append("{};{};{} (point)".format(lvl1_label, lvl2_label, lvl3_label))
+                                    geo_list.append(geo)
+                                    break
+                            else:
+                                continue  # only executed if the inner loop did NOT break
+                            break  # only executed if the inner loop DID break
 
                     finding_list_poly = list(glob(os.path.join(lvl3_path, "*_polygon.shp")))
                     if len(finding_list_poly) > 0:
-                        poly_shp_path = finding_list_poly[0]
-                        gdf_landmark_poly = fiona.open(poly_shp_path)
+                        for poly_shp_path in finding_list_poly:
+                            gdf_landmark_poly = fiona.open(poly_shp_path)
 
-                        for next_shp in gdf_landmark_poly:
-                            geo = shape(next_shp['geometry'])
-                            if cluster_poly.intersects(geo):  # polygon intersects a polygon landmark
-                                poly_label_list.append("{};{};{} (polygon)".format(lvl1_label, lvl2_label, lvl3_label))
-                                geo_list.append(geo)
-                                break
+                            for next_shp in gdf_landmark_poly:
+                                geo = shape(next_shp['geometry'])
+                                if cluster_poly.intersects(geo):  # polygon intersects a polygon landmark
+                                    poly_label_list.append("{};{};{} (polygon)".format(lvl1_label, lvl2_label, lvl3_label))
+                                    geo_list.append(geo)
+                                    break
+                            else:
+                                continue  # only executed if the inner loop did NOT break
+                            break  # only executed if the inner loop DID break
 
         result_json = {"matched_labels": point_label_list + list(set(poly_label_list) - set(point_label_list)),
                        "point_labels": point_label_list,
                        "poly_labels": poly_label_list,
                        "matched_geometries": geo_list}
 
         return result_json
@@ -205,26 +216,31 @@
                 lvl2_path = lvl1_path + os.sep + lvl2_label
                 for lvl3_label in os.listdir(lvl2_path):
                     # print("    Level 3 : " + lvl3_label)
                     lvl3_path = lvl2_path + os.sep + lvl3_label
 
                     finding_list_point = list(glob(os.path.join(lvl3_path, "*_point.shp")))
                     if len(finding_list_point) > 0:
-                        point_shp_path = finding_list_point[0]
+                        gdf_landmark = pd.DataFrame()
+                        for point_shp_path in finding_list_point:
+                            gdf_landmark = gdf_landmark.append(gpd.read_file(point_shp_path))
+                            gdf_landmark.reset_index(inplace=True, drop=True)
 
-                        gdf_landmark = gpd.read_file(point_shp_path)
                         nearest_POI = dist.dist_to_point(cluster_centroid_point_p, gdf_landmark, proj=2163)
                         dist2point_df["{};{};{} (point)".format(lvl1_label, lvl2_label, lvl3_label)] = \
                             nearest_POI["dist2point"]
 
                     finding_list_poly = list(glob(os.path.join(lvl3_path, "*_polygon.shp")))
                     if len(finding_list_poly) > 0:
-                        poly_shp_path = finding_list_poly[0]
+                        gdf_landmark = pd.DataFrame()
+                        for poly_shp_path in finding_list_poly:
+                            gdf_landmark = gdf_landmark.append(gpd.read_file(poly_shp_path))
+                            gdf_landmark.reset_index(inplace=True, drop=True)
+
 
-                        gdf_landmark = gpd.read_file(poly_shp_path)
                         gdf_landmark = gdf_landmark.to_crs('epsg:2163')
                         gdf_landmark.geometry = gdf_landmark.geometry.centroid
 
                         nearest_POI = dist.dist_to_point(cluster_centroid_point_p, gdf_landmark, proj=2163)
                         dist2point_df["{};{};{} (polygon)".format(lvl1_label, lvl2_label, lvl3_label)] = \
                             nearest_POI["dist2point"]
```

### Comparing `osm_annotation-0.1.8/osm_annotation.egg-info/PKG-INFO` & `osm_annotation-0.1.9/osm_annotation.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-annotation
-Version: 0.1.8
+Version: 0.1.9
 Summary: An easy-to-use Python package that annotate location data with semantic labels from OpenStreetMap
 Home-page: https://bitbucket.org/mhealthresearchgroup/osm_annotation/src/main/
 Author: Jixin Li
 Author-email: li.jix@northeastern.edu
 Project-URL: Bug Tracker, https://bitbucket.org/mhealthresearchgroup/osm_annotation/issues?status=new&status=open
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,27 +12,27 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # location_annotation_with_openstreetmap
 This is an easy-to-use Python package for annotating location data with OpenStreetMap Point-of-interest tags. It provides a solution for researchers to adding additional layer of context information to location data at large scale in an automatic way. For example, the input can be pairs of coordinates (lat, lon), and the output are types of places of the input locations, such as "gym", "restaurant", "university", "office", etc. Annotation using this package incurs no cost when this package downloads and uses free POI data from [Geofabrik](https://www.geofabrik.de/) that reflect daily changes from [OpenStreetMap](https://en.wikipedia.org/wiki/OpenStreetMap). For questions about this package, please leave an [issue](https://bitbucket.org/mhealthresearchgroup/osm_annotation/issues?status=new&status=open) or contact the [author](mailto:li.jix@northeastern.edu).
 
-### Author and Credits
-Jixin Li, mHealth research group@Northeastern University  
-
-This package integrates the geodf and dist functions from the GPS2space package (https://gps2space.readthedocs.io/en/latest/).  
-
-A paper is in submission. If you use this package, please cite it as below.  
-> Li, Jixin. (2023). osm_annotation (version 0.1.8) [Python package]. https://bitbucket.org/mhealthresearchgroup/osm_annotation/src/main/
-
-
 ### Two general steps
 **1. Download and create a geofabrik POI database in local system**  
 **2. Annotate location data using the POI database**  
 
+## Contact
+- Author: Jixin Li @ [mHealth research group](https://www.mhealthgroup.org/)
+- For questions about this package, please leave an [issue](https://bitbucket.org/mhealthresearchgroup/osm_annotation/issues?status=new&status=open&is_spam=!spam).
+  
+## Citation
+- This repository is a part of journal paper submission that is currently under review. Full citation information will come soon. In the meanwhile, please cite as below:
+> Jixin Li. 2023. location_annotation_with_openstreetmap (osm_annotation). https://bitbucket.org/mhealthresearchgroup/osm_annotation/src/main/ 
+- This package also integrates the geodf and dist functions from the GPS2space package (https://gps2space.readthedocs.io/en/latest/).
+
 ## Dependencies
 - geopandas
 - fiona
 - gps2space
 - tqdm
 - Python >= 3.7
 
@@ -76,59 +76,72 @@
 ```python
 # coordinates of Fenway Park in Boston
 centroid_latitude = 42.34653831212525
 centroid_longitude = -71.09724395926423
 semantic_annotator.annotate_single_point(centroid_latitude, centroid_longitude)
 ```
 
-Returned result is a json file with
-- matched_labels: semantic label matched with the query point
-- min_distance: the distance from the query point to the matched POI, in meters
-- distances_to_pois: distance to other types of POIs
-> {'matched_labels': 'recreational;outdoor;pitch (polygon)',
- 'min_distance': 6.169761255410299,
- 'distances_to_pois': {'busines;busines;company (polygon)': 326501.593160387,
-  'busines;busines;convention_center (polygon)': 2682942.101031607,
-  'busines;busines;factory (polygon)': 3612.955363467255,
-  'busines;busines;industrial (polygon)': 486.88772114370636,
-  'busines;busines;office (polygon)': 932.2980449124797,
-  'commercial;food;bakery (point)': 738.1374807550822,
-> ...
-> }
+Returned result is a json file with  
+    - matched_labels: semantic label matched with the query point  
+    - min_distance: the distance from the query point to the matched POI, in meters  
+    - distances_to_pois: distance to other types of POIs  
+    
+```json
+   {  
+    'matched_labels': 'recreational;outdoor;pitch (polygon)',  
+    'min_distance': 6.169761255410299,  
+    'distances_to_pois': {  
+        'busines;busines;company (polygon)': 326501.593160387,  
+        'busines;busines;convention_center (polygon)': 2682942.101031607,  
+        'busines;busines;factory (polygon)': 3612.955363467255,  
+        'busines;busines;industrial (polygon)': 486.88772114370636,  
+        'busines;busines;office (polygon)': 932.2980449124797,  
+        'commercial;food;bakery (point)': 738.1374807550822,  
+        ...
+   }
+```
 
 
 ### Example of Method 2
 ```python
 # bounding box (NW corner,NE corner, SE corner, SW corner) of Museum of Fine Arts in Boston
 lat_list = [42.33969558839377, 42.34039653732734, 42.339235761638996, 42.33847311473655]
 lon_list = [-71.09563225696323, -71.09348529667446, -71.09270768730832, -71.0948470612041]
 semantic_annotator.annotate_single_shape(lat_list, lon_list)
 ```
 
-Returned result is a json file with
-- matched_labels: semantic labels matched with the query shape
-- point_labels: semantic labels of point POI matched with the query shape
-- poly_labels: semantic labels of polygon POI matched with the query shape
+Returned result is a json file with  
+- matched_labels: semantic labels matched with the query shape  
+- point_labels: semantic labels of point POI matched with the query shape  
+- poly_labels: semantic labels of polygon POI matched with the query shape  
 - matched_geometries: geometries of POIs matched with the query shape
-> {'matched_labels': ['commercial;food;cafe (point)',
-  'commercial;shopping;shop (point)',
-  'commercial;leisure;museum (polygon)',
-  'service;transportation;parking (polygon)',
-  'recreational;outdoor;nature (polygon)'],
- 'point_labels': ['commercial;food;cafe (point)',
-  'commercial;shopping;shop (point)'],
- 'poly_labels': ['commercial;leisure;museum (polygon)',
-  'recreational;outdoor;nature (polygon)',
-  'service;transportation;parking (polygon)'],
- 'matched_geometries': [<shapely.geometry.point.Point at 0x2b8b25338410>,
-  <shapely.geometry.polygon.Polygon at 0x2b8b25353b10>,
-  <shapely.geometry.point.Point at 0x2b8b253415d0>,
-  <shapely.geometry.polygon.Polygon at 0x2b8b250b0910>,
-  <shapely.geometry.polygon.Polygon at 0x2b8b25331690>]}
 
+```json
+   {
+    'matched_labels': 
+       ['commercial;food;cafe (point)',
+       'commercial;shopping;shop (point)',
+       'commercial;leisure;museum (polygon)',
+       'service;transportation;parking (polygon)',
+       'recreational;outdoor;nature (polygon)'],
+    'point_labels': 
+       ['commercial;food;cafe (point)',
+       'commercial;shopping;shop (point)'],
+    'poly_labels': 
+       ['commercial;leisure;museum (polygon)',
+       'recreational;outdoor;nature (polygon)',
+       'service;transportation;parking (polygon)'],
+    'matched_geometries': 
+        [<shapely.geometry.point.Point at 0x2b8b25338410>,
+        <shapely.geometry.polygon.Polygon at 0x2b8b25353b10>,
+        <shapely.geometry.point.Point at 0x2b8b253415d0>,
+        <shapely.geometry.polygon.Polygon at 0x2b8b250b0910>,
+        <shapely.geometry.polygon.Polygon at 0x2b8b25331690>]
+   }
+```
 
 
 ### Example of Method 3
 ```python
 # library, cafe, gym, and train station around the Northeastern University campus
 locations = [[42.33833,-71.08795], # library
              [42.33909,-71.08758], # cafe
@@ -138,8 +151,8 @@
 semantic_annotator.annotate_batch_points(dataframe = location_dataframe, latitude_colname = 'latitude', longitude_colname = 'longitude')
 ```
 
 Returned result is a dataframe with
 - matched_labels: semantic labels matched with the query points
 - min_distance: the distance from the query point to the matched POI, in meters
 
-![alt text](https://github.com/rexli999/location_annotation_with_openstreetmap/blob/main/batch_results.png "batch result")
+![Batch_result](batch_results.png)
```

### Comparing `osm_annotation-0.1.8/setup.cfg` & `osm_annotation-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 736d 5f61 6e6e 6f74 6174 696f   = osm_annotatio
 00000020: 6e0d 0a76 6572 7369 6f6e 203d 2030 2e31  n..version = 0.1
-00000030: 2e38 0d0a 6175 7468 6f72 203d 204a 6978  .8..author = Jix
+00000030: 2e39 0d0a 6175 7468 6f72 203d 204a 6978  .9..author = Jix
 00000040: 696e 204c 690d 0a61 7574 686f 725f 656d  in Li..author_em
 00000050: 6169 6c20 3d20 6c69 2e6a 6978 406e 6f72  ail = li.jix@nor
 00000060: 7468 6561 7374 6572 6e2e 6564 750d 0a64  theastern.edu..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2041 6e20  escription = An 
 00000080: 6561 7379 2d74 6f2d 7573 6520 5079 7468  easy-to-use Pyth
 00000090: 6f6e 2070 6163 6b61 6765 2074 6861 7420  on package that 
 000000a0: 616e 6e6f 7461 7465 206c 6f63 6174 696f  annotate locatio
```

### Comparing `osm_annotation-0.1.8/setup.py` & `osm_annotation-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='osm_annotation',
-    version="0.1.8",
+    version="0.1.9",
     description='An easy-to-use Python package that annotate location data with semantic labels from OpenStreetMap',
     url='https://bitbucket.org/mhealthresearchgroup/osm_annotation/src/main/',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Jixin Li',
     author_email='li.jix@northeastern.edu',
     classifiers=[
```

