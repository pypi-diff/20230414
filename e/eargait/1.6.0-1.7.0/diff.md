# Comparing `tmp/eargait-1.6.0.tar.gz` & `tmp/eargait-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eargait-1.6.0.tar", max compression
+gzip compressed data, was "eargait-1.7.0.tar", max compression
```

## Comparing `eargait-1.6.0.tar` & `eargait-1.7.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1072 2023-04-11 06:58:46.010700 eargait-1.6.0/LICENSE
--rw-r--r--   0        0        0     5531 2023-04-11 06:58:46.010700 eargait-1.6.0/README.md
--rw-r--r--   0        0        0      154 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/base/__init__.py
--rw-r--r--   0        0        0     5028 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/base/base_eargait.py
--rw-r--r--   0        0        0    13447 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/eargait.py
--rw-r--r--   0        0        0      411 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/__init__.py
--rw-r--r--   0        0        0    10101 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/base_event_detection.py
--rw-r--r--   0        0        0     4990 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/diao_adapted_event_detection.py
--rw-r--r--   0        0        0     8327 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/diao_event_detection.py
--rw-r--r--   0        0        0     9077 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/jarchi_event_detection.py
--rw-r--r--   0        0        0     9367 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/event_detection/mixed_event_detection.py
--rw-r--r--   0        0        0      307 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/preprocessing/__init__.py
--rw-r--r--   0        0        0     2275 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/preprocessing/load_data_helpers.py
--rw-r--r--   0        0        0     6833 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/preprocessing/rotations.py
--rw-r--r--   0        0        0      204 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/spatial_params/__init__.py
--rw-r--r--   0        0        0      296 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/spatial_params/spatial_params_base.py
--rw-r--r--   0        0        0     1340 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/spatial_params/spatial_params_example_class.py
--rw-r--r--   0        0        0        0 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/utils/__init__.py
--rw-r--r--   0        0        0      609 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/utils/consts.py
--rw-r--r--   0        0        0     1334 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/utils/example_data.py
--rw-r--r--   0        0        0     5535 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/utils/gait_parameters.py
--rw-r--r--   0        0        0     3809 2023-04-11 06:58:46.022700 eargait-1.6.0/eargait/utils/helper_datatype.py
--rw-r--r--   0        0        0    58034 2023-04-11 06:58:46.026700 eargait-1.6.0/eargait/utils/helper_gaitmap.py
--rw-r--r--   0        0        0     2033 2023-04-11 06:58:46.026700 eargait-1.6.0/eargait/utils/helpers.py
--rw-r--r--   0        0        0     2458 2023-04-11 06:58:46.090701 eargait-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 eargait-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-14 12:01:13.097482 eargait-1.7.0/LICENSE
+-rw-r--r--   0        0        0     5531 2023-04-14 12:01:13.097482 eargait-1.7.0/README.md
+-rw-r--r--   0        0        0      154 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/base/__init__.py
+-rw-r--r--   0        0        0     5028 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/base/base_eargait.py
+-rw-r--r--   0        0        0    13447 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/eargait.py
+-rw-r--r--   0        0        0      411 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/event_detection/__init__.py
+-rw-r--r--   0        0        0    10101 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/event_detection/base_event_detection.py
+-rw-r--r--   0        0        0     4990 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/event_detection/diao_adapted_event_detection.py
+-rw-r--r--   0        0        0     8327 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/event_detection/diao_event_detection.py
+-rw-r--r--   0        0        0     9077 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/event_detection/jarchi_event_detection.py
+-rw-r--r--   0        0        0     9367 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/event_detection/mixed_event_detection.py
+-rw-r--r--   0        0        0      307 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2275 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/preprocessing/load_data_helpers.py
+-rw-r--r--   0        0        0     6833 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/preprocessing/rotations.py
+-rw-r--r--   0        0        0      204 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/spatial_params/__init__.py
+-rw-r--r--   0        0        0      296 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/spatial_params/spatial_params_base.py
+-rw-r--r--   0        0        0     1340 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/spatial_params/spatial_params_example_class.py
+-rw-r--r--   0        0        0        0 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/utils/__init__.py
+-rw-r--r--   0        0        0      609 2023-04-14 12:01:13.105482 eargait-1.7.0/eargait/utils/consts.py
+-rw-r--r--   0        0        0     1334 2023-04-14 12:01:13.109482 eargait-1.7.0/eargait/utils/example_data.py
+-rw-r--r--   0        0        0     5535 2023-04-14 12:01:13.109482 eargait-1.7.0/eargait/utils/gait_parameters.py
+-rw-r--r--   0        0        0     3809 2023-04-14 12:01:13.109482 eargait-1.7.0/eargait/utils/helper_datatype.py
+-rw-r--r--   0        0        0    58034 2023-04-14 12:01:13.109482 eargait-1.7.0/eargait/utils/helper_gaitmap.py
+-rw-r--r--   0        0        0     2033 2023-04-14 12:01:13.109482 eargait-1.7.0/eargait/utils/helpers.py
+-rw-r--r--   0        0        0     2458 2023-04-14 12:01:13.169483 eargait-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 eargait-1.7.0/PKG-INFO
```

### Comparing `eargait-1.6.0/LICENSE` & `eargait-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/README.md` & `eargait-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/base/base_eargait.py` & `eargait-1.7.0/eargait/base/base_eargait.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/eargait.py` & `eargait-1.7.0/eargait/eargait.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/event_detection/base_event_detection.py` & `eargait-1.7.0/eargait/event_detection/base_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/event_detection/diao_adapted_event_detection.py` & `eargait-1.7.0/eargait/event_detection/diao_adapted_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/event_detection/diao_event_detection.py` & `eargait-1.7.0/eargait/event_detection/diao_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/event_detection/jarchi_event_detection.py` & `eargait-1.7.0/eargait/event_detection/jarchi_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/event_detection/mixed_event_detection.py` & `eargait-1.7.0/eargait/event_detection/mixed_event_detection.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/preprocessing/load_data_helpers.py` & `eargait-1.7.0/eargait/preprocessing/load_data_helpers.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/preprocessing/rotations.py` & `eargait-1.7.0/eargait/preprocessing/rotations.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/spatial_params/spatial_params_example_class.py` & `eargait-1.7.0/eargait/spatial_params/spatial_params_example_class.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/utils/consts.py` & `eargait-1.7.0/eargait/utils/consts.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/utils/example_data.py` & `eargait-1.7.0/eargait/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/utils/gait_parameters.py` & `eargait-1.7.0/eargait/utils/gait_parameters.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/utils/helper_datatype.py` & `eargait-1.7.0/eargait/utils/helper_datatype.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/utils/helper_gaitmap.py` & `eargait-1.7.0/eargait/utils/helper_gaitmap.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/eargait/utils/helpers.py` & `eargait-1.7.0/eargait/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `eargait-1.6.0/pyproject.toml` & `eargait-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eargait"
-version = "1.6.0"
+version = "1.7.0"
 description = "*Eargait* provides a set of algorithms and functions to process IMU data recorded with ear-worn IMU sensors and to estimate characteristic gait parameters. "
 authors = ["Ann-Kristin Seifer <ann-kristin.seifer@fau.de>",
             "Arne Küderle <arne.kuederle@fau.de>"]
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/eargait"
 repository = "https://github.com/mad-lab-fau/eargait"
 
@@ -12,15 +12,15 @@
 python = ">=3.8,<4.0"
 joblib = ">=1.2.0"
 tpcp = ">=0.12, <1.0.0"
 scipy = "^1, !=1.6.0"
 pyts = "^0.11.0"
 nilspodlib = "^3.2.2"
 fau-colors = "^1.0.1"
-signialib = "^2.2.0"
+signialib = "^2.3.0"
 pandas = ">=1.5.2"
 numba =  [
     {version = ">=0.55"},
     {version = ">=0.55.2", markers = "sys_platform == 'darwin' and platform_machine == 'arm64'"}
 ]
 numpy = ">=1.20"
```

