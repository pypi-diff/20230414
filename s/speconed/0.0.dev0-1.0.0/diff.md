# Comparing `tmp/speconed-0.0.dev0.tar.gz` & `tmp/speconed-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speconed-0.0.dev0.tar", last modified: Fri Apr 14 06:02:53 2023, max compression
+gzip compressed data, was "speconed-1.0.0.tar", last modified: Fri Apr 14 07:56:47 2023, max compression
```

## Comparing `speconed-0.0.dev0.tar` & `speconed-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 06:02:53.479655 speconed-0.0.dev0/
--rw-r--r--   0 jtschindler   (501) staff       (20)     1499 2023-04-14 05:00:23.000000 speconed-0.0.dev0/LICENSE
--rw-r--r--   0 jtschindler   (501) staff       (20)     2419 2023-04-14 06:02:53.479716 speconed-0.0.dev0/PKG-INFO
--rw-r--r--   0 jtschindler   (501) staff       (20)       81 2023-04-14 05:00:23.000000 speconed-0.0.dev0/README.md
--rw-r--r--   0 jtschindler   (501) staff       (20)       86 2023-04-14 06:00:57.000000 speconed-0.0.dev0/pyproject.toml
--rw-r--r--   0 jtschindler   (501) staff       (20)     1091 2023-04-14 06:02:53.480002 speconed-0.0.dev0/setup.cfg
--rw-r--r--   0 jtschindler   (501) staff       (20)      125 2023-03-06 14:40:10.000000 speconed-0.0.dev0/setup.py
-drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 06:02:53.478352 speconed-0.0.dev0/speconed/
--rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 05:06:10.000000 speconed-0.0.dev0/speconed/__init__.py
--rw-r--r--   0 jtschindler   (501) staff       (20)   129325 2023-04-14 05:29:54.000000 speconed-0.0.dev0/speconed/speconed.py
-drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 06:02:53.479566 speconed-0.0.dev0/speconed.egg-info/
--rw-r--r--   0 jtschindler   (501) staff       (20)     2419 2023-04-14 06:02:53.000000 speconed-0.0.dev0/speconed.egg-info/PKG-INFO
--rw-r--r--   0 jtschindler   (501) staff       (20)      252 2023-04-14 06:02:53.000000 speconed-0.0.dev0/speconed.egg-info/SOURCES.txt
--rw-r--r--   0 jtschindler   (501) staff       (20)        1 2023-04-14 06:02:53.000000 speconed-0.0.dev0/speconed.egg-info/dependency_links.txt
--rw-r--r--   0 jtschindler   (501) staff       (20)      100 2023-04-14 06:02:53.000000 speconed-0.0.dev0/speconed.egg-info/requires.txt
--rw-r--r--   0 jtschindler   (501) staff       (20)        9 2023-04-14 06:02:53.000000 speconed-0.0.dev0/speconed.egg-info/top_level.txt
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 07:56:47.878183 speconed-1.0.0/
+-rw-r--r--   0 jtschindler   (501) staff       (20)     1499 2023-04-14 05:00:23.000000 speconed-1.0.0/LICENSE
+-rw-r--r--   0 jtschindler   (501) staff       (20)     2807 2023-04-14 07:56:47.878256 speconed-1.0.0/PKG-INFO
+-rw-r--r--   0 jtschindler   (501) staff       (20)      472 2023-04-14 07:46:28.000000 speconed-1.0.0/README.md
+-rw-r--r--   0 jtschindler   (501) staff       (20)       86 2023-04-14 06:00:57.000000 speconed-1.0.0/pyproject.toml
+-rw-r--r--   0 jtschindler   (501) staff       (20)     1110 2023-04-14 07:56:47.878570 speconed-1.0.0/setup.cfg
+-rw-r--r--   0 jtschindler   (501) staff       (20)      125 2023-03-06 14:40:10.000000 speconed-1.0.0/setup.py
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 07:56:47.877220 speconed-1.0.0/speconed/
+-rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 05:06:10.000000 speconed-1.0.0/speconed/__init__.py
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 07:56:47.877995 speconed-1.0.0/speconed/data/
+-rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 06:33:26.000000 speconed-1.0.0/speconed/data/__init__.py
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 07:56:47.878098 speconed-1.0.0/speconed/data/passbands/
+-rw-r--r--   0 jtschindler   (501) staff       (20)        0 2023-04-14 06:33:40.000000 speconed-1.0.0/speconed/data/passbands/__init__.py
+-rw-r--r--   0 jtschindler   (501) staff       (20)   129538 2023-04-14 06:25:17.000000 speconed-1.0.0/speconed/speconed.py
+drwxr-xr-x   0 jtschindler   (501) staff       (20)        0 2023-04-14 07:56:47.877883 speconed-1.0.0/speconed.egg-info/
+-rw-r--r--   0 jtschindler   (501) staff       (20)     2807 2023-04-14 07:56:47.000000 speconed-1.0.0/speconed.egg-info/PKG-INFO
+-rw-r--r--   0 jtschindler   (501) staff       (20)      314 2023-04-14 07:56:47.000000 speconed-1.0.0/speconed.egg-info/SOURCES.txt
+-rw-r--r--   0 jtschindler   (501) staff       (20)        1 2023-04-14 07:56:47.000000 speconed-1.0.0/speconed.egg-info/dependency_links.txt
+-rw-r--r--   0 jtschindler   (501) staff       (20)      119 2023-04-14 07:56:47.000000 speconed-1.0.0/speconed.egg-info/requires.txt
+-rw-r--r--   0 jtschindler   (501) staff       (20)        9 2023-04-14 07:56:47.000000 speconed-1.0.0/speconed.egg-info/top_level.txt
```

### Comparing `speconed-0.0.dev0/LICENSE` & `speconed-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `speconed-0.0.dev0/PKG-INFO` & `speconed-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speconed
-Version: 0.0.dev0
+Version: 1.0.0
 Summary: A lightweight package for the manipulation of 1-D astronomical specta
 Home-page: https://github.com/jtschindler/speconed
 Author: Jan-Torge Schindler
 Author-email: schindler@strw.leidenuniv.nl
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jtschindler/speconed/issues
 Keywords: spectroscopy,astronomy,science,python
@@ -15,17 +15,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# speconed
-A lightweight package for the manipulation of 1-D astronomical specta
+# SpecOneD
+##### (Version 1.0.0)
 
+[![Documentation Status](https://readthedocs.org/projects/speconed/badge/?version=latest)](https://speconed.readthedocs.io/en/latest/?badge=latest)
+
+SpecOneD is a lightweight python package that introduces the SpecOneD class for the manipulation of one-dimensional astronomical spectra.
+
+For installation instructions and documentation visit [SpecOneD's ReadTheDocs]
+
+
+
+[SpecOneD's ReadTheDocs]: https://speconed.readthedocs.io/en/latest/
 BSD 3-Clause License
 
 Copyright (c) 2023, JT Schindler
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
```

