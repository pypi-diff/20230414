# Comparing `tmp/xmipy-1.3.0.tar.gz` & `tmp/xmipy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmipy-1.3.0.tar", last modified: Tue Mar 21 09:04:37 2023, max compression
+gzip compressed data, was "xmipy-1.3.1.tar", last modified: Fri Apr 14 13:07:49 2023, max compression
```

## Comparing `xmipy-1.3.0.tar` & `xmipy-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 09:04:37.735331 xmipy-1.3.0/
--rw-rw-rw-   0        0        0     7169 2023-01-05 07:24:58.000000 xmipy-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     1666 2023-03-21 09:04:37.734331 xmipy-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      887 2023-01-05 07:24:58.000000 xmipy-1.3.0/README.md
--rw-rw-rw-   0        0        0     1406 2023-03-21 08:46:12.000000 xmipy-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-21 09:04:37.735331 xmipy-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0       96 2023-03-21 08:46:12.000000 xmipy-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 09:04:37.722695 xmipy-1.3.0/tests/
--rw-rw-rw-   0        0        0    13393 2023-03-21 08:46:12.000000 xmipy-1.3.0/tests/test_mf6_dis_bmi.py
--rw-rw-rw-   0        0        0     1345 2023-01-05 07:24:58.000000 xmipy-1.3.0/tests/test_mf6_dis_errors.py
--rw-rw-rw-   0        0        0     1494 2023-01-05 07:24:58.000000 xmipy-1.3.0/tests/test_mf6_dis_utils.py
--rw-rw-rw-   0        0        0     5503 2023-01-05 07:24:58.000000 xmipy-1.3.0/tests/test_mf6_dis_xmi.py
--rw-rw-rw-   0        0        0     4057 2023-01-05 07:24:58.000000 xmipy-1.3.0/tests/test_mf6_disu_bmi.py
--rw-rw-rw-   0        0        0     1191 2023-03-21 08:46:12.000000 xmipy-1.3.0/tests/test_timers.py
-drwxrwxrwx   0        0        0        0 2023-03-21 09:04:37.727695 xmipy-1.3.0/xmipy/
--rw-rw-rw-   0        0        0      175 2023-03-21 08:50:46.000000 xmipy-1.3.0/xmipy/__init__.py
--rw-rw-rw-   0        0        0      349 2023-01-05 07:24:58.000000 xmipy-1.3.0/xmipy/errors.py
--rw-rw-rw-   0        0        0        0 2023-01-05 07:24:58.000000 xmipy-1.3.0/xmipy/py.typed
-drwxrwxrwx   0        0        0        0 2023-03-21 09:04:37.734331 xmipy-1.3.0/xmipy/timers/
--rw-rw-rw-   0        0        0        0 2023-01-05 07:24:58.000000 xmipy-1.3.0/xmipy/timers/__init__.py
--rw-rw-rw-   0        0        0     2118 2023-01-05 07:24:58.000000 xmipy-1.3.0/xmipy/timers/timer.py
--rw-rw-rw-   0        0        0     2813 2023-01-05 07:24:58.000000 xmipy-1.3.0/xmipy/timers/timers.py
--rw-rw-rw-   0        0        0      236 2023-01-05 07:24:58.000000 xmipy-1.3.0/xmipy/utils.py
--rw-rw-rw-   0        0        0     4797 2023-01-05 07:24:58.000000 xmipy-1.3.0/xmipy/xmi.py
--rw-rw-rw-   0        0        0    25876 2023-03-21 08:46:12.000000 xmipy-1.3.0/xmipy/xmiwrapper.py
-drwxrwxrwx   0        0        0        0 2023-03-21 09:04:37.731317 xmipy-1.3.0/xmipy.egg-info/
--rw-rw-rw-   0        0        0     1666 2023-03-21 09:04:37.000000 xmipy-1.3.0/xmipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-03-21 09:04:37.000000 xmipy-1.3.0/xmipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 09:04:37.000000 xmipy-1.3.0/xmipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-21 09:04:37.000000 xmipy-1.3.0/xmipy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       99 2023-03-21 09:04:37.000000 xmipy-1.3.0/xmipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-21 09:04:37.000000 xmipy-1.3.0/xmipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:49.947616 xmipy-1.3.1/
+-rw-rw-rw-   0        0        0     7169 2023-03-23 10:39:36.000000 xmipy-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     1666 2023-04-14 13:07:49.946645 xmipy-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      887 2023-03-23 10:39:36.000000 xmipy-1.3.1/README.md
+-rw-rw-rw-   0        0        0     1349 2023-03-28 13:43:37.000000 xmipy-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:07:49.947616 xmipy-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       96 2023-03-23 10:39:36.000000 xmipy-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:49.918618 xmipy-1.3.1/tests/
+-rw-rw-rw-   0        0        0    13035 2023-04-12 07:24:33.000000 xmipy-1.3.1/tests/test_mf6_dis_bmi.py
+-rw-rw-rw-   0        0        0      917 2023-04-12 07:24:33.000000 xmipy-1.3.1/tests/test_mf6_dis_errors.py
+-rw-rw-rw-   0        0        0     1216 2023-04-12 07:24:33.000000 xmipy-1.3.1/tests/test_mf6_dis_utils.py
+-rw-rw-rw-   0        0        0     1620 2023-04-12 07:24:33.000000 xmipy-1.3.1/tests/test_mf6_dis_xmi.py
+-rw-rw-rw-   0        0        0     2329 2023-04-12 07:24:33.000000 xmipy-1.3.1/tests/test_mf6_disu_bmi.py
+-rw-rw-rw-   0        0        0     1298 2023-04-12 07:24:33.000000 xmipy-1.3.1/tests/test_timers.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:49.929684 xmipy-1.3.1/xmipy/
+-rw-rw-rw-   0        0        0      175 2023-04-14 13:07:17.000000 xmipy-1.3.1/xmipy/__init__.py
+-rw-rw-rw-   0        0        0      349 2023-03-23 10:39:36.000000 xmipy-1.3.1/xmipy/errors.py
+-rw-rw-rw-   0        0        0        0 2023-03-23 10:39:36.000000 xmipy-1.3.1/xmipy/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:49.944741 xmipy-1.3.1/xmipy/timers/
+-rw-rw-rw-   0        0        0        0 2023-03-23 10:39:36.000000 xmipy-1.3.1/xmipy/timers/__init__.py
+-rw-rw-rw-   0        0        0     2118 2023-03-23 10:39:36.000000 xmipy-1.3.1/xmipy/timers/timer.py
+-rw-rw-rw-   0        0        0     2813 2023-03-23 10:39:36.000000 xmipy-1.3.1/xmipy/timers/timers.py
+-rw-rw-rw-   0        0        0      236 2023-03-23 10:39:36.000000 xmipy-1.3.1/xmipy/utils.py
+-rw-rw-rw-   0        0        0     4796 2023-03-28 13:43:37.000000 xmipy-1.3.1/xmipy/xmi.py
+-rw-rw-rw-   0        0        0    26261 2023-04-14 13:07:04.000000 xmipy-1.3.1/xmipy/xmiwrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:07:49.939615 xmipy-1.3.1/xmipy.egg-info/
+-rw-rw-rw-   0        0        0     1666 2023-04-14 13:07:49.000000 xmipy-1.3.1/xmipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-04-14 13:07:49.000000 xmipy-1.3.1/xmipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:07:49.000000 xmipy-1.3.1/xmipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-24 09:46:20.000000 xmipy-1.3.1/xmipy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       98 2023-04-14 13:07:49.000000 xmipy-1.3.1/xmipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 13:07:49.000000 xmipy-1.3.1/xmipy.egg-info/top_level.txt
```

### Comparing `xmipy-1.3.0/LICENSE` & `xmipy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmipy-1.3.0/PKG-INFO` & `xmipy-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmipy
-Version: 1.3.0
+Version: 1.3.1
 Summary: xmipy is an extension to the bmipy Python package
 Author-email: Martijn Russcher <Martijn.Russcher@deltares.nl>, Julian Hofer <Julian.Hofer@deltares.nl>, "Joseph D. Hughes" <jdhughes@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://deltares.github.io/xmipy/xmipy.html
 Project-URL: Source, https://github.com/Deltares/xmipy
 Keywords: BMI,Basic Model Interface
 Classifier: Intended Audience :: Science/Research