### Comparing `eargait-1.6.0/PKG-INFO` & `eargait-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eargait
-Version: 1.6.0
+Version: 1.7.0
 Summary: *Eargait* provides a set of algorithms and functions to process IMU data recorded with ear-worn IMU sensors and to estimate characteristic gait parameters. 
 Home-page: https://github.com/mad-lab-fau/eargait
 Author: Ann-Kristin Seifer
 Author-email: ann-kristin.seifer@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -16,15 +16,15 @@
 Requires-Dist: nilspodlib (>=3.2.2,<4.0.0)
 Requires-Dist: numba (>=0.55)
 Requires-Dist: numba (>=0.55.2) ; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: pandas (>=1.5.2)
 Requires-Dist: pyts (>=0.11.0,<0.12.0)
 Requires-Dist: scipy (>=1,<2,!=1.6.0)
-Requires-Dist: signialib (>=2.2.0,<3.0.0)
+Requires-Dist: signialib (>=2.3.0,<3.0.0)
 Requires-Dist: tpcp (>=0.12,<1.0.0)
 Project-URL: Repository, https://github.com/mad-lab-fau/eargait
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/eargait)](https://pypi.org/project/eargait/)
 [![Documentation Status](https://readthedocs.org/projects/eargait/badge/?version=latest)](https://eargait.readthedocs.io/en/latest/?badge=latest)
 [![Test and Lint](https://github.com/mad-lab-fau/eargait/actions/workflows/test-and-lint.yml/badge.svg?branch=main)](https://github.com/mad-lab-fau/eargait/actions/workflows/test-and-lint.yml)
```

