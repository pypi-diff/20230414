# Comparing `tmp/energyplus_idd_idf_utilities-0.87.tar.gz` & `tmp/energyplus_idd_idf_utilities-0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_idd_idf_utilities-0.87.tar", last modified: Thu Mar  2 19:27:13 2023, max compression
+gzip compressed data, was "energyplus_idd_idf_utilities-0.88.tar", last modified: Fri Apr 14 15:26:34 2023, max compression
```

## Comparing `energyplus_idd_idf_utilities-0.87.tar` & `energyplus_idd_idf_utilities-0.88.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 19:27:13.651886 energyplus_idd_idf_utilities-0.87/
--rw-r--r--   0 runner    (1001) docker     (122)     6333 2023-03-02 19:27:13.651886 energyplus_idd_idf_utilities-0.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 19:27:13.651886 energyplus_idd_idf_utilities-0.87/energyplus_idd_idf_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6333 2023-03-02 19:27:13.000000 energyplus_idd_idf_utilities-0.87/energyplus_idd_idf_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-03-02 19:27:13.000000 energyplus_idd_idf_utilities-0.87/energyplus_idd_idf_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-02 19:27:13.000000 energyplus_idd_idf_utilities-0.87/energyplus_idd_idf_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-03-02 19:27:13.000000 energyplus_idd_idf_utilities-0.87/energyplus_idd_idf_utilities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-02 19:27:13.000000 energyplus_idd_idf_utilities-0.87/energyplus_idd_idf_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 19:27:13.651886 energyplus_idd_idf_utilities-0.87/energyplus_iddidf/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/energyplus_iddidf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/energyplus_iddidf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4305 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/energyplus_iddidf/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     4040 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/energyplus_iddidf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/energyplus_iddidf/idd_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    25443 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/energyplus_iddidf/idd_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)    17223 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/energyplus_iddidf/idf_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     9393 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/energyplus_iddidf/idf_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/energyplus_iddidf/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-03-02 19:27:13.651886 energyplus_idd_idf_utilities-0.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-03-02 19:27:04.000000 energyplus_idd_idf_utilities-0.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:34.256370 energyplus_idd_idf_utilities-0.88/
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6712 2023-04-14 15:26:34.256370 energyplus_idd_idf_utilities-0.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:34.252370 energyplus_idd_idf_utilities-0.88/energyplus_idd_idf_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6712 2023-04-14 15:26:34.000000 energyplus_idd_idf_utilities-0.88/energyplus_idd_idf_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-14 15:26:34.000000 energyplus_idd_idf_utilities-0.88/energyplus_idd_idf_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 15:26:34.000000 energyplus_idd_idf_utilities-0.88/energyplus_idd_idf_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-14 15:26:34.000000 energyplus_idd_idf_utilities-0.88/energyplus_idd_idf_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-14 15:26:34.000000 energyplus_idd_idf_utilities-0.88/energyplus_idd_idf_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:34.256370 energyplus_idd_idf_utilities-0.88/energyplus_iddidf/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/energyplus_iddidf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/energyplus_iddidf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4305 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/energyplus_iddidf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4040 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/energyplus_iddidf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/energyplus_iddidf/idd_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25443 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/energyplus_iddidf/idd_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17223 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/energyplus_iddidf/idf_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9393 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/energyplus_iddidf/idf_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/energyplus_iddidf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-14 15:26:34.256370 energyplus_idd_idf_utilities-0.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-04-14 15:26:25.000000 energyplus_idd_idf_utilities-0.88/setup.py
```

### Comparing `energyplus_idd_idf_utilities-0.87/PKG-INFO` & `energyplus_idd_idf_utilities-0.88/energyplus_idd_idf_utilities.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
-Name: energyplus_idd_idf_utilities
-Version: 0.87
+Name: energyplus-idd-idf-utilities
+Version: 0.88
 Summary: EnergyPlus idd/idf manipulation in Python.
 Home-page: https://github.com/myoldmopar/py-idd-idf
