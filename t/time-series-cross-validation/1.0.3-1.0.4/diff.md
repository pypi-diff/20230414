# Comparing `tmp/time_series_cross_validation-1.0.3.tar.gz` & `tmp/time_series_cross_validation-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series_cross_validation-1.0.3.tar", last modified: Wed Apr 12 13:45:44 2023, max compression
+gzip compressed data, was "time_series_cross_validation-1.0.4.tar", last modified: Fri Apr 14 00:54:06 2023, max compression
```

## Comparing `time_series_cross_validation-1.0.3.tar` & `time_series_cross_validation-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-12 13:45:44.591994 time_series_cross_validation-1.0.3/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 20:55:29.000000 time_series_cross_validation-1.0.3/LICENSE.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-12 13:45:44.591994 time_series_cross_validation-1.0.3/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       35 2023-04-11 20:55:44.000000 time_series_cross_validation-1.0.3/README.md
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-12 13:45:44.591994 time_series_cross_validation-1.0.3/setup.cfg
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      784 2023-04-12 13:45:17.000000 time_series_cross_validation-1.0.3/setup.py
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-12 13:45:44.591994 time_series_cross_validation-1.0.3/time_series_cross_validation/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       56 2023-04-11 21:13:00.000000 time_series_cross_validation-1.0.3/time_series_cross_validation/__init__.py
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     6185 2023-04-12 13:45:01.000000 time_series_cross_validation-1.0.3/time_series_cross_validation/time_series_cross_validation.py
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-12 13:45:44.591994 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-12 13:45:44.000000 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      391 2023-04-12 13:45:44.000000 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/SOURCES.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-12 13:45:44.000000 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/dependency_links.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       32 2023-04-12 13:45:44.000000 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/requires.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       29 2023-04-12 13:45:44.000000 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/top_level.txt
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-14 00:54:06.286413 time_series_cross_validation-1.0.4/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 20:55:29.000000 time_series_cross_validation-1.0.4/LICENSE.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-14 00:54:06.286413 time_series_cross_validation-1.0.4/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       35 2023-04-11 20:55:44.000000 time_series_cross_validation-1.0.4/README.md
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-14 00:54:06.286413 time_series_cross_validation-1.0.4/setup.cfg
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      784 2023-04-14 00:53:44.000000 time_series_cross_validation-1.0.4/setup.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-14 00:54:06.286413 time_series_cross_validation-1.0.4/time_series_cross_validation/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       56 2023-04-11 21:13:00.000000 time_series_cross_validation-1.0.4/time_series_cross_validation/__init__.py
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     5204 2023-04-14 00:53:37.000000 time_series_cross_validation-1.0.4/time_series_cross_validation/time_series_cross_validation.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-14 00:54:06.286413 time_series_cross_validation-1.0.4/time_series_cross_validation.egg-info/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-14 00:54:06.000000 time_series_cross_validation-1.0.4/time_series_cross_validation.egg-info/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      391 2023-04-14 00:54:06.000000 time_series_cross_validation-1.0.4/time_series_cross_validation.egg-info/SOURCES.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-14 00:54:06.000000 time_series_cross_validation-1.0.4/time_series_cross_validation.egg-info/dependency_links.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       32 2023-04-14 00:54:06.000000 time_series_cross_validation-1.0.4/time_series_cross_validation.egg-info/requires.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       29 2023-04-14 00:54:06.000000 time_series_cross_validation-1.0.4/time_series_cross_validation.egg-info/top_level.txt
```

### Comparing `time_series_cross_validation-1.0.3/LICENSE.txt` & `time_series_cross_validation-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `time_series_cross_validation-1.0.3/PKG-INFO` & `time_series_cross_validation-1.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time_series_cross_validation
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for cross-validating time series
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep time series cross validation data science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `time_series_cross_validation-1.0.3/setup.py` & `time_series_cross_validation-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='time_series_cross_validation',
-    version='1.0.3',
+    version='1.0.4',
     description='Library for cross-validating time series',
     long_description = 'Library for cross-validating time series',
     author='Gabriel Nuernberg Biazoto',
     author_email='biazotogabriel@gmail.com',
     url='https://github.com/biazotogabriel/deep_tracking',
     packages=['time_series_cross_validation'],
     license = 'MIT',
```

### Comparing `time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/PKG-INFO` & `time_series_cross_validation-1.0.4/time_series_cross_validation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-series-cross-validation
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for cross-validating time series
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep time series cross validation data science
 Classifier: Programming Language :: Python :: 3
```

