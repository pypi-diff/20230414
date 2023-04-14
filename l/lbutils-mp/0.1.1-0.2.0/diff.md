# Comparing `tmp/lbutils-mp-0.1.1.tar.gz` & `tmp/lbutils-mp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbutils-mp-0.1.1.tar", last modified: Wed Mar 29 08:53:43 2023, max compression
+gzip compressed data, was "lbutils-mp-0.2.0.tar", last modified: Fri Apr 14 16:39:47 2023, max compression
```

## Comparing `lbutils-mp-0.1.1.tar` & `lbutils-mp-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 08:53:43.664108 lbutils-mp-0.1.1/
--rw-rw-r--   0 david     (1000) david     (1000)     1064 2023-03-28 09:54:55.000000 lbutils-mp-0.1.1/LICENCE
--rw-rw-r--   0 david     (1000) david     (1000)     2976 2023-03-29 08:53:43.664108 lbutils-mp-0.1.1/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     2366 2023-03-28 10:16:28.000000 lbutils-mp-0.1.1/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 08:53:43.660108 lbutils-mp-0.1.1/lbutils/
--rw-rw-r--   0 david     (1000) david     (1000)     3596 2023-03-29 08:52:07.000000 lbutils-mp-0.1.1/lbutils/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 08:53:43.660108 lbutils-mp-0.1.1/lbutils/drivers/
--rw-rw-r--   0 david     (1000) david     (1000)     2116 2023-03-28 17:02:07.000000 lbutils-mp-0.1.1/lbutils/drivers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8167 2023-03-29 08:45:26.000000 lbutils-mp-0.1.1/lbutils/drivers/seven_segment.py
--rw-rw-r--   0 david     (1000) david     (1000)    12139 2023-03-29 08:48:53.000000 lbutils-mp-0.1.1/lbutils/drivers/seven_segment_hex.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 08:53:43.664108 lbutils-mp-0.1.1/lbutils/examples/
--rw-rw-r--   0 david     (1000) david     (1000)     2280 2023-03-29 08:27:43.000000 lbutils-mp-0.1.1/lbutils/examples/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3034 2023-03-28 16:31:27.000000 lbutils-mp-0.1.1/lbutils/examples/seven_segment_example.py
--rw-rw-r--   0 david     (1000) david     (1000)     3046 2023-03-29 08:32:44.000000 lbutils-mp-0.1.1/lbutils/examples/seven_segment_hex_example.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 08:53:43.664108 lbutils-mp-0.1.1/lbutils/helpers/
--rw-rw-r--   0 david     (1000) david     (1000)     1568 2023-03-28 10:26:38.000000 lbutils-mp-0.1.1/lbutils/helpers/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 08:53:43.664108 lbutils-mp-0.1.1/lbutils/pmod/
--rw-rw-r--   0 david     (1000) david     (1000)     1894 2023-03-28 10:30:36.000000 lbutils-mp-0.1.1/lbutils/pmod/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-29 08:53:43.664108 lbutils-mp-0.1.1/lbutils_mp.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     2976 2023-03-29 08:53:43.000000 lbutils-mp-0.1.1/lbutils_mp.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      456 2023-03-29 08:53:43.000000 lbutils-mp-0.1.1/lbutils_mp.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-03-29 08:53:43.000000 lbutils-mp-0.1.1/lbutils_mp.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-03-29 08:53:43.000000 lbutils-mp-0.1.1/lbutils_mp.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      800 2023-03-28 10:45:23.000000 lbutils-mp-0.1.1/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-03-29 08:53:43.664108 lbutils-mp-0.1.1/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/
+-rw-rw-r--   0 david     (1000) david     (1000)     1064 2023-03-28 09:54:55.000000 lbutils-mp-0.2.0/LICENCE
+-rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     5583 2023-04-13 07:19:57.000000 lbutils-mp-0.2.0/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.690387 lbutils-mp-0.2.0/lbutils/
+-rw-rw-r--   0 david     (1000) david     (1000)     2911 2023-04-13 06:53:45.000000 lbutils-mp-0.2.0/lbutils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1456 2023-04-13 06:56:17.000000 lbutils-mp-0.2.0/lbutils/abc.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.690387 lbutils-mp-0.2.0/lbutils/drivers/
+-rw-rw-r--   0 david     (1000) david     (1000)     2256 2023-04-13 06:48:47.000000 lbutils-mp-0.2.0/lbutils/drivers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8527 2023-04-13 07:51:03.000000 lbutils-mp-0.2.0/lbutils/drivers/seven_segment.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12530 2023-04-13 07:50:12.000000 lbutils-mp-0.2.0/lbutils/drivers/seven_segment_hex.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.690387 lbutils-mp-0.2.0/lbutils/examples/
+-rw-rw-r--   0 david     (1000) david     (1000)     2291 2023-04-13 06:59:17.000000 lbutils-mp-0.2.0/lbutils/examples/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.690387 lbutils-mp-0.2.0/lbutils/graphics/
+-rw-rw-r--   0 david     (1000) david     (1000)     4632 2023-04-13 06:44:10.000000 lbutils-mp-0.2.0/lbutils/graphics/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22594 2023-04-13 07:35:45.000000 lbutils-mp-0.2.0/lbutils/graphics/canvas.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9715 2023-04-12 21:37:18.000000 lbutils-mp-0.2.0/lbutils/graphics/colours.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11461 2023-04-12 21:19:45.000000 lbutils-mp-0.2.0/lbutils/graphics/helpers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/lbutils/helpers/
+-rw-rw-r--   0 david     (1000) david     (1000)     1614 2023-04-12 20:42:47.000000 lbutils-mp-0.2.0/lbutils/helpers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3859 2023-04-12 20:42:47.000000 lbutils-mp-0.2.0/lbutils/helpers/i2c.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/lbutils/pmods/
+-rw-rw-r--   0 david     (1000) david     (1000)     1897 2023-04-12 20:46:12.000000 lbutils-mp-0.2.0/lbutils/pmods/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3517 2023-04-12 20:37:20.000000 lbutils-mp-0.2.0/lbutils/typing.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/lbutils_mp.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     6193 2023-04-14 16:39:47.000000 lbutils-mp-0.2.0/lbutils_mp.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      537 2023-04-14 16:39:47.000000 lbutils-mp-0.2.0/lbutils_mp.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-04-14 16:39:47.000000 lbutils-mp-0.2.0/lbutils_mp.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2023-04-14 16:39:47.000000 lbutils-mp-0.2.0/lbutils_mp.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     2068 2023-04-14 16:39:28.000000 lbutils-mp-0.2.0/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-04-14 16:39:47.694387 lbutils-mp-0.2.0/setup.cfg
```

### Comparing `lbutils-mp-0.1.1/LICENCE` & `lbutils-mp-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `lbutils-mp-0.1.1/lbutils/drivers/__init__.py` & `lbutils-mp-0.2.0/lbutils/drivers/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-"""
-Drivers for low-level components, including those using the SPI or I2C busses
-
-Overview
---------
-
-This is mostly a collection of drivers, some third-party, which provide low-level access to devices. In most cases additional code will be required to _use_ these devices: the focus of the code in here is only on providing _access_ to those devices.
-
-Examples for how to use the library can be found in the '`examples`' folder: or [in the documentation](https://dlove24.github.io/urest/lbutils/examples/index.html).
-
-**NOTE:** The Digilent '`pmod`' devices are split into their own special section, and should be imported using the '`pmod`' libraries.
+# This module, and all included code, is made available under the terms of the
+# MIT Licence
+#
+# Copyright (c) 2023 David Love
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+"""Drivers for low-level components, including those using the SPI or I2C
+busses. This is mostly a collection of drivers, some third-party, which provide
+low-level access to devices. In most cases additional code will be required to
+_use_ these devices: the focus of the code in here is only on providing _access_
+to those devices.
+
+Examples for how to use the library can be found in the '`examples`' folder: or in
+the documentation for specific classes. In some cases the examples will require a
+specific example circuit: where this is the case, in most cases classes will
+additionally provide an example on [WokWi](https://wokwi.com).
+
+!!! Note
+    The Digilent '`pmod`' devices are split into their own special section, and
+    should be imported using the '`pmod`' libraries.
 
 Tested Implementations
 ----------------------
 
 This version is written for MicroPython 3.4, and has been tested on:
 
   * Raspberry Pi Pico H/W
-
-Licence
--------
-
-This module, and all included code, is made available under the terms of the MIT Licence
-
-> Copyright (c) 2023 David Love
-
-> Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-> The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 ### Expose the `drivers` module interface as a full package
 from .seven_segment import SegDisplay
 from .seven_segment_hex import SegHexDisplay
```

