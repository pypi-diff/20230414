# Comparing `tmp/QPUIQ-0.1.2.tar.gz` & `tmp/QPUIQ-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.1.2.tar", last modified: Mon Mar 13 18:12:44 2023, max compression
+gzip compressed data, was "QPUIQ-0.1.3.tar", last modified: Fri Apr 14 18:26:32 2023, max compression
```

## Comparing `QPUIQ-0.1.2.tar` & `QPUIQ-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,71 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-03-13 18:12:44.561641 QPUIQ-0.1.2/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.2/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2047 2023-03-13 18:12:44.561469 QPUIQ-0.1.2/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-03-13 18:12:44.548176 QPUIQ-0.1.2/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-03-13 18:12:44.551370 QPUIQ-0.1.2/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)      134 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      648 2023-03-13 17:06:52.000000 QPUIQ-0.1.2/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      576 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1625 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      374 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      543 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      814 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1188 2023-03-13 17:05:50.000000 QPUIQ-0.1.2/PUI/PySide6/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-03-13 18:12:44.553392 QPUIQ-0.1.2/PUI/Qt5/
--rw-r--r--   0 Bug        (504) staff       (20)      134 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/Qt5/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      645 2023-03-13 17:04:28.000000 QPUIQ-0.1.2/PUI/Qt5/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      576 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/Qt5/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1619 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/Qt5/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      374 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/Qt5/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/Qt5/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      814 2023-03-13 15:01:12.000000 QPUIQ-0.1.2/PUI/Qt5/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1146 2023-03-13 17:06:10.000000 QPUIQ-0.1.2/PUI/Qt5/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      101 2023-03-12 11:19:10.000000 QPUIQ-0.1.2/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      150 2023-03-11 14:26:04.000000 QPUIQ-0.1.2/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     1619 2023-03-13 17:07:54.000000 QPUIQ-0.1.2/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-03-13 18:12:44.557737 QPUIQ-0.1.2/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      112 2023-03-13 14:42:28.000000 QPUIQ-0.1.2/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.2/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      536 2023-03-13 16:17:26.000000 QPUIQ-0.1.2/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.2/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      843 2023-03-13 17:03:57.000000 QPUIQ-0.1.2/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.2/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      553 2023-03-13 17:06:36.000000 QPUIQ-0.1.2/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     1636 2023-03-13 16:19:24.000000 QPUIQ-0.1.2/PUI/generic.py
--rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-03-13 17:02:57.000000 QPUIQ-0.1.2/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)     1196 2023-03-13 18:12:41.000000 QPUIQ-0.1.2/PUI/state.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-03-13 18:12:44.560623 QPUIQ-0.1.2/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      134 2023-03-13 14:32:48.000000 QPUIQ-0.1.2/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      315 2023-03-13 17:14:19.000000 QPUIQ-0.1.2/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      583 2023-03-11 07:47:43.000000 QPUIQ-0.1.2/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      929 2023-03-11 19:15:30.000000 QPUIQ-0.1.2/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      458 2023-03-11 07:47:32.000000 QPUIQ-0.1.2/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1168 2023-03-13 18:02:16.000000 QPUIQ-0.1.2/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      923 2023-03-12 15:05:45.000000 QPUIQ-0.1.2/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1306 2023-03-13 17:57:03.000000 QPUIQ-0.1.2/PUI/tkinter/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      741 2023-03-13 10:42:13.000000 QPUIQ-0.1.2/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-03-13 18:12:44.561237 QPUIQ-0.1.2/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     2047 2023-03-13 18:12:44.000000 QPUIQ-0.1.2/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)      879 2023-03-13 18:12:44.000000 QPUIQ-0.1.2/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-03-13 18:12:44.000000 QPUIQ-0.1.2/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-03-13 18:12:44.000000 QPUIQ-0.1.2/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     1788 2023-03-13 18:10:38.000000 QPUIQ-0.1.2/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-03-13 18:12:44.561684 QPUIQ-0.1.2/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      507 2023-03-13 18:12:23.000000 QPUIQ-0.1.2/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.184424 QPUIQ-0.1.3/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.3/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2786 2023-04-14 18:26:32.184251 QPUIQ-0.1.3/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.172098 QPUIQ-0.1.3/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.174467 QPUIQ-0.1.3/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)      362 2023-03-14 19:58:34.000000 QPUIQ-0.1.3/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:58:40.000000 QPUIQ-0.1.3/PUI/PySide6/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      853 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      638 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1625 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      374 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      543 2023-03-16 10:07:28.000000 QPUIQ-0.1.3/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      486 2023-03-14 19:58:20.000000 QPUIQ-0.1.3/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      814 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1595 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/PySide6/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.177054 QPUIQ-0.1.3/PUI/Qt5/
+-rw-r--r--   0 Bug        (504) staff       (20)      362 2023-03-14 19:52:55.000000 QPUIQ-0.1.3/PUI/Qt5/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:53:05.000000 QPUIQ-0.1.3/PUI/Qt5/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      850 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/Qt5/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      638 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/Qt5/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1619 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/Qt5/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      374 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/Qt5/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/Qt5/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      486 2023-03-14 19:54:41.000000 QPUIQ-0.1.3/PUI/Qt5/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      814 2023-03-13 15:01:12.000000 QPUIQ-0.1.3/PUI/Qt5/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1557 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/Qt5/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      463 2023-03-16 06:42:21.000000 QPUIQ-0.1.3/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      236 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1953 2023-03-16 09:17:17.000000 QPUIQ-0.1.3/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.179061 QPUIQ-0.1.3/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      398 2023-03-14 19:57:42.000000 QPUIQ-0.1.3/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:55:09.000000 QPUIQ-0.1.3/PUI/flet/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.3/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.3/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.3/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.3/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.3/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      682 2023-04-14 18:25:52.000000 QPUIQ-0.1.3/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3171 2023-04-14 18:23:56.000000 QPUIQ-0.1.3/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)     8425 2023-04-14 18:23:56.000000 QPUIQ-0.1.3/PUI/state.py
+-rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.3/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.181464 QPUIQ-0.1.3/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      359 2023-03-14 19:48:08.000000 QPUIQ-0.1.3/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:43:49.000000 QPUIQ-0.1.3/PUI/tkinter/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      359 2023-03-14 19:48:57.000000 QPUIQ-0.1.3/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      550 2023-03-14 19:48:50.000000 QPUIQ-0.1.3/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      896 2023-03-14 19:49:44.000000 QPUIQ-0.1.3/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:49:39.000000 QPUIQ-0.1.3/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1102 2023-03-14 19:49:35.000000 QPUIQ-0.1.3/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      490 2023-03-14 19:50:09.000000 QPUIQ-0.1.3/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      890 2023-03-14 19:49:07.000000 QPUIQ-0.1.3/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1272 2023-03-16 07:43:13.000000 QPUIQ-0.1.3/PUI/tkinter/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.183511 QPUIQ-0.1.3/PUI/urwid/
+-rw-r--r--   0 Bug        (504) staff       (20)      375 2023-03-14 19:40:06.000000 QPUIQ-0.1.3/PUI/urwid/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      597 2023-03-14 19:36:22.000000 QPUIQ-0.1.3/PUI/urwid/__main__.py
+-rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.3/PUI/urwid/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.3/PUI/urwid/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.3/PUI/urwid/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.3/PUI/urwid/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.3/PUI/urwid/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1318 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/urwid/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1268 2023-04-14 18:19:33.000000 QPUIQ-0.1.3/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-14 18:26:32.184028 QPUIQ-0.1.3/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     2786 2023-04-14 18:26:32.000000 QPUIQ-0.1.3/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1236 2023-04-14 18:26:32.000000 QPUIQ-0.1.3/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-04-14 18:26:32.000000 QPUIQ-0.1.3/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-04-14 18:26:32.000000 QPUIQ-0.1.3/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2526 2023-04-14 18:25:52.000000 QPUIQ-0.1.3/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-04-14 18:26:32.184467 QPUIQ-0.1.3/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      507 2023-04-14 18:25:24.000000 QPUIQ-0.1.3/setup.py
```

### Comparing `QPUIQ-0.1.2/LICENSE.txt` & `QPUIQ-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.2/PKG-INFO` & `QPUIQ-0.1.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,20 @@
-Metadata-Version: 2.1
-Name: QPUIQ
-Version: 0.1.2
-Summary: "PUI" Python Declarative UI Framework
-Home-page: https://github.com/buganini/PUI
-Author: Buganini Chiu
-Author-email: buganini@b612.tw
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Install
 ```
 pip install QPUIQ
 ```
 
 # Example
 ## Code
 ```python
-import PUI
-PUI.BACKEND = "PySide6"
 from PUI import State
-from PUI.generic import *
+# from PUI.tkinter import *
+from PUI.PySide6 import *
+# from PUI.Qt5 import *
+# from PUI.flet import *
 
 data = State()
 class Example(Window):
     def __init__(self):
         super().__init__(title="blah", size=(640,480))
         data.var = 50
 
@@ -76,39 +67,79 @@
   }
 }
 ```
 
 # More Example
 See `examples/*.py`
 
