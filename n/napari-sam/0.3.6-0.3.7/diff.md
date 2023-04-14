# Comparing `tmp/napari-sam-0.3.6.tar.gz` & `tmp/napari-sam-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.3.6.tar", last modified: Thu Apr 13 19:56:14 2023, max compression
+gzip compressed data, was "napari-sam-0.3.7.tar", last modified: Fri Apr 14 17:31:26 2023, max compression
```

## Comparing `napari-sam-0.3.6.tar` & `napari-sam-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:56:14.912959 napari-sam-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-13 19:55:57.000000 napari-sam-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 19:55:57.000000 napari-sam-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 19:56:14.912959 napari-sam-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-13 19:55:57.000000 napari-sam-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 19:55:57.000000 napari-sam-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 19:56:14.916959 napari-sam-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:56:14.912959 napari-sam-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:56:14.912959 napari-sam-0.3.6/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 19:55:57.000000 napari-sam-0.3.6/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39447 2023-04-13 19:55:57.000000 napari-sam-0.3.6/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 19:55:57.000000 napari-sam-0.3.6/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-13 19:55:57.000000 napari-sam-0.3.6/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:56:14.912959 napari-sam-0.3.6/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 19:56:14.000000 napari-sam-0.3.6/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:31:26.302404 napari-sam-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 17:31:10.000000 napari-sam-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 17:31:10.000000 napari-sam-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-14 17:31:26.302404 napari-sam-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-14 17:31:10.000000 napari-sam-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 17:31:10.000000 napari-sam-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-14 17:31:26.302404 napari-sam-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:31:26.298404 napari-sam-0.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:31:26.302404 napari-sam-0.3.7/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 17:31:10.000000 napari-sam-0.3.7/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39447 2023-04-14 17:31:10.000000 napari-sam-0.3.7/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-14 17:31:10.000000 napari-sam-0.3.7/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-14 17:31:10.000000 napari-sam-0.3.7/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:31:26.302404 napari-sam-0.3.7/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 17:31:26.000000 napari-sam-0.3.7/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.3.6/LICENSE` & `napari-sam-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.6/PKG-INFO` & `napari-sam-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.6
+Version: 0.3.7
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.6 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.7 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

### Comparing `napari-sam-0.3.6/README.md` & `napari-sam-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.6/setup.cfg` & `napari-sam-0.3.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.6/src/napari_sam/_widget.py` & `napari-sam-0.3.7/src/napari_sam/_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
 
                 self.viewer.mouse_drag_callbacks.append(self.callback_click)
                 self.viewer.keymap['Delete'] = self.on_delete
                 self.label_layer.keymap['Control-Z'] = self.on_undo
                 self.label_layer.keymap['Control-Shift-Z'] = self.on_redo
 
             elif self.annotator_mode == AnnotatorMode.AUTO:
-                image = self.image_layer.data
+                image = np.asarray(self.image_layer.data)
                 if not self.image_layer.rgb:
                     image = np.stack((image,)*3, axis=-1)  # Expand to 3-channel image
                 image = image[..., :3]  # Remove a potential alpha channel
                 records = self.sam_anything_predictor.generate(image)
                 masks = np.asarray([record["segmentation"] for record in records])
                 prediction = np.argmax(masks, axis=0)
                 self.label_layer.data = prediction
@@ -500,15 +500,15 @@
         self.label_layer.data = self.label_layer.data
 
     def on_contrast_limits_change(self):
         print("Contrast limit change")
         self.set_image()
 
     def set_image(self):
-        image = self.image_layer.data
+        image = np.asarray(self.image_layer.data)
         if self.image_layer.ndim == 2:
             if not self.image_layer.rgb:
                 image = np.stack((image,)*3, axis=-1)  # Expand to 3-channel image
             image = image[..., :3]  # Remove a potential alpha channel
             self.sam_predictor.set_image(image)
             self.sam_features = self.sam_predictor.features
         elif self.image_layer.ndim == 3:
@@ -561,24 +561,25 @@
                 labels_flattended.extend(labels)
 
             prediction, predicted_slices = self.predict(points_flattened, labels_flattended)
         else:
             prediction = np.zeros_like(self.label_layer.data)
             predicted_slices = slice(None, None)
 
+        label_layer = np.asarray(self.label_layer.data)
         changed_indices = np.where(prediction == 1)
-        index_labels_old = self.label_layer.data[changed_indices]
-        self.label_layer.data[predicted_slices][self.label_layer.data[predicted_slices] == point_label] = 0
+        index_labels_old = label_layer[changed_indices]
+        label_layer[predicted_slices][label_layer[predicted_slices] == point_label] = 0
         if self.segmentation_mode == SegmentationMode.SEMANTIC or point_label == 0:
-            self.label_layer.data[prediction == 1] = point_label
+            label_layer[prediction == 1] = point_label
         else:
-            self.label_layer.data[(prediction == 1) & (self.label_layer.data == 0)] = point_label
-        index_labels_new = self.label_layer.data[changed_indices]
+            label_layer[(prediction == 1) & (label_layer == 0)] = point_label
+        index_labels_new = label_layer[changed_indices]
         self.label_layer_changes = {"indices": changed_indices, "old_values": index_labels_old, "new_values": index_labels_new}
-        self.label_layer.data = self.label_layer.data
+        self.label_layer.data = label_layer
         self.old_points = copy.deepcopy(self.points_layer.data)
         # self.label_layer.refresh()
 
     def predict(self, points, labels):
         points = np.asarray(points)
         old_point, new_point = self.find_changed_point(np.asarray(self.old_points), points)
         if self.image_layer.ndim == 2:
```

### Comparing `napari-sam-0.3.6/src/napari_sam/utils.py` & `napari-sam-0.3.7/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.3.6/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.3.7/src/napari_sam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.3.6
+Version: 0.3.7
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napari-sam Version: 0.3.6 Summary: Segment anything
+Metadata-Version: 2.1 Name: napari-sam Version: 0.3.7 Summary: Segment anything
 with Meta AI's new SAM model! Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski Author-email: karol.gotkowski@dkfz.de License: Apache-
 2.0 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
 Project-URL: Source Code, https://github.com/MIC-DKFZ/napari-sam Project-URL:
 User Support, https://github.com/MIC-DKFZ/napari-sam/issues Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Framework :: napari Classifier:
```

