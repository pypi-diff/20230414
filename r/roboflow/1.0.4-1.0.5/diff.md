# Comparing `tmp/roboflow-1.0.4.tar.gz` & `tmp/roboflow-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboflow-1.0.4.tar", last modified: Fri Apr 14 14:32:00 2023, max compression
+gzip compressed data, was "roboflow-1.0.5.tar", last modified: Fri Apr 14 18:46:32 2023, max compression
```

## Comparing `roboflow-1.0.4.tar` & `roboflow-1.0.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.680906 roboflow-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-14 14:31:38.000000 roboflow-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-14 14:32:00.680906 roboflow-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-14 14:31:38.000000 roboflow-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 14:31:38.000000 roboflow-1.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.676906 roboflow-1.0.4/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.676906 roboflow-1.0.4/roboflow/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/archive/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.676906 roboflow-1.0.4/roboflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22648 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/core/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    28721 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/core/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.676906 roboflow-1.0.4/roboflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/models/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/models/instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19743 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/models/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/models/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.676906 roboflow-1.0.4/roboflow/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/util/active_learning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/util/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/util/clip_compare_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/util/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/util/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/util/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/util/two_stage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-14 14:31:38.000000 roboflow-1.0.4/roboflow/util/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.676906 roboflow-1.0.4/roboflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-14 14:32:00.000000 roboflow-1.0.4/roboflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-14 14:32:00.000000 roboflow-1.0.4/roboflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:32:00.000000 roboflow-1.0.4/roboflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-14 14:32:00.000000 roboflow-1.0.4/roboflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 14:32:00.000000 roboflow-1.0.4/roboflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:32:00.680906 roboflow-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-14 14:31:38.000000 roboflow-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.676906 roboflow-1.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.676906 roboflow-1.0.4/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/models/test_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/models/test_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/models/test_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.680906 roboflow-1.0.4/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:32:00.680906 roboflow-1.0.4/tests/util/dummy_module/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/util/dummy_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/util/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-14 14:31:38.000000 roboflow-1.0.4/tests/util/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.691317 roboflow-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-14 18:46:10.000000 roboflow-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-14 18:46:32.691317 roboflow-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-14 18:46:10.000000 roboflow-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 18:46:10.000000 roboflow-1.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/archive/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22648 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/active_learning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/clip_compare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/two_stage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-14 18:46:32.000000 roboflow-1.0.5/roboflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-14 18:46:32.000000 roboflow-1.0.5/roboflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:46:32.000000 roboflow-1.0.5/roboflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-14 18:46:32.000000 roboflow-1.0.5/roboflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 18:46:32.000000 roboflow-1.0.5/roboflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:46:32.691317 roboflow-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-14 18:46:10.000000 roboflow-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/models/test_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/models/test_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/models/test_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.691317 roboflow-1.0.5/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.691317 roboflow-1.0.5/tests/util/dummy_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/util/dummy_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/util/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/util/test_versions.py
```

### Comparing `roboflow-1.0.4/LICENSE` & `roboflow-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/PKG-INFO` & `roboflow-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.0.4
+Version: 1.0.5
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.0.4 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.0.5 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.0.4/README.md` & `roboflow-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/__init__.py` & `roboflow-1.0.5/roboflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 from roboflow.config import API_URL, APP_URL, DEMO_KEYS, load_roboflow_api_key
 from roboflow.core.project import Project
 from roboflow.core.workspace import Workspace
 from roboflow.util.general import write_line
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 
 def check_key(api_key, model, notebook, num_retries=0):
     if type(api_key) is not str:
         raise RuntimeError(
             "API Key is of Incorrect Type \n Expected Type: "
             + str(type(""))
```

### Comparing `roboflow-1.0.4/roboflow/archive/plot.py` & `roboflow-1.0.5/roboflow/archive/plot.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/config.py` & `roboflow-1.0.5/roboflow/config.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/core/project.py` & `roboflow-1.0.5/roboflow/core/project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/core/version.py` & `roboflow-1.0.5/roboflow/core/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,40 +429,14 @@
             previous_epochs = copy.deepcopy(epochs)
 
             time.sleep(5)
 
         # return the model object
         return self.model
 
-    def get_pt_weights(self, location="."):
-        workspace, project, *_ = self.id.rsplit("/")
-
-        # get pt url
-        pt_api_url = f"{API_URL}/{workspace}/{project}/{self.version}/ptFile"
-
-        r = requests.get(pt_api_url, params={"api_key": self.__api_key})
-
-        r.raise_for_status()
-
-        pt_weights_url = r.json()["weightsUrl"]
-
-        def bar_progress(current, total, width=80):
-            progress_message = (
-                "Downloading weights to "
-                + location
-                + "/weights.pt"
-                + ": %d%% [%d / %d] bytes" % (current / total * 100, current, total)
-            )
-            sys.stdout.write("\r" + progress_message)
-            sys.stdout.flush()
-
-        wget.download(pt_weights_url, out=location + "/weights.pt", bar=bar_progress)
-
-        return
-
     # @warn_for_wrong_dependencies_versions([("ultralytics", "<=", "8.0.20")])
     def deploy(self, model_type: str, model_path: str) -> None:
         """Uploads provided weights file to Roboflow
 
         Args:
             model_path (str): File path to model weights to be uploaded
         """
```

### Comparing `roboflow-1.0.4/roboflow/core/workspace.py` & `roboflow-1.0.5/roboflow/core/workspace.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/models/classification.py` & `roboflow-1.0.5/roboflow/models/classification.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/models/inference.py` & `roboflow-1.0.5/roboflow/models/inference.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/models/instance_segmentation.py` & `roboflow-1.0.5/roboflow/models/instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/models/object_detection.py` & `roboflow-1.0.5/roboflow/models/object_detection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import base64
 import copy
 import io
 import json
 import os
 import random
+import sys
 import urllib
 from pathlib import Path
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import requests
+import wget
 from PIL import Image
 
-from roboflow.config import OBJECT_DETECTION_MODEL
+from roboflow.config import API_URL, OBJECT_DETECTION_MODEL
 from roboflow.util.image_utils import check_image_url
 from roboflow.util.prediction import PredictionGroup
 from roboflow.util.versions import (
     print_warn_for_wrong_dependencies_versions,
     warn_for_wrong_dependencies_versions,
 )
 
@@ -455,14 +457,46 @@
         if within_jupyter:
             display(stopButton)
             thread = threading.Thread(target=view, args=(stopButton,))
             thread.start()
         else:
             view(stopButton)
 
+    def download(self, format="pt", location="."):
+        supported_formats = ["pt"]
+        if format not in supported_formats:
+            raise Exception(
+                f"Unsupported format {format}. Must be one of {supported_formats}"
+            )
+
+        workspace, project, version = self.id.rsplit("/")
+
+        # get pt url
+        pt_api_url = f"{API_URL}/{workspace}/{project}/{self.version}/ptFile"
+
+        r = requests.get(pt_api_url, params={"api_key": self.__api_key})
+
+        r.raise_for_status()
+
+        pt_weights_url = r.json()["weightsUrl"]
+
+        def bar_progress(current, total, width=80):
+            progress_message = (
+                "Downloading weights to "
+                + location
+                + "/weights.pt"
+                + ": %d%% [%d / %d] bytes" % (current / total * 100, current, total)
+            )
+            sys.stdout.write("\r" + progress_message)
+            sys.stdout.flush()
+
+        wget.download(pt_weights_url, out=location + "/weights.pt", bar=bar_progress)
+
+        return
+
     def __exception_check(self, image_path_check=None):
         # Check if Image path exists exception check (for both hosted URL and local image)
         if image_path_check is not None:
             if not os.path.exists(image_path_check) and not check_image_url(
                 image_path_check
             ):
                 raise Exception("Image does not exist at " + image_path_check + "!")
```

### Comparing `roboflow-1.0.4/roboflow/models/semantic_segmentation.py` & `roboflow-1.0.5/roboflow/models/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/util/active_learning_utils.py` & `roboflow-1.0.5/roboflow/util/active_learning_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/util/clip_compare_utils.py` & `roboflow-1.0.5/roboflow/util/clip_compare_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/util/image_utils.py` & `roboflow-1.0.5/roboflow/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/util/prediction.py` & `roboflow-1.0.5/roboflow/util/prediction.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/util/two_stage_utils.py` & `roboflow-1.0.5/roboflow/util/two_stage_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow/util/versions.py` & `roboflow-1.0.5/roboflow/util/versions.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/roboflow.egg-info/PKG-INFO` & `roboflow-1.0.5/roboflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.0.4
+Version: 1.0.5
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.0.4 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.0.5 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.0.4/roboflow.egg-info/SOURCES.txt` & `roboflow-1.0.5/roboflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/setup.py` & `roboflow-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/tests/models/test_instance_segmentation.py` & `roboflow-1.0.5/tests/models/test_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/tests/models/test_object_detection.py` & `roboflow-1.0.5/tests/models/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/tests/models/test_semantic_segmentation.py` & `roboflow-1.0.5/tests/models/test_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/tests/test_project.py` & `roboflow-1.0.5/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/tests/test_queries.py` & `roboflow-1.0.5/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/tests/test_version.py` & `roboflow-1.0.5/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/tests/util/test_image_utils.py` & `roboflow-1.0.5/tests/util/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.4/tests/util/test_versions.py` & `roboflow-1.0.5/tests/util/test_versions.py`

 * *Files identical despite different names*

