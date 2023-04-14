# Comparing `tmp/napari-hough-circle-detector-0.0.2.tar.gz` & `tmp/napari-hough-circle-detector-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-hough-circle-detector-0.0.2.tar", last modified: Wed Apr  5 14:39:14 2023, max compression
+gzip compressed data, was "napari-hough-circle-detector-0.0.3.tar", last modified: Fri Apr 14 13:42:41 2023, max compression
```

## Comparing `napari-hough-circle-detector-0.0.2.tar` & `napari-hough-circle-detector-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aymanns  (193172) IMAGING-GE-unit (11027)        0 2023-04-05 14:39:14.775382 napari-hough-circle-detector-0.0.2/
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)    35106 2023-04-03 14:10:26.000000 napari-hough-circle-detector-0.0.2/LICENSE
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      474 2023-04-05 14:39:14.775382 napari-hough-circle-detector-0.0.2/PKG-INFO
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      100 2023-04-03 14:10:26.000000 napari-hough-circle-detector-0.0.2/README.md
-drwxr-xr-x   0 aymanns  (193172) IMAGING-GE-unit (11027)        0 2023-04-05 14:39:14.775382 napari-hough-circle-detector-0.0.2/napari_hough_circle_detector/
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)    11720 2023-04-05 14:28:14.000000 napari-hough-circle-detector-0.0.2/napari_hough_circle_detector/__init__.py
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      370 2023-03-31 09:00:07.000000 napari-hough-circle-detector-0.0.2/napari_hough_circle_detector/napari.yaml
-drwxr-xr-x   0 aymanns  (193172) IMAGING-GE-unit (11027)        0 2023-04-05 14:39:14.775382 napari-hough-circle-detector-0.0.2/napari_hough_circle_detector.egg-info/
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      474 2023-04-05 14:39:14.000000 napari-hough-circle-detector-0.0.2/napari_hough_circle_detector.egg-info/PKG-INFO
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      438 2023-04-05 14:39:14.000000 napari-hough-circle-detector-0.0.2/napari_hough_circle_detector.egg-info/SOURCES.txt
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)        1 2023-04-05 14:39:14.000000 napari-hough-circle-detector-0.0.2/napari_hough_circle_detector.egg-info/dependency_links.txt
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)       90 2023-04-05 14:39:14.000000 napari-hough-circle-detector-0.0.2/napari_hough_circle_detector.egg-info/entry_points.txt
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)       55 2023-04-05 14:39:14.000000 napari-hough-circle-detector-0.0.2/napari_hough_circle_detector.egg-info/requires.txt
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)       29 2023-04-05 14:39:14.000000 napari-hough-circle-detector-0.0.2/napari_hough_circle_detector.egg-info/top_level.txt
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      101 2023-04-03 13:33:22.000000 napari-hough-circle-detector-0.0.2/pyproject.toml
--rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      755 2023-04-05 14:39:14.775382 napari-hough-circle-detector-0.0.2/setup.cfg
+drwxr-xr-x   0 aymanns  (193172) IMAGING-GE-unit (11027)        0 2023-04-14 13:42:41.197172 napari-hough-circle-detector-0.0.3/
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)    35106 2023-04-03 14:10:26.000000 napari-hough-circle-detector-0.0.3/LICENSE
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      474 2023-04-14 13:42:41.197172 napari-hough-circle-detector-0.0.3/PKG-INFO
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      100 2023-04-03 14:10:26.000000 napari-hough-circle-detector-0.0.3/README.md
+drwxr-xr-x   0 aymanns  (193172) IMAGING-GE-unit (11027)        0 2023-04-14 13:42:41.197172 napari-hough-circle-detector-0.0.3/napari_hough_circle_detector/
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)    13250 2023-04-14 13:35:16.000000 napari-hough-circle-detector-0.0.3/napari_hough_circle_detector/__init__.py
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      370 2023-03-31 09:00:07.000000 napari-hough-circle-detector-0.0.3/napari_hough_circle_detector/napari.yaml
+drwxr-xr-x   0 aymanns  (193172) IMAGING-GE-unit (11027)        0 2023-04-14 13:42:41.197172 napari-hough-circle-detector-0.0.3/napari_hough_circle_detector.egg-info/
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      474 2023-04-14 13:42:41.000000 napari-hough-circle-detector-0.0.3/napari_hough_circle_detector.egg-info/PKG-INFO
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      438 2023-04-14 13:42:41.000000 napari-hough-circle-detector-0.0.3/napari_hough_circle_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)        1 2023-04-14 13:42:41.000000 napari-hough-circle-detector-0.0.3/napari_hough_circle_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)       90 2023-04-14 13:42:41.000000 napari-hough-circle-detector-0.0.3/napari_hough_circle_detector.egg-info/entry_points.txt
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)       68 2023-04-14 13:42:41.000000 napari-hough-circle-detector-0.0.3/napari_hough_circle_detector.egg-info/requires.txt
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)       29 2023-04-14 13:42:41.000000 napari-hough-circle-detector-0.0.3/napari_hough_circle_detector.egg-info/top_level.txt
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      101 2023-04-03 13:33:22.000000 napari-hough-circle-detector-0.0.3/pyproject.toml
+-rw-r--r--   0 aymanns  (193172) IMAGING-GE-unit (11027)      769 2023-04-14 13:42:41.197172 napari-hough-circle-detector-0.0.3/setup.cfg
```

### Comparing `napari-hough-circle-detector-0.0.2/LICENSE` & `napari-hough-circle-detector-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-hough-circle-detector-0.0.2/napari_hough_circle_detector/__init__.py` & `napari-hough-circle-detector-0.0.3/napari_hough_circle_detector/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import functools
 import itertools