### Comparing `speconed-0.0.dev0/setup.cfg` & `speconed-1.0.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = speconed
-version = 0.0dev0
+version = 1.0.0
 author = Jan-Torge Schindler
 author_email = schindler@strw.leidenuniv.nl
 description = A lightweight package for the manipulation of 1-D astronomical specta
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/jtschindler/speconed
 project_urls = 
@@ -29,20 +29,22 @@
 python_requires = >=3.9
 install_requires = 
 	numpy
 	scipy
 	pandas
 	h5py
 	extinction
-	pgk_resources
 	spectres
 	astropy
 	matplotlib
+	tables
+	notebook
 	nbsphinx
 	nbsphinx-link
+	sphinx-rtd-theme
 requirement_files = 
 	requirements.txt
 
 [options.packages.find]
 exclude = 
 	examples
```

### Comparing `speconed-0.0.dev0/speconed/speconed.py` & `speconed-1.0.0/speconed/speconed.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import numpy as np
 import scipy as sp
 import pandas as pd
 
 import h5py
 import extinction as ext
-import pkg_resources
+import importlib.resources
 import spectres
 
 from astropy.io import fits
 from astropy import constants as const
 from astropy import units as u
 from astropy.convolution import convolve, Gaussian1DKernel, Box1DKernel
 
@@ -2251,19 +2251,24 @@
         passband files contain a large range of 0 values below and above the \
         passband. The default value for the tolerance is 0.005, i.e. 0.5% \
         throughput.
         :type tolerance: float
         :return:
         """
 
-        passband_filename = \
-            pkg_resources.resource_filename('sculptor',
-                                    'data/passbands/{}.dat'.format(
-                                        passband_name))
-        passband_data = np.genfromtxt(passband_filename)
+        # passband_filename = \
+        #     pkg_resources.resource_filename('sculptor',
+        #                             'data/passbands/{}.dat'.format(
+        #                                 passband_name))
+        #
+        ref = importlib.resources.files('speconed') / \
+              'data/passbands/{}.dat'.format(passband_name)
+
+        with importlib.resources.as_file(ref) as passband_filename:
+            passband_data = np.genfromtxt(passband_filename)
 
         wavelength = passband_data[:, 0]
         throughput = passband_data[:, 1]
 
         # Change wavelength to Angstroem for all passbands
         filter_group = passband_name.split('-')[0]
```

### Comparing `speconed-0.0.dev0/speconed.egg-info/PKG-INFO` & `speconed-1.0.0/speconed.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speconed
-Version: 0.0.dev0
+Version: 1.0.0
 Summary: A lightweight package for the manipulation of 1-D astronomical specta
 Home-page: https://github.com/jtschindler/speconed
 Author: Jan-Torge Schindler
 Author-email: schindler@strw.leidenuniv.nl
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jtschindler/speconed/issues
 Keywords: spectroscopy,astronomy,science,python
@@ -15,17 +15,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# speconed
-A lightweight package for the manipulation of 1-D astronomical specta
+# SpecOneD
+##### (Version 1.0.0)
 
+[![Documentation Status](https://readthedocs.org/projects/speconed/badge/?version=latest)](https://speconed.readthedocs.io/en/latest/?badge=latest)
+
+SpecOneD is a lightweight python package that introduces the SpecOneD class for the manipulation of one-dimensional astronomical spectra.
+
+For installation instructions and documentation visit [SpecOneD's ReadTheDocs]
+
+
+
+[SpecOneD's ReadTheDocs]: https://speconed.readthedocs.io/en/latest/
 BSD 3-Clause License
 
 Copyright (c) 2023, JT Schindler
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
```