+# Planned Backends
+* tkinter
+* PyQt5
+* PySide6
+* flet
+* urwid (Text Mode)
+
+# Generic Expression
+## Elements
+* HBox()
+* VBox()
+* Button(text, callback)
+* Label(text)
+* TextField(binding)
+* ProgressBar(progress `0-1`)
+* Canvas
+    * CanvasText
+    * CanvasLine
+## Layout
+* .layout(weight=1)
+* .weight(1)
+
+# Hot Reload
+Add these lines to your view file and run with `reloadium`
+```python
+import reloadium
+
+# reloadium: after_reload
+def after_reload(actions):
+    PUIView.reload()
+```
+
 # Progress
 * State
     * ~~Update Trigger~~
     * ~~Binding~~
-    * List/Dict and Lazy UI
-* Verify Nested View
+    * ~~StateList~~
+    * ~~StateDict~~
+    * Lazy UI?
+* Passing state to subview
+* StateObject decorator
 * Adapters
-    * Split Application/Window
+    * Split Application/Window, multi-windows
+    * Navigation Stack
+    * View Router
     * ~~Label~~
     * ~~Button~~
     * ~~TextField~~
+    * ~~TimelimeView~~
     * Layout
         * ~~HBox~~
         * ~~VBox~~
         * ZBox
         * Grid
             * Row
             * Column
