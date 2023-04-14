# Comparing `tmp/qutewindow-0.1.8.tar.gz` & `tmp/qutewindow-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qutewindow-0.1.8.tar", max compression
+gzip compressed data, was "qutewindow-0.1.9.tar", max compression
```

## Comparing `qutewindow-0.1.8.tar` & `qutewindow-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      736 2023-03-29 20:38:11.398364 qutewindow-0.1.8/README.md
--rw-r--r--   0        0        0      674 2023-03-29 20:16:26.433749 qutewindow-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       62 2023-03-29 01:31:27.345787 qutewindow-0.1.8/qutewindow/__init__.py
--rw-r--r--   0        0        0      181 2023-03-29 01:33:27.825641 qutewindow-0.1.8/qutewindow/platforms/__init__.py
--rw-r--r--   0        0        0     1041 2023-03-29 01:32:51.184344 qutewindow-0.1.8/qutewindow/platforms/mac/QuteDialog.py
--rw-r--r--   0        0        0     1040 2023-03-28 21:03:12.182087 qutewindow-0.1.8/qutewindow/platforms/mac/QuteMainWindow.py
--rw-r--r--   0        0        0     1051 2023-03-28 20:58:24.095544 qutewindow-0.1.8/qutewindow/platforms/mac/QuteWindow.py
--rw-r--r--   0        0        0      113 2023-03-29 01:33:21.553404 qutewindow-0.1.8/qutewindow/platforms/mac/__init__.py
--rw-r--r--   0        0        0     1850 2023-03-28 20:57:11.581098 qutewindow-0.1.8/qutewindow/platforms/mac/utils.py
--rw-r--r--   0        0        0     1254 2023-03-29 01:31:27.346151 qutewindow-0.1.8/qutewindow/platforms/windows/QuteDialog.py
--rw-r--r--   0        0        0     1265 2023-03-29 01:31:27.346261 qutewindow-0.1.8/qutewindow/platforms/windows/QuteMainWindow.py
--rw-r--r--   0        0        0     1253 2023-03-29 01:31:27.346911 qutewindow-0.1.8/qutewindow/platforms/windows/QuteWindow.py
--rw-r--r--   0        0        0      113 2023-03-29 01:31:27.347399 qutewindow-0.1.8/qutewindow/platforms/windows/__init__.py
--rw-r--r--   0        0        0      788 2023-03-14 12:24:22.059817 qutewindow-0.1.8/qutewindow/platforms/windows/c_structures.py
--rw-r--r--   0        0        0     3517 2023-03-29 01:31:27.347503 qutewindow-0.1.8/qutewindow/platforms/windows/native_event.py
--rw-r--r--   0        0        0     5950 2023-03-29 01:31:27.347904 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/TitleBar.py
--rw-r--r--   0        0        0        0 2023-03-14 12:24:22.060071 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/__init__.py
--rw-r--r--   0        0        0      549 2023-03-14 12:24:22.060433 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/resources.qrc
--rw-r--r--   0        0        0    13350 2023-03-14 12:24:22.060633 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/resources_rc.py
--rw-r--r--   0        0        0      245 2023-03-14 12:24:22.060836 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/close.png
--rw-r--r--   0        0        0      352 2023-03-14 12:24:22.060991 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/close@2x.png
--rw-r--r--   0        0        0      447 2023-03-14 12:24:22.061121 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/close@3x.png
--rw-r--r--   0        0        0      177 2023-03-14 12:24:22.061258 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/maximize.png
--rw-r--r--   0        0        0      255 2023-03-14 12:24:22.061708 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/maximize@2x.png
--rw-r--r--   0        0        0      319 2023-03-14 12:24:22.061965 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/maximize@3x.png
--rw-r--r--   0        0        0      150 2023-03-14 12:24:22.062116 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/minimize.png
--rw-r--r--   0        0        0      159 2023-03-14 12:24:22.062254 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/minimize@2x.png
--rw-r--r--   0        0        0      185 2023-03-14 12:24:22.062391 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/minimize@3x.png
--rw-r--r--   0        0        0      227 2023-03-14 12:24:22.062532 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/restore.png
--rw-r--r--   0        0        0      310 2023-03-14 12:24:22.062679 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/restore@2x.png
--rw-r--r--   0        0        0      385 2023-03-14 12:24:22.062826 qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/title-bar/restore@3x.png
--rw-r--r--   0        0        0     1314 2023-03-29 01:31:27.348184 qutewindow-0.1.8/qutewindow/platforms/windows/utils.py
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 qutewindow-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      736 2023-03-29 20:38:11.398364 qutewindow-0.1.9/README.md
+-rw-r--r--   0        0        0      674 2023-03-29 21:08:23.490898 qutewindow-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-03-29 01:31:27.345787 qutewindow-0.1.9/qutewindow/__init__.py
+-rw-r--r--   0        0        0      181 2023-03-29 01:33:27.825641 qutewindow-0.1.9/qutewindow/platforms/__init__.py
+-rw-r--r--   0        0        0     1041 2023-03-29 01:32:51.184344 qutewindow-0.1.9/qutewindow/platforms/mac/QuteDialog.py
+-rw-r--r--   0        0        0     1040 2023-03-28 21:03:12.182087 qutewindow-0.1.9/qutewindow/platforms/mac/QuteMainWindow.py
+-rw-r--r--   0        0        0     1051 2023-03-28 20:58:24.095544 qutewindow-0.1.9/qutewindow/platforms/mac/QuteWindow.py
+-rw-r--r--   0        0        0      113 2023-03-29 01:33:21.553404 qutewindow-0.1.9/qutewindow/platforms/mac/__init__.py
+-rw-r--r--   0        0        0     1850 2023-03-28 20:57:11.581098 qutewindow-0.1.9/qutewindow/platforms/mac/utils.py
+-rw-r--r--   0        0        0     1254 2023-03-29 01:31:27.346151 qutewindow-0.1.9/qutewindow/platforms/windows/QuteDialog.py
+-rw-r--r--   0        0        0     1265 2023-03-29 01:31:27.346261 qutewindow-0.1.9/qutewindow/platforms/windows/QuteMainWindow.py
+-rw-r--r--   0        0        0     1253 2023-03-29 01:31:27.346911 qutewindow-0.1.9/qutewindow/platforms/windows/QuteWindow.py
+-rw-r--r--   0        0        0      113 2023-03-29 01:31:27.347399 qutewindow-0.1.9/qutewindow/platforms/windows/__init__.py
+-rw-r--r--   0        0        0      788 2023-03-14 12:24:22.059817 qutewindow-0.1.9/qutewindow/platforms/windows/c_structures.py
+-rw-r--r--   0        0        0     3517 2023-03-29 01:31:27.347503 qutewindow-0.1.9/qutewindow/platforms/windows/native_event.py
+-rw-r--r--   0        0        0     5950 2023-03-29 01:31:27.347904 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/TitleBar.py
+-rw-r--r--   0        0        0        0 2023-03-14 12:24:22.060071 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/__init__.py
+-rw-r--r--   0        0        0      549 2023-03-14 12:24:22.060433 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/resources.qrc
+-rw-r--r--   0        0        0    13350 2023-03-14 12:24:22.060633 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/resources_rc.py
+-rw-r--r--   0        0        0      245 2023-03-14 12:24:22.060836 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/close.png
+-rw-r--r--   0        0        0      352 2023-03-14 12:24:22.060991 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/close@2x.png
+-rw-r--r--   0        0        0      447 2023-03-14 12:24:22.061121 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/close@3x.png
+-rw-r--r--   0        0        0      177 2023-03-14 12:24:22.061258 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/maximize.png
+-rw-r--r--   0        0        0      255 2023-03-14 12:24:22.061708 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/maximize@2x.png
+-rw-r--r--   0        0        0      319 2023-03-14 12:24:22.061965 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/maximize@3x.png
+-rw-r--r--   0        0        0      150 2023-03-14 12:24:22.062116 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/minimize.png
+-rw-r--r--   0        0        0      159 2023-03-14 12:24:22.062254 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/minimize@2x.png
+-rw-r--r--   0        0        0      185 2023-03-14 12:24:22.062391 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/minimize@3x.png
+-rw-r--r--   0        0        0      227 2023-03-14 12:24:22.062532 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/restore.png
+-rw-r--r--   0        0        0      310 2023-03-14 12:24:22.062679 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/restore@2x.png
+-rw-r--r--   0        0        0      385 2023-03-14 12:24:22.062826 qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/title-bar/restore@3x.png
+-rw-r--r--   0        0        0     1314 2023-03-29 01:31:27.348184 qutewindow-0.1.9/qutewindow/platforms/windows/utils.py
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 qutewindow-0.1.9/PKG-INFO
```

### Comparing `qutewindow-0.1.8/README.md` & `qutewindow-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/pyproject.toml` & `qutewindow-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qutewindow"
-version = "0.1.8"
+version = "0.1.9"
 description = "Cross-platform frameless window based on Python and Qt"
 authors = ["Parham Oyan <parhamoyan@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/parhamoyan/qutewindow"
 keywords = ["qt", "pyqt", "pyqt6", "pyqt5", "pyside", "pyside2", "pyside6", "frameless-window", "cross-platform"]
```

### Comparing `qutewindow-0.1.8/qutewindow/platforms/mac/QuteDialog.py` & `qutewindow-0.1.9/qutewindow/platforms/mac/QuteDialog.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/mac/QuteMainWindow.py` & `qutewindow-0.1.9/qutewindow/platforms/mac/QuteMainWindow.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/mac/QuteWindow.py` & `qutewindow-0.1.9/qutewindow/platforms/mac/QuteWindow.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/mac/utils.py` & `qutewindow-0.1.9/qutewindow/platforms/mac/utils.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/windows/QuteDialog.py` & `qutewindow-0.1.9/qutewindow/platforms/windows/QuteDialog.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/windows/QuteMainWindow.py` & `qutewindow-0.1.9/qutewindow/platforms/windows/QuteMainWindow.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/windows/QuteWindow.py` & `qutewindow-0.1.9/qutewindow/platforms/windows/QuteWindow.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/windows/c_structures.py` & `qutewindow-0.1.9/qutewindow/platforms/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/windows/native_event.py` & `qutewindow-0.1.9/qutewindow/platforms/windows/native_event.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/TitleBar.py` & `qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/TitleBar.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/resources.qrc` & `qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/resources.qrc`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/windows/title_bar/resources_rc.py` & `qutewindow-0.1.9/qutewindow/platforms/windows/title_bar/resources_rc.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/qutewindow/platforms/windows/utils.py` & `qutewindow-0.1.9/qutewindow/platforms/windows/utils.py`

 * *Files identical despite different names*

### Comparing `qutewindow-0.1.8/PKG-INFO` & `qutewindow-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qutewindow
-Version: 0.1.8
+Version: 0.1.9
 Summary: Cross-platform frameless window based on Python and Qt
 Home-page: https://github.com/parhamoyan/qutewindow
 License: MIT
 Keywords: qt,pyqt,pyqt6,pyqt5,pyside,pyside2,pyside6,frameless-window,cross-platform
 Author: Parham Oyan
 Author-email: parhamoyan@yahoo.com
 Requires-Python: >=3.0
```

