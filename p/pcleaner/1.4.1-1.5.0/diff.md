# Comparing `tmp/pcleaner-1.4.1.tar.gz` & `tmp/pcleaner-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.4.1.tar", last modified: Wed Apr 12 23:00:21 2023, max compression
+gzip compressed data, was "pcleaner-1.5.0.tar", last modified: Thu Apr 13 23:46:24 2023, max compression
```

## Comparing `pcleaner-1.4.1.tar` & `pcleaner-1.5.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 23:00:21.437795 pcleaner-1.4.1/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.4.1/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-12 23:00:21.437795 pcleaner-1.4.1/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.4.1/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 23:00:21.434462 pcleaner-1.4.1/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       47 2023-04-12 23:00:08.000000 pcleaner-1.4.1/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    17222 2023-04-11 21:05:32.000000 pcleaner-1.4.1/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8623 2023-04-12 22:59:58.000000 pcleaner-1.4.1/pcleaner/cleaner.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5672 2023-01-23 03:12:00.000000 pcleaner-1.4.1/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 23:00:21.434462 pcleaner-1.4.1/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 23:00:21.434462 pcleaner-1.4.1/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 23:00:21.437795 pcleaner-1.4.1/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 23:00:21.437795 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2007 2023-04-11 20:28:36.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.4.1/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    33652 2023-04-12 03:17:56.000000 pcleaner-1.4.1/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5736 2023-04-12 03:29:15.000000 pcleaner-1.4.1/pcleaner/ctd_interface.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4865 2023-04-12 22:59:58.000000 pcleaner-1.4.1/pcleaner/denoiser.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    22979 2023-04-12 22:59:58.000000 pcleaner-1.4.1/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    22404 2023-04-12 03:17:45.000000 pcleaner-1.4.1/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4717 2023-01-08 14:40:11.000000 pcleaner-1.4.1/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7679 2023-04-12 03:17:45.000000 pcleaner-1.4.1/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.4.1/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12959 2023-04-11 02:23:20.000000 pcleaner-1.4.1/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-12 23:00:21.434462 pcleaner-1.4.1/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-12 23:00:21.000000 pcleaner-1.4.1/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1392 2023-04-12 23:00:21.000000 pcleaner-1.4.1/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-12 23:00:21.000000 pcleaner-1.4.1/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-12 23:00:21.000000 pcleaner-1.4.1/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      171 2023-04-12 23:00:21.000000 pcleaner-1.4.1/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-12 23:00:21.000000 pcleaner-1.4.1/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.4.1/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1039 2023-04-12 23:00:21.441128 pcleaner-1.4.1/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.4.1/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.5.0/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-13 23:46:24.673959 pcleaner-1.5.0/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.5.0/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       47 2023-04-13 19:33:03.000000 pcleaner-1.5.0/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    17222 2023-04-11 21:05:32.000000 pcleaner-1.5.0/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8889 2023-04-13 23:45:01.000000 pcleaner-1.5.0/pcleaner/cleaner.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5672 2023-01-23 03:12:00.000000 pcleaner-1.5.0/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35861 2023-04-13 14:02:44.000000 pcleaner-1.5.0/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6082 2023-04-13 17:19:01.000000 pcleaner-1.5.0/pcleaner/ctd_interface.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5651 2023-04-13 23:39:08.000000 pcleaner-1.5.0/pcleaner/denoiser.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      767 2023-04-13 18:30:59.000000 pcleaner-1.5.0/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23338 2023-04-13 18:46:48.000000 pcleaner-1.5.0/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    24546 2023-04-13 22:47:46.000000 pcleaner-1.5.0/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4717 2023-01-08 14:40:11.000000 pcleaner-1.5.0/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8183 2023-04-13 18:07:02.000000 pcleaner-1.5.0/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.5.0/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13299 2023-04-13 19:11:27.000000 pcleaner-1.5.0/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1412 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      171 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.5.0/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1039 2023-04-13 23:46:24.673959 pcleaner-1.5.0/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.5.0/setup.py
```

### Comparing `pcleaner-1.4.1/LICENSE` & `pcleaner-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/PKG-INFO` & `pcleaner-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.4.1
+Version: 1.5.0
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pcleaner-1.4.1/README.md` & `pcleaner-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/analytics.py` & `pcleaner-1.5.0/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/cleaner.py` & `pcleaner-1.5.0/pcleaner/cleaner.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     :return: Analytics, consisting of the json file path, and a list of whether the mask was generated, the index of
         the best mask, and the border uniformity of the best mask for each box.
     """
 
     page_data = st.PageData.from_json(c_data.json_path.read_text())
 
     # Make a shorter alias.
-    cleaner_conf = c_data.cleaner_config
+    g_conf = c_data.general_config
+    c_conf = c_data.cleaner_config
 
     original_path = Path(page_data.original_path)
     original_img_path_as_png = original_path.with_suffix(
         ".png"
     )  # Make sure all derived file names are .png.
     # Clobber protection prefixes have the form "[A-Z]{4}-\d+_file name", ex. JMCF-0_0023.json
     clobber_protection_prefix = c_data.json_path.stem.split("_")[0]
@@ -58,15 +59,16 @@
     mask_fitments: list[st.MaskFittingResults] = [
         ops.pick_best_mask(
             base=base_image,
             precise_mask=cut_mask,
             box_mask=box_mask,
             masking_box=masking_box,
             reference_box=reference_box,
-            cleaner_conf=cleaner_conf,
+            cleaner_conf=c_conf,
+            scale=page_data.scale,
             save_masks=c_data.show_masks,
             analytics_page_path=Path(original_img_path_as_png),
         )
         for masking_box, reference_box in zip(
             page_data.merged_extended_boxes, page_data.reference_boxes
         )
     ]
@@ -84,72 +86,72 @@
     if c_data.show_masks:
         # Save the masks in the debug folder.
         ops.visualize_mask_fitments(
             base_image, mask_fitments, cache_out_path.with_stem(cache_out_path.stem + "_masks")
         )
 
         # Output the result with the debug filter.
-        combined_mask_debug = ops.apply_debug_filter_to_mask(
-            combined_mask, cleaner_conf.debug_mask_color
-        )
+        combined_mask_debug = ops.apply_debug_filter_to_mask(combined_mask, c_conf.debug_mask_color)
         base_image_copy = base_image.copy()
         base_image_copy.paste(combined_mask_debug, (0, 0), combined_mask_debug)
         save_mask(base_image_copy, "_with_masks")
 
-    cleaned_image = base_image.copy()
-    cleaned_image.paste(combined_mask, (0, 0), combined_mask)
-
-    # Save the combined mask and cleaned image. This will be used for denoising.
+    # Save the combined mask for denoising.
     combined_mask_path = cache_out_path.with_stem(cache_out_path.stem + "_combined_mask")
     combined_mask.save(combined_mask_path)
-    cleaned_image_path = cache_out_path.with_stem(cache_out_path.stem + "_cleaned")
-    ops.save_optimized(cleaned_image, cleaned_image_path, original_path)
     save_denoising_data(
         Path(page_data.original_path),
         original_img_path_as_png,
-        cleaned_image_path,
         combined_mask_path,
+        Path(page_data.image_path),
         cache_out_path,
+        page_data.scale,
+        c_conf.mask_max_standard_deviation,
         mask_fitments,
     )
 
     # Settle on the final output path for the cleaned image.
     # Check if outputting directly.
     if c_data.output_dir is not None:
+        # If the scale isn't 1, then we need to reload the original image and scale the mask to fit.
+        if page_data.scale != 1:
+            cleaned_image = Image.open(page_data.original_path)
+            combined_mask = combined_mask.resize(cleaned_image.size, Image.NEAREST)
+        else:
+            cleaned_image = base_image.copy()
+
+        cleaned_image.paste(combined_mask, (0, 0), combined_mask)
+
         if c_data.output_dir.is_absolute():
             final_out_path = c_data.output_dir / original_img_path_as_png.name
         else:
             # Take the original image path, and place the image in a subdirectory.
             # This is for when multiple directories were passed in.
             final_out_path = (
                 original_img_path_as_png.parent / c_data.output_dir / original_img_path_as_png.name
             )
 
         final_out_path.parent.mkdir(parents=True, exist_ok=True)
         final_cleaned_out_path = final_out_path.with_name(final_out_path.stem + "_clean.png")
         final_mask_out_path = final_out_path.with_name(final_out_path.stem + "_mask.png")
 
         # Check what the preferred output format is.
-        if cleaner_conf.preferred_file_type is None:
+        if g_conf.preferred_file_type is None:
             # Use the original file type.
             final_cleaned_out_path = final_cleaned_out_path.with_suffix(
                 Path(page_data.original_path).suffix
             )
         else:
-            final_cleaned_out_path = final_cleaned_out_path.with_suffix(
-                cleaner_conf.preferred_file_type
-            )
+            final_cleaned_out_path = final_cleaned_out_path.with_suffix(g_conf.preferred_file_type)
 
-        if cleaner_conf.preferred_mask_file_type is None:
+        if g_conf.preferred_mask_file_type is None:
             # Use png by default.
             final_mask_out_path = final_mask_out_path.with_suffix(".png")
         else:
-            final_mask_out_path = final_mask_out_path.with_suffix(
-                cleaner_conf.preferred_mask_file_type
-            )
+            final_mask_out_path = final_mask_out_path.with_suffix(g_conf.preferred_mask_file_type)
 
         logger.debug(f"Final output path: {final_cleaned_out_path}")
 
         # The arg parser should ensure that both can't be true at once, not like that'd be an issue, just plain silly.
         if not c_data.save_only_mask and not c_data.save_only_text:
             # Save the final image.
             logger.debug(f"Saving final image to {final_cleaned_out_path}")
@@ -161,50 +163,50 @@
             ops.save_optimized(combined_mask, final_mask_out_path)
 
         if c_data.extract_text:
             # Extract the text layer from the image.
             logger.debug(f"Extracting text from {final_cleaned_out_path}")
             text_img = ops.extract_text(base_image, combined_mask)
             text_out_path = final_out_path.with_name(final_out_path.stem + "_text.png")
-            if cleaner_conf.preferred_mask_file_type is None:
+            if g_conf.preferred_mask_file_type is None:
                 # Use png by default.
                 text_out_path = text_out_path.with_suffix(".png")
             else:
-                text_out_path = text_out_path.with_suffix(cleaner_conf.preferred_mask_file_type)
+                text_out_path = text_out_path.with_suffix(g_conf.preferred_mask_file_type)
             ops.save_optimized(text_img, text_out_path, original_path)
 
     return analytics
 
 
 def save_denoising_data(
     original_path: Path,
     target_path: Path,
-    cleaned_path: Path,
     mask_path: Path,
+    base_image_path: Path,
     cache_path: Path,
+    scale: float,
+    mask_max_deviation: float,
     mask_fitments: list[st.MaskFittingResults],
 ):
     """
     Save the data needed for denoising.
 
