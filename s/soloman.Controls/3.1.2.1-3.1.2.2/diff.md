# Comparing `tmp/soloman.Controls-3.1.2.1.tar.gz` & `tmp/soloman.Controls-3.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soloman.Controls-3.1.2.1.tar", last modified: Thu Mar 30 15:49:40 2023, max compression
+gzip compressed data, was "soloman.Controls-3.1.2.2.tar", last modified: Fri Apr 14 16:20:53 2023, max compression
```

## Comparing `soloman.Controls-3.1.2.1.tar` & `soloman.Controls-3.1.2.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.417012 soloman.Controls-3.1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-30 15:49:40.417012 soloman.Controls-3.1.2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PyQt5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PyQt5/Qt5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.413012 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/SButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/SComboBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/SDatePicker.qml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/SProperties.qml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/STab.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/STabView.qml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/STextArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/STextField.qml
--rw-r--r--   0 runner    (1001) docker     (123)    97112 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/fa_regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PyQt6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PyQt6/Qt6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.413012 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/SButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/SComboBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/SDatePicker.qml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/SProperties.qml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/STab.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/STabView.qml
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/STextArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/STextField.qml
--rw-r--r--   0 runner    (1001) docker     (123)    97112 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/fa_regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PySide2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PySide2/qml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PySide2/qml/soloman/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.417012 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/SButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/SComboBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/SDatePicker.qml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/SProperties.qml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/STab.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/STabView.qml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/STextArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/STextField.qml
--rw-r--r--   0 runner    (1001) docker     (123)    97112 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/fa_regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PySide6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PySide6/qml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.409012 soloman.Controls-3.1.2.1/PySide6/qml/soloman/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.417012 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/SButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/SComboBox.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/SDatePicker.qml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/SProperties.qml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/STab.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/STabView.qml
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/STextArea.qml
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/STextField.qml
--rw-r--r--   0 runner    (1001) docker     (123)    97112 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/fa_regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/qmldir
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 15:49:40.417012 soloman.Controls-3.1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-30 15:49:21.000000 soloman.Controls-3.1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:49:40.417012 soloman.Controls-3.1.2.1/soloman.Controls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-30 15:49:40.000000 soloman.Controls-3.1.2.1/soloman.Controls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-30 15:49:40.000000 soloman.Controls-3.1.2.1/soloman.Controls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 15:49:40.000000 soloman.Controls-3.1.2.1/soloman.Controls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-30 15:49:40.000000 soloman.Controls-3.1.2.1/soloman.Controls.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.669812 soloman.Controls-3.1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-14 16:20:53.669812 soloman.Controls-3.1.2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PyQt5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PyQt5/Qt5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/SButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/SComboBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/SDatePicker.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/SProperties.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/STab.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/STabView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/STextArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/STextField.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    97112 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/fa_regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PyQt6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PyQt6/Qt6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.669812 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/SButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/SComboBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/SDatePicker.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/SProperties.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/STab.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/STabView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/STextArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/STextField.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    97112 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/fa_regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PySide2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PySide2/qml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PySide2/qml/soloman/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.669812 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/SButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/SComboBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/SDatePicker.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/SProperties.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/STab.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/STabView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/STextArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/STextField.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    97112 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/fa_regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PySide6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PySide6/qml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.665812 soloman.Controls-3.1.2.2/PySide6/qml/soloman/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.669812 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/SButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/SComboBox.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/SDatePicker.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/SProperties.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/STab.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/STabView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/STextArea.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/STextField.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    97112 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/fa_regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/qmldir
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:20:53.669812 soloman.Controls-3.1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-14 16:20:40.000000 soloman.Controls-3.1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:20:53.669812 soloman.Controls-3.1.2.2/soloman.Controls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-14 16:20:53.000000 soloman.Controls-3.1.2.2/soloman.Controls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-14 16:20:53.000000 soloman.Controls-3.1.2.2/soloman.Controls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:20:53.000000 soloman.Controls-3.1.2.2/soloman.Controls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 16:20:53.000000 soloman.Controls-3.1.2.2/soloman.Controls.egg-info/top_level.txt
```

### Comparing `soloman.Controls-3.1.2.1/LICENSE` & `soloman.Controls-3.1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PKG-INFO` & `soloman.Controls-3.1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soloman.Controls
-Version: 3.1.2.1
+Version: 3.1.2.2
 Summary: For the love of python and qml
 Home-page: https://github.com/deuteronomy-works/soloman
 Author: Amoh - Gyebi Godwin Ampofo Michael
 Author-email: amohgyebigodwin@gmail.com
 Project-URL: Bug Tracker, https://github.com/deuteronomy-works/soloman/issues/
 Project-URL: Documentation, https://github.com/deuteronomy-works/soloman/wiki/
 Project-URL: Source Code, https://github.com/deuteronomy-works/soloman/
