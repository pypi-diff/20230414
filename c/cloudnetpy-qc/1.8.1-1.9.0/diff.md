# Comparing `tmp/cloudnetpy_qc-1.8.1.tar.gz` & `tmp/cloudnetpy_qc-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudnetpy_qc-1.8.1.tar", last modified: Thu Apr  6 13:10:19 2023, max compression
+gzip compressed data, was "cloudnetpy_qc-1.9.0.tar", last modified: Fri Apr 14 09:53:09 2023, max compression
```

## Comparing `cloudnetpy_qc-1.8.1.tar` & `cloudnetpy_qc-1.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:10:19.044060 cloudnetpy_qc-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-06 13:10:19.044060 cloudnetpy_qc-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:10:19.040059 cloudnetpy_qc-1.8.1/cloudnetpy_qc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:10:19.044060 cloudnetpy_qc-1.8.1/cloudnetpy_qc/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/data/area-type-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/data/cf-standard-name-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/data/data_quality_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/data/metadata_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/data/standardized-region-list.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15828 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:10:19.040059 cloudnetpy_qc-1.8.1/cloudnetpy_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-06 13:10:18.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-06 13:10:19.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:10:18.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-06 13:10:18.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 13:10:18.000000 cloudnetpy_qc-1.8.1/cloudnetpy_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 13:10:19.044060 cloudnetpy_qc-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-06 13:10:07.000000 cloudnetpy_qc-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:09.989345 cloudnetpy_qc-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-14 09:53:09.989345 cloudnetpy_qc-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:09.985345 cloudnetpy_qc-1.9.0/cloudnetpy_qc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:09.989345 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/area-type-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/cf-standard-name-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/data_quality_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/metadata_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/standardized-region-list.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15828 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30001 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:53:09.985345 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-14 09:53:09.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-14 09:53:09.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:53:09.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 09:53:09.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 09:53:09.000000 cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:53:09.989345 cloudnetpy_qc-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-14 09:53:01.000000 cloudnetpy_qc-1.9.0/setup.py
```

### Comparing `cloudnetpy_qc-1.8.1/LICENSE` & `cloudnetpy_qc-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.8.1/PKG-INFO` & `cloudnetpy_qc-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudnetpy_qc
-Version: 1.8.1
+Version: 1.9.0
 Summary: Quality control routines for CloudnetPy products
 Home-page: https://github.com/actris-cloudnet/cloudnetpy-qc
 Author: Finnish Meteorological Institute
 Author-email: actris-cloudnet@fmi.fi
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudnetpy_qc-1.8.1/README.md` & `cloudnetpy_qc-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.8.1/cloudnetpy_qc/data/area-type-table.xml` & `cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/area-type-table.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.8.1/cloudnetpy_qc/data/cf-standard-name-table.xml` & `cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/cf-standard-name-table.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.8.1/cloudnetpy_qc/data/data_quality_config.ini` & `cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/data_quality_config.ini`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.8.1/cloudnetpy_qc/data/standardized-region-list.xml` & `cloudnetpy_qc-1.9.0/cloudnetpy_qc/data/standardized-region-list.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.8.1/cloudnetpy_qc/quality.py` & `cloudnetpy_qc-1.9.0/cloudnetpy_qc/quality.py`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.8.1/cloudnetpy_qc/utils.py` & `cloudnetpy_qc-1.9.0/cloudnetpy_qc/utils.py`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.8.1/cloudnetpy_qc/variables.py` & `cloudnetpy_qc-1.9.0/cloudnetpy_qc/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     # Level 1b
     RADAR = "radar"
     LIDAR = "lidar"
     MWR = "mwr"
     DISDROMETER = "disdrometer"
     MODEL = "model"
     WEATHER_STATION = "weather-station"
+    DOPPLER_LIDAR = "doppler-lidar"
     # Level 1c
     CATEGORIZE = "categorize"
     # Level 2
     CLASSIFICATION = "classification"
     IWC = "iwc"
     LWC = "lwc"
     DRIZZLE = "drizzle"
@@ -131,15 +132,16 @@
     ),
     "quality_bits": Variable(
         long_name="Data quality bits", dtype=Dtype.INT, required=[Product.CATEGORIZE]
     ),
     "beta": Variable(
         long_name="Attenuated backscatter coefficient",
         units="sr-1 m-1",
-        required=[Product.CATEGORIZE],
+        # Lidar has its own beta test
+        required=[Product.CATEGORIZE, Product.DOPPLER_LIDAR],
     ),
     "beta_error": Variable(
         long_name="Error in attenuated backscatter coefficient",
         units="dB",
         required=[Product.CATEGORIZE],
     ),
     "beta_bias": Variable(
@@ -370,15 +372,15 @@
     ),
     "range": Variable(
         long_name="Range from instrument", units="m", required=[Product.RADAR, Product.LIDAR]
     ),
     "v": Variable(
         long_name="Doppler velocity",
         units="m s-1",
-        required=[Product.RADAR, Product.CATEGORIZE],
+        required=[Product.RADAR, Product.CATEGORIZE, Product.DOPPLER_LIDAR],
     ),
     "temperature": Variable(
         long_name="Temperature", units="K", required=[Product.MODEL, Product.CATEGORIZE]
     ),
     "pressure": Variable(
         long_name="Pressure", units="Pa", required=[Product.MODEL, Product.CATEGORIZE]
     ),
```

### Comparing `cloudnetpy_qc-1.8.1/cloudnetpy_qc.egg-info/PKG-INFO` & `cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudnetpy-qc
-Version: 1.8.1
+Version: 1.9.0
 Summary: Quality control routines for CloudnetPy products
 Home-page: https://github.com/actris-cloudnet/cloudnetpy-qc
 Author: Finnish Meteorological Institute
 Author-email: actris-cloudnet@fmi.fi
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudnetpy_qc-1.8.1/cloudnetpy_qc.egg-info/SOURCES.txt` & `cloudnetpy_qc-1.9.0/cloudnetpy_qc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.8.1/setup.py` & `cloudnetpy_qc-1.9.0/setup.py`

 * *Files identical despite different names*

