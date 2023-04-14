# Comparing `tmp/lbutils-mp-0.2.0.tar.gz` & `tmp/lbutils-mp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbutils-mp-0.2.0.tar", last modified: Fri Apr 14 16:39:47 2023, max compression
+gzip compressed data, was "lbutils-mp-0.2.1.tar", last modified: Fri Apr 14 19:33:23 2023, max compression
```

## Comparing `lbutils-mp-0.2.0.tar` & `lbutils-mp-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,42 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/
--rw-rw-r--   0 david     (1000) david     (1000)     1064 2023-03-28 09:54:55.000000 lbutils-mp-0.2.0/LICENCE
--rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     5583 2023-04-13 07:19:57.000000 lbutils-mp-0.2.0/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.690387 lbutils-mp-0.2.0/lbutils/
--rw-rw-r--   0 david     (1000) david     (1000)     2911 2023-04-13 06:53:45.000000 lbutils-mp-0.2.0/lbutils/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1456 2023-04-13 06:56:17.000000 lbutils-mp-0.2.0/lbutils/abc.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.690387 lbutils-mp-0.2.0/lbutils/drivers/
--rw-rw-r--   0 david     (1000) david     (1000)     2256 2023-04-13 06:48:47.000000 lbutils-mp-0.2.0/lbutils/drivers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8527 2023-04-13 07:51:03.000000 lbutils-mp-0.2.0/lbutils/drivers/seven_segment.py
--rw-rw-r--   0 david     (1000) david     (1000)    12530 2023-04-13 07:50:12.000000 lbutils-mp-0.2.0/lbutils/drivers/seven_segment_hex.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.690387 lbutils-mp-0.2.0/lbutils/examples/
--rw-rw-r--   0 david     (1000) david     (1000)     2291 2023-04-13 06:59:17.000000 lbutils-mp-0.2.0/lbutils/examples/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.690387 lbutils-mp-0.2.0/lbutils/graphics/
--rw-rw-r--   0 david     (1000) david     (1000)     4632 2023-04-13 06:44:10.000000 lbutils-mp-0.2.0/lbutils/graphics/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    22594 2023-04-13 07:35:45.000000 lbutils-mp-0.2.0/lbutils/graphics/canvas.py
--rw-rw-r--   0 david     (1000) david     (1000)     9715 2023-04-12 21:37:18.000000 lbutils-mp-0.2.0/lbutils/graphics/colours.py
--rw-rw-r--   0 david     (1000) david     (1000)    11461 2023-04-12 21:19:45.000000 lbutils-mp-0.2.0/lbutils/graphics/helpers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/lbutils/helpers/
--rw-rw-r--   0 david     (1000) david     (1000)     1614 2023-04-12 20:42:47.000000 lbutils-mp-0.2.0/lbutils/helpers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3859 2023-04-12 20:42:47.000000 lbutils-mp-0.2.0/lbutils/helpers/i2c.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/lbutils/pmods/
--rw-rw-r--   0 david     (1000) david     (1000)     1897 2023-04-12 20:46:12.000000 lbutils-mp-0.2.0/lbutils/pmods/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3517 2023-04-12 20:37:20.000000 lbutils-mp-0.2.0/lbutils/typing.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/lbutils_mp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 16:39:47.000000 lbutils-mp-0.2.0/lbutils_mp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      537 2023-04-14 16:39:47.000000 lbutils-mp-0.2.0/lbutils_mp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-14 16:39:47.000000 lbutils-mp-0.2.0/lbutils_mp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-14 16:39:47.000000 lbutils-mp-0.2.0/lbutils_mp.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)     2068 2023-04-14 16:39:28.000000 lbutils-mp-0.2.0/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/
+-rw-rw-r--   0 david     (1000) david     (1000)     1064 2023-03-28 09:54:55.000000 lbutils-mp-0.2.1/LICENCE
+-rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     5583 2023-04-13 07:19:57.000000 lbutils-mp-0.2.1/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.847021 lbutils-mp-0.2.1/lbutils/
+-rw-rw-r--   0 david     (1000) david     (1000)     2911 2023-04-13 06:53:45.000000 lbutils-mp-0.2.1/lbutils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1456 2023-04-13 06:56:17.000000 lbutils-mp-0.2.1/lbutils/abc.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.847021 lbutils-mp-0.2.1/lbutils/drivers/
+-rw-rw-r--   0 david     (1000) david     (1000)     2256 2023-04-13 06:48:47.000000 lbutils-mp-0.2.1/lbutils/drivers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8527 2023-04-13 07:51:03.000000 lbutils-mp-0.2.1/lbutils/drivers/seven_segment.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12530 2023-04-13 07:50:12.000000 lbutils-mp-0.2.1/lbutils/drivers/seven_segment_hex.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.847021 lbutils-mp-0.2.1/lbutils/examples/
+-rw-rw-r--   0 david     (1000) david     (1000)     2291 2023-04-13 06:59:17.000000 lbutils-mp-0.2.1/lbutils/examples/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.847021 lbutils-mp-0.2.1/lbutils/graphics/
+-rw-rw-r--   0 david     (1000) david     (1000)     4632 2023-04-13 06:44:10.000000 lbutils-mp-0.2.1/lbutils/graphics/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22594 2023-04-13 07:35:45.000000 lbutils-mp-0.2.1/lbutils/graphics/canvas.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9715 2023-04-12 21:37:18.000000 lbutils-mp-0.2.1/lbutils/graphics/colours.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils/graphics/fonts/
+-rw-rw-r--   0 david     (1000) david     (1000)     2903 2023-04-12 21:25:04.000000 lbutils-mp-0.2.1/lbutils/graphics/fonts/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8797 2023-04-12 21:21:45.000000 lbutils-mp-0.2.1/lbutils/graphics/fonts/base_font.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10858 2023-04-12 17:06:52.000000 lbutils-mp-0.2.1/lbutils/graphics/fonts/font06.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13731 2023-04-12 17:06:52.000000 lbutils-mp-0.2.1/lbutils/graphics/fonts/font08.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12653 2023-04-13 21:29:43.000000 lbutils-mp-0.2.1/lbutils/graphics/fonts/org_01.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11461 2023-04-12 21:19:45.000000 lbutils-mp-0.2.1/lbutils/graphics/helpers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils/helpers/
+-rw-rw-r--   0 david     (1000) david     (1000)     1614 2023-04-12 20:42:47.000000 lbutils-mp-0.2.1/lbutils/helpers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3859 2023-04-12 20:42:47.000000 lbutils-mp-0.2.1/lbutils/helpers/i2c.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils/pmods/
+-rw-rw-r--   0 david     (1000) david     (1000)     1897 2023-04-12 20:46:12.000000 lbutils-mp-0.2.1/lbutils/pmods/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils/pmods/i2c/
+-rw-rw-r--   0 david     (1000) david     (1000)     1617 2023-04-14 19:33:01.000000 lbutils-mp-0.2.1/lbutils/pmods/i2c/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils/pmods/spi/
+-rw-rw-r--   0 david     (1000) david     (1000)     4133 2023-04-14 17:16:30.000000 lbutils-mp-0.2.1/lbutils/pmods/spi/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    23545 2023-04-12 21:34:43.000000 lbutils-mp-0.2.1/lbutils/pmods/spi/oledrgb.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3517 2023-04-12 20:37:20.000000 lbutils-mp-0.2.1/lbutils/typing.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/lbutils_mp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 19:33:23.000000 lbutils-mp-0.2.1/lbutils_mp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      796 2023-04-14 19:33:23.000000 lbutils-mp-0.2.1/lbutils_mp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-14 19:33:23.000000 lbutils-mp-0.2.1/lbutils_mp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-14 19:33:23.000000 lbutils-mp-0.2.1/lbutils_mp.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     2136 2023-04-14 17:12:57.000000 lbutils-mp-0.2.1/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-14 19:33:23.851021 lbutils-mp-0.2.1/setup.cfg
```

### Comparing `lbutils-mp-0.2.0/LICENCE` & `lbutils-mp-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/PKG-INFO` & `lbutils-mp-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbutils-mp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers
 Author-email: David Love <david.love@leedsbeckett.ac.uk>
 Project-URL: Homepage, https://github.com/dlove24/lbutils
 Project-URL: Documentation, https://dlove24.github.io/lbutils/lbutils/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbutils-mp-0.2.0/README.md` & `lbutils-mp-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/__init__.py` & `lbutils-mp-0.2.1/lbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/abc.py` & `lbutils-mp-0.2.1/lbutils/abc.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/drivers/__init__.py` & `lbutils-mp-0.2.1/lbutils/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/drivers/seven_segment.py` & `lbutils-mp-0.2.1/lbutils/drivers/seven_segment.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/drivers/seven_segment_hex.py` & `lbutils-mp-0.2.1/lbutils/drivers/seven_segment_hex.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/examples/__init__.py` & `lbutils-mp-0.2.1/lbutils/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/graphics/__init__.py` & `lbutils-mp-0.2.1/lbutils/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/graphics/canvas.py` & `lbutils-mp-0.2.1/lbutils/graphics/canvas.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/graphics/colours.py` & `lbutils-mp-0.2.1/lbutils/graphics/colours.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/graphics/helpers.py` & `lbutils-mp-0.2.1/lbutils/graphics/helpers.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/helpers/__init__.py` & `lbutils-mp-0.2.1/lbutils/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/helpers/i2c.py` & `lbutils-mp-0.2.1/lbutils/helpers/i2c.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/pmods/__init__.py` & `lbutils-mp-0.2.1/lbutils/pmods/__init__.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils/typing.py` & `lbutils-mp-0.2.1/lbutils/typing.py`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.2.0/lbutils_mp.egg-info/PKG-INFO` & `lbutils-mp-0.2.1/lbutils_mp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbutils-mp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers
 Author-email: David Love <david.love@leedsbeckett.ac.uk>
 Project-URL: Homepage, https://github.com/dlove24/lbutils
 Project-URL: Documentation, https://dlove24.github.io/lbutils/lbutils/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbutils-mp-0.2.0/pyproject.toml` & `lbutils-mp-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lbutils-mp"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="David Love", email="david.love@leedsbeckett.ac.uk" },
 ]
 description = "Utility library for MicroPython, used at Leeds Beckett University and primarily aimed at the Pico H/W microcontrollers"
 readme = "README.md"
 requires-python = ">=3.4"
 classifiers = [
@@ -25,15 +25,15 @@
 recursive = true
 wrap-summaries = 80
 wrap-descriptions = 80
 syntax = "numpy"
 black = true
 
 [tool.setuptools]
-packages = ["lbutils", "lbutils.drivers", "lbutils.graphics", "lbutils.helpers", "lbutils.pmods"]
+packages = ["lbutils", "lbutils.drivers", "lbutils.graphics", "lbutils.graphics.fonts", "lbutils.helpers", "lbutils.pmods", "lbutils.pmods.spi", "lbutils.pmods.i2c"]
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
```