```

### Comparing `soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/SButton.qml` & `soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/SButton.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/SComboBox.qml` & `soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/SComboBox.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/SDatePicker.qml` & `soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/SDatePicker.qml`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,18 @@
         Soloman.SButton {
             Layout.fillWidth: true
             implicitHeight: 24
             Layout.alignment: Qt.AlignLeft | Qt.AlignVCenter
             text: control.selectedDate
             color: "transparent"
 
-            onClicked: popup.open()
+            onClicked: {
+                popup.x = this.x + popup.width > width ? width - popup.width : this.x
+                popup.open()
+            }
         }
     }
 
 
     Popup {
         id: popup
```

### Comparing `soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/STabView.qml` & `soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/STabView.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/fa_regular.otf` & `soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/fa_regular.otf`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PyQt5/Qt5/qml/soloman/Controls/qmldir` & `soloman.Controls-3.1.2.2/PyQt5/Qt5/qml/soloman/Controls/qmldir`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/SButton.qml` & `soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/SButton.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/SComboBox.qml` & `soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/SComboBox.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/SDatePicker.qml` & `soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/SDatePicker.qml`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,18 @@
         Soloman.SButton {
             Layout.fillWidth: true
             implicitHeight: 24
             Layout.alignment: Qt.AlignLeft | Qt.AlignVCenter
             text: control.selectedDate
             color: "transparent"
 
-            onClicked: popup.open()
+            onClicked: {
+                popup.x = this.x + popup.width > width ? width - popup.width : this.x
+                popup.open()
+            }
         }
     }
 
 
     Popup {
         id: popup
```

### Comparing `soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/STabView.qml` & `soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/STabView.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/fa_regular.otf` & `soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/fa_regular.otf`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PyQt6/Qt6/qml/soloman/Controls/qmldir` & `soloman.Controls-3.1.2.2/PyQt6/Qt6/qml/soloman/Controls/qmldir`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/SButton.qml` & `soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/SButton.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/SComboBox.qml` & `soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/SComboBox.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/SDatePicker.qml` & `soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/SDatePicker.qml`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,18 @@
         Soloman.SButton {
             Layout.fillWidth: true
             implicitHeight: 24
             Layout.alignment: Qt.AlignLeft | Qt.AlignVCenter
             text: control.selectedDate
             color: "transparent"
 
-            onClicked: popup.open()
+            onClicked: {
+                popup.x = this.x + popup.width > width ? width - popup.width : this.x
+                popup.open()
+            }
         }
     }
 
 
     Popup {
         id: popup
```

### Comparing `soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/STabView.qml` & `soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/STabView.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/fa_regular.otf` & `soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/fa_regular.otf`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PySide2/qml/soloman/Controls/qmldir` & `soloman.Controls-3.1.2.2/PySide2/qml/soloman/Controls/qmldir`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/SButton.qml` & `soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/SButton.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/SComboBox.qml` & `soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/SComboBox.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/SDatePicker.qml` & `soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/SDatePicker.qml`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,18 @@
         Soloman.SButton {
             Layout.fillWidth: true
             implicitHeight: 24
             Layout.alignment: Qt.AlignLeft | Qt.AlignVCenter
             text: control.selectedDate
             color: "transparent"
 
-            onClicked: popup.open()
+            onClicked: {
+                popup.x = this.x + popup.width > width ? width - popup.width : this.x
+                popup.open()
+            }
         }
     }
 
 
     Popup {
         id: popup
```

### Comparing `soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/STabView.qml` & `soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/STabView.qml`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/fa_regular.otf` & `soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/fa_regular.otf`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/PySide6/qml/soloman/Controls/qmldir` & `soloman.Controls-3.1.2.2/PySide6/qml/soloman/Controls/qmldir`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/README.md` & `soloman.Controls-3.1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/setup.py` & `soloman.Controls-3.1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `soloman.Controls-3.1.2.1/soloman.Controls.egg-info/PKG-INFO` & `soloman.Controls-3.1.2.2/soloman.Controls.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soloman.Controls
-Version: 3.1.2.1
+Version: 3.1.2.2
 Summary: For the love of python and qml
 Home-page: https://github.com/deuteronomy-works/soloman
 Author: Amoh - Gyebi Godwin Ampofo Michael
 Author-email: amohgyebigodwin@gmail.com
 Project-URL: Bug Tracker, https://github.com/deuteronomy-works/soloman/issues/
 Project-URL: Documentation, https://github.com/deuteronomy-works/soloman/wiki/
 Project-URL: Source Code, https://github.com/deuteronomy-works/soloman/
```

### Comparing `soloman.Controls-3.1.2.1/soloman.Controls.egg-info/SOURCES.txt` & `soloman.Controls-3.1.2.2/soloman.Controls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

