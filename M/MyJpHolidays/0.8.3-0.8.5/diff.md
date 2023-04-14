# Comparing `tmp/MyJpHolidays-0.8.3.tar.gz` & `tmp/MyJpHolidays-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyJpHolidays-0.8.3.tar", last modified: Fri Apr 14 03:25:46 2023, max compression
+gzip compressed data, was "MyJpHolidays-0.8.5.tar", last modified: Fri Apr 14 07:55:28 2023, max compression
```

## Comparing `MyJpHolidays-0.8.3.tar` & `MyJpHolidays-0.8.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 03:25:46.506821 MyJpHolidays-0.8.3/
--rw-rw-rw-   0        0        0     1089 2023-04-13 00:10:36.000000 MyJpHolidays-0.8.3/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-14 03:25:46.467819 MyJpHolidays-0.8.3/MyJpHolidays/
--rw-rw-rw-   0        0        0    58782 2023-04-14 03:23:31.000000 MyJpHolidays-0.8.3/MyJpHolidays/MyJpHolidays.py
--rw-rw-rw-   0        0        0       54 2023-04-14 03:23:18.000000 MyJpHolidays-0.8.3/MyJpHolidays/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 03:25:46.497821 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-04-14 03:25:45.000000 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-14 03:25:46.000000 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 03:25:45.000000 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-14 03:25:45.000000 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 03:25:45.000000 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2085 2023-04-14 03:25:46.505821 MyJpHolidays-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     1283 2023-04-14 03:21:53.000000 MyJpHolidays-0.8.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 03:25:46.509822 MyJpHolidays-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-04-14 02:25:02.000000 MyJpHolidays-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:55:28.475981 MyJpHolidays-0.8.5/
+-rw-rw-rw-   0        0        0     1089 2023-04-13 00:10:36.000000 MyJpHolidays-0.8.5/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-14 07:55:28.428978 MyJpHolidays-0.8.5/MyJpHolidays/
+-rw-rw-rw-   0        0        0    58782 2023-04-14 07:54:02.000000 MyJpHolidays-0.8.5/MyJpHolidays/MyJpHolidays.py
+-rw-rw-rw-   0        0        0       54 2023-04-14 07:53:52.000000 MyJpHolidays-0.8.5/MyJpHolidays/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:55:28.463980 MyJpHolidays-0.8.5/MyJpHolidays.egg-info/
+-rw-rw-rw-   0        0        0     2661 2023-04-14 07:55:28.000000 MyJpHolidays-0.8.5/MyJpHolidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-14 07:55:28.000000 MyJpHolidays-0.8.5/MyJpHolidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 07:55:28.000000 MyJpHolidays-0.8.5/MyJpHolidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 07:55:28.000000 MyJpHolidays-0.8.5/MyJpHolidays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 07:55:28.000000 MyJpHolidays-0.8.5/MyJpHolidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2661 2023-04-14 07:55:28.473981 MyJpHolidays-0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1283 2023-04-14 03:21:53.000000 MyJpHolidays-0.8.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 07:55:28.477981 MyJpHolidays-0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     2092 2023-04-14 07:53:26.000000 MyJpHolidays-0.8.5/setup.py
```

### Comparing `MyJpHolidays-0.8.3/LICENSE` & `MyJpHolidays-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MyJpHolidays-0.8.3/MyJpHolidays/MyJpHolidays.py` & `MyJpHolidays-0.8.5/MyJpHolidays/MyJpHolidays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 更新日 2023.04.14
 #
-# MyJpHolidays	v0.8.3
+# MyJpHolidays	v0.8.5
 #
 
 import datetime
 import re
 import numpy as np
 import configparser
 import os
```

### Comparing `MyJpHolidays-0.8.3/MyJpHolidays.egg-info/PKG-INFO` & `MyJpHolidays-0.8.5/MyJpHolidays.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: MyJpHolidays
-Version: 0.8.3
+Version: 0.8.5
 Summary: MyJpHolidays: You get a combined list of Japan-Holidays. You can customize orignal holidays used ini-file.
 Home-page: https://github.com/Supper-Smille/MyJpHolidays20230412
 Author: Supper-Smille
 Author-email: ak2004@support.email.ne.jp
 Maintainer: Supper-Smille
 Maintainer-email: ak2004@support.email.ne.jp
 License: MIT License
@@ -37,8 +37,20 @@
         
         ## デモプログラム<br>
         https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py
          
             
         
 Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Classifier: Topic :: Office/Business
+Classifier: Topic :: Office/Business :: Scheduling
+Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8.10
```

### Comparing `MyJpHolidays-0.8.3/PKG-INFO` & `MyJpHolidays-0.8.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: MyJpHolidays
-Version: 0.8.3
+Version: 0.8.5
 Summary: MyJpHolidays: You get a combined list of Japan-Holidays. You can customize orignal holidays used ini-file.
 Home-page: https://github.com/Supper-Smille/MyJpHolidays20230412
 Author: Supper-Smille
 Author-email: ak2004@support.email.ne.jp
 Maintainer: Supper-Smille
 Maintainer-email: ak2004@support.email.ne.jp
 License: MIT License
@@ -37,8 +37,20 @@
         
         ## デモプログラム<br>
         https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py
          
             
         
 Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Classifier: Topic :: Office/Business
+Classifier: Topic :: Office/Business :: Scheduling
+Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8.10
```

### Comparing `MyJpHolidays-0.8.3/README.md` & `MyJpHolidays-0.8.5/README.md`

 * *Files identical despite different names*