+import os
 import pathlib
 import typing
 
 import cv2
 import magicgui
 import napari
 import numpy as np
 import qtpy.QtWidgets
+import skimage
 
 __author__ = "Florian Aymanns"
 __email__ = "florian.aymanns@epfl.ch"
 
 
 def _extract_img_data(img: napari.layers.Image, view_only: bool = False) -> np.ndarray:
     """
@@ -218,40 +221,72 @@
                 },
                 "points",
             )
         )
     return layer_data_tuples
 
 
-def export_csv(points: napari.layers.Points, filename=pathlib.Path("./circles.csv")):
-    centers = points.data
-    radii = points.size / 2
-    data = np.concatenate([centers, radii], axis=1)
-    np.savetxt(
-        filename,
-        data[:, :-1],
-        delimiter=",",
-        header="center x, center y, radius",
-        fmt="%.1f",
-    )
-    print(f"Saved file to {filename}.")
+def export(
+    sliders_widget,
+    napari_viewer: napari.Viewer,
+    output_type: str,
+    export_stack: bool,
+    folder: pathlib.Path = pathlib.Path("."),
+    filename: str = "circles.csv",
+):
+    stack = sliders_widget.img.value
 
+    n_slices = napari_viewer.dims.nsteps[0]
+    current_slice = napari_viewer.dims.current_step[0]
+    channel = napari_viewer.dims.current_step[1]
 
-def export_mask(
-    points: napari.layers.Points,
-    filename=pathlib.Path("./circles.tif"),
-    size=(1024, 1024),
-):
-    centers = points.data.astype(int)[:, ::-1]
-    radii = (points.size[:, 0] / 2).astype(int)
-    mask = np.zeros(size)
-    for center, radius in zip(centers, radii):
-        mask = cv2.circle(mask, center, radius, (1, 1, 1), -1)
-    cv2.imwrite(str(filename), mask)
-    print(f"Saved file to {filename}.")
+    if export_stack:
+        slice_indices = np.arange(n_slices)
+    else:
+        slice_indices = (current_slice,)
+    slice_results = []
+    img_data = _extract_img_data(stack, view_only=False)
+    for slice_idx in slice_indices:
+        _, circles = _compute_edges_and_circles(
+            img_data[slice_idx, channel],
+            sliders_widget.dp.value,
+            sliders_widget.minDist.value,
+            sliders_widget.param1.value,
+            sliders_widget.param2.value,
+            sliders_widget.minRadius.value,
+            sliders_widget.maxRadius.value,
+            contrast_limits=stack.contrast_limits,
+        )
+        indices = np.array([[slice_idx, channel]] * circles.shape[0])
+        circles = np.concatenate([indices, circles], axis=1)
+        slice_results.append(circles)
+    slice_results = np.concatenate(slice_results, axis=0)
+
+    if output_type == "csv":
+        np.savetxt(
+            filename,
+            slice_results,
+            delimiter=",",
+            header="frame, channel, center x, center y, radius",
+            fmt="%.1f",
+        )
+        print(f"Saved file to {filename}.")
+    elif output_type == "mask":
+        masks = []
+        for slice_idx in slice_indices:
+            mask = np.zeros(img_data.shape[-2:], dtype=np.uint8)
+            slice_mask = slice_results[:, 0] == slice_idx
+            slice_circles = slice_results[slice_mask, 2:].astype(int)
+            for center_x, center_y, radius in slice_circles:
+                mask = cv2.circle(mask, (center_x, center_y), radius, 255, -1)
+            masks.append(mask)
+        mask = np.stack(masks, axis=0)
+        mask = np.squeeze(mask)
+        skimage.io.imsave(str(filename), mask)
+        print(f"Saved file to {filename}.")
 
 
 class CircleDetectorWidget(qtpy.QtWidgets.QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         filter_widget = magicgui.magicgui(
             median_filter,
@@ -264,56 +299,39 @@
             dp={"widget_type": "FloatSlider", "min": 0.1, "max": 10},
             minDist={"widget_type": "IntSlider", "min": 1, "max": 200},
             param1={"widget_type": "IntSlider", "min": 10, "max": 1000},
             param2={"widget_type": "IntSlider", "min": 10, "max": 300},
             minRadius={"widget_type": "IntSlider", "min": 1, "max": 300},
             maxRadius={"widget_type": "IntSlider", "min": 1, "max": 500},
         )
-        export_csv_widget = magicgui.magicgui(
-            export_csv, call_button="Export circles to csv"
-        )
-        export_mask_widget = magicgui.magicgui(
-            export_mask, call_button="Export circles to mask"
+        export_widget = magicgui.magicgui(
+            functools.partial(export, sliders_widget),
+            call_button="Export circles",
+            folder={"mode": "d"},
+            output_type={"choices": ["csv", "mask"]},
         )
         self._children = [
             filter_widget,
             sliders_widget,
-            export_csv_widget,
-            export_mask_widget,
+            export_widget,
         ]
 
         self.setLayout(qtpy.QtWidgets.QVBoxLayout())
 
         self.layout().addWidget(filter_widget.native)
         filter_widget.img.reset_choices()
         napari_viewer.layers.events.inserted.connect(filter_widget.img.reset_choices)
         napari_viewer.layers.events.removed.connect(filter_widget.img.reset_choices)
 
         self.layout().addWidget(sliders_widget.native)
         sliders_widget.img.reset_choices()
         napari_viewer.layers.events.inserted.connect(sliders_widget.img.reset_choices)
         napari_viewer.layers.events.removed.connect(sliders_widget.img.reset_choices)
 
-        self.layout().addWidget(export_csv_widget.native)
-        export_csv_widget.points.reset_choices()
-        napari_viewer.layers.events.inserted.connect(
-            export_csv_widget.points.reset_choices
-        )
-        napari_viewer.layers.events.removed.connect(
-            export_csv_widget.points.reset_choices
-        )
-
-        self.layout().addWidget(export_mask_widget.native)
-        export_mask_widget.points.reset_choices()
-        napari_viewer.layers.events.inserted.connect(
-            export_mask_widget.points.reset_choices
-        )
-        napari_viewer.layers.events.removed.connect(
-            export_mask_widget.points.reset_choices
-        )
+        self.layout().addWidget(export_widget.native)
 
         # Update circles when slice or channel is changes
         napari_viewer.dims.events.current_step.connect(lambda event: sliders_widget())
 
         def connect_contrast_limits(widget):
             """
             Update circles when contrast limits are changes
