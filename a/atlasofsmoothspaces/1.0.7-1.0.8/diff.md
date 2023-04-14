# Comparing `tmp/atlasofsmoothspaces-1.0.7.tar.gz` & `tmp/atlasofsmoothspaces-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasofsmoothspaces-1.0.7.tar", last modified: Thu Apr 13 19:01:21 2023, max compression
+gzip compressed data, was "atlasofsmoothspaces-1.0.8.tar", last modified: Fri Apr 14 03:10:33 2023, max compression
```

## Comparing `atlasofsmoothspaces-1.0.7.tar` & `atlasofsmoothspaces-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-13 19:01:21.334562 atlasofsmoothspaces-1.0.7/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-13 19:01:21.330562 atlasofsmoothspaces-1.0.7/PKG-INFO
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-13 19:01:21.330562 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces/__init__.py
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)    12951 2023-04-13 18:59:47.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces/main.py
-drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-13 19:01:21.330562 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces.egg-info/
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-13 19:01:21.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces.egg-info/PKG-INFO
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-13 19:01:21.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces.egg-info/SOURCES.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-13 19:01:21.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces.egg-info/dependency_links.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-13 19:01:21.000000 atlasofsmoothspaces-1.0.7/atlasofsmoothspaces.egg-info/top_level.txt
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-13 19:01:21.334562 atlasofsmoothspaces-1.0.7/setup.cfg
--rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-13 19:00:31.000000 atlasofsmoothspaces-1.0.7/setup.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-14 03:10:33.300506 atlasofsmoothspaces-1.0.8/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-14 03:10:33.300506 atlasofsmoothspaces-1.0.8/PKG-INFO
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-14 03:10:33.300506 atlasofsmoothspaces-1.0.8/atlasofsmoothspaces/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       19 2023-04-11 07:32:02.000000 atlasofsmoothspaces-1.0.8/atlasofsmoothspaces/__init__.py
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)    20746 2023-04-14 03:02:55.000000 atlasofsmoothspaces-1.0.8/atlasofsmoothspaces/main.py
+drwxrwxr-x   0 leonhard  (1000) leonhard  (1000)        0 2023-04-14 03:10:33.300506 atlasofsmoothspaces-1.0.8/atlasofsmoothspaces.egg-info/
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      442 2023-04-14 03:10:33.000000 atlasofsmoothspaces-1.0.8/atlasofsmoothspaces.egg-info/PKG-INFO
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      240 2023-04-14 03:10:33.000000 atlasofsmoothspaces-1.0.8/atlasofsmoothspaces.egg-info/SOURCES.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)        1 2023-04-14 03:10:33.000000 atlasofsmoothspaces-1.0.8/atlasofsmoothspaces.egg-info/dependency_links.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       20 2023-04-14 03:10:33.000000 atlasofsmoothspaces-1.0.8/atlasofsmoothspaces.egg-info/top_level.txt
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)       38 2023-04-14 03:10:33.300506 atlasofsmoothspaces-1.0.8/setup.cfg
+-rw-rw-r--   0 leonhard  (1000) leonhard  (1000)      888 2023-04-13 19:13:59.000000 atlasofsmoothspaces-1.0.8/setup.py
```

### Comparing `atlasofsmoothspaces-1.0.7/setup.py` & `atlasofsmoothspaces-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.7' 
+VERSION = '1.0.8' 
 DESCRIPTION = 'Calculating Smoothness from Input Stream'
 LONG_DESCRIPTION = 'Smoothness is calculated from an input stream. The input data format is midi.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="atlasofsmoothspaces",
```

