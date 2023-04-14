# Comparing `tmp/anylabeling-0.1.5.tar.gz` & `tmp/anylabeling-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.1.5.tar", last modified: Fri Apr 14 02:34:17 2023, max compression
+gzip compressed data, was "anylabeling-0.1.6.tar", last modified: Fri Apr 14 19:17:44 2023, max compression
```

## Comparing `anylabeling-0.1.5.tar` & `anylabeling-0.1.6.tar`

### file list

```diff
@@ -1,137 +1,141 @@
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.424086 anylabeling-0.1.5/
--rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.1.5/LICENSE
--rw-r--r--   0 vietanhdev   (501) staff       (20)      113 2023-04-12 17:03:45.000000 anylabeling-0.1.5/MANIFEST.in
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-14 02:34:17.423927 anylabeling-0.1.5/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1921 2023-04-12 01:16:28.000000 anylabeling-0.1.5/README.md
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.404389 anylabeling-0.1.5/anylabeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       67 2023-04-12 17:16:44.000000 anylabeling-0.1.5/anylabeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      927 2023-04-13 15:24:26.000000 anylabeling-0.1.5/anylabeling/app.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      114 2023-04-14 02:34:01.000000 anylabeling-0.1.5/anylabeling/app_info.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.405863 anylabeling-0.1.5/anylabeling/configs/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/configs/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.406056 anylabeling-0.1.5/anylabeling/configs/__pycache__/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.1.5/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/configs/anylabeling_config.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)      316 2023-04-12 17:03:45.000000 anylabeling-0.1.5/anylabeling/configs/autolabel_segment_anything.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1172 2023-04-12 17:03:45.000000 anylabeling-0.1.5/anylabeling/configs/autolabel_yolov5m.yaml
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1172 2023-04-12 17:03:45.000000 anylabeling-0.1.5/anylabeling/configs/autolabel_yolov5s.yaml
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.406516 anylabeling-0.1.5/anylabeling/resources/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/resources/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)   477720 2023-04-12 17:04:48.000000 anylabeling-0.1.5/anylabeling/resources/resources.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.406965 anylabeling-0.1.5/anylabeling/services/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/services/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.407752 anylabeling-0.1.5/anylabeling/services/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3537 2023-04-13 15:20:55.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5371 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9870 2023-04-12 17:27:56.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1335 2023-04-12 17:29:20.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5286 2023-04-12 17:30:50.000000 anylabeling-0.1.5/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/utils.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.407975 anylabeling-0.1.5/anylabeling/views/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/views/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.408324 anylabeling-0.1.5/anylabeling/views/common/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/views/common/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.1.5/anylabeling/views/common/tableview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9583 2023-04-12 17:30:44.000000 anylabeling-0.1.5/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.409521 anylabeling-0.1.5/anylabeling/views/labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:53:51.000000 anylabeling-0.1.5/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5590 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/labeling/__main__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2771 2023-04-12 17:31:48.000000 anylabeling-0.1.5/anylabeling/views/labeling/config.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.420933 anylabeling-0.1.5/anylabeling/views/labeling/icons/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/.DS_Store
--rw-r--r--   0 vietanhdev   (501) staff       (20)        8 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/app.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)    31379 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/app.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1645 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/app.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/cancel.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/cartesian.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/circle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/color-line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/color.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/color_line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/copy.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/delete.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/done.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/done.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/edit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/expert.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/expert1.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/expert2.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/eye.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/feBlend-icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/file.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/fit-width.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/fit-window.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/fit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/format_createml.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/format_voc.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/format_yolo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/help.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)  1128131 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/icon.icns
--rw-r--r--   0 vietanhdev   (501) staff       (20)   183198 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/icon.ico
--rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/icon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/labels.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    36597 2023-04-12 17:03:45.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/labels.svg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/line-strip.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/line.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/new.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/next.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/objects.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/open.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/paste.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/point.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/polygon.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/prev.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/quit.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/rectangle.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/resetall.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/save-as.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/save.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/undo-cross.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/undo.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/upload_brain.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/verify.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom-in.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom-out.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom.png
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5995 2023-04-12 17:33:36.000000 anylabeling-0.1.5/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    89248 2023-04-14 02:33:50.000000 anylabeling-0.1.5/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.1.5/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1786 2023-04-12 01:57:00.000000 anylabeling-0.1.5/anylabeling/views/labeling/logger.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    10441 2023-04-12 17:34:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/shape.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.421776 anylabeling-0.1.5/anylabeling/views/labeling/utils/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-12 17:21:05.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.423316 anylabeling-0.1.5/anylabeling/views/labeling/widgets/
--rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.423707 anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     7373 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)    46656 2023-04-14 02:33:50.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     8027 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5780 2023-04-12 17:34:51.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-14 02:24:11.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.1.5/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 vietanhdev   (501) staff       (20)      915 2023-04-12 16:58:37.000000 anylabeling-0.1.5/anylabeling/views/mainwindow.py
-drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 02:34:17.405230 anylabeling-0.1.5/anylabeling.egg-info/
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2757 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 vietanhdev   (501) staff       (20)     5055 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      188 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/requires.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-14 02:34:17.000000 anylabeling-0.1.5/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 vietanhdev   (501) staff       (20)      175 2023-04-12 17:16:19.000000 anylabeling-0.1.5/pyproject.toml
--rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-14 02:34:17.424131 anylabeling-0.1.5/setup.cfg
--rw-r--r--   0 vietanhdev   (501) staff       (20)     2333 2023-04-13 15:22:05.000000 anylabeling-0.1.5/setup.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:44.003970 anylabeling-0.1.6/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    35149 2023-04-08 18:49:24.000000 anylabeling-0.1.6/LICENSE
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      113 2023-04-12 17:03:45.000000 anylabeling-0.1.6/MANIFEST.in
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2965 2023-04-14 19:17:44.003812 anylabeling-0.1.6/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2129 2023-04-14 18:24:46.000000 anylabeling-0.1.6/README.md
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.987513 anylabeling-0.1.6/anylabeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       67 2023-04-12 17:16:44.000000 anylabeling-0.1.6/anylabeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      927 2023-04-13 15:24:26.000000 anylabeling-0.1.6/anylabeling/app.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      114 2023-04-14 19:12:33.000000 anylabeling-0.1.6/anylabeling/app_info.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.990586 anylabeling-0.1.6/anylabeling/configs/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/configs/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.990710 anylabeling-0.1.6/anylabeling/configs/__pycache__/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      166 2023-04-08 18:50:19.000000 anylabeling-0.1.6/anylabeling/configs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/configs/anylabeling_config.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      388 2023-04-14 18:53:48.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_segment_anything.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:53:56.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5l.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:53:58.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5m.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:01.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5n.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5s.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5x.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8l.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8m.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8n.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:20.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8s.yaml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1223 2023-04-14 18:54:17.000000 anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8x.yaml
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.990927 anylabeling-0.1.6/anylabeling/resources/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/resources/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)   477720 2023-04-12 17:04:48.000000 anylabeling-0.1.6/anylabeling/resources/resources.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.991523 anylabeling-0.1.6/anylabeling/services/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/services/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.992329 anylabeling-0.1.6/anylabeling/services/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4337 2023-04-14 19:03:06.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6106 2023-04-14 19:00:06.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10178 2023-04-14 18:55:46.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1335 2023-04-12 17:29:20.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5329 2023-04-14 19:02:27.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5089 2023-04-14 19:02:27.000000 anylabeling-0.1.6/anylabeling/services/auto_labeling/yolov8.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      379 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/utils.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.992536 anylabeling-0.1.6/anylabeling/views/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/views/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.992863 anylabeling-0.1.6/anylabeling/views/common/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/views/common/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1326 2023-04-08 18:49:39.000000 anylabeling-0.1.6/anylabeling/views/common/tableview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9583 2023-04-12 17:30:44.000000 anylabeling-0.1.6/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.994006 anylabeling-0.1.6/anylabeling/views/labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        0 2023-04-12 01:53:51.000000 anylabeling-0.1.6/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5590 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/labeling/__main__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2771 2023-04-12 17:31:48.000000 anylabeling-0.1.6/anylabeling/views/labeling/config.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:44.000657 anylabeling-0.1.6/anylabeling/views/labeling/icons/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6148 2023-04-09 05:07:05.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/.DS_Store
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    28068 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6844 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/cancel.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    11383 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/cartesian.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15818 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/circle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/color-line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    23824 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/color.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2368 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/color_line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10021 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/copy.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7842 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/delete.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2198 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/done.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22232 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/done.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    15023 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/edit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7718 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/expert.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      278 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/expert1.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      335 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/expert2.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    37652 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/eye.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8059 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/feBlend-icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/file.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    17368 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/fit-width.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2186 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/fit-window.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2262 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/fit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4156 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/format_createml.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      786 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/format_voc.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      675 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/format_yolo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14479 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/help.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    44771 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/icon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2381 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/labels.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    36597 2023-04-12 17:03:45.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/labels.svg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7253 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/line-strip.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     9457 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/line.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      977 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/new.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7482 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/next.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    26255 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/objects.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4886 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/open.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10572 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/paste.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    13847 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/point.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    14286 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/polygon.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7275 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/prev.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    22460 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/quit.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2136 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/rectangle.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3637 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/resetall.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2811 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/save-as.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     6118 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/save.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2004 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/undo-cross.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2018 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/undo.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    18083 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/upload_brain.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3041 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/verify.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1099 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom-in.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1074 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom-out.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1139 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom.png
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5995 2023-04-12 17:33:36.000000 anylabeling-0.1.6/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    90545 2023-04-14 19:10:28.000000 anylabeling-0.1.6/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      610 2023-04-12 01:47:51.000000 anylabeling-0.1.6/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1786 2023-04-12 01:57:00.000000 anylabeling-0.1.6/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    10441 2023-04-12 17:34:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      870 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:44.001429 anylabeling-0.1.6/anylabeling/views/labeling/utils/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      526 2023-04-12 17:21:05.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      668 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2339 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      218 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2449 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     3598 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:44.003171 anylabeling-0.1.6/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      492 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:44.003603 anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       29 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     7373 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     4146 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1670 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)    46999 2023-04-14 17:35:30.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1204 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      301 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2429 2023-04-08 19:49:25.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     8027 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5780 2023-04-12 17:34:51.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1394 2023-04-12 01:47:30.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     1260 2023-04-14 02:24:11.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      779 2023-04-11 17:52:02.000000 anylabeling-0.1.6/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      915 2023-04-12 16:58:37.000000 anylabeling-0.1.6/anylabeling/views/mainwindow.py
+drwxr-xr-x   0 vietanhdev   (501) staff       (20)        0 2023-04-14 19:17:43.988330 anylabeling-0.1.6/anylabeling.egg-info/
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2965 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     5235 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)        1 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       53 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      188 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       12 2023-04-14 19:17:43.000000 anylabeling-0.1.6/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 vietanhdev   (501) staff       (20)      267 2023-04-14 19:13:58.000000 anylabeling-0.1.6/pyproject.toml
+-rw-r--r--   0 vietanhdev   (501) staff       (20)       38 2023-04-14 19:17:44.004015 anylabeling-0.1.6/setup.cfg
+-rw-r--r--   0 vietanhdev   (501) staff       (20)     2333 2023-04-13 15:22:05.000000 anylabeling-0.1.6/setup.py
```

### Comparing `anylabeling-0.1.5/LICENSE` & `anylabeling-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/PKG-INFO` & `anylabeling-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.1.5
+Version: 0.1.6
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
@@ -42,54 +42,70 @@
 ## I. Install and run
 
 - Requirements: Python >= 3.8
 - Recommended: Miniconda/Anaconda <https://docs.conda.io/en/latest/miniconda.html>
 
 - Create environment:
 
