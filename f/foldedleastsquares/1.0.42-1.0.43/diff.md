# Comparing `tmp/foldedleastsquares-1.0.42.tar.gz` & `tmp/foldedleastsquares-1.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foldedleastsquares-1.0.42.tar", last modified: Thu Apr 13 20:38:35 2023, max compression
+gzip compressed data, was "foldedleastsquares-1.0.43.tar", last modified: Fri Apr 14 07:42:19 2023, max compression
```

## Comparing `foldedleastsquares-1.0.42.tar` & `foldedleastsquares-1.0.43.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:38:35.271780 foldedleastsquares-1.0.42/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-13 20:38:35.271780 foldedleastsquares-1.0.42/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:38:35.267780 foldedleastsquares-1.0.42/foldedleastsquares/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:38:35.267780 foldedleastsquares-1.0.42/foldedleastsquares/template_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/template_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/template_generator/default_transit_template_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/template_generator/tailed_transit_template_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/template_generator/transit_template_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:38:35.271780 foldedleastsquares-1.0.42/foldedleastsquares/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_FAP.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_catalog_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_cleaned_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_duration_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_multi_planet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_period_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_stats_gap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_transit_depth_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_uncertainties.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/tls_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/foldedleastsquares/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:38:35.267780 foldedleastsquares-1.0.42/foldedleastsquares.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-13 20:38:35.000000 foldedleastsquares-1.0.42/foldedleastsquares.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-13 20:38:35.000000 foldedleastsquares-1.0.42/foldedleastsquares.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:38:35.000000 foldedleastsquares-1.0.42/foldedleastsquares.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 20:38:35.000000 foldedleastsquares-1.0.42/foldedleastsquares.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 20:38:35.000000 foldedleastsquares-1.0.42/foldedleastsquares.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 20:38:35.000000 foldedleastsquares-1.0.42/foldedleastsquares.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:38:35.271780 foldedleastsquares-1.0.42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-13 20:38:26.000000 foldedleastsquares-1.0.42/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:42:19.106163 foldedleastsquares-1.0.43/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-14 07:42:19.106163 foldedleastsquares-1.0.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:42:19.102163 foldedleastsquares-1.0.43/foldedleastsquares/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:42:19.102163 foldedleastsquares-1.0.43/foldedleastsquares/template_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/template_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/template_generator/default_transit_template_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/template_generator/tailed_transit_template_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/template_generator/transit_template_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:42:19.106163 foldedleastsquares-1.0.43/foldedleastsquares/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_FAP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_catalog_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_cleaned_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_duration_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_multi_planet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_period_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_stats_gap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_transit_depth_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_uncertainties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/tls_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/foldedleastsquares/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:42:19.102163 foldedleastsquares-1.0.43/foldedleastsquares.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-14 07:42:18.000000 foldedleastsquares-1.0.43/foldedleastsquares.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-14 07:42:19.000000 foldedleastsquares-1.0.43/foldedleastsquares.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:42:18.000000 foldedleastsquares-1.0.43/foldedleastsquares.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 07:42:18.000000 foldedleastsquares-1.0.43/foldedleastsquares.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 07:42:18.000000 foldedleastsquares-1.0.43/foldedleastsquares.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 07:42:18.000000 foldedleastsquares-1.0.43/foldedleastsquares.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 07:42:19.106163 foldedleastsquares-1.0.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-14 07:42:08.000000 foldedleastsquares-1.0.43/setup.py
```

### Comparing `foldedleastsquares-1.0.42/LICENSE` & `foldedleastsquares-1.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/PKG-INFO` & `foldedleastsquares-1.0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldedleastsquares
-Version: 1.0.42
+Version: 1.0.43
 Summary: An optimized transit-fitting algorithm to search for periodic features in light curves
 Home-page: https://github.com/hippke/tls
 Author: Martín Dévora Pajares
 Author-email: martin.devora.pajares@gmail.com
 License: MIT
 Description: ![Logo](https://raw.githubusercontent.com/hippke/tls/master/docs/source/logo.png)
         ### An optimized transit-fitting algorithm to search for periodic transits of small planets
```

### Comparing `foldedleastsquares-1.0.42/README.md` & `foldedleastsquares-1.0.43/README.md`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/__init__.py` & `foldedleastsquares-1.0.43/foldedleastsquares/__init__.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/catalog.py` & `foldedleastsquares-1.0.43/foldedleastsquares/catalog.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/command_line.py` & `foldedleastsquares-1.0.43/foldedleastsquares/command_line.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/core.py` & `foldedleastsquares-1.0.43/foldedleastsquares/core.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/grid.py` & `foldedleastsquares-1.0.43/foldedleastsquares/grid.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/helpers.py` & `foldedleastsquares-1.0.43/foldedleastsquares/helpers.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/interpolation.py` & `foldedleastsquares-1.0.43/foldedleastsquares/interpolation.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/main.py` & `foldedleastsquares-1.0.43/foldedleastsquares/main.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/results.py` & `foldedleastsquares-1.0.43/foldedleastsquares/results.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/stats.py` & `foldedleastsquares-1.0.43/foldedleastsquares/stats.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/template_generator/default_transit_template_generator.py` & `foldedleastsquares-1.0.43/foldedleastsquares/template_generator/default_transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/template_generator/tailed_transit_template_generator.py` & `foldedleastsquares-1.0.43/foldedleastsquares/template_generator/tailed_transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/template_generator/transit_template_generator.py` & `foldedleastsquares-1.0.43/foldedleastsquares/template_generator/transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_catalog_data.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_catalog_data.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_cleaned_array.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_cleaned_array.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_duration_grid.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_duration_grid.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_multi_planet.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_multi_planet.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_period_grid.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_period_grid.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_resample.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_shapes.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_stats_gap.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_stats_gap.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_synthetic.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_transit_depth_min.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_transit_depth_min.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_uncertainties.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_uncertainties.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tests/test_validation.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/tls_constants.py` & `foldedleastsquares-1.0.43/foldedleastsquares/tls_constants.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares/validate.py` & `foldedleastsquares-1.0.43/foldedleastsquares/validate.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares.egg-info/PKG-INFO` & `foldedleastsquares-1.0.43/foldedleastsquares.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldedleastsquares
-Version: 1.0.42
+Version: 1.0.43
 Summary: An optimized transit-fitting algorithm to search for periodic features in light curves
 Home-page: https://github.com/hippke/tls
 Author: Martín Dévora Pajares
 Author-email: martin.devora.pajares@gmail.com
 License: MIT
 Description: ![Logo](https://raw.githubusercontent.com/hippke/tls/master/docs/source/logo.png)
         ### An optimized transit-fitting algorithm to search for periodic transits of small planets
```

### Comparing `foldedleastsquares-1.0.42/foldedleastsquares.egg-info/SOURCES.txt` & `foldedleastsquares-1.0.43/foldedleastsquares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.42/setup.py` & `foldedleastsquares-1.0.43/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     packages=setuptools.find_packages(),
     include_package_data=True,
     package_data={'': ['*.csv', '*.cfg']},
     entry_points = {'console_scripts': ['transitleastsquares=transitleastsquares.command_line:main'],},
     install_requires=[
         'astropy<3;python_version<"3"',  # astropy 3 doesn't install in Python 2, but is req for astroquery
         'astroquery>=0.3.9',  # earlier has bug for "from astroquery.mast import Catalogs"
-        'numpy',
-        'numba',
+        'numpy==1.23.5',
+        'numba==0.56.4',
         'tqdm',
         'batman-package',
         'argparse',
         'configparser'
         ]
 )
```

