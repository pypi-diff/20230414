# Comparing `tmp/random_utils-0.2.1.tar.gz` & `tmp/random_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/random_utils-0.2.1.tar", last modified: Tue Jan 26 22:58:29 2021, max compression
+gzip compressed data, was "random_utils-1.0.0.tar", last modified: Fri Apr 14 02:10:39 2023, max compression
```

## Comparing `random_utils-0.2.1.tar` & `random_utils-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2021-01-26 22:58:29.917378 random_utils-0.2.1/
--rw-rw-r--   0 arjun     (1000) arjun     (1000)      725 2021-01-26 22:58:29.917378 random_utils-0.2.1/PKG-INFO
--rw-rw-r--   0 arjun     (1000) arjun     (1000)      205 2021-01-23 00:17:46.000000 random_utils-0.2.1/README.md
-drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2021-01-26 22:58:29.913378 random_utils-0.2.1/random_utils/
--rw-rw-r--   0 arjun     (1000) arjun     (1000)      125 2021-01-24 02:22:01.000000 random_utils-0.2.1/random_utils/__init__.py
-drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2021-01-26 22:58:29.913378 random_utils-0.2.1/random_utils/colors/
--rw-rw-r--   0 arjun     (1000) arjun     (1000)       25 2021-01-21 05:33:05.000000 random_utils-0.2.1/random_utils/colors/__init__.py
--rw-rw-r--   0 arjun     (1000) arjun     (1000)     1067 2021-01-17 05:43:42.000000 random_utils-0.2.1/random_utils/colors/conversions.py
-drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2021-01-26 22:58:29.917378 random_utils-0.2.1/random_utils/datatypes/
--rw-rw-r--   0 arjun     (1000) arjun     (1000)       50 2021-01-26 22:58:17.000000 random_utils-0.2.1/random_utils/datatypes/__init__.py
--rw-rw-r--   0 arjun     (1000) arjun     (1000)     1881 2021-01-26 04:24:56.000000 random_utils-0.2.1/random_utils/datatypes/queue.py
--rw-rw-r--   0 arjun     (1000) arjun     (1000)     1772 2021-01-24 04:15:52.000000 random_utils-0.2.1/random_utils/datatypes/stack.py
-drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2021-01-26 22:58:29.917378 random_utils-0.2.1/random_utils/funcs/
--rw-rw-r--   0 arjun     (1000) arjun     (1000)      584 2021-01-23 00:40:23.000000 random_utils-0.2.1/random_utils/funcs/__init__.py
-drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2021-01-26 22:58:29.917378 random_utils-0.2.1/random_utils/math/
--rw-rw-r--   0 arjun     (1000) arjun     (1000)      632 2021-01-23 02:18:45.000000 random_utils-0.2.1/random_utils/math/__init__.py
--rw-rw-r--   0 arjun     (1000) arjun     (1000)     5086 2021-01-24 04:43:52.000000 random_utils-0.2.1/random_utils/math/vector.py
-drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2021-01-26 22:58:29.917378 random_utils-0.2.1/random_utils/pygame/
--rw-rw-r--   0 arjun     (1000) arjun     (1000)     4739 2021-01-16 22:36:05.000000 random_utils-0.2.1/random_utils/pygame/__init__.py
-drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2021-01-26 22:58:29.917378 random_utils-0.2.1/random_utils/time/
--rw-rw-r--   0 arjun     (1000) arjun     (1000)      258 2021-01-16 22:36:05.000000 random_utils-0.2.1/random_utils/time/__init__.py
-drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2021-01-26 22:58:29.913378 random_utils-0.2.1/random_utils.egg-info/
--rw-rw-r--   0 arjun     (1000) arjun     (1000)      725 2021-01-26 22:58:29.000000 random_utils-0.2.1/random_utils.egg-info/PKG-INFO
--rw-rw-r--   0 arjun     (1000) arjun     (1000)      539 2021-01-26 22:58:29.000000 random_utils-0.2.1/random_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 arjun     (1000) arjun     (1000)        1 2021-01-26 22:58:29.000000 random_utils-0.2.1/random_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 arjun     (1000) arjun     (1000)        6 2021-01-26 22:58:29.000000 random_utils-0.2.1/random_utils.egg-info/requires.txt
--rw-rw-r--   0 arjun     (1000) arjun     (1000)       13 2021-01-26 22:58:29.000000 random_utils-0.2.1/random_utils.egg-info/top_level.txt
--rw-rw-r--   0 arjun     (1000) arjun     (1000)       38 2021-01-26 22:58:29.917378 random_utils-0.2.1/setup.cfg
--rw-rw-r--   0 arjun     (1000) arjun     (1000)      751 2021-01-26 22:58:29.000000 random_utils-0.2.1/setup.py
+drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2023-04-14 02:10:39.809952 random_utils-1.0.0/
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)    35149 2021-01-16 22:36:05.000000 random_utils-1.0.0/LICENSE
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)      668 2023-04-14 02:10:39.809952 random_utils-1.0.0/PKG-INFO
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)      205 2021-01-23 00:17:46.000000 random_utils-1.0.0/README.md
+drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2023-04-14 02:10:39.805951 random_utils-1.0.0/random_utils/
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)      829 2021-02-24 18:02:45.000000 random_utils-1.0.0/random_utils/__init__.py
+drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2023-04-14 02:10:39.809952 random_utils-1.0.0/random_utils/colors/
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)      729 2021-02-24 18:02:06.000000 random_utils-1.0.0/random_utils/colors/__init__.py
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)     1770 2021-02-24 18:02:00.000000 random_utils-1.0.0/random_utils/colors/conversions.py
+drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2023-04-14 02:10:39.809952 random_utils-1.0.0/random_utils/datatypes/
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)      753 2021-02-24 18:02:15.000000 random_utils-1.0.0/random_utils/datatypes/__init__.py
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)     2738 2021-02-24 18:02:23.000000 random_utils-1.0.0/random_utils/datatypes/queue.py
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)     2629 2021-02-24 18:02:30.000000 random_utils-1.0.0/random_utils/datatypes/stack.py
+drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2023-04-14 02:10:39.809952 random_utils-1.0.0/random_utils/funcs/
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)     1287 2021-03-22 06:31:17.000000 random_utils-1.0.0/random_utils/funcs/__init__.py
+drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2023-04-14 02:10:39.809952 random_utils-1.0.0/random_utils/math/
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)     1335 2021-02-24 18:02:52.000000 random_utils-1.0.0/random_utils/math/__init__.py
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)     5789 2021-02-24 18:02:56.000000 random_utils-1.0.0/random_utils/math/vector.py
+drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2023-04-14 02:10:39.809952 random_utils-1.0.0/random_utils/pygame/
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)     5442 2021-02-24 18:03:05.000000 random_utils-1.0.0/random_utils/pygame/__init__.py
+drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2023-04-14 02:10:39.809952 random_utils-1.0.0/random_utils/time/
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)     1204 2021-03-22 06:43:17.000000 random_utils-1.0.0/random_utils/time/__init__.py
+drwxrwxr-x   0 arjun     (1000) arjun     (1000)        0 2023-04-14 02:10:39.805951 random_utils-1.0.0/random_utils.egg-info/
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)      668 2023-04-14 02:10:39.000000 random_utils-1.0.0/random_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)      547 2023-04-14 02:10:39.000000 random_utils-1.0.0/random_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)        1 2023-04-14 02:10:39.000000 random_utils-1.0.0/random_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)        6 2023-04-14 02:10:39.000000 random_utils-1.0.0/random_utils.egg-info/requires.txt
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)       13 2023-04-14 02:10:39.000000 random_utils-1.0.0/random_utils.egg-info/top_level.txt
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)       38 2023-04-14 02:10:39.809952 random_utils-1.0.0/setup.cfg
+-rw-rw-r--   0 arjun     (1000) arjun     (1000)     1454 2023-04-14 02:10:39.000000 random_utils-1.0.0/setup.py
```

### Comparing `random_utils-0.2.1/PKG-INFO` & `random_utils-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: random_utils
-Version: 0.2.1
+Version: 1.0.0
 Summary: Module with various useful utilities.
 Home-page: https://github.com/ArjunSahlot/random_utils
 Author: Arjun Sahlot
 Author-email: iarjun.sahlot@gmail.com