+        * SwiftUI style overlay ??
     * Canvas
         * ~~Text~~
         * ~~Line~~
         * Rect
         * Arc
         * Image
         * ...
     * Table
     * Tree
-    * Scrollbar
+    * Scrollbar (or as a layout setting)
 * Better DOM syncer
     * Prevent unnecessary nested update
     * Trace Event Source (TextField) and prevent udpate it DOM Sync
-    * update() -> sync()/inflate()/update()
+    * update() -> sync()/inflate()/update() ?
+* Pydantic State
```

### Comparing `QPUIQ-0.1.2/PUI/PySide6/base.py` & `QPUIQ-0.1.3/PUI/PySide6/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from .. import *
 
-from PySide6 import QtWidgets
+from PySide6 import QtCore, QtWidgets
 
 class QtBaseWidget(PUINode):
     def destroy(self):
         self.ui.deleteLater()
 
 class QtBaseLayout(PUINode):
     def addChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.ui.addLayout(child.ui)
-        else:
+        elif isinstance(child, QtBaseWidget):
             params = {}
             if not child.layout_weight is None:
                 params["stretch"] = child.layout_weight
             self.ui.addWidget(child.ui, **params)
+        else:
+            self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
-            self.ui.removeItem(child.ui)
+            self.box.removeItem(child.ui)
+        elif isinstance(child, QtBaseWidget):
+            child.ui.setParent(None)
         else:
-            child.ui.setParent(None)
+            self.removeChild(idx, child.children[0])
```

### Comparing `QPUIQ-0.1.2/PUI/PySide6/button.py` & `QPUIQ-0.1.3/PUI/PySide6/button.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,13 +7,16 @@
         self.text = text
         self.callback = callback
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
             self.ui.setText(self.text)
-            self.ui.clicked.disconnect()
+            try:
+                self.ui.clicked.disconnect()
+            except:
+                pass
             self.ui.clicked.connect(self.callback)
         else:
             self.ui = QtWidgets.QPushButton(text=self.text)
             self.ui.clicked.connect(self.callback)
         return self.ui
```

### Comparing `QPUIQ-0.1.2/PUI/PySide6/canvas.py` & `QPUIQ-0.1.3/PUI/PySide6/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.2/PUI/PySide6/layout.py` & `QPUIQ-0.1.3/PUI/PySide6/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.2/PUI/PySide6/textfield.py` & `QPUIQ-0.1.3/PUI/PySide6/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.2/PUI/PySide6/window.py` & `QPUIQ-0.1.3/PUI/Qt5/window.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from .. import *
 from .base import *
 
+class QtWindowSignal(QtCore.QObject):
+    redraw = QtCore.pyqtSignal()
+
 class QtWindow(PUIView):
     def __init__(self, title=None, size=None):
         super().__init__()
         self.title = title
         self.size = size
+        self.signal = QtWindowSignal()
+        self.signal.redraw.connect(self.update)
+
+    def redraw(self):
+        self.signal.redraw.emit()
 
     def update(self):
         if not hasattr(self, "window"):
