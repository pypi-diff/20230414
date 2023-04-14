# Comparing `tmp/smplotlib-0.0.3.tar.gz` & `tmp/smplotlib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiaxuanli/Dropbox (Princeton)/Research/Packages/smplotlib/dist/.tmp-_2ix_lfm/smplotlib-0.0.3.tar", last modified: Fri Apr 14 03:01:24 2023, max compression
+gzip compressed data, was "/Users/jiaxuanli/Dropbox (Princeton)/Research/Packages/smplotlib/dist/.tmp-4oh_qll9/smplotlib-0.0.4.tar", last modified: Fri Apr 14 03:04:36 2023, max compression
```

## Comparing `smplotlib-0.0.3.tar` & `smplotlib-0.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:01:24.000000 smplotlib-0.0.3/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1067 2023-04-14 01:14:04.000000 smplotlib-0.0.3/LICENSE
--rw-r--r--   0 jiaxuanli   (501) staff       (20)       40 2023-04-14 02:56:41.000000 smplotlib-0.0.3/MANIFEST.in
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1965 2023-04-14 03:01:24.000000 smplotlib-0.0.3/PKG-INFO
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1439 2023-04-14 02:47:08.000000 smplotlib-0.0.3/README.md
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     2024 2023-04-14 02:12:53.000000 smplotlib-0.0.3/demo.py
--rw-r--r--   0 jiaxuanli   (501) staff       (20)      652 2023-04-14 03:00:59.000000 smplotlib-0.0.3/pyproject.toml
--rw-r--r--   0 jiaxuanli   (501) staff       (20)       38 2023-04-14 03:01:24.000000 smplotlib-0.0.3/setup.cfg
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:01:23.000000 smplotlib-0.0.3/src/
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:01:23.000000 smplotlib-0.0.3/src/smplotlib/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     3192 2023-04-14 02:45:26.000000 smplotlib-0.0.3/src/smplotlib/__init__.py
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    40706 2023-04-14 02:45:38.000000 smplotlib-0.0.3/src/smplotlib/smplot.mplstyle
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:01:23.000000 smplotlib-0.0.3/src/smplotlib.egg-info/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1965 2023-04-14 03:01:23.000000 smplotlib-0.0.3/src/smplotlib.egg-info/PKG-INFO
--rw-r--r--   0 jiaxuanli   (501) staff       (20)      965 2023-04-14 03:01:23.000000 smplotlib-0.0.3/src/smplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 jiaxuanli   (501) staff       (20)        1 2023-04-14 03:01:23.000000 smplotlib-0.0.3/src/smplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 jiaxuanli   (501) staff       (20)       24 2023-04-14 03:01:23.000000 smplotlib-0.0.3/src/smplotlib.egg-info/top_level.txt
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:01:23.000000 smplotlib-0.0.3/src/test_data/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    16128 2023-04-14 01:21:30.000000 smplotlib-0.0.3/src/test_data/test_array.npy
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:01:24.000000 smplotlib-0.0.3/src/ttf/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    70276 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyComplexHeavy.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    68936 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyComplexHeavyItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    88976 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyComplexLight.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    79800 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyComplexLightItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)   131412 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyComplexMedium.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)   122572 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyComplexMediumItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    24356 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyDuplexHeavy.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    22544 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyDuplexHeavyItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    44468 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyDuplexLight.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    39724 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyDuplexLightItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    25640 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyDuplexMedium.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    23516 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheyDuplexMediumItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    28444 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheySimplexHeavy.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    25056 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheySimplexHeavyItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    60092 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheySimplexLight.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    52776 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheySimplexLightItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    28256 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheySimplexMedium.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    25140 2023-04-14 01:19:42.000000 smplotlib-0.0.3/src/ttf/AVHersheySimplexMediumItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    45260 2023-04-14 02:12:59.000000 smplotlib-0.0.3/two_phase.png
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:04:36.000000 smplotlib-0.0.4/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     1067 2023-04-14 01:14:04.000000 smplotlib-0.0.4/LICENSE
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)       40 2023-04-14 02:56:41.000000 smplotlib-0.0.4/MANIFEST.in
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     1965 2023-04-14 03:04:36.000000 smplotlib-0.0.4/PKG-INFO
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     1439 2023-04-14 02:47:08.000000 smplotlib-0.0.4/README.md
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     2018 2023-04-14 03:04:00.000000 smplotlib-0.0.4/demo.py
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)      652 2023-04-14 03:04:08.000000 smplotlib-0.0.4/pyproject.toml
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)       38 2023-04-14 03:04:36.000000 smplotlib-0.0.4/setup.cfg
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:04:36.000000 smplotlib-0.0.4/src/
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:04:36.000000 smplotlib-0.0.4/src/smplotlib/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     3192 2023-04-14 02:45:26.000000 smplotlib-0.0.4/src/smplotlib/__init__.py
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    40706 2023-04-14 02:45:38.000000 smplotlib-0.0.4/src/smplotlib/smplot.mplstyle
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:04:36.000000 smplotlib-0.0.4/src/smplotlib.egg-info/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     1965 2023-04-14 03:04:36.000000 smplotlib-0.0.4/src/smplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)      965 2023-04-14 03:04:36.000000 smplotlib-0.0.4/src/smplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)        1 2023-04-14 03:04:36.000000 smplotlib-0.0.4/src/smplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)       24 2023-04-14 03:04:36.000000 smplotlib-0.0.4/src/smplotlib.egg-info/top_level.txt
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:04:36.000000 smplotlib-0.0.4/src/test_data/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    16128 2023-04-14 01:21:30.000000 smplotlib-0.0.4/src/test_data/test_array.npy
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-14 03:04:36.000000 smplotlib-0.0.4/src/ttf/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    70276 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyComplexHeavy.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    68936 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyComplexHeavyItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    88976 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyComplexLight.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    79800 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyComplexLightItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)   131412 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyComplexMedium.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)   122572 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyComplexMediumItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    24356 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyDuplexHeavy.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    22544 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyDuplexHeavyItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    44468 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyDuplexLight.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    39724 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyDuplexLightItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    25640 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyDuplexMedium.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    23516 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheyDuplexMediumItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    28444 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheySimplexHeavy.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    25056 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheySimplexHeavyItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    60092 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheySimplexLight.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    52776 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheySimplexLightItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    28256 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheySimplexMedium.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    25140 2023-04-14 01:19:42.000000 smplotlib-0.0.4/src/ttf/AVHersheySimplexMediumItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    45260 2023-04-14 02:12:59.000000 smplotlib-0.0.4/two_phase.png
```

### Comparing `smplotlib-0.0.3/LICENSE` & `smplotlib-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/PKG-INFO` & `smplotlib-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smplotlib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Matplotlib template for SuperMongo style
 Author-email: Jiaxuan Li <jiaxuanl@princeton.edu>
 Project-URL: Homepage, https://github.com/AstroJacobLi/smplotlib
 Project-URL: Bug Tracker, https://github.com/AstroJacobLi/smplotlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smplotlib-0.0.3/README.md` & `smplotlib-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/demo.py` & `smplotlib-0.0.4/demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import smplotlib
 