-    Gather the following to construct a MaskData struct:
-    - original_path: Path
-    - cleaned_path: Path
-    - mask_path: Path
-    - boxes_with_deviation: list[tuple[tuple[int, int, int, int], float]]
-
     :param original_path: The path to the original image.
     :param target_path: The path to the original image with png suffix.
-    :param cleaned_path: The path to the cleaned image.
     :param mask_path: The path to the combined mask.
+    :param base_image_path: The path to the cached base image.
     :param cache_path: The path to the cache directory.
+    :param scale: The scale of the original image to the cached base image.
+    :param mask_max_deviation: The maximum deviation of the mask.
     :param mask_fitments: The mask fitments.
     """
 
-    # Gather the data needed for denoising.
-    boxes_with_deviation = [m.noise_mask_data for m in mask_fitments]
+    # Gather the data needed for denoising, don't include those with a deviation greater than the max deviation.
+    boxes_with_deviation = [
+        m.noise_mask_data for m in mask_fitments if m.analytics_std_deviation <= mask_max_deviation
+    ]
 
     # Save the data.
     mask_data = st.MaskData(
-        original_path, target_path, cleaned_path, mask_path, boxes_with_deviation
+        original_path, target_path, base_image_path, mask_path, scale, boxes_with_deviation
     )
     mask_data.write_json(cache_path.with_name(cache_path.stem + "_mask_data.json"))
```

### Comparing `pcleaner-1.4.1/pcleaner/cli_utils.py` & `pcleaner-1.5.0/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os.path as osp
 import glob
 from pathlib import Path
 import cv2
 import numpy as np
 import json
 
-# These need to be restored after patching to a new version of the comic text detector.
 IMG_EXT = [".jpeg", ".jpg", ".png", ".bmp", ".tiff", ".tif", ".jp2", ".dib", ".webp", ".ppm"]
 
 NP_BOOL_TYPES = (np.bool_, np.bool8)
 NP_FLOAT_TYPES = (np.float_, np.float16, np.float32, np.float64)
 NP_INT_TYPES = (
     np.int_,
     np.int8,
```

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/config.py` & `pcleaner-1.5.0/pcleaner/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,83 @@
 from pcleaner import model_downloader as md
 
 
 RESERVED_PROFILE_NAMES = ["builtin", "none"]
 
 
 @dataclass
-class TextDetectorConfig:
-    model_path: str | None = None
-    concurrent_models: int = 1
+class GeneralConfig:
+    preferred_file_type: str | None = None
+    preferred_mask_file_type: str | None = None
+    input_size_scale: float = 1.0
 
     def export_to_conf(self, config_updater: cu.ConfigUpdater) -> None:
         """
         Write the config to the config updater object.
 
         No add_after_section here since it is the first section.
 
         :param config_updater: An existing config updater object.
         """
 
         config_str = f"""\
