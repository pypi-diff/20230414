# Comparing `tmp/pycoare-2023.4a2.tar.gz` & `tmp/pycoare-2023.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycoare-2023.4a2.tar", last modified: Wed Apr 12 23:25:49 2023, max compression
+gzip compressed data, was "pycoare-2023.4a3.tar", last modified: Fri Apr 14 05:40:25 2023, max compression
```

## Comparing `pycoare-2023.4a2.tar` & `pycoare-2023.4a3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:25:49.508627 pycoare-2023.4a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-12 23:25:39.000000 pycoare-2023.4a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-12 23:25:49.508627 pycoare-2023.4a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-04-12 23:25:39.000000 pycoare-2023.4a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:25:49.508627 pycoare-2023.4a2/pycoare/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 23:25:39.000000 pycoare-2023.4a2/pycoare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-04-12 23:25:39.000000 pycoare-2023.4a2/pycoare/coare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:25:49.508627 pycoare-2023.4a2/pycoare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-12 23:25:49.000000 pycoare-2023.4a2/pycoare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 23:25:49.000000 pycoare-2023.4a2/pycoare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:25:49.000000 pycoare-2023.4a2/pycoare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 23:25:49.000000 pycoare-2023.4a2/pycoare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 23:25:49.000000 pycoare-2023.4a2/pycoare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 23:25:39.000000 pycoare-2023.4a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 23:25:49.512627 pycoare-2023.4a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:25:49.508627 pycoare-2023.4a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-12 23:25:39.000000 pycoare-2023.4a2/tests/test_coare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:40:25.468278 pycoare-2023.4a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-14 05:40:12.000000 pycoare-2023.4a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-04-14 05:40:25.468278 pycoare-2023.4a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-14 05:40:12.000000 pycoare-2023.4a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:40:25.464278 pycoare-2023.4a3/pycoare/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 05:40:12.000000 pycoare-2023.4a3/pycoare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-04-14 05:40:12.000000 pycoare-2023.4a3/pycoare/coare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:40:25.468278 pycoare-2023.4a3/pycoare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-04-14 05:40:25.000000 pycoare-2023.4a3/pycoare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 05:40:25.000000 pycoare-2023.4a3/pycoare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:40:25.000000 pycoare-2023.4a3/pycoare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 05:40:25.000000 pycoare-2023.4a3/pycoare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 05:40:25.000000 pycoare-2023.4a3/pycoare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-14 05:40:12.000000 pycoare-2023.4a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 05:40:25.468278 pycoare-2023.4a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:40:25.468278 pycoare-2023.4a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-14 05:40:12.000000 pycoare-2023.4a3/tests/test_coare.py
```

### Comparing `pycoare-2023.4a2/LICENSE` & `pycoare-2023.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycoare-2023.4a2/PKG-INFO` & `pycoare-2023.4a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pycoare
-Version: 2023.4a2
+Version: 2023.4a3
 Summary: A Python implementation of the COARE bulk air-sea flux algorithm.
 Author: C. W. Fairall, Byron Blomquist, Ludovic Bariteau, J. B. Edson
 Maintainer-email: Andrew Scherer <scherand@oregonstate.edu>
 License: MIT License
