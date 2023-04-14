# Comparing `tmp/anylabeling-0.1.4.tar.gz` & `tmp/anylabeling-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.1.4.tar", last modified: Thu Apr 13 15:31:28 2023, max compression
+gzip compressed data, was "anylabeling-0.1.5.tar", last modified: Fri Apr 14 02:34:17 2023, max compression
```

## Comparing `anylabeling-0.1.4.tar` & `anylabeling-0.1.5.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.637069 anylabeling-0.1.4/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.1.4/LICENSE
--rw-r--r--   0 vietanhdev   (501) staff       (20)      113 2023-04-12 17:03:45.000000 anylabeling-0.1.4/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-13 15:31:28.636837 anylabeling-0.1.4/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.1.4/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.619087 anylabeling-0.1.4/anylabeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       67 2023-04-12 17:16:44.000000 anylabeling-0.1.4/anylabeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      927 2023-04-13 15:24:26.000000 anylabeling-0.1.4/anylabeling/app.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      114 2023-04-13 15:29:28.000000 anylabeling-0.1.4/anylabeling/app_info.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.620573 anylabeling-0.1.4/anylabeling/configs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.4/anylabeling/configs/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.620707 anylabeling-0.1.4/anylabeling/configs/__pycache__/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.1.4/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.1.4/anylabeling/configs/anylabeling_config.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)      316 2023-04-12 17:03:45.000000 anylabeling-0.1.4/anylabeling/configs/autolabel_segment_anything.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1172 2023-04-12 17:03:45.000000 anylabeling-0.1.4/anylabeling/configs/autolabel_yolov5m.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1172 2023-04-12 17:03:45.000000 anylabeling-0.1.4/anylabeling/configs/autolabel_yolov5s.yaml
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.620922 anylabeling-0.1.4/anylabeling/resources/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.4/anylabeling/resources/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)   477720 2023-04-12 17:04:48.000000 anylabeling-0.1.4/anylabeling/resources/resources.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.621306 anylabeling-0.1.4/anylabeling/services/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.4/anylabeling/services/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.622038 anylabeling-0.1.4/anylabeling/services/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.1.4/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3537 2023-04-13 15:20:55.000000 anylabeling-0.1.4/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5371 2023-04-12 16:58:37.000000 anylabeling-0.1.4/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9870 2023-04-12 17:27:56.000000 anylabeling-0.1.4/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1335 2023-04-12 17:29:20.000000 anylabeling-0.1.4/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5286 2023-04-12 17:30:50.000000 anylabeling-0.1.4/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.1.4/anylabeling/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.622265 anylabeling-0.1.4/anylabeling/views/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.4/anylabeling/views/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.622648 anylabeling-0.1.4/anylabeling/views/common/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.4/anylabeling/views/common/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.1.4/anylabeling/views/common/tableview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9583 2023-04-12 17:30:44.000000 anylabeling-0.1.4/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.623802 anylabeling-0.1.4/anylabeling/views/labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:53:51.000000 anylabeling-0.1.4/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5590 2023-04-12 16:58:37.000000 anylabeling-0.1.4/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2771 2023-04-12 17:31:48.000000 anylabeling-0.1.4/anylabeling/views/labeling/config.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.633679 anylabeling-0.1.4/anylabeling/views/labeling/icons/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/.DS_Store
--rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/app.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/app.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/app.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/cancel.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/cartesian.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/circle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/color-line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/color.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/color_line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/copy.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/delete.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/done.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/done.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/edit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/expert.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/expert1.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/expert2.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/eye.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/feBlend-icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/file.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/fit-width.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/fit-window.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/fit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/format_createml.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/format_voc.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/format_yolo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/help.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/icon.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/icon.ico
--rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/labels.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    36597 2023-04-12 17:03:45.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/labels.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/line-strip.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/new.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/next.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/objects.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/open.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/paste.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/point.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/polygon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/prev.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/quit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/rectangle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/resetall.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/save-as.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/save.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/undo-cross.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/undo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/upload_brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/verify.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/zoom-in.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/zoom-out.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/icons/zoom.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5995 2023-04-12 17:33:36.000000 anylabeling-0.1.4/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    89248 2023-04-12 17:35:36.000000 anylabeling-0.1.4/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.1.4/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1786 2023-04-12 01:57:00.000000 anylabeling-0.1.4/anylabeling/views/labeling/logger.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10441 2023-04-12 17:34:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/shape.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.634547 anylabeling-0.1.4/anylabeling/views/labeling/utils/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-12 17:21:05.000000 anylabeling-0.1.4/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.1.4/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-12 16:58:37.000000 anylabeling-0.1.4/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.636288 anylabeling-0.1.4/anylabeling/views/labeling/widgets/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-12 16:58:37.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.636647 anylabeling-0.1.4/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7373 2023-04-12 16:58:37.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    46656 2023-04-12 17:34:43.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8027 2023-04-12 16:58:37.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5780 2023-04-12 17:34:51.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-11 17:52:02.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.1.4/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      915 2023-04-12 16:58:37.000000 anylabeling-0.1.4/anylabeling/views/mainwindow.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-13 15:31:28.619966 anylabeling-0.1.4/anylabeling.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-13 15:31:28.000000 anylabeling-0.1.4/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5055 2023-04-13 15:31:28.000000 anylabeling-0.1.4/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-13 15:31:28.000000 anylabeling-0.1.4/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-13 15:31:28.000000 anylabeling-0.1.4/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      188 2023-04-13 15:31:28.000000 anylabeling-0.1.4/anylabeling.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-13 15:31:28.000000 anylabeling-0.1.4/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      175 2023-04-12 17:16:19.000000 anylabeling-0.1.4/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-13 15:31:28.637116 anylabeling-0.1.4/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2333 2023-04-13 15:22:05.000000 anylabeling-0.1.4/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.424086 anylabeling-0.1.5/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.1.5/LICENSE
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      113 2023-04-12 17:03:45.000000 anylabeling-0.1.5/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-14 02:34:17.423927 anylabeling-0.1.5/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.1.5/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.404389 anylabeling-0.1.5/anylabeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       67 2023-04-12 17:16:44.000000 anylabeling-0.1.5/anylabeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      927 2023-04-13 15:24:26.000000 anylabeling-0.1.5/anylabeling/app.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      114 2023-04-14 02:34:01.000000 anylabeling-0.1.5/anylabeling/app_info.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.405863 anylabeling-0.1.5/anylabeling/configs/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/configs/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.406056 anylabeling-0.1.5/anylabeling/configs/__pycache__/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.1.5/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/configs/anylabeling_config.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      316 2023-04-12 17:03:45.000000 anylabeling-0.1.5/anylabeling/configs/autolabel_segment_anything.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1172 2023-04-12 17:03:45.000000 anylabeling-0.1.5/anylabeling/configs/autolabel_yolov5m.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1172 2023-04-12 17:03:45.000000 anylabeling-0.1.5/anylabeling/configs/autolabel_yolov5s.yaml
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.406516 anylabeling-0.1.5/anylabeling/resources/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/resources/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   477720 2023-04-12 17:04:48.000000 anylabeling-0.1.5/anylabeling/resources/resources.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.406965 anylabeling-0.1.5/anylabeling/services/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/services/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.407752 anylabeling-0.1.5/anylabeling/services/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3537 2023-04-13 15:20:55.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5371 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9870 2023-04-12 17:27:56.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1335 2023-04-12 17:29:20.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5286 2023-04-12 17:30:50.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.407975 anylabeling-0.1.5/anylabeling/views/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/views/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.408324 anylabeling-0.1.5/anylabeling/views/common/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/views/common/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/views/common/tableview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9583 2023-04-12 17:30:44.000000 anylabeling-0.1.5/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.409521 anylabeling-0.1.5/anylabeling/views/labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:53:51.000000 anylabeling-0.1.5/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5590 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2771 2023-04-12 17:31:48.000000 anylabeling-0.1.5/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.420933 anylabeling-0.1.5/anylabeling/views/labeling/icons/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/.DS_Store
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/app.icns
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/app.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/app.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/icon.icns
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/icon.ico
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    36597 2023-04-12 17:03:45.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5995 2023-04-12 17:33:36.000000 anylabeling-0.1.5/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    89248 2023-04-14 02:33:50.000000 anylabeling-0.1.5/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.1.5/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1786 2023-04-12 01:57:00.000000 anylabeling-0.1.5/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10441 2023-04-12 17:34:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.421776 anylabeling-0.1.5/anylabeling/views/labeling/utils/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-12 17:21:05.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.423316 anylabeling-0.1.5/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.423707 anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7373 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    46656 2023-04-14 02:33:50.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8027 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5780 2023-04-12 17:34:51.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-14 02:24:11.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      915 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/mainwindow.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.405230 anylabeling-0.1.5/anylabeling.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5055 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      188 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      175 2023-04-12 17:16:19.000000 anylabeling-0.1.5/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-14 02:34:17.424131 anylabeling-0.1.5/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2333 2023-04-13 15:22:05.000000 anylabeling-0.1.5/setup.py
```

### Comparing `anylabeling-0.1.4/LICENSE` & `anylabeling-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/PKG-INFO` & `anylabeling-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.1.4
+Version: 0.1.5
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.1.4 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.1.5 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.1.4/README.md` & `anylabeling-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/app.py` & `anylabeling-0.1.5/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.1.5/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/configs/autolabel_yolov5m.yaml` & `anylabeling-0.1.5/anylabeling/configs/autolabel_yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/configs/autolabel_yolov5s.yaml` & `anylabeling-0.1.5/anylabeling/configs/autolabel_yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/resources/resources.py` & `anylabeling-0.1.5/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.1.5/anylabeling/services/auto_labeling/model.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.1.5/anylabeling/services/auto_labeling/model_manager.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.1.5/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.1.5/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.1.5/anylabeling/services/auto_labeling/yolov5.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/common/tableview.py` & `anylabeling-0.1.5/anylabeling/views/common/tableview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/common/toaster.py` & `anylabeling-0.1.5/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/__main__.py` & `anylabeling-0.1.5/anylabeling/views/labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/config.py` & `anylabeling-0.1.5/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/.DS_Store` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/app.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/app.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/app.svg` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/app.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/brain.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/cancel.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/cartesian.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/cartesian.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/circle.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/circle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/color-line.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/color.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/color.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/color_line.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/color_line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/copy.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/copy.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/delete.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/delete.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/done.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/done.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/done.svg` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/done.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/edit.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/edit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/expert.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/expert.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/eye.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/eye.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/feBlend-icon.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/file.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/file.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/fit-width.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/fit-window.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/fit.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/fit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/format_createml.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/format_createml.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/format_voc.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/format_voc.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/format_yolo.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/format_yolo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/help.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/help.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/icon.icns` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/icon.ico` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/icon.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/labels.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/labels.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/labels.svg` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/line-strip.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/line-strip.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/line.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/new.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/new.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/next.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/next.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/objects.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/objects.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/open.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/open.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/paste.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/paste.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/point.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/point.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/polygon.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/prev.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/prev.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/quit.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/quit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/rectangle.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/resetall.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/resetall.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/save-as.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/save.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/save.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/undo-cross.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/undo.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/undo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/upload_brain.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/upload_brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/verify.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/verify.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/zoom-in.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/zoom-out.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/icons/zoom.png` & `anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/label_file.py` & `anylabeling-0.1.5/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.1.5/anylabeling/views/labeling/label_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.1.5/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/logger.py` & `anylabeling-0.1.5/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/shape.py` & `anylabeling-0.1.5/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/testing.py` & `anylabeling-0.1.5/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.1.5/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.1.5/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.1.5/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.1.5/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.1.5/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.1.5/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling/views/mainwindow.py` & `anylabeling-0.1.5/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.1.5/anylabeling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.1.4
+Version: 0.1.5
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.1.4 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.1.5 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.1.4/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.1.5/anylabeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.4/setup.py` & `anylabeling-0.1.5/setup.py`

 * *Files identical despite different names*