+        [General]
+        
+        # Preferred file type to save the cleaned image as.
+        # If no file type is specified, the original file type will be used.
+        preferred_file_type = {self.preferred_file_type if self.preferred_file_type else ""}
+
+        # Preferred file type to save the mask as.
+        # If no file type is specified, png will be used.
+        # This is because the mask image must use transparency, which is not supported by all image formats.
+        preferred_mask_file_type = {self.preferred_mask_file_type if self.preferred_mask_file_type else ""}
+        
+        # Scale the input image by this amount before processing.
+        # This is useful for significantly speeding up processing on large images.
+        # The image will be scaled down, processed, and then only the mask is scaled back up.
+        # Meaning that the cleaned output will still use the original, unscaled image to prevent any loss in quality.
+        # Images larger than 3000x3000 pixels should be scaled down, so that they fall within this range.
+        # E.g. an Image with the size 7000x10000 pixels should be scaled down with a factor of 0.25,
+        # so that it has the size 1750x2500 pixels during processing.
+        # The default value is 1.0, which means no scaling.
+        input_size_scale = {self.input_size_scale}
+        
+        """
+        config_updater.read_string(multi_left_strip(config_str))
+
+    def import_from_conf(self, config_updater: cu.ConfigUpdater) -> None:
+        """
+        Read the config from the config updater object.
+
+        :param config_updater: An existing config updater object.
+        """
+        section = "General"
+        if not config_updater.has_section(section):
+            logger.info(f"No {section} section found in the profile, using defaults.")
+            return
+
+        try_to_load(self, config_updater, section, str | None, "preferred_file_type")
+        try_to_load(self, config_updater, section, str | None, "preferred_mask_file_type")
+        try_to_load(self, config_updater, section, float, "input_size_scale")
+
+
+@dataclass
+class TextDetectorConfig:
+    model_path: str | None = None
+    concurrent_models: int = 1
+
+    def export_to_conf(self, config_updater: cu.ConfigUpdater, add_after_section: str) -> None:
+        """
+        Write the config to the config updater object.
+
+        :param config_updater: An existing config updater object.
+        :param add_after_section: The section to add the config after.
+        """
+
+        config_str = f"""\
         [TextDetector]
         
         # Path to the text detection model, leave empty to use the built-in model.
         # The model can be found here:
         # https://github.com/zyddnys/manga-image-translator/releases/latest
         model_path = {none_to_empty(self.model_path)}
         
@@ -38,15 +93,18 @@
         # (or VRAM with CUDA) to run multiple models at the same time.
         # This, of course, will increase the speed of the process, but can also
         # crash your computer if you overestimate your hardware.
         # I recommend using 1 model per 2 GB of memory available.
         concurrent_models = {self.concurrent_models}
         
         """
-        config_updater.read_string(multi_left_strip(config_str))
+        detector_conf = cu.ConfigUpdater()
+        detector_conf.read_string(multi_left_strip(config_str))
+        general_section = detector_conf["TextDetector"]
+        config_updater[add_after_section].add_after.space(2).section(general_section.detach())
 
     def import_from_conf(self, config_updater: cu.ConfigUpdater) -> None:
         """
         Read the config from the config updater object.
 
         :param config_updater: An existing config updater object.
         """
@@ -153,16 +211,14 @@
         try_to_load(self, config_updater, section, int, "box_padding_extended")
         try_to_load(self, config_updater, section, int, "box_right_padding_extended")
         try_to_load(self, config_updater, section, int, "box_reference_padding")
 
 
 @dataclass
 class CleanerConfig:
-    preferred_file_type: str | None = None
-    preferred_mask_file_type: str | None = None
     mask_growth_step_pixels: int = 2
     mask_growth_steps: int = 11
     off_white_max_threshold: int = 240
     mask_improvement_threshold: float = 0.1
     mask_selection_fast: bool = False
     mask_max_standard_deviation: float = 15
     debug_mask_color: tuple[int, int, int, int] = (108, 30, 240, 127)
@@ -174,23 +230,14 @@
         :param config_updater: An existing config updater object.
         :param add_after_section: The section to add the new section after.
         """
         config_str = f"""\
         [Cleaner]
         
         
-        # Preferred file type to save the cleaned image as.
-        # If no file type is specified, the original file type will be used.
-        preferred_file_type = {self.preferred_file_type if self.preferred_file_type else ""}
-        
-        # Preferred file type to save the mask as.
-        # If no file type is specified, png will be used.
-        # This is because the mask image must use transparency, which is not supported by all image formats.
-        preferred_mask_file_type = {self.preferred_mask_file_type if self.preferred_mask_file_type else ""}
-        
         # Number of pixels to grow the mask by each step.
         # This bulks up the outline of the mask, so smaller values will be more accurate but slower.
         mask_growth_step_pixels = {self.mask_growth_step_pixels}
         
         # Number of steps to grow the mask by.
         # A higher number will make more and larger masks, ultimately limited by the reference box size.
         mask_growth_steps = {self.mask_growth_steps}
@@ -236,16 +283,14 @@
         :param config_updater: An existing config updater object.
         """
         section = "Cleaner"
         if not config_updater.has_section(section):
             logger.info(f"No {section} section found in the profile, using defaults.")
             return
 