```

### Comparing `xmipy-1.3.0/README.md` & `xmipy-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `xmipy-1.3.0/pyproject.toml` & `xmipy-1.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,53 +3,39 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xmipy"
 description = "xmipy is an extension to the bmipy Python package"
 readme = "README.md"
 authors = [
-    {name = "Martijn Russcher", email = "Martijn.Russcher@deltares.nl"},
-    {name = "Julian Hofer", email = "Julian.Hofer@deltares.nl"},
-    {name = "Joseph D. Hughes", email = "jdhughes@usgs.gov"},
+    { name = "Martijn Russcher", email = "Martijn.Russcher@deltares.nl" },
+    { name = "Julian Hofer", email = "Julian.Hofer@deltares.nl" },
+    { name = "Joseph D. Hughes", email = "jdhughes@usgs.gov" },
 ]
 keywords = ["BMI", "Basic Model Interface"]
-license = {text = "CC0"}
+license = { text = "CC0" }
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     "Topic :: Scientific/Engineering :: Hydrology",
 ]
 requires-python = ">=3.8"
-dependencies = [
-    "bmipy",
-    "numpy",
-]
+dependencies = ["bmipy", "numpy"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-tests = [
-    "flopy >=3.3.6",
-    "pytest",
-    "pytest-cov",
-    "requests",
-]
-lint = [
-    "black",
-    "isort",
-    "mypy",
-]
-docs = [
-    "pdoc",
-]
+tests = ["flopy >=3.3.6", "pytest", "pytest-cov", "requests"]
+lint = ["black", "ruff", "mypy"]
+docs = ["pdoc"]
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.dynamic]
-version = {attr = "xmipy.__version__"}
+version = { attr = "xmipy.__version__" }
 
 [tool.setuptools.packages.find]
 include = ["xmipy", "xmipy.*"]
 
 [tool.setuptools.package-data]
 "xmipy" = ["py.typed"]
```

