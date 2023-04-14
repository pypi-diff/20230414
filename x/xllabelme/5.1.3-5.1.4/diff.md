# Comparing `tmp/xllabelme-5.1.3.tar.gz` & `tmp/xllabelme-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xllabelme-5.1.3.tar", last modified: Tue Apr  4 13:48:11 2023, max compression
+gzip compressed data, was "xllabelme-5.1.4.tar", last modified: Fri Apr 14 09:39:52 2023, max compression
```

## Comparing `xllabelme-5.1.3.tar` & `xllabelme-5.1.4.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 13:48:11.163784 xllabelme-5.1.3/
--rw-rw-rw-   0        0        0      707 2020-11-09 02:22:17.000000 xllabelme-5.1.3/LICENSE
--rw-rw-rw-   0        0        0       19 2020-08-05 08:41:43.000000 xllabelme-5.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0    11738 2023-04-04 13:48:11.163784 xllabelme-5.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     9202 2022-04-20 05:38:39.000000 xllabelme-5.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 13:48:11.110141 xllabelme-5.1.3/docs/
-drwxrwxrwx   0        0        0        0 2023-04-04 13:48:11.114161 xllabelme-5.1.3/docs/man/
--rw-rw-rw-   0        0        0     2148 2020-08-05 08:41:43.000000 xllabelme-5.1.3/docs/man/labelme.1
--rw-rw-rw-   0        0        0       42 2023-04-04 13:48:11.163784 xllabelme-5.1.3/setup.cfg
--rw-rw-rw-   0        0        0     5290 2023-04-04 11:32:18.000000 xllabelme-5.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 13:48:11.119097 xllabelme-5.1.3/xllabelme/
--rw-rw-rw-   0        0        0     1072 2023-04-04 13:48:09.000000 xllabelme-5.1.3/xllabelme/__init__.py
--rw-rw-rw-   0        0        0     7166 2023-04-04 12:31:34.000000 xllabelme-5.1.3/xllabelme/__main__.py
--rw-rw-rw-   0        0        0    76366 2023-04-04 11:38:01.000000 xllabelme-5.1.3/xllabelme/app.py
-drwxrwxrwx   0        0        0        0 2023-04-04 13:48:11.126103 xllabelme-5.1.3/xllabelme/cli/
--rw-rw-rw-   0        0        0      129 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/cli/__init__.py
--rw-rw-rw-   0        0        0     1404 2022-04-20 05:42:00.000000 xllabelme-5.1.3/xllabelme/cli/draw_json.py
--rw-rw-rw-   0        0        0      667 2021-06-08 03:21:06.000000 xllabelme-5.1.3/xllabelme/cli/draw_label_png.py
--rw-rw-rw-   0        0        0     2473 2022-04-20 05:42:14.000000 xllabelme-5.1.3/xllabelme/cli/json_to_dataset.py
--rw-rw-rw-   0        0        0     2851 2022-04-20 05:42:22.000000 xllabelme-5.1.3/xllabelme/cli/on_docker.py
-drwxrwxrwx   0        0        0        0 2023-04-04 13:48:11.128099 xllabelme-5.1.3/xllabelme/config/
--rw-rw-rw-   0        0        0     2784 2021-06-08 03:21:07.000000 xllabelme-5.1.3/xllabelme/config/__init__.py
--rw-rw-rw-   0        0        0     2320 2023-04-04 02:59:12.000000 xllabelme-5.1.3/xllabelme/config/default_config.yaml
--rw-rw-rw-   0        0        0    46178 2023-04-04 11:26:42.000000 xllabelme-5.1.3/xllabelme/config/xllabellib.py
-drwxrwxrwx   0        0        0        0 2023-04-04 13:48:11.151815 xllabelme-5.1.3/xllabelme/icons/
--rw-rw-rw-   0        0        0     2136 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/cancel.png
--rw-rw-rw-   0        0        0     3111 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/close.png
--rw-rw-rw-   0        0        0     2368 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/color-line.png
--rw-rw-rw-   0        0        0     1461 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/color.png
--rw-rw-rw-   0        0        0      646 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/copy.png
--rw-rw-rw-   0        0        0     1486 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/delete.png
--rw-rw-rw-   0        0        0     2198 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/done.png
--rw-rw-rw-   0        0        0    22632 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/done.svg
--rw-rw-rw-   0        0        0     1092 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/edit.png
--rw-rw-rw-   0        0        0     7718 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/expert.png
--rw-rw-rw-   0        0        0     1264 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/eye.png
--rw-rw-rw-   0        0        0     8059 2019-01-15 04:29:26.000000 xllabelme-5.1.3/xllabelme/icons/feBlend-icon.png
--rw-rw-rw-   0        0        0      765 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/file.png
--rw-rw-rw-   0        0        0     1365 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/fit-width.png
--rw-rw-rw-   0        0        0     1102 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/fit-window.png
--rw-rw-rw-   0        0        0     2262 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/fit.png
--rw-rw-rw-   0        0        0     1587 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/help.png
--rw-rw-rw-   0        0        0   183198 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/icon.ico
--rw-rw-rw-   0        0        0    44771 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/icon.png
--rw-rw-rw-   0        0        0    38362 2023-04-04 10:35:02.000000 xllabelme-5.1.3/xllabelme/icons/icon2.ico
--rw-rw-rw-   0        0        0    34213 2023-04-04 10:24:55.000000 xllabelme-5.1.3/xllabelme/icons/icon2.png
--rw-rw-rw-   0        0        0     2381 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/labels.png
--rw-rw-rw-   0        0        0    37512 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/labels.svg
--rw-rw-rw-   0        0        0      977 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/new.png
--rw-rw-rw-   0        0        0    30288 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/next.png
--rw-rw-rw-   0        0        0     1103 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/objects.png
--rw-rw-rw-   0        0        0     2073 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/open.png
--rw-rw-rw-   0        0        0    18773 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/open.svg
--rw-rw-rw-   0        0        0    30665 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/prev.png
--rw-rw-rw-   0        0        0     1915 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/quit.png
--rw-rw-rw-   0        0        0     2811 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/save-as.png
--rw-rw-rw-   0        0        0    65363 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/save-as.svg
--rw-rw-rw-   0        0        0     1187 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/save.png
--rw-rw-rw-   0        0        0    31292 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/save.svg
--rw-rw-rw-   0        0        0     2004 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/undo-cross.png
--rw-rw-rw-   0        0        0     2018 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/undo.png
--rw-rw-rw-   0        0        0     1099 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/zoom-in.png
--rw-rw-rw-   0        0        0     1074 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/zoom-out.png
--rw-rw-rw-   0        0        0     1139 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/icons/zoom.png
--rw-rw-rw-   0        0        0     6926 2023-03-31 08:55:46.000000 xllabelme-5.1.3/xllabelme/label_file.py
--rw-rw-rw-   0        0        0     1907 2023-03-31 08:56:10.000000 xllabelme-5.1.3/xllabelme/logger.py
--rw-rw-rw-   0        0        0     9649 2022-04-26 01:24:19.000000 xllabelme-5.1.3/xllabelme/shape.py
--rw-rw-rw-   0        0        0      886 2021-06-08 03:21:06.000000 xllabelme-5.1.3/xllabelme/testing.py
--rw-rw-rw-   0        0        0    44799 2023-04-04 12:30:43.000000 xllabelme-5.1.3/xllabelme/ts.py
-drwxrwxrwx   0        0        0        0 2023-04-04 13:48:11.154808 xllabelme-5.1.3/xllabelme/utils/
--rw-rw-rw-   0        0        0      749 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/utils/__init__.py
--rw-rw-rw-   0        0        0      698 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/utils/_io.py
--rw-rw-rw-   0        0        0     2468 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/utils/image.py
--rw-rw-rw-   0        0        0     6290 2023-04-04 09:31:32.000000 xllabelme-5.1.3/xllabelme/utils/qt.py
--rw-rw-rw-   0        0        0     3764 2021-06-08 03:21:06.000000 xllabelme-5.1.3/xllabelme/utils/shape.py
-drwxrwxrwx   0        0        0        0 2023-04-04 13:48:11.162786 xllabelme-5.1.3/xllabelme/widgets/
--rw-rw-rw-   0        0        0      554 2022-04-20 05:44:54.000000 xllabelme-5.1.3/xllabelme/widgets/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-03-31 14:44:05.000000 xllabelme-5.1.3/xllabelme/widgets/brightness_contrast_dialog.py
--rw-rw-rw-   0        0        0    35438 2023-03-31 14:49:37.000000 xllabelme-5.1.3/xllabelme/widgets/canvas.py
--rw-rw-rw-   0        0        0     1231 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/widgets/color_dialog.py
--rw-rw-rw-   0        0        0      290 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/widgets/escapable_qlist_widget.py
--rw-rw-rw-   0        0        0     2451 2023-03-24 09:08:22.000000 xllabelme-5.1.3/xllabelme/widgets/file_dialog_preview.py
--rw-rw-rw-   0        0        0    19741 2022-10-24 08:25:25.000000 xllabelme-5.1.3/xllabelme/widgets/label_dialog.py
--rw-rw-rw-   0        0        0     6194 2023-03-31 08:45:59.000000 xllabelme-5.1.3/xllabelme/widgets/label_list_widget.py
--rw-rw-rw-   0        0        0      998 2020-08-05 08:41:43.000000 xllabelme-5.1.3/xllabelme/widgets/tool_bar.py
--rw-rw-rw-   0        0        0     1666 2023-03-31 08:47:05.000000 xllabelme-5.1.3/xllabelme/widgets/unique_label_qlist_widget.py
--rw-rw-rw-   0        0        0      735 2023-04-04 11:11:05.000000 xllabelme-5.1.3/xllabelme/widgets/zoom_widget.py
--rw-rw-rw-   0        0        0    11835 2023-04-04 11:39:23.000000 xllabelme-5.1.3/xllabelme/xlapp.py
-drwxrwxrwx   0        0        0        0 2023-04-04 13:48:11.122740 xllabelme-5.1.3/xllabelme.egg-info/
--rw-rw-rw-   0        0        0    11738 2023-04-04 13:48:11.000000 xllabelme-5.1.3/xllabelme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2243 2023-04-04 13:48:11.000000 xllabelme-5.1.3/xllabelme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 13:48:11.000000 xllabelme-5.1.3/xllabelme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      281 2023-04-04 13:48:11.000000 xllabelme-5.1.3/xllabelme.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      116 2023-04-04 13:48:11.000000 xllabelme-5.1.3/xllabelme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-04 13:48:11.000000 xllabelme-5.1.3/xllabelme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.746422 xllabelme-5.1.4/
+-rw-rw-rw-   0        0        0      707 2020-11-09 02:22:17.000000 xllabelme-5.1.4/LICENSE
+-rw-rw-rw-   0        0        0       19 2020-08-05 08:41:43.000000 xllabelme-5.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    11738 2023-04-14 09:39:52.745425 xllabelme-5.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9202 2022-04-20 05:38:39.000000 xllabelme-5.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.659174 xllabelme-5.1.4/docs/
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.665365 xllabelme-5.1.4/docs/man/
+-rw-rw-rw-   0        0        0     2148 2020-08-05 08:41:43.000000 xllabelme-5.1.4/docs/man/labelme.1
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:39:52.746422 xllabelme-5.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     5290 2023-04-04 11:32:18.000000 xllabelme-5.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.674341 xllabelme-5.1.4/xllabelme/
+-rw-rw-rw-   0        0        0     1072 2023-04-14 09:39:50.000000 xllabelme-5.1.4/xllabelme/__init__.py
+-rw-rw-rw-   0        0        0     7419 2023-04-13 14:13:41.000000 xllabelme-5.1.4/xllabelme/__main__.py
+-rw-rw-rw-   0        0        0    78177 2023-04-14 09:19:03.000000 xllabelme-5.1.4/xllabelme/app.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.683909 xllabelme-5.1.4/xllabelme/cli/
+-rw-rw-rw-   0        0        0      129 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/cli/__init__.py
+-rw-rw-rw-   0        0        0     1404 2022-04-20 05:42:00.000000 xllabelme-5.1.4/xllabelme/cli/draw_json.py
+-rw-rw-rw-   0        0        0      667 2021-06-08 03:21:06.000000 xllabelme-5.1.4/xllabelme/cli/draw_label_png.py
+-rw-rw-rw-   0        0        0     2473 2022-04-20 05:42:14.000000 xllabelme-5.1.4/xllabelme/cli/json_to_dataset.py
+-rw-rw-rw-   0        0        0     2851 2022-04-20 05:42:22.000000 xllabelme-5.1.4/xllabelme/cli/on_docker.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.686904 xllabelme-5.1.4/xllabelme/config/
+-rw-rw-rw-   0        0        0     2784 2021-06-08 03:21:07.000000 xllabelme-5.1.4/xllabelme/config/__init__.py
+-rw-rw-rw-   0        0        0     2320 2023-04-04 02:59:12.000000 xllabelme-5.1.4/xllabelme/config/default_config.yaml
+-rw-rw-rw-   0        0        0    48869 2023-04-14 09:20:52.000000 xllabelme-5.1.4/xllabelme/config/xllabellib.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.725477 xllabelme-5.1.4/xllabelme/icons/
+-rw-rw-rw-   0        0        0     2136 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/cancel.png
+-rw-rw-rw-   0        0        0     3111 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/close.png
+-rw-rw-rw-   0        0        0     2368 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/color-line.png
+-rw-rw-rw-   0        0        0     1461 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/color.png
+-rw-rw-rw-   0        0        0      646 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/copy.png
+-rw-rw-rw-   0        0        0     1486 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/delete.png
+-rw-rw-rw-   0        0        0     2198 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/done.png
+-rw-rw-rw-   0        0        0    22632 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/done.svg
+-rw-rw-rw-   0        0        0     1092 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/edit.png
+-rw-rw-rw-   0        0        0     7718 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/expert.png
+-rw-rw-rw-   0        0        0     1264 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/eye.png
+-rw-rw-rw-   0        0        0     8059 2019-01-15 04:29:26.000000 xllabelme-5.1.4/xllabelme/icons/feBlend-icon.png
+-rw-rw-rw-   0        0        0      765 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/file.png
+-rw-rw-rw-   0        0        0     1365 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/fit-width.png
+-rw-rw-rw-   0        0        0     1102 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/fit-window.png
+-rw-rw-rw-   0        0        0     2262 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/fit.png
+-rw-rw-rw-   0        0        0     1587 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/help.png
+-rw-rw-rw-   0        0        0   183198 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/icon.ico
+-rw-rw-rw-   0        0        0    44771 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/icon.png
+-rw-rw-rw-   0        0        0    38362 2023-04-04 10:35:02.000000 xllabelme-5.1.4/xllabelme/icons/icon2.ico
+-rw-rw-rw-   0        0        0    34213 2023-04-04 10:24:55.000000 xllabelme-5.1.4/xllabelme/icons/icon2.png
+-rw-rw-rw-   0        0        0     2381 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/labels.png
+-rw-rw-rw-   0        0        0    37512 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/labels.svg
+-rw-rw-rw-   0        0        0      977 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/new.png
+-rw-rw-rw-   0        0        0    30288 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/next.png
+-rw-rw-rw-   0        0        0     1103 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/objects.png
+-rw-rw-rw-   0        0        0     2073 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/open.png
+-rw-rw-rw-   0        0        0    18773 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/open.svg
+-rw-rw-rw-   0        0        0    30665 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/prev.png
+-rw-rw-rw-   0        0        0     1915 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/quit.png
+-rw-rw-rw-   0        0        0     2811 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/save-as.png
+-rw-rw-rw-   0        0        0    65363 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/save-as.svg
+-rw-rw-rw-   0        0        0     1187 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/save.png
+-rw-rw-rw-   0        0        0    31292 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/save.svg
+-rw-rw-rw-   0        0        0     2004 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/undo-cross.png
+-rw-rw-rw-   0        0        0     2018 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/undo.png
+-rw-rw-rw-   0        0        0     1099 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/zoom-in.png
+-rw-rw-rw-   0        0        0     1074 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/zoom-out.png
+-rw-rw-rw-   0        0        0     1139 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/icons/zoom.png
+-rw-rw-rw-   0        0        0     7004 2023-04-13 14:18:20.000000 xllabelme-5.1.4/xllabelme/label_file.py
+-rw-rw-rw-   0        0        0     1907 2023-03-31 08:56:10.000000 xllabelme-5.1.4/xllabelme/logger.py
+-rw-rw-rw-   0        0        0     9649 2022-04-26 01:24:19.000000 xllabelme-5.1.4/xllabelme/shape.py
+-rw-rw-rw-   0        0        0      886 2021-06-08 03:21:06.000000 xllabelme-5.1.4/xllabelme/testing.py
+-rw-rw-rw-   0        0        0    44799 2023-04-04 12:30:43.000000 xllabelme-5.1.4/xllabelme/ts.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.730464 xllabelme-5.1.4/xllabelme/utils/
+-rw-rw-rw-   0        0        0      749 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/utils/__init__.py
+-rw-rw-rw-   0        0        0      698 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/utils/_io.py
+-rw-rw-rw-   0        0        0     2468 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/utils/image.py
+-rw-rw-rw-   0        0        0     6290 2023-04-04 09:31:32.000000 xllabelme-5.1.4/xllabelme/utils/qt.py
+-rw-rw-rw-   0        0        0     3764 2021-06-08 03:21:06.000000 xllabelme-5.1.4/xllabelme/utils/shape.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.744428 xllabelme-5.1.4/xllabelme/widgets/
+-rw-rw-rw-   0        0        0      554 2022-04-20 05:44:54.000000 xllabelme-5.1.4/xllabelme/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-03-31 14:44:05.000000 xllabelme-5.1.4/xllabelme/widgets/brightness_contrast_dialog.py
+-rw-rw-rw-   0        0        0    35438 2023-03-31 14:49:37.000000 xllabelme-5.1.4/xllabelme/widgets/canvas.py
+-rw-rw-rw-   0        0        0     1231 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/widgets/color_dialog.py
+-rw-rw-rw-   0        0        0      290 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/widgets/escapable_qlist_widget.py
+-rw-rw-rw-   0        0        0     2451 2023-03-24 09:08:22.000000 xllabelme-5.1.4/xllabelme/widgets/file_dialog_preview.py
+-rw-rw-rw-   0        0        0    19741 2022-10-24 08:25:25.000000 xllabelme-5.1.4/xllabelme/widgets/label_dialog.py
+-rw-rw-rw-   0        0        0     6194 2023-03-31 08:45:59.000000 xllabelme-5.1.4/xllabelme/widgets/label_list_widget.py
+-rw-rw-rw-   0        0        0      998 2020-08-05 08:41:43.000000 xllabelme-5.1.4/xllabelme/widgets/tool_bar.py
+-rw-rw-rw-   0        0        0     1666 2023-03-31 08:47:05.000000 xllabelme-5.1.4/xllabelme/widgets/unique_label_qlist_widget.py
+-rw-rw-rw-   0        0        0      735 2023-04-04 11:11:05.000000 xllabelme-5.1.4/xllabelme/widgets/zoom_widget.py
+-rw-rw-rw-   0        0        0    11756 2023-04-14 09:15:35.000000 xllabelme-5.1.4/xllabelme/xlapp.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:52.679327 xllabelme-5.1.4/xllabelme.egg-info/
+-rw-rw-rw-   0        0        0    11738 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2243 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      281 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      116 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 09:39:52.000000 xllabelme-5.1.4/xllabelme.egg-info/top_level.txt
```

### Comparing `xllabelme-5.1.3/LICENSE` & `xllabelme-5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/PKG-INFO` & `xllabelme-5.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xllabelme
-Version: 5.1.3
+Version: 5.1.4
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada
 Author-email: 877362867@qq.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xllabelme Version: 5.1.3 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: xllabelme Version: 5.1.4 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada Author-email: 877362867@qq.com License: GPLv3
 Keywords: Image Annotation,Machine Learning Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `xllabelme-5.1.3/README.md` & `xllabelme-5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/docs/man/labelme.1` & `xllabelme-5.1.4/docs/man/labelme.1`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/setup.py` & `xllabelme-5.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/__init__.py` & `xllabelme-5.1.4/xllabelme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Semantic Versioning 2.0.0: https://semver.org/
 # 1. MAJOR version when you make incompatible API changes;
 # 2. MINOR version when you add functionality in a backwards-compatible manner;
 # 3. PATCH version when you make backwards-compatible bug fixes.
 
 # 每当官方有第2位版本号更新，比如5.2、5.3时，我会尽力做个源码的同步
 # 然后我个人功能，会在第3位上自增，比如5.1.2、5.1.3