-```
+```bash
 conda create -n anylabeling python=3.8
 conda activate anylabeling
 ```
 
 - **(For macOS only)** Install PyQt5 using Conda:
 
-```
+```bash
 conda install -c conda-forge pyqt==5.15.7
 ```
 
 - Install anylabeling:
 
-```
+```bash
 pip install anylabeling
 ```
 
 - Run app:
 
-```
+```bash
 anylabeling
 ```
 
 Or
 
-```
+```bash
 python -m anylabeling.app
 ```
 
 ## II. Development
 
 - Generate resources:
 
-```
+```bash
 pyrcc5 -o anylabeling/resources/resources.py anylabeling/resources/resources.qrc
 ```
 
 - Run app:
 
-```
+```bash
 python anylabeling/app.py
 ```
 
-## III. References
+## III. Build executable
+
+- Install PyInstaller:
+
+```bash
+pip install -r requirements-dev.txt
+```
+
+- Build:
+
+```bash
+bash build_executable.sh
+```
+
+- Check the outputs in: `dist/`.
+
+## IV. References
 
 - Labeling UI built with ideas and components from [LabelImg](https://github.com/heartexlabs/labelImg), [labelme](https://github.com/wkentaro/labelme).
 - Icons: Flat Icons
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.1.5 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.1.6 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -18,17 +18,20 @@
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
 isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/issues) [![Pypi Downloads](https://pepy.tech/badge/
 anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] **Youtube
 Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/
 watch?v=5iQSGL7ebXE) ## I. Install and run - Requirements: Python >= 3.8 -
 Recommended: Miniconda/Anaconda
-docs.conda.io/en/latest/miniconda.html> - Create environment: ``` conda create
--n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS only)**
-Install PyQt5 using Conda: ``` conda install -c conda-forge pyqt==5.15.7 ``` -
-Install anylabeling: ``` pip install anylabeling ``` - Run app: ``` anylabeling
-``` Or ``` python -m anylabeling.app ``` ## II. Development - Generate
-resources: ``` pyrcc5 -o anylabeling/resources/resources.py anylabeling/
-resources/resources.qrc ``` - Run app: ``` python anylabeling/app.py ``` ##
-III. References - Labeling UI built with ideas and components from [LabelImg]
-(https://github.com/heartexlabs/labelImg), [labelme](https://github.com/
-wkentaro/labelme). - Icons: Flat Icons
+docs.conda.io/en/latest/miniconda.html> - Create environment: ```bash conda
+create -n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS
+only)** Install PyQt5 using Conda: ```bash conda install -c conda-forge
+pyqt==5.15.7 ``` - Install anylabeling: ```bash pip install anylabeling ``` -
+Run app: ```bash anylabeling ``` Or ```bash python -m anylabeling.app ``` ##
+II. Development - Generate resources: ```bash pyrcc5 -o anylabeling/resources/
+resources.py anylabeling/resources/resources.qrc ``` - Run app: ```bash python
+anylabeling/app.py ``` ## III. Build executable - Install PyInstaller: ```bash
+pip install -r requirements-dev.txt ``` - Build: ```bash bash
+build_executable.sh ``` - Check the outputs in: `dist/`. ## IV. References -
+Labeling UI built with ideas and components from [LabelImg](https://github.com/
+heartexlabs/labelImg), [labelme](https://github.com/wkentaro/labelme). - Icons:
+Flat Icons
```