-        try_to_load(self, config_updater, section, str | None, "preferred_file_type")
-        try_to_load(self, config_updater, section, str | None, "preferred_mask_file_type")
         try_to_load(self, config_updater, section, int, "mask_growth_step_pixels")
         try_to_load(self, config_updater, section, int, "mask_growth_steps")
         try_to_load(self, config_updater, section, int, "off_white_max_threshold")
         try_to_load(self, config_updater, section, float, "mask_improvement_threshold")
         try_to_load(self, config_updater, section, bool, "mask_selection_fast")
         try_to_load(self, config_updater, section, float, "mask_max_standard_deviation")
         try:
@@ -348,28 +393,31 @@
 
 @dataclass
 class Profile:
     """
     A profile is a collection of settings that can be saved and loaded from disk.
     """
 
+    general: GeneralConfig = GeneralConfig()
     text_detector: TextDetectorConfig = TextDetectorConfig()
     pre_processor: PreProcessorConfig = PreProcessorConfig()
     cleaner: CleanerConfig = CleanerConfig()
     denoiser: DenoiserConfig = DenoiserConfig()
 
     def write(self, path: Path) -> bool:
         """
         Write the profile to a file.
 
         :param path: The path to write the profile to.
         :return: True if the profile was written successfully, False otherwise.
         """
+        logger.debug("Writing profile to disk...")
         config_updater = cu.ConfigUpdater()
-        self.text_detector.export_to_conf(config_updater)
+        self.general.export_to_conf(config_updater)
+        self.text_detector.export_to_conf(config_updater, "General")
         self.pre_processor.export_to_conf(config_updater, "TextDetector")
         self.cleaner.export_to_conf(config_updater, "PreProcessor")
         self.denoiser.export_to_conf(config_updater, "Cleaner")
         try:
             with open(path, "w") as file:
                 config_updater.write(file)
             return True
@@ -378,18 +426,20 @@
             return False
 
     @classmethod
     def load(cls, path: Path) -> "Profile":
         """
         Load a profile from a config file.
         """
+        logger.debug("Loading profile from disk...")
         config = cu.ConfigUpdater()
         try:
             config.read(path)
             profile = cls()
+            profile.general.import_from_conf(config)
             profile.text_detector.import_from_conf(config)
             profile.pre_processor.import_from_conf(config)
             profile.cleaner.import_from_conf(config)
             profile.denoiser.import_from_conf(config)
         except Exception as e:
             logger.error(f"Failed to load profile from {path}:\n{e}")
             profile = cls()
```

### Comparing `pcleaner-1.4.1/pcleaner/denoiser.py` & `pcleaner-1.5.0/pcleaner/denoiser.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,38 +10,50 @@
 def denoise_page(d_data: st.DenoiserData) -> st.DenoiseAnalytic:
     """
     Load the MaskData from the json file and perform the denoising process.
 
     :param d_data: All the data needed for the denoising process.
     :return: Analytics.
     """
-
     # Load all the cached data.
     mask_data = st.MaskData.from_json(d_data.json_path.read_text())
-    cleaned_image = Image.open(mask_data.cleaned_path)
     mask_image = Image.open(mask_data.mask_path)
+
+    # Scale the mask to the original image size, if needed.
+    scale = mask_data.scale
+    cleaned_image = Image.open(mask_data.original_path)
+    mask_image = mask_image.convert("LA")
+    cleaned_image = cleaned_image.convert("RGB")
+    if scale != 1.0:
+        mask_image = mask_image.resize(cleaned_image.size, resample=Image.NEAREST)
+
+    cleaned_image.paste(mask_image, (0, 0), mask_image)
     original_path: Path = mask_data.original_path
 
     # Alias.
+    g_conf = d_data.general_config
     d_conf = d_data.denoiser_config
-    c_conf = d_data.cleaner_config
 
     # Filter for the min deviation to consider for denoising.
     boxes_to_denoise: list[tuple[int, int, int, int]] = [
-        box
+        scaled_box(box, scale)
         for box, deviation in mask_data.boxes_with_deviation
         if deviation > d_conf.noise_min_standard_deviation
     ]
 
     noise_masks_with_coords: list[tuple[Image.Image, tuple[int, int]]] = [
         ops.generate_noise_mask(cleaned_image, mask_image, box, d_conf) for box in boxes_to_denoise
     ]
 
-    combined_noise_mask = ops.combine_noise_masks(cleaned_image.size, noise_masks_with_coords)
-    cleaned_image.paste(combined_noise_mask, (0, 0), combined_noise_mask)
+    if noise_masks_with_coords:
+        logger.info("coombining noise masks...")
+        combined_noise_mask = ops.combine_noise_masks(cleaned_image.size, noise_masks_with_coords)
+        cleaned_image.paste(combined_noise_mask, (0, 0), combined_noise_mask)
+    else:
+        combined_noise_mask = Image.new("LA", cleaned_image.size, (0, 0))
 
     # Debug save.
     if d_data.show_masks:
         cache_out_path = d_data.cache_dir / (mask_data.target_path.stem + "_noise_mask.png")
         combined_noise_mask.save(cache_out_path)
 
     # Settle on the final output path for the cleaned image.
@@ -58,25 +70,25 @@
     final_cleaned_out_path = final_out_path.with_name(final_out_path.stem + "_clean.png")
     final_mask_out_path = final_out_path.with_name(final_out_path.stem + "_mask.png")
     final_mask_denoised_out_path = final_out_path.with_name(
         final_out_path.stem + "_denoised_mask.png"
     )
 
     # Check what the preferred output format is.
