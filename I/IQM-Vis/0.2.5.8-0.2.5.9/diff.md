# Comparing `tmp/IQM-VIS-0.2.5.8.tar.gz` & `tmp/IQM-VIS-0.2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IQM-VIS-0.2.5.8.tar", last modified: Tue Nov 15 20:42:46 2022, max compression
+gzip compressed data, was "IQM-VIS-0.2.5.9.tar", last modified: Wed Nov 16 12:11:19 2022, max compression
```

## Comparing `IQM-VIS-0.2.5.8.tar` & `IQM-VIS-0.2.5.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/IQM_VIS/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/IQM_VIS/UI/
--rw-rw-r--   0 matt      (1000) matt      (1000)       83 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/UI/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5410 2022-11-15 18:38:30.000000 IQM-VIS-0.2.5.8/IQM_VIS/UI/images.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4067 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/UI/layout.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      854 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/UI/main.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8519 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/UI/widgets.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      213 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2019 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/api.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1490 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/data.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/IQM_VIS/examples/
--rw-rw-r--   0 matt      (1000) matt      (1000)       50 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/examples/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1507 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/examples/multiple.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      846 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/examples/simple.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/layers/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/layers/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     9218 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/layers/divisive_normalisation.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    27784 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/pyramids.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/utils/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/utils/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1485 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/utils/conv.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5359 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/utils/fourier.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    22712 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/utils/pyramid_filters.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/metrics.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/IQM_VIS/transformations/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/transformations/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2994 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/transformations/transforms.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/IQM_VIS/utils/
--rw-rw-r--   0 matt      (1000) matt      (1000)      123 2022-11-15 19:07:32.000000 IQM-VIS-0.2.5.8/IQM_VIS/utils/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2327 2022-11-15 20:42:18.000000 IQM-VIS-0.2.5.8/IQM_VIS/utils/gui_utils.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      190 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/IQM_VIS/utils/image_utils.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2855 2022-11-15 11:52:33.000000 IQM-VIS-0.2.5.8/IQM_VIS/utils/plot_utils.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/IQM_VIS.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)      208 2022-11-15 20:42:46.000000 IQM-VIS-0.2.5.8/IQM_VIS.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     1086 2022-11-15 20:42:46.000000 IQM-VIS-0.2.5.8/IQM_VIS.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2022-11-15 20:42:46.000000 IQM-VIS-0.2.5.8/IQM_VIS.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       69 2022-11-15 20:42:46.000000 IQM-VIS-0.2.5.8/IQM_VIS.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       14 2022-11-15 20:42:46.000000 IQM-VIS-0.2.5.8/IQM_VIS.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)      208 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     1451 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.8/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)      638 2022-11-15 20:42:30.000000 IQM-VIS-0.2.5.8/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-15 20:42:46.768202 IQM-VIS-0.2.5.8/tests/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-10-25 10:42:10.000000 IQM-VIS-0.2.5.8/tests/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1154 2022-10-25 10:30:48.000000 IQM-VIS-0.2.5.8/tests/test_inputs.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.887005 IQM-VIS-0.2.5.9/IQM_VIS/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.887005 IQM-VIS-0.2.5.9/IQM_VIS/UI/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       83 2022-11-11 10:05:53.000000 IQM-VIS-0.2.5.9/IQM_VIS/UI/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5410 2022-11-16 09:46:43.000000 IQM-VIS-0.2.5.9/IQM_VIS/UI/images.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4067 2022-11-10 17:05:53.000000 IQM-VIS-0.2.5.9/IQM_VIS/UI/layout.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      854 2022-11-10 17:06:39.000000 IQM-VIS-0.2.5.9/IQM_VIS/UI/main.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8519 2022-11-10 17:06:47.000000 IQM-VIS-0.2.5.9/IQM_VIS/UI/widgets.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      213 2022-11-11 11:52:07.000000 IQM-VIS-0.2.5.9/IQM_VIS/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2019 2022-11-11 11:45:47.000000 IQM-VIS-0.2.5.9/IQM_VIS/api.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1490 2022-11-11 10:38:41.000000 IQM-VIS-0.2.5.9/IQM_VIS/data.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/IQM_VIS/examples/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       50 2022-11-11 11:04:42.000000 IQM-VIS-0.2.5.9/IQM_VIS/examples/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1507 2022-11-11 11:36:52.000000 IQM-VIS-0.2.5.9/IQM_VIS/examples/multiple.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      846 2022-11-11 11:18:18.000000 IQM-VIS-0.2.5.9/IQM_VIS/examples/simple.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-11 15:39:11.000000 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-11 10:53:25.000000 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/layers/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-11 10:52:07.000000 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/layers/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     9218 2022-10-19 12:03:23.000000 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/layers/divisive_normalisation.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    27784 2022-11-11 11:22:35.000000 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/pyramids.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/utils/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-11 10:51:59.000000 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/utils/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1485 2022-10-19 12:03:23.000000 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/utils/conv.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5359 2022-10-19 12:03:23.000000 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/utils/fourier.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    22712 2022-10-19 12:03:23.000000 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/utils/pyramid_filters.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2022-11-11 11:21:48.000000 IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/metrics.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/IQM_VIS/transformations/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-11 15:37:17.000000 IQM-VIS-0.2.5.9/IQM_VIS/transformations/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2994 2022-11-11 10:27:31.000000 IQM-VIS-0.2.5.9/IQM_VIS/transformations/transforms.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/IQM_VIS/utils/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      123 2022-11-16 09:46:43.000000 IQM-VIS-0.2.5.9/IQM_VIS/utils/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2327 2022-11-16 09:46:43.000000 IQM-VIS-0.2.5.9/IQM_VIS/utils/gui_utils.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      190 2022-11-11 11:18:16.000000 IQM-VIS-0.2.5.9/IQM_VIS/utils/image_utils.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2855 2022-11-16 09:46:43.000000 IQM-VIS-0.2.5.9/IQM_VIS/utils/plot_utils.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.887005 IQM-VIS-0.2.5.9/IQM_VIS.egg-info/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1700 2022-11-16 12:11:19.000000 IQM-VIS-0.2.5.9/IQM_VIS.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1086 2022-11-16 12:11:19.000000 IQM-VIS-0.2.5.9/IQM_VIS.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2022-11-16 12:11:19.000000 IQM-VIS-0.2.5.9/IQM_VIS.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       69 2022-11-16 12:11:19.000000 IQM-VIS-0.2.5.9/IQM_VIS.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       14 2022-11-16 12:11:19.000000 IQM-VIS-0.2.5.9/IQM_VIS.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1700 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1451 2022-11-11 11:27:39.000000 IQM-VIS-0.2.5.9/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)      850 2022-11-16 12:11:02.000000 IQM-VIS-0.2.5.9/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-11-16 12:11:19.891005 IQM-VIS-0.2.5.9/tests/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-10-26 10:50:28.000000 IQM-VIS-0.2.5.9/tests/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1154 2022-10-24 17:01:55.000000 IQM-VIS-0.2.5.9/tests/test_inputs.py
```

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/UI/images.py` & `IQM-VIS-0.2.5.9/IQM_VIS/UI/images.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/UI/layout.py` & `IQM-VIS-0.2.5.9/IQM_VIS/UI/layout.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/UI/main.py` & `IQM-VIS-0.2.5.9/IQM_VIS/UI/main.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/UI/widgets.py` & `IQM-VIS-0.2.5.9/IQM_VIS/UI/widgets.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/api.py` & `IQM-VIS-0.2.5.9/IQM_VIS/api.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/data.py` & `IQM-VIS-0.2.5.9/IQM_VIS/data.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/examples/multiple.py` & `IQM-VIS-0.2.5.9/IQM_VIS/examples/multiple.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/examples/simple.py` & `IQM-VIS-0.2.5.9/IQM_VIS/examples/simple.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/layers/divisive_normalisation.py` & `IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/layers/divisive_normalisation.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/pyramids.py` & `IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/pyramids.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/utils/conv.py` & `IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/utils/conv.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/utils/fourier.py` & `IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/utils/fourier.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/expert/utils/pyramid_filters.py` & `IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/expert/utils/pyramid_filters.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/image_metrics/metrics.py` & `IQM-VIS-0.2.5.9/IQM_VIS/image_metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/transformations/transforms.py` & `IQM-VIS-0.2.5.9/IQM_VIS/transformations/transforms.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/utils/gui_utils.py` & `IQM-VIS-0.2.5.9/IQM_VIS/utils/gui_utils.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS/utils/plot_utils.py` & `IQM-VIS-0.2.5.9/IQM_VIS/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/IQM_VIS.egg-info/SOURCES.txt` & `IQM-VIS-0.2.5.9/IQM_VIS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/README.md` & `IQM-VIS-0.2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `IQM-VIS-0.2.5.8/tests/test_inputs.py` & `IQM-VIS-0.2.5.9/tests/test_inputs.py`

 * *Files identical despite different names*

