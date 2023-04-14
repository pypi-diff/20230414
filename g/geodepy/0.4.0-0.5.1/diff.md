# Comparing `tmp/geodepy-0.4.0.tar.gz` & `tmp/geodepy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/GeodePy/GeodePy/dist/tmpbqhkfjse/geodepy-0.4.0.tar", last modified: Sun Aug  7 23:10:23 2022, max compression
+gzip compressed data, was "/home/runner/work/GeodePy/GeodePy/dist/.tmp-atrpvhoo/geodepy-0.5.1.tar", last modified: Fri Apr 14 00:58:52 2023, max compression
```

## Comparing `geodepy-0.4.0.tar` & `geodepy-0.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-07 23:10:23.000000 geodepy-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-08-07 23:10:12.000000 geodepy-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-08-07 23:10:23.000000 geodepy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-08-07 23:10:12.000000 geodepy-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-07 23:10:23.000000 geodepy-0.4.0/geodepy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34164 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/angles.py
--rw-r--r--   0 runner    (1001) docker     (121)    36702 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    20287 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)    17794 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/coord.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/fileio.py
--rw-r--r--   0 runner    (1001) docker     (121)    16962 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/geodesy.py
--rw-r--r--   0 runner    (1001) docker     (121)    22943 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/gnss.py
--rw-r--r--   0 runner    (1001) docker     (121)     8313 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/height.py
--rw-r--r--   0 runner    (1001) docker     (121)     8851 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/inputoutput.py
--rw-r--r--   0 runner    (1001) docker     (121)    20362 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/ntv2reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     8503 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     8100 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/survey.py
--rw-r--r--   0 runner    (1001) docker     (121)    10946 2022-08-07 23:10:12.000000 geodepy-0.4.0/geodepy/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-07 23:10:23.000000 geodepy-0.4.0/geodepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-08-07 23:10:23.000000 geodepy-0.4.0/geodepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-08-07 23:10:23.000000 geodepy-0.4.0/geodepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-07 23:10:23.000000 geodepy-0.4.0/geodepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-07 23:10:23.000000 geodepy-0.4.0/geodepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-07 23:10:23.000000 geodepy-0.4.0/geodepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-07 23:10:23.000000 geodepy-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-08-07 23:10:12.000000 geodepy-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:58:52.000000 geodepy-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-14 00:58:41.000000 geodepy-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 00:58:52.000000 geodepy-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-14 00:58:41.000000 geodepy-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:58:52.000000 geodepy-0.5.1/geodepy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34164 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36702 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/geodesy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33731 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/gnss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/height.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/inputoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20362 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/ntv2reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22103 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-04-14 00:58:41.000000 geodepy-0.5.1/geodepy/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:58:52.000000 geodepy-0.5.1/geodepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 00:58:52.000000 geodepy-0.5.1/geodepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-14 00:58:52.000000 geodepy-0.5.1/geodepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:58:52.000000 geodepy-0.5.1/geodepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 00:58:52.000000 geodepy-0.5.1/geodepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 00:58:52.000000 geodepy-0.5.1/geodepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:58:52.000000 geodepy-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-14 00:58:41.000000 geodepy-0.5.1/setup.py
```

### Comparing `geodepy-0.4.0/LICENSE` & `geodepy-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/README.md` & `geodepy-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/geodepy/angles.py` & `geodepy-0.5.1/geodepy/angles.py`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/geodepy/constants.py` & `geodepy-0.5.1/geodepy/constants.py`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/geodepy/convert.py` & `geodepy-0.5.1/geodepy/convert.py`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/geodepy/coord.py` & `geodepy-0.5.1/geodepy/coord.py`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/geodepy/fileio.py` & `geodepy-0.5.1/geodepy/fileio.py`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/geodepy/geodesy.py` & `geodepy-0.5.1/geodepy/geodesy.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,15 +176,16 @@
     # Convert Angles to Decimal Degrees (if required)
     lat1 = angular_typecheck(lat1)
     lon1 = angular_typecheck(lon1)
     lat2 = angular_typecheck(lat2)
     lon2 = angular_typecheck(lon2)
 
     # Exit if the two input points are the same
-    if lat1 == lat2 and lon1 == lon2:
+    tolerance = 0.0000000001
+    if abs(lat1 - lat2) < tolerance and abs(lon1 - lon2) < tolerance:
         return 0, 0, 0
 
     # Equation numbering is from the GDA2020 Tech Manual v1.0
 
     # Eq. 71
     u1 = atan((1 - ellipsoid.f) * tan(radians(lat1)))
```

### Comparing `geodepy-0.4.0/geodepy/height.py` & `geodepy-0.5.1/geodepy/height.py`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/geodepy/inputoutput.py` & `geodepy-0.5.1/geodepy/inputoutput.py`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/geodepy/ntv2reader.py` & `geodepy-0.5.1/geodepy/ntv2reader.py`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/geodepy/statistics.py` & `geodepy-0.5.1/geodepy/statistics.py`

 * *Files identical despite different names*

### Comparing `geodepy-0.4.0/geodepy/transform.py` & `geodepy-0.5.1/geodepy/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,8 +265,7 @@
         tf_lat = lat + shifts[0] / 3600
         tf_lon = lon - shifts[1] / 3600
     else:
         tf_lat = lat - shifts[0] / 3600
         tf_lon = lon + shifts[1] / 3600
 
     return tf_lat, tf_lon
-
```