-    if c_conf.preferred_file_type is None:
+    if g_conf.preferred_file_type is None:
         # Use the original file type.
         final_cleaned_out_path = final_cleaned_out_path.with_suffix(original_path.suffix)
     else:
-        final_cleaned_out_path = final_cleaned_out_path.with_suffix(c_conf.preferred_file_type)
+        final_cleaned_out_path = final_cleaned_out_path.with_suffix(g_conf.preferred_file_type)
 
-    if c_conf.preferred_mask_file_type is None:
+    if g_conf.preferred_mask_file_type is None:
         # Use png by default.
         final_mask_out_path = final_mask_out_path.with_suffix(".png")
     else:
-        final_mask_out_path = final_mask_out_path.with_suffix(c_conf.preferred_mask_file_type)
+        final_mask_out_path = final_mask_out_path.with_suffix(g_conf.preferred_mask_file_type)
 
     logger.debug(f"Final output path: {final_cleaned_out_path}")
 
     # The arg parser should ensure that both can't be true at once, not like that'd be an issue, just plain silly.
     if not d_data.save_only_mask:
         # Save the final image.
         logger.debug(f"Saving final image to {final_cleaned_out_path}")
@@ -98,16 +110,24 @@
 
     if d_data.extract_text:
         # Extract the text layer from the image.
         logger.debug(f"Extracting text from {original_path}")
         base_image = Image.open(original_path)
         text_img = ops.extract_text(base_image, mask_image)
         text_out_path = final_out_path.with_name(final_out_path.stem + "_text.png")
-        if c_conf.preferred_mask_file_type is None:
+        if g_conf.preferred_mask_file_type is None:
             # Use png by default.
             text_out_path = text_out_path.with_suffix(".png")
         else:
-            text_out_path = text_out_path.with_suffix(c_conf.preferred_mask_file_type)
+            text_out_path = text_out_path.with_suffix(g_conf.preferred_mask_file_type)
         ops.save_optimized(text_img, text_out_path, original_path)
 
     # Package the analytics. We're only interested in the std deviations.
     return st.DenoiseAnalytic(tuple(deviation for _, deviation in mask_data.boxes_with_deviation))
+
+
+def scaled_box(box: tuple[int, int, int, int], scale: float) -> tuple[int, int, int, int]:
+    """Scales a box by a given scale."""
+    if scale == 1.0:
+        return box
+    # noinspection PyTypeChecker
+    return tuple(int(x * scale) for x in box)
```

### Comparing `pcleaner-1.4.1/pcleaner/image_ops.py` & `pcleaner-1.5.0/pcleaner/image_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import cv2
 import scipy
 from PIL import Image, ImageFilter
 from logzero import logger
 
 import pcleaner.structures as st
 import pcleaner.config as cfg
+import pcleaner.helpers as hp
 
 
 class BlankMaskError(Exception):
     pass
 
 
 def convert_mask_to_rgba(mask: Image, color: int | tuple[int, int, int, int] = 255) -> Image:
@@ -96,24 +97,25 @@
 
     :param base_image: The base image to stack the masks on top of.
     :param mask_fitments: The data of the masks to apply.
     :param output_path: The path to save the image to.
     """
     # Compose all masks of the same index into one mask.
     # Each fitment result contains a list of the sub-masks and their positions.
-    masks = [
-        compose_masks(
-            base_image.size,
-            [
-                (mask_fitment.debug_masks[index], mask_fitment.mask_coords)
-                for mask_fitment in mask_fitments
-            ],
-        )
-        for index in range(len(mask_fitments[0].debug_masks))
-    ]
+    masks = []
+    max_masks = max(len(mask_fitment.debug_masks) for mask_fitment in mask_fitments)
+    for index in range(max_masks):
+        mask_list = []
+        for mask_fitment in mask_fitments:
+            if index >= len(mask_fitment.debug_masks):
+                continue
+            mask_tuple = (mask_fitment.debug_masks[index], mask_fitment.mask_coords)
+            mask_list.append(mask_tuple)
+        mask = compose_masks(base_image.size, mask_list)
+        masks.append(mask)
 
     # Don't modify the original image.
     base_image = base_image.copy()
 
     # Generate colors for each mask.
     hues = map(lambda i: (0.15 * i) % 1, range(len(masks)))
 
@@ -261,14 +263,15 @@
 def pick_best_mask(
     base: Image,
     precise_mask: Image,
     box_mask: Image,
     masking_box: tuple[int, int, int, int],
     reference_box: tuple[int, int, int, int],
     cleaner_conf: cfg.CleanerConfig,
+    scale: float,
     save_masks: bool,
     analytics_page_path: Path,
 ) -> None | st.MaskFittingResults:
     """
     Generate various sizes of the precise mask and pick the best one from
     among them, and the box mask.
 
@@ -287,14 +290,15 @@
 
     :param base: The base image.
     :param precise_mask: The precise mask.
     :param box_mask: The box mask.
     :param masking_box: The box to cut the mask out of.
     :param reference_box: The box to cut the base image out of.
     :param cleaner_conf: The cleaner config.
+    :param scale: The scale of the original image to the base image.
     :param save_masks: Whether to save the masks.
     :param analytics_page_path: The path to the original image for the analytics.
     :return: The best mask and what color to make it and the box (along with analytics). If no best
         mask was found, return None for the mask and color.
     """
     # Calculate offset coords between the reference box and the mask box.
     # The mask box was grown by n pixels in each direction to make the reference box,
@@ -314,16 +318,19 @@
         return None
 
     box_mask = cut_out_mask(box_mask, masking_box, base.size, x_offset, y_offset)
 
     # Generate masks of various sizes for the precise mask, then add the box mask to the list.
     # The generated masks are in ascending size order.
     mask_gen = make_mask_steps_convolution(
-        precise_mask, cleaner_conf.mask_growth_step_pixels, cleaner_conf.mask_growth_steps
+        precise_mask,
+        hp.scale_length_rounded(cleaner_conf.mask_growth_step_pixels, scale),
+        cleaner_conf.mask_growth_steps,
     )
+
     # When using the fast mask selection, make a new generator with the box mask as the first mask,
     # followed by the generated masks.
     def generator_with_first(generator, first):
         yield first
         yield from generator
 
     def generator_with_last(generator, last):
```

### Comparing `pcleaner-1.4.1/pcleaner/main.py` & `pcleaner-1.5.0/pcleaner/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 """
 
 
 import time
 from multiprocessing import Pool
 from pathlib import Path
 import itertools
