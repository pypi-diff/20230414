# Comparing `tmp/pcleaner-1.5.1.tar.gz` & `tmp/pcleaner-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.5.1.tar", last modified: Fri Apr 14 12:35:42 2023, max compression
+gzip compressed data, was "pcleaner-1.5.2.tar", last modified: Fri Apr 14 12:56:51 2023, max compression
```

## Comparing `pcleaner-1.5.1.tar` & `pcleaner-1.5.2.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.460964 pcleaner-1.5.1/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.5.1/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-14 12:35:42.460964 pcleaner-1.5.1/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.5.1/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.457631 pcleaner-1.5.1/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       47 2023-04-14 12:07:42.000000 pcleaner-1.5.1/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    17222 2023-04-11 21:05:32.000000 pcleaner-1.5.1/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8765 2023-04-14 12:31:00.000000 pcleaner-1.5.1/pcleaner/cleaner.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5672 2023-01-23 03:12:00.000000 pcleaner-1.5.1/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.457631 pcleaner-1.5.1/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.457631 pcleaner-1.5.1/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.457631 pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.460964 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.5.1/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35861 2023-04-13 14:02:44.000000 pcleaner-1.5.1/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6082 2023-04-13 17:19:01.000000 pcleaner-1.5.1/pcleaner/ctd_interface.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.5.1/pcleaner/denoiser.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)      767 2023-04-13 18:30:59.000000 pcleaner-1.5.1/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23338 2023-04-13 18:46:48.000000 pcleaner-1.5.1/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    24546 2023-04-14 12:23:58.000000 pcleaner-1.5.1/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4717 2023-01-08 14:40:11.000000 pcleaner-1.5.1/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8183 2023-04-13 18:07:02.000000 pcleaner-1.5.1/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.5.1/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13299 2023-04-13 19:11:27.000000 pcleaner-1.5.1/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:35:42.457631 pcleaner-1.5.1/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1412 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      171 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-14 12:35:42.000000 pcleaner-1.5.1/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.5.1/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1039 2023-04-14 12:35:42.460964 pcleaner-1.5.1/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.5.1/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.5.2/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-14 12:56:51.407667 pcleaner-1.5.2/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.5.2/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       47 2023-04-14 12:56:46.000000 pcleaner-1.5.2/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    17222 2023-04-11 21:05:32.000000 pcleaner-1.5.2/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8765 2023-04-14 12:31:00.000000 pcleaner-1.5.2/pcleaner/cleaner.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5672 2023-01-23 03:12:00.000000 pcleaner-1.5.2/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.5.2/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35861 2023-04-13 14:02:44.000000 pcleaner-1.5.2/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6082 2023-04-13 17:19:01.000000 pcleaner-1.5.2/pcleaner/ctd_interface.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.5.2/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner/gui/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.5.2/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      767 2023-04-13 18:30:59.000000 pcleaner-1.5.2/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23338 2023-04-13 18:46:48.000000 pcleaner-1.5.2/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    24649 2023-04-14 12:54:02.000000 pcleaner-1.5.2/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.5.2/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8183 2023-04-13 18:07:02.000000 pcleaner-1.5.2/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.5.2/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13299 2023-04-13 19:11:27.000000 pcleaner-1.5.2/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:56:51.407667 pcleaner-1.5.2/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1437 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      171 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-14 12:56:51.000000 pcleaner-1.5.2/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.5.2/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1039 2023-04-14 12:56:51.407667 pcleaner-1.5.2/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.5.2/setup.py
```

### Comparing `pcleaner-1.5.1/LICENSE` & `pcleaner-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/PKG-INFO` & `pcleaner-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.5.1
+Version: 1.5.2
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pcleaner-1.5.1/README.md` & `pcleaner-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/analytics.py` & `pcleaner-1.5.2/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/cleaner.py` & `pcleaner-1.5.2/pcleaner/cleaner.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/cli_utils.py` & `pcleaner-1.5.2/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.5.2/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/config.py` & `pcleaner-1.5.2/pcleaner/config.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/ctd_interface.py` & `pcleaner-1.5.2/pcleaner/ctd_interface.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/denoiser.py` & `pcleaner-1.5.2/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/helpers.py` & `pcleaner-1.5.2/pcleaner/helpers.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/image_ops.py` & `pcleaner-1.5.2/pcleaner/image_ops.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/main.py` & `pcleaner-1.5.2/pcleaner/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         [--keep-cache] [--cache-masks] [--debug]
     pcleaner profile (list | new <profile_name> [<profile_path>] | add <profile_name> <profile_path> |
         open <profile_name> | delete <profile_name> | set-default <profile_name> | repair <profile_name> |
         purge-missing) [--debug]
     pcleaner ocr [<image_path> ...] [--output-path=<output_path>] [--debug]
     pcleaner config (show | open)
     pcleaner cache clear (all | models | cleaner)
