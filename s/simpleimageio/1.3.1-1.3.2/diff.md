# Comparing `tmp/simpleimageio-1.3.1.tar.gz` & `tmp/simpleimageio-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleimageio-1.3.1.tar", last modified: Wed Apr 12 18:32:52 2023, max compression
+gzip compressed data, was "simpleimageio-1.3.2.tar", last modified: Fri Apr 14 12:04:17 2023, max compression
```

## Comparing `simpleimageio-1.3.1.tar` & `simpleimageio-1.3.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.480255 simpleimageio-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.476256 simpleimageio-1.3.1/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.476256 simpleimageio-1.3.1/Core/External/
--rw-r--r--   0 runner    (1001) docker     (123)   114725 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/fpng.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/fpng.h
--rw-r--r--   0 runner    (1001) docker     (123)   319839 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/miniz.c
--rw-r--r--   0 runner    (1001) docker     (123)    69441 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/miniz.h
--rw-r--r--   0 runner    (1001) docker     (123)   273149 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/stb_image.h
--rw-r--r--   0 runner    (1001) docker     (123)    69564 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/stb_image_write.h
--rw-r--r--   0 runner    (1001) docker     (123)   163059 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/tiny_dng_loader.h
--rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/tiny_dng_writer.h
--rw-r--r--   0 runner    (1001) docker     (123)   269883 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/External/tinyexr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/error_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/filter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/image.h
--rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/imageio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/manipulation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/tonemapping.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/Core/vec3.h
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 18:32:49.000000 simpleimageio-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-12 18:32:52.480255 simpleimageio-1.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.476256 simpleimageio-1.3.1/PyWrapper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.480255 simpleimageio-1.3.1/PyWrapper/simpleimageio/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/corelib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/error_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    35670 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/imageViewer.js
--rw-r--r--   0 runner    (1001) docker     (123)    89794 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/jquery-3.6.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/manip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/tev.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/PyWrapper/simpleimageio/tonemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:32:52.480255 simpleimageio-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-12 18:32:50.000000 simpleimageio-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:32:52.480255 simpleimageio-1.3.1/simpleimageio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-12 18:32:52.000000 simpleimageio-1.3.1/simpleimageio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 18:32:52.000000 simpleimageio-1.3.1/simpleimageio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:32:52.000000 simpleimageio-1.3.1/simpleimageio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 18:32:52.000000 simpleimageio-1.3.1/simpleimageio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 18:32:52.000000 simpleimageio-1.3.1/simpleimageio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.105553 simpleimageio-1.3.2/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/Core/External/
+-rw-r--r--   0 runner    (1001) docker     (123)   114725 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/fpng.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/fpng.h
+-rw-r--r--   0 runner    (1001) docker     (123)   319839 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/miniz.c
+-rw-r--r--   0 runner    (1001) docker     (123)    69441 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/miniz.h
+-rw-r--r--   0 runner    (1001) docker     (123)   273149 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/stb_image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69564 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/stb_image_write.h
+-rw-r--r--   0 runner    (1001) docker     (123)   163059 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/tiny_dng_loader.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/tiny_dng_writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)   269883 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/External/tinyexr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/error_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/imageio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/manipulation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/tonemapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/Core/vec3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.101553 simpleimageio-1.3.2/PyWrapper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/PyWrapper/simpleimageio/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/corelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/error_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37535 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/imageViewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89794 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/jquery-3.6.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/manip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/tev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/PyWrapper/simpleimageio/tonemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-14 12:04:11.000000 simpleimageio-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:17.109553 simpleimageio-1.3.2/simpleimageio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-14 12:04:17.000000 simpleimageio-1.3.2/simpleimageio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-14 12:04:17.000000 simpleimageio-1.3.2/simpleimageio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:04:17.000000 simpleimageio-1.3.2/simpleimageio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 12:04:17.000000 simpleimageio-1.3.2/simpleimageio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-14 12:04:17.000000 simpleimageio-1.3.2/simpleimageio.egg-info/top_level.txt
```

### Comparing `simpleimageio-1.3.1/Core/CMakeLists.txt` & `simpleimageio-1.3.2/Core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/External/fpng.cpp` & `simpleimageio-1.3.2/Core/External/fpng.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/External/fpng.h` & `simpleimageio-1.3.2/Core/External/fpng.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/External/miniz.c` & `simpleimageio-1.3.2/Core/External/miniz.c`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/External/miniz.h` & `simpleimageio-1.3.2/Core/External/miniz.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/External/stb_image.h` & `simpleimageio-1.3.2/Core/External/stb_image.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/External/stb_image_write.h` & `simpleimageio-1.3.2/Core/External/stb_image_write.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/External/tiny_dng_loader.h` & `simpleimageio-1.3.2/Core/External/tiny_dng_loader.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/External/tiny_dng_writer.h` & `simpleimageio-1.3.2/Core/External/tiny_dng_writer.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/External/tinyexr.h` & `simpleimageio-1.3.2/Core/External/tinyexr.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/error_metrics.cpp` & `simpleimageio-1.3.2/Core/error_metrics.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/filter.cpp` & `simpleimageio-1.3.2/Core/filter.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/image.h` & `simpleimageio-1.3.2/Core/image.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/imageio.cpp` & `simpleimageio-1.3.2/Core/imageio.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/manipulation.cpp` & `simpleimageio-1.3.2/Core/manipulation.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/tonemapping.cpp` & `simpleimageio-1.3.2/Core/tonemapping.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/Core/vec3.h` & `simpleimageio-1.3.2/Core/vec3.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/LICENSE` & `simpleimageio-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/PKG-INFO` & `simpleimageio-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleimageio
-Version: 1.3.1
+Version: 1.3.2
 Summary: A very simple Python wrapper to read and write various HDR and LDR image file formats.
 Home-page: https://github.com/pgrit/SimpleImageIO
 Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.1 Summary: A very simple
+Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.2 Summary: A very simple
 Python wrapper to read and write various HDR and LDR image file formats. Home-
 page: https://github.com/pgrit/SimpleImageIO Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE ![Build](https://github.com/pgrit/SimpleImageIO/workflows/Build/
 badge.svg) [https://buildstats.info/nuget/SimpleImageIO] # Simple Image IO A
```

