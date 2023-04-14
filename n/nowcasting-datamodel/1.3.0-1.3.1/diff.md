# Comparing `tmp/nowcasting_datamodel-1.3.0.tar.gz` & `tmp/nowcasting_datamodel-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.3.0.tar", last modified: Wed Apr 12 11:46:36 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.3.1.tar", last modified: Fri Apr 14 13:07:53 2023, max compression
```

## Comparing `nowcasting_datamodel-1.3.0.tar` & `nowcasting_datamodel-1.3.1.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:46:36.073648 nowcasting_datamodel-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-12 11:46:36.073648 nowcasting_datamodel-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:46:36.065648 nowcasting_datamodel-1.3.0/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:46:36.069648 nowcasting_datamodel-1.3.0/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:46:36.069648 nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:46:36.069648 nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)    22415 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/read_pv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:46:36.073648 nowcasting_datamodel-1.3.0/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:46:36.065648 nowcasting_datamodel-1.3.0/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-12 11:46:36.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-12 11:46:36.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 11:46:36.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 11:46:36.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 11:46:36.000000 nowcasting_datamodel-1.3.0/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 11:46:36.073648 nowcasting_datamodel-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 11:46:36.073648 nowcasting_datamodel-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-12 11:46:23.000000 nowcasting_datamodel-1.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:53.612360 nowcasting_datamodel-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-14 13:07:53.612360 nowcasting_datamodel-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:53.608360 nowcasting_datamodel-1.3.1/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:53.608360 nowcasting_datamodel-1.3.1/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:53.608360 nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:53.612360 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:53.612360 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/read_pv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:53.612360 nowcasting_datamodel-1.3.1/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:53.608360 nowcasting_datamodel-1.3.1/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-14 13:07:53.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-14 13:07:53.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:07:53.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 13:07:53.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 13:07:53.000000 nowcasting_datamodel-1.3.1/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:07:53.612360 nowcasting_datamodel-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:07:53.612360 nowcasting_datamodel-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-14 13:07:44.000000 nowcasting_datamodel-1.3.1/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.3.0/PKG-INFO` & `nowcasting_datamodel-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.3.0
+Version: 1.3.1
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.3.0/README.md` & `nowcasting_datamodel-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/diagram.png` & `nowcasting_datamodel-1.3.1/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/diagram_pv.png` & `nowcasting_datamodel-1.3.1/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,19 +382,20 @@
 
     return query
 
 
 def get_forecast_values(
     session: Session,
     gsp_id: Optional[int] = None,
-    gsp_ids: Optional[int] = None,
+    gsp_ids: Optional[List[int]] = None,
     start_datetime: Optional[datetime] = None,
     forecast_horizon_minutes: Optional[int] = None,
     only_return_latest: Optional[bool] = False,
     model: Optional = ForecastValueSQL,
+    model_name: Optional[str] = None,
 ) -> List[ForecastValueSQL]:
     """
     Get forecast values
 
     :param session: database session
     :param gsp_id: optional to gsp id, to filter query on
         If None is given then all are returned. This should be changed to [gsp_id]
@@ -450,32 +451,37 @@
             >= text(f"interval '{forecast_horizon_minutes} minute'")
         )
         query = query.filter(
             model.created_utc - datetime.now(tz=timezone.utc)
             <= text(f"interval '{forecast_horizon_minutes} minute'")
         )
 
+    if (gsp_id is not None) or (gsp_ids is not None) or (model_name is not None):
+        query = query.join(ForecastSQL)
+
     # filter on gsp_id
     if gsp_id is not None:
         logger.warning('We should now use "gsp_ids" not "gsp_id"')
-        query = query.join(ForecastSQL)
         query = query.join(LocationSQL)
         query = query.filter(LocationSQL.gsp_id == gsp_id)
 
     if gsp_ids is not None:
         logger.debug(f"Filtering for {gsp_ids=}")
-        query = query.join(ForecastSQL)
         query = query.join(LocationSQL)
         query = query.filter(LocationSQL.gsp_id.in_(gsp_ids))
 
         # prevent n+1 queries on forecasts after initial query
         query = query.options(
             contains_eager(model.forecast, ForecastSQL.location)
         ).populate_existing()
 
+    if model_name is not None:
+        query = query.join(MLModelSQL)
+        query = query.filter(MLModelSQL.name == model_name)
+
     # order by target time and created time desc
     query = query.order_by(*order_by_columns)
 
     # get all results
     forecasts = query.all()
 
     # add utc timezone
```

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.3.0
+Version: 1.3.1
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.3.0/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.3.1/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,19 +22,22 @@
 nowcasting_datamodel/models/forecast.py
 nowcasting_datamodel/models/gsp.py
 nowcasting_datamodel/models/metric.py
 nowcasting_datamodel/models/models.py
 nowcasting_datamodel/models/pv.py
 nowcasting_datamodel/models/utils.py
 nowcasting_datamodel/read/__init__.py
-nowcasting_datamodel/read/blend.py
 nowcasting_datamodel/read/read.py
 nowcasting_datamodel/read/read_gsp.py
 nowcasting_datamodel/read/read_metric.py
 nowcasting_datamodel/read/read_pv.py
+nowcasting_datamodel/read/blend/__init__.py
+nowcasting_datamodel/read/blend/blend.py
+nowcasting_datamodel/read/blend/utils.py
+nowcasting_datamodel/read/blend/weights.py
 nowcasting_datamodel/save/__init__.py
 nowcasting_datamodel/save/adjust.py
 nowcasting_datamodel/save/save.py
 nowcasting_datamodel/save/update.py
 tests/test_databaseconnection.py
 tests/test_fake.py
 tests/test_fake_pv.py
```

### Comparing `nowcasting_datamodel-1.3.0/setup.py` & `nowcasting_datamodel-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.3.1/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/tests/test_fake.py` & `nowcasting_datamodel-1.3.1/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/tests/test_fake_pv.py` & `nowcasting_datamodel-1.3.1/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/tests/test_national.py` & `nowcasting_datamodel-1.3.1/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.3.0/tests/test_utils.py` & `nowcasting_datamodel-1.3.1/tests/test_utils.py`

 * *Files identical despite different names*