-            from PySide6 import QtWidgets
             self.app = QtWidgets.QApplication([])
             self.window = QtWidgets.QWidget()
             self.window.setObjectName("Window")
             self.box = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.Direction.LeftToRight)
             self.window.setLayout(self.box)
 
         if not self.title is None:
@@ -22,19 +29,23 @@
             self.window.resize(*self.size)
 
         super().update()
 
     def addChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.box.addLayout(child.ui)
-        else:
+        elif isinstance(child, QtBaseWidget):
             self.box.addWidget(child.ui)
+        else:
+            self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.box.removeItem(child.ui)
-        else:
+        elif isinstance(child, QtBaseWidget):
             child.ui.setParent(None)
+        else:
+            self.removeChild(idx, child.children[0])
 
     def start(self):
         self.window.show()
         self.app.exec_()
```

### Comparing `QPUIQ-0.1.2/PUI/Qt5/base.py` & `QPUIQ-0.1.3/PUI/Qt5/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from .. import *
-from PyQt5 import QtWidgets
+from PyQt5 import QtCore, QtWidgets
 
 class QtBaseWidget(PUINode):
     def destroy(self):
         self.ui.deleteLater()
 
 class QtBaseLayout(PUINode):
     def addChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.ui.addLayout(child.ui)
-        else:
+        elif isinstance(child, QtBaseWidget):
             params = {}
             if not child.layout_weight is None:
                 params["stretch"] = child.layout_weight
             self.ui.addWidget(child.ui, **params)
+        else:
+            self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
-            self.ui.removeItem(child.ui)
+            self.box.removeItem(child.ui)
+        elif isinstance(child, QtBaseWidget):
+            child.ui.setParent(None)
         else:
-            child.ui.setParent(None)
+            self.removeChild(idx, child.children[0])
```

### Comparing `QPUIQ-0.1.2/PUI/Qt5/button.py` & `QPUIQ-0.1.3/PUI/Qt5/button.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,13 +7,16 @@
         self.text = text
         self.callback = callback
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
             self.ui.setText(self.text)
-            self.ui.clicked.disconnect()
+            try:
+                self.ui.clicked.disconnect()
+            except:
+                pass
             self.ui.clicked.connect(self.callback)
         else:
             self.ui = QtWidgets.QPushButton(text=self.text)
             self.ui.clicked.connect(self.callback)
         return self.ui
```

### Comparing `QPUIQ-0.1.2/PUI/Qt5/canvas.py` & `QPUIQ-0.1.3/PUI/Qt5/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.2/PUI/Qt5/layout.py` & `QPUIQ-0.1.3/PUI/Qt5/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.2/PUI/Qt5/textfield.py` & `QPUIQ-0.1.3/PUI/Qt5/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.2/PUI/Qt5/window.py` & `QPUIQ-0.1.3/PUI/PySide6/window.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from .. import *
 from .base import *
 
+class QtWindowSignal(QtCore.QObject):
+    redraw = QtCore.Signal()
+
 class QtWindow(PUIView):
     def __init__(self, title=None, size=None):
         super().__init__()
         self.title = title
         self.size = size
+        self.signal = QtWindowSignal()
+        self.signal.redraw.connect(self.update)
+
+    def redraw(self):
+        self.signal.redraw.emit()
 
     def update(self):
         if not hasattr(self, "window"):
+            from PySide6 import QtWidgets
             self.app = QtWidgets.QApplication([])
             self.window = QtWidgets.QWidget()
             self.window.setObjectName("Window")
             self.box = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.Direction.LeftToRight)
             self.window.setLayout(self.box)
 
         if not self.title is None:
@@ -21,19 +30,23 @@
             self.window.resize(*self.size)
 
         super().update()
 
     def addChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.box.addLayout(child.ui)
-        else:
+        elif isinstance(child, QtBaseWidget):
             self.box.addWidget(child.ui)
+        else:
+            self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.box.removeItem(child.ui)
-        else:
+        elif isinstance(child, QtBaseWidget):
             child.ui.setParent(None)
+        else:
+            self.removeChild(idx, child.children[0])
 
     def start(self):
         self.window.show()
         self.app.exec_()
```

### Comparing `QPUIQ-0.1.2/PUI/dom.py` & `QPUIQ-0.1.3/PUI/dom.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 def recur_delete(node, idx, child):
     for sidx,sc in enumerate(child.children):
         recur_delete(child, sidx, sc)
     node.removeChild(idx, child)
     child.destroy()
 