-__version__ = "5.1.3"
+__version__ = "5.1.4"
 
 # 2 扩展的更灵活的labelme，兼容官方的功能，但有更强的可视化效果，能查看shape的多个属性值
 __appname__ = f"xllabelme v{__version__}"
 
 QT4 = QT_VERSION[0] == "4"
 QT5 = QT_VERSION[0] == "5"
 del QT_VERSION
```

### Comparing `xllabelme-5.1.3/xllabelme/__main__.py` & `xllabelme-5.1.4/xllabelme/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from xllabelme.xlapp import XlMainWindow
 from xllabelme.config import get_config
 from xllabelme.logger import logger
 from xllabelme.utils import newIcon
 import xllabelme.ts
 
 from pyxllib.prog.pupil import dprint  # 在任意地方均可以使用dprint调试
+from pyxllib.prog.pupil import format_exception
+from pyxllib.ext.qt import show_message_box
 
 
 def default_argument_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--version", "-V", action="store_true", help="show version"
     )
@@ -204,8 +206,11 @@
     win.show()
     win.raise_()
     sys.exit(app.exec_())
 
 
 # this main block is required to generate executable by pyinstaller
 if __name__ == "__main__":
-    main(XlMainWindow)
+    try:
+        main(XlMainWindow)
+    except Exception as e:
+        show_message_box(format_exception(e), '程序跑路了，给管理员发这个截图让他来破案吧！')
```

### Comparing `xllabelme-5.1.3/xllabelme/app.py` & `xllabelme-5.1.4/xllabelme/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     FIT_WINDOW, FIT_WIDTH, MANUAL_ZOOM = 0, 1, 2
 
     def __init__(
             self,
             config=None,
             filename=None,
             output=None,
-            output_file=None,
-            output_dir=None,
+            output_file=None,  # 导出json标注的一个示例文件
+            output_dir=None,  # 导出json标注的目录
     ):
         if output is not None:
             logger.warning(
                 "argument output is deprecated, use output_file instead"
             )
             if output_file is None:
                 output_file = output