+from PIL import Image
 
 from manga_ocr import MangaOcr
 from docopt import magic_docopt
 from logzero import logger, loglevel, DEBUG, INFO
 from tqdm import tqdm
 from natsort import natsorted
 import torch
@@ -122,14 +123,21 @@
 import pcleaner.cli_utils as cli
 import pcleaner.pre_processor as pp
 import pcleaner.analytics as an
 import pcleaner.structures as st
 import pcleaner.profile_cli as pc
 import pcleaner.denoiser as dn
 import pcleaner.model_downloader as md
+import pcleaner.helpers as hp
+
+# Supported image suffixes.
+IMG_EXT = [".jpeg", ".jpg", ".png", ".bmp", ".tiff", ".tif", ".jp2", ".dib", ".webp", ".ppm"]
+
+# Allow loading of large images.
+Image.MAX_IMAGE_PIXELS = 2**32
 
 
 def main():
 
     args = magic_docopt(__doc__, version=f"Panel Cleaner {__version__}")
     # Loglevel is info by default.
     if args.debug:
@@ -278,32 +286,40 @@
     # If caching masks, direct the user to the cache directory.
     if cache_masks:
         print(
             f"You can find the masks being generated in real-time in the cache directory:\n\n{cache_dir}\n"
         )
 
     if not skip_text_detection:
+        # Find all the images in the given image paths.
+        image_paths = discover_all_images(image_paths)
+        if not image_paths:
+            print("No images found.")
+            return
+        else:
+            print(f"Found {len(image_paths)} {hp.f_plural(len(image_paths), 'image', 'images')}.")
+            debug_path_printout = "\n".join(map(str, image_paths))
+            logger.debug(f"Image paths: \n{debug_path_printout}")
+
         # Delete the cache directory if not explicitly keeping it.
         if len(list(cache_dir.glob("*"))) > 0 and not keep_cache:
             cli.empty_cache_dir(cache_dir)
         # Get the model file, downloading it if necessary.
         cuda = torch.cuda.is_available()
         model_path = config.get_model_path(cuda)
 
         print("Running text detection AI model...")
-        print(profile.text_detector)
         pp.generate_mask_data(
-            image_paths, config=profile.text_detector, model_path=model_path, output_dir=cache_dir
+            image_paths,
+            config_general=profile.general,
+            config_detector=profile.text_detector,
+            model_path=model_path,
+            output_dir=cache_dir,
         )
 
-        if debug:
-            loglevel(DEBUG)
-        else:
-            loglevel(INFO)
-
         # Leave some extra space here if drawing analytics, so it looks better.
         if not hide_analytics:
             print("\n")
 
     if not skip_pre_processing:
         # Flush it so it shows up before the progress bar.
         print("Running box data Pre-Processor...", flush=True)