-def sync(node, oldDOM, newDOM):
+def sync(node, oldDOM, newDOM, children_first):
     oldMap = [x.key for x in oldDOM]
 
     skipHead = 0
     for i in range(0, min(len(oldDOM), len(newDOM))):
         if oldDOM[i].key == newDOM[i].key:
             oldMap[i] = None
             old = oldDOM[i]
             new = newDOM[i]
             new.update(old)
-            sync(new, old.children, new.children)
+            sync(new, old.children, new.children, children_first)
             skipHead += 1
         else:
             break
 
     skipTail = 0
     # for i in range(0, min(len(oldDOM)-skipHead, len(newDOM)-skipHead)):
     #     if oldDOM[-1-i].key == newDOM[-1-i].key:
@@ -35,18 +35,24 @@
         new_idx = skipHead + i
         try:
             old_idx = oldMap.index(new.key)
             oldMap[old_idx] = None
             old = oldDOM[old_idx]
             node.removeChild(old_idx, old)
             new.update(old)
+            if children_first:
+                sync(new, old.children, new.children, children_first)
             node.addChild(new_idx, old)
-            sync(new, old.children, new.children)
+            if not children_first:
+                sync(new, old.children, new.children, children_first)
         except:
             new.update(None)
+            if children_first:
+                sync(new, [], new.children, children_first)
             node.addChild(new_idx, new)
-            sync(new, [], new.children)
+            if not children_first:
+                sync(new, [], new.children, children_first)
 
     for old_idx, key in enumerate(oldMap):
         if key:
             old = oldDOM[old_idx]
             recur_delete(node, old_idx, old)
```

### Comparing `QPUIQ-0.1.2/PUI/flet/button.py` & `QPUIQ-0.1.3/PUI/flet/button.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,12 +7,15 @@
         self.text = text
         self.callback = callback
         self.kwargs = kwargs
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
+            self.ui.text = self.text
+            self.ui.on_click = self.on_click
+            self.ui.update()
         else:
             self.ui = ft.ElevatedButton(text=self.text, on_click=self.on_click, expand=self.layout_weight, **self.kwargs)
 
     def on_click(self, *args):
         self.callback()
```

### Comparing `QPUIQ-0.1.2/PUI/flet/layout.py` & `QPUIQ-0.1.3/PUI/flet/window.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from .. import *
 from .base import *
 
-class FRow(FBase):
-    def update(self, prev):
-        if prev and hasattr(prev, "ui"):
-            self.ui = prev.ui
-        else:
-            self.ui = ft.Row(expand=self.layout_weight)
+class FWindow(PUIView):
+    def __init__(self, title=None, size=None):
+        super().__init__()
+        self.ready = False
+        self.children_first = True
+        self.title = title
+        self.size = size
+
+    def update(self):
+        if not self.ready:
+            return
+        super().update()
+
+    def flet_app(self, page: ft.Page):
+        self.ui = page
+        self.ui.title = self.title
+        self.ready = True
+        self.update()
 
     def addChild(self, idx, child):
-        self.ui.controls.append(child.ui)
-        self.ui.update()
+        self.ui.add(child.ui)
 
     def removeChild(self, idx, child):
-        self.ui.controls.remove(child.ui)
-        self.ui.update()
+        self.ui.remove(child.ui)
 
-class FColumn(FBase):
-    def update(self, prev):
-        if prev and hasattr(prev, "ui"):
-            self.ui = prev.ui
-        else:
-            self.ui = ft.Column(expand=self.layout_weight)
-
-    def addChild(self, idx, child):
-        self.ui.controls.append(child.ui)
-        self.ui.update()
-
-    def removeChild(self, idx, child):
-        self.ui.controls.remove(child.ui)
-        self.ui.update()
+    def start(self):
+        ft.app(self.flet_app)
```

### Comparing `QPUIQ-0.1.2/PUI/flet/textfield.py` & `QPUIQ-0.1.3/PUI/flet/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.2/PUI/flet/window.py` & `QPUIQ-0.1.3/PUI/urwid/layout.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from .. import *
 from .base import *
 
-class FWindow(PUIView):
-    def __init__(self, title=None, size=None):
-        super().__init__()
-        self.ready = False
-        self.title = title
-        self.size = size
-
-    def flet_app(self, page: ft.Page):
-        self.ui = page
-        self.ui.title = self.title
-        self.ready = True
-        self.update()
+class UColumns(UBase):
+    def update(self, prev):
+        if prev and hasattr(prev, "ui"):
+            self.ui = prev.ui
+        else:
+            self.ui = urwid.Columns([])
 
     def addChild(self, idx, child):
-        self.ui.add(child.ui)
+        self.ui.contents.append((child.ui, self.ui.options()))
 
     def removeChild(self, idx, child):
