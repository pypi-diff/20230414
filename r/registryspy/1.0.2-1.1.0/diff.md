# Comparing `tmp/registryspy-1.0.2.tar.gz` & `tmp/registryspy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "registryspy-1.0.2.tar", last modified: Sun Feb 20 07:35:29 2022, max compression
+gzip compressed data, was "registryspy-1.1.0.tar", last modified: Fri Apr 14 00:44:56 2023, max compression
```

## Comparing `registryspy-1.0.2.tar` & `registryspy-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2022-02-20 07:35:29.093370 registryspy-1.0.2/
--rw-rw-rw-   0        0        0    35821 2021-11-06 03:18:01.000000 registryspy-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       66 2021-11-05 23:32:04.000000 registryspy-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2964 2022-02-20 07:35:29.092371 registryspy-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2078 2021-11-06 02:51:29.000000 registryspy-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-02-20 07:35:29.030343 registryspy-1.0.2/registryspy/
--rw-rw-rw-   0        0        0        0 2021-11-05 22:11:04.000000 registryspy-1.0.2/registryspy/__init__.py
--rw-rw-rw-   0        0        0     9086 2021-11-06 02:50:28.000000 registryspy-1.0.2/registryspy/find_dialog.py
--rw-rw-rw-   0        0        0     1859 2022-02-20 07:33:18.000000 registryspy-1.0.2/registryspy/helpers.py
--rw-rw-rw-   0        0        0     2480 2021-09-28 03:39:57.000000 registryspy-1.0.2/registryspy/hive_info_table.py
-drwxrwxrwx   0        0        0        0 2022-02-20 07:35:29.090368 registryspy-1.0.2/registryspy/img/
--rw-rw-rw-   0        0        0    16153 2021-09-24 21:31:36.000000 registryspy-1.0.2/registryspy/img/close.png
--rw-rw-rw-   0        0        0    17901 2021-09-25 02:11:53.000000 registryspy-1.0.2/registryspy/img/close_all.png
--rw-rw-rw-   0        0        0    14108 2021-10-13 07:30:10.000000 registryspy-1.0.2/registryspy/img/find.png
--rw-rw-rw-   0        0        0    19147 2021-10-15 09:39:47.000000 registryspy-1.0.2/registryspy/img/find_next.png
--rw-rw-rw-   0        0        0    19250 2021-10-15 09:39:41.000000 registryspy-1.0.2/registryspy/img/find_previous.png
--rw-rw-rw-   0        0        0     6514 2021-09-26 00:41:32.000000 registryspy-1.0.2/registryspy/img/folder.png
--rw-rw-rw-   0        0        0   131727 2021-10-08 23:15:51.000000 registryspy-1.0.2/registryspy/img/icon.ico
--rw-rw-rw-   0        0        0   129088 2021-09-24 07:37:11.000000 registryspy-1.0.2/registryspy/img/icon.png
--rw-rw-rw-   0        0        0     8238 2021-09-24 21:24:04.000000 registryspy-1.0.2/registryspy/img/open.png
--rw-rw-rw-   0        0        0    26026 2021-09-24 08:07:28.000000 registryspy-1.0.2/registryspy/img/reg_bin.png
--rw-rw-rw-   0        0        0    21333 2021-09-24 08:04:52.000000 registryspy-1.0.2/registryspy/img/reg_num.png
--rw-rw-rw-   0        0        0    22084 2021-09-24 07:57:39.000000 registryspy-1.0.2/registryspy/img/reg_str.png
--rw-rw-rw-   0        0        0    18499 2021-10-09 06:03:46.000000 registryspy-1.0.2/registryspy/img/splash.png
--rw-rw-rw-   0        0        0    17409 2021-10-09 05:57:18.000000 registryspy-1.0.2/registryspy/img/wordmark.png
--rw-rw-rw-   0        0        0    10844 2022-02-20 07:14:40.000000 registryspy-1.0.2/registryspy/key_tree.py
--rw-rw-rw-   0        0        0     1019 2021-11-05 22:25:12.000000 registryspy-1.0.2/registryspy/license_dialog.py
--rw-rw-rw-   0        0        0    12757 2021-11-05 22:25:18.000000 registryspy-1.0.2/registryspy/registryspy.py
--rw-rw-rw-   0        0        0    44713 2021-10-06 09:00:16.000000 registryspy-1.0.2/registryspy/third_party_licenses.txt
--rw-rw-rw-   0        0        0     7607 2021-11-05 22:25:03.000000 registryspy-1.0.2/registryspy/value_table.py
-drwxrwxrwx   0        0        0        0 2022-02-20 07:35:29.064579 registryspy-1.0.2/registryspy.egg-info/
--rw-rw-rw-   0        0        0     2964 2022-02-20 07:35:28.000000 registryspy-1.0.2/registryspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2022-02-20 07:35:28.000000 registryspy-1.0.2/registryspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-20 07:35:28.000000 registryspy-1.0.2/registryspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2022-02-20 07:35:28.000000 registryspy-1.0.2/registryspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2022-02-20 07:35:28.000000 registryspy-1.0.2/registryspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-02-20 07:35:28.000000 registryspy-1.0.2/registryspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       98 2021-11-06 02:39:54.000000 registryspy-1.0.2/run.py
--rw-rw-rw-   0        0        0       42 2022-02-20 07:35:29.094371 registryspy-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1349 2022-02-20 07:34:15.000000 registryspy-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:44:56.262763 registryspy-1.1.0/
+-rw-rw-rw-   0        0        0    35821 2021-11-06 03:18:01.000000 registryspy-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       66 2021-11-05 23:32:04.000000 registryspy-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3149 2023-04-14 00:44:56.262763 registryspy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2252 2023-04-14 00:41:41.000000 registryspy-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 00:44:56.237546 registryspy-1.1.0/registryspy/
+-rw-rw-rw-   0        0        0        0 2021-11-05 22:11:04.000000 registryspy-1.1.0/registryspy/__init__.py
+-rw-rw-rw-   0        0        0     1772 2023-04-13 02:18:20.000000 registryspy-1.1.0/registryspy/data_viewer.py
+-rw-rw-rw-   0        0        0     9086 2021-11-06 02:50:28.000000 registryspy-1.1.0/registryspy/find_dialog.py
+-rw-rw-rw-   0        0        0     2369 2023-04-13 02:22:25.000000 registryspy-1.1.0/registryspy/helpers.py
+-rw-rw-rw-   0        0        0     2491 2023-04-13 01:14:58.000000 registryspy-1.1.0/registryspy/hive_info_table.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:44:56.261544 registryspy-1.1.0/registryspy/img/
+-rw-rw-rw-   0        0        0    16153 2021-09-24 21:31:36.000000 registryspy-1.1.0/registryspy/img/close.png
+-rw-rw-rw-   0        0        0    17901 2021-09-25 02:11:53.000000 registryspy-1.1.0/registryspy/img/close_all.png
+-rw-rw-rw-   0        0        0    14108 2021-10-13 07:30:10.000000 registryspy-1.1.0/registryspy/img/find.png
+-rw-rw-rw-   0        0        0    19147 2021-10-15 09:39:47.000000 registryspy-1.1.0/registryspy/img/find_next.png
+-rw-rw-rw-   0        0        0    19250 2021-10-15 09:39:41.000000 registryspy-1.1.0/registryspy/img/find_previous.png
+-rw-rw-rw-   0        0        0     6514 2021-09-26 00:41:32.000000 registryspy-1.1.0/registryspy/img/folder.png
+-rw-rw-rw-   0        0        0   131727 2021-10-08 23:15:51.000000 registryspy-1.1.0/registryspy/img/icon.ico
+-rw-rw-rw-   0        0        0   129088 2021-09-24 07:37:11.000000 registryspy-1.1.0/registryspy/img/icon.png
+-rw-rw-rw-   0        0        0     8238 2021-09-24 21:24:04.000000 registryspy-1.1.0/registryspy/img/open.png
+-rw-rw-rw-   0        0        0    26026 2021-09-24 08:07:28.000000 registryspy-1.1.0/registryspy/img/reg_bin.png
+-rw-rw-rw-   0        0        0    21333 2021-09-24 08:04:52.000000 registryspy-1.1.0/registryspy/img/reg_num.png
+-rw-rw-rw-   0        0        0    22084 2021-09-24 07:57:39.000000 registryspy-1.1.0/registryspy/img/reg_str.png
+-rw-rw-rw-   0        0        0    18499 2021-10-09 06:03:46.000000 registryspy-1.1.0/registryspy/img/splash.png
+-rw-rw-rw-   0        0        0    17409 2021-10-09 05:57:18.000000 registryspy-1.1.0/registryspy/img/wordmark.png
+-rw-rw-rw-   0        0        0    10844 2022-02-20 07:14:40.000000 registryspy-1.1.0/registryspy/key_tree.py
+-rw-rw-rw-   0        0        0     1019 2021-11-05 22:25:12.000000 registryspy-1.1.0/registryspy/license_dialog.py
+-rw-rw-rw-   0        0        0    12503 2023-04-13 01:33:11.000000 registryspy-1.1.0/registryspy/registryspy.py
+-rw-rw-rw-   0        0        0    44713 2021-10-06 09:00:16.000000 registryspy-1.1.0/registryspy/third_party_licenses.txt
+-rw-rw-rw-   0        0        0     7247 2023-04-13 01:33:11.000000 registryspy-1.1.0/registryspy/value_table.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:44:56.249548 registryspy-1.1.0/registryspy.egg-info/
+-rw-rw-rw-   0        0        0     3149 2023-04-14 00:44:56.000000 registryspy-1.1.0/registryspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      921 2023-04-14 00:44:56.000000 registryspy-1.1.0/registryspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 00:44:56.000000 registryspy-1.1.0/registryspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-14 00:44:56.000000 registryspy-1.1.0/registryspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-04-14 00:44:56.000000 registryspy-1.1.0/registryspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 00:44:56.000000 registryspy-1.1.0/registryspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       98 2021-11-06 02:39:54.000000 registryspy-1.1.0/run.py
+-rw-rw-rw-   0        0        0       42 2023-04-14 00:44:56.263544 registryspy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1346 2023-04-13 02:22:38.000000 registryspy-1.1.0/setup.py
```

### Comparing `registryspy-1.0.2/LICENSE` & `registryspy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/PKG-INFO` & `registryspy-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: registryspy
-Version: 1.0.2
+Version: 1.1.0
 Summary: Cross-platform Windows Registry browser
 Home-page: https://github.com/andyjsmith/Registry-Spy
 Author: Andy Smith