### Comparing `lbutils-mp-0.1.1/lbutils/drivers/seven_segment.py` & `lbutils-mp-0.2.0/lbutils/drivers/seven_segment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,200 +1,207 @@
-"""
-Simple (decimal) numeric driver for a seven-segment display, requiring seven GPIO pins.
+# This module, and all included code, is made available under the terms of
+# the MIT Licence
+#
+# Copyright (c) 2023 Roz Wyatt-Millington, David Love
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+"""Simple (decimal) numeric driver for a seven-segment display, requiring seven
+GPIO pins.
 
 Overview
 --------
 
 During initialisation the user must supply a list of exactly seven GPIO pins,
 using the numeric pin identifier (e.g. 16 for GPIO Pin 16). Each entry in the
 list corresponds to the segment 'a' (for the first entry) to 'g' (for the last
 entry). Physically, each LED segment is also assumed to be laid out in the
 standard pattern, shown below. Once the constructor has been called, no further
 changes are possible: and the driver will also assume exclusive use of the
 relevant GPIO pins.
 
+````
      - A -
    |       |
    F       B
    | - G - |
    E       C
    |       |
      - D -
+````
 
 **Figure 1: Assumed Layout of the Seven Segment Display**
 
 To display a character, the `display` method of the class is used: passing in an
 integer in the range 0..9 representing the number to show on the seven segment.
 Not that by default the `display` method assumes that GPIO pins must be held