@@ -109,15 +109,15 @@
             completion=self._config["label_completion"],
             fit_to_content=self._config["fit_to_content"],
             flags=self._config["label_flags"],
         )
 
         # Polygon Labels 控件
         self.labelList = LabelListWidget()
-        self.lastOpenDir = None
+        self.lastOpenDir = None  # 最近打开的图片目录
 
         self.flag_dock = self.flag_widget = None
         self.flag_dock = QtWidgets.QDockWidget(self.tr("Flags"), self)
         self.flag_dock.setObjectName("Flags")
         self.flag_widget = QtWidgets.QListWidget()
         if config["flags"]:
             self.loadFlags({k: False for k in config["flags"]})
@@ -125,15 +125,15 @@
         self.flag_widget.itemChanged.connect(self.setDirty)
 
         self.labelList.itemSelectionChanged.connect(self.labelSelectionChanged)
         self.labelList.itemDoubleClicked.connect(self.editLabel)
         self.labelList.itemChanged.connect(self.labelItemChanged)
         self.labelList.itemDropped.connect(self.labelOrderChanged)
         self.shape_dock = QtWidgets.QDockWidget(
-            self.tr("Polygon Labels"), self
+            self.tr("Polygon Labels"), self  # 多边形标签
         )
         self.shape_dock.setObjectName("Labels")
         self.shape_dock.setWidget(self.labelList)
 
         self.uniqLabelList = UniqueLabelQListWidget()
         self.uniqLabelList.setToolTip(
             self.tr(
@@ -143,15 +143,15 @@
         )
         if self._config["labels"]:
             for label in self._config["labels"]:
                 item = self.uniqLabelList.createItemFromLabel(label)
                 self.uniqLabelList.addItem(item)
                 rgb = self._get_rgb_by_label(label)
                 self.uniqLabelList.setItemLabel(item, label, rgb)
-        self.label_dock = QtWidgets.QDockWidget(self.tr("Label List"), self)
+        self.label_dock = QtWidgets.QDockWidget(self.tr("Label List"), self)  # 文件列表
         self.label_dock.setObjectName("Label List")
         self.label_dock.setWidget(self.uniqLabelList)
 
         self.fileSearch = QtWidgets.QLineEdit()
         self.fileSearch.setPlaceholderText(self.tr("Search Filename"))
         self.fileSearch.textChanged.connect(self.fileSearchChanged)
         self.fileListWidget = QtWidgets.QListWidget()
@@ -562,28 +562,37 @@
             self.editLabel,
             shortcuts["edit_label"],
             "edit",
             self.tr("Modify the label of the selected polygon"),
             enabled=False,
         )
 
