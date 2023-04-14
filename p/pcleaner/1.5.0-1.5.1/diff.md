# Comparing `tmp/pcleaner-1.5.0.tar.gz` & `tmp/pcleaner-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.5.0.tar", last modified: Thu Apr 13 23:46:24 2023, max compression
+gzip compressed data, was "pcleaner-1.5.1.tar", last modified: Fri Apr 14 12:35:42 2023, max compression
```

## Comparing `pcleaner-1.5.0.tar` & `pcleaner-1.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.5.0/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-13 23:46:24.673959 pcleaner-1.5.0/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.5.0/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       47 2023-04-13 19:33:03.000000 pcleaner-1.5.0/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    17222 2023-04-11 21:05:32.000000 pcleaner-1.5.0/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8889 2023-04-13 23:45:01.000000 pcleaner-1.5.0/pcleaner/cleaner.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5672 2023-01-23 03:12:00.000000 pcleaner-1.5.0/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.5.0/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35861 2023-04-13 14:02:44.000000 pcleaner-1.5.0/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6082 2023-04-13 17:19:01.000000 pcleaner-1.5.0/pcleaner/ctd_interface.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5651 2023-04-13 23:39:08.000000 pcleaner-1.5.0/pcleaner/denoiser.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      767 2023-04-13 18:30:59.000000 pcleaner-1.5.0/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23338 2023-04-13 18:46:48.000000 pcleaner-1.5.0/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    24546 2023-04-13 22:47:46.000000 pcleaner-1.5.0/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4717 2023-01-08 14:40:11.000000 pcleaner-1.5.0/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8183 2023-04-13 18:07:02.000000 pcleaner-1.5.0/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.5.0/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13299 2023-04-13 19:11:27.000000 pcleaner-1.5.0/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-13 23:46:24.673959 pcleaner-1.5.0/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1412 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      171 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-13 23:46:24.000000 pcleaner-1.5.0/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.5.0/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1039 2023-04-13 23:46:24.673959 pcleaner-1.5.0/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.5.0/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.460964 pcleaner-1.5.1/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.5.1/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-14 12:35:42.460964 pcleaner-1.5.1/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.5.1/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.457631 pcleaner-1.5.1/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       47 2023-04-14 12:07:42.000000 pcleaner-1.5.1/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    17222 2023-04-11 21:05:32.000000 pcleaner-1.5.1/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8765 2023-04-14 12:31:00.000000 pcleaner-1.5.1/pcleaner/cleaner.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5672 2023-01-23 03:12:00.000000 pcleaner-1.5.1/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.457631 pcleaner-1.5.1/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.457631 pcleaner-1.5.1/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.457631 pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.460964 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35861 2023-04-13 14:02:44.000000 pcleaner-1.5.1/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6082 2023-04-13 17:19:01.000000 pcleaner-1.5.1/pcleaner/ctd_interface.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.5.1/pcleaner/denoiser.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      767 2023-04-13 18:30:59.000000 pcleaner-1.5.1/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23338 2023-04-13 18:46:48.000000 pcleaner-1.5.1/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    24546 2023-04-14 12:23:58.000000 pcleaner-1.5.1/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4717 2023-01-08 14:40:11.000000 pcleaner-1.5.1/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8183 2023-04-13 18:07:02.000000 pcleaner-1.5.1/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.5.1/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13299 2023-04-13 19:11:27.000000 pcleaner-1.5.1/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.457631 pcleaner-1.5.1/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1412 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      171 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.5.1/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1039 2023-04-14 12:35:42.460964 pcleaner-1.5.1/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.5.1/setup.py
```

### Comparing `pcleaner-1.5.0/LICENSE` & `pcleaner-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/PKG-INFO` & `pcleaner-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.5.0
+Version: 1.5.1
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pcleaner-1.5.0/README.md` & `pcleaner-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/analytics.py` & `pcleaner-1.5.1/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/cleaner.py` & `pcleaner-1.5.1/pcleaner/cleaner.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         ".png"
     )  # Make sure all derived file names are .png.
     # Clobber protection prefixes have the form "[A-Z]{4}-\d+_file name", ex. JMCF-0_0023.json
     clobber_protection_prefix = c_data.json_path.stem.split("_")[0]
     cache_out_path = (
         c_data.cache_dir / f"{clobber_protection_prefix}_{original_img_path_as_png.name}"
     )
