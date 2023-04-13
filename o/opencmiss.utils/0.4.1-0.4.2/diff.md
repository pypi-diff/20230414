# Comparing `tmp/opencmiss.utils-0.4.1.tar.gz` & `tmp/opencmiss.utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss.utils-0.4.1.tar", last modified: Tue Jul 26 03:49:10 2022, max compression
+gzip compressed data, was "opencmiss.utils-0.4.2.tar", last modified: Thu Apr 13 22:22:03 2023, max compression
```

## Comparing `opencmiss.utils-0.4.1.tar` & `opencmiss.utils-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,12 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 03:49:10.020649 opencmiss.utils-0.4.1/
--rw-r--r--   0 hsor001  (1210695619) 1403514002    11357 2020-11-24 09:14:04.000000 opencmiss.utils-0.4.1/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002    13859 2022-07-26 03:49:10.020325 opencmiss.utils-0.4.1/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      389 2020-11-24 09:14:04.000000 opencmiss.utils-0.4.1/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2022-07-26 03:49:10.020736 opencmiss.utils-0.4.1/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1442 2021-11-01 11:14:16.000000 opencmiss.utils-0.4.1/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 03:49:10.014294 opencmiss.utils-0.4.1/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 03:49:10.015783 opencmiss.utils-0.4.1/src/opencmiss/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      123 2020-11-24 09:14:04.000000 opencmiss.utils-0.4.1/src/opencmiss/__init__.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 03:49:10.017836 opencmiss.utils-0.4.1/src/opencmiss/utils/
--rw-r--r--   0 hsor001  (1210695619) 1403514002       23 2022-07-26 03:47:30.000000 opencmiss.utils-0.4.1/src/opencmiss/utils/__init__.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 03:49:10.018339 opencmiss.utils-0.4.1/src/opencmiss/utils/geometry/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2020-11-24 09:14:04.000000 opencmiss.utils-0.4.1/src/opencmiss/utils/geometry/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3344 2022-06-07 04:35:46.000000 opencmiss.utils-0.4.1/src/opencmiss/utils/geometry/plane.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     2574 2022-06-07 23:36:32.000000 opencmiss.utils-0.4.1/src/opencmiss/utils/image.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 03:49:10.019871 opencmiss.utils-0.4.1/src/opencmiss/utils/zinc/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2020-11-24 09:14:04.000000 opencmiss.utils-0.4.1/src/opencmiss/utils/zinc/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    31332 2022-06-07 23:30:59.000000 opencmiss.utils-0.4.1/src/opencmiss/utils/zinc/field.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    18088 2022-06-07 23:27:58.000000 opencmiss.utils-0.4.1/src/opencmiss/utils/zinc/finiteelement.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6118 2022-06-07 23:28:59.000000 opencmiss.utils-0.4.1/src/opencmiss/utils/zinc/general.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1665 2020-11-24 09:14:04.000000 opencmiss.utils-0.4.1/src/opencmiss/utils/zinc/material.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-07-26 03:49:10.017345 opencmiss.utils-0.4.1/src/opencmiss.utils.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002    13859 2022-07-26 03:49:09.000000 opencmiss.utils-0.4.1/src/opencmiss.utils.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      635 2022-07-26 03:49:09.000000 opencmiss.utils-0.4.1/src/opencmiss.utils.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-07-26 03:49:09.000000 opencmiss.utils-0.4.1/src/opencmiss.utils.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2020-11-24 09:14:44.000000 opencmiss.utils-0.4.1/src/opencmiss.utils.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002       31 2022-07-26 03:49:09.000000 opencmiss.utils-0.4.1/src/opencmiss.utils.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       10 2022-07-26 03:49:09.000000 opencmiss.utils-0.4.1/src/opencmiss.utils.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-13 22:22:03.752923 opencmiss.utils-0.4.2/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    11357 2023-04-13 21:56:10.000000 opencmiss.utils-0.4.2/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      636 2023-04-13 22:22:03.752701 opencmiss.utils-0.4.2/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      299 2023-04-13 22:14:27.000000 opencmiss.utils-0.4.2/README.rst
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-13 22:22:03.752383 opencmiss.utils-0.4.2/opencmiss.utils.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      636 2023-04-13 22:22:03.000000 opencmiss.utils-0.4.2/opencmiss.utils.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      221 2023-04-13 22:22:03.000000 opencmiss.utils-0.4.2/opencmiss.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-13 22:22:03.000000 opencmiss.utils-0.4.2/opencmiss.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       13 2023-04-13 22:22:03.000000 opencmiss.utils-0.4.2/opencmiss.utils.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-13 22:22:03.000000 opencmiss.utils-0.4.2/opencmiss.utils.egg-info/top_level.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-13 22:22:03.753007 opencmiss.utils-0.4.2/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      742 2023-04-13 22:21:33.000000 opencmiss.utils-0.4.2/setup.py
```

### Comparing `opencmiss.utils-0.4.1/LICENSE` & `opencmiss.utils-0.4.2/LICENSE`

 * *Files identical despite different names*

