# Comparing `tmp/pyxboxcontroller-0.6.2.tar.gz` & `tmp/pyxboxcontroller-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxboxcontroller-0.6.2.tar", last modified: Fri Nov  4 16:59:27 2022, max compression
+gzip compressed data, was "pyxboxcontroller-0.6.3.tar", last modified: Thu Apr 13 22:37:20 2023, max compression
```

## Comparing `pyxboxcontroller-0.6.2.tar` & `pyxboxcontroller-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-04 16:59:27.899808 pyxboxcontroller-0.6.2/
--rw-rw-rw-   0        0        0     1086 2022-10-20 14:56:56.000000 pyxboxcontroller-0.6.2/LICENCE
--rw-rw-rw-   0        0        0      797 2022-11-04 16:59:27.899808 pyxboxcontroller-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2022-11-03 22:54:39.000000 pyxboxcontroller-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2022-11-04 16:59:27.864913 pyxboxcontroller-0.6.2/pyxboxcontroller/
--rw-rw-rw-   0        0        0     1250 2022-11-03 23:19:02.000000 pyxboxcontroller-0.6.2/pyxboxcontroller/XInput.py
--rw-rw-rw-   0        0        0      105 2022-11-03 23:49:44.000000 pyxboxcontroller-0.6.2/pyxboxcontroller/__init__.py
--rw-rw-rw-   0        0        0     8312 2022-11-04 16:54:52.000000 pyxboxcontroller-0.6.2/pyxboxcontroller/controller.py
-drwxrwxrwx   0        0        0        0 2022-11-04 16:59:27.899808 pyxboxcontroller-0.6.2/pyxboxcontroller.egg-info/
--rw-rw-rw-   0        0        0      797 2022-11-04 16:59:27.000000 pyxboxcontroller-0.6.2/pyxboxcontroller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2022-11-04 16:59:27.000000 pyxboxcontroller-0.6.2/pyxboxcontroller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-04 16:59:27.000000 pyxboxcontroller-0.6.2/pyxboxcontroller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-11-04 16:59:27.000000 pyxboxcontroller-0.6.2/pyxboxcontroller.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-04 16:59:27.905320 pyxboxcontroller-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1107 2022-11-04 16:58:47.000000 pyxboxcontroller-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:37:20.527360 pyxboxcontroller-0.6.3/
+-rw-rw-rw-   0        0        0     1086 2022-10-20 14:56:56.000000 pyxboxcontroller-0.6.3/LICENCE
+-rw-rw-rw-   0        0        0      797 2023-04-13 22:37:20.527360 pyxboxcontroller-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1079 2023-04-13 22:08:02.000000 pyxboxcontroller-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 22:37:20.517351 pyxboxcontroller-0.6.3/pyxboxcontroller/
+-rw-rw-rw-   0        0        0     1250 2022-11-03 23:19:02.000000 pyxboxcontroller-0.6.3/pyxboxcontroller/XInput.py
+-rw-rw-rw-   0        0        0      151 2023-04-13 22:31:22.000000 pyxboxcontroller-0.6.3/pyxboxcontroller/__init__.py
+-rw-rw-rw-   0        0        0     8312 2022-11-04 16:54:52.000000 pyxboxcontroller-0.6.3/pyxboxcontroller/controller.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:37:20.525358 pyxboxcontroller-0.6.3/pyxboxcontroller/examples/
+-rw-rw-rw-   0        0        0      104 2023-04-13 22:37:04.000000 pyxboxcontroller-0.6.3/pyxboxcontroller/examples/__init__.py
+-rw-rw-rw-   0        0        0     1082 2023-04-13 22:20:17.000000 pyxboxcontroller-0.6.3/pyxboxcontroller/examples/example_print_state.py
+-rw-rw-rw-   0        0        0     4607 2023-04-13 22:20:32.000000 pyxboxcontroller-0.6.3/pyxboxcontroller/examples/example_state_gui.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:37:20.522356 pyxboxcontroller-0.6.3/pyxboxcontroller.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-04-13 22:37:20.000000 pyxboxcontroller-0.6.3/pyxboxcontroller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-04-13 22:37:20.000000 pyxboxcontroller-0.6.3/pyxboxcontroller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 22:37:20.000000 pyxboxcontroller-0.6.3/pyxboxcontroller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-13 22:37:20.000000 pyxboxcontroller-0.6.3/pyxboxcontroller.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 22:37:20.527360 pyxboxcontroller-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-04-13 22:23:04.000000 pyxboxcontroller-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:37:20.526359 pyxboxcontroller-0.6.3/tests/
+-rw-rw-rw-   0        0        0     1098 2022-11-04 16:54:27.000000 pyxboxcontroller-0.6.3/tests/test_controller.py
```

### Comparing `pyxboxcontroller-0.6.2/LICENCE` & `pyxboxcontroller-0.6.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.6.2/PKG-INFO` & `pyxboxcontroller-0.6.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxboxcontroller
-Version: 0.6.2
+Version: 0.6.3
 Summary: Allows simple access to the current state of connected Xbox controllers on Windows.
 Home-page: https://github.com/SimpleHydrogen/pyxboxcontroller
 Author: Dan Forbes
 Author-email: danielforbes.123412@gmail.com
 License: MIT
 Keywords: xbox controller,XInput,xbox,controller,python,xbox-controller,xboxcontroller
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pyxboxcontroller-0.6.2/README.md` & `pyxboxcontroller-0.6.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 `from pyxboxcontroller import XboxController, XboxControllerState`
 
 ## Connect to controller
 Connect to the controller with id (starting at 0) using:
 `controller = XboxController(id)`
 ## Getting the current state of the controller
 The current state of the controller can be gotten with:
-`state:XboxControllerState = controller.state`
+`state: XboxControllerState = controller.state`
 This returns an `XboxControllerState` object.
 
 
 Some examples of accessing the states' values:
-```
-left_thumbstick_x:float = state.l_thumb_x
-right_thumbstick_y:float = state.r_thumb_y
-x_pressed:bool = state.x
-lb_pressed:bool = state.lb
+```python
+left_thumbstick_x: float = state.l_thumb_x
+right_thumbstick_y: float = state.r_thumb_y
+x_pressed: bool = state.x
+lb_pressed: bool = state.lb
 ```
 
 Alternately the state of the button (e.g. x) can be gotten with:
-` button_pressed:bool = state.buttons["x"]`
+` button_pressed: bool = state.buttons["x"]`
```

### Comparing `pyxboxcontroller-0.6.2/pyxboxcontroller/XInput.py` & `pyxboxcontroller-0.6.3/pyxboxcontroller/XInput.py`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.6.2/pyxboxcontroller/controller.py` & `pyxboxcontroller-0.6.3/pyxboxcontroller/controller.py`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.6.2/pyxboxcontroller.egg-info/PKG-INFO` & `pyxboxcontroller-0.6.3/pyxboxcontroller.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxboxcontroller
-Version: 0.6.2
+Version: 0.6.3
 Summary: Allows simple access to the current state of connected Xbox controllers on Windows.
 Home-page: https://github.com/SimpleHydrogen/pyxboxcontroller
 Author: Dan Forbes
 Author-email: danielforbes.123412@gmail.com
 License: MIT
 Keywords: xbox controller,XInput,xbox,controller,python,xbox-controller,xboxcontroller
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pyxboxcontroller-0.6.2/setup.py` & `pyxboxcontroller-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.6.2"
+VERSION = "0.6.3"
 DESCRIPTION = 'Allows simple access to the current state of connected Xbox controllers on Windows.'
 
 setup(name='pyxboxcontroller',
     version = VERSION,
     description = DESCRIPTION,
     license = "MIT",
     author = 'Dan Forbes',
```