-License: UNKNOWN
-Description: # random_utils
-        
-        A [python module](https://pypi.org/project/random-utils/) with various useful utilities.
-        
-        ## Read about features on the [wiki](https://github.com/ArjunSahlot/random_utils/wiki/Feature-List)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# random_utils
+
+A [python module](https://pypi.org/project/random-utils/) with various useful utilities.
+
+## Read about features on the [wiki](https://github.com/ArjunSahlot/random_utils/wiki/Feature-List)
```

### Comparing `random_utils-0.2.1/random_utils/math/vector.py` & `random_utils-1.0.0/random_utils/math/vector.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+#
+#  Random utils
+#  
+#  Copyright Arjun Sahlot 2021
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#
+
 from math import atan, sin, cos, radians, degrees
 import numpy as np
 
 
 class Vector:
     """
     A vector class which has many useful vector methods.
```

### Comparing `random_utils-0.2.1/random_utils/pygame/__init__.py` & `random_utils-1.0.0/random_utils/pygame/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+#
+#  Random utils
+#  
+#  Copyright Arjun Sahlot 2021
+#
+#  This program is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  This program is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#
+
 import pygame
 from colorsys import rgb_to_hsv, hsv_to_rgb
 import numpy as np
 import os
 
 class ColorPicker:
     def __init__(self, wheel_pos, wheel_rad, slider_pos, slider_size, slider_horiz, slider_invert, cursor_rad, display_rect_loc, display_rect_size=(150, 150)):
```

### Comparing `random_utils-0.2.1/random_utils.egg-info/PKG-INFO` & `random_utils-1.0.0/random_utils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: random-utils
-Version: 0.2.1
+Version: 1.0.0
 Summary: Module with various useful utilities.
 Home-page: https://github.com/ArjunSahlot/random_utils
 Author: Arjun Sahlot
 Author-email: iarjun.sahlot@gmail.com
-License: UNKNOWN
-Description: # random_utils
-        
-        A [python module](https://pypi.org/project/random-utils/) with various useful utilities.
-        
-        ## Read about features on the [wiki](https://github.com/ArjunSahlot/random_utils/wiki/Feature-List)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# random_utils
+
+A [python module](https://pypi.org/project/random-utils/) with various useful utilities.
+
+## Read about features on the [wiki](https://github.com/ArjunSahlot/random_utils/wiki/Feature-List)
```

### Comparing `random_utils-0.2.1/random_utils.egg-info/SOURCES.txt` & `random_utils-1.0.0/random_utils.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 random_utils/__init__.py
 random_utils.egg-info/PKG-INFO
 random_utils.egg-info/SOURCES.txt
 random_utils.egg-info/dependency_links.txt
 random_utils.egg-info/requires.txt
```