-        self.ui.remove(child.ui)
+        self.ui.contents.pop(idx)
 
-    def start(self):
-        ft.app(self.flet_app)
+
+class UPile(UBase):
+    def update(self, prev):
+        if prev and hasattr(prev, "ui"):
+            self.ui = prev.ui
+        else:
+            self.ui = urwid.Pile([])
+
+    def addChild(self, idx, child):
+        self.ui.contents.append((child.ui, self.ui.options()))
+
+    def removeChild(self, idx, child):
+        self.ui.contents.pop(idx)
```

### Comparing `QPUIQ-0.1.2/PUI/node.py` & `QPUIQ-0.1.3/PUI/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 def find_pui():
     import inspect
     from .view import PUIView
     frame = inspect.currentframe()
+    frames = []
     while frame:
+        frames.insert(0, frame)
         views = [v for k,v in frame.f_locals.items() if isinstance(v, PUIView) and v.frames]
         if views:
             root = views[0]
             parent = root.frames[-1]
-            return root, parent
+
+            for f in frames:
+                fi = inspect.getframeinfo(f)
+                # print(repr(fi.function), fi.filename, fi.lineno)
+                if fi.function != "__wrapped_content__":
+                    key = f"{fi.filename}:{fi.lineno}"
+                    break
+
+            return root, parent, key
         frame = frame.f_back
     else:
         raise RuntimeError("PUIView not found")
 
-def get_key(root, node):
-    return "|".join([type(x).__name__ for x in root.frames]+[type(node).__name__])
-
 class PUINode():
     def __init__(self):
         from .view import PUIView
         self.layout_weight = None
         self.ui = None
         if isinstance(self, PUIView):
             self.root = self
             self.parent = self
+            self.key = "|".join([type(x).__name__ for x in self.root.frames]+[type(self).__name__])
         else:
-            self.root, self.parent = find_pui()
+            self.root, self.parent, key = find_pui()
+            self.key = "|".join([type(x).__name__ for x in self.root.frames]+[type(self).__name__]+[key])
 
         self.children = []
 
         if self.parent is self:
             self.path = tuple()
         else:
             self.path = self.parent.path + tuple([len(self.parent.children)])
             self.parent.children.append(self)
         # print(type(self).__name__, self.path, "parent=", self.parent.path)
 
-        self.key = get_key(self.root, self)
 
     def __enter__(self):
         # print("enter", type(self).__name__, id(self))
         self.root.frames.append(self)
         return self
 
     def __exit__(self, ex_type, value, traceback):
         # print("exit", type(self).__name__, id(self))
         self.root.frames.pop()
-        if type is None:
+        if ex_type is None: # don't consume exception
             return self
 
     def comment(self):
         return None
 
     def update(self, prev):
         return None
@@ -69,16 +77,16 @@
             "  "*len(self.path),
             type(self).__name__,
             # f"@{str(id(self))}", # print view id
             " {",
         ]
 
         # print view key
-        # headline.append(" # ")
-        # headline.append(self.key)
+        headline.append(" # ")
+        headline.append(self.key)
 
         headline.append("\n")
         segs.append("".join(headline))
 
         comment = self.comment()
         if comment:
             segs.append("  "*(len(self.path)+1))
@@ -90,10 +98,15 @@
             if i > 0:
                 segs.append(",\n")
             segs.append(c.__repr__())
         segs.append("\n")
         segs.append("".join(["  "*len(self.path), "}"]))
         return "".join(segs)
 
+    def layout(self, weight=None):
+        if not weight is None:
+            self.layout_weight = weight
+        return self
+
     def weight(self, v):
         self.layout_weight = v
         return self
```

### Comparing `QPUIQ-0.1.2/PUI/state.py` & `QPUIQ-0.1.3/PUI/timeline.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-import inspect
+from threading import Timer
 from .view import *
 
-class MutableWrapper():
-    def __init__(self, parent, key):
-        self.parent = parent
-        self.key = key
-        dt = type(getattr(self.parent, self.key))
-        if dt is str:
-            self.func = str
-        elif dt is int:
-            self.func = int
-        elif dt is float:
-            self.func = float
+class TimelineView(PUINode):
+    def __init__(self, ttl_sec):
+        super().__init__()
+        self.ttl_sec = ttl_sec
+
+    def update(self, prev):
+        if prev and hasattr(prev, "timer"):
+            self.timer = prev.timer
         else:
-            self.func = lambda x:x
+            self.timer = Timer(self.ttl_sec, self.timer_cb)
+            self.timer.start()
 