### Comparing `xmipy-1.3.0/tests/test_mf6_dis_bmi.py` & `xmipy-1.3.1/tests/test_mf6_dis_bmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,14 @@
 import pytest
 
 from xmipy import XmiWrapper
 from xmipy.errors import InputError
 
 
 @pytest.fixture
-def flopy_dis_mf6(flopy_dis, modflow_lib_path, request):
-    mf6 = XmiWrapper(lib_path=modflow_lib_path, working_directory=flopy_dis.sim_path)
-
-    # If initialized, call finalize() at end of use
-    request.addfinalizer(mf6.__del__)
-
-    # Write output to screen
-    mf6.set_int("ISTDOUTTOFILE", 0)
-
-    return flopy_dis, mf6
-
-
-@pytest.fixture
 def flopy_dis_idomain_mf6(flopy_dis_idomain, modflow_lib_path, request):
     mf6 = XmiWrapper(
         lib_path=modflow_lib_path, working_directory=flopy_dis_idomain.sim_path
     )
 
     # If initialized, call finalize() at end of use
     request.addfinalizer(mf6.__del__)
@@ -191,18 +178,18 @@
 
 def test_get_var_grid(flopy_dis_mf6):
     flopy_dis, mf6 = flopy_dis_mf6
     mf6.initialize()
 
     # Getting the grid id from the model, requires specifying one variable
     k11_tag = mf6.get_var_address("K11", flopy_dis.model_name, "NPF")
-    prescriped_grid_id = mf6.get_var_grid(k11_tag)
+    prescribed_grid_id = mf6.get_var_grid(k11_tag)
 
     id_tag = mf6.get_var_address("ID", flopy_dis.model_name)
-    assert mf6.get_value_ptr(id_tag) == [prescriped_grid_id]
+    assert mf6.get_value_ptr(id_tag) == [prescribed_grid_id]
 
 
 def test_get_grid_type(flopy_dis_mf6):
     """Tests if the grid type can be extracted"""
     flopy_dis, mf6 = flopy_dis_mf6
     mf6.initialize()
```

### Comparing `xmipy-1.3.0/xmipy/timers/timer.py` & `xmipy-1.3.1/xmipy/timers/timer.py`

 * *Files identical despite different names*

### Comparing `xmipy-1.3.0/xmipy/timers/timers.py` & `xmipy-1.3.1/xmipy/timers/timers.py`

 * *Files identical despite different names*

### Comparing `xmipy-1.3.0/xmipy/xmi.py` & `xmipy-1.3.1/xmipy/xmi.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         """
         ...
 
     @abstractmethod
     def finalize_time_step(self) -> None:
         """Finalize the time step.
 
-        Write messsages and output after model convergence has
+        Write messages and output after model convergence has
         been achieved.
         """
         ...
 
     @abstractmethod
     def get_subcomponent_count(self) -> int:
         """Get the number of components in the simulation.
```

### Comparing `xmipy-1.3.0/xmipy/xmiwrapper.py` & `xmipy-1.3.1/xmipy/xmiwrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import logging
 import os
 import platform
-import sys
 from ctypes import (
     CDLL,
     POINTER,
     byref,
     c_char,
     c_char_p,
     c_double,
     c_int,
     c_void_p,
-    cdll,
     create_string_buffer,
 )
 from enum import Enum, IntEnum, unique
 from pathlib import Path
 from typing import Any, Callable, Tuple, Union
 
 import numpy as np
