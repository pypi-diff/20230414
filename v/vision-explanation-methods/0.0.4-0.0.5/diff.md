# Comparing `tmp/vision_explanation_methods-0.0.4.tar.gz` & `tmp/vision_explanation_methods-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_explanation_methods-0.0.4.tar", last modified: Tue Mar 28 16:19:40 2023, max compression
+gzip compressed data, was "vision_explanation_methods-0.0.5.tar", last modified: Fri Apr 14 18:36:27 2023, max compression
```

## Comparing `vision_explanation_methods-0.0.4.tar` & `vision_explanation_methods-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:19:40.807526 vision_explanation_methods-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-28 16:19:40.000000 vision_explanation_methods-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-03-28 16:19:40.807526 vision_explanation_methods-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-28 16:04:25.000000 vision_explanation_methods-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 16:19:40.807526 vision_explanation_methods-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-28 16:04:25.000000 vision_explanation_methods-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:19:40.807526 vision_explanation_methods-0.0.4/vision_explanation_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-03-28 16:04:25.000000 vision_explanation_methods-0.0.4/vision_explanation_methods/DRISE_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-28 16:04:25.000000 vision_explanation_methods-0.0.4/vision_explanation_methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:19:40.807526 vision_explanation_methods-0.0.4/vision_explanation_methods/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-28 16:04:25.000000 vision_explanation_methods-0.0.4/vision_explanation_methods/explanations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-03-28 16:04:25.000000 vision_explanation_methods-0.0.4/vision_explanation_methods/explanations/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-03-28 16:04:25.000000 vision_explanation_methods-0.0.4/vision_explanation_methods/explanations/drise.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-28 16:04:25.000000 vision_explanation_methods-0.0.4/vision_explanation_methods/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:19:40.807526 vision_explanation_methods-0.0.4/vision_explanation_methods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-03-28 16:19:40.000000 vision_explanation_methods-0.0.4/vision_explanation_methods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-28 16:19:40.000000 vision_explanation_methods-0.0.4/vision_explanation_methods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 16:19:40.000000 vision_explanation_methods-0.0.4/vision_explanation_methods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 16:19:40.000000 vision_explanation_methods-0.0.4/vision_explanation_methods.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-28 16:19:40.000000 vision_explanation_methods-0.0.4/vision_explanation_methods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-28 16:19:40.000000 vision_explanation_methods-0.0.4/vision_explanation_methods.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:36:27.621512 vision_explanation_methods-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-14 18:36:27.617512 vision_explanation_methods-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:36:27.621512 vision_explanation_methods-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:36:27.617512 vision_explanation_methods-0.0.5/vision_explanation_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/DRISE_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:36:27.617512 vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/drise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-14 18:21:04.000000 vision_explanation_methods-0.0.5/vision_explanation_methods/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:36:27.617512 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 18:36:27.000000 vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/top_level.txt
```

### Comparing `vision_explanation_methods-0.0.4/LICENSE.txt` & `vision_explanation_methods-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.4/PKG-INFO` & `vision_explanation_methods-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_explanation_methods
-Version: 0.0.4
+Version: 0.0.5
 Summary: Microsoft Vision Explanation Methods SDK for Python
 Home-page: https://github.com/microsoft/vision-explanation-methods
 Author: Microsoft Corp
 Author-email: jamhall@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vision_explanation_methods-0.0.4/README.md` & `vision_explanation_methods-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.4/setup.py` & `vision_explanation_methods-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.4/vision_explanation_methods/DRISE_runner.py` & `vision_explanation_methods-0.0.5/vision_explanation_methods/DRISE_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Method for generating saliency maps for object detection models."""
 
-import os
+from io import BytesIO
 from typing import Optional, Tuple
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy
+import requests
 import torch
 import torchvision
 from captum.attr import visualization as viz
 from ml_wrappers.model.image_model_wrapper import PytorchDRiseWrapper
 from PIL import Image
 from torchvision import transforms as T
 from torchvision.models import detection
@@ -117,23 +118,29 @@
 
     if not model:
         unwrapped_model = detection.fasterrcnn_resnet50_fpn(
             pretrained=True, map_location=device)
         unwrapped_model.to(device)
         model = PytorchDRiseWrapper(unwrapped_model, numclasses)
 
-    test_image = Image.open(imagelocation).convert('RGB')
+    image_open_pointer = imagelocation
+    if (imagelocation.startswith("http://")
+       or imagelocation.startswith("https://")):
+        response = requests.get(imagelocation)
+        image_open_pointer = BytesIO(response.content)
+
+    test_image = Image.open(image_open_pointer).convert('RGB')
 
     detections = model.predict(
-        T.ToTensor()(test_image).unsqueeze(0).repeat(2, 1, 1, 1).to(device))
+        T.ToTensor()(test_image).unsqueeze(0).to(device))
 
     saliency_scores = drise.DRISE_saliency(
         model=model,
         # Repeated the tensor to test batching
-        image_tensor=T.ToTensor()(test_image).repeat(2, 1, 1, 1).to(device),
+        image_tensor=T.ToTensor()(test_image).unsqueeze(0).to(device),
         target_detections=detections,
         # This is how many masks to run -
         # more is slower but gives higher quality mask.
         number_of_masks=nummasks,
         mask_padding=maskpadding,
         device=device,
         # This is the resolution of the random masks.
@@ -149,18 +156,17 @@
                        for i in range(len(saliency_scores[img_index]))
                        if not torch.isnan(
                        saliency_scores[img_index][i]['detection']).any()]
 
     num_detections = len(saliency_scores)
 
     if num_detections == 0:  # If no objects have been detected...
-        fail = Image.open(os.path.join("python", "vision_explanation_methods",
-                                       "images", "notfound.jpg"))
+        fail = Image.new('RGB', (100, 100))
         fail = fail.save(savename)
-        return None, None
+        return None, None, None
 
     label_list = []
     fig_list = []
     for i in range((max_figures if num_detections > max_figures
                     else num_detections)):
         fig, ax = plt.subplots(1, 1, figsize=(10, 10))
         label = int(torch.argmax(detections[img_index].class_scores[i]))
```

### Comparing `vision_explanation_methods-0.0.4/vision_explanation_methods/explanations/common.py` & `vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/common.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.4/vision_explanation_methods/explanations/drise.py` & `vision_explanation_methods-0.0.5/vision_explanation_methods/explanations/drise.py`

 * *Files identical despite different names*

### Comparing `vision_explanation_methods-0.0.4/vision_explanation_methods.egg-info/PKG-INFO` & `vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-explanation-methods
-Version: 0.0.4
+Version: 0.0.5
 Summary: Microsoft Vision Explanation Methods SDK for Python
 Home-page: https://github.com/microsoft/vision-explanation-methods
 Author: Microsoft Corp
 Author-email: jamhall@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vision_explanation_methods-0.0.4/vision_explanation_methods.egg-info/SOURCES.txt` & `vision_explanation_methods-0.0.5/vision_explanation_methods.egg-info/SOURCES.txt`

 * *Files identical despite different names*

