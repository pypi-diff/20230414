# Comparing `tmp/ml_wrappers-0.4.6.tar.gz` & `tmp/ml_wrappers-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ml_wrappers-0.4.6.tar", last modified: Fri Mar 17 00:33:10 2023, max compression
+gzip compressed data, was "dist/ml_wrappers-0.4.7.tar", last modified: Fri Apr 14 19:12:19 2023, max compression
```

## Comparing `ml_wrappers-0.4.6.tar` & `ml_wrappers-0.4.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/common/gpu_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/common/warnings_suppressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/dataset/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28409 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/dataset/timestamp_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers/model/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/base_wrapped_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/endpoint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/fastai_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16616 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/image_model_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/model_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/predictions_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/pytorch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/tensorflow_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/text_model_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/wrapped_classification_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/wrapped_classification_without_proba_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/model/wrapped_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/ml_wrappers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/ml_wrappers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-17 00:33:10.000000 ml_wrappers-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-17 00:29:26.000000 ml_wrappers-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/common/gpu_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/common/warnings_suppressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/dataset/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28409 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/dataset/timestamp_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/base_wrapped_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/endpoint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/fastai_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24120 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/image_model_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/model_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/predictions_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/pytorch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/tensorflow_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/text_model_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/wrapped_classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/wrapped_classification_without_proba_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/model/wrapped_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/ml_wrappers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/ml_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 19:12:19.000000 ml_wrappers-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-14 19:09:10.000000 ml_wrappers-0.4.7/setup.py
```

### Comparing `ml_wrappers-0.4.6/LICENSE.txt` & `ml_wrappers-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/PKG-INFO` & `ml_wrappers-0.4.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_wrappers
-Version: 0.4.6
+Version: 0.4.7
 Summary: Machine Learning Wrappers SDK for Python
 Home-page: https://github.com/microsoft/ml-wrappers
 Author: Microsoft Corp
 Author-email: ilmat@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_wrappers-0.4.6/README.md` & `ml_wrappers-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/__init__.py` & `ml_wrappers-0.4.7/ml_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/common/constants.py` & `ml_wrappers-0.4.7/ml_wrappers/common/constants.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/common/gpu_kmeans.py` & `ml_wrappers-0.4.7/ml_wrappers/common/gpu_kmeans.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/common/warnings_suppressor.py` & `ml_wrappers-0.4.7/ml_wrappers/common/warnings_suppressor.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/dataset/dataset_utils.py` & `ml_wrappers-0.4.7/ml_wrappers/dataset/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/dataset/dataset_wrapper.py` & `ml_wrappers-0.4.7/ml_wrappers/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/dataset/timestamp_featurizer.py` & `ml_wrappers-0.4.7/ml_wrappers/dataset/timestamp_featurizer.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/__init__.py` & `ml_wrappers-0.4.7/ml_wrappers/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/base_wrapped_model.py` & `ml_wrappers-0.4.7/ml_wrappers/model/base_wrapped_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/endpoint_wrapper.py` & `ml_wrappers-0.4.7/ml_wrappers/model/endpoint_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/evaluator.py` & `ml_wrappers-0.4.7/ml_wrappers/model/evaluator.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/fastai_wrapper.py` & `ml_wrappers-0.4.7/ml_wrappers/model/fastai_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/function_wrapper.py` & `ml_wrappers-0.4.7/ml_wrappers/model/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/image_model_wrapper.py` & `ml_wrappers-0.4.7/ml_wrappers/model/image_model_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """Defines wrappers for vision-based models."""
 
 import logging
-from typing import Any
+from typing import Any, Dict, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from ml_wrappers.common.constants import ModelTask
 from ml_wrappers.dataset.dataset_wrapper import DatasetWrapper
 from ml_wrappers.model.evaluator import _eval_model
 from ml_wrappers.model.pytorch_wrapper import WrappedPytorchModel