@@ -325,23 +343,43 @@
         connect_contrast_limits(sliders_widget)
 
         # Make sure the connection to the contrast limits persists when the input layer is changed
         sliders_widget.img.changed.connect(
             lambda event: connect_contrast_limits(sliders_widget)
         )
 
+        def update_file_extension(widget):
+            output_type = widget.output_type.value
+            name = widget.filename.value
+            name_wo_extension = os.path.splitext(name)[0]
+            if output_type == "csv":
+                widget.filename.value = name_wo_extension + ".csv"
+            elif output_type == "mask":
+                widget.filename.value = name_wo_extension + ".tif"
+
+        export_widget.output_type.changed.connect(
+            lambda event: update_file_extension(export_widget)
+        )
+
         # Update default output file names when the layer is changed
-        def update_default_file_name(widget, extension):
-            folder = pathlib.Path(widget.filename.value).parents[0]
+        def update_default_file_name(widget):
+            if sliders_widget.img.value is None:
+                return
             name = sliders_widget.img.value.name
-            step = napari_viewer.dims.current_step[0]
-            extension = extension.rstrip(".")
-            widget.filename.value = folder / pathlib.Path(
-                f"{name}_{step:05}.{extension}"
-            )
+            extension = os.path.splitext(widget.filename.value)[1]
+            extension = extension.lstrip(".")
+            export_stack = widget.export_stack.value
+            if export_stack:
+                widget.filename.value = f"{name}_stack.{extension}"
+            else:
+                step = napari_viewer.dims.current_step[0]
+                widget.filename.value = f"{name}_{step:05}.{extension}"
 
         sliders_widget.img.changed.connect(
-            lambda event: update_default_file_name(export_csv_widget, "csv")
+            lambda event: update_default_file_name(export_widget)
         )
-        sliders_widget.img.changed.connect(
-            lambda event: update_default_file_name(export_mask_widget, "tif")
+        napari_viewer.dims.events.current_step.connect(
+            lambda event: update_default_file_name(export_widget)
+        )
+        export_widget.export_stack.changed.connect(
+            lambda event: update_default_file_name(export_widget)
         )
```

### Comparing `napari-hough-circle-detector-0.0.2/setup.cfg` & `napari-hough-circle-detector-0.0.3/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-hough-circle-detector
-version = 0.0.2
+version = 0.0.3
 classifiers = 
 	Framework :: napari
 author = Florian Aymanns
 author_email = florian.aymanns@epfl.ch
 maintainer = Florian Aymanns
 maintainer_email = florian.aymanns@epfl.ch
 description = An interactive Hough transform for napari.
@@ -16,14 +16,15 @@
 packages = find:
 include_package_data = True
 install_requires = 
 	napari[all]
 	opencv-contrib-python-headless
 	numpy
 	pyqt5
+	scikit-image
 
 [options.entry_points]
 napari.manifest = 
 	napari-hough-circle-detector = napari_hough_circle_detector:napari.yaml
 
 [options.package_data]
 napari-hough-circle-detector = napari.yaml
```