+        clear_label = action(
+            self.tr("清空所有标注"),
+            self.clearLabel,
+            None,
+            "delete",
+            self.tr("Modify the label of the selected polygon"),
+            enabled=True,
+        )
+
         fill_drawing = action(
             self.tr("Fill Drawing Polygon"),
             self.canvas.setFillDrawing,
             None,
             "color",
             self.tr("Fill polygon while drawing"),
             checkable=True,
             enabled=True,
         )
         fill_drawing.trigger()
 
         # Lavel list context menu.
         labelMenu = QtWidgets.QMenu()
-        utils.addActions(labelMenu, (edit, delete))
+        utils.addActions(labelMenu, (edit, delete, clear_label))
         self.labelList.setContextMenuPolicy(Qt.CustomContextMenu)
         self.labelList.customContextMenuRequested.connect(
             self.popLabelListMenu
         )
 
         # Store actions for further handling.
         self.actions = utils.struct(
@@ -862,26 +871,32 @@
             self.actions.createLineMode,
             self.actions.createPointMode,
             self.actions.createLineStripMode,
             self.actions.editMode,
         )
         utils.addActions(self.menus.edit, list(actions) + list(self.actions.editMenu))
 
-    def setDirty(self):
+    def setDirty(self, dirty=True):
+        """
+        :param dirty: 需要设置不同级别，默认True处理。这里建议使用位运算区别不同内容的备份。
+            1、True，labelme默认处理
+            2，需要保存图片数据
+        :return:
+        """
         # Even if we autosave the file, we keep the ability to undo
         self.actions.undo.setEnabled(self.canvas.isShapeRestorable)
 
         if self._config["auto_save"] or self.actions.saveAuto.isChecked():
             label_file = osp.splitext(self.imagePath)[0] + ".json"
             if self.output_dir:
                 label_file_without_path = osp.basename(label_file)
                 label_file = osp.join(self.output_dir, label_file_without_path)
             self.saveLabels(label_file)
             return