### Comparing `anylabeling-0.1.5/README.md` & `anylabeling-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -20,54 +20,70 @@
 ## I. Install and run
 
 - Requirements: Python >= 3.8
 - Recommended: Miniconda/Anaconda <https://docs.conda.io/en/latest/miniconda.html>
 
 - Create environment:
 
-```
+```bash
 conda create -n anylabeling python=3.8
 conda activate anylabeling
 ```
 
 - **(For macOS only)** Install PyQt5 using Conda:
 
-```
+```bash
 conda install -c conda-forge pyqt==5.15.7
 ```
 
 - Install anylabeling:
 
-```
+```bash
 pip install anylabeling
 ```
 
 - Run app:
 
-```
+```bash
 anylabeling
 ```
 
 Or
 
-```
+```bash
 python -m anylabeling.app
 ```
 
 ## II. Development
 
 - Generate resources:
 
-```
+```bash
 pyrcc5 -o anylabeling/resources/resources.py anylabeling/resources/resources.qrc
 ```
 
 - Run app:
 
-```
+```bash
 python anylabeling/app.py
 ```
 
-## III. References
+## III. Build executable
+
+- Install PyInstaller:
+
+```bash
+pip install -r requirements-dev.txt
+```
+
+- Build:
+
+```bash
+bash build_executable.sh
+```
+
+- Check the outputs in: `dist/`.
+
+## IV. References
 
 - Labeling UI built with ideas and components from [LabelImg](https://github.com/heartexlabs/labelImg), [labelme](https://github.com/wkentaro/labelme).
 - Icons: Flat Icons
```

