# Comparing `tmp/nowcasting_datamodel-1.3.2.tar.gz` & `tmp/nowcasting_datamodel-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.3.2.tar", last modified: Fri Apr 14 14:15:29 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.3.3.tar", last modified: Fri Apr 14 15:09:31 2023, max compression
```

## Comparing `nowcasting_datamodel-1.3.2.tar` & `nowcasting_datamodel-1.3.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:29.676996 nowcasting_datamodel-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-14 14:15:29.676996 nowcasting_datamodel-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:29.672996 nowcasting_datamodel-1.3.2/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:29.672996 nowcasting_datamodel-1.3.2/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:29.672996 nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:29.672996 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:29.672996 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/read_pv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:29.676996 nowcasting_datamodel-1.3.2/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:29.672996 nowcasting_datamodel-1.3.2/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-14 14:15:29.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-14 14:15:29.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:15:29.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 14:15:29.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 14:15:29.000000 nowcasting_datamodel-1.3.2/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:15:29.676996 nowcasting_datamodel-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:15:29.676996 nowcasting_datamodel-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-14 14:15:18.000000 nowcasting_datamodel-1.3.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.250066 nowcasting_datamodel-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-14 15:09:31.250066 nowcasting_datamodel-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.246066 nowcasting_datamodel-1.3.3/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.246066 nowcasting_datamodel-1.3.3/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.246066 nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.246066 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.250066 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/read_pv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.250066 nowcasting_datamodel-1.3.3/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.246066 nowcasting_datamodel-1.3.3/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-14 15:09:31.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-14 15:09:31.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:09:31.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 15:09:31.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 15:09:31.000000 nowcasting_datamodel-1.3.3/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:09:31.250066 nowcasting_datamodel-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:09:31.250066 nowcasting_datamodel-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-14 15:09:21.000000 nowcasting_datamodel-1.3.3/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.3.2/PKG-INFO` & `nowcasting_datamodel-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.3.2
+Version: 1.3.3
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.3.2/README.md` & `nowcasting_datamodel-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/diagram.png` & `nowcasting_datamodel-1.3.3/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/diagram_pv.png` & `nowcasting_datamodel-1.3.3/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/fake.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,28 +276,26 @@
         start_datetime_utc=datetime(2023, 1, 1),
         end_datetime_utc=datetime(2023, 1, 8),
     )
     location = get_location(
         gsp_id=0, session=session, installed_capacity_mw=14000, label=national_gb_label
     )
 
-    model = get_model(session=session, name="fake_model", version="0.1.2")
-
     session.add_all([location, datetime_interval, metric])
 
     metric_values = []
     for forecast_horizon in range(0, 60 * 9, 30):
         for minutes in range(0, 60 * 24, 30):
             time_of_day = time(hour=minutes // 60, minute=minutes % 60)
             m = MetricValueSQL(
                 value=forecast_horizon * 10000 + minutes,
                 time_of_day=time_of_day,
                 forecast_horizon_minutes=forecast_horizon,
                 number_of_data_points=1,
                 datetime_interval=datetime_interval,
                 metric=metric,
                 location=location,
-                model=model,
+                model_name="fake_model",
             )
             metric_values.append(m)
 
     return metric_values
```

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     __tablename__ = "metric_value"
 
     id = Column(Integer, primary_key=True)
     value = Column(Float, nullable=False)
     number_of_data_points = Column(Integer, nullable=False)
     forecast_horizon_minutes = Column(Integer, nullable=True)
     time_of_day = Column(Time, nullable=True)
+    model_name = Column(String, nullable=True)
 
     # many (metric values) to one (metric)
     metric = relationship("MetricSQL", back_populates="metric_value")
     metric_id = Column(Integer, ForeignKey("metric.id"), index=True)
 
     # many (metric values) to one (location)
     location = relationship("LocationSQL", back_populates="metric_value")
@@ -146,14 +147,16 @@
     datetime_interval_id = Column(Integer, ForeignKey("datetime_interval.id"), index=True)
 
     # many (metric values) to one (model)
     model = relationship("MLModelSQL", back_populates="metric_value")
     model_id = Column(Integer, ForeignKey("model.id"), index=True)
 
 
+
+
 class MetricValue(EnhancedBaseModel):
     """Location that the forecast is for"""
 
     value: str = Field(..., description="The value of the metric")
     number_of_data_points: int = Field(
         ..., description="The number of data points used to make the value"
     )
```

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/blend/blend.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/blend/blend.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/blend/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/read_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,13 @@
     query = query.order_by(
         MetricValueSQL.time_of_day,
         MetricValueSQL.forecast_horizon_minutes,
         MetricValueSQL.created_utc.desc(),
     )
 
     if model_name is not None:
-        query = query.join(MLModelSQL)
-        query = query.filter(MLModelSQL.name == model_name)
+        query = query.filter(MetricValueSQL.model_name == model_name)
 
     # get all results
     metric_values = query.all()
 
     return metric_values
```

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.3.2
+Version: 1.3.3
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.3.2/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.3.3/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/setup.py` & `nowcasting_datamodel-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.3.3/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/tests/test_fake.py` & `nowcasting_datamodel-1.3.3/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/tests/test_fake_pv.py` & `nowcasting_datamodel-1.3.3/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/tests/test_national.py` & `nowcasting_datamodel-1.3.3/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.2/tests/test_utils.py` & `nowcasting_datamodel-1.3.3/tests/test_utils.py`

 * *Files identical despite different names*