-        self.dirty = True
+        self.dirty = self.dirty | dirty
         self.actions.save.setEnabled(True)
         title = f'{__appname__}'
         if self.filename is not None:
             title = "{} - {}*".format(title, self.filename)
         self.setWindowTitle(title)
 
     def setClean(self):
@@ -1097,26 +1112,32 @@
         self.setDirty()
         if self.uniqLabelList.findItemByLabel(shape.label) is None:
             item = self.uniqLabelList.createItemFromLabel(shape.label)
             self.uniqLabelList.addItem(item)
             rgb = self._get_rgb_by_label(shape.label)
             self.uniqLabelList.setItemLabel(item, shape.label, rgb)
 
+    def clearLabel(self):
+        self.labelList.clear()
+        self.canvas.shapes.clear()
+        self.canvas.repaint()
+        self.setDirty()
+
     def fileSearchChanged(self):
         self.importDirImages(
             self.lastOpenDir,
             pattern=self.fileSearch.text(),
             load=False,
         )
 
     def fileSelectionChanged(self):
-        items = self.fileListWidget.selectedItems()
+        items = self.fileListWidget.selectedItems()  # 选中的文件
         if not items:
             return
-        item = items[0]
+        item = items[0]  # 默认只能选中一个文件的
 
         if not self.mayContinue():
             return
 
         currIndex = self.imageList.index(str(item.text()))
         if currIndex < len(self.imageList):
             filename = self.imageList[currIndex]
@@ -1453,18 +1474,19 @@
             self.fileListWidget.repaint()
             return
 
         self.resetState()
         self.canvas.setEnabled(False)
         if filename is None:
             filename = self.settings.value("filename", "")
-        filename = str(filename)
+        # filename = str(filename)
+        filename = osp.join(self.lastOpenDir, str(filename))
         if not QtCore.QFile.exists(filename):
             self.errorMessage(
-                self.tr("Error opening file"),
+                self.tr("Error opening file"),  # 打开文件发生错误
                 self.tr("No such file: <b>%s</b>") % filename,
             )
             return False
         # assumes same name, but json extension
         self.status(
             str(self.tr("Loading %s...")) % osp.basename(str(filename))
         )
@@ -1472,15 +1494,15 @@
         if self.output_dir:
             label_file_without_path = osp.basename(label_file)
             label_file = osp.join(self.output_dir, label_file_without_path)
         if QtCore.QFile.exists(label_file) and LabelFile.is_label_file(
                 label_file
         ):
             try:
-                self.labelFile = LabelFile(label_file)
+                self.labelFile = LabelFile(label_file, filename)
             except LabelFileError as e:
                 self.errorMessage(
                     self.tr("Error opening file"),
                     self.tr(
                         "<p><b>%s</b></p>"
                         "<p>Make sure <i>%s</i> is a valid label file."
                     )
@@ -1688,30 +1710,31 @@
                 Qt.ControlModifier | Qt.ShiftModifier
         ):
             self._config["keep_prev"] = True
 
         if not self.mayContinue():
             return
 
-        if len(self.imageList) <= 0:
+        imageList = self.imageList
+        if len(imageList) <= 0:
             return
 
-        filename = None
         if self.filename is None:
-            filename = self.imageList[0]
+            filename = imageList[0]
         else:
             try:
-                currIndex = self.imageList.index(self.filename)
-                if currIndex + offset < len(self.imageList):
-                    filename = self.imageList[currIndex + offset]
+                fn = XlPath(self.filename).relpath(self.lastOpenDir).as_posix()
+                currIndex = imageList.index(fn)
+                if currIndex + offset < len(imageList):
+                    filename = imageList[currIndex + offset]
                 else:
-                    filename = self.imageList[-1]
+                    filename = imageList[-1]
             except ValueError:  # 找不到则默认用第1个
-                filename = self.imageList[0]
-        self.filename = filename
+                filename = imageList[0]
+        self.filename = XlPath(self.lastOpenDir, filename)
 
         if self.filename and load:
             self.loadFile(self.filename)
 
         self._config["keep_prev"] = keep_prev
 
     def openFile(self, _value=False):
@@ -1773,14 +1796,18 @@
             self.fileListWidget.setCurrentRow(
                 self.imageList.index(current_filename)
             )
             self.fileListWidget.repaint()
 
     def saveFile(self, _value=False):
         assert not self.image.isNull(), "cannot save empty image"
+
+        if self.dirty & 2:  # 需要保存图片
+            self.canvas.pixmap.save(self.imagePath, osp.splitext(self.imagePath)[1][1:])
+
         if self.labelFile:
             # DL20180323 - overwrite when in directory
             self._saveFile(self.labelFile.filename)
         elif self.output_file:
             self._saveFile(self.output_file)
             self.close()
         else:
