# Comparing `tmp/dearwatson-0.6.1.tar.gz` & `tmp/dearwatson-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearwatson-0.6.1.tar", last modified: Wed Apr 12 20:50:55 2023, max compression
+gzip compressed data, was "dearwatson-0.7.0.tar", last modified: Fri Apr 14 18:49:27 2023, max compression
```

## Comparing `dearwatson-0.6.1.tar` & `dearwatson-0.7.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:55.745071 dearwatson-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 20:50:44.000000 dearwatson-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 20:50:44.000000 dearwatson-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-12 20:50:55.745071 dearwatson-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-12 20:50:44.000000 dearwatson-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:55.741071 dearwatson-0.6.1/dearwatson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-12 20:50:55.000000 dearwatson-0.6.1/dearwatson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-12 20:50:55.000000 dearwatson-0.6.1/dearwatson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:50:55.000000 dearwatson-0.6.1/dearwatson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 20:50:55.000000 dearwatson-0.6.1/dearwatson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 20:50:55.000000 dearwatson-0.6.1/dearwatson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:50:55.745071 dearwatson-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-12 20:50:45.000000 dearwatson-0.6.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-12 20:50:45.000000 dearwatson-0.6.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:55.741071 dearwatson-0.6.1/watson/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:55.741071 dearwatson-0.6.1/watson/data_validation_report/
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/data_validation_report/DvrPreparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/data_validation_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:55.737071 dearwatson-0.6.1/watson/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:55.741071 dearwatson-0.6.1/watson/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/resources/images/sherlock3.png
--rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/resources/images/watson.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:55.741071 dearwatson-0.6.1/watson/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/tests/test_watson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:50:55.745071 dearwatson-0.6.1/watson/tpfplotterSub/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:50:46.000000 dearwatson-0.6.1/watson/tpfplotterSub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-04-12 20:50:46.000000 dearwatson-0.6.1/watson/tpfplotterSub/tpfplotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-12 20:50:46.000000 dearwatson-0.6.1/watson/tpfplotterSub/tpfplotter_py2.py
--rw-r--r--   0 runner    (1001) docker     (123)   106233 2023-04-12 20:50:45.000000 dearwatson-0.6.1/watson/watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.644649 dearwatson-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-14 18:49:15.000000 dearwatson-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 18:49:15.000000 dearwatson-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-14 18:49:27.644649 dearwatson-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-14 18:49:15.000000 dearwatson-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.640649 dearwatson-0.7.0/dearwatson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-14 18:49:27.000000 dearwatson-0.7.0/dearwatson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-14 18:49:27.000000 dearwatson-0.7.0/dearwatson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:49:27.000000 dearwatson-0.7.0/dearwatson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 18:49:27.000000 dearwatson-0.7.0/dearwatson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 18:49:27.000000 dearwatson-0.7.0/dearwatson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:49:27.644649 dearwatson-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 18:49:16.000000 dearwatson-0.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 18:49:16.000000 dearwatson-0.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.640649 dearwatson-0.7.0/watson/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.640649 dearwatson-0.7.0/watson/data_validation_report/
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/data_validation_report/DvrPreparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/data_validation_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.640649 dearwatson-0.7.0/watson/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.640649 dearwatson-0.7.0/watson/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   524520 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/resources/images/sherlock3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   738619 2023-04-14 18:49:16.000000 dearwatson-0.7.0/watson/resources/images/watson.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.644649 dearwatson-0.7.0/watson/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:17.000000 dearwatson-0.7.0/watson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-14 18:49:17.000000 dearwatson-0.7.0/watson/tests/test_watson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:49:27.644649 dearwatson-0.7.0/watson/tpfplotterSub/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:49:18.000000 dearwatson-0.7.0/watson/tpfplotterSub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-04-14 18:49:18.000000 dearwatson-0.7.0/watson/tpfplotterSub/tpfplotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-14 18:49:18.000000 dearwatson-0.7.0/watson/tpfplotterSub/tpfplotter_py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106233 2023-04-14 18:49:17.000000 dearwatson-0.7.0/watson/watson.py
```

### Comparing `dearwatson-0.6.1/LICENSE` & `dearwatson-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/PKG-INFO` & `dearwatson-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.6.1
+Version: 0.7.0
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.6.1/README.md` & `dearwatson-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/dearwatson.egg-info/PKG-INFO` & `dearwatson-0.7.0/dearwatson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.6.1
+Version: 0.7.0
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.6.1/dearwatson.egg-info/SOURCES.txt` & `dearwatson-0.7.0/dearwatson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/setup.py` & `dearwatson-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.6.1"
+version = "0.7.0"
 setuptools.setup(
     name="dearwatson", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Visual Vetting and Analysis of Transits from Space ObservatioNs",
     long_description=long_description,
@@ -23,15 +23,15 @@
     python_requires='>=3.8',
     install_requires=[
                         "bokeh==2.4.2", # TPFPlotter dependency
                         'configparser==5.0.1',
                         "cython==0.29.21",
                         "extension-helpers==0.1",
                         "imageio==2.9.0",
-                        "lcbuilder==0.11.2",
+                        "lcbuilder==0.12.0",
                         "matplotlib==3.5.2",
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "pyyaml==5.4.1",
                         "reportlab==3.5.59",
                         'setuptools>=41.0.0',
     ]
 )
```

### Comparing `dearwatson-0.6.1/watson/data_validation_report/DvrPreparer.py` & `dearwatson-0.7.0/watson/data_validation_report/DvrPreparer.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/watson/neighbours.py` & `dearwatson-0.7.0/watson/neighbours.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/watson/report.py` & `dearwatson-0.7.0/watson/report.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/watson/resources/images/sherlock3.png` & `dearwatson-0.7.0/watson/resources/images/sherlock3.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/watson/resources/images/watson.png` & `dearwatson-0.7.0/watson/resources/images/watson.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/watson/tests/test_watson.py` & `dearwatson-0.7.0/watson/tests/test_watson.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/watson/tpfplotterSub/tpfplotter.py` & `dearwatson-0.7.0/watson/tpfplotterSub/tpfplotter.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/watson/tpfplotterSub/tpfplotter_py2.py` & `dearwatson-0.7.0/watson/tpfplotterSub/tpfplotter_py2.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.6.1/watson/watson.py` & `dearwatson-0.7.0/watson/watson.py`

 * *Files identical despite different names*