-    logger.debug(f"Masking {cache_out_path.name}...")
 
     def save_mask(img, name_suffix):
         if c_data.show_masks:
             img.save(cache_out_path.with_stem(cache_out_path.stem + name_suffix))
 
     # Load the base image.
     base_image = Image.open(page_data.image_path)
@@ -145,16 +144,14 @@
 
         if g_conf.preferred_mask_file_type is None:
             # Use png by default.
             final_mask_out_path = final_mask_out_path.with_suffix(".png")
         else:
             final_mask_out_path = final_mask_out_path.with_suffix(g_conf.preferred_mask_file_type)
 
-        logger.debug(f"Final output path: {final_cleaned_out_path}")
-
         # The arg parser should ensure that both can't be true at once, not like that'd be an issue, just plain silly.
         if not c_data.save_only_mask and not c_data.save_only_text:
             # Save the final image.
             logger.debug(f"Saving final image to {final_cleaned_out_path}")
             ops.save_optimized(cleaned_image, final_cleaned_out_path, original_path)
 
         if not c_data.save_only_cleaned and not c_data.save_only_text:
```

### Comparing `pcleaner-1.5.0/pcleaner/cli_utils.py` & `pcleaner-1.5.1/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/config.py` & `pcleaner-1.5.1/pcleaner/config.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/ctd_interface.py` & `pcleaner-1.5.1/pcleaner/ctd_interface.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/denoiser.py` & `pcleaner-1.5.1/pcleaner/denoiser.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,18 @@
     ]
 
     noise_masks_with_coords: list[tuple[Image.Image, tuple[int, int]]] = [
         ops.generate_noise_mask(cleaned_image, mask_image, box, d_conf) for box in boxes_to_denoise
     ]
 
     if noise_masks_with_coords:
-        logger.info("coombining noise masks...")
         combined_noise_mask = ops.combine_noise_masks(cleaned_image.size, noise_masks_with_coords)
         cleaned_image.paste(combined_noise_mask, (0, 0), combined_noise_mask)
     else:
+        # noinspection PyTypeChecker
         combined_noise_mask = Image.new("LA", cleaned_image.size, (0, 0))
 
     # Debug save.
     if d_data.show_masks:
         cache_out_path = d_data.cache_dir / (mask_data.target_path.stem + "_noise_mask.png")
         combined_noise_mask.save(cache_out_path)
 
@@ -82,16 +82,14 @@
 
     if g_conf.preferred_mask_file_type is None:
         # Use png by default.
         final_mask_out_path = final_mask_out_path.with_suffix(".png")
     else:
         final_mask_out_path = final_mask_out_path.with_suffix(g_conf.preferred_mask_file_type)
 
-    logger.debug(f"Final output path: {final_cleaned_out_path}")
-
     # The arg parser should ensure that both can't be true at once, not like that'd be an issue, just plain silly.
     if not d_data.save_only_mask:
         # Save the final image.
         logger.debug(f"Saving final image to {final_cleaned_out_path}")
         ops.save_optimized(cleaned_image, final_cleaned_out_path, original_path)
 
     if not d_data.save_only_cleaned:
```

### Comparing `pcleaner-1.5.0/pcleaner/helpers.py` & `pcleaner-1.5.1/pcleaner/helpers.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/image_ops.py` & `pcleaner-1.5.1/pcleaner/image_ops.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/main.py` & `pcleaner-1.5.1/pcleaner/main.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/model_downloader.py` & `pcleaner-1.5.1/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/pre_processor.py` & `pcleaner-1.5.1/pcleaner/pre_processor.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/profile_cli.py` & `pcleaner-1.5.1/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner/structures.py` & `pcleaner-1.5.1/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.5.1/pcleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.5.0
+Version: 1.5.1
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pcleaner-1.5.0/pcleaner.egg-info/SOURCES.txt` & `pcleaner-1.5.1/pcleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.0/setup.cfg` & `pcleaner-1.5.1/setup.cfg`

 * *Files identical despite different names*