@@ -1860,15 +1887,19 @@
         if osp.exists(label_file):
             os.remove(label_file)
             logger.info("Label file is removed: {}".format(label_file))
 
             item = self.fileListWidget.currentItem()
             item.setCheckState(Qt.Unchecked)
 
+            filename = self.filename  # 这个参数不能清
             self.resetState()
+            self.filename = filename
+
+            self.openNextImg(offset=0)
 
     # Message Dialogs. #
     def hasLabels(self):
         if self.noShapes():
             self.errorMessage(
                 "No objects labeled",
                 "You must label at least one object to save the file.",
@@ -1880,14 +1911,15 @@
         if self.filename is None:
             return False
 
         label_file = self.getLabelFile()
         return osp.exists(label_file)
 
     def mayContinue(self):
+        """ 切换窗口或数据的时候，判断上一份数据是否要保存 """
         if not self.dirty:
             return True
 
         mb = QtWidgets.QMessageBox
         msg = self.tr('Save annotations to "{}" before closing?').format(
             self.filename
         )
@@ -1993,18 +2025,20 @@
 
         self.filename = None
         for file in imageFiles:
             if file in self.imageList or not file.lower().endswith(
                     tuple(extensions)
             ):
                 continue
-            label_file = osp.splitext(file)[0] + ".json"
+            # label_file = osp.splitext(file)[0] + ".json"
             if self.output_dir:
                 label_file_without_path = osp.basename(label_file)
                 label_file = osp.join(self.output_dir, label_file_without_path)
+            else:
+                label_file = osp.join(self.lastOpenDir, label_file)
             item = QtWidgets.QListWidgetItem(file)
             item.setFlags(Qt.ItemIsEnabled | Qt.ItemIsSelectable)
             if QtCore.QFile.exists(label_file) and LabelFile.is_label_file(
                     label_file
             ):
                 item.setCheckState(Qt.Checked)
             else:
@@ -2024,53 +2058,58 @@
         if not self.mayContinue() or not dirpath:
             return
 
         self.lastOpenDir = dirpath
         self.filename = filename
         self.fileListWidget.clear()
 
-        if self.xllabel.image_root is None:
-            for filename in self.scanAllImages(dirpath):
-                if pattern and pattern not in filename:
-                    continue
-                label_file = osp.splitext(filename)[0] + ".json"
-                if self.output_dir:
-                    label_file_without_path = osp.basename(label_file)
-                    label_file = osp.join(self.output_dir, label_file_without_path)
-                item = QtWidgets.QListWidgetItem(filename)
-                item.setFlags(Qt.ItemIsEnabled | Qt.ItemIsSelectable)
-                if QtCore.QFile.exists(label_file) and LabelFile.is_label_file(
-                        label_file
-                ):
-                    item.setCheckState(Qt.Checked)
-                else:
-                    item.setCheckState(Qt.Unchecked)
-                self.fileListWidget.addItem(item)
-        else:  # ckz，我要扩展一个读取json来展示图片的功能
-            root = self.xllabel.image_root
-            for label_file in XlPath(dirpath).rglob('*.json'):
-                data = label_file.read_json()
-                if 'imagePath' in data:
-                    filename = str(root / label_file.relpath(dirpath))
-                else:
-                    continue
-                item = QtWidgets.QListWidgetItem(filename)
-                item.setFlags(Qt.ItemIsEnabled | Qt.ItemIsSelectable)
+        image_root = self.xllabel.image_root or dirpath
+        for filename in self.scanAllImages(image_root):
+            if pattern and pattern not in filename:
+                continue
+            label_file = osp.splitext(filename)[0] + ".json"
+            # label_file = osp.join(self.lastOpenDir, osp.basename(filename) + ".json")
+            if self.output_dir:
+                label_file_without_path = osp.basename(label_file)
+                label_file = osp.join(self.output_dir, label_file_without_path)
+            else:
+                label_file = osp.join(self.lastOpenDir, label_file)
+            item = QtWidgets.QListWidgetItem(filename)
+            item.setFlags(Qt.ItemIsEnabled | Qt.ItemIsSelectable)
+            if QtCore.QFile.exists(label_file) and LabelFile.is_label_file(
+                    label_file
+            ):
                 item.setCheckState(Qt.Checked)
-                self.fileListWidget.addItem(item)
+            else:
+                item.setCheckState(Qt.Unchecked)
+            self.fileListWidget.addItem(item)
+
+        # else:  # ckz，我要扩展一个读取json来展示图片的功能
+        #     root = self.xllabel.image_root
+        #     for label_file in XlPath(dirpath).rglob('*.json'):
+        #         data = label_file.read_json()
+        #         if 'imagePath' in data:
+        #             filename = str(label_file.relpath(dirpath))
+        #         else:
+        #             continue
+        #         item = QtWidgets.QListWidgetItem(filename)
+        #         item.setFlags(Qt.ItemIsEnabled | Qt.ItemIsSelectable)
+        #         item.setCheckState(Qt.Checked)
+        #         self.fileListWidget.addItem(item)
 
         self.openNextImg(load=load, offset=offset)
 
     def scanAllImages(self, folderPath):
         extensions = [
             ".%s" % fmt.data().decode().lower()
             for fmt in QtGui.QImageReader.supportedImageFormats()
         ]
 
         images = []
         for root, dirs, files in os.walk(folderPath):
             for file in files:
                 if file.lower().endswith(tuple(extensions)):
-                    relativePath = osp.join(root, file)
-                    images.append(relativePath)
+                    # relativePath = osp.join(root, file)
+                    # images.append(relativePath)
+                    images.append((XlPath(root) / file).relpath(folderPath).as_posix())  # ckz: 只保存，显示相对路径
         images = natsort.os_sorted(images)
         return images
```

### Comparing `xllabelme-5.1.3/xllabelme/cli/draw_json.py` & `xllabelme-5.1.4/xllabelme/cli/draw_json.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/cli/draw_label_png.py` & `xllabelme-5.1.4/xllabelme/cli/draw_label_png.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/cli/json_to_dataset.py` & `xllabelme-5.1.4/xllabelme/cli/json_to_dataset.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/cli/on_docker.py` & `xllabelme-5.1.4/xllabelme/cli/on_docker.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/config/__init__.py` & `xllabelme-5.1.4/xllabelme/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/config/default_config.yaml` & `xllabelme-5.1.4/xllabelme/config/default_config.yaml`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/config/xllabellib.py` & `xllabelme-5.1.4/xllabelme/config/xllabellib.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,16 @@
             a.triggered.connect(func)
             return a
 
         settings_menu = self.mainwin.menus.settings
         settings_menu.addMenu(create_project_menu())
         settings_menu.addSeparator()
         settings_menu.addAction(create_auto_rec_text_action())
-        settings_menu.addAction(create_set_image_root_action())
+        # 关闭该功能，发现原本就有类似的功能，是我重复造轮子了
+        # settings_menu.addAction(create_set_image_root_action())
         settings_menu.addSeparator()
         settings_menu.addAction(create_reset_config_action())
 
     def convert_to_rectangle_action(self):
         """ 将shape形状改为四边形 """
 
         def func():
@@ -256,14 +257,74 @@
                             func,
                             None,  # 快捷键
                             None,  # 图标
                             mainwin.tr("将当前shape形状转为Rectangle矩形")  # 左下角的提示
                             )
         return a
 
+    def rotate_image_action(self):
+        """ 旋转图片 """
+
+        def flip_points(sp, h):
+            from pyxllib.algo.geo import resort_quad_points
+            pts = sp.points
+            if sp.shape_type == 'rectangle':
+                # 矩形要特殊处理，仍然确保第1个点在左上角
+                x1, y1 = pts[0].x(), pts[0].y()
+                x2, y2 = pts[1].x(), pts[1].y()
+
+                pts[0].setX(h - y2)
+                pts[0].setY(x1)
+                pts[1].setX(h - y1)
+                pts[1].setY(x2)
+            elif sp.shape_type == 'polygon' and len(pts) == 4:
+                pts = [[h - p.y(), p.x()] for p in pts]
+                pts = resort_quad_points(pts)
+                for p1, p2 in zip(sp.points, pts):
+                    p1.setX(p2[0])
+                    p1.setY(p2[1])
+            else:  # 其他形状暂不特殊处理
+                for point in sp.points:
+                    x = point.x()  # 要中转存储下，不然等下x会被新值覆盖
+                    point.setX(h - point.y())
+                    point.setY(x)
+
+        def func():
+            """ 每次执行顺时针旋转90度 """
+            from PyQt5.QtGui import QTransform
+
+            # 1 旋转shapes坐标
+            canvas = mainwin.canvas
+            h = canvas.pixmap.height()
+            shapes = canvas.shapes
+            for sp in shapes:
+                flip_points(sp, h)
+
+            # 2 旋转图片
+            mainwin.updateShapes(shapes)
+            transform = QTransform()
+            transform.rotate(90)
+            canvas.pixmap = canvas.pixmap.transformed(transform)
+
+            # 3 end
+            canvas.repaint()
+            mainwin.setDirty(3)
+
+        mainwin = self.mainwin
+        a = utils.newAction(mainwin,
+                            mainwin.tr("旋转图片"),
+                            func,
+                            None,  # 快捷键
+                            None,  # 图标
+                            mainwin.tr("将图片和当前标注的形状，顺时针旋转90度，可以多次操作调整到合适方向。"
+                                       "注意1：软件中操作并未改变原始图片，需要保存标注文件后，外部图片文件才会更新。"
+                                       "注意2：图片操作目前是撤销不了的，不过可以不保存再重新打开文件恢复初始状态。")  # 左下角的提示
+                            )
+        return a
+
     def create(self):
         mainwin = self.mainwin
 
         # 1 设置菜单
         self.config_settings_menu()
 
         # 2 帮助菜单
@@ -288,26 +349,26 @@
         ]
 
         # 4 右键菜单增加功能
         mainwin.actions.menu = list(mainwin.actions.menu) + [
             None,
             self.convert_to_rectangle_action(),
             self.xllabel.split_shape_action(),
+            None,
+            self.rotate_image_action(),
         ]
 
         # 5 一些操作习惯
-
-
         mainwin.populateModeActions()
 
     def destroy(self):
         """ 销毁项目相关配置 """
         self.mainwin.menus.settings.clear()
         self.mainwin.actions.editMenu = self.mainwin.actions.editMenu[:-3]
-        self.mainwin.actions.menu = self.mainwin.actions.menu[:-3]
+        self.mainwin.actions.menu = self.mainwin.actions.menu[:-5]
 
     def update_shape(self, shape, label_list_item=None):
         """
         :param shape:
         :param label_list_item: item是shape的父级，挂在labelList下的项目
         """
         mainwin = self.mainwin
```

### Comparing `xllabelme-5.1.3/xllabelme/icons/cancel.png` & `xllabelme-5.1.4/xllabelme/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/close.png` & `xllabelme-5.1.4/xllabelme/icons/close.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/color-line.png` & `xllabelme-5.1.4/xllabelme/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/color.png` & `xllabelme-5.1.4/xllabelme/icons/color.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/copy.png` & `xllabelme-5.1.4/xllabelme/icons/copy.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/delete.png` & `xllabelme-5.1.4/xllabelme/icons/delete.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/done.png` & `xllabelme-5.1.4/xllabelme/icons/done.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/done.svg` & `xllabelme-5.1.4/xllabelme/icons/done.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/edit.png` & `xllabelme-5.1.4/xllabelme/icons/edit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/expert.png` & `xllabelme-5.1.4/xllabelme/icons/expert.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/eye.png` & `xllabelme-5.1.4/xllabelme/icons/eye.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/feBlend-icon.png` & `xllabelme-5.1.4/xllabelme/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/file.png` & `xllabelme-5.1.4/xllabelme/icons/file.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/fit-width.png` & `xllabelme-5.1.4/xllabelme/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/fit-window.png` & `xllabelme-5.1.4/xllabelme/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/fit.png` & `xllabelme-5.1.4/xllabelme/icons/fit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/help.png` & `xllabelme-5.1.4/xllabelme/icons/help.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/icon.ico` & `xllabelme-5.1.4/xllabelme/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/icon.png` & `xllabelme-5.1.4/xllabelme/icons/icon.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/icon2.ico` & `xllabelme-5.1.4/xllabelme/icons/icon2.ico`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/icon2.png` & `xllabelme-5.1.4/xllabelme/icons/icon2.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/labels.png` & `xllabelme-5.1.4/xllabelme/icons/labels.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/labels.svg` & `xllabelme-5.1.4/xllabelme/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/new.png` & `xllabelme-5.1.4/xllabelme/icons/new.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/next.png` & `xllabelme-5.1.4/xllabelme/icons/next.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/objects.png` & `xllabelme-5.1.4/xllabelme/icons/objects.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/open.png` & `xllabelme-5.1.4/xllabelme/icons/open.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/open.svg` & `xllabelme-5.1.4/xllabelme/icons/open.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/prev.png` & `xllabelme-5.1.4/xllabelme/icons/prev.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/quit.png` & `xllabelme-5.1.4/xllabelme/icons/quit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/save-as.png` & `xllabelme-5.1.4/xllabelme/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/save-as.svg` & `xllabelme-5.1.4/xllabelme/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/save.png` & `xllabelme-5.1.4/xllabelme/icons/save.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/save.svg` & `xllabelme-5.1.4/xllabelme/icons/save.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/undo-cross.png` & `xllabelme-5.1.4/xllabelme/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/undo.png` & `xllabelme-5.1.4/xllabelme/icons/undo.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/zoom-in.png` & `xllabelme-5.1.4/xllabelme/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/zoom-out.png` & `xllabelme-5.1.4/xllabelme/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/icons/zoom.png` & `xllabelme-5.1.4/xllabelme/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/label_file.py` & `xllabelme-5.1.4/xllabelme/label_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,21 @@
 class LabelFileError(Exception):
     pass
 
 
 class LabelFile(object):
     suffix = ".json"
 
-    def __init__(self, filename=None):
+    def __init__(self, filename=None, image_file=None):
         self.shapes = []
         self.imagePath = None
         self.imageData = None
+
+        self.image_file = image_file
+
         if filename is not None:
             self.load(filename)
         self.filename = filename
 
     @staticmethod
     def load_image_file(filename):
         try:
@@ -106,15 +109,15 @@
 
             if data["imageData"] is not None:
                 imageData = base64.b64decode(data["imageData"])
                 if PY2 and QT4:
                     imageData = utils.img_data_to_png_data(imageData)
             else:
                 # relative path from label file to relative path from cwd
-                imagePath = osp.join(osp.dirname(filename), data["imagePath"])
+                imagePath = self.image_file or osp.join(osp.dirname(filename), data["imagePath"])
                 imageData = self.load_image_file(imagePath)
             flags = data.get("flags") or {}
             imagePath = data["imagePath"]
             self._check_image_height_and_width(
                 base64.b64encode(imageData).decode("utf-8"),
                 data.get("imageHeight"),
                 data.get("imageWidth"),
```

### Comparing `xllabelme-5.1.3/xllabelme/logger.py` & `xllabelme-5.1.4/xllabelme/logger.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/shape.py` & `xllabelme-5.1.4/xllabelme/shape.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/testing.py` & `xllabelme-5.1.4/xllabelme/testing.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/ts.py` & `xllabelme-5.1.4/xllabelme/ts.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/utils/__init__.py` & `xllabelme-5.1.4/xllabelme/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/utils/_io.py` & `xllabelme-5.1.4/xllabelme/utils/_io.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/utils/image.py` & `xllabelme-5.1.4/xllabelme/utils/image.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/utils/qt.py` & `xllabelme-5.1.4/xllabelme/utils/qt.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/utils/shape.py` & `xllabelme-5.1.4/xllabelme/utils/shape.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/widgets/__init__.py` & `xllabelme-5.1.4/xllabelme/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/widgets/brightness_contrast_dialog.py` & `xllabelme-5.1.4/xllabelme/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/widgets/canvas.py` & `xllabelme-5.1.4/xllabelme/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/widgets/color_dialog.py` & `xllabelme-5.1.4/xllabelme/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/widgets/file_dialog_preview.py` & `xllabelme-5.1.4/xllabelme/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/widgets/label_dialog.py` & `xllabelme-5.1.4/xllabelme/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/widgets/label_list_widget.py` & `xllabelme-5.1.4/xllabelme/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/widgets/tool_bar.py` & `xllabelme-5.1.4/xllabelme/widgets/tool_bar.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/widgets/unique_label_qlist_widget.py` & `xllabelme-5.1.4/xllabelme/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/widgets/zoom_widget.py` & `xllabelme-5.1.4/xllabelme/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.3/xllabelme/xlapp.py` & `xllabelme-5.1.4/xllabelme/xlapp.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,15 +192,14 @@
             item = self.flag_widget.item(i)
             key = item.text()
             flag = item.checkState() == Qt.Checked
             flags[key] = flag
         try:
             imagePath = osp.relpath(self.imagePath, osp.dirname(filename))
             # 强制不保存 imageData
-            dprint(self._config["store_data"])
             imageData = self.imageData if self._config["store_data"] else None
             if osp.dirname(filename) and not osp.exists(osp.dirname(filename)):
                 os.makedirs(osp.dirname(filename))
             lf.save(
                 filename=filename,
                 shapes=shapes,
                 imagePath=imagePath,
@@ -271,16 +270,16 @@
         if not self.imagePath:
             return ''
         canvas = self.canvas
         pixmap = canvas.pixmap
         # files_num = len(self.fileListWidget)
         filesize = XlPath(self.imagePath).size(human_readable=True)
         shapes_num = len(self.canvas.shapes)
-        tip = f'本图信息：图片文件大小={filesize}, height×width={pixmap.height()}×{pixmap.width()}，' \
-              f'scale={canvas.scale:g}，shapes_num={shapes_num}'
+        tip = f'本图信息：图片文件大小={filesize}, 高×宽={pixmap.height()}×{pixmap.width()}，' \
+              f'形状数={shapes_num}'
         return tip
 
     def get_shape_desc(self, shape, pos):
         # 1 形状、坐标点（四舍五入保留整数值）
         tip = 'shape信息：' + shape.shape_type
         tip += ' ' + str([(round_int(p.x()), round_int(p.y())) for p in shape.points])
         # 2 如果有flags标记
```

### Comparing `xllabelme-5.1.3/xllabelme.egg-info/PKG-INFO` & `xllabelme-5.1.4/xllabelme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xllabelme
-Version: 5.1.3
+Version: 5.1.4
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada
 Author-email: 877362867@qq.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xllabelme Version: 5.1.3 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: xllabelme Version: 5.1.4 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada Author-email: 877362867@qq.com License: GPLv3
 Keywords: Image Annotation,Machine Learning Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `xllabelme-5.1.3/xllabelme.egg-info/SOURCES.txt` & `xllabelme-5.1.4/xllabelme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