-License: UNKNOWN
 Keywords: registry,forensics,windows forensics,forensics tools
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Environment :: MacOS X
 Requires-Python: >=3.8
@@ -25,23 +24,23 @@
 
 # Registry Spy: Cross-Platform Windows Registry Browser
 
 Registry Spy is a free, open-source cross-platform Windows Registry viewer. It is a fast, modern, and versatile explorer for raw registry files.
 
 Features include:
 
--   Fast, on-the-fly parsing means no upfront overhead
--   Open multiple hives at a time
--   Searching
--   Hex viewer
--   Modification timestamps
+- Fast, on-the-fly parsing means no upfront overhead
+- Open multiple hives at a time
+- Searching
+- Hex viewer
+- Modification timestamps
 
 ## Requirements
 
--   Python 3.8+
+- Python 3.8+
 
 ## Installation
 
 Download the latest version from the [releases page](https://github.com/andyjsmith/Registry-Spy/releases). Alternatively, use one of the following methods.
 
 ### pip (recommended)
 
@@ -69,34 +68,38 @@
 
 ![Find Dialog](https://github.com/andyjsmith/Registry-Spy/raw/master/screenshots/find.png)
 
 ## Building
 
 Dependencies:
 
--   PyInstaller 4.5+
+- PyInstaller 5.10+
+
+Delete any existing venv, dist, and build directories.
+
+Create and activate a new venv and install the requirements.txt and pyinstaller.
 
 Regular building:
 `pyinstaller registryspy_install.spec`
 
 Creating a single file: `pyinstaller registryspy_onefile.spec`
 
+Create the EXE installer with Inno Setup.
+
 ## License
 
 Registry Spy
 
-Copyright (C) 2021 Andy Smith
+Copyright (C) 2023 Andy Smith
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program. If not, see <https://www.gnu.org/licenses/>.
-
-
```

### Comparing `registryspy-1.0.2/README.md` & `registryspy-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 # Registry Spy: Cross-Platform Windows Registry Browser
 
 Registry Spy is a free, open-source cross-platform Windows Registry viewer. It is a fast, modern, and versatile explorer for raw registry files.
 
 Features include:
 
--   Fast, on-the-fly parsing means no upfront overhead
--   Open multiple hives at a time
--   Searching
--   Hex viewer
--   Modification timestamps
+- Fast, on-the-fly parsing means no upfront overhead
+- Open multiple hives at a time
+- Searching
+- Hex viewer
+- Modification timestamps
 
 ## Requirements
 
--   Python 3.8+
+- Python 3.8+
 
 ## Installation
 
 Download the latest version from the [releases page](https://github.com/andyjsmith/Registry-Spy/releases). Alternatively, use one of the following methods.
 
 ### pip (recommended)
 
@@ -46,26 +46,32 @@
 
 ![Find Dialog](https://github.com/andyjsmith/Registry-Spy/raw/master/screenshots/find.png)
 
 ## Building
 
 Dependencies:
 
--   PyInstaller 4.5+
+- PyInstaller 5.10+
+
+Delete any existing venv, dist, and build directories.
+
+Create and activate a new venv and install the requirements.txt and pyinstaller.
 
 Regular building:
 `pyinstaller registryspy_install.spec`
 
 Creating a single file: `pyinstaller registryspy_onefile.spec`
 
+Create the EXE installer with Inno Setup.
+
 ## License
 
 Registry Spy
 
-Copyright (C) 2021 Andy Smith
+Copyright (C) 2023 Andy Smith
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `registryspy-1.0.2/registryspy/find_dialog.py` & `registryspy-1.1.0/registryspy/find_dialog.py`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/helpers.py` & `registryspy-1.1.0/registryspy/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import sys
+import string
 
 import PySide6.QtWidgets as QtWidgets
 
 
 APP_NAME = "Registry Spy"
-VERSION = (1, 0, 2)
+VERSION = (1, 1, 0)
 ORGANIZATION_NAME = "Andy Smith"
-ORGANIZATION_DOMAIN = "ajsmith.us"
+ORGANIZATION_DOMAIN = "ajsmith.org"
 ABOUT_TEXT = f"""\
 {APP_NAME}
 {".".join(str(i) for i in VERSION)}
-Copyright (C) 2021 Andy Smith
+Copyright (C) 2023 Andy Smith
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -24,16 +25,27 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
+def bytes_to_printable(b: bytes, encoding="windows-1252") -> str:
+    """Convert bytes to string, replacing control and non-printable chars"""
+    decoded = b.decode(encoding, "replace")
+    # Replace the unicode replacement character
+    decoded = decoded.replace("\uFFFD", ".")
+    # Replace control characters
+    banned = "".join([chr(i) for i in range(0x20)] + ["\x7f", "\xa0", "\xad"])
+    decoded = "".join([c if c not in banned else "." for c in decoded])
+    return decoded
+
+
 def resource_path(relative_path: str) -> str:
-    """ Get absolute path to resource, works for dev and for PyInstaller """
+    """Get absolute path to resource, works for dev and for PyInstaller"""
     try:
         # PyInstaller creates a temp folder and stores path in _MEIPASS
         base_path = sys._MEIPASS
     except Exception:
         base_path = os.path.dirname(os.path.realpath(__file__))
 
     return os.path.join(base_path, relative_path)
```

### Comparing `registryspy-1.0.2/registryspy/hive_info_table.py` & `registryspy-1.1.0/registryspy/hive_info_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.resizeRowsToContents()
         self.setAutoScroll(False)
         self.setVerticalScrollMode(
             QtWidgets.QAbstractItemView.ScrollMode.ScrollPerPixel)
         self.setHorizontalScrollMode(
             QtWidgets.QAbstractItemView.ScrollMode.ScrollPerPixel)
         self.setWordWrap(False)
-        self.verticalHeader().setSectionResizeMode(self.verticalHeader().Fixed)
+        self.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.ResizeMode.Fixed)
 
         # Call so that the cells become uneditable
         self.set_info("", "", "", "")
 
     def set_info(self, hive_path, hive_type, hive_name, root_name):
         """Set the hive info table data"""
```

### Comparing `registryspy-1.0.2/registryspy/img/close.png` & `registryspy-1.1.0/registryspy/img/close.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/close_all.png` & `registryspy-1.1.0/registryspy/img/close_all.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/find.png` & `registryspy-1.1.0/registryspy/img/find.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/find_next.png` & `registryspy-1.1.0/registryspy/img/find_next.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/find_previous.png` & `registryspy-1.1.0/registryspy/img/find_previous.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/folder.png` & `registryspy-1.1.0/registryspy/img/folder.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/icon.ico` & `registryspy-1.1.0/registryspy/img/icon.ico`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/icon.png` & `registryspy-1.1.0/registryspy/img/icon.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/open.png` & `registryspy-1.1.0/registryspy/img/open.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/reg_bin.png` & `registryspy-1.1.0/registryspy/img/reg_bin.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/reg_num.png` & `registryspy-1.1.0/registryspy/img/reg_num.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/reg_str.png` & `registryspy-1.1.0/registryspy/img/reg_str.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/splash.png` & `registryspy-1.1.0/registryspy/img/splash.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/img/wordmark.png` & `registryspy-1.1.0/registryspy/img/wordmark.png`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/key_tree.py` & `registryspy-1.1.0/registryspy/key_tree.py`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/license_dialog.py` & `registryspy-1.1.0/registryspy/license_dialog.py`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/registryspy.py` & `registryspy-1.1.0/registryspy/registryspy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 
 import PySide6.QtGui as QtGui
 import PySide6.QtWidgets as QtWidgets
 import PySide6.QtCore as QtCore
 
+from . import data_viewer
 from . import value_table
 from . import key_tree
 from . import hive_info_table
 from . import license_dialog
 from . import find_dialog
 from . import helpers
 
@@ -163,24 +164,19 @@
         hive_geometry.setHeight(5)
         self.hive_info.setGeometry(hive_geometry)
         self.hive_info.setMinimumHeight(10)
         self.hive_info.setSizeAdjustPolicy(
             self.hive_info.SizeAdjustPolicy.AdjustToContents)
         tree_container_layout.addWidget(self.hive_info)
 
-        value_splitter = QtWidgets.QSplitter(
-            QtGui.Qt.Orientation.Vertical)
+        self.data_viewer = data_viewer.DataViewer()
+
+        value_splitter = QtWidgets.QSplitter(QtGui.Qt.Orientation.Vertical)
         value_splitter.addWidget(self.value_table)
-        self.value_hex = QtWidgets.QPlainTextEdit()
-        mono_font = QtGui.QFont()
-        mono_font.setFamilies(["Courier New", "Monospaced"])
-        mono_font.setStyleHint(QtGui.QFont.Monospace)
-        self.value_hex.setFont(mono_font)
-        self.value_hex.setLineWrapMode(self.value_hex.LineWrapMode.NoWrap)
-        value_splitter.addWidget(self.value_hex)
+        value_splitter.addWidget(self.data_viewer)
         value_splitter.setStretchFactor(0, 2)
         value_splitter.setStretchFactor(1, 1)
 
         main_splitter = QtWidgets.QSplitter(main_widget)
         main_splitter.addWidget(tree_container)
         main_splitter.addWidget(value_splitter)
         main_splitter.setStretchFactor(0, 4)
```

### Comparing `registryspy-1.0.2/registryspy/third_party_licenses.txt` & `registryspy-1.1.0/registryspy/third_party_licenses.txt`

 * *Files identical despite different names*

### Comparing `registryspy-1.0.2/registryspy/value_table.py` & `registryspy-1.1.0/registryspy/value_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,32 +55,20 @@
     def handle_selection_change(self, selected: QtCore.QItemSelection, deselected: QtCore.QItemSelection):
         if len(selected.indexes()) < 1:
             return
 
         index = selected.indexes()[2]
 
         value: ValueData = self.itemFromIndex(index)
-
-        hex_text = ""
-
-        def chunks(lst, n):
-            """Yield successive n-sized chunks from lst."""
-            for i in range(0, len(lst), n):
-                yield lst[i:i + n]
-
-        for chunk in chunks(value.raw_data, 16):
-            hex_text += " ".join(["{:02x}".format(x)
-                                  for x in chunk]) + "\n"
-
-        self.window().value_hex.setPlainText(hex_text)
+        self.window().data_viewer.set_value(value.raw_data)
 
     def set_data(self, reg_values: "list[Registry.RegistryValue]"):
         self.clearContents()
         self.setRowCount(0)
-        self.window().value_hex.setPlainText("")
+        self.window().data_viewer.set_value(b"")
 
         for value in reg_values:
             index = self.rowCount()
             self.insertRow(index)
             value_name = QtWidgets.QTableWidgetItem(value.name())
             value_name.setFlags(value_name.flags() & ~
                                 QtCore.Qt.ItemFlag.ItemIsEditable)
```

### Comparing `registryspy-1.0.2/registryspy.egg-info/PKG-INFO` & `registryspy-1.1.0/registryspy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: registryspy
-Version: 1.0.2
+Version: 1.1.0
 Summary: Cross-platform Windows Registry browser
 Home-page: https://github.com/andyjsmith/Registry-Spy
 Author: Andy Smith
-License: UNKNOWN
 Keywords: registry,forensics,windows forensics,forensics tools
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Environment :: MacOS X
 Requires-Python: >=3.8
@@ -25,23 +24,23 @@
 
 # Registry Spy: Cross-Platform Windows Registry Browser
 
 Registry Spy is a free, open-source cross-platform Windows Registry viewer. It is a fast, modern, and versatile explorer for raw registry files.
 
 Features include:
 
--   Fast, on-the-fly parsing means no upfront overhead
--   Open multiple hives at a time
--   Searching
--   Hex viewer
--   Modification timestamps
+- Fast, on-the-fly parsing means no upfront overhead
+- Open multiple hives at a time
+- Searching
+- Hex viewer
+- Modification timestamps
 
 ## Requirements
 
--   Python 3.8+
+- Python 3.8+
 
 ## Installation
 
 Download the latest version from the [releases page](https://github.com/andyjsmith/Registry-Spy/releases). Alternatively, use one of the following methods.
 
 ### pip (recommended)
 
@@ -69,34 +68,38 @@
 
 ![Find Dialog](https://github.com/andyjsmith/Registry-Spy/raw/master/screenshots/find.png)
 
 ## Building
 
 Dependencies:
 
--   PyInstaller 4.5+
+- PyInstaller 5.10+
+
+Delete any existing venv, dist, and build directories.
+
+Create and activate a new venv and install the requirements.txt and pyinstaller.
 
 Regular building:
 `pyinstaller registryspy_install.spec`
 
 Creating a single file: `pyinstaller registryspy_onefile.spec`
 
+Create the EXE installer with Inno Setup.
+
 ## License
 
 Registry Spy
 
-Copyright (C) 2021 Andy Smith
+Copyright (C) 2023 Andy Smith
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program. If not, see <https://www.gnu.org/licenses/>.
-
-
```

### Comparing `registryspy-1.0.2/registryspy.egg-info/SOURCES.txt` & `registryspy-1.1.0/registryspy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 run.py
 setup.py
 registryspy/__init__.py
+registryspy/data_viewer.py
 registryspy/find_dialog.py
 registryspy/helpers.py
 registryspy/hive_info_table.py
 registryspy/key_tree.py
 registryspy/license_dialog.py
 registryspy/registryspy.py
 registryspy/third_party_licenses.txt
```

### Comparing `registryspy-1.0.2/setup.py` & `registryspy-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="registryspy",
-    version="1.0.2",
+    version="1.1.0",
     author="Andy Smith",
     description="Cross-platform Windows Registry browser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andyjsmith/Registry-Spy",
-    keywords=[
-        "registry",
-        "forensics",
-        "windows forensics",
-        "forensics tools"
-    ],
+    keywords=["registry", "forensics", "windows forensics", "forensics tools"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Environment :: Win32 (MS Windows)",
         "Environment :: X11 Applications",
         "Environment :: X11 Applications :: Qt",
-        "Environment :: MacOS X"
+        "Environment :: MacOS X",
     ],
     packages=find_packages(),
     python_requires=">=3.8",
-    install_requires=[
-        "PySide6",
-        "python-registry"
-    ],
+    install_requires=["PySide6>=6.5", "python-registry>=1.3.1"],
     entry_points={
         "console_scripts": ["registryspy=registryspy.registryspy:main"],
     },
-    include_package_data=True
+    include_package_data=True,
 )
```