#### html2text {}

```diff
@@ -7,17 +7,20 @@
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
 isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/issues) [![Pypi Downloads](https://pepy.tech/badge/
 anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] **Youtube
 Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/
 watch?v=5iQSGL7ebXE) ## I. Install and run - Requirements: Python >= 3.8 -
 Recommended: Miniconda/Anaconda
-docs.conda.io/en/latest/miniconda.html> - Create environment: ``` conda create
--n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS only)**
-Install PyQt5 using Conda: ``` conda install -c conda-forge pyqt==5.15.7 ``` -
-Install anylabeling: ``` pip install anylabeling ``` - Run app: ``` anylabeling
-``` Or ``` python -m anylabeling.app ``` ## II. Development - Generate
-resources: ``` pyrcc5 -o anylabeling/resources/resources.py anylabeling/
-resources/resources.qrc ``` - Run app: ``` python anylabeling/app.py ``` ##
-III. References - Labeling UI built with ideas and components from [LabelImg]
-(https://github.com/heartexlabs/labelImg), [labelme](https://github.com/
-wkentaro/labelme). - Icons: Flat Icons
+docs.conda.io/en/latest/miniconda.html> - Create environment: ```bash conda
+create -n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS
+only)** Install PyQt5 using Conda: ```bash conda install -c conda-forge
+pyqt==5.15.7 ``` - Install anylabeling: ```bash pip install anylabeling ``` -
+Run app: ```bash anylabeling ``` Or ```bash python -m anylabeling.app ``` ##
+II. Development - Generate resources: ```bash pyrcc5 -o anylabeling/resources/
+resources.py anylabeling/resources/resources.qrc ``` - Run app: ```bash python
+anylabeling/app.py ``` ## III. Build executable - Install PyInstaller: ```bash
+pip install -r requirements-dev.txt ``` - Build: ```bash bash
+build_executable.sh ``` - Check the outputs in: `dist/`. ## IV. References -
+Labeling UI built with ideas and components from [LabelImg](https://github.com/
+heartexlabs/labelImg), [labelme](https://github.com/wkentaro/labelme). - Icons:
+Flat Icons
```

### Comparing `anylabeling-0.1.5/anylabeling/app.py` & `anylabeling-0.1.6/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.1.6/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/configs/autolabel_yolov5m.yaml` & `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov8x.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-type: yolov5
-name: yolov5m
-display_name: YOLOv5m Ultralytics
-model_path: anylabeling_assets/models/yolov5/yolov5m.onnx
+type: yolov8
+name: yolov8x-r20230415
+display_name: YOLOv8x Ultralytics
+model_path: https://github.com/vietanhdev/anylabeling-assets/releases/download/v0.0.1/yolov8x.onnx
 input_width: 640
 input_height: 640
 score_threshold: 0.5
 nms_threshold: 0.45
 confidence_threshold: 0.45
 classes:
   - person
```

### Comparing `anylabeling-0.1.5/anylabeling/configs/autolabel_yolov5s.yaml` & `anylabeling-0.1.6/anylabeling/configs/autolabel_yolov5l.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 type: yolov5
-name: yolov5s
-display_name: YOLOv5s Ultralytics
-model_path: anylabeling_assets/models/yolov5/yolov5s.onnx
+name: yolov5l-r20230415
+display_name: YOLOv5l Ultralytics
+model_path: https://github.com/vietanhdev/anylabeling-assets/releases/download/v0.0.1/yolov5l.onnx
 input_width: 640
 input_height: 640
 score_threshold: 0.5
 nms_threshold: 0.45
 confidence_threshold: 0.45
 classes:
   - person
```

### Comparing `anylabeling-0.1.5/anylabeling/resources/resources.py` & `anylabeling-0.1.6/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.1.6/anylabeling/services/auto_labeling/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,61 +37,85 @@
 
     def get_required_buttons(self):
         """
         Get required buttons for showing in UI
         """
         return self.Meta.buttons
 
-    def get_model_abs_path(self, model_path):
+    def get_model_abs_path(self, model_path, model_folder_name):
         """
         Get model absolute path from config path or download from url
         """
         # Try getting model path from config folder
         model_abs_path = os.path.abspath(model_path)
         if os.path.exists(model_abs_path):
             return model_abs_path
 
-        # Try download model from url
+        self.on_message(
+            "Downloading model from model registry. This may take a while..."
+        )
+
+        # Build download url
+        filename = os.path.basename(model_path)
         if model_path.startswith("anylabeling_assets/"):