-    pcleaner load model [--cuda | --cpu | --both] [--force]
+    pcleaner load models [--cuda | --cpu | --both] [--force]
     pcleaner --help
     pcleaner --version
 
 Subcommands:
     clean            Clean the given image(s). Any number of images and directories can be given.
     profile          Manage profiles. These are files storing the settings for the program.
         list         List all saved profiles.
@@ -35,15 +35,15 @@
     config           View or edit the config file. This stores setting independent of profiles.
         show         Show the current configuration. This doesn't show the current profile.
         open         Open the config file in the default editor (unless specified in the config).
     cache clear      Clear the cache. This is where the program stores downloaded models and other files.
         all          Clear all cache files.
         models       Clear only the models.
         cleaner      Clear only the temporary masks and debug data.
-    load models      Download the models used by the program. If neither --cuda nor --cpu is specified, the program will
+    load models       Download the models used by the program. If neither --cuda nor --cpu is specified, the program will
                      try to use CUDA if available. If it is not, it will fall back to CPU.
                      This is done automatically when needed, but can be done manually.
 
 
 Options:
     <image_path>                    One or multiple files or directories to clean.
                                     Leave blank to use the current working directory.
@@ -182,27 +182,27 @@
         config = cfg.load_config()
         run_ocr(config, args.image_path, args.output_path)
 
     elif args.cache and args.clear:
         config = cfg.load_config()
         clear_cache(config, args.all, args.models, args.cleaner)
 
-    elif args.load and args.model:
+    elif args.load and args.models:
         config = cfg.load_config()
         md.download_models(config, args.force, args.cuda or args.both, args.cpu or args.both)
 
     elif args.config:
         # Handle config subcommand.
         config = cfg.load_config()
 
         if args.show:
             config.show()
         elif args.open:
             cli.open_file_with_editor(cli.get_config_path(), config.profile_editor)
-    else:
+    elif args.clean:
         # Do the actual work.
         config = cfg.load_config()
         config.load_profile(args["--profile"])
         logger.debug(config)
 
         if args.output_dir is None:
             args.output_dir = Path("cleaned")
@@ -230,14 +230,17 @@
             keep_cache=args.keep_cache,
             debug=args.debug,
         )
         # end timer.
         end = time.time()
         print(f"\nTime elapsed: {end - start:.2f} seconds")
 
+    else:
+        print("Invalid command. See 'pcleaner --help' for more information.")
+
 
 def run_cleaner(
     image_paths: list[Path],
     output_dir: Path,
     config: cfg.Config,
     skip_text_detection: bool,
     skip_pre_processing: bool,
```

### Comparing `pcleaner-1.5.1/pcleaner/model_downloader.py` & `pcleaner-1.5.2/pcleaner/model_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from pathlib import Path
 from hashlib import sha256
 
 import requests
 import tqdm
 import torch
+from manga_ocr import MangaOcr
 
 
 MODEL_URL = "https://github.com/zyddnys/manga-image-translator/releases/download/beta-0.3/"
 TORCH_MODEL_NAME = "comictextdetector.pt"
 TORCH_SHA256 = "1f90fa60aeeb1eb82e2ac1167a66bf139a8a61b8780acd351ead55268540cccb"
 CV2_MODEL_NAME = "comictextdetector.pt.onnx"
 CV2_SHA256 = "1a86ace74961413cbd650002e7bb4dcec4980ffa21b2f19b86933372071d718f"
@@ -125,7 +126,10 @@
             config.default_cv2_model_path = download_cv2_model(cache_dir)
         else:
             print(
                 f"Skipping OpenCV model download, path already set to: {config.default_cv2_model_path}"
             )
 
     config.save()
+
+    # Also load the OCR model, but there is only one option and can't be forced.
+    MangaOcr()
```

### Comparing `pcleaner-1.5.1/pcleaner/pre_processor.py` & `pcleaner-1.5.2/pcleaner/pre_processor.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/profile_cli.py` & `pcleaner-1.5.2/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner/structures.py` & `pcleaner-1.5.2/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.1/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.5.2/pcleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.5.1
+Version: 1.5.2
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pcleaner-1.5.1/pcleaner.egg-info/SOURCES.txt` & `pcleaner-1.5.2/pcleaner.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 pcleaner/comic_text_detector/utils/general.py
 pcleaner/comic_text_detector/utils/imgproc_utils.py
 pcleaner/comic_text_detector/utils/io_utils.py
 pcleaner/comic_text_detector/utils/loss.py
 pcleaner/comic_text_detector/utils/textblock.py
 pcleaner/comic_text_detector/utils/textmask.py
 pcleaner/comic_text_detector/utils/weight_init.py
-pcleaner/comic_text_detector/utils/yolov5_utils.py
+pcleaner/comic_text_detector/utils/yolov5_utils.py
+pcleaner/gui/__init__.py
```

### Comparing `pcleaner-1.5.1/setup.cfg` & `pcleaner-1.5.2/setup.cfg`

 * *Files identical despite different names*

