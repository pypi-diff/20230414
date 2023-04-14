# Comparing `tmp/lbutils-mp-0.2.1.tar.gz` & `tmp/lbutils-mp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbutils-mp-0.2.1.tar", last modified: Fri Apr 14 19:33:23 2023, max compression
+gzip compressed data, was "lbutils-mp-0.2.2.tar", last modified: Fri Apr 14 20:26:36 2023, max compression
```

## Comparing `lbutils-mp-0.2.1.tar` & `lbutils-mp-0.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/
--rw-rw-r--   0 david     (1000) david     (1000)     1064 2023-03-28 09:54:55.000000 lbutils-mp-0.2.1/LICENCE
--rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     5583 2023-04-13 07:19:57.000000 lbutils-mp-0.2.1/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.847021 lbutils-mp-0.2.1/lbutils/
--rw-rw-r--   0 david     (1000) david     (1000)     2911 2023-04-13 06:53:45.000000 lbutils-mp-0.2.1/lbutils/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1456 2023-04-13 06:56:17.000000 lbutils-mp-0.2.1/lbutils/abc.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.847021 lbutils-mp-0.2.1/lbutils/drivers/
--rw-rw-r--   0 david     (1000) david     (1000)     2256 2023-04-13 06:48:47.000000 lbutils-mp-0.2.1/lbutils/drivers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8527 2023-04-13 07:51:03.000000 lbutils-mp-0.2.1/lbutils/drivers/seven_segment.py
--rw-rw-r--   0 david     (1000) david     (1000)    12530 2023-04-13 07:50:12.000000 lbutils-mp-0.2.1/lbutils/drivers/seven_segment_hex.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.847021 lbutils-mp-0.2.1/lbutils/examples/
--rw-rw-r--   0 david     (1000) david     (1000)     2291 2023-04-13 06:59:17.000000 lbutils-mp-0.2.1/lbutils/examples/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.847021 lbutils-mp-0.2.1/lbutils/graphics/
--rw-rw-r--   0 david     (1000) david     (1000)     4632 2023-04-13 06:44:10.000000 lbutils-mp-0.2.1/lbutils/graphics/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    22594 2023-04-13 07:35:45.000000 lbutils-mp-0.2.1/lbutils/graphics/canvas.py
--rw-rw-r--   0 david     (1000) david     (1000)     9715 2023-04-12 21:37:18.000000 lbutils-mp-0.2.1/lbutils/graphics/colours.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils/graphics/fonts/
--rw-rw-r--   0 david     (1000) david     (1000)     2903 2023-04-12 21:25:04.000000 lbutils-mp-0.2.1/lbutils/graphics/fonts/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8797 2023-04-12 21:21:45.000000 lbutils-mp-0.2.1/lbutils/graphics/fonts/base_font.py
--rw-rw-r--   0 david     (1000) david     (1000)    10858 2023-04-12 17:06:52.000000 lbutils-mp-0.2.1/lbutils/graphics/fonts/font06.py
--rw-rw-r--   0 david     (1000) david     (1000)    13731 2023-04-12 17:06:52.000000 lbutils-mp-0.2.1/lbutils/graphics/fonts/font08.py
--rw-rw-r--   0 david     (1000) david     (1000)    12653 2023-04-13 21:29:43.000000 lbutils-mp-0.2.1/lbutils/graphics/fonts/org_01.py
--rw-rw-r--   0 david     (1000) david     (1000)    11461 2023-04-12 21:19:45.000000 lbutils-mp-0.2.1/lbutils/graphics/helpers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils/helpers/
--rw-rw-r--   0 david     (1000) david     (1000)     1614 2023-04-12 20:42:47.000000 lbutils-mp-0.2.1/lbutils/helpers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3859 2023-04-12 20:42:47.000000 lbutils-mp-0.2.1/lbutils/helpers/i2c.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils/pmods/
--rw-rw-r--   0 david     (1000) david     (1000)     1897 2023-04-12 20:46:12.000000 lbutils-mp-0.2.1/lbutils/pmods/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils/pmods/i2c/
--rw-rw-r--   0 david     (1000) david     (1000)     1617 2023-04-14 19:33:01.000000 lbutils-mp-0.2.1/lbutils/pmods/i2c/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils/pmods/spi/
--rw-rw-r--   0 david     (1000) david     (1000)     4133 2023-04-14 17:16:30.000000 lbutils-mp-0.2.1/lbutils/pmods/spi/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    23545 2023-04-12 21:34:43.000000 lbutils-mp-0.2.1/lbutils/pmods/spi/oledrgb.py
--rw-rw-r--   0 david     (1000) david     (1000)     3517 2023-04-12 20:37:20.000000 lbutils-mp-0.2.1/lbutils/typing.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils_mp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 19:33:23.000000 lbutils-mp-0.2.1/lbutils_mp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      796 2023-04-14 19:33:23.000000 lbutils-mp-0.2.1/lbutils_mp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-14 19:33:23.000000 lbutils-mp-0.2.1/lbutils_mp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-14 19:33:23.000000 lbutils-mp-0.2.1/lbutils_mp.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)     2136 2023-04-14 17:12:57.000000 lbutils-mp-0.2.1/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/
+-rw-rw-r--   0 david     (1000) david     (1000)     1064 2023-03-28 09:54:55.000000 lbutils-mp-0.2.2/LICENCE
+-rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     5583 2023-04-13 07:19:57.000000 lbutils-mp-0.2.2/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/
+-rw-rw-r--   0 david     (1000) david     (1000)     2911 2023-04-13 06:53:45.000000 lbutils-mp-0.2.2/lbutils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1456 2023-04-13 06:56:17.000000 lbutils-mp-0.2.2/lbutils/abc.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/drivers/
+-rw-rw-r--   0 david     (1000) david     (1000)     2256 2023-04-13 06:48:47.000000 lbutils-mp-0.2.2/lbutils/drivers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8527 2023-04-13 07:51:03.000000 lbutils-mp-0.2.2/lbutils/drivers/seven_segment.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12530 2023-04-13 07:50:12.000000 lbutils-mp-0.2.2/lbutils/drivers/seven_segment_hex.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/examples/
+-rw-rw-r--   0 david     (1000) david     (1000)     2291 2023-04-13 06:59:17.000000 lbutils-mp-0.2.2/lbutils/examples/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/graphics/
+-rw-rw-r--   0 david     (1000) david     (1000)     4632 2023-04-13 06:44:10.000000 lbutils-mp-0.2.2/lbutils/graphics/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22594 2023-04-14 20:24:00.000000 lbutils-mp-0.2.2/lbutils/graphics/canvas.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9715 2023-04-14 20:24:00.000000 lbutils-mp-0.2.2/lbutils/graphics/colours.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/graphics/fonts/
+-rw-rw-r--   0 david     (1000) david     (1000)     2903 2023-04-12 21:25:04.000000 lbutils-mp-0.2.2/lbutils/graphics/fonts/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8797 2023-04-12 21:21:45.000000 lbutils-mp-0.2.2/lbutils/graphics/fonts/base_font.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10858 2023-04-12 17:06:52.000000 lbutils-mp-0.2.2/lbutils/graphics/fonts/font06.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13731 2023-04-12 17:06:52.000000 lbutils-mp-0.2.2/lbutils/graphics/fonts/font08.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12653 2023-04-13 21:29:43.000000 lbutils-mp-0.2.2/lbutils/graphics/fonts/org_01.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12178 2023-04-14 20:24:00.000000 lbutils-mp-0.2.2/lbutils/graphics/helpers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.503870 lbutils-mp-0.2.2/lbutils/helpers/
+-rw-rw-r--   0 david     (1000) david     (1000)     1614 2023-04-12 20:42:47.000000 lbutils-mp-0.2.2/lbutils/helpers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3859 2023-04-12 20:42:47.000000 lbutils-mp-0.2.2/lbutils/helpers/i2c.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/lbutils/pmods/
+-rw-rw-r--   0 david     (1000) david     (1000)     1897 2023-04-12 20:46:12.000000 lbutils-mp-0.2.2/lbutils/pmods/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/lbutils/pmods/i2c/
+-rw-rw-r--   0 david     (1000) david     (1000)     1617 2023-04-14 19:33:01.000000 lbutils-mp-0.2.2/lbutils/pmods/i2c/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/lbutils/pmods/spi/
+-rw-rw-r--   0 david     (1000) david     (1000)     4133 2023-04-14 17:16:30.000000 lbutils-mp-0.2.2/lbutils/pmods/spi/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    23548 2023-04-14 20:24:55.000000 lbutils-mp-0.2.2/lbutils/pmods/spi/oledrgb.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3517 2023-04-12 20:37:20.000000 lbutils-mp-0.2.2/lbutils/typing.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/lbutils_mp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 20:26:36.000000 lbutils-mp-0.2.2/lbutils_mp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      796 2023-04-14 20:26:36.000000 lbutils-mp-0.2.2/lbutils_mp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-14 20:26:36.000000 lbutils-mp-0.2.2/lbutils_mp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-14 20:26:36.000000 lbutils-mp-0.2.2/lbutils_mp.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     2136 2023-04-14 20:23:41.000000 lbutils-mp-0.2.2/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-14 20:26:36.507870 lbutils-mp-0.2.2/setup.cfg
```

### Comparing `lbutils-mp-0.2.1/LICENCE` & `lbutils-mp-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/PKG-INFO` & `lbutils-mp-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbutils-mp
-Version: 0.2.1
+Version: 0.2.2
 Summary: Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers
 Author-email: David Love <david.love@leedsbeckett.ac.uk>
 Project-URL: Homepage, https://github.com/dlove24/lbutils
 Project-URL: Documentation, https://dlove24.github.io/lbutils/lbutils/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbutils-mp-0.2.1/README.md` & `lbutils-mp-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/__init__.py` & `lbutils-mp-0.2.2/lbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/abc.py` & `lbutils-mp-0.2.2/lbutils/abc.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/drivers/__init__.py` & `lbutils-mp-0.2.2/lbutils/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/drivers/seven_segment.py` & `lbutils-mp-0.2.2/lbutils/drivers/seven_segment.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/drivers/seven_segment_hex.py` & `lbutils-mp-0.2.2/lbutils/drivers/seven_segment_hex.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/examples/__init__.py` & `lbutils-mp-0.2.2/lbutils/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/graphics/__init__.py` & `lbutils-mp-0.2.2/lbutils/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/graphics/canvas.py` & `lbutils-mp-0.2.2/lbutils/graphics/canvas.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/graphics/colours.py` & `lbutils-mp-0.2.2/lbutils/graphics/colours.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/graphics/fonts/__init__.py` & `lbutils-mp-0.2.2/lbutils/graphics/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/graphics/fonts/base_font.py` & `lbutils-mp-0.2.2/lbutils/graphics/fonts/base_font.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/graphics/fonts/font06.py` & `lbutils-mp-0.2.2/lbutils/graphics/fonts/font06.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/graphics/fonts/font08.py` & `lbutils-mp-0.2.2/lbutils/graphics/fonts/font08.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/graphics/fonts/org_01.py` & `lbutils-mp-0.2.2/lbutils/graphics/fonts/org_01.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/graphics/helpers.py` & `lbutils-mp-0.2.2/lbutils/graphics/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,21 @@
 
 ## Tested Implementations
 
 *   Raspberry Pi Pico W (MicroPython 3.4)
 *   CPython (3.10)
 """
 
-from typing import Type
+# Import the typing hints if available. Use our backup version
+# if the offical library is missing
+try:
+    from typing import Type
+except ImportError:
+    from lbutils.typing import Type
+
 from .colours import Colour, COLOUR_WHITE, COLOUR_BLACK
 
 ###
 ### Classes
 ###
 
 
@@ -168,22 +174,32 @@
     Attributes
     ----------
 
     x: int
             The X co-oridinate value.
     y: int
             The Y co-ordinate value.
+    min_x: int
+            The minimum value allowed for the `x` co-ordinate. Defaults to
+            `0`.
+    min_y: int
+            The minimum value allowed for the `y` co-ordinate. Defaults to
+            `0`.`
+    max_x: int
+            The maximum value allowed for the `x` co-ordinate
+    max_y: int
+            The maximum value allowed for the `y` co-ordinate
     """
 
     def __init__(
         self,
         x: int,
         y: int,
         max_x: int,
-        max_y,
+        max_y: int,
         min_x: int = 0,
         min_y: int = 0,
         clip: bool = True,
     ):
         """Creates a `Pixel` instance holding the specified `x` and `y` co-
         ordinates, together representing the Cartesian point '(`x`, `y`)'. This
         `x` and `y` value is guaranteed to be maintained between `min_x` and
@@ -225,23 +241,27 @@
                 The parameter order is specified to allow easier definition
                 in the common case where the lower limits for `x` and `y` are
                 `0`, and the positional parameter order is being used. If all
                 four limits are being used, consider the use of named
                 parameters to avoid ambiguity.
         """
 