### Comparing `simpleimageio-1.3.1/PyWrapper/simpleimageio/corelib.py` & `simpleimageio-1.3.2/PyWrapper/simpleimageio/corelib.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/PyWrapper/simpleimageio/error_metrics.py` & `simpleimageio-1.3.2/PyWrapper/simpleimageio/error_metrics.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/PyWrapper/simpleimageio/flip.py` & `simpleimageio-1.3.2/PyWrapper/simpleimageio/flip.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/PyWrapper/simpleimageio/image.py` & `simpleimageio-1.3.2/PyWrapper/simpleimageio/image.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/PyWrapper/simpleimageio/imageViewer.js` & `simpleimageio-1.3.2/PyWrapper/simpleimageio/imageViewer.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,39 @@
-// globals that track the position and zoom operations
+// globals that track states and data of all images and views
 var dragTarget = null;
 var dragXStart = 0;
 var dragYStart = 0;
 var zoomLevels = new Map();
 var positions = new Map();
 var curImageIdx = new Map();
 var magnifierStates = new Map();
+var flipBookImages = new Map();
+
+// Auto-delete the global state if a corresponding HTMLElement was removed from the DOM
+function addRemovalObserver() {
+    new MutationObserver(_ => {
+        flipBookImages.forEach((_1, container, _2) => {
+            if (!document.body.contains(container)) {
+                zoomLevels.delete(container);
+                positions.delete(container);
+                curImageIdx.delete(container);
+                magnifierStates.delete(container);
+                flipBookImages.delete(container);
+            }
+        });
+    }).observe(document.body, {
+        childList: true,
+        subtree: true
+    });
+}
+
+if (document.readyState === "complete")
+    addRemovalObserver();
+else
+    addEventListener("load", (_) => addRemovalObserver());
 
 var wheelOpt = false;
 try {
     window.addEventListener("test", null, Object.defineProperty({}, 'passive', {
         get: function() {
             wheelOpt = {
                 passive: false
@@ -250,15 +274,14 @@
     let table = magnifier.find("table");
     table.children().remove();
 
     let activeImage = flipBookImages.get(container)[curImageIdx.get(container) - 1];
     let size = 2 * MagnifierResolution + 1;
 
     let canvas = activeImage.canvas;
-    let pixels = activeImage.pixels instanceof Float32Array ? activeImage.pixels : null;
     let ctx = canvas.getContext('2d');
     let buffer = ctx.getImageData(state.col - MagnifierResolution, state.row - MagnifierResolution,
         size, size).data;
 
     let bufRow = -1;
     for (let row = state.row - MagnifierResolution; row <= state.row + MagnifierResolution; ++row) {
         bufRow++;
@@ -277,32 +300,47 @@
                 classNames += " selected";
 
             let clrR = buffer[(bufRow * size + bufCol) * 4 + 0];
             let clrG = buffer[(bufRow * size + bufCol) * 4 + 1];
             let clrB = buffer[(bufRow * size + bufCol) * 4 + 2];
 
             let r, g, b;
-            if (pixels === null) {
+            let numChan = 3;
+            if (activeImage.pixels instanceof ImageData) {
+                r = activeImage.pixels.data[4 * (row * canvas.width + col) + 0] / 255;
+                g = activeImage.pixels.data[4 * (row * canvas.width + col) + 1] / 255;
+                b = activeImage.pixels.data[4 * (row * canvas.width + col) + 2] / 255;
+            } else if (activeImage.pixels instanceof Float32Array) {
+                numChan = activeImage.pixels.length / canvas.width / canvas.height;
+                r = activeImage.pixels[numChan * (row * canvas.width + col) + 0 % numChan];
+                g = activeImage.pixels[numChan * (row * canvas.width + col) + 1 % numChan];
+                b = activeImage.pixels[numChan * (row * canvas.width + col) + 2 % numChan];
+            } else {
                 r = clrR / 255;
                 g = clrG / 255;
                 b = clrB / 255;
-            } else {
-                r = activeImage.pixels[3 * (row * canvas.width + col) + 0];
-                g = activeImage.pixels[3 * (row * canvas.width + col) + 1];
-                b = activeImage.pixels[3 * (row * canvas.width + col) + 2];
             }
 
-            tr.append(`
-            <td class='${classNames}'
-                style="background-color: rgb(${clrR}, ${clrG}, ${clrB});">
-                <p class="magnifier" style="color: rgb(255,70,30);">${formatNumber(r)}</p>
-                <p class="magnifier" style="color: rgb(77, 250, 57);">${formatNumber(g)}</p>
-                <p class="magnifier" style="color: rgb(0,180,255);">${formatNumber(b)}</p>
-            </td>
-            `);
+            if (numChan == 3) {
+                tr.append(`
+                <td class='${classNames}'
+                    style="background-color: rgb(${clrR}, ${clrG}, ${clrB});">
+                    <p class="magnifier" style="color: rgb(255,70,30);">${formatNumber(r)}</p>
+                    <p class="magnifier" style="color: rgb(77, 250, 57);">${formatNumber(g)}</p>
+                    <p class="magnifier" style="color: rgb(0,180,255);">${formatNumber(b)}</p>
+                </td>
+                `);
+            } else {
+                tr.append(`
+                <td class='${classNames}'
+                    style="background-color: rgb(${clrR}, ${clrG}, ${clrB});">
+                    <p class="magnifier" style="color: rgb(255,255,255);">${formatNumber(r)}</p>
+                </td>
+                `);
+            }
         }
     }
 }
 
 function showMagnifier(magnifierLeft, magnifierTop, magnifyCol, magnifyRow, container) {
     magnifier = $(container).find("div.magnifier");
     magnifier.addClass("visible");
@@ -325,27 +363,22 @@
         "visible": false
     });
     $(".magnifier").removeClass("visible");
 }
 
 function computeZoomScale(container, evt, left, top) {
     const ScrollSpeed = 0.25;
-    const MaxScale = 1000;
+    const MaxScale = 100;
     const MinScale = 0.05;
 
-    var direction = evt.wheelDeltaY < 0 ? 1 : -1;
-    var factor = 1.0 - direction * ScrollSpeed;
+    const oldScale = zoomLevels.get(container);
+    const scale = oldScale * (1 + Math.sign(evt.wheelDeltaY) * ScrollSpeed);
+    const factor = scale / oldScale;
 
-    var scale = zoomLevels.get(container);
-    if (scale * factor > MaxScale) {
-        return;
-    } else if (scale * factor < MinScale) {
-        return;
-    }
-    scale *= factor;
+    if (scale > MaxScale || scale < MinScale) return;
 
     // Adjust the position of the top left corner, so we get a scale pivot at the mouse cursor.
     var relX = evt.offsetX - left;
     var relY = evt.offsetY - top;
     var deltaX = (1 - factor) * relX;
     var deltaY = (1 - factor) * relY;
 
@@ -390,37 +423,36 @@
     }
     apply(tmo) {
         this.currentTMO = tmo;
         this.dirty = true;
     }
 }
 
-var flipBookImages = new Map();
-
 function makeImages(flipbook, rawPixels, initialTMO) {
     let container = $(flipbook).find(".image-container")[0];
 
     // connect each canvas to its raw data
     let images = []
     for (let i = 0; i < rawPixels.length; ++i) {
         let pixels = rawPixels[i];
-
         let canvas = $(flipbook).find(`.image-${i + 1}`)
 
-        if (canvas.hasClass('ldr')) {
-            images.push(canvas[0])
-        } else {
-            images.push(new HDRImage(pixels, canvas[0], container));
+        // Convert image element to ImageData object so we can access its pixel values directly
+        if (pixels instanceof HTMLImageElement) {
+            const offscreen = new OffscreenCanvas(pixels.naturalWidth, pixels.naturalHeight);
+            const ctx = offscreen.getContext('2d');
+            ctx.drawImage(pixels, 0, 0);
+            pixels = ctx.getImageData(0, 0, pixels.naturalWidth, pixels.naturalHeight);
         }
+
+        images.push(new HDRImage(pixels, canvas[0], container));
     }
 
     function apply(fn) {
-        images.forEach(img => {
-            if (img instanceof HDRImage) img.apply(fn);
-        });
+        images.forEach(img => img.apply(fn));
     }
 
     flipBookImages.set(container, images);
 
     // attach TMO controls for scripting
     let scriptTxt = $(flipbook).find(".tmo-script").find('textarea')[0];
 
@@ -529,14 +561,15 @@
         precision highp float;
 
         in vec2 uv;
         out vec4 FragColor;
 
         uniform sampler2D hdr;
         uniform bool isLdr;
+        uniform bool isMono;
 
         const vec3[] inferno = vec3[](vec3(0.000113157585, 3.6067417E-05, 0.0010732203), vec3(0.00025610387, 0.00017476911, 0.0018801669), vec3(0.0004669041, 0.00036492254, 0.0029950093), vec3(0.00074387394, 0.0006001055, 0.004434588), vec3(0.0010894359, 0.00087344326, 0.006229556), vec3(0.0015088051, 0.001177559, 0.0084160855), vec3(0.0020109902, 0.0015040196, 0.01103472), vec3(0.0026039002, 0.0018438299, 0.0141367605), vec3(0.0033011902, 0.0021884087, 0.017756652), vec3(0.004120199, 0.0025247426, 0.021956626), vec3(0.0050788447, 0.002843587, 0.026762031), vec3(0.006197755, 0.0031312993, 0.032229163), vec3(0.0075137066, 0.0033734855, 0.038373485), vec3(0.009052796, 0.0035592811, 0.045200158), vec3(0.010849649, 0.0036771009, 0.0526849), vec3(0.012937295, 0.0037212505, 0.060759768), vec3(0.015345546, 0.003692564, 0.06930094), vec3(0.018098025, 0.0035980744, 0.07813061), vec3(0.021208616, 0.0034528747, 0.08703171), vec3(0.024674637, 0.003281221, 0.09575732), vec3(0.028485317, 0.0031094865, 0.1040848), vec3(0.032620963, 0.0029626512, 0.11183704), vec3(0.03706181, 0.0028607259, 0.118899666), vec3(0.04178865, 0.0028177549, 0.12522277), vec3(0.046788756, 0.0028406673, 0.13080563), vec3(0.052054882, 0.0029312726, 0.13568167), vec3(0.057582982, 0.003088596, 0.13990062), vec3(0.063372016, 0.0033096694, 0.1435242), vec3(0.06942662, 0.0035893016, 0.14660975), vec3(0.07575159, 0.003922615, 0.14921187), vec3(0.08235316, 0.0043047923, 0.15138116), vec3(0.08923761, 0.0047312886, 0.15316024), vec3(0.09641238, 0.005197805, 0.15458518), vec3(0.10388431, 0.0057007573, 0.15568596), vec3(0.111662984, 0.006236934, 0.1564891), vec3(0.119754754, 0.006803522, 0.157015), vec3(0.12816563, 0.007398661, 0.1572824), vec3(0.1369046, 0.008020017, 0.15730207), vec3(0.14597888, 0.008666312, 0.15708491), vec3(0.15539509, 0.00933656, 0.1566394), vec3(0.16515826, 0.010029963, 0.15597263), vec3(0.17527373, 0.01074636, 0.15509336), vec3(0.18574715, 0.011485828, 0.15400328), vec3(0.19658448, 0.01224859, 0.15270615), vec3(0.20778736, 0.013035462, 0.15120722), vec3(0.21936052, 0.013847772, 0.14951044), vec3(0.23130418, 0.014686857, 0.14761913), vec3(0.24362104, 0.01555458, 0.14553647), vec3(0.25630945, 0.016453197, 0.1432689), vec3(0.26937073, 0.01738554, 0.14082028), vec3(0.2828013, 0.018354744, 0.13819626), vec3(0.29659814, 0.019364305, 0.13540421), vec3(0.3107568, 0.02041837, 0.13245139), vec3(0.32527044, 0.021521611, 0.1293436), vec3(0.34013203, 0.02267913, 0.12609199), vec3(0.35533002, 0.023896633, 0.122706555), vec3(0.37085614, 0.025180677, 0.11919673), vec3(0.38669696, 0.026537934, 0.1155722), vec3(0.4028372, 0.027976284, 0.11184702), vec3(0.41926005, 0.029504173, 0.10803284), vec3(0.43594778, 0.03113045, 0.104143575), vec3(0.4528798, 0.032865155, 0.100191556), vec3(0.47003177, 0.034718376, 0.09618961), vec3(0.48738313, 0.036701936, 0.09215296), vec3(0.50490403, 0.03882792, 0.08809595), vec3(0.52256775, 0.041108996, 0.0840326), vec3(0.5403422, 0.043558538, 0.079977006), vec3(0.5581976, 0.046191607, 0.07594139), vec3(0.57609993, 0.049023066, 0.07193904), vec3(0.59401315, 0.052068174, 0.067982584), vec3(0.6119005, 0.05534375, 0.06408458), vec3(0.6297258, 0.058866736, 0.060255717), vec3(0.64745015, 0.062653854, 0.056505997), vec3(0.6650338, 0.06672315, 0.052845273), vec3(0.682442, 0.071092464, 0.049281087), vec3(0.6996317, 0.0757799, 0.045820754), vec3(0.7165659, 0.08080393, 0.04247028), vec3(0.7332067, 0.08618197, 0.039235454), vec3(0.7495165, 0.091932856, 0.036119446), vec3(0.7654613, 0.098073415, 0.03312616), vec3(0.78100467, 0.1046214, 0.03025803), vec3(0.7961156, 0.111594625, 0.02751637), vec3(0.81076324, 0.11900943, 0.024902778), vec3(0.82491744, 0.12688157, 0.022417907), vec3(0.8385498, 0.13522667, 0.020062417), vec3(0.85163677, 0.14406104, 0.017836837), vec3(0.8641513, 0.15339826, 0.01574141), vec3(0.87607443, 0.1632525, 0.013777557), vec3(0.88738364, 0.1736395, 0.011946086), vec3(0.89805984, 0.18457112, 0.010249078), vec3(0.9080843, 0.19606017, 0.00868905), vec3(0.91744196, 0.20812023, 0.0072697657), vec3(0.926115, 0.22076279, 0.0059960275), vec3(0.93409115, 0.23400038, 0.004873595), vec3(0.9413553, 0.24784505, 0.0039101415), vec3(0.9478939, 0.26230624, 0.0031146826), vec3(0.9536967, 0.2773987, 0.0024980311), vec3(0.95874923, 0.29313073, 0.0020732752), vec3(0.9630435, 0.30951315, 0.001855572), vec3(0.966567, 0.32655644, 0.0018628523), vec3(0.9693118, 0.34427127, 0.0021157656), vec3(0.9712692, 0.3626653, 0.0026382324), vec3(0.97243184, 0.38174677, 0.003457789), vec3(0.97279316, 0.4015281, 0.0046063773), vec3(0.9723491, 0.42201203, 0.006120531), vec3(0.9710965, 0.44320524, 0.008042514), vec3(0.9690359, 0.46511263, 0.010420951), vec3(0.9661676, 0.4877382, 0.013312584), vec3(0.96249765, 0.51108307, 0.01678281), vec3(0.95804363, 0.53513855, 0.020907598), vec3(0.9528328, 0.55990005, 0.025776993), vec3(0.9469009, 0.5853509, 0.0314954), vec3(0.9402773, 0.611476, 0.038189955), vec3(0.9330464, 0.6382382, 0.04600755), vec3(0.9253274, 0.6655842, 0.055122882), vec3(0.91723233, 0.69345576, 0.06575425), vec3(0.9090141, 0.72174126, 0.07814396), vec3(0.90098083, 0.75029904, 0.092582785), vec3(0.89355445, 0.7789444, 0.10940892), vec3(0.8873942, 0.80739737, 0.12894122), vec3(0.8833361, 0.83531785, 0.15145478), vec3(0.8823836, 0.8623218, 0.17706329), vec3(0.8855449, 0.8880533, 0.20560762), vec3(0.89356405, 0.9122939, 0.23662856), vec3(0.90671027, 0.9350294, 0.26947564), vec3(0.92478114, 0.9564351, 0.30354354), vec3(0.9473031, 0.976763, 0.3383212), vec3(0.97372925, 0.99627715, 0.37352222));
 
         vec3 infernoMap(float min, float max, float value) {
             if (value <= min) return inferno[0];
             if (value >= max) return inferno[inferno.length() - 1];
 
@@ -582,14 +615,15 @@
         bool anyinf(vec3 v) {
             return isinf(v.x) || isinf(v.y) || isinf(v.z);
         }
 
         void main(void) {
             vec3 rgb = vec3(texture(hdr, uv));
             if (isLdr) rgb = vec3(SrgbToLinear(rgb.x), SrgbToLinear(rgb.y), SrgbToLinear(rgb.z));
+            if (isMono) rgb = vec3(rgb.x, rgb.x, rgb.x);
             ${toneMapCode}
             FragColor = vec4(LinearToSrgb(rgb.x), LinearToSrgb(rgb.y), LinearToSrgb(rgb.z), 1);
         }
     `;
 
     function loadShader(gl, type, source) {
         const shader = gl.createShader(type);
@@ -620,14 +654,15 @@
     const attribLocations = {
         vertexPosition: gl.getAttribLocation(shaderProgram, "aVertexPosition"),
         textureCoord: gl.getAttribLocation(shaderProgram, "aTextureCoord"),
     };
     const uniformLocations = {
         hdr: gl.getUniformLocation(shaderProgram, "hdr"),
         isLdr: gl.getUniformLocation(shaderProgram, "isLdr"),
+        isMono: gl.getUniformLocation(shaderProgram, "isMono"),
     }
 
     // vertex buffer
     const vertexBuffer = gl.createBuffer();
     gl.bindBuffer(gl.ARRAY_BUFFER, vertexBuffer);
     const positions = [
         -1.0, -1.0, 0.0,
@@ -646,19 +681,26 @@
         1.0, 1.0,
         1.0, 0.0
     ];
     gl.bufferData(gl.ARRAY_BUFFER, new Float32Array(texcoords), gl.STATIC_DRAW);
 
     const texture = gl.createTexture();
     gl.bindTexture(gl.TEXTURE_2D, texture);
-    let isLdr;
+    let isLdr, isMono = false;
     if (pixels instanceof Float32Array) {
-        gl.texImage2D(gl.TEXTURE_2D, 0, gl.RGB32F, canvas.width, canvas.height, 0, gl.RGB, gl.FLOAT, new Float32Array(pixels));
+        const numChan = pixels.length / canvas.width / canvas.height;
+        if (numChan == 3)
+            gl.texImage2D(gl.TEXTURE_2D, 0, gl.RGB32F, canvas.width, canvas.height, 0, gl.RGB, gl.FLOAT, new Float32Array(pixels));
+        else if (numChan == 1) {
+            isMono = true;
+            gl.texImage2D(gl.TEXTURE_2D, 0, gl.R32F, canvas.width, canvas.height, 0, gl.RED, gl.FLOAT, new Float32Array(pixels));
+        } else
+            alert('unsupported number of channels, expected 1 or 3');
         isLdr = false;
-    } else if (pixels instanceof Image) {
+    } else if (pixels instanceof ImageData) {
         gl.texImage2D(gl.TEXTURE_2D, 0, gl.RGBA, canvas.width, canvas.height, 0, gl.RGBA, gl.UNSIGNED_BYTE, pixels);
         isLdr = true;
     } else {
         alert('unsupported image data format, expected Float32Array or Image');
     }
     gl.texParameteri(gl.TEXTURE_2D, gl.TEXTURE_MIN_FILTER, gl.NEAREST);
     gl.texParameteri(gl.TEXTURE_2D, gl.TEXTURE_MAG_FILTER, gl.NEAREST);
@@ -666,14 +708,15 @@
     gl.clearColor(0.0, 1.0, 0.0, 1.0);
     gl.clear(gl.COLOR_BUFFER_BIT);
 
     gl.activeTexture(gl.TEXTURE0);
     gl.bindTexture(gl.TEXTURE_2D, texture);
     gl.uniform1i(uniformLocations.hdr, 0);
     gl.uniform1i(uniformLocations.isLdr, isLdr);
+    gl.uniform1i(uniformLocations.isMono, isMono);
 
     gl.bindBuffer(gl.ARRAY_BUFFER, vertexBuffer);
     gl.vertexAttribPointer(attribLocations.vertexPosition, 3, gl.FLOAT, false, 0, 0);
     gl.enableVertexAttribArray(attribLocations.vertexPosition);
 
     gl.bindBuffer(gl.ARRAY_BUFFER, uvBuffer);
     gl.vertexAttribPointer(attribLocations.textureCoord, 2, gl.FLOAT, false, 0, 0);
@@ -746,26 +789,17 @@
     let methodList = flipbook.find(".method-list");
     let imageList = flipbook.find(".image-placer");
 
     for (let i = 0; i < names.length; ++i) {
         methodList.append(`
             <button class='method-label method-${i+1}'><span class='method-key'>${i+1}</span> ${names[i]}</button>
         `);
-        // if (images[i] instanceof Image) { // LDR image in the form of a src string
-        //     imageList.append(`
-        //         <canvas draggable='false' class='image image-${i+1} ldr' width="${width}" height="${height}"></canvas>
-        //     `);
-        //     let canvas = imageList.find(`.image-${i + 1}`)[0];
-        //     let ctx = canvas.getContext('2d', { willReadFrequently: true });
-        //     ctx.drawImage(images[i], 0, 0);
-        // } else {
         imageList.append(`
-                <canvas draggable='false' class='image image-${i+1}' width="${width}" height="${height}"></canvas>
-            `);
-        // }
+            <canvas draggable='false' class='image image-${i+1}' width="${width}" height="${height}"></canvas>
+        `);
     }
 
     initImageViewers(flipbook[0], width, height, initialZoom);
     makeImages(flipbook[0], images, initialTMO);
 }
 
 function copyImage(flipIdx) {
```

### Comparing `simpleimageio-1.3.1/PyWrapper/simpleimageio/jquery-3.6.4.min.js` & `simpleimageio-1.3.2/PyWrapper/simpleimageio/jquery-3.6.4.min.js`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/PyWrapper/simpleimageio/manip.py` & `simpleimageio-1.3.2/PyWrapper/simpleimageio/manip.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/PyWrapper/simpleimageio/style.css` & `simpleimageio-1.3.2/PyWrapper/simpleimageio/style.css`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/PyWrapper/simpleimageio/tev.py` & `simpleimageio-1.3.2/PyWrapper/simpleimageio/tev.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/PyWrapper/simpleimageio/tonemap.py` & `simpleimageio-1.3.2/PyWrapper/simpleimageio/tonemap.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/README.md` & `simpleimageio-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.3.1/setup.py` & `simpleimageio-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         os.chdir(str(cwd))
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='simpleimageio',
-    version='1.3.1',
+    version='1.3.2',
     author='Pascal Grittmann',
     url='https://github.com/pgrit/SimpleImageIO',
 
     description='A very simple Python wrapper to read and write various HDR and LDR image file formats.',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `simpleimageio-1.3.1/simpleimageio.egg-info/PKG-INFO` & `simpleimageio-1.3.2/simpleimageio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleimageio
-Version: 1.3.1
+Version: 1.3.2
 Summary: A very simple Python wrapper to read and write various HDR and LDR image file formats.
 Home-page: https://github.com/pgrit/SimpleImageIO
 Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.1 Summary: A very simple
+Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.2 Summary: A very simple
 Python wrapper to read and write various HDR and LDR image file formats. Home-
 page: https://github.com/pgrit/SimpleImageIO Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE ![Build](https://github.com/pgrit/SimpleImageIO/workflows/Build/
 badge.svg) [https://buildstats.info/nuget/SimpleImageIO] # Simple Image IO A
```

### Comparing `simpleimageio-1.3.1/simpleimageio.egg-info/SOURCES.txt` & `simpleimageio-1.3.2/simpleimageio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

