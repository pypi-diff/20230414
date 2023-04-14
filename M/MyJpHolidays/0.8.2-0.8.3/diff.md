# Comparing `tmp/MyJpHolidays-0.8.2.tar.gz` & `tmp/MyJpHolidays-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyJpHolidays-0.8.2.tar", last modified: Fri Apr 14 02:37:24 2023, max compression
+gzip compressed data, was "MyJpHolidays-0.8.3.tar", last modified: Fri Apr 14 03:25:46 2023, max compression
```

## Comparing `MyJpHolidays-0.8.2.tar` & `MyJpHolidays-0.8.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 02:37:24.431373 MyJpHolidays-0.8.2/
--rw-rw-rw-   0        0        0     1089 2023-04-13 00:10:36.000000 MyJpHolidays-0.8.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-14 02:37:24.380370 MyJpHolidays-0.8.2/MyJpHolidays/
--rw-rw-rw-   0        0        0    58782 2023-04-13 07:32:54.000000 MyJpHolidays-0.8.2/MyJpHolidays/MyJpHolidays.py
--rw-rw-rw-   0        0        0       54 2023-04-14 02:35:50.000000 MyJpHolidays-0.8.2/MyJpHolidays/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 02:37:24.418372 MyJpHolidays-0.8.2/MyJpHolidays.egg-info/
--rw-rw-rw-   0        0        0     2160 2023-04-14 02:37:23.000000 MyJpHolidays-0.8.2/MyJpHolidays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-14 02:37:23.000000 MyJpHolidays-0.8.2/MyJpHolidays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 02:37:23.000000 MyJpHolidays-0.8.2/MyJpHolidays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-14 02:37:23.000000 MyJpHolidays-0.8.2/MyJpHolidays.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 02:37:23.000000 MyJpHolidays-0.8.2/MyJpHolidays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2160 2023-04-14 02:37:24.428372 MyJpHolidays-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     1358 2023-04-14 01:42:53.000000 MyJpHolidays-0.8.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 02:37:24.433373 MyJpHolidays-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-04-14 02:25:02.000000 MyJpHolidays-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:25:46.506821 MyJpHolidays-0.8.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-13 00:10:36.000000 MyJpHolidays-0.8.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-14 03:25:46.467819 MyJpHolidays-0.8.3/MyJpHolidays/
+-rw-rw-rw-   0        0        0    58782 2023-04-14 03:23:31.000000 MyJpHolidays-0.8.3/MyJpHolidays/MyJpHolidays.py
+-rw-rw-rw-   0        0        0       54 2023-04-14 03:23:18.000000 MyJpHolidays-0.8.3/MyJpHolidays/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:25:46.497821 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-04-14 03:25:45.000000 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-14 03:25:46.000000 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 03:25:45.000000 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 03:25:45.000000 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 03:25:45.000000 MyJpHolidays-0.8.3/MyJpHolidays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2085 2023-04-14 03:25:46.505821 MyJpHolidays-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1283 2023-04-14 03:21:53.000000 MyJpHolidays-0.8.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 03:25:46.509822 MyJpHolidays-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-04-14 02:25:02.000000 MyJpHolidays-0.8.3/setup.py
```

### Comparing `MyJpHolidays-0.8.2/LICENSE` & `MyJpHolidays-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MyJpHolidays-0.8.2/MyJpHolidays/MyJpHolidays.py` & `MyJpHolidays-0.8.3/MyJpHolidays/MyJpHolidays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# 更新日 2023.04.13
+# 更新日 2023.04.14
 #
-# MyJpHolidays	v0.8.1
+# MyJpHolidays	v0.8.3
 #
 
 import datetime
 import re
 import numpy as np
 import configparser
 import os
```

### Comparing `MyJpHolidays-0.8.2/MyJpHolidays.egg-info/PKG-INFO` & `MyJpHolidays-0.8.3/MyJpHolidays.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: MyJpHolidays
-Version: 0.8.2
+Version: 0.8.3
 Summary: MyJpHolidays: You get a combined list of Japan-Holidays. You can customize orignal holidays used ini-file.
 Home-page: https://github.com/Supper-Smille/MyJpHolidays20230412
 Author: Supper-Smille
 Author-email: ak2004@support.email.ne.jp
 Maintainer: Supper-Smille
 Maintainer-email: ak2004@support.email.ne.jp
 License: MIT License
@@ -32,13 +32,13 @@
         複合配列内の日付は、strです、datetimeではありません  
         アクセスの仕方はデモを参考にして下さい   
         
         ## インストール方法  
         pip install MyJpHolidays  
         
         ## デモプログラム<br>
-        [https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py](https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py)
+        https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py
          
             
         
 Platform: UNKNOWN
 Requires-Python: >=3.8.10
```

### Comparing `MyJpHolidays-0.8.2/PKG-INFO` & `MyJpHolidays-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: MyJpHolidays
-Version: 0.8.2
+Version: 0.8.3
 Summary: MyJpHolidays: You get a combined list of Japan-Holidays. You can customize orignal holidays used ini-file.
 Home-page: https://github.com/Supper-Smille/MyJpHolidays20230412
 Author: Supper-Smille
 Author-email: ak2004@support.email.ne.jp
 Maintainer: Supper-Smille
 Maintainer-email: ak2004@support.email.ne.jp
 License: MIT License
@@ -32,13 +32,13 @@
         複合配列内の日付は、strです、datetimeではありません  
         アクセスの仕方はデモを参考にして下さい   
         
         ## インストール方法  
         pip install MyJpHolidays  
         
         ## デモプログラム<br>
-        [https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py](https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py)
+        https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py
          
             
         
 Platform: UNKNOWN
 Requires-Python: >=3.8.10
```

### Comparing `MyJpHolidays-0.8.2/README.md` & `MyJpHolidays-0.8.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 複合配列内の日付は、strです、datetimeではありません  
 アクセスの仕方はデモを参考にして下さい   
 
 ## インストール方法  
 pip install MyJpHolidays  
 
 ## デモプログラム<br>
-[https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py](https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py)
+https://github.com/Supper-Smille/MyJpHolidays20230412/blob/main/demo.py
```

### Comparing `MyJpHolidays-0.8.2/setup.py` & `MyJpHolidays-0.8.3/setup.py`

 * *Files identical despite different names*