@@ -65,28 +63,29 @@
             The working directory the shared library expects when being called,
             by default None
 
         timing : bool, optional
             Whether timing should be activated, by default False
         """
 
+        self._state = State.UNINITIALIZED
+
         if lib_dependency:
             self._add_lib_dependency(lib_dependency)
         # LoadLibraryEx flag (py38+): LOAD_WITH_ALTERED_SEARCH_PATH 0x08
         # -> uses the altered search path for resolving dll dependencies
         # `winmode` has no effect while running on Linux or macOS
         # Note: this could make xmipy less secure (dll-injection)
         # Can we get it to work without this flag?
         self.lib = CDLL(str(lib_path), winmode=0x08)
 
         if working_directory:
             self.working_directory = Path(working_directory)
         else:
             self.working_directory = Path().cwd()
-        self._state = State.UNINITIALIZED
         self.timing = timing
         self.libname = os.path.basename(lib_path)
 
         if self.timing:
             self.timer = Timer(
                 name=self.libname,
                 text="Elapsed time for {name}.{fn_name}: {seconds:0.4f} seconds",
@@ -130,20 +129,30 @@
         if self._state == State.UNINITIALIZED:
             with cd(self.working_directory):
                 self._execute_function(self.lib.initialize, config_file.encode())
                 self._state = State.INITIALIZED
         else:
             raise InputError("The library is already initialized")
 
+    def initialize_mpi(self, value: int) -> None:
+        if self._state == State.UNINITIALIZED:
+            with cd(self.working_directory):
+                comm = c_int(value)
+                self._execute_function(self.lib.initialize_mpi, byref(comm))
+                self._state = State.INITIALIZED
+        else:
+            raise InputError("The library is already initialized")
+
     def update(self) -> None:
         with cd(self.working_directory):
             self._execute_function(self.lib.update)
 
     def update_until(self, time: float) -> None:
-        raise NotImplementedError
+        with cd(self.working_directory):
+            self._execute_function(self.lib.update_until, c_double(time))
 
     def finalize(self) -> None:
         if self._state == State.INITIALIZED:
             with cd(self.working_directory):
                 self._execute_function(self.lib.finalize)
                 self._state = State.UNINITIALIZED
         else:
@@ -694,33 +703,31 @@
         """
 
         if self.timing:
             self.timer.start(function.__name__)
 
         try:
             if function(*args) != Status.SUCCESS:
-                msg = f"BMI exception in: {function.__name__} ({detail})"
+                msg = f"BMI exception in {function.__name__} ({detail}):"
 
                 # try to get detailed error msg, beware:
                 # directly call CDLL methods to avoid recursion
                 try:
                     len_err_msg = self.get_constant_int("BMI_LENERRMESSAGE")
                     err_msg = create_string_buffer(len_err_msg)
                     self.lib.get_last_bmi_error(byref(err_msg))
 
                     len_name = self.get_constant_int("BMI_LENCOMPONENTNAME")
                     component_name = create_string_buffer(len_name)
                     self.lib.get_component_name(byref(component_name))
 
-                    print(
-                        "--- Kernel message ("
-                        + component_name.value.decode()
-                        + ") ---\n=> "
-                        + err_msg.value.decode()
+                    msg += (
+                        f" Message from {component_name.value.decode()} '"
+                        + f"{err_msg.value.decode()}'"
                     )
                 except AttributeError:
-                    print("--- Kernel message ---\n" + "=> no details ...")
+                    logging.warn("Couldn't extract error message")
 
                 raise XMIError(msg)
         finally:
             if self.timing:
                 self.timer.stop(function.__name__)
```

### Comparing `xmipy-1.3.0/xmipy.egg-info/PKG-INFO` & `xmipy-1.3.1/xmipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmipy
-Version: 1.3.0
+Version: 1.3.1
 Summary: xmipy is an extension to the bmipy Python package
 Author-email: Martijn Russcher <Martijn.Russcher@deltares.nl>, Julian Hofer <Julian.Hofer@deltares.nl>, "Joseph D. Hughes" <jdhughes@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://deltares.github.io/xmipy/xmipy.html
 Project-URL: Source, https://github.com/Deltares/xmipy
 Keywords: BMI,Basic Model Interface
 Classifier: Intended Audience :: Science/Research
```

### Comparing `xmipy-1.3.0/xmipy.egg-info/SOURCES.txt` & `xmipy-1.3.1/xmipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