-Author: Edwin Lee
-Author-email: leeed2001@gmail.com
-License: UnlicensedForNow
+Author: Edwin Lee, for NREL, for the United States Department of Energy
+License: ModifiedBSD
 Description: # EnergyPlus Python IDD/IDF Utilities
         
         Python library of EnergyPlus IDD/IDF manipulation utilities.
         
         ## Documentation
         
         [![Documentation Status](https://readthedocs.org/projects/energyplus-idd-idf/badge/?version=latest)](https://energyplus-idd-idf.readthedocs.io/en/latest/?badge=latest)
@@ -135,15 +134,21 @@
         ## Test Coverage
         
         [![Coverage Status](https://coveralls.io/repos/github/Myoldmopar/py-idd-idf/badge.svg?branch=master)](https://coveralls.io/github/Myoldmopar/py-idd-idf?branch=master)
         
         Coverage of the code from unit testing is reported to Coveralls at https://coveralls.io/github/Myoldmopar/py-idd-idf.
         Anything less than 100% coverage will be frowned upon. :)
         
-Platform: UNKNOWN
+Keywords: energyplus_launch,ep_launch,EnergyPlus,eplus,Energy+,Building Simulation,Whole Building Energy Simulation,Heat Transfer,HVAC,Modeling
+Platform: Linux (Tested on Ubuntu)
+Platform: MacOSX
+Platform: Windows
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Utilities
-Classifier: License :: Public Domain
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `energyplus_idd_idf_utilities-0.87/README.md` & `energyplus_idd_idf_utilities-0.88/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_idd_idf_utilities-0.87/energyplus_idd_idf_utilities.egg-info/PKG-INFO` & `energyplus_idd_idf_utilities-0.88/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
-Name: energyplus-idd-idf-utilities
-Version: 0.87
+Name: energyplus_idd_idf_utilities
+Version: 0.88
 Summary: EnergyPlus idd/idf manipulation in Python.
 Home-page: https://github.com/myoldmopar/py-idd-idf
-Author: Edwin Lee
-Author-email: leeed2001@gmail.com
-License: UnlicensedForNow
+Author: Edwin Lee, for NREL, for the United States Department of Energy
+License: ModifiedBSD
 Description: # EnergyPlus Python IDD/IDF Utilities
         
         Python library of EnergyPlus IDD/IDF manipulation utilities.
         
         ## Documentation
         
         [![Documentation Status](https://readthedocs.org/projects/energyplus-idd-idf/badge/?version=latest)](https://energyplus-idd-idf.readthedocs.io/en/latest/?badge=latest)
@@ -135,15 +134,21 @@
         ## Test Coverage
         
         [![Coverage Status](https://coveralls.io/repos/github/Myoldmopar/py-idd-idf/badge.svg?branch=master)](https://coveralls.io/github/Myoldmopar/py-idd-idf?branch=master)
         
         Coverage of the code from unit testing is reported to Coveralls at https://coveralls.io/github/Myoldmopar/py-idd-idf.
         Anything less than 100% coverage will be frowned upon. :)
         
-Platform: UNKNOWN
+Keywords: energyplus_launch,ep_launch,EnergyPlus,eplus,Energy+,Building Simulation,Whole Building Energy Simulation,Heat Transfer,HVAC,Modeling
+Platform: Linux (Tested on Ubuntu)
+Platform: MacOSX
+Platform: Windows
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Utilities
-Classifier: License :: Public Domain
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `energyplus_idd_idf_utilities-0.87/energyplus_idd_idf_utilities.egg-info/SOURCES.txt` & `energyplus_idd_idf_utilities-0.88/energyplus_idd_idf_utilities.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.cfg
 setup.py
 energyplus_idd_idf_utilities.egg-info/PKG-INFO
 energyplus_idd_idf_utilities.egg-info/SOURCES.txt
 energyplus_idd_idf_utilities.egg-info/dependency_links.txt
 energyplus_idd_idf_utilities.egg-info/entry_points.txt
```

### Comparing `energyplus_idd_idf_utilities-0.87/energyplus_iddidf/cli.py` & `energyplus_idd_idf_utilities-0.88/energyplus_iddidf/cli.py`

 * *Files identical despite different names*

### Comparing `energyplus_idd_idf_utilities-0.87/energyplus_iddidf/exceptions.py` & `energyplus_idd_idf_utilities-0.88/energyplus_iddidf/exceptions.py`

 * *Files identical despite different names*

### Comparing `energyplus_idd_idf_utilities-0.87/energyplus_iddidf/idd_objects.py` & `energyplus_idd_idf_utilities-0.88/energyplus_iddidf/idd_objects.py`

 * *Files identical despite different names*

### Comparing `energyplus_idd_idf_utilities-0.87/energyplus_iddidf/idd_processor.py` & `energyplus_idd_idf_utilities-0.88/energyplus_iddidf/idd_processor.py`

 * *Files identical despite different names*

### Comparing `energyplus_idd_idf_utilities-0.87/energyplus_iddidf/idf_objects.py` & `energyplus_idd_idf_utilities-0.88/energyplus_iddidf/idf_objects.py`

 * *Files identical despite different names*

### Comparing `energyplus_idd_idf_utilities-0.87/energyplus_iddidf/idf_processor.py` & `energyplus_idd_idf_utilities-0.88/energyplus_iddidf/idf_processor.py`

 * *Files identical despite different names*

