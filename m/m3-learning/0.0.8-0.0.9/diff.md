# Comparing `tmp/m3_learning-0.0.8.tar.gz` & `tmp/m3_learning-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3_learning-0.0.8.tar", last modified: Mon Nov  7 04:30:15 2022, max compression
+gzip compressed data, was "m3_learning-0.0.9.tar", last modified: Mon Nov  7 04:36:54 2022, max compression
```

## Comparing `m3_learning-0.0.8.tar` & `m3_learning-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-11-07 04:30:15.665634 m3_learning-0.0.8/
--rw-rw-rw-   0        0        0      445 2022-11-07 04:30:15.665634 m3_learning-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-11-07 04:30:15.665634 m3_learning-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      754 2022-11-06 23:50:06.000000 m3_learning-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-07 04:30:15.582530 m3_learning-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-11-07 04:30:15.589530 m3_learning-0.0.8/src/m3_learning/
--rw-rw-rw-   0        0        0       73 2022-11-05 16:21:07.000000 m3_learning-0.0.8/src/m3_learning/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-07 04:30:15.613531 m3_learning-0.0.8/src/m3_learning/be/
--rw-rw-rw-   0        0        0       44 2022-11-06 00:14:55.000000 m3_learning-0.0.8/src/m3_learning/be/__init__.py
--rw-rw-rw-   0        0        0      431 2022-11-06 23:47:20.000000 m3_learning-0.0.8/src/m3_learning/be/processing.py
--rw-rw-rw-   0        0        0     5302 2022-11-06 23:45:40.000000 m3_learning-0.0.8/src/m3_learning/be/util.py
-drwxrwxrwx   0        0        0        0 2022-11-07 04:30:15.619529 m3_learning-0.0.8/src/m3_learning/nn/
--rw-rw-rw-   0        0        0       50 2022-11-05 15:28:09.000000 m3_learning-0.0.8/src/m3_learning/nn/__init__.py
--rw-rw-rw-   0        0        0      613 2022-11-05 15:29:57.000000 m3_learning-0.0.8/src/m3_learning/nn/random.py
-drwxrwxrwx   0        0        0        0 2022-11-07 04:30:15.629530 m3_learning-0.0.8/src/m3_learning/nn/time_series_nn/
--rw-rw-rw-   0        0        0       21 2022-11-01 20:33:42.000000 m3_learning-0.0.8/src/m3_learning/nn/time_series_nn/__init__.py
--rw-rw-rw-   0        0        0     8839 2022-11-01 20:33:42.000000 m3_learning-0.0.8/src/m3_learning/nn/time_series_nn/nn_util.py
-drwxrwxrwx   0        0        0        0 2022-11-07 04:30:15.657666 m3_learning-0.0.8/src/m3_learning/util/
--rw-rw-rw-   0        0        0      100 2022-11-03 17:38:49.000000 m3_learning-0.0.8/src/m3_learning/util/__init__.py
--rw-rw-rw-   0        0        0     1355 2022-11-06 23:40:58.000000 m3_learning-0.0.8/src/m3_learning/util/data_generators.py
--rw-rw-rw-   0        0        0     3732 2022-11-07 03:24:22.000000 m3_learning-0.0.8/src/m3_learning/util/file_IO.py
--rw-rw-rw-   0        0        0     1265 2022-11-06 23:38:45.000000 m3_learning-0.0.8/src/m3_learning/util/h5_util.py
--rw-rw-rw-   0        0        0     1332 2022-11-06 23:36:07.000000 m3_learning-0.0.8/src/m3_learning/util/preprocessing.py
--rw-rw-rw-   0        0        0      849 2022-11-01 20:33:42.000000 m3_learning-0.0.8/src/m3_learning/util/rand_util.py
-drwxrwxrwx   0        0        0        0 2022-11-07 04:30:15.664652 m3_learning-0.0.8/src/m3_learning/viz/
--rw-rw-rw-   0        0        0       41 2022-11-05 15:38:52.000000 m3_learning-0.0.8/src/m3_learning/viz/__init__.py
--rw-rw-rw-   0        0        0     7422 2022-11-06 23:47:50.000000 m3_learning-0.0.8/src/m3_learning/viz/layout.py
--rw-rw-rw-   0        0        0     1125 2022-11-06 23:48:27.000000 m3_learning-0.0.8/src/m3_learning/viz/style.py
-drwxrwxrwx   0        0        0        0 2022-11-07 04:30:15.605530 m3_learning-0.0.8/src/m3_learning.egg-info/
--rw-rw-rw-   0        0        0      445 2022-11-07 04:30:15.000000 m3_learning-0.0.8/src/m3_learning.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      772 2022-11-07 04:30:15.000000 m3_learning-0.0.8/src/m3_learning.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-07 04:30:15.000000 m3_learning-0.0.8/src/m3_learning.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2022-11-07 04:30:15.000000 m3_learning-0.0.8/src/m3_learning.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-11-07 04:30:15.000000 m3_learning-0.0.8/src/m3_learning.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-07 04:36:54.071576 m3_learning-0.0.9/
+-rw-rw-rw-   0        0        0      445 2022-11-07 04:36:54.071576 m3_learning-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2022-11-07 04:36:54.071576 m3_learning-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      754 2022-11-07 04:36:20.000000 m3_learning-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-07 04:36:54.049915 m3_learning-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-11-07 04:36:54.055934 m3_learning-0.0.9/src/m3_learning/
+-rw-rw-rw-   0        0        0       73 2022-11-05 16:21:07.000000 m3_learning-0.0.9/src/m3_learning/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-07 04:36:54.055934 m3_learning-0.0.9/src/m3_learning/be/
+-rw-rw-rw-   0        0        0       44 2022-11-06 00:14:55.000000 m3_learning-0.0.9/src/m3_learning/be/__init__.py
+-rw-rw-rw-   0        0        0      431 2022-11-06 23:47:20.000000 m3_learning-0.0.9/src/m3_learning/be/processing.py
+-rw-rw-rw-   0        0        0     5302 2022-11-06 23:45:40.000000 m3_learning-0.0.9/src/m3_learning/be/util.py
+drwxrwxrwx   0        0        0        0 2022-11-07 04:36:54.055934 m3_learning-0.0.9/src/m3_learning/nn/
+-rw-rw-rw-   0        0        0       50 2022-11-05 15:28:09.000000 m3_learning-0.0.9/src/m3_learning/nn/__init__.py
+-rw-rw-rw-   0        0        0      613 2022-11-05 15:29:57.000000 m3_learning-0.0.9/src/m3_learning/nn/random.py
+drwxrwxrwx   0        0        0        0 2022-11-07 04:36:54.071576 m3_learning-0.0.9/src/m3_learning/nn/time_series_nn/
+-rw-rw-rw-   0        0        0       21 2022-11-01 20:33:42.000000 m3_learning-0.0.9/src/m3_learning/nn/time_series_nn/__init__.py
+-rw-rw-rw-   0        0        0     8839 2022-11-01 20:33:42.000000 m3_learning-0.0.9/src/m3_learning/nn/time_series_nn/nn_util.py
+drwxrwxrwx   0        0        0        0 2022-11-07 04:36:54.071576 m3_learning-0.0.9/src/m3_learning/util/
+-rw-rw-rw-   0        0        0      100 2022-11-03 17:38:49.000000 m3_learning-0.0.9/src/m3_learning/util/__init__.py
+-rw-rw-rw-   0        0        0     1355 2022-11-06 23:40:58.000000 m3_learning-0.0.9/src/m3_learning/util/data_generators.py
+-rw-rw-rw-   0        0        0     3732 2022-11-07 03:24:22.000000 m3_learning-0.0.9/src/m3_learning/util/file_IO.py
+-rw-rw-rw-   0        0        0     1265 2022-11-06 23:38:45.000000 m3_learning-0.0.9/src/m3_learning/util/h5_util.py
+-rw-rw-rw-   0        0        0     1332 2022-11-06 23:36:07.000000 m3_learning-0.0.9/src/m3_learning/util/preprocessing.py
+-rw-rw-rw-   0        0        0      849 2022-11-01 20:33:42.000000 m3_learning-0.0.9/src/m3_learning/util/rand_util.py
+drwxrwxrwx   0        0        0        0 2022-11-07 04:36:54.071576 m3_learning-0.0.9/src/m3_learning/viz/
+-rw-rw-rw-   0        0        0       41 2022-11-05 15:38:52.000000 m3_learning-0.0.9/src/m3_learning/viz/__init__.py
+-rw-rw-rw-   0        0        0     7422 2022-11-06 23:47:50.000000 m3_learning-0.0.9/src/m3_learning/viz/layout.py
+-rw-rw-rw-   0        0        0     1125 2022-11-06 23:48:27.000000 m3_learning-0.0.9/src/m3_learning/viz/style.py
+drwxrwxrwx   0        0        0        0 2022-11-07 04:36:54.055934 m3_learning-0.0.9/src/m3_learning.egg-info/
+-rw-rw-rw-   0        0        0      445 2022-11-07 04:36:53.000000 m3_learning-0.0.9/src/m3_learning.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2022-11-07 04:36:54.000000 m3_learning-0.0.9/src/m3_learning.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-07 04:36:53.000000 m3_learning-0.0.9/src/m3_learning.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2929 2022-11-07 04:36:53.000000 m3_learning-0.0.9/src/m3_learning.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2022-11-07 04:36:53.000000 m3_learning-0.0.9/src/m3_learning.egg-info/top_level.txt
```

### Comparing `m3_learning-0.0.8/setup.py` & `m3_learning-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("src/requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="m3_learning",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(where="src"),
     url="https://github.com/jagar2/m3_learning.git",
     install_requires=requirements,
     license=" BSD-3-Clause",
     author="Joshua C. Agar",
     author_email="jca92@drexel.edu",
     description="Tutorials, Projects, and datasets from the M3-learning research group",
```

### Comparing `m3_learning-0.0.8/src/m3_learning/be/util.py` & `m3_learning-0.0.9/src/m3_learning/be/util.py`

 * *Files identical despite different names*

### Comparing `m3_learning-0.0.8/src/m3_learning/nn/random.py` & `m3_learning-0.0.9/src/m3_learning/nn/random.py`

 * *Files identical despite different names*

### Comparing `m3_learning-0.0.8/src/m3_learning/nn/time_series_nn/nn_util.py` & `m3_learning-0.0.9/src/m3_learning/nn/time_series_nn/nn_util.py`

 * *Files identical despite different names*

### Comparing `m3_learning-0.0.8/src/m3_learning/util/data_generators.py` & `m3_learning-0.0.9/src/m3_learning/util/data_generators.py`

 * *Files identical despite different names*

### Comparing `m3_learning-0.0.8/src/m3_learning/util/file_IO.py` & `m3_learning-0.0.9/src/m3_learning/util/file_IO.py`

 * *Files identical despite different names*

### Comparing `m3_learning-0.0.8/src/m3_learning/util/h5_util.py` & `m3_learning-0.0.9/src/m3_learning/util/h5_util.py`

 * *Files identical despite different names*

### Comparing `m3_learning-0.0.8/src/m3_learning/util/preprocessing.py` & `m3_learning-0.0.9/src/m3_learning/util/preprocessing.py`

 * *Files identical despite different names*

### Comparing `m3_learning-0.0.8/src/m3_learning/util/rand_util.py` & `m3_learning-0.0.9/src/m3_learning/util/rand_util.py`

 * *Files identical despite different names*

### Comparing `m3_learning-0.0.8/src/m3_learning/viz/layout.py` & `m3_learning-0.0.9/src/m3_learning/viz/layout.py`

 * *Files identical despite different names*

### Comparing `m3_learning-0.0.8/src/m3_learning/viz/style.py` & `m3_learning-0.0.9/src/m3_learning/viz/style.py`

 * *Files identical despite different names*

### Comparing `m3_learning-0.0.8/src/m3_learning.egg-info/SOURCES.txt` & `m3_learning-0.0.9/src/m3_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