-            self.on_message(
-                "Downloading model from model registry. This may take a"
-                " while..."
-            )
-            relative_path = model_path.replace("anylabeling_assets/", "")
-            download_url = self.BASE_DOWNLOAD_URL + relative_path
-            home_dir = os.path.expanduser("~")
-            model_abs_path = os.path.abspath(
-                os.path.join(home_dir, "anylabeling_data", relative_path)
+            download_url = (
+                self.BASE_DOWNLOAD_URL
+                + model_path[len("anylabeling_assets/") :]
             )
-            if os.path.exists(model_abs_path):
-                return model_abs_path
-            pathlib.Path(model_abs_path).parent.mkdir(
-                parents=True, exist_ok=True
+        elif model_path.startswith(("http://", "https://")):
+            download_url = model_path
+        else:
+            raise Exception(
+                f"Unknown model path: {model_path}. "
+                "Model path must start with anylabeling_assets/ or "
+                "http:// or https://"
             )
 
-            # Download model from url
-            logging.info(
-                f"Downloading model from {download_url} to {model_abs_path}"
+        # Create model folder
+        home_dir = os.path.expanduser("~")
+        model_abs_path = os.path.abspath(
+            os.path.join(
+                home_dir,
+                "anylabeling_data",
+                "models",
+                model_folder_name,
+                filename,
             )
+        )
+        if os.path.exists(model_abs_path):
+            return model_abs_path
+        pathlib.Path(model_abs_path).parent.mkdir(parents=True, exist_ok=True)
 
-            try:
-                data = urllib.request.urlopen(download_url).read()
-                with open(model_abs_path, "wb") as f:
-                    f.write(data)
-            except Exception as e:  # noqa
+        # Download model from url
+        ellipsis_download_url = download_url
+        if len(download_url) > 40:
+            ellipsis_download_url = (
+                download_url[:20] + "..." + download_url[-20:]
+            )
+        logging.info(
+            f"Downloading model from {ellipsis_download_url} to {model_abs_path}"
+        )
+        try:
+            # Download and show progress
+            def _progress(count, block_size, total_size):
+                percent = int(count * block_size * 100 / total_size)
                 self.on_message(
-                    f"Could not downloading model from {download_url}"
+                    f"Downloading model from {ellipsis_download_url}: {percent}%"
                 )
-                raise Exception(
-                    f"Could not downloading model from {download_url}: {e}"
-                ) from e
 
-            return model_abs_path
+            urllib.request.urlretrieve(
+                download_url, model_abs_path, reporthook=_progress
+            )
+        except Exception as e:  # noqa
+            self.on_message(f"Could not download model from {download_url}")
+            raise Exception(
+                f"Could not download model from {download_url}: {e}"
+            ) from e
 
-        return None
+        return model_abs_path
 
     def check_missing_config(self, config_names, config):
         """
         Check if config has all required config names
         """
         for name in config_names:
             if name not in config:
```

### Comparing `anylabeling-0.1.5/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.1.6/anylabeling/services/auto_labeling/model_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,25 @@
     new_model_status = pyqtSignal(str)
     model_loaded = pyqtSignal(list)
     new_auto_labeling_result = pyqtSignal(AutoLabelingResult)
     auto_segmentation_model_selected = pyqtSignal()
     auto_segmentation_model_unselected = pyqtSignal()
 
     model_configs = {
-        "segment_anything_vit_b": "autolabel_segment_anything.yaml",
-        "yolov5s": "autolabel_yolov5s.yaml",
-        "yolov5m": "autolabel_yolov5m.yaml",
+        "segment_anything_vit_b-r20230415": "autolabel_segment_anything.yaml",
+        "yolov5n-r20230415": "autolabel_yolov5n.yaml",
+        "yolov5s-r20230415": "autolabel_yolov5s.yaml",
+        "yolov5m-r20230415": "autolabel_yolov5m.yaml",
+        "yolov5l-r20230415": "autolabel_yolov5l.yaml",
+        "yolov5x-r20230415": "autolabel_yolov5x.yaml",
+        "yolov8n-r20230415": "autolabel_yolov8n.yaml",
+        "yolov8s-r20230415": "autolabel_yolov8s.yaml",
+        "yolov8m-r20230415": "autolabel_yolov8m.yaml",
+        "yolov8l-r20230415": "autolabel_yolov8l.yaml",
+        "yolov8x-r20230415": "autolabel_yolov8x.yaml",
     }
 
     def __init__(self):
         super().__init__()
         self.model_infos = {}
         for model_name, config_name in ModelManager.model_configs.items():
             self.model_infos[model_name] = {}
@@ -100,22 +108,28 @@
         """Load and return model info"""
         if self.loaded_model_info is not None:
             self.loaded_model_info["model"].unload()
             self.loaded_model_info = None
             self.auto_segmentation_model_unselected.emit()
 
         model_info = copy.deepcopy(self.model_infos[model_name])
-
         if model_info["type"] == "yolov5":
             from .yolov5 import YOLOv5
 
             model_info["model"] = YOLOv5(
                 model_info, on_message=self.new_model_status.emit
             )
             self.auto_segmentation_model_unselected.emit()
+        elif model_info["type"] == "yolov8":
+            from .yolov8 import YOLOv8
+
+            model_info["model"] = YOLOv8(
+                model_info, on_message=self.new_model_status.emit
+            )
+            self.auto_segmentation_model_unselected.emit()
         elif model_info["type"] == "segment_anything":
             from .segment_anything import SegmentAnything
 
             model_info["model"] = SegmentAnything(
                 model_info, on_message=self.new_model_status.emit
             )
             self.auto_segmentation_model_selected.emit()
```

### Comparing `anylabeling-0.1.5/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.1.6/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,30 +39,36 @@
         super().__init__(config_path, on_message)
         self.input_size = self.config["input_size"]
         self.max_width = self.config["max_width"]
         self.max_height = self.config["max_height"]
 
         # Get encoder and decoder model paths
         encoder_model_abs_path = self.get_model_abs_path(
-            self.config["encoder_model_path"]
+            self.config["encoder_model_path"], self.config["name"]
         )
         if not os.path.isfile(encoder_model_abs_path):
             raise Exception(f"Encoder not found: {encoder_model_abs_path}")
         decoder_model_abs_path = self.get_model_abs_path(
-            self.config["decoder_model_path"]
+            self.config["decoder_model_path"], self.config["name"]
         )
         if not os.path.isfile(decoder_model_abs_path):
             raise Exception(f"Decoder not found: {decoder_model_abs_path}")
 
         # Load models
+        cuda = True if onnxruntime.get_device() == "GPU" else False
+        providers = (
+            ["CUDAExecutionProvider", "CPUExecutionProvider"]
+            if cuda
+            else ["CPUExecutionProvider"]
+        )
         self.encoder_session = onnxruntime.InferenceSession(
-            encoder_model_abs_path
+            encoder_model_abs_path, providers=providers
         )
         self.decoder_session = onnxruntime.InferenceSession(
-            decoder_model_abs_path
+            decoder_model_abs_path, providers=providers
         )
 
         # Mark for auto labeling
         # points, rectangles
         self.marks = []
 
         self.last_image = None
```

### Comparing `anylabeling-0.1.5/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.1.6/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.1.6/anylabeling/services/auto_labeling/yolov5.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,17 @@
         ]
         buttons = ["button_run"]
 
     def __init__(self, model_config, on_message) -> None:
         # Run the parent class's init method
         super().__init__(model_config, on_message)
 
-        model_abs_path = self.get_model_abs_path(self.config["model_path"])
+        model_abs_path = self.get_model_abs_path(
+            self.config["model_path"], self.config["name"]
+        )
         if not os.path.isfile(model_abs_path):
             raise Exception(f"Model not found: {model_abs_path}")
 
         self.net = cv2.dnn.readNet(model_abs_path)
         self.net.setPreferableBackend(cv2.dnn.DNN_BACKEND_CUDA)
         self.net.setPreferableTarget(cv2.dnn.DNN_TARGET_CUDA)
         self.classes = self.config["classes"]
```

### Comparing `anylabeling-0.1.5/anylabeling/views/common/tableview.py` & `anylabeling-0.1.6/anylabeling/views/common/tableview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/common/toaster.py` & `anylabeling-0.1.6/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/__main__.py` & `anylabeling-0.1.6/anylabeling/views/labeling/__main__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/config.py` & `anylabeling-0.1.6/anylabeling/views/labeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/.DS_Store` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/brain.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/cancel.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/cartesian.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/cartesian.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/circle.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/circle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/color-line.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/color.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/color.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/color_line.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/color_line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/copy.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/copy.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/delete.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/delete.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/done.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/done.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/done.svg` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/done.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/edit.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/edit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/expert.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/expert.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/eye.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/eye.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/feBlend-icon.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/file.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/file.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/fit-width.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/fit-window.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/fit.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/fit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/format_createml.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/format_createml.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/format_voc.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/format_voc.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/format_yolo.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/format_yolo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/help.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/help.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/icon.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/icon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/labels.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/labels.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/labels.svg` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/line-strip.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/line-strip.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/line.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/line.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/new.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/new.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/next.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/next.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/objects.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/objects.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/open.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/open.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/paste.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/paste.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/point.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/point.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/polygon.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/prev.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/prev.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/quit.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/quit.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/rectangle.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/resetall.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/resetall.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/save-as.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/save.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/save.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/undo-cross.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/undo.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/undo.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/upload_brain.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/upload_brain.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/verify.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/verify.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom-in.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom-out.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/icons/zoom.png` & `anylabeling-0.1.6/anylabeling/views/labeling/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/label_file.py` & `anylabeling-0.1.6/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.1.6/anylabeling/views/labeling/label_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1150,15 +1150,26 @@
         In the middle of drawing, toggling between modes should be disabled.
         """
         self.actions.edit_mode.setEnabled(not drawing)
         self.actions.undo_last_point.setEnabled(drawing)
         self.actions.undo.setEnabled(not drawing)
         self.actions.delete.setEnabled(not drawing)
 
-    def toggle_draw_mode(self, edit=True, create_mode="rectangle"):
+    def toggle_draw_mode(
+        self, edit=True, create_mode="rectangle", disable_auto_labeling=True
+    ):
+        # Disable auto labeling if needed
+        if (
+            disable_auto_labeling
+            and self.auto_labeling_widget.auto_labeling_mode
+            != AutoLabelingMode.NONE
+        ):
+            self.clear_auto_labeling_marks()
+            self.auto_labeling_widget.set_auto_labeling_mode(None)
+
         self.canvas.set_editing(edit)
         self.canvas.create_mode = create_mode
         if edit:
             self.actions.create_mode.setEnabled(True)
             self.actions.create_rectangle_mode.setEnabled(True)
             self.actions.create_cirle_mode.setEnabled(True)
             self.actions.create_line_mode.setEnabled(True)
@@ -1366,15 +1377,23 @@
         label_list_item = LabelListWidgetItem(text, shape)
         self.label_list.add_iem(label_list_item)
         if not self.unique_label_list.find_items_by_label(shape.label):
             item = self.unique_label_list.create_item_from_label(shape.label)
             self.unique_label_list.addItem(item)
             rgb = self._get_rgb_by_label(shape.label)
             self.unique_label_list.set_item_label(item, shape.label, rgb)
-        self.label_dialog.add_label_history(shape.label)
+
+        # Add label to history if it is not a special label
+        if shape.label not in [
+            AutoLabelingMode.OBJECT,
+            AutoLabelingMode.ADD,
+            AutoLabelingMode.REMOVE,
+        ]:
+            self.label_dialog.add_label_history(shape.label)
+
         for action in self.actions.on_shapes_present:
             action.setEnabled(True)
 
         self._update_shape_color(shape)
         label_list_item.setText(
             '{} <font color="#{:02x}{:02x}{:02x}">●</font>'.format(
                 html.escape(text), *shape.fill_color.getRgb()[:3]
@@ -1598,32 +1617,39 @@
         group_id = None
 
         if self.canvas.shapes[-1].label in [
             AutoLabelingMode.ADD,
             AutoLabelingMode.REMOVE,
         ]:
             text = self.canvas.shapes[-1].label
-        elif self._config["display_label_popup"] or not text:
+        elif (
+            self._config["display_label_popup"]
+            or not text
+            or self.canvas.shapes[-1].label == AutoLabelingMode.OBJECT
+        ):
             previous_text = self.label_dialog.edit.text()
             text, flags, group_id = self.label_dialog.pop_up(text)
             if not text:
                 self.label_dialog.edit.setText(previous_text)
 
         if text and not self.validate_label(text):
             self.error_message(
                 self.tr("Invalid label"),
                 self.tr("Invalid label '{}' with validation type '{}'").format(
                     text, self._config["validate_label"]
                 ),
             )
             text = ""
+            return
+
         if text:
             self.label_list.clearSelection()
             shape = self.canvas.set_last_label(text, flags)
             shape.group_id = group_id
+            shape.label = text
             self.add_label(shape)
             self.actions.edit_mode.setEnabled(True)
             self.actions.undo_last_point.setEnabled(False)
             self.actions.undo.setEnabled(True)
             self.set_dirty()
         else:
             self.canvas.undo_last_line()
@@ -2425,34 +2451,51 @@
                 AutoLabelingMode.OBJECT,
                 AutoLabelingMode.ADD,
                 AutoLabelingMode.REMOVE,
             ]
         ]
         self.canvas.update()
 
+    def find_last_label(self):
+        """
+        Find the last label in the label list.
+        Exclude labels for auto labeling.
+        """
+        for item in reversed(self.label_list):
+            shape = item.data(Qt.UserRole)
+            if shape.label not in [
+                AutoLabelingMode.OBJECT,
+                AutoLabelingMode.ADD,
+                AutoLabelingMode.REMOVE,
+            ]:
+                return shape.label
+        return ""
+
     def finish_auto_labeling_object(self):
         """Finish auto labeling object."""
         has_object = False
         for shape in self.canvas.shapes:
             if shape.label == AutoLabelingMode.OBJECT:
                 has_object = True
                 break
 
         # If there is no object, do nothing
         if not has_object:
             return
 
         # Ask a label for the object
+        previous_text = self.label_dialog.edit.text()
         text, flags, group_id = self.label_dialog.pop_up(
-            text="",
+            text=self.find_last_label(),
             flags={},
             group_id=None,
         )
-        if text is None:
-            return
+        if not text:
+            self.label_dialog.edit.setText(previous_text)
+
         if not self.validate_label(text):
             self.error_message(
                 self.tr("Invalid label"),
                 self.tr("Invalid label '{}' with validation type '{}'").format(
                     text, self._config["validate_label"]
                 ),
             )
```

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.1.6/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/logger.py` & `anylabeling-0.1.6/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/shape.py` & `anylabeling-0.1.6/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/testing.py` & `anylabeling-0.1.6/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/utils/__init__.py` & `anylabeling-0.1.6/anylabeling/views/labeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.1.6/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.1.6/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.1.6/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.1.6/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,17 @@
         if mode == AutoLabelingMode.NONE:
             self.is_auto_labeling = False
             self.auto_labeling_mode = mode
         else:
             self.is_auto_labeling = True
             self.auto_labeling_mode = mode
             self.create_mode = mode.shape_type
-            self.parent.toggle_draw_mode(False, mode.shape_type)
+            self.parent.toggle_draw_mode(
+                False, mode.shape_type, disable_auto_labeling=False
+            )
 
     def fill_drawing(self):
         """Get option to fill shapes by color"""
         return self._fill_drawing
 
     def set_fill_drawing(self, value):
         """Set shape filling option"""
@@ -197,15 +199,17 @@
         return self.mode == self.EDIT
 
     def set_auto_labeling(self, value=True):
         """Set auto labeling mode"""
         self.is_auto_labeling = value
         if self.auto_labeling_mode is None:
             self.auto_labeling_mode = AutoLabelingMode.NONE
-            self.parent.toggle_draw_mode(False, "rectangle")
+            self.parent.toggle_draw_mode(
+                False, "rectangle", disable_auto_labeling=True
+            )
 
     def get_mode(self):
         """Get current mode"""
         if self.is_auto_labeling:
             return "Auto Labeling"
         if self.mode == self.CREATE:
             return "Drawing"
@@ -861,16 +865,22 @@
             return True
         w, h = self.pixmap.width(), self.pixmap.height()
         return not (0 <= p.x() <= w - 1 and 0 <= p.y() <= h - 1)
 
     def finalise(self):
         """Finish drawing for a shape"""
         assert self.current
-        if self.is_auto_labeling:
+        if (
+            self.is_auto_labeling
+            and self.auto_labeling_mode != AutoLabelingMode.NONE
+        ):
             self.current.label = self.auto_labeling_mode.edit_mode
+        # TODO(vietanhdev): Temporrally fix. Need to refactor
+        if self.current.label is None:
+            self.current.label = ""
         self.current.close()
         # Sort tl -> br for rectangle
         if self.current.shape_type == "rectangle":
             x_min = min(self.current.points[0].x(), self.current.points[1].x())
             y_min = min(self.current.points[0].y(), self.current.points[1].y())
             x_max = max(self.current.points[0].x(), self.current.points[1].x())
             y_max = max(self.current.points[0].y(), self.current.points[1].y())
```

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.1.6/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling/views/mainwindow.py` & `anylabeling-0.1.6/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.1.5/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.1.6/anylabeling.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.1.5
+Version: 0.1.6
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
@@ -42,54 +42,70 @@
 ## I. Install and run
 
 - Requirements: Python >= 3.8
 - Recommended: Miniconda/Anaconda <https://docs.conda.io/en/latest/miniconda.html>
 
 - Create environment:
 
-```
+```bash
 conda create -n anylabeling python=3.8
 conda activate anylabeling
 ```
 
 - **(For macOS only)** Install PyQt5 using Conda:
 
-```
+```bash
 conda install -c conda-forge pyqt==5.15.7
 ```
 
 - Install anylabeling:
 
-```
+```bash
 pip install anylabeling
 ```
 
 - Run app:
 
-```
+```bash
 anylabeling
 ```
 
 Or
 
-```
+```bash
 python -m anylabeling.app
 ```
 
 ## II. Development
 
 - Generate resources:
 
-```
+```bash
 pyrcc5 -o anylabeling/resources/resources.py anylabeling/resources/resources.qrc
 ```
 
 - Run app:
 
-```
+```bash
 python anylabeling/app.py
 ```
 
-## III. References
+## III. Build executable
+
+- Install PyInstaller:
+
+```bash
+pip install -r requirements-dev.txt
+```
+
+- Build:
+
+```bash
+bash build_executable.sh
+```
+
+- Check the outputs in: `dist/`.
+
+## IV. References
 
 - Labeling UI built with ideas and components from [LabelImg](https://github.com/heartexlabs/labelImg), [labelme](https://github.com/wkentaro/labelme).
 - Icons: Flat Icons
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.1.5 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.1.6 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -18,17 +18,20 @@
 vietanhdev/anylabeling/blob/master/LICENSE) [![open issues](https://
 isitmaintained.com/badge/open/vietanhdev/anylabeling.svg)](https://github.com/
 vietanhdev/anylabeling/issues) [![Pypi Downloads](https://pepy.tech/badge/
 anylabeling)](https://pypi.org/project/anylabeling/) [AnyLabeling] **Youtube
 Demo:** [https://www.youtube.com/watch?v=5iQSGL7ebXE](https://www.youtube.com/
 watch?v=5iQSGL7ebXE) ## I. Install and run - Requirements: Python >= 3.8 -
 Recommended: Miniconda/Anaconda
-docs.conda.io/en/latest/miniconda.html> - Create environment: ``` conda create
--n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS only)**
-Install PyQt5 using Conda: ``` conda install -c conda-forge pyqt==5.15.7 ``` -
-Install anylabeling: ``` pip install anylabeling ``` - Run app: ``` anylabeling
-``` Or ``` python -m anylabeling.app ``` ## II. Development - Generate
-resources: ``` pyrcc5 -o anylabeling/resources/resources.py anylabeling/
-resources/resources.qrc ``` - Run app: ``` python anylabeling/app.py ``` ##
-III. References - Labeling UI built with ideas and components from [LabelImg]
-(https://github.com/heartexlabs/labelImg), [labelme](https://github.com/
-wkentaro/labelme). - Icons: Flat Icons
+docs.conda.io/en/latest/miniconda.html> - Create environment: ```bash conda
+create -n anylabeling python=3.8 conda activate anylabeling ``` - **(For macOS
+only)** Install PyQt5 using Conda: ```bash conda install -c conda-forge
+pyqt==5.15.7 ``` - Install anylabeling: ```bash pip install anylabeling ``` -
+Run app: ```bash anylabeling ``` Or ```bash python -m anylabeling.app ``` ##
+II. Development - Generate resources: ```bash pyrcc5 -o anylabeling/resources/
+resources.py anylabeling/resources/resources.qrc ``` - Run app: ```bash python
+anylabeling/app.py ``` ## III. Build executable - Install PyInstaller: ```bash
+pip install -r requirements-dev.txt ``` - Build: ```bash bash
+build_executable.sh ``` - Check the outputs in: `dist/`. ## IV. References -
+Labeling UI built with ideas and components from [LabelImg](https://github.com/
+heartexlabs/labelImg), [labelme](https://github.com/wkentaro/labelme). - Icons:
+Flat Icons
```

### Comparing `anylabeling-0.1.5/setup.py` & `anylabeling-0.1.6/setup.py`

 * *Files identical despite different names*