-        self.y = int(x)
-        self.x = int(y)
+        # Set-up the maximum and minimum parameters first
+        self.min_y = int(min_y)
+        self.max_y = int(max_y)
 
         self.min_x = int(min_x)
         self.max_x = int(max_x)
 
-        self.min_x = int(min_x)
-        self.max_x = int(max_x)
+        # Now attempt to set the actual `x` and `y` inside those
+        # parameters
+        self.y = int(y)
+        self.x = int(x)
 
+        # Set the clipping switch
         self.clip = clip
 
     ##
     ## Properties
     ##
 
     @property
```

### Comparing `lbutils-mp-0.2.1/lbutils/helpers/__init__.py` & `lbutils-mp-0.2.2/lbutils/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/helpers/i2c.py` & `lbutils-mp-0.2.2/lbutils/helpers/i2c.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/pmods/__init__.py` & `lbutils-mp-0.2.2/lbutils/pmods/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/pmods/i2c/__init__.py` & `lbutils-mp-0.2.2/lbutils/pmods/i2c/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/pmods/spi/__init__.py` & `lbutils-mp-0.2.2/lbutils/pmods/spi/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils/pmods/spi/oledrgb.py` & `lbutils-mp-0.2.2/lbutils/pmods/spi/oledrgb.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,17 +493,17 @@
 
         data = ustruct.pack(
             self._ENCODE_LINE,
             x1,
             y1,
             x2,
             y2,
-            fg_colour.r,
-            fg_colour.g,
-            fg_colour.b,
+            fg_colour.bR,
+            fg_colour.bG,
+            fg_colour.bB,
         )
         self._write(_DRAWLINE, data)
 
     def draw_rectangle(
         self,
         x: int,
         y: int,
```

### Comparing `lbutils-mp-0.2.1/lbutils/typing.py` & `lbutils-mp-0.2.2/lbutils/typing.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/lbutils_mp.egg-info/PKG-INFO` & `lbutils-mp-0.2.2/lbutils_mp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbutils-mp
-Version: 0.2.1
+Version: 0.2.2
 Summary: Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers
 Author-email: David Love <david.love@leedsbeckett.ac.uk>
 Project-URL: Homepage, https://github.com/dlove24/lbutils
 Project-URL: Documentation, https://dlove24.github.io/lbutils/lbutils/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbutils-mp-0.2.1/lbutils_mp.egg-info/SOURCES.txt` & `lbutils-mp-0.2.2/lbutils_mp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.1/pyproject.toml` & `lbutils-mp-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lbutils-mp"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="David Love", email="david.love@leedsbeckett.ac.uk" },
 ]
 description = "Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers"
 readme = "README.md"
 requires-python = ">=3.4"
 classifiers = [
```