@@ -343,14 +359,15 @@
 
         # Zip together the json files and the out path thing.
         data = [
             st.CleanerData(
                 json_file,
                 cleaner_output_dir,
                 cache_dir,
+                profile.general,
                 profile.cleaner,
                 save_only_mask,
                 save_only_cleaned,
                 save_only_text,
                 extract_text,
                 cache_masks,
                 debug,
@@ -373,16 +390,16 @@
 
         # Zip together the json files and the out path thing.
         data = [
             st.DenoiserData(
                 json_file,
                 output_dir,
                 cache_dir,
+                profile.general,
                 profile.denoiser,
-                profile.cleaner,
                 save_only_mask,
                 save_only_cleaned,
                 extract_text,
                 separate_noise_mask,
                 cache_masks,
                 debug,
             )
@@ -456,15 +473,15 @@
         if ocr_analytic:
             ocr_analytics.append(ocr_analytic)
 
     # Output the OCRed text from the analytics.
     removed_texts = list(itertools.chain.from_iterable(a[3] for a in ocr_analytics))
 
     # Find and then remove the longest common prefix from the file paths.
-    prefix = an.longest_common_prefix([str(Path(path).parent) for path, _ in removed_texts])
+    prefix = an.longest_common_path_prefix([str(Path(path).parent) for path, _ in removed_texts])
     if prefix:
         removed_texts = [(path[len(prefix) :], text) for path, text in removed_texts]
     # Remove a rogue / or \ from the start of the path, if they all have one.
     if all(path.startswith("/") or path.startswith("\\") for path, _ in removed_texts):
         removed_texts = [(path[1:], text) for path, text in removed_texts]
 
     removed_texts = natsorted(removed_texts, key=lambda x: x[0])
@@ -514,9 +531,55 @@
 
     if images:
         image_cache_dir = config.get_cleaner_cache_dir()
         cli.empty_cache_dir(image_cache_dir)
         print(f"Cleared image cache at {image_cache_dir}")
 
 
+def discover_all_images(img_paths: str | Path | list[str | Path]) -> list[Path]:
+    """
+    Discover all images in the given paths.
+    Perform a shallow search in directories, not recursing into subdirectories.
+
+    :param img_paths: A path to a single image, directory, or multiple of either.
+    :return: A list of all images found by path only.
+    """
+    img_list: list[Path] = []
+
+    # Wrap single paths in a list.
+    if isinstance(img_paths, str):
+        img_list = [Path(img_paths)]
+        img_paths = []
+    elif isinstance(img_paths, Path):
+        img_list = [img_paths]
+        img_paths = []
+
+    # Convert all strings to paths.
+    img_paths = [Path(path) for path in img_paths]
+
+    for img_path in img_paths:
+        if img_path.is_dir():
+            img_list.extend(find_all_images_shallow(img_path))
+        elif img_path.is_file() and img_path.suffix.lower() in IMG_EXT:
+            img_list.append(img_path)
+        else:
+            raise FileNotFoundError(f"Image path {img_path} does not exist.")
+
+    # Ensure all paths are absolute.
+    img_list = [path.resolve() for path in img_list]
+
+    return img_list
+
+
+def find_all_images_shallow(img_dir: Path) -> list[Path]:
+    image_list: list[Path] = []
+    for file_path in img_dir.glob("*"):
+        file_suffix = file_path.suffix
+        if file_suffix.lower() not in IMG_EXT:
+            continue
+        else:
+            image_list.append(file_path)
+    return image_list
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `pcleaner-1.4.1/pcleaner/model_downloader.py` & `pcleaner-1.5.0/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/pre_processor.py` & `pcleaner-1.5.0/pcleaner/pre_processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 import json
 import re
 from dataclasses import asdict
 from pathlib import Path
+from functools import partial
 
 from PIL import Image
 from manga_ocr import MangaOcr
 
 import pcleaner.ctd_interface as ctm
 import pcleaner.structures as st
 import pcleaner.config as cfg
+import pcleaner.helpers as hp
 
 
 def generate_mask_data(
-    image_path: list[Path], config: cfg.TextDetectorConfig, model_path: Path, output_dir: Path
+    image_path: list[Path],
+    config_general: cfg.GeneralConfig,
+    config_detector: cfg.TextDetectorConfig,
+    model_path: Path,
+    output_dir: Path,
 ) -> None:
     """
     Run the ai model to generate masks and box data for the given image,
     or all images in the given directory.
 
     :param image_path: Path to the image or directory of images.
-    :param config: Text detector configuration, part of the profile.
+    :param config_general: General configuration, part of the profile.
+    :param config_detector: Text detector configuration, part of the profile.
     :param model_path: Path to the model file.
     :param output_dir: Path to the directory where the results will be saved.
     """
 
-    ctm.model2annotations(config, model_path, image_path, output_dir)
+    ctm.model2annotations(config_general, config_detector, model_path, image_path, output_dir)
 
 
 def prep_json_file(
     json_file_path: Path,
     pre_processor_conf: cfg.PreProcessorConfig,
     cache_masks: bool,
     mocr: MangaOcr | None = None,
@@ -50,72 +57,82 @@
 
     :param json_file_path: Path to the json file.
     :param pre_processor_conf: Pre processor configuration, part of the profile.
     :param cache_masks: Whether to cache the masks.
     :param mocr: [Optional] Manga ocr object.
     :return: Analytics data if the manga ocr object is given, None otherwise.
     """
+
     # Check if the file was already processed.
     if json_file_path.name.endswith("_clean.json"):
         return
     if json_file_path.name.endswith("_mask_data.json"):
         return
 
     json_data = json.loads(json_file_path.read_text())
 
     image_path = json_data["image_path"]
     mask_path = json_data["mask_path"]
     original_path = json_data["original_path"]
+    scale = json_data["scale"]
     boxes = []
 
+    scale_len = partial(hp.scale_length_rounded, scale=scale)
+    scale_area = partial(hp.scale_area_rounded, scale=scale)
+
     for data in json_data["blk_list"]:
         # Check minimum size of box.
         x1, y1, x2, y2 = data["xyxy"]
         box_size = (x2 - x1) * (y2 - y1)
-        if box_size > pre_processor_conf.box_min_size:
+        if box_size > scale_area(pre_processor_conf.box_min_size):
             # Sussy box. Discard if it's too small.
-            if (
-                data["language"] == "unknown"
-                and box_size < pre_processor_conf.suspicious_box_min_size
+            if data["language"] == "unknown" and box_size < scale_area(
+                pre_processor_conf.suspicious_box_min_size
             ):
                 continue
             boxes.append(data["xyxy"])
 
-    page_data = st.PageData(image_path, mask_path, original_path, boxes, [], [], [])
+    page_data = st.PageData(image_path, mask_path, original_path, scale, boxes, [], [], [])
 
     # Run OCR to discard small boxes that only contain symbols.
     analytics = None
     if mocr is not None:
         page_data, analytics = ocr_check(
             page_data,
             mocr,
-            pre_processor_conf.ocr_max_size,
+            scale_area(pre_processor_conf.ocr_max_size),
             pre_processor_conf.ocr_blacklist_pattern,
         )
 
     # Pad the boxes a bit, save a copy, and then pad them some more.
     # The copy is used as a smaller mask, and the padded copy is used as a larger mask.
-    page_data.grow_boxes(pre_processor_conf.box_padding_initial, st.BoxType.BOX)
-    page_data.right_pad_boxes(pre_processor_conf.box_right_padding_initial, st.BoxType.BOX)
+    page_data.grow_boxes(scale_len(pre_processor_conf.box_padding_initial), st.BoxType.BOX)
+    page_data.right_pad_boxes(
+        scale_len(pre_processor_conf.box_right_padding_initial), st.BoxType.BOX
+    )
 
     # A shallow copy of the box list suffices, because the tuples inside are immutable.
     page_data.extended_boxes = page_data.boxes.copy()
 
-    page_data.grow_boxes(pre_processor_conf.box_padding_extended, st.BoxType.EXTENDED_BOX)
+    page_data.grow_boxes(
+        scale_len(pre_processor_conf.box_padding_extended), st.BoxType.EXTENDED_BOX
+    )
     page_data.right_pad_boxes(
-        pre_processor_conf.box_right_padding_extended, st.BoxType.EXTENDED_BOX
+        scale_len(pre_processor_conf.box_right_padding_extended), st.BoxType.EXTENDED_BOX
     )
 
     # Check for overlapping boxes among the extended boxes.
     # The resulting list is saved in the page_data.merged_extended_boxes attribute.
     page_data.resolve_overlaps()
 
     # Copy the merged extended boxes to the reference boxes and grow them once again.
     page_data.reference_boxes = page_data.merged_extended_boxes.copy()
-    page_data.grow_boxes(pre_processor_conf.box_reference_padding, st.BoxType.REFERENCE_BOX)
+    page_data.grow_boxes(
+        scale_len(pre_processor_conf.box_reference_padding), st.BoxType.REFERENCE_BOX
+    )
 
     # Write the json file with the cleaned data.
     json_out_path = json_file_path.parent / f"{json_file_path.stem}_clean.json"
     # Remove the _image_size attribute, because it's a cached value that may be unset.
     page_data_dict = asdict(page_data)
     del page_data_dict["_image_size"]
     json_out_path.write_text(json.dumps(page_data_dict, indent=4))
```

### Comparing `pcleaner-1.4.1/pcleaner/profile_cli.py` & `pcleaner-1.5.0/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.4.1/pcleaner/structures.py` & `pcleaner-1.5.0/pcleaner/structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     Boxes are represented as tuples of (x1, y1, x2, y2), where (x1, y1) is the top left corner,
     and (x2, y2) is the bottom right corner.
     """
 
     image_path: str  # Path to the copied png.
     mask_path: str  # Path to the generated mask.png
     original_path: str  # Path to the original image. (used for relative output)
+    scale: float  # The size of the original image relative to the png.
     boxes: list[tuple[int, int, int, int]]
     extended_boxes: list[tuple[int, int, int, int]]
     merged_extended_boxes: list[tuple[int, int, int, int]]
     reference_boxes: list[tuple[int, int, int, int]]
     _image_size: tuple[
         int, int
     ] = None  # Cache the image size, so we don't have to load the image every time.
@@ -58,14 +59,15 @@
         :param json_str: The json string to load from.
         """
         json_data = json.loads(json_str)
         return cls(
             json_data["image_path"],
             json_data["mask_path"],
             json_data["original_path"],
+            json_data["scale"],
             json_data["boxes"],
             json_data["extended_boxes"],
             json_data["merged_extended_boxes"],
             json_data["reference_boxes"],
         )
 
     @property
@@ -263,25 +265,28 @@
 class CleanerData:
     """
     This is a simple struct to hold the inputs for the cleaner.
     The data is a tuple of:
     - The json file path.
     - The image output directory. When none, output to the cache dir for denoising to continue.
     - The image cache directory.
+    - The general config.
+    - The cleaner config.
     - The save only mask flag.
     - The save only cleaned flag.
     - The save only text flag.
     - The extract text flag.
     - The show masks flag. (when true, save intermediate masks to the cache directory)
     - The debug flag.
     """
 
     json_path: Path
     output_dir: Path | None
     cache_dir: Path
+    general_config: cfg.GeneralConfig
     cleaner_config: cfg.CleanerConfig
     save_only_mask: bool
     save_only_cleaned: bool
     save_only_text: bool
     extract_text: bool
     show_masks: bool
     debug: bool
@@ -293,81 +298,85 @@
     This is a simple struct to hold all the extra information needed to perform the
     denoising process.
 
     - The original image path.
     - The target image path.
     - The cleaned image path.
     - The mask image path.
+    - The scale of the original image to the base image.
     - The box coordinates with their respective standard deviation for the masks.
     """
 
     original_path: Path
     target_path: Path
-    cleaned_path: Path
+    base_image_path: Path
     mask_path: Path
+    scale: float
     boxes_with_deviation: list[tuple[tuple[int, int, int, int], float]]
 
     @classmethod
     def from_json(cls, json_str: str) -> "MaskData":
         """
         Create a MaskData object from a json string.
 
         :param json_str: The json string.
         :return: The MaskData object.
         """
         data = json.loads(json_str)
         return cls(
             Path(data["original_path"]),
             Path(data["target_path"]),
-            Path(data["cleaned_path"]),
+            Path(data["base_image_path"]),
             Path(data["mask_path"]),
+            data["scale"],
             data["boxes_with_deviation"],
         )
 
     def write_json(self, json_path: Path):
         """
         Write the MaskData object to a json file.
 
         :param json_path: The path to write the json file to.
         """
         # Convert the Path objects to strings.
         data = {
             "original_path": str(self.original_path),
             "target_path": str(self.target_path),
-            "cleaned_path": str(self.cleaned_path),
+            "base_image_path": str(self.base_image_path),
             "mask_path": str(self.mask_path),
+            "scale": self.scale,
             "boxes_with_deviation": self.boxes_with_deviation,
         }
         with open(json_path, "w") as f:
             json.dump(data, f, indent=4)
 
 
 @dataclass
 class DenoiserData:
     """
     This is a simple struct to hold the inputs for the denoiser.
     The data is a tuple of:
     - The json file path.
     - The image output directory.
     - The image cache directory.
+    - The general config.
     - The denoiser config.
-    - The cleaner config.
     - The save only mask flag.
     - The save only cleaned flag.
     - The extract text flag.
     - The separate noise mask flag.
     - The show masks flag. (when true, save intermediate masks to the cache directory)
     - The debug flag.
     """
 
     json_path: Path
     output_dir: Path
     cache_dir: Path
+    general_config: cfg.GeneralConfig
     denoiser_config: cfg.DenoiserConfig
-    cleaner_config: cfg.CleanerConfig
     save_only_mask: bool
     save_only_cleaned: bool
     extract_text: bool
     separate_noise_masks: bool
     show_masks: bool
     debug: bool
```

### Comparing `pcleaner-1.4.1/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.5.0/pcleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.4.1
+Version: 1.5.0
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pcleaner-1.4.1/pcleaner.egg-info/SOURCES.txt` & `pcleaner-1.5.0/pcleaner.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pcleaner/__init__.py
 pcleaner/analytics.py
 pcleaner/cleaner.py
 pcleaner/cli_utils.py
 pcleaner/config.py
 pcleaner/ctd_interface.py
 pcleaner/denoiser.py
+pcleaner/helpers.py
 pcleaner/image_ops.py
 pcleaner/main.py
 pcleaner/model_downloader.py
 pcleaner/pre_processor.py
 pcleaner/profile_cli.py
 pcleaner/structures.py
 pcleaner.egg-info/PKG-INFO
```

### Comparing `pcleaner-1.4.1/setup.cfg` & `pcleaner-1.5.0/setup.cfg`

 * *Files identical despite different names*