-_low_ for the segment to display: i.e. the behaviour normally used by common
+*low* for the segment to display: i.e. the behaviour normally used by common
 anode seven-segment displays. If you need the requested GPIO pin to be held
-_high_ to display a segment, pass in `True` to the `inverted` parameter of the
+*high* to display a segment, pass in `True` to the `inverted` parameter of the
 `display` method.
 
-.. Note: This driver will only display characters in the range '0' to 'F', and
-will raise a `ValueError` exception if the requested character is not in an
-appropriate range.
+!!! Note
+    This driver will only display characters in the range '0' to '9', and
+    will raise a `ValueError` exception if the requested character is not in an
+    appropriate range.
 
 Examples
 --------
 
-* Examples Folder: `seven_segment_example.py`
+* Examples Folder: `examples/drivers/seven_segment_example.py`
 * [WokWi](https://wokwi.com/projects/360451068863047681)
 
 Tested Implementations
 ----------------------
 
 This version is written for MicroPython 3.4, and has been tested on:
 
 * Raspberry Pi Pico H/W
-
-Licence
--------
-
-This module, and all included code, is made available under the terms of the MIT Licence
-
-> Copyright (c) 2023 Roz Wyatt-Millington, David Love
-
-> Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-> The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 # Import MicroPython libraries for GPIO access if available
 try:
-    from machine import ADC
     from machine import Pin
 except ImportError:
     print("Ignoring MicroPython includes")
 
 ##
 ## Classes
 ##
 
 
 class SegDisplay:
-    char_list = [
+    """Simple (decimal) numeric driver for a seven-segment display, requiring
+    seven GPIO pins.
+
+    **Note:** This driver will only display characters in the range '0' to '9',
+    and will raise a `ValueError` exception if the requested character is not in
+    an appropriate range.
+    """
+
+    _char_list = [
         [False, False, False, False, False, False, True],
         [True, False, False, True, True, True, True],
         [False, False, True, False, False, True, False],
         [False, False, False, False, True, True, False],
         [True, False, False, True, True, False, False],
         [False, True, False, False, True, False, False],
         [False, True, False, False, False, False, False],
         [False, False, False, True, True, True, True],
         [False, False, False, False, False, False, False],
         [False, False, False, True, True, False, False],
     ]
-    """
-    Defines how characters are rendered, from zero ('0') in the first entry to
-    nine ('9') as the last entry. Note that pins which are listed here as
-    `False` will be _on_ using the default options to the `display` method.
+    """Defines how characters are rendered, from zero ('0') in the first entry
+    to nine ('9') as the last entry.
+
+    Note that pins which are listed here as `False` will be *on* using the
+    default options to the `display` method.
     """
 
-    def __init__(self, gpio_request: list):
-        """
-        Initialise a seven-segment display, using the user supplied
-        list of GPIO pins in `gpio_request` as reference for pins to
-        drive.
+    def __init__(self, gpio_request: list) -> None:
+        """Initialise a seven-segment display, using the user supplied list of
+        GPIO pins in `gpio_request` as reference for pins to drive.
 
         This class also assume a common anode seven-segment display by default,
-        and so will assume that pulling a GPIO pin _low_ will turn the relevant
-        segment _on_. If you need to modify this behaviour, see the `inverted`
+        and so will assume that pulling a GPIO pin *low* will turn the relevant
+        segment *on*. If you need to modify this behaviour, see the `inverted`
         parameter for the `display` method.
 
-        .. Note::
-            This list of entries in the `gpio_request` _must_ be exactly seven
-            entries long, or the class will throw a `ValueError` in the
+        !!! Note
+            This list of entries in the `gpio_request` *must* be **exactly**
+            seven entries long, or the class will throw a `ValueError` in the
             constructor.
 
         Parameters
         ----------
 
         gpio_request: list
             The pin-ordered list of GPIO pins to use for the segment positions
             'a' (as the first entry in the list) to 'g' (as the last entry in
             the list).
 
-            **NOTE**: The `SegDisplay` class will also attempt to create the
+            **Note**: The `SegDisplay` class will also attempt to create the
             underlying GPIO object for each of the entries in the list. If
             the GPIO pins need to be initialised first, this must be done
-            _before_ calling this constructor.
+            *before* calling this constructor.
 
         Raises
         ------
 
-        * `ValueError` if the `gpio_request` is empty, or does not have exactly
-          seven elements in the list.
+        ValueError
+            The `gpio_request` is empty, or does not have exactly
+            seven elements in the list.
         """
         self.pin_list = []
 
         if (gpio_request is None) or (not gpio_request):
             raise ValueError("The GPIO Request List is empty")
         elif len(gpio_request) != 7:
             raise ValueError("The GPIO Request List must be EXACTLY seven entries long")
         else:
             for segment in range(7):
                 self.pin_list.append(Pin(gpio_request[segment], Pin.OUT))
 
-    def display(self, character: int, inverted: bool = False):
-        """
-        Display the given `character` on the seven-segment display,
-        using the `char_list` as a guide for which pins to turn on or off. By default
-        the `display` method will use the entries in the `char_list` directly: if you
-        need to invert the 'normal' sense, set the `inverted` parameter to `True`.
+    def display(self, character: int, inverted: bool = False) -> None:
+        """Display the given `character` on the seven-segment display, using the
+        `_char_list` as a guide for which pins to turn on or off. By default the
+        `display` method will use the entries in the `_char_list` directly: if
+        you need to invert the 'normal' sense, set the `inverted` parameter to
+        `True`.
 
         Parameters
         ----------
 
         character: int
             The value to be displayed on the seven segment display, which must be
             between zero ('0') and nine ('9')
-
-        inverted: bool
-            By default the `display` method assumes that pulling a GPIO pin _low_
-            will turn the relevant segment _on_; i.e. the typical behaviour for a
-            common anode display. If the attached display needs to raise a GPIO pin
-            _high_ to set the segment _on_ (i.e. the typical behaviour for a common
-            cathode display), call the `display` method with `inverted` set to `True`.
+        inverted: bool, optional
+            By default the `display` method assumes that pulling a GPIO pin *low*
+            will turn the relevant segment *on*; i.e. the typical behaviour for a
+            common anode display. If the attached display needs to raise a GPIO
+            pin *high* to set the segment *on* (i.e. the typical behaviour for a
+            common cathode display), call the `display` method with `inverted`
+            set to `True`.
 
         Raises
         ------
 
-        * `IndexError` if the `character` is not in a range that can be displayed.
+        IndexError
+            The `character` is not in a range that can be displayed.
         """
-
         # For a character in the valid range...
         if 0 <= character <= 9:
-
             if not inverted:
                 # ... if the request is to display in the non-inverted form, then
-                # select the row in `char_list` corresponding to the character to
+                # select the row in `_char_list` corresponding to the character to
                 # be displayed and then set in turn each of the GPIO pins corresponding
                 # to the segment values either high or low depending on the column
-                # value in `char_list` for that segment value
+                # value in `_char_list` for that segment value
                 for pin in range(7):
-                    self.pin_list[pin].value(self.char_list[character][pin])
+                    self.pin_list[pin].value(self._char_list[character][pin])
             else:
                 # ... if the request is to display in the inverted form, then
-                # select the row in `char_list` corresponding to the character to
+                # select the row in `_char_list` corresponding to the character to
                 # be displayed and then set in turn each of the GPIO pins corresponding
-                # to the segment values either high or low depending on the _inverse_ of
-                # the column value in `char_list` for that segment value
+                # to the segment values either high or low depending on the *inverse* of
+                # the column value in `_char_list` for that segment value
                 for pin in range(7):
-                    self.pin_list[pin].value(not self.char_list[character][pin])
+                    self.pin_list[pin].value(not self._char_list[character][pin])
         else:
             raise IndexError(
                 "The display character must be between zero ('0') and nine ('9')"
             )
```

### Comparing `lbutils-mp-0.1.1/lbutils/drivers/seven_segment_hex.py` & `lbutils-mp-0.2.0/lbutils/drivers/seven_segment_hex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,31 @@
-"""
-Simple hexadecimal driver for a seven-segment display, requiring seven GPIO pins.
+# This module, and all included code, is made available under the terms of
+# the MIT Licence
+#
+# Copyright (c) 2023 Roz Wyatt-Millington, David Love
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+"""Simple hexadecimal driver for a seven-segment display, requiring seven GPIO
+pins.
 
 Overview
 --------
 
 During initialisation the user must supply a list of exactly seven GPIO pins,
 using the numeric pin identifier (e.g. 16 for GPIO Pin 16). Each entry in the
 list corresponds to the segment 'a' (for the first entry) to 'g' (for the last
@@ -26,59 +48,35 @@
 integer in the range 0..F representing the number to show on the seven segment.
 Not that by default the `display` method assumes that GPIO pins must be held
 _low_ for the segment to display: i.e. the behaviour normally used by common
 anode seven-segment displays. If you need the requested GPIO pin to be held
 _high_ to display a segment, pass in `True` to the `inverted` parameter of the
 `display` method.
 
-.. Note: This driver will only display characters in the range '0' to 'F', and
-will raise a `ValueError` exception if the requested character is not in an
-appropriate range.
+!!! Note
+    This driver will only display characters in the range '0' to 'F', and
+    will raise a `ValueError` exception if the requested character is not in an
+    appropriate range.
 
 Examples
 --------
 
-* Examples Folder: `seven_segment_hex_example.py`
+* Examples Folder: `examples/drivers/seven_segment_hex_example.py`
 * [WokWi](https://wokwi.com/projects/360462223276690433)
 
 Tested Implementations
 ----------------------
 
 This version is written for MicroPython 3.4, and has been tested on:
 
 * Raspberry Pi Pico H/W
-
-Licence
--------
-
-This module, and all included code, is made available under the terms of the MIT Licence
-
-> Copyright (c) 2023 Roz Wyatt-Millington, David Love
-
-> Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-> The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 # Import MicroPython libraries for GPIO access if available
 try:
-    from machine import ADC
     from machine import Pin
 except ImportError:
     print("Ignoring MicroPython includes")
 
 # Import the Python type libraries if available
 try:
     from typing import Union
@@ -86,31 +84,39 @@
     print("The Python type library isn't present. Ignoring.")
 
 ##
 ## Constants
 ##
 
 ASCII_UPPERCASE = set("abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ")
-""" Constant for the set of ASCII letters """
+"""Constant for the set of ASCII letters."""
 ASCII_DIGITS = set("0123456789")
-""" Constant for the set of ASCII digits """
+"""Constant for the set of ASCII digits."""
 ASCII_HEX_DIGITS = set("0123456789ABCDEF")
-""" Constant for the set of ASCII hexadecimal decimal digits,
-including _only_ those which don't fit into `ASCII_DIGITS`"""
+"""Constant for the set of ASCII hexadecimal decimal digits, including _only_
+those which don't fit into `ASCII_DIGITS`"""
 ASCII_HEX_EXTRA_DIGITS = set("ABCDEF")
-""" Constant for the set of ASCII hexadecimal decimal digits,
-including _only_ those which don't fit into `ASCII_DIGITS`"""
+"""Constant for the set of ASCII hexadecimal decimal digits, including _only_
+those which don't fit into `ASCII_DIGITS`"""
 
 ##
 ## Classes
 ##
 
 
 class SegHexDisplay:
-    char_list = [
+    """Simple hexadecimal driver for a seven-segment display, requiring seven
+    GPIO pins.
+
+    **Note:** This driver will only display characters in the range '0' to
+    'F', and will raise a `ValueError` exception if the requested character
+    is not in an appropriate range.
+    """
+
+    _char_list = [
         [False, False, False, False, False, False, True],
         [True, False, False, True, True, True, True],
         [False, False, True, False, False, True, False],
         [False, False, False, False, True, True, False],
         [True, False, False, True, True, False, False],
         [False, True, False, False, True, False, False],
         [False, True, False, False, False, False, False],
@@ -120,34 +126,34 @@
         [False, False, False, True, False, False, False],
         [True, True, False, False, False, False, False],
         [False, True, True, False, False, False, True],
         [True, False, False, False, False, True, False],
         [False, True, True, False, False, False, False],
         [False, True, True, True, False, False, False],
     ]
-    """
-    Defines how characters are rendered, from zero ('0') in the first entry to
-    nine ('9') as the last entry. Note that pins which are listed here as
-    `False` will be _on_ using the default options to the `display` method.
+    """Defines how characters are rendered, from zero ('0') in the first entry
+    to nine ('9') as the last entry.
+
+    Note that pins which are listed here as `False` will be _on_ using the
+    default options to the `display` method.
     """
 
-    def __init__(self, gpio_request: list):
-        """
-        Initialise a seven-segment display, using the user supplied
-        list of GPIO pins in `gpio_request` as reference for pins to
-        drive.
+    def __init__(self, gpio_request: list) -> None:
+        """Initialise a seven-segment display, using the user supplied list of
+        GPIO pins in `gpio_request` as reference for pins to drive.
 
         This class also assume a common anode seven-segment display by default,
         and so will assume that pulling a GPIO pin _low_ will turn the relevant
         segment _on_. If you need to modify this behaviour, see the `inverted`
         parameter for the `display` method.
 
-        .. Note::
-            This list of entries in the `gpio_request` _must_ be exactly seven
-            entries long, or the class will throw a `ValueError` in the constructor.
+        !!! Note
+            This list of entries in the `gpio_request` _must_ be **exactly**
+            seven entries long, or the class will throw a `ValueError` in the
+            constructor.
 
         Parameters
         ----------
 
         gpio_request: list
             The pin-ordered list of GPIO pins to use for the segment positions
             'a' (as the first entry in the list) to 'g' (as the last entry
@@ -157,126 +163,126 @@
             underlying GPIO object for each of the entries in the list. If
             the GPIO pins need to be initialised first, this must be done
             _before_ calling this constructor.
 
         Raises
         ------
 
-        * `ValueError` if the `gpio_request` is empty, or does not have exactly
-          seven elements in the list.
+        ValueError
+            The `gpio_request` is empty, or does not have exactly
+            seven elements in the list.
         """
         self.pin_list = []
 
         if (gpio_request is None) or (not gpio_request):
             raise ValueError("The GPIO Request List is empty")
         elif len(gpio_request) != 7:
             raise ValueError("The GPIO Request List must be EXACTLY seven entries long")
         else:
             for segment in range(7):
                 self.pin_list.append(Pin(gpio_request[segment], Pin.OUT))
 
-    def display(self, character: Union[int, str], inverted: bool = False):
-        """
-        Display the given `character` on the seven-segment display,
-        using the `char_list` as a guide for which pins to turn on or off. By default the
-        `display` method will use the entries in the `char_list` directly: if you need to
-        invert the 'normal' sense, set the `inverted` parameter to `True`.
+    def display(self, character: Union[int, str], inverted: bool = False) -> None:
+        """Display the given `character` on the seven-segment display, using the
+        `_char_list` as a guide for which pins to turn on or off. By default the
+        `display` method will use the entries in the `_char_list` directly: if
+        you need to invert the 'normal' sense, set the `inverted` parameter to
+        `True`.
 
         Parameters
         ----------
 
         character: int or str
-            The value to be displayed on the seven segment display. The value must be
-            either a `str` or an `int`, and will be interpreted as follows:
-
-            `int`: The value must be between zero ('0') and sixteen decimal ('F'), and
-            will be interpreted as a single, hexadecimal digit.
-
-            `str`: The value will be interpreted directly as a hexadecimal digit, and
-            must be in the range `[0..F]`.
-
-            If the type does not conform to the above, then a `TypeError` will be raised.
-
-        inverted: bool
-            By default the `display` method assumes that pulling a GPIO pin _low_ will
-            turn the relevant segment _on_; i.e. the typical behaviour for a common
-            anode display. If the attached display needs to raise a GPIO pin _high_ to
-            set the segment _on_ (i.e. the typical behaviour for a common cathode
-            display), call the `display` method with `inverted` set to `True`.
+            The value to be displayed on the seven segment display. The value
+            must be either a `str` or an `int`, and will be interpreted as
+            follows:
+
+            `int`: The value must be between zero ('0') and sixteen decimal
+            ('F'), and will be interpreted as a single, hexadecimal digit.
+
+            `str`: The value will be interpreted directly as a hexadecimal digit,
+            and must be in the range `[0..F]`.
+
+            If the type does not conform to the above, then a `TypeError` will be
+            raised.
+        inverted: bool, optional
+            By default the `display` method assumes that pulling a GPIO pin _low_
+            will turn the relevant segment _on_; i.e. the typical behaviour for a
+            common anode display. If the attached display needs to raise a GPIO
+            pin _high_ to set the segment _on_ (i.e. the typical behaviour for a
+            common cathode display), call the `display` method with `inverted`
+            set to `True`.
 
         Raises
         ------
 
-        * `IndexError` if the `character` is not in a range that can be displayed.
-        * `TypeError` if the `character` is not either an `int` or a `str`
+        IndexError
+            The `character` is not in a range that can be displayed.
+        TypeError
+            The `character` is not either an `int` or a `str`
         """
-
         # Convert a decimal integer in the range [0..15], and then display
         if isinstance(character, int):
-
             # For a character in the valid range...
             if 0 <= character <= 15:
-
                 if not inverted:
                     # ... if the request is to display in the non-inverted form, then
-                    # select the row in `char_list` corresponding to the character to
+                    # select the row in `_char_list` corresponding to the character to
                     # be displayed and then set in turn each of the GPIO pins corresponding
                     # to the segment values either high or low depending on the column
-                    # value in `char_list` for that segment value
+                    # value in `_char_list` for that segment value
                     for pin in range(7):
-                        self.pin_list[pin].value(self.char_list[character][pin])
+                        self.pin_list[pin].value(self._char_list[character][pin])
                 else:
                     # ... if the request is to display in the inverted form, then
-                    # select the row in `char_list` corresponding to the character to
+                    # select the row in `_char_list` corresponding to the character to
                     # be displayed and then set in turn each of the GPIO pins corresponding
                     # to the segment values either high or low depending on the _inverse_ of
-                    # the column value in `char_list` for that segment value
+                    # the column value in `_char_list` for that segment value
                     for pin in range(7):
-                        self.pin_list[pin].value(not self.char_list[character][pin])
+                        self.pin_list[pin].value(not self._char_list[character][pin])
             else:
                 raise IndexError(
                     "The display character must be between zero ('0') and sixteen ('F')"
                 )
 
         # Convert a string integer in the range [0..F], and then display
         elif isinstance(character, str):
-
             # Normalise the character by converting to upper case
             normalised_character = character.upper()
 
             # Check if this normalise character is a valid hexadecimal digit...
             if normalised_character in ASCII_HEX_DIGITS:
-
                 # ... if so, convert the hexadecimal string to an integer, so we can use
                 # this as the index for the character lookup
-                char_list_index = int(normalised_character, 16)
+                _char_list_index = int(normalised_character, 16)
 
                 if not inverted:
                     # If the request is to display in the non-inverted form, then
-                    # select the row in `char_list` corresponding to the `char_list_index` to
+                    # select the row in `_char_list` corresponding to the `_char_list_index` to
                     # be displayed and then set in turn each of the GPIO pins corresponding
                     # to the segment values either high or low depending on the column
-                    # value in `char_list` for that segment value
+                    # value in `_char_list` for that segment value
                     for pin in range(7):
-                        self.pin_list[pin].value(self.char_list[char_list_index][pin])
+                        self.pin_list[pin].value(self._char_list[_char_list_index][pin])
 
                 else:
                     # If the request is to display in the inverted form, then
-                    # select the row in `char_list` corresponding to the `char_list_index` to
+                    # select the row in `_char_list` corresponding to the `_char_list_index` to
                     # be displayed and then set in turn each of the GPIO pins corresponding
                     # to the segment values either high or low depending on the _inverse_ of
-                    # the column value in `char_list` for that segment value
+                    # the column value in `_char_list` for that segment value
                     for pin in range(7):
                         self.pin_list[pin].value(
-                            not self.char_list[char_list_index][pin]
+                            not self._char_list[_char_list_index][pin]
                         )
             else:
                 raise IndexError(
                     "The display character must be a string between '0' and 'F'"
                 )
 
         # If we can't convert the input `character`, raise an exception
         else:
             raise TypeError(
-                "The 'character' parameter must either be an integer\
-                ('int') or a string ('str') type."
+                "The 'character' parameter must either be an integer ('int') or a"
+                " string ('str') type."
             )
```

### Comparing `lbutils-mp-0.1.1/lbutils/examples/__init__.py` & `lbutils-mp-0.2.0/lbutils/examples/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-"""
-Examples for the library use: mostly as _incomplete_ code fragments and demonstrations.
+# This module, and all included code, is made available under the terms of the MIT Licence
+#
+# Copyright (c) 2023 David Love
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+"""Examples for the library use: mostly as _incomplete_ code fragments and
+demonstrations.
 
 Overview
 --------
 
 This is a collection of examples, utility classes and other scraps of code which
 demonstrate the use of the library in common applications. Many of these
 examples will require extension, or further development in real applications.
 However they should give some idea of what those more complete applications may
 look like.
 
 Demonstrations
 --------------
 
-Many of the examples require a working board to reproduce, and so where possible examples have been provided on [WokWi](https://wokwi.com/).
+Many of the examples require a working board to reproduce, and so where possible
+examples have been provided on [WokWi](https://wokwi.com/).
 
 Current demonstrations are
 
-* `lbutils.drivers.seven_segment.SegDisplay`: [7-Segment Display](https://wokwi.com/projects/360451068863047681)
-* `lbutils.drivers.seven_segment_hex.SegHexDisplay`: [7-Segment Hex Digits Display](https://wokwi.com/projects/360462223276690433)
+* `lbutils.drivers.seven_segment.SegDisplay`: [7-Segment Display](https://
+wokwi.com/projects/360451068863047681)
+* `lbutils.drivers.seven_segment_hex.SegHexDisplay`: [7-Segment Hex Digits
+Display](https://wokwi.com/projects/360462223276690433)
 
 Tested Implementations
 ----------------------
 
 This version is written for MicroPython 3.4, and has been tested on:
 
   * Raspberry Pi Pico H/W
-
-Licence
--------
-
-This module, and all included code, is made available under the terms of the MIT Licence
-
-> Copyright (c) 2023 David Love
-
-> Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-> The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 __pdoc__ = {"seven_segment_example": False, "seven_segment_hex_example": False}
```

### Comparing `lbutils-mp-0.1.1/lbutils/helpers/__init__.py` & `lbutils-mp-0.2.0/lbutils/helpers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-"""
-Helper code and utilities, mostly helping to automate common tasks and replace boiler-plate code.
-
-Overview
---------
-
-This is a collection of functions and classes which help replace boiler-plate code for tasks such as setting up network access.
+# This module, and all included code, is made available under the terms of the
+# MIT Licence
+#
+# Copyright (c) 2023 David Love
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+"""Helper code and utilities, mostly helping to automate common tasks and
+replace boiler-plate code. Many of the classes and utilities in this collection
+are aimed at supporting the Leeds Beckett micro-controller development board,
+but may also be helpful for bare Pico H/W support.
 
 Tested Implementations
 ----------------------
 
 This version is written for MicroPython 3.4, and has been tested on:
 
   * Raspberry Pi Pico H/W
-
-Licence
--------
-
-This module, and all included code, is made available under the terms of the MIT Licence
-
-> Copyright (c) 2023 David Love
-
-> Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-> The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
```

### Comparing `lbutils-mp-0.1.1/lbutils/pmod/__init__.py` & `lbutils-mp-0.2.0/lbutils/pmods/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-"""Utilities and Drivers for the Drivers and support for the Digilent Peripheral Modules
-
-Overview
---------
-
-This library is designed to provide drivers and support for the [Digilent peripheral modules](https://digilent.com/reference/pmod/start). Not all boards are supported: and in some cases only certain busses are supported (e.g. using only the I2C bus, even though the `pmod` supports both I2C and SPI).
-
-Examples for how to use the library can be found in the '`examples`' folder: or [in the documentation](https://dlove24.github.io/urest/lbutils/examples/index.html).
+# This module, and all included code, is made available under the terms of the MIT
+# Licence
+#
+# Copyright 2022-2023, David Love
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+"""Utilities and Drivers for the Drivers and support for the Digilent Peripheral
+Modules. This library is designed to provide drivers and support for the
+[Digilent peripheral modules](https://digilent.com/reference/pmod/start). Not
+all boards are supported: and in some cases only certain busses are supported
+(e.g. using only the I2C bus, even though the `pmod` supports both I2C and SPI).
+
+Examples for how to use the library can be found in the '`examples`' folder: or
+[in the documentation](https://lbutils.readthedocs.io/en/latest/) for the
+specific classes.
 
 Tested Implementations
 ----------------------
 
 This version is written for MicroPython 3.4, and has been tested on:
 
   * Raspberry Pi Pico H/W
-
-Licence
--------
-
-This module, and all included code, is made available under the terms of the MIT Licence
-
-> Copyright (c) 2023 David Love
-
-> Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-> The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
```