+Project-URL: Source, https://github.com/andrew-s28/COARE-algorithm
 Keywords: oceanography,air-sea,bulk flux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyCOARE
 [![CI](https://github.com/andrew-s28/COARE-algorithm/workflows/tests/badge.svg?branch=master)](https://github.com/andrew-s28/COARE-algorithm/actions)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](ttps://github.com/andrew-s28/COARE-algorithm/blob/master/LICENSE.txt)
 [![Code coverage](https://codecov.io/gh/andrew-s28/COARE-algorithm/branch/master/graph/badge.svg)](https://app.codecov.io/gh/andrew-s28/COARE-algorithm)
-[![Available on pypi](https://badge.fury.io/py/pycoare.svg)](https://pypi.python.org/pypi/pycoare/)
+[![Available on pypi](https://badge.fury.io/py/pycoare.svg)](https://badge.fury.io/py/pycoare)
 
 ## COARE-algorithm
 
 This is an alpha-quality fork of the Python version of the [COARE algorithm](https://github.com/NOAA-PSL/COARE-algorithm) that was written with the goal of standardizing testing, packaging, and distribution of the algorithm. Currently only COARE v3.5 is implemented - hopefully v3.6 will come soon! 
 
 The functionality of the code is ideally the same as that for the scripts found in the NOAA PSL repository linked above. My only intended contributions are towards formatting, testing, and packaging. To that end, tests have been constructed based on the output of the original MATLAB code for COARE v3.5. [View the results of the tests](https://github.com/andrew-s28/COARE-algorithm/actions) or [download the data](https://github.com/andrew-s28/COARE-algorithm/tree/master/tests/data) and run them yourself. All results from this script agree to at least five significant figures with the MATLAB scripts in the NOAA repository, provided the testing badge above stays green.
```

### Comparing `pycoare-2023.4a2/README.md` & `pycoare-2023.4a3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyCOARE
 [![CI](https://github.com/andrew-s28/COARE-algorithm/workflows/tests/badge.svg?branch=master)](https://github.com/andrew-s28/COARE-algorithm/actions)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](ttps://github.com/andrew-s28/COARE-algorithm/blob/master/LICENSE.txt)
 [![Code coverage](https://codecov.io/gh/andrew-s28/COARE-algorithm/branch/master/graph/badge.svg)](https://app.codecov.io/gh/andrew-s28/COARE-algorithm)
-[![Available on pypi](https://badge.fury.io/py/pycoare.svg)](https://pypi.python.org/pypi/pycoare/)
+[![Available on pypi](https://badge.fury.io/py/pycoare.svg)](https://badge.fury.io/py/pycoare)
 
 ## COARE-algorithm
 
 This is an alpha-quality fork of the Python version of the [COARE algorithm](https://github.com/NOAA-PSL/COARE-algorithm) that was written with the goal of standardizing testing, packaging, and distribution of the algorithm. Currently only COARE v3.5 is implemented - hopefully v3.6 will come soon! 
 
 The functionality of the code is ideally the same as that for the scripts found in the NOAA PSL repository linked above. My only intended contributions are towards formatting, testing, and packaging. To that end, tests have been constructed based on the output of the original MATLAB code for COARE v3.5. [View the results of the tests](https://github.com/andrew-s28/COARE-algorithm/actions) or [download the data](https://github.com/andrew-s28/COARE-algorithm/tree/master/tests/data) and run them yourself. All results from this script agree to at least five significant figures with the MATLAB scripts in the NOAA repository, provided the testing badge above stays green.
```

### Comparing `pycoare-2023.4a2/pycoare/coare.py` & `pycoare-2023.4a3/pycoare/coare.py`

 * *Files identical despite different names*

### Comparing `pycoare-2023.4a2/pycoare.egg-info/PKG-INFO` & `pycoare-2023.4a3/pycoare.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pycoare
-Version: 2023.4a2
+Version: 2023.4a3
 Summary: A Python implementation of the COARE bulk air-sea flux algorithm.
 Author: C. W. Fairall, Byron Blomquist, Ludovic Bariteau, J. B. Edson
 Maintainer-email: Andrew Scherer <scherand@oregonstate.edu>
 License: MIT License
+Project-URL: Source, https://github.com/andrew-s28/COARE-algorithm
 Keywords: oceanography,air-sea,bulk flux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyCOARE
 [![CI](https://github.com/andrew-s28/COARE-algorithm/workflows/tests/badge.svg?branch=master)](https://github.com/andrew-s28/COARE-algorithm/actions)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](ttps://github.com/andrew-s28/COARE-algorithm/blob/master/LICENSE.txt)
 [![Code coverage](https://codecov.io/gh/andrew-s28/COARE-algorithm/branch/master/graph/badge.svg)](https://app.codecov.io/gh/andrew-s28/COARE-algorithm)
-[![Available on pypi](https://badge.fury.io/py/pycoare.svg)](https://pypi.python.org/pypi/pycoare/)
+[![Available on pypi](https://badge.fury.io/py/pycoare.svg)](https://badge.fury.io/py/pycoare)
 
 ## COARE-algorithm
 
 This is an alpha-quality fork of the Python version of the [COARE algorithm](https://github.com/NOAA-PSL/COARE-algorithm) that was written with the goal of standardizing testing, packaging, and distribution of the algorithm. Currently only COARE v3.5 is implemented - hopefully v3.6 will come soon! 
 
 The functionality of the code is ideally the same as that for the scripts found in the NOAA PSL repository linked above. My only intended contributions are towards formatting, testing, and packaging. To that end, tests have been constructed based on the output of the original MATLAB code for COARE v3.5. [View the results of the tests](https://github.com/andrew-s28/COARE-algorithm/actions) or [download the data](https://github.com/andrew-s28/COARE-algorithm/tree/master/tests/data) and run them yourself. All results from this script agree to at least five significant figures with the MATLAB scripts in the NOAA repository, provided the testing badge above stays green.
```

### Comparing `pycoare-2023.4a2/pyproject.toml` & `pycoare-2023.4a3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     {name = 'Byron Blomquist'},
     {name = 'Ludovic Bariteau'},
     {name = 'J. B. Edson'}
 ]
 maintainers = [
     {name = 'Andrew Scherer', email = 'scherand@oregonstate.edu'}
 ]
-version = "2023.4a2"
+version = "2023.4a3"
 description = 'A Python implementation of the COARE bulk air-sea flux algorithm.'
 readme = {file = 'README.md', content-type = 'text/markdown'}
 requires-python = ">=3.7"
 keywords = ['oceanography', 'air-sea', 'bulk flux']
 license = {text = "MIT License"}
 classifiers = [
     'Development Status :: 3 - Alpha',
@@ -25,9 +25,13 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Topic :: Scientific/Engineering',
     'Intended Audience :: Science/Research'
 ]
 dependencies = ['numpy']
 
+[project.urls]
+
+Source = 'https://github.com/andrew-s28/COARE-algorithm'
+
```

### Comparing `pycoare-2023.4a2/tests/test_coare.py` & `pycoare-2023.4a3/tests/test_coare.py`

 * *Files identical despite different names*