-    @property
-    def value(self):
-        return getattr(self.parent, self.key)
-
-    @value.setter
-    def value(self, value):
+    def timer_cb(self):
         try:
-            setattr(self.parent, self.key, self.func(value))
+            self.root.redraw()
+            self.timer = Timer(self.ttl_sec, self.timer_cb)
+            self.timer.start()
         except:
             pass
 
-class State():
-    def __init__(self):
-        self.__listeners = set()
-
-    def __getattribute__(self, key):
-        if not key.startswith("_"):
-            try:
-                root, parent = find_pui()
-                self.__listeners.add(root)
-            except:
-                pass
-        return object.__getattribute__(self, key)
-
-    def __setattr__(self, key, value):
-        object.__setattr__(self, key, value)
-        for l in self.__listeners:
-            l.update()
+    @property
+    def ui(self):
+        return self.children[0].ui
+
+    @ui.setter
+    def ui(self, new_ui):
+        pass
+
+    def destroy(self):
+        timer = self.timer
+        self.timer = None
+        if timer:
+            timer.cancel()
+
+    def addChild(self, idx, child):
+        self.parent.addChild(idx, child)
 
-    def __call__(self, key):
-        return MutableWrapper(self, key)
+    def removeChild(self, idx, child):
+        self.parent.removeChild(idx, child)
```

### Comparing `QPUIQ-0.1.2/PUI/tkinter/canvas.py` & `QPUIQ-0.1.3/PUI/tkinter/canvas.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,14 @@
         super().__init__(**kwargs)
         self.size = size
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            import tkinter as tk
             self.ui = tk.Canvas(self.parent.ui, **self.kwargs)
         self.ui.delete("all")
         return self.ui
 
 class TkCanvasText(PUINode):
     def __init__(self, x, y, text):
         super().__init__()
```

### Comparing `QPUIQ-0.1.2/PUI/tkinter/layout.py` & `QPUIQ-0.1.3/PUI/tkinter/layout.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from .base import *
 
 class TkHBox(TkBaseWidget):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            import tkinter as tk
             self.ui = tk.Frame(self.parent.ui)
             self.ui.rowconfigure(0, weight=1)
 
     def addChild(self, idx, child):
         child.ui.grid(row=0, column=idx, sticky='nsew')
         if not child.layout_weight is None:
             self.ui.columnconfigure(idx, weight=child.layout_weight)
@@ -19,15 +18,14 @@
         child.ui.grid_forget()
 
 class TkVBox(TkBaseWidget):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            import tkinter as tk
             self.ui = tk.Frame(self.parent.ui)
             self.ui.config(bg="white")
             self.ui.columnconfigure(0, weight=1)
 
     def addChild(self, idx, child):
         child.ui.grid(row=idx, column=0, sticky='nsew')
         if not child.layout_weight is None:
```

### Comparing `QPUIQ-0.1.2/PUI/tkinter/textfield.py` & `QPUIQ-0.1.3/PUI/tkinter/textfield.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         if prev and hasattr(prev, "ui"):
             self.variable = prev.variable
             self.ui = prev.ui
             if prev.last_value != value:
                 self.variable.set(value)
             self.last_value = value
         else:
-            import tkinter as tk
             self.variable = tk.StringVar(self.parent.ui, str(value))
             self.variable.trace_add("write", self.on_variable_changed)
             self.last_value = value
             self.ui = tk.Entry(self.parent.ui, textvariable=self.variable, **self.kwargs)
 
         return self.ui
```

### Comparing `QPUIQ-0.1.2/PUI/tkinter/window.py` & `QPUIQ-0.1.3/PUI/tkinter/window.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from .. import *
-import tkinter as tk
+from .base import *
 
 class TkWindow(PUIView):
     def __init__(self, title=None, size=None):
         super().__init__()
         self.title = title
         self.size = size
 
     def update(self):
         if not hasattr(self, "ui") or not self.ui:
-            import tkinter as tk
             self.ui = tk.Tk()
         if not self.title is None:
             self.ui.title(self.title)
         if not self.size is None:
             self.ui.geometry("x".join([str(v) for v in self.size]))
         self.ui.resizable(False, False)
         self.ui.iconbitmap('icon.ico')
