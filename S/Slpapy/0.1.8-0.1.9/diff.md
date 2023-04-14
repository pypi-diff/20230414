# Comparing `tmp/Slpapy-0.1.8.tar.gz` & `tmp/Slpapy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.1.8.tar", last modified: Mon Apr 10 03:56:31 2023, max compression
+gzip compressed data, was "Slpapy-0.1.9.tar", last modified: Fri Apr 14 06:22:28 2023, max compression
```

## Comparing `Slpapy-0.1.8.tar` & `Slpapy-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:56:31.844361 Slpapy-0.1.8/
--rw-rw-rw-   0        0        0      159 2023-04-10 03:56:31.843361 Slpapy-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 03:56:31.832360 Slpapy-0.1.8/Slpapy/
--rw-rw-rw-   0        0        0     1924 2023-04-10 03:20:00.000000 Slpapy-0.1.8/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.8/Slpapy/MZ_ppm_match.py
--rw-rw-rw-   0        0        0      453 2023-04-06 10:17:32.000000 Slpapy-0.1.8/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5164 2023-04-10 03:33:43.000000 Slpapy-0.1.8/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:56:31.841361 Slpapy-0.1.8/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-04-10 03:56:31.000000 Slpapy-0.1.8/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-10 03:56:31.000000 Slpapy-0.1.8/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:56:31.000000 Slpapy-0.1.8/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-10 03:56:31.000000 Slpapy-0.1.8/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 03:56:31.000000 Slpapy-0.1.8/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 03:56:31.844361 Slpapy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      486 2023-04-10 03:56:14.000000 Slpapy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 06:22:28.760415 Slpapy-0.1.9/
+-rw-rw-rw-   0        0        0      159 2023-04-14 06:22:28.759413 Slpapy-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 06:22:28.748412 Slpapy-0.1.9/Slpapy/
+-rw-rw-rw-   0        0        0     1924 2023-04-10 03:20:00.000000 Slpapy-0.1.9/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.9/Slpapy/MZ_ppm_match.py
+-rw-rw-rw-   0        0        0      525 2023-04-14 06:21:10.000000 Slpapy-0.1.9/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5164 2023-04-10 03:33:43.000000 Slpapy-0.1.9/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-04-14 06:22:28.757414 Slpapy-0.1.9/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-04-14 06:22:28.000000 Slpapy-0.1.9/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-14 06:22:28.000000 Slpapy-0.1.9/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 06:22:28.000000 Slpapy-0.1.9/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-14 06:22:28.000000 Slpapy-0.1.9/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 06:22:28.000000 Slpapy-0.1.9/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 06:22:28.760415 Slpapy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      486 2023-04-14 06:21:10.000000 Slpapy-0.1.9/setup.py
```

### Comparing `Slpapy-0.1.8/Slpapy/Data_reconstruction.py` & `Slpapy-0.1.9/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.8/Slpapy/MZ_ppm_match.py` & `Slpapy-0.1.9/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.8/Slpapy/processing_analyze.py` & `Slpapy-0.1.9/Slpapy/processing_analyze.py`

 * *Files identical despite different names*