@@ -21,38 +21,38 @@
 
 try:
     import torch
     import torch.nn as nn
     from torch import Tensor
 except ImportError:
     Tensor = Any
-    module_logger.debug('Could not import torch, required if using a' +
+    module_logger.debug('Could not import torch, required if using a ' +
                         'PyTorch model')
 
 try:
     from vision_explanation_methods.explanations import common as od_common
     from vision_explanation_methods.explanations.common import \
         GeneralObjectDetectionModelWrapper
 except ImportError:
     GeneralObjectDetectionModelWrapper = object
-    module_logger.debug('Could not import vision_explanation_methods,' +
+    module_logger.debug('Could not import vision_explanation_methods, ' +
                         'required if using PytorchDRiseWrapper')
 
 try:
     import torchvision
     from torchvision import transforms as T
 except ImportError:
-    module_logger.debug('Could not import torchvision, required if' +
+    module_logger.debug('Could not import torchvision, required if ' +
                         'using PytorchDRiseWrapper')
 
 try:
     from mlflow.pyfunc import PyFuncModel
 except ImportError:
     PyFuncModel = Any
-    module_logger.debug('Could not import mlflow, required if using an' +
+    module_logger.debug('Could not import mlflow, required if using an ' +
                         'mlflow model')
 
 FASTAI_MODEL_SUFFIX = "fastai.learner.Learner'>"
 BOXES = 'boxes'
 LABELS = 'labels'
 SCORES = 'scores'
 
@@ -104,68 +104,159 @@
     nms_prediction = orig_prediction
     nms_prediction[BOXES] = nms_prediction[BOXES][keep]
     nms_prediction[SCORES] = nms_prediction[SCORES][keep]
     nms_prediction[LABELS] = nms_prediction[LABELS][keep]
     return nms_prediction
 
 
-def _wrap_image_model(model, examples, model_task, is_function, number_of_classes=None):
+def _process_automl_detections_to_raw_detections(
+        image_detections,
+        label_dict: Dict[str, int],
+        image_size: Tuple[int, int]) -> Dict[str, Tensor]:
+    """Process AutoML mlflow object detections from a single image.
+
+    The length of image_detections list will be equal to the number
+    of objects the AutoML MLflow model detected in a single image.
+    Below is an example of image_detections when the model detected
+    two objects:
+
+    [{'box': {'topX': 0.645,
+              'topY': 0.373,
+              'bottomX': 0.8276,
+              'bottomY': 0.6102
+                },
+      'label': 'can',
+      'score': 0.945},
+     {'box': {'topX': 0.324,
+              'topY': 0.5643,
+              'bottomX': 0.6511,
+              'bottomY': 0.865
+                },
+      'label': 'milk_bottle',
+      'score': 0.93}
+    ]
+    The bbox coordinates need to be scaled by the image dimensions.
+
+    :param image_detections: AutoML mlflow detections
+    :type image_detections: list
+    :param label_dict: Label dictionary mapping class names to an index
+    :type label_dict: dict
+    :param image_size: Image size
+    :type image_size: tuple(int, int)
+    :return: Raw detections
+    :rtype: dict
+    """
+
+    x, y = image_size
+
+    boxes = []
+    scores = []
+    labels = []
+    for detection in image_detections:
+        # predicted class label
+        label = detection['label']
+        # confidence score from model
+        score = detection['score']
+        # predicted bbox coordinates
+        box = detection["box"]
+
+        ymin, xmin, ymax, xmax = (
+            box["topY"], box["topX"], box["bottomY"], box["bottomX"])
+
+        # the automl mlflow model generates normalized bbox coordinates
+        # they need to be scaled by the size of the image
+        x_min_scaled, y_min_scaled = x * xmin, y * ymin
+        x_max_scaled, y_max_scaled = x * xmax, y * ymax
+
+        scores.append(score)
+        labels.append(label)
+        boxes.append([x_min_scaled, y_min_scaled, x_max_scaled, y_max_scaled])
+    try:
+        labels = [int(x) for x in labels]
+    except BaseException:
+        labels = [label_dict[x] for x in labels]
+
+    return {
+        "boxes": Tensor(boxes),
+        "labels": Tensor(labels),
+        "scores": Tensor(scores)}
+
+
+def _wrap_image_model(model, examples, model_task, is_function,
+                      number_of_classes: int = None,
+                      classes: Union[list, np.array] = None):
     """If needed, wraps the model or function in a common API.
 
     Wraps the model based on model task and prediction function contract.
 
     :param model: The model or function to evaluate on the examples.
     :type model: function or model to wrap
     :param examples: The model evaluation examples.
-    :type examples: ml_wrappers.DatasetWrapper or numpy.ndarray
-        or pandas.DataFrame or panads.Series or scipy.sparse.csr_matrix
-        or shap.DenseData or torch.Tensor
+    :type examples: ml_wrappers.DatasetWrapper
+    or numpy.ndarray or pandas.DataFrame or panads.Series
+    or scipy.sparse.csr_matrix or shap.DenseData
+    or torch.Tensor.
     :param model_task: Parameter to specify whether the model is an
-        'image_classification' or another type of image model.
+    'image_classification' or another type of image model.
     :type model_task: str
-    :param number_of_classes: optional parameter specifying the number of classes in
-        the dataset
+    :param classes: optional parameter specifying a list of class names
+    the dataset
+    :type classes: list or np.ndarray
+    :param number_of_classes: optional parameter specifying the
+    number of classes in the dataset
     :type number_of_classes: int
     :return: The function chosen from given model and chosen domain, or
-        model wrapping the function and chosen domain.
+    model wrapping the function and chosen domain.
     :rtype: (function, str) or (model, str)
     """
     _wrapped_model = model
     if model_task == ModelTask.IMAGE_CLASSIFICATION:
         try:
             if isinstance(model, nn.Module):
                 model = WrappedPytorchModel(model, image_to_tensor=True)
                 if not isinstance(examples, DatasetWrapper):
                     examples = DatasetWrapper(examples)
-                eval_function, eval_ml_domain = _eval_model(model, examples, model_task)
+                eval_function, eval_ml_domain = _eval_model(
+                    model, examples, model_task)
                 return (
                     WrappedClassificationModel(model, eval_function, examples),
                     eval_ml_domain,
                 )
         except (NameError, AttributeError):
             module_logger.debug(
                 'Could not import torch, required if using a pytorch model'
             )
 
         if _is_fastai_model(model):
             _wrapped_model = WrappedFastAIImageClassificationModel(model)
         elif hasattr(model, '_model_impl'):
             if str(type(model._model_impl.python_model)).endswith(
-                "azureml.automl.dnn.vision.common.mlflow.mlflow_model_wrapper.MLFlowImagesModelWrapper'>"
+                ("azureml.automl.dnn.vision.common.mlflow." +
+                    "mlflow_model_wrapper.MLFlowImagesModelWrapper'>")
             ):
-                _wrapped_model = WrappedMlflowAutomlImagesClassificationModel(model)
+                _wrapped_model = WrappedMlflowAutomlImagesClassificationModel(
+                    model)
         else:
             _wrapped_model = WrappedTransformerImageClassificationModel(model)
     elif model_task == ModelTask.MULTILABEL_IMAGE_CLASSIFICATION:
         if _is_fastai_model(model):
             _wrapped_model = WrappedFastAIImageClassificationModel(
                 model, multilabel=True
             )
     elif model_task == ModelTask.OBJECT_DETECTION:
-        _wrapped_model = WrappedObjectDetectionModel(model, number_of_classes)
+        if hasattr(model, '_model_impl'):
+            if str(type(model._model_impl.python_model)).endswith(
+                ("azureml.automl.dnn.vision.common.mlflow." +
+                    "mlflow_model_wrapper.MLFlowImagesModelWrapper'>")
+            ):
+                _wrapped_model = WrappedMlflowAutomlObjectDetectionModel(
+                    model, classes)
+        else:
+            _wrapped_model = WrappedObjectDetectionModel(
+                model, number_of_classes)
     return _wrapped_model, model_task
 
 
 class WrappedTransformerImageClassificationModel(object):
     """A class for wrapping a Transformers model in the scikit-learn style."""
 
     def __init__(self, model):
@@ -256,15 +347,16 @@
         :return: The predicted probabilities.
         :rtype: numpy.ndarray
         """
         return self._fastai_predict(dataset, 2)
 
 
 class WrappedMlflowAutomlImagesClassificationModel:
-    """A class for wrapping an AutoML for images MLflow model in the scikit-learn style."""
+    """A class for wrapping an AutoML for images MLflow classification
+        model in the scikit-learn style."""
 
     def __init__(self, model: PyFuncModel) -> None:
         """Initialize the WrappedMlflowAutomlImagesClassificationModel.
 
         :param model: mlflow model
         :type model: mlflow.pyfunc.PyFuncModel
         """
@@ -301,25 +393,28 @@
         :rtype: numpy.ndarray
         """
         predictions = self._mlflow_predict(dataset)
         return np.stack(predictions.probs.values)
 
 
 class WrappedObjectDetectionModel:
-    """A class for wrapping a object detection model in the scikit-learn style."""
+    """A class for wrapping a object detection model in the scikit-learn
+        style."""
 
     def __init__(self, model: Any, number_of_classes: int) -> None:
-        """Initialize the WrappedObjectDetectionModel with the model and evaluation function.
+        """Initialize the WrappedObjectDetectionModel with the model
+            and evaluation function.
 
         :param model: mlflow model
         :type model: Any
         """
         self._device = torch.device("cuda" if torch.cuda.is_available()
                                     else "cpu")
         model.eval()
+        model.to(self._device)
         self._model = model
         self._number_of_classes = number_of_classes
 
     def predict(self, x, iou_thresh: float = 0.5, score_thresh: float = 0.5):
         """Create a list of detection records from the image predictions.
 
         :param x: Tensor of the image
@@ -351,15 +446,15 @@
                 raw_detections = self._model(
                     image.to(self._device).unsqueeze(0))
             else:
                 raw_detections = self._model(
                     T.ToTensor()(image).to(self._device).unsqueeze(0))
 
             for raw_detection in raw_detections:
-                raw_detection = _apply_nms(raw_detection)
+                raw_detection = _apply_nms(raw_detection, .5)
                 raw_detection = _filter_score(raw_detection)
                 image_predictions = torch.cat((raw_detection["labels"]
                                                .unsqueeze(1),
                                                raw_detection["boxes"],
                                                raw_detection["scores"]
                                                .unsqueeze(1)), dim=1)
 
@@ -368,20 +463,134 @@
         return detections
 
     def predict_proba(self, dataset, iou_threshold=0.1):
         """Predict the output probability using the wrapped model.
 
         :param dataset: The dataset to predict_proba on.
         :type dataset: ml_wrappers.DatasetWrapper
-        param iou_threshold: amount of acceptable error.
+        :param iou_threshold: amount of acceptable error.
             objects with error scores higher than the threshold will be removed
-        type iou_threshold: float
+        :type iou_threshold: float
         """
         predictions = self.predict(dataset, iou_threshold)
-        prob_scores = [[pred.class_scores for pred in image_prediction] for image_prediction in predictions]
+        prob_scores = [[pred.class_scores for pred in image_prediction]
+                       for image_prediction in predictions]
+        return prob_scores
+
+
+class WrappedMlflowAutomlObjectDetectionModel:
+    """A class for wrapping an AutoML for images MLflow object detection model
+        in the scikit-learn style."""
+
+    def __init__(self, model: PyFuncModel,
+                 classes: Union[list, np.array]) -> None:
+        """Initialize the WrappedMlflowAutomlObjectDetectionModel.
+
+        :param model: mlflow model
+        :type model: mlflow.pyfunc.PyFuncModel
+        :param classes: list of class names
+        :type classes: list or np.array
+        """
+
+        self._model = model
+        self._classes = classes
+        self._label_dict = {label: (i+1) for i, label in enumerate(classes)}
+
+    def _mlflow_predict(self, dataset: pd.DataFrame) -> pd.DataFrame:
+        """Perform the inference using the wrapped MLflow model.
+
+        :param dataset: The dataset to predict on.
+        :type dataset: pandas.DataFrame
+        :return: The predicted data.
+        :rtype: pandas.DataFrame
+        """
+
+        predictions = self._model.predict(dataset)
+        return predictions
+
+    def predict(self, dataset: pd.DataFrame, iou_thresh: float = 0.5,
+                score_thresh: float = 0.5):
+        """Create a list of detection records from the image predictions.
+
+        Below is example Label (y) representation for a cohort of 2 images,
+        with 3 objects detected for the first image and 1 for the second image.
+
+        [
+         [
+            [class, topX, topY, bottomX, bottomY, (optional) confidence_score],
+            [class, topX, topY, bottomX, bottomY, (optional) confidence_score],
+            [class, topX, topY, bottomX, bottomY, (optional) confidence_score],
+         ],
+         [
+            [class, topX, topY, bottomX, bottomY, (optional) confidence_score],
+         ]
+
+        ]
+
+        :param dataset: The dataset to predict on.
+        :type dataset: pandas.DataFrame
+        :param iou_thresh: Intersection-over-Union (IoU) threshold for NMS (or
+                           the amount of acceptable error). Objects with error
+                           cores higher than the threshold will be removed.
+        :type iou_thresh: float
+        :param score_thresh: Threshold to filter detections based on
+                            predicted confidence scores.
+        :type score_thresh: float
+        :return: Final detections from the object detector
+        :rtype: List of Detection Records
+        """
+        image_sizes = dataset['image_size']
+
+        dataset = dataset.drop(['image_size'], axis=1)
+
+        predictions = self._mlflow_predict(dataset)
+        if not len(predictions['boxes']) == len(image_sizes):
+            raise ValueError("Internal Error: Number of predictions " +
+                             "does not match number of images")
+
+        detections = []
+        for image_detections, img_size in \
+                zip(predictions['boxes'], image_sizes):
+
+            # process automl mlflow detection outputs
+            raw_detections = _process_automl_detections_to_raw_detections(
+                image_detections, self._label_dict, img_size)
+
+            raw_detections = _apply_nms(raw_detections, iou_thresh)
+            raw_detections = _filter_score(raw_detections, score_thresh)
+
+            image_predictions = torch.cat((
+                raw_detections["labels"].unsqueeze(1),
+                raw_detections["boxes"],
+                raw_detections["scores"].unsqueeze(1)
+            ),
+                dim=1
+            )
+
+            detections.append(
+                image_predictions.detach().cpu().numpy().tolist())
+
+        return detections
+
+    def predict_proba(self, dataset: pd.DataFrame,
+                      iou_thresh=0.1) -> np.ndarray:
+        """Predict the output probability using the MLflow model.
+
+        :param dataset: The dataset to predict_proba on.
+        :type dataset: pandas.DataFrame
+        :param iou_thresh: amount of acceptable error.
+            objects with error scores higher than the threshold will be removed
+        :type iou_thresh: float
+        :return: The predicted probabilities.
+        :rtype: numpy.ndarray
+        """
+
+        predictions = self.predict(dataset, iou_thresh=iou_thresh)
+        prob_scores = [[pred[-1] for pred in image_prediction]
+                       for image_prediction in predictions]
         return prob_scores
 
 
 class PytorchDRiseWrapper(GeneralObjectDetectionModelWrapper):
     """Wraps a PytorchFasterRCNN model with a predict API function.
 
     To be compatible with the D-RISE explainability method,
@@ -395,14 +604,16 @@
         """Initialize the PytorchDRiseWrapper.
 
         :param model: Object detection model
         :type model: PytorchFasterRCNN model
         :param number_of_classes: Number of classes the model is predicting
         :type number_of_classes: int
         """
+        device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+        model.to(device)
         model.eval()
         self._model = model
         self._number_of_classes = number_of_classes
 
     def predict(self, x: Tensor):
         """Create a list of detection records from the image predictions.
 
@@ -411,15 +622,15 @@
         :return: Baseline detections to get saliency maps for
         :rtype: List of Detection Records
         """
         raw_detections = self._model(x)
 
         detections = []
         for raw_detection in raw_detections:
-            raw_detection = _apply_nms(raw_detection, 0.005)
+            raw_detection = _apply_nms(raw_detection, 0.5)
 
             # Note that FasterRCNN doesn't return a score for each class, only
             # the predicted class. DRISE requires a score for each class.
             # We approximate the score for each class
             # by dividing (class score) evenly among the other classes.
 
             raw_detection = _filter_score(raw_detection, 0.5)
@@ -432,8 +643,9 @@
                 od_common.DetectionRecord(
                     bounding_boxes=raw_detection[BOXES],
                     class_scores=expanded_class_scores,
                     objectness_scores=torch.tensor(
                         [1.0]*raw_detection[BOXES].shape[0]),
                 )
             )
+
         return detections
```

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/model_utils.py` & `ml_wrappers-0.4.7/ml_wrappers/model/model_utils.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/model_wrapper.py` & `ml_wrappers-0.4.7/ml_wrappers/model/model_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
-"""Defines helpful model wrapper and utils for implicitly rewrapping the model to conform to explainer contracts."""
+"""Defines helpful model wrapper and utils for implicitly rewrapping the model
+    to conform to explainer contracts."""
 
 import logging
 import warnings
+from typing import Union
 
+import numpy as np
 from ml_wrappers.model.wrapped_classification_model import \
     WrappedClassificationModel
 from ml_wrappers.model.wrapped_classification_without_proba_model import \
     WrappedClassificationWithoutProbaModel
 from ml_wrappers.model.wrapped_regression_model import WrappedRegressionModel
 from sklearn.linear_model import SGDClassifier
 
@@ -21,106 +24,131 @@
 from .fastai_wrapper import WrappedFastAITabularModel, _is_fastai_tabular_model
 from .image_model_wrapper import _wrap_image_model
 from .pytorch_wrapper import WrappedPytorchModel
 from .tensorflow_wrapper import WrappedTensorflowModel, is_sequential
 from .text_model_wrapper import _is_transformers_pipeline, _wrap_text_model
 
 with warnings.catch_warnings():
-    warnings.filterwarnings('ignore', 'Starting from version 2.2.1', UserWarning)
+    warnings.filterwarnings(
+        'ignore', 'Starting from version 2.2.1', UserWarning)
 
 
 module_logger = logging.getLogger(__name__)
 module_logger.setLevel(logging.INFO)
 
 
 try:
     import torch.nn as nn
 except ImportError:
-    module_logger.debug('Could not import torch, required if using a PyTorch model')
+    module_logger.debug(
+        'Could not import torch, required if using a PyTorch model')
 
 
-def wrap_model(model, examples, model_task=ModelTask.UNKNOWN, num_classes=None):
-    """If needed, wraps the model in a common API based on model task and prediction function contract.
+def wrap_model(model, examples, model_task: str = ModelTask.UNKNOWN,
+               num_classes: int = None, classes: Union[list, np.array] = None):
+    """If needed, wraps the model in a common API based on model task and
+        prediction function contract.
 
     :param model: The model to evaluate on the examples.
     :type model: model with a predict or predict_proba function.
     :param examples: The model evaluation examples.
         Note the examples will be wrapped in a DatasetWrapper, if not
         wrapped when input.
     :type examples: ml_wrappers.DatasetWrapper or numpy.ndarray
         or pandas.DataFrame or panads.Series or scipy.sparse.csr_matrix
         or shap.DenseData or torch.Tensor
-    :param model_task: Optional parameter to specify whether the model is a classification or regression model.
-        In most cases, the type of the model can be inferred based on the shape of the output, where a classifier
-        has a predict_proba method and outputs a 2 dimensional array, while a regressor has a predict method and
-        outputs a 1 dimensional array.
+    :param model_task: Optional parameter to specify whether the model
+                       is a classification or regression model.
+                       In most cases, the type of the model can be inferred
+                       based on the shape of the output, where a classifier
+                       has a predict_proba method and outputs a 2 dimensional
+                       array, while a regressor has a predict method and
+                       outputs a 1 dimensional array.
+    :param classes: optional parameter specifying a list of class names
+        the dataset
+    :type classes: list or np.ndarray
     :param num_classes: optional parameter specifying the number of classes in
         the dataset
     :type num_classes: int
     :type model_task: str
     :return: The wrapper model.
     :rtype: model
     """
     if model_task == ModelTask.UNKNOWN and _is_transformers_pipeline(model):
         # TODO: can we also dynamically figure out the task if it was
         # originally unknown for text scenarios?
         raise ValueError("ModelTask must be specified for text-based models")
     if model_task in text_model_tasks:
         return _wrap_text_model(model, examples, model_task, False)[0]
     if model_task in image_model_tasks:
-        return _wrap_image_model(model, examples, model_task, False, num_classes)[0]
+        return _wrap_image_model(model, examples, model_task,
+                                 False,  num_classes, classes)[0]
     return _wrap_model(model, examples, model_task, False)[0]
 
 
 def _wrap_model(model, examples, model_task, is_function):
-    """If needed, wraps the model or function in a common API based on model task and prediction function contract.
+    """If needed, wraps the model or function in a common API based on model
+        task and prediction function contract.
 
     :param model: The model or function to evaluate on the examples.
     :type model: function or model with a predict or predict_proba function
     :param examples: The model evaluation examples.
         Note the examples will be wrapped in a DatasetWrapper, if not
         wrapped when input.
     :type examples: ml_wrappers.DatasetWrapper or numpy.ndarray
         or pandas.DataFrame or panads.Series or scipy.sparse.csr_matrix
         or shap.DenseData or torch.Tensor
-    :param model_task: Optional parameter to specify whether the model is a classification or regression model.
-        In most cases, the type of the model can be inferred based on the shape of the output, where a classifier
-        has a predict_proba method and outputs a 2 dimensional array, while a regressor has a predict method and
-        outputs a 1 dimensional array.
+    :param model_task: Optional parameter to specify whether the model
+                       is a classification or regression model.
+                       In most cases, the type of the model can be inferred
+                       based on the shape of the output, where a classifier
+                       has a predict_proba method and outputs a 2 dimensional
+                       array, while a regressor has a predict method and
+                       outputs a 1 dimensional array.
     :type model_task: str
-    :return: The function chosen from given model and chosen domain, or model wrapping the function and chosen domain.
+    :return: The function chosen from given model and chosen domain, or
+             model wrapping the function and chosen domain.
     :rtype: (function, str) or (model, str)
     """
     if not isinstance(examples, DatasetWrapper):
         examples = DatasetWrapper(examples)
     if is_function:
         return _eval_function(model, examples, model_task)
     else:
         try:
             if isinstance(model, nn.Module):
-                # Wrap the model in an extra layer that converts the numpy array
-                # to pytorch Variable and adds predict and predict_proba functions
+                # Wrap the model in an extra layer that
+                # converts the numpy array
+
+                # to pytorch Variable and adds predict and
+                # predict_proba functions
                 model = WrappedPytorchModel(model)
         except (NameError, AttributeError):
-            module_logger.debug('Could not import torch, required if using a pytorch model')
+            module_logger.debug(
+                'Could not import torch, required if using a pytorch model')
         if _is_fastai_tabular_model(model):
             model = WrappedFastAITabularModel(model)
         if is_sequential(model):
             model = WrappedTensorflowModel(model)
         if _classifier_without_proba(model):
             model = WrappedClassificationWithoutProbaModel(model)
-        eval_function, eval_ml_domain = _eval_model(model, examples, model_task)
+        eval_function, eval_ml_domain = _eval_model(
+            model, examples, model_task)
         if eval_ml_domain == ModelTask.CLASSIFICATION:
-            return WrappedClassificationModel(model, eval_function, examples), eval_ml_domain
+            return WrappedClassificationModel(model, eval_function, examples),\
+                eval_ml_domain
         else:
-            return WrappedRegressionModel(model, eval_function, examples), eval_ml_domain
+            return WrappedRegressionModel(model, eval_function, examples), \
+                eval_ml_domain
 
 
 def _classifier_without_proba(model):
-    """Returns True if the given model is a classifier without predict_proba, eg SGDClassifier.
+    """Returns True if the given model is a classifier without predict_proba,
+        eg SGDClassifier.
 
     :param model: The model to evaluate on the examples.
     :type model: model with a predict or predict_proba function
     :return: True if the given model is a classifier without predict_proba.
     :rtype: bool
     """
-    return isinstance(model, SGDClassifier) and not hasattr(model, SKLearn.PREDICT_PROBA)
+    return isinstance(model, SGDClassifier) and not \
+        hasattr(model, SKLearn.PREDICT_PROBA)
```

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/predictions_wrapper.py` & `ml_wrappers-0.4.7/ml_wrappers/model/predictions_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         :param query_test_data_row: The query data instance.
         :type query_test_data_row: pd.DataFrame
         :return: The filtered dataframe based on the values in query data.
         :rtype: pd.DataFrame
         """
         queries = []
-        for column_name, column_data in query_test_data_row.squeeze().iteritems():
+        for column_name, column_data in query_test_data_row.squeeze().items():
             if isinstance(column_data, str):
                 queries.append("`{}` == '{}'".format(
                     column_name, column_data))
             else:
                 queries.append("`{}` == {}".format(
                     column_name, column_data))
```

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/pytorch_wrapper.py` & `ml_wrappers-0.4.7/ml_wrappers/model/pytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/tensorflow_wrapper.py` & `ml_wrappers-0.4.7/ml_wrappers/model/tensorflow_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/text_model_wrapper.py` & `ml_wrappers-0.4.7/ml_wrappers/model/text_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/wrapped_classification_model.py` & `ml_wrappers-0.4.7/ml_wrappers/model/wrapped_classification_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/wrapped_classification_without_proba_model.py` & `ml_wrappers-0.4.7/ml_wrappers/model/wrapped_classification_without_proba_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers/model/wrapped_regression_model.py` & `ml_wrappers-0.4.7/ml_wrappers/model/wrapped_regression_model.py`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/ml_wrappers.egg-info/PKG-INFO` & `ml_wrappers-0.4.7/ml_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-wrappers
-Version: 0.4.6
+Version: 0.4.7
 Summary: Machine Learning Wrappers SDK for Python
 Home-page: https://github.com/microsoft/ml-wrappers
 Author: Microsoft Corp
 Author-email: ilmat@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_wrappers-0.4.6/ml_wrappers.egg-info/SOURCES.txt` & `ml_wrappers-0.4.7/ml_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_wrappers-0.4.6/setup.py` & `ml_wrappers-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     'Operating System :: Microsoft :: Windows',
     'Operating System :: MacOS',
     'Operating System :: POSIX :: Linux'
 ]
 
 DEPENDENCIES = [
     'numpy',
-    'pandas',
+    'pandas<2.0.0',
     'scipy',
     'scikit-learn'
 ]
 
 with open(README_FILE, 'r', encoding='utf-8') as f:
     README = f.read()
```

