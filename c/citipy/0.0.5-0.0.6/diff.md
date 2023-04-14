# Comparing `tmp/citipy-0.0.5.tar.gz` & `tmp/citipy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/citipy-0.0.5.tar", last modified: Wed Jan  4 07:43:24 2017, max compression
+gzip compressed data, was "citipy-0.0.6.tar", last modified: Fri Apr 14 17:37:53 2023, max compression
```

## Comparing `citipy-0.0.5.tar` & `citipy-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2017-01-04 07:43:24.000000 citipy-0.0.5/
-drwxr-xr-x   0 user       (501) staff       (20)        0 2017-01-04 07:43:24.000000 citipy-0.0.5/citipy/
--rw-r--r--   0 user       (501) staff       (20)        0 2016-03-28 04:19:51.000000 citipy-0.0.5/citipy/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1111 2017-01-04 07:40:40.000000 citipy-0.0.5/citipy/citipy.py
--rw-r--r--   0 user       (501) staff       (20)  1524355 2015-10-24 16:59:56.000000 citipy-0.0.5/citipy/worldcities.csv
-drwxr-xr-x   0 user       (501) staff       (20)        0 2017-01-04 07:43:24.000000 citipy-0.0.5/citipy.egg-info/
--rw-r--r--   0 user       (501) staff       (20)        1 2017-01-04 07:43:24.000000 citipy-0.0.5/citipy.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)      294 2017-01-04 07:43:24.000000 citipy-0.0.5/citipy.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)       13 2017-01-04 07:43:24.000000 citipy-0.0.5/citipy.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)      226 2017-01-04 07:43:24.000000 citipy-0.0.5/citipy.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        7 2017-01-04 07:43:24.000000 citipy-0.0.5/citipy.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)      294 2017-01-04 07:43:24.000000 citipy-0.0.5/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      100 2017-01-04 07:43:24.000000 citipy-0.0.5/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      461 2017-01-04 07:41:31.000000 citipy-0.0.5/setup.py
+drwxr-xr-x   0 wingchen  (1000) wingchen  (1000)        0 2023-04-14 17:37:53.026397 citipy-0.0.6/
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)     1076 2023-04-14 17:28:13.000000 citipy-0.0.6/LICENSE
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)     1087 2023-04-14 17:28:13.000000 citipy-0.0.6/LICENSE.txt
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)      300 2023-04-14 17:37:53.026397 citipy-0.0.6/PKG-INFO
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)     1457 2023-04-14 17:28:13.000000 citipy-0.0.6/README.md
+drwxr-xr-x   0 wingchen  (1000) wingchen  (1000)        0 2023-04-14 17:37:53.024397 citipy-0.0.6/citipy/
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)        0 2023-04-14 17:28:13.000000 citipy-0.0.6/citipy/__init__.py
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)     1185 2023-04-14 17:28:13.000000 citipy-0.0.6/citipy/citipy.py
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)  1616692 2023-04-14 17:28:13.000000 citipy-0.0.6/citipy/worldcities.csv
+drwxr-xr-x   0 wingchen  (1000) wingchen  (1000)        0 2023-04-14 17:37:53.026397 citipy-0.0.6/citipy.egg-info/
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)      300 2023-04-14 17:37:52.000000 citipy-0.0.6/citipy.egg-info/PKG-INFO
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)      256 2023-04-14 17:37:52.000000 citipy-0.0.6/citipy.egg-info/SOURCES.txt
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)        1 2023-04-14 17:37:52.000000 citipy-0.0.6/citipy.egg-info/dependency_links.txt
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)       13 2023-04-14 17:37:52.000000 citipy-0.0.6/citipy.egg-info/requires.txt
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)        7 2023-04-14 17:37:52.000000 citipy-0.0.6/citipy.egg-info/top_level.txt
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)       79 2023-04-14 17:37:53.027397 citipy-0.0.6/setup.cfg
+-rw-r--r--   0 wingchen  (1000) wingchen  (1000)      458 2023-04-14 17:34:46.000000 citipy-0.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `citipy-0.0.5/citipy/citipy.py` & `citipy-0.0.6/citipy/citipy.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 
 class City:
     '''
     City wraps up the info about a city, including its name, coordinates,
     and belonging country.
     '''
-    def __init__(self, city_name, country_code):
+    def __init__(self, city_name, country_code, lat, lng):
         self.city_name = city_name
         self.country_code = country_code
+        self.lat = lat
+        self.lng = lng
 
 
 # load the city data up
 _current_dir, _current_filename = os.path.split(__file__)
 _world_cities_csv_path = os.path.join(_current_dir, 'worldcities.csv')
 _world_cities_kdtree = kdtree.create(dimensions=2)
 WORLD_CITIES_DICT = {}
@@ -25,14 +27,14 @@
     # discard the headers
     cities.__next__()
 
     # populate geo points into kdtree
     for city in cities:
         city_coordinate_key = (float(city[2]), float(city[3]))
         _world_cities_kdtree.add(city_coordinate_key)
-        c = City(city[1], city[0])
+        c = City(city[1], city[0], city[2], city[3])
         WORLD_CITIES_DICT[city_coordinate_key] = c
 
 
 def nearest_city(latitude, longitude):
     nearest_city_coordinate = _world_cities_kdtree.search_nn((latitude, longitude, ))
     return WORLD_CITIES_DICT[nearest_city_coordinate[0].data]
```

