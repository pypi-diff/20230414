# Comparing `tmp/nowcasting_forecast-1.3.3.tar.gz` & `tmp/nowcasting_forecast-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_forecast-1.3.3.tar", last modified: Tue Apr 11 15:00:35 2023, max compression
+gzip compressed data, was "nowcasting_forecast-1.3.4.tar", last modified: Fri Apr 14 15:23:22 2023, max compression
```

## Comparing `nowcasting_forecast-1.3.3.tar` & `nowcasting_forecast-1.3.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:00:35.716607 nowcasting_forecast-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-11 15:00:35.716607 nowcasting_forecast-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:00:35.712607 nowcasting_forecast-1.3.3/nowcasting_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/nowcasting_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/nowcasting_forecast/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/nowcasting_forecast/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/nowcasting_forecast/dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:00:35.716607 nowcasting_forecast-1.3.3/nowcasting_forecast/models/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/nowcasting_forecast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/nowcasting_forecast/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/nowcasting_forecast/models/nwp_solar_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/nowcasting_forecast/models/sun.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/nowcasting_forecast/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/nowcasting_forecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:00:35.712607 nowcasting_forecast-1.3.3/nowcasting_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-11 15:00:35.000000 nowcasting_forecast-1.3.3/nowcasting_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-11 15:00:35.000000 nowcasting_forecast-1.3.3/nowcasting_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:00:35.000000 nowcasting_forecast-1.3.3/nowcasting_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-11 15:00:35.000000 nowcasting_forecast-1.3.3/nowcasting_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 15:00:35.000000 nowcasting_forecast-1.3.3/nowcasting_forecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:00:35.716607 nowcasting_forecast-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:00:35.716607 nowcasting_forecast-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-11 15:00:23.000000 nowcasting_forecast-1.3.3/tests/test_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:23:22.572342 nowcasting_forecast-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-14 15:23:22.572342 nowcasting_forecast-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:23:22.572342 nowcasting_forecast-1.3.4/nowcasting_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/nowcasting_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/nowcasting_forecast/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/nowcasting_forecast/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/nowcasting_forecast/dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:23:22.572342 nowcasting_forecast-1.3.4/nowcasting_forecast/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/nowcasting_forecast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/nowcasting_forecast/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/nowcasting_forecast/models/nwp_solar_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/nowcasting_forecast/models/sun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/nowcasting_forecast/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/nowcasting_forecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:23:22.572342 nowcasting_forecast-1.3.4/nowcasting_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-14 15:23:22.000000 nowcasting_forecast-1.3.4/nowcasting_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 15:23:22.000000 nowcasting_forecast-1.3.4/nowcasting_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:23:22.000000 nowcasting_forecast-1.3.4/nowcasting_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 15:23:22.000000 nowcasting_forecast-1.3.4/nowcasting_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 15:23:22.000000 nowcasting_forecast-1.3.4/nowcasting_forecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:23:22.572342 nowcasting_forecast-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:23:22.572342 nowcasting_forecast-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-14 15:23:13.000000 nowcasting_forecast-1.3.4/tests/test_batch.py
```

### Comparing `nowcasting_forecast-1.3.3/LICENSE` & `nowcasting_forecast-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/PKG-INFO` & `nowcasting_forecast-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_forecast
-Version: 1.3.3
+Version: 1.3.4
 Summary: Live forecast for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_forecast
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: artificial intelligence,forecast
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_forecast-1.3.3/README.md` & `nowcasting_forecast-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/nowcasting_forecast/app.py` & `nowcasting_forecast-1.3.4/nowcasting_forecast/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/nowcasting_forecast/batch.py` & `nowcasting_forecast-1.3.4/nowcasting_forecast/batch.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/nowcasting_forecast/dataloader.py` & `nowcasting_forecast-1.3.4/nowcasting_forecast/dataloader.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/nowcasting_forecast/models/hub.py` & `nowcasting_forecast-1.3.4/nowcasting_forecast/models/hub.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/nowcasting_forecast/models/nwp_solar_simple.py` & `nowcasting_forecast-1.3.4/nowcasting_forecast/models/nwp_solar_simple.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/nowcasting_forecast/models/sun.py` & `nowcasting_forecast-1.3.4/nowcasting_forecast/models/sun.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/nowcasting_forecast/models/utils.py` & `nowcasting_forecast-1.3.4/nowcasting_forecast/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/nowcasting_forecast/utils.py` & `nowcasting_forecast-1.3.4/nowcasting_forecast/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/nowcasting_forecast.egg-info/PKG-INFO` & `nowcasting_forecast-1.3.4/nowcasting_forecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-forecast
-Version: 1.3.3
+Version: 1.3.4
 Summary: Live forecast for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_forecast
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: artificial intelligence,forecast
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_forecast-1.3.3/nowcasting_forecast.egg-info/SOURCES.txt` & `nowcasting_forecast-1.3.4/nowcasting_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/setup.py` & `nowcasting_forecast-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/tests/test_app.py` & `nowcasting_forecast-1.3.4/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_forecast-1.3.3/tests/test_batch.py` & `nowcasting_forecast-1.3.4/tests/test_batch.py`

 * *Files identical despite different names*

