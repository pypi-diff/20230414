# Comparing `tmp/MyJpHolidays-0.8.0.tar.gz` & `tmp/MyJpHolidays-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyJpHolidays-0.8.0.tar", last modified: Thu Apr 13 06:29:35 2023, max compression
+gzip compressed data, was "MyJpHolidays-0.8.1.tar", last modified: Thu Apr 13 07:35:52 2023, max compression
```

## Comparing `MyJpHolidays-0.8.0.tar` & `MyJpHolidays-0.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:29:35.318431 MyJpHolidays-0.8.0/
--rw-rw-rw-   0        0        0     1089 2023-04-13 00:10:36.000000 MyJpHolidays-0.8.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-13 06:29:35.216425 MyJpHolidays-0.8.0/MyJpHolidays/
--rw-rw-rw-   0        0        0    58754 2023-04-11 00:57:08.000000 MyJpHolidays-0.8.0/MyJpHolidays/MyJpHolidays.py
--rw-rw-rw-   0        0        0       54 2023-04-12 07:41:08.000000 MyJpHolidays-0.8.0/MyJpHolidays/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:29:35.297430 MyJpHolidays-0.8.0/MyJpHolidays.egg-info/
--rw-rw-rw-   0        0        0      539 2023-04-13 06:29:34.000000 MyJpHolidays-0.8.0/MyJpHolidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-13 06:29:34.000000 MyJpHolidays-0.8.0/MyJpHolidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:29:34.000000 MyJpHolidays-0.8.0/MyJpHolidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-13 06:29:34.000000 MyJpHolidays-0.8.0/MyJpHolidays.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 06:29:34.000000 MyJpHolidays-0.8.0/MyJpHolidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      539 2023-04-13 06:29:35.314431 MyJpHolidays-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-04-13 00:06:27.000000 MyJpHolidays-0.8.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 06:29:35.320431 MyJpHolidays-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1272 2023-04-12 07:53:26.000000 MyJpHolidays-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:35:52.086045 MyJpHolidays-0.8.1/
+-rw-rw-rw-   0        0        0     1089 2023-04-13 00:10:36.000000 MyJpHolidays-0.8.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-13 07:35:52.045042 MyJpHolidays-0.8.1/MyJpHolidays/
+-rw-rw-rw-   0        0        0    58782 2023-04-13 07:32:54.000000 MyJpHolidays-0.8.1/MyJpHolidays/MyJpHolidays.py
+-rw-rw-rw-   0        0        0       54 2023-04-13 07:29:16.000000 MyJpHolidays-0.8.1/MyJpHolidays/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:35:52.078044 MyJpHolidays-0.8.1/MyJpHolidays.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-04-13 07:35:51.000000 MyJpHolidays-0.8.1/MyJpHolidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-13 07:35:51.000000 MyJpHolidays-0.8.1/MyJpHolidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 07:35:51.000000 MyJpHolidays-0.8.1/MyJpHolidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 07:35:51.000000 MyJpHolidays-0.8.1/MyJpHolidays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 07:35:51.000000 MyJpHolidays-0.8.1/MyJpHolidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      539 2023-04-13 07:35:52.082044 MyJpHolidays-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2023-04-13 00:06:27.000000 MyJpHolidays-0.8.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 07:35:52.087045 MyJpHolidays-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2023-04-13 07:30:00.000000 MyJpHolidays-0.8.1/setup.py
```

### Comparing `MyJpHolidays-0.8.0/LICENSE` & `MyJpHolidays-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MyJpHolidays-0.8.0/MyJpHolidays/MyJpHolidays.py` & `MyJpHolidays-0.8.1/MyJpHolidays/MyJpHolidays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-# 更新日 2023.04.08
+# 更新日 2023.04.13
 #
+# MyJpHolidays	v0.8.1
+#
+
 import datetime
 import re
 import numpy as np
 import configparser
 import os
 
 gOneDay : object
```

### Comparing `MyJpHolidays-0.8.0/MyJpHolidays.egg-info/PKG-INFO` & `MyJpHolidays-0.8.1/MyJpHolidays.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: MyJpHolidays
-Version: 0.8.0
+Version: 0.8.1
 Summary: MyJpHolidays: You get a combined list of Japan-Holidays. You can customize orignal holidays used ini-file.
 Home-page: https://github.com/Supper-Smille/MyJpHolidays20230412
 Author: Supper-Smille
 Author-email: ak2004@support.email.ne.jp
 Maintainer: Supper-Smille
 Maintainer-email: ak2004@support.email.ne.jp
 License: MIT License
```

### Comparing `MyJpHolidays-0.8.0/PKG-INFO` & `MyJpHolidays-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: MyJpHolidays
-Version: 0.8.0
+Version: 0.8.1
 Summary: MyJpHolidays: You get a combined list of Japan-Holidays. You can customize orignal holidays used ini-file.
 Home-page: https://github.com/Supper-Smille/MyJpHolidays20230412
 Author: Supper-Smille
 Author-email: ak2004@support.email.ne.jp
 Maintainer: Supper-Smille
 Maintainer-email: ak2004@support.email.ne.jp
 License: MIT License
```

### Comparing `MyJpHolidays-0.8.0/README.md` & `MyJpHolidays-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `MyJpHolidays-0.8.0/setup.py` & `MyJpHolidays-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 LICENSE = 'MIT License'
 DOWNLOAD_URL = 'https://github.com/Supper-Smille/MyJpHolidays20230412'
 VERSION = MyJpHolidays.__version__
 PYTHON_REQUIRES = ">=3.8.10"
 
 
 INSTALL_REQUIRES = [
-    'numpy >=1.23.1', 
-    're>=2.2.1'
+    'numpy >=1.23.1'
 ]
 
 
 PACKAGES = [
     'MyJpHolidays'
 ]
```