```

### Comparing `QPUIQ-0.1.2/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.2
+Version: 0.1.3
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -12,18 +12,19 @@
 ```
 pip install QPUIQ
 ```
 
 # Example
 ## Code
 ```python
-import PUI
-PUI.BACKEND = "PySide6"
 from PUI import State
-from PUI.generic import *
+# from PUI.tkinter import *
+from PUI.PySide6 import *
+# from PUI.Qt5 import *
+# from PUI.flet import *
 
 data = State()
 class Example(Window):
     def __init__(self):
         super().__init__(title="blah", size=(640,480))
         data.var = 50
 
@@ -76,39 +77,79 @@
   }
 }
 ```
 
 # More Example
 See `examples/*.py`
 
+# Planned Backends
+* tkinter
+* PyQt5
+* PySide6
+* flet
+* urwid (Text Mode)
+
+# Generic Expression
+## Elements
+* HBox()
+* VBox()
+* Button(text, callback)
+* Label(text)
+* TextField(binding)
+* ProgressBar(progress `0-1`)
+* Canvas
+    * CanvasText
+    * CanvasLine
+## Layout
+* .layout(weight=1)
+* .weight(1)
+
+# Hot Reload
+Add these lines to your view file and run with `reloadium`
+```python
+import reloadium
+
+# reloadium: after_reload
+def after_reload(actions):
+    PUIView.reload()
+```
+
 # Progress
 * State
     * ~~Update Trigger~~
     * ~~Binding~~
-    * List/Dict and Lazy UI
-* Verify Nested View
+    * ~~StateList~~
+    * ~~StateDict~~
+    * Lazy UI?
+* Passing state to subview
+* StateObject decorator
 * Adapters
-    * Split Application/Window
+    * Split Application/Window, multi-windows
+    * Navigation Stack
+    * View Router
     * ~~Label~~
     * ~~Button~~
     * ~~TextField~~
+    * ~~TimelimeView~~
     * Layout
         * ~~HBox~~
         * ~~VBox~~
         * ZBox
         * Grid
             * Row
             * Column
+        * SwiftUI style overlay ??
     * Canvas
         * ~~Text~~
         * ~~Line~~
         * Rect
         * Arc
         * Image
         * ...
     * Table
     * Tree
-    * Scrollbar
+    * Scrollbar (or as a layout setting)
 * Better DOM syncer
     * Prevent unnecessary nested update
     * Trace Event Source (TextField) and prevent udpate it DOM Sync
-    * update() -> sync()/inflate()/update()
+    * update() -> sync()/inflate()/update() ?
+* Pydantic State
```

### Comparing `QPUIQ-0.1.2/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.1.3/QPUIQ.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,61 @@
 LICENSE.txt
 README.md
 setup.py
 PUI/__init__.py
 PUI/decorator.py
 PUI/dom.py
-PUI/generic.py
 PUI/node.py
 PUI/state.py
+PUI/timeline.py
 PUI/view.py
 PUI/PySide6/__init__.py
+PUI/PySide6/__main__.py
 PUI/PySide6/base.py
 PUI/PySide6/button.py
 PUI/PySide6/canvas.py
 PUI/PySide6/label.py
 PUI/PySide6/layout.py
+PUI/PySide6/progressbar.py
 PUI/PySide6/textfield.py
 PUI/PySide6/window.py
 PUI/Qt5/__init__.py
+PUI/Qt5/__main__.py
 PUI/Qt5/base.py
 PUI/Qt5/button.py
 PUI/Qt5/canvas.py
 PUI/Qt5/label.py
 PUI/Qt5/layout.py
+PUI/Qt5/progressbar.py
 PUI/Qt5/textfield.py
 PUI/Qt5/window.py
 PUI/flet/__init__.py
+PUI/flet/__main__.py
 PUI/flet/base.py
 PUI/flet/button.py
 PUI/flet/label.py
 PUI/flet/layout.py
+PUI/flet/progressbar.py
 PUI/flet/textfield.py
 PUI/flet/window.py
 PUI/tkinter/__init__.py
+PUI/tkinter/__main__.py
 PUI/tkinter/base.py
 PUI/tkinter/button.py
 PUI/tkinter/canvas.py
 PUI/tkinter/label.py
 PUI/tkinter/layout.py
+PUI/tkinter/progressbar.py
 PUI/tkinter/textfield.py
 PUI/tkinter/window.py
+PUI/urwid/__init__.py
+PUI/urwid/__main__.py
+PUI/urwid/base.py
+PUI/urwid/button.py
+PUI/urwid/label.py
+PUI/urwid/layout.py
+PUI/urwid/progressbar.py
+PUI/urwid/window.py
 QPUIQ.egg-info/PKG-INFO
 QPUIQ.egg-info/SOURCES.txt
 QPUIQ.egg-info/dependency_links.txt
 QPUIQ.egg-info/top_level.txt
```