-data = np.load('./smplotlib/test_data/test_array.npy')
+data = np.load('./src/test_data/test_array.npy')
 Pr = data[0]
 Teqs = data[1]
 
 fig, ax = plt.subplots(figsize=(5.5, 5.5))
 
 plt.plot(Pr[(Teqs > 5e3)], Teqs[(Teqs > 5e3)], c='k', lw=1, ls='-')
 plt.plot(Pr[(Teqs < 1.8e2)], Teqs[(Teqs < 1.8e2)], c='k', lw=1, ls='-')
```

### Comparing `smplotlib-0.0.3/src/smplotlib/__init__.py` & `smplotlib-0.0.4/src/smplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/smplotlib/smplot.mplstyle` & `smplotlib-0.0.4/src/smplotlib/smplot.mplstyle`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/smplotlib.egg-info/PKG-INFO` & `smplotlib-0.0.4/src/smplotlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smplotlib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Matplotlib template for SuperMongo style
 Author-email: Jiaxuan Li <jiaxuanl@princeton.edu>
 Project-URL: Homepage, https://github.com/AstroJacobLi/smplotlib
 Project-URL: Bug Tracker, https://github.com/AstroJacobLi/smplotlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smplotlib-0.0.3/src/smplotlib.egg-info/SOURCES.txt` & `smplotlib-0.0.4/src/smplotlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/test_data/test_array.npy` & `smplotlib-0.0.4/src/test_data/test_array.npy`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyComplexHeavy.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyComplexHeavy.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyComplexHeavyItalic.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyComplexHeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyComplexLight.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyComplexLight.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyComplexLightItalic.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyComplexLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyComplexMedium.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyComplexMedium.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyComplexMediumItalic.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyComplexMediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyDuplexHeavy.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyDuplexHeavy.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyDuplexHeavyItalic.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyDuplexHeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyDuplexLight.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyDuplexLight.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyDuplexLightItalic.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyDuplexLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyDuplexMedium.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyDuplexMedium.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheyDuplexMediumItalic.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheyDuplexMediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheySimplexHeavy.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheySimplexHeavy.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheySimplexHeavyItalic.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheySimplexHeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheySimplexLight.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheySimplexLight.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheySimplexLightItalic.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheySimplexLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheySimplexMedium.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheySimplexMedium.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/src/ttf/AVHersheySimplexMediumItalic.ttf` & `smplotlib-0.0.4/src/ttf/AVHersheySimplexMediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.3/two_phase.png` & `smplotlib-0.0.4/two_phase.png`

 * *Files identical despite different names*

