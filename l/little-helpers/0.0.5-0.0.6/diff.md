# Comparing `tmp/little_helpers-0.0.5.tar.gz` & `tmp/little_helpers-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/almami/Alexander/Python_Skripte/00_packages/little_helpers/dist/tmpe4683wf6/little_helpers-0.0.5.tar", last modified: Wed Feb 23 23:14:36 2022, max compression
+gzip compressed data, was "little_helpers-0.0.6.tar", last modified: Fri Apr 14 20:41:39 2023, max compression
```

## Comparing `little_helpers-0.0.5.tar` & `little_helpers-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2022-02-23 23:14:36.000000 little_helpers-0.0.5/
--rw-rw-r--   0 almami    (1000) almami    (1000)     1074 2021-10-18 17:44:25.000000 little_helpers-0.0.5/LICENSE
--rw-rw-r--   0 almami    (1000) almami    (1000)     2639 2022-02-23 23:14:36.000000 little_helpers-0.0.5/PKG-INFO
--rw-rw-r--   0 almami    (1000) almami    (1000)     2068 2021-11-06 18:58:23.000000 little_helpers-0.0.5/README.md
--rw-rw-r--   0 almami    (1000) almami    (1000)      104 2021-10-16 18:41:13.000000 little_helpers-0.0.5/pyproject.toml
--rw-rw-r--   0 almami    (1000) almami    (1000)      659 2022-02-23 23:14:36.000000 little_helpers-0.0.5/setup.cfg
--rw-rw-r--   0 almami    (1000) almami    (1000)      262 2022-02-23 23:11:42.000000 little_helpers-0.0.5/setup.py
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2022-02-23 23:14:36.000000 little_helpers-0.0.5/src/
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2022-02-23 23:14:36.000000 little_helpers-0.0.5/src/little_helpers/
--rw-rw-r--   0 almami    (1000) almami    (1000)      268 2022-01-27 20:03:13.000000 little_helpers-0.0.5/src/little_helpers/__init__.py
--rw-rw-r--   0 almami    (1000) almami    (1000)     5680 2022-02-23 19:40:14.000000 little_helpers-0.0.5/src/little_helpers/array_tools.py
--rw-rw-r--   0 almami    (1000) almami    (1000)    12722 2022-02-23 22:52:55.000000 little_helpers-0.0.5/src/little_helpers/geometry.py
--rw-rw-r--   0 almami    (1000) almami    (1000)     1877 2021-12-22 20:40:35.000000 little_helpers-0.0.5/src/little_helpers/hydrogel_conversions.py
--rw-rw-r--   0 almami    (1000) almami    (1000)    17567 2022-02-23 19:40:14.000000 little_helpers-0.0.5/src/little_helpers/math_functions.py
--rw-rw-r--   0 almami    (1000) almami    (1000)     2843 2022-01-27 20:03:13.000000 little_helpers-0.0.5/src/little_helpers/math_to_word.py
--rw-rw-r--   0 almami    (1000) almami    (1000)     2242 2021-10-18 17:44:25.000000 little_helpers-0.0.5/src/little_helpers/num_derive.py
--rw-rw-r--   0 almami    (1000) almami    (1000)      834 2021-10-18 17:44:25.000000 little_helpers-0.0.5/src/little_helpers/statsmodel_wrapper.py
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2022-02-23 23:14:36.000000 little_helpers-0.0.5/src/little_helpers.egg-info/
--rw-rw-r--   0 almami    (1000) almami    (1000)     2639 2022-02-23 23:14:36.000000 little_helpers-0.0.5/src/little_helpers.egg-info/PKG-INFO
--rw-rw-r--   0 almami    (1000) almami    (1000)      545 2022-02-23 23:14:36.000000 little_helpers-0.0.5/src/little_helpers.egg-info/SOURCES.txt
--rw-rw-r--   0 almami    (1000) almami    (1000)        1 2022-02-23 23:14:36.000000 little_helpers-0.0.5/src/little_helpers.egg-info/dependency_links.txt
--rw-rw-r--   0 almami    (1000) almami    (1000)       73 2022-02-23 23:14:36.000000 little_helpers-0.0.5/src/little_helpers.egg-info/requires.txt
--rw-rw-r--   0 almami    (1000) almami    (1000)       15 2022-02-23 23:14:36.000000 little_helpers-0.0.5/src/little_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 20:41:38.855529 little_helpers-0.0.6/
+-rw-rw-rw-   0        0        0     1095 2023-01-17 12:21:27.000000 little_helpers-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2651 2023-04-14 20:41:39.498727 little_helpers-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2102 2023-01-17 12:21:27.000000 little_helpers-0.0.6/README.md
+-rw-rw-rw-   0        0        0      110 2023-01-17 12:21:27.000000 little_helpers-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      688 2023-04-14 20:41:39.512074 little_helpers-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      284 2023-04-14 20:39:46.000000 little_helpers-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:41:38.859529 little_helpers-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 20:41:38.859529 little_helpers-0.0.6/src/little_helpers/
+-rw-rw-rw-   0        0        0      276 2023-01-17 12:21:27.000000 little_helpers-0.0.6/src/little_helpers/__init__.py
+-rw-rw-rw-   0        0        0     5849 2023-01-17 12:21:27.000000 little_helpers-0.0.6/src/little_helpers/array_tools.py
+-rw-rw-rw-   0        0        0    14348 2023-01-17 12:21:28.000000 little_helpers-0.0.6/src/little_helpers/geometry.py
+-rw-rw-rw-   0        0        0     1938 2023-01-17 12:21:28.000000 little_helpers-0.0.6/src/little_helpers/hydrogel_conversions.py
+-rw-rw-rw-   0        0        0    18073 2023-01-17 12:21:28.000000 little_helpers-0.0.6/src/little_helpers/math_functions.py
+-rw-rw-rw-   0        0        0     2929 2023-01-17 12:21:28.000000 little_helpers-0.0.6/src/little_helpers/math_to_word.py
+-rw-rw-rw-   0        0        0     2303 2023-01-17 12:21:28.000000 little_helpers-0.0.6/src/little_helpers/num_derive.py
+-rw-rw-rw-   0        0        0     1312 2023-04-14 20:37:43.000000 little_helpers-0.0.6/src/little_helpers/statsmodel_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:41:38.867529 little_helpers-0.0.6/src/little_helpers.egg-info/
+-rw-rw-rw-   0        0        0     2651 2023-04-14 20:41:38.000000 little_helpers-0.0.6/src/little_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-04-14 20:41:38.000000 little_helpers-0.0.6/src/little_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 20:41:38.000000 little_helpers-0.0.6/src/little_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-04-14 20:41:38.000000 little_helpers-0.0.6/src/little_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 20:41:38.000000 little_helpers-0.0.6/src/little_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 20:41:38.871529 little_helpers-0.0.6/tests/
+-rw-rw-rw-   0        0        0     2001 2023-01-17 12:21:28.000000 little_helpers-0.0.6/tests/test_array_tools.py
+-rw-rw-rw-   0        0        0     1629 2023-01-17 12:21:28.000000 little_helpers-0.0.6/tests/test_hydrogel_conversions.py
+-rw-rw-rw-   0        0        0     1832 2023-01-17 12:21:28.000000 little_helpers-0.0.6/tests/test_math_functions.py
+-rw-rw-rw-   0        0        0      584 2023-01-17 12:21:28.000000 little_helpers-0.0.6/tests/test_num_derive.py
+-rw-rw-rw-   0        0        0      586 2023-01-17 12:21:28.000000 little_helpers-0.0.6/tests/test_statsmodel_wrapper.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `little_helpers-0.0.5/LICENSE` & `little_helpers-0.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Alexander Southan
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Alexander Southan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `little_helpers-0.0.5/PKG-INFO` & `little_helpers-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,49 @@
-Metadata-Version: 2.1
-Name: little_helpers
-Version: 0.0.5
-Summary: little helper functions
-Home-page: https://github.com/AlexanderSouthan/little_helpers
-Author: Alexander Southan
-Author-email: alexander.southan@web.de
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/little_helpers/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![build workflow](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/AlexanderSouthan/little_helpers/branch/main/graph/badge.svg?token=W7O1I2YKGO)](https://codecov.io/gh/AlexanderSouthan/little_helpers)
-
-# little_helpers
-Some helpful functions that keep being used in various of my repositories, install via:
-```
-pip install little_helpers
-```
-
-## array_tools.py
-* y_at_y: Find values in y_values that belongs to the values in x_values clostest to x.
-* closest_index: Find the index of a value in array x_values that is clostest to x.
-* segment_xy_values: Segment the x_values and y_values according to segment borders.
-
-## math_functions.py
-* langmuir_isotherm: Calculate the q_e values of a simple Langmuir isotherm.
-* langmuir_isotherm_hydrogel: Calculate the adsotpion inside a hydrogel based on a Langmuir model taking the swelling into account.
-* langmuir_comp: Calculate the q_e values of a Langmuir isotherm taking into account competetive adsorption of two species.
-* triangle: Calculate a triangle function.
-* gaussian: Calculate one or a superposition of Gaussian normal distributions.
-* boxcar: Calculate a boxcar function.
-* boxcar_convolution: Calculate the convolution of a boxcar function with another function.
-* piecewise_polynomial: Calculate the y values of a piecewise polynomial.
-* flory_rehner: Calculate 1/M_c according to the Flory-Rehner equation.
-* Herschel_Bulkley: Calculate the stress according tot he Herschel-Bulkley model.
-* cum_dist_normal: Cumulative distribution function for the normal distribution.
-* cum_dist_normal_with_rise: Superposition of cum_dist_normal and a linear function through the origin.
-
-## num_derive.py
-A simple method to calculate the derivative of discrete data.
-
-## statsmodel_wrapper.py
-A universal sklearn-style wrapper for statsmodels regressors.
-
-
+Metadata-Version: 2.1
+Name: little_helpers
+Version: 0.0.6
+Summary: little helper functions
+Home-page: https://github.com/AlexanderSouthan/little_helpers
+Author: Alexander Southan
+Author-email: alexander.southan@web.de
+Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/little_helpers/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![build workflow](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/AlexanderSouthan/little_helpers/branch/main/graph/badge.svg?token=W7O1I2YKGO)](https://codecov.io/gh/AlexanderSouthan/little_helpers)
+
+# little_helpers
+Some helpful functions that keep being used in various of my repositories, install via:
+```
+pip install little_helpers
+```
+
+## array_tools.py
+* y_at_y: Find values in y_values that belongs to the values in x_values clostest to x.
+* closest_index: Find the index of a value in array x_values that is clostest to x.
+* segment_xy_values: Segment the x_values and y_values according to segment borders.
+
+## math_functions.py
+* langmuir_isotherm: Calculate the q_e values of a simple Langmuir isotherm.
+* langmuir_isotherm_hydrogel: Calculate the adsotpion inside a hydrogel based on a Langmuir model taking the swelling into account.
+* langmuir_comp: Calculate the q_e values of a Langmuir isotherm taking into account competetive adsorption of two species.
+* triangle: Calculate a triangle function.
+* gaussian: Calculate one or a superposition of Gaussian normal distributions.
+* boxcar: Calculate a boxcar function.
+* boxcar_convolution: Calculate the convolution of a boxcar function with another function.
+* piecewise_polynomial: Calculate the y values of a piecewise polynomial.
+* flory_rehner: Calculate 1/M_c according to the Flory-Rehner equation.
+* Herschel_Bulkley: Calculate the stress according tot he Herschel-Bulkley model.
+* cum_dist_normal: Cumulative distribution function for the normal distribution.
+* cum_dist_normal_with_rise: Superposition of cum_dist_normal and a linear function through the origin.
+
+## num_derive.py
+A simple method to calculate the derivative of discrete data.
+
+## statsmodel_wrapper.py
+A universal sklearn-style wrapper for statsmodels regressors.
```

### Comparing `little_helpers-0.0.5/README.md` & `little_helpers-0.0.6/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![build workflow](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/AlexanderSouthan/little_helpers/branch/main/graph/badge.svg?token=W7O1I2YKGO)](https://codecov.io/gh/AlexanderSouthan/little_helpers)
-
-# little_helpers
-Some helpful functions that keep being used in various of my repositories, install via:
-```
-pip install little_helpers
-```
-
-## array_tools.py
-* y_at_y: Find values in y_values that belongs to the values in x_values clostest to x.
-* closest_index: Find the index of a value in array x_values that is clostest to x.
-* segment_xy_values: Segment the x_values and y_values according to segment borders.
-
-## math_functions.py
-* langmuir_isotherm: Calculate the q_e values of a simple Langmuir isotherm.
-* langmuir_isotherm_hydrogel: Calculate the adsotpion inside a hydrogel based on a Langmuir model taking the swelling into account.
-* langmuir_comp: Calculate the q_e values of a Langmuir isotherm taking into account competetive adsorption of two species.
-* triangle: Calculate a triangle function.
-* gaussian: Calculate one or a superposition of Gaussian normal distributions.
-* boxcar: Calculate a boxcar function.
-* boxcar_convolution: Calculate the convolution of a boxcar function with another function.
-* piecewise_polynomial: Calculate the y values of a piecewise polynomial.
-* flory_rehner: Calculate 1/M_c according to the Flory-Rehner equation.
-* Herschel_Bulkley: Calculate the stress according tot he Herschel-Bulkley model.
-* cum_dist_normal: Cumulative distribution function for the normal distribution.
-* cum_dist_normal_with_rise: Superposition of cum_dist_normal and a linear function through the origin.
-
-## num_derive.py
-A simple method to calculate the derivative of discrete data.
-
-## statsmodel_wrapper.py
-A universal sklearn-style wrapper for statsmodels regressors.
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![build workflow](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/AlexanderSouthan/little_helpers/branch/main/graph/badge.svg?token=W7O1I2YKGO)](https://codecov.io/gh/AlexanderSouthan/little_helpers)
+
+# little_helpers
+Some helpful functions that keep being used in various of my repositories, install via:
+```
+pip install little_helpers
+```
+
+## array_tools.py
+* y_at_y: Find values in y_values that belongs to the values in x_values clostest to x.
+* closest_index: Find the index of a value in array x_values that is clostest to x.
+* segment_xy_values: Segment the x_values and y_values according to segment borders.
+
+## math_functions.py
+* langmuir_isotherm: Calculate the q_e values of a simple Langmuir isotherm.
+* langmuir_isotherm_hydrogel: Calculate the adsotpion inside a hydrogel based on a Langmuir model taking the swelling into account.
+* langmuir_comp: Calculate the q_e values of a Langmuir isotherm taking into account competetive adsorption of two species.
+* triangle: Calculate a triangle function.
+* gaussian: Calculate one or a superposition of Gaussian normal distributions.
+* boxcar: Calculate a boxcar function.
+* boxcar_convolution: Calculate the convolution of a boxcar function with another function.
+* piecewise_polynomial: Calculate the y values of a piecewise polynomial.
+* flory_rehner: Calculate 1/M_c according to the Flory-Rehner equation.
+* Herschel_Bulkley: Calculate the stress according tot he Herschel-Bulkley model.
+* cum_dist_normal: Cumulative distribution function for the normal distribution.
+* cum_dist_normal_with_rise: Superposition of cum_dist_normal and a linear function through the origin.
+
+## num_derive.py
+A simple method to calculate the derivative of discrete data.
+
+## statsmodel_wrapper.py
+A universal sklearn-style wrapper for statsmodels regressors.
```

### Comparing `little_helpers-0.0.5/src/little_helpers/array_tools.py` & `little_helpers-0.0.6/src/little_helpers/array_tools.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-import numpy as np
-
-
-def y_at_x(x, x_values, y_values):
-    """
-    Find values in y_values that belongs to the values in x_values clostest to x.
-
-    Parameters
-    ----------
-    x : float or list of float
-        The values to look for in x_values. If the exact values do not exist,
-        the values in x_values clostest to x will be used.
-    x_values : ndarray
-        The array containing the independent variable.
-    y_values : ndarray
-        The array containing the dependent variable.
-
-    Returns
-    -------
-    ndarray
-        The values in y_values that are at the indices of the values of
-        x_values that are clostest to the values in x.
-
-    """
-    y_values = np.asarray(y_values)
-
-    return y_values[closest_index(x, x_values)]
-
-def closest_value(x, x_values):
-    """
-    Find value in x_values that is closest to x.
-
-    Parameters
-    ----------
-    x : float
-        The values to look for in x_values.
-    x_values : ndarray
-        The array containing the numbers to look through.
-
-    Returns
-    -------
-    ndarray
-        The value in x_values closest to x.
-
-    """
-    x_values = np.asarray(x_values)
-
-    return x_values[closest_index(x, x_values)]
-
-def closest_index(x, x_values):
-    """
-    Find the index of a value in array x_values that is clostest to x.
-
-    Parameters
-    ----------
-    x : float or list of float
-        A single value or a list of values to look for in x_values.
-    x_values : ndarray or list
-        The array with the values to compare to x.
-
-    Returns
-    -------
-    ndarray
-        The indices of the values in x_values that are clostest to x.
-
-    """
-    x_values = np.asarray(x_values)
-
-    return np.argmin(np.abs(x-x_values[:, np.newaxis]), axis=0)
-
-def segment_xy_values(x_values, segment_borders, y_values=None):
-    """
-    Segment the x_values and y_values according to segment borders.
-
-    This function is used in the functions piecewise_polynomial_fit and
-    piecewise_polynomial.
-
-    Parameters
-    ----------
-    x_values : ndarray
-        A 1D array with the length M holding the independent variable used for
-        the fit. Must be sorted for the segmetation, so is sorted ascending if
-        it is not already.
-    segment_borders : list of int or float
-        The values with respect to x_values at which the data is divided into
-        segments. An arbitrary number of segment borders may be given, and it
-        is recommended to provide a sorted list in order to avoid confusion.
-    y_values : ndarray or None, optional
-        A 1D array with the length M holding the dependent varibale used for
-        the fit. Default is None which means that no y_values are processed.
-
-    Returns
-    -------
-    x_segments : list of ndarray
-        The segments of x_values used for piecewise polynomial calculations.
-        All segments overlap by one point.
-    y_segments : list of ndarray
-        The segments of y_values used for piecewise polynomial calculations.
-        All segments overlap by one point. Only if y_values are passed to the
-        function.
-
-    """
-    x_values = np.asarray(x_values)
-    if y_values is not None:
-        y_values = np.asarray(y_values)
-
-    if (not np.all(x_values[:-1] <= x_values[1:])):
-        sort_index = np.argsort(x_values)
-        x_values = x_values[sort_index]
-        if y_values is not None:
-            y_values = y_values[sort_index]
-
-    # segment_borders are sorted by x values in segment_borders in order to
-    # avoid problems during segmentation
-    segment_borders = np.sort(segment_borders)
-
-    # ascending_x = x_values[1] > x_values[0]
-
-    # if not ascending_x:
-    #     x_values = np.flip(x_values)
-    #     if y_values is not None:
-    #         y_values = np.flip(y_values)
-
-    # Segmentation indices are the indices of the values in x_values clostest
-    # to the values given by segment_borders. At these points, the data is
-    # split into segments that are fitted individually. Additionally, the index
-    # zero is added for the first data point and the data point number for the
-    # last data point.
-    segmentation_indices = np.array([0, len(x_values)])
-    segmentation_indices = np.insert(segmentation_indices, 1,
-                                     closest_index(segment_borders, x_values))
-    # segmentation_indices = np.insert(segmentation_indices, 1, np.argmin(
-    #     np.abs(x_values[:, np.newaxis]-segment_borders), axis=0))
-
-    # Later on, the right sides of the segments except the last one have to be
-    # extended by one relative to the segmentation indices in order to have an
-    # overlap of one point between the segments.
-    segment_additions = np.zeros(len(segmentation_indices)-1, dtype='int')
-    segment_additions[:-1] = 1
-
-    x_segments = []
-    if y_values is not None:
-        y_segments = []
-    for curr_start, curr_end, curr_add in zip(
-            segmentation_indices[:-1], segmentation_indices[1:],
-            segment_additions):
-        x_segments.append(x_values[curr_start:curr_end + curr_add])
-        if y_values is not None:
-            y_segments.append(y_values[curr_start:curr_end + curr_add])
-
-    # if not ascending_x:
-    #     x_segments = [x_seg[::-1] for x_seg in x_segments][::-1]
-    #     if y_values is not None:
-    #         y_segments = [y_seg[::-1] for y_seg in y_segments][::-1]
-
-    if y_values is not None:
-        return (x_segments, y_segments)
-    else:
-        return x_segments
-    
-def is_numeric(array):
-    array = np.asarray(array)
-    # Make sure all values are numeric or can be converted to numeric
-    try:
-        array.astype(float)
-        numeric = True
-    except:
-        numeric = False
-
+import numpy as np
+
+
+def y_at_x(x, x_values, y_values):
+    """
+    Find values in y_values that belongs to the values in x_values clostest to x.
+
+    Parameters
+    ----------
+    x : float or list of float
+        The values to look for in x_values. If the exact values do not exist,
+        the values in x_values clostest to x will be used.
+    x_values : ndarray
+        The array containing the independent variable.
+    y_values : ndarray
+        The array containing the dependent variable.
+
+    Returns
+    -------
+    ndarray
+        The values in y_values that are at the indices of the values of
+        x_values that are clostest to the values in x.
+
+    """
+    y_values = np.asarray(y_values)
+
+    return y_values[closest_index(x, x_values)]
+
+def closest_value(x, x_values):
+    """
+    Find value in x_values that is closest to x.
+
+    Parameters
+    ----------
+    x : float
+        The values to look for in x_values.
+    x_values : ndarray
+        The array containing the numbers to look through.
+
+    Returns
+    -------
+    ndarray
+        The value in x_values closest to x.
+
+    """
+    x_values = np.asarray(x_values)
+
+    return x_values[closest_index(x, x_values)]
+
+def closest_index(x, x_values):
+    """
+    Find the index of a value in array x_values that is clostest to x.
+
+    Parameters
+    ----------
+    x : float or list of float
+        A single value or a list of values to look for in x_values.
+    x_values : ndarray or list
+        The array with the values to compare to x.
+
+    Returns
+    -------
+    ndarray
+        The indices of the values in x_values that are clostest to x.
+
+    """
+    x_values = np.asarray(x_values)
+
+    return np.argmin(np.abs(x-x_values[:, np.newaxis]), axis=0)
+
+def segment_xy_values(x_values, segment_borders, y_values=None):
+    """
+    Segment the x_values and y_values according to segment borders.
+
+    This function is used in the functions piecewise_polynomial_fit and
+    piecewise_polynomial.
+
+    Parameters
+    ----------
+    x_values : ndarray
+        A 1D array with the length M holding the independent variable used for
+        the fit. Must be sorted for the segmetation, so is sorted ascending if
+        it is not already.
+    segment_borders : list of int or float
+        The values with respect to x_values at which the data is divided into
+        segments. An arbitrary number of segment borders may be given, and it
+        is recommended to provide a sorted list in order to avoid confusion.
+    y_values : ndarray or None, optional
+        A 1D array with the length M holding the dependent varibale used for
+        the fit. Default is None which means that no y_values are processed.
+
+    Returns
+    -------
+    x_segments : list of ndarray
+        The segments of x_values used for piecewise polynomial calculations.
+        All segments overlap by one point.
+    y_segments : list of ndarray
+        The segments of y_values used for piecewise polynomial calculations.
+        All segments overlap by one point. Only if y_values are passed to the
+        function.
+
+    """
+    x_values = np.asarray(x_values)
+    if y_values is not None:
+        y_values = np.asarray(y_values)
+
+    if (not np.all(x_values[:-1] <= x_values[1:])):
+        sort_index = np.argsort(x_values)
+        x_values = x_values[sort_index]
+        if y_values is not None:
+            y_values = y_values[sort_index]
+
+    # segment_borders are sorted by x values in segment_borders in order to
+    # avoid problems during segmentation
+    segment_borders = np.sort(segment_borders)
+
+    # ascending_x = x_values[1] > x_values[0]
+
+    # if not ascending_x:
+    #     x_values = np.flip(x_values)
+    #     if y_values is not None:
+    #         y_values = np.flip(y_values)
+
+    # Segmentation indices are the indices of the values in x_values clostest
+    # to the values given by segment_borders. At these points, the data is
+    # split into segments that are fitted individually. Additionally, the index
+    # zero is added for the first data point and the data point number for the
+    # last data point.
+    segmentation_indices = np.array([0, len(x_values)])
+    segmentation_indices = np.insert(segmentation_indices, 1,
+                                     closest_index(segment_borders, x_values))
+    # segmentation_indices = np.insert(segmentation_indices, 1, np.argmin(
+    #     np.abs(x_values[:, np.newaxis]-segment_borders), axis=0))
+
+    # Later on, the right sides of the segments except the last one have to be
+    # extended by one relative to the segmentation indices in order to have an
+    # overlap of one point between the segments.
+    segment_additions = np.zeros(len(segmentation_indices)-1, dtype='int')
+    segment_additions[:-1] = 1
+
+    x_segments = []
+    if y_values is not None:
+        y_segments = []
+    for curr_start, curr_end, curr_add in zip(
+            segmentation_indices[:-1], segmentation_indices[1:],
+            segment_additions):
+        x_segments.append(x_values[curr_start:curr_end + curr_add])
+        if y_values is not None:
+            y_segments.append(y_values[curr_start:curr_end + curr_add])
+
+    # if not ascending_x:
+    #     x_segments = [x_seg[::-1] for x_seg in x_segments][::-1]
+    #     if y_values is not None:
+    #         y_segments = [y_seg[::-1] for y_seg in y_segments][::-1]
+
+    if y_values is not None:
+        return (x_segments, y_segments)
+    else:
+        return x_segments
+    
+def is_numeric(array):
+    array = np.asarray(array)
+    # Make sure all values are numeric or can be converted to numeric
+    try:
+        array.astype(float)
+        numeric = True
+    except:
+        numeric = False
+
     return numeric
```

### Comparing `little_helpers-0.0.5/src/little_helpers/geometry.py` & `little_helpers-0.0.6/src/little_helpers/geometry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,316 +1,353 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Jan 27 19:12:39 2022
-
-@author: Alexander Southan
-"""
-
-import numpy as np
-
-
-def point_inside_circle(
-        x_values, y_values, z_values=None, x_c=0, y_c=0, z_c=None, r=1):
-    """
-    Calculate if a set of points is inside a circle.
-
-    Parameters
-    ----------
-    x_values : float or ndarray
-        The x coordinates of the points.
-    y_values : float or ndarray
-        The y coordinates of the points. Must have the same length like
-        x_values.
-    z_values : float or ndarray, optional
-        The z coordinates of the points. Must have the same length like
-        x_values. The default is None so that calculations are done in 2D.
-    x_c : float, optional
-        The x coordinate of the circle center. The default is 0.
-    y_c : float, optional
-        The y coordinate of the circle center. The default is 0.
-    z_c : float or None, optional
-        The z coordinate of the circle center. Default is None so that
-        calculations are done in 2D.
-    r : float, optinal
-        The radius of the circle. The default is 1.
-
-    Returns
-    -------
-    bool or ndarray
-        A boolean or an array of booleans stating if the points are within the
-        circle. Has the same shape like x_values and y_values.
-
-    """
-    if (z_c is None) or (z_values is None):
-        params = np.asarray([x_values-x_c, y_values-y_c])
-    else:
-        params = np.asarray([x_values-x_c, y_values-y_c, z_values-z_c])
-
-    return ((params)**2).sum(axis=0) <= r**2
-
-
-def point_inside_cartesianbox(
-        x_values, y_values=None, z_values=None, x_limits=[-1, 1],
-        y_limits=[-1, 1], z_limits=[-1, 1]):
-    """
-    Calculate if points are inside of a cartesian box.
-
-    The cartesian box can be a 1D, 2D or 3D box. The 2D box is a rectangle and
-    the 3D box a rectangular prism.
-
-    Parameters
-    ----------
-    x_values : float or ndarray
-        The x coordinates of the points.
-    y_values : float or ndarray, optional
-        The y coordinates of the points. Must have the same length like
-        x_values. The default is None.
-    z_values : float or ndarray, optional
-        The z coordinates of the points. Must have the same length like
-        x_values. The default is None.
-    x_limits : ndarray or None, optional
-        Contains two elements, first the lower limit and second the upper limit
-        allowed for the x coordinate. Each value can be None, so that the
-        corresponding limit does not exist. The default is [-1, 1].
-    y_limits : ndarray or None, optional
-        Contains two elements, first the lower limit and second the upper limit
-        allowed for the y coordinate. Each value can be None, so that the
-        corresponding limit does not exist. The default is [-1, 1].
-    z_limits : ndarray or None, optional
-        Contains two elements, first the lower limit and second the upper limit
-        allowed for the z coordinate. Each value can be None, so that the
-        corresponding limit does not exist. The default is [-1, 1].
-
-    Returns
-    -------
-    ndarray or bool
-        A boolean ndarray or a signle boolean value in the shape of x_values,
-        stating if the points are within the box or not.
-
-    """
-    if (y_values is None) and (z_values is None):
-        dims = 1
-    elif z_values is None:
-        dims = 2
-    else:
-        dims = 3
-
-    limits = np.asarray([curr_lims for curr_lims
-                         in [x_limits, y_limits, z_limits][:dims]])
-    coords = np.asarray([curr_coords for curr_coords in
-                         [x_values, y_values, z_values][:dims]])
-
-    inside_box = np.empty_like(coords, dtype='bool')
-
-    for curr_idx, (curr_values, curr_limits) in enumerate(zip(coords, limits)):
-        if (curr_limits is None) or (curr_limits[0] is None):
-            below_lower = np.full_like(curr_values, False, dtype='bool')
-        else:
-            below_lower = curr_values < curr_limits[0]
-
-        if (curr_limits is None) or (curr_limits[1] is None):
-            above_upper = np.full_like(curr_values, False, dtype='bool')
-        else:
-            above_upper = curr_values > curr_limits[1]
-
-        inside_box[curr_idx] = ~(below_lower | above_upper)
-
-    return np.all(inside_box, axis=0)
-
-
-def line_through_box(x_values, y_values, box={'x': [-1, 1], 'y': [-1, 1]}):
-    """
-    Calculate if a line defined by two points passes through a rectangular box.
-
-    The two points define an endless line in two dimensions and it is
-    calculated if this endless line travels through the box. So it is totally
-    irrelevant where exactly the two points are.
-
-    Parameters
-    ----------
-    x_values : list or ndarray
-        A list containing two values which are the x coodinates of the two
-        data points.
-    y_values : list or ndarray
-        A list containing two values which are the x coodinates of the two
-        data points.
-    box : dict, optional
-        A dictionary containing the box limits. Must contain the keys 'x' for
-        the lower and upper limits on the x coordinate and 'y' for the lower
-        and upper limits on the y coordinate, both given as a list or ndarray
-        with two entries. The default is {'x': [-1, 1], 'y': [-1, 1]}.
-
-    Returns
-    -------
-    float
-        The distance the line travels through the box.
-    list
-        The two x coordinates where the line intersects the box walls.
-    list
-        The two y coordinates where the line intersects the box walls.
-
-    """
-    slope = (y_values[1]-y_values[0])/(x_values[1]-x_values[0])
-    intercept = y_values[0] - slope*x_values[0]
-
-    if slope != 0:
-        intersect_x = np.sort((box['y']-intercept)/slope)
-        overlap_x = [max(intersect_x[0], box['x'][0]),
-                     min(intersect_x[1], box['x'][1])]
-        overlap_x = overlap_x if overlap_x[0] < overlap_x[1] else []
-    else:
-        if ((y_values[0] > box['y'][0]) & (y_values[0] < box['y'][1])):
-            overlap_x = box['x']
-        else:
-            overlap_x = []
-
-    if overlap_x:
-        overlap_y = [slope*curr_x+intercept for curr_x in overlap_x]
-        score = np.sqrt((overlap_x[1]-overlap_x[0])**2 +
-                        (overlap_y[1]-overlap_y[0])**2)
-        return (score, overlap_x, overlap_y)
-    else:
-        return (0, [], [])
-
-
-def reflect_line_in_box(start, end, limits):
-    """
-    Reflect a line defined by two points within a one- to threedimensional box.
-
-    Parameters
-    ----------
-    start : 2D ndarray
-        The start points of the lines to be reflected. Must be a 2D array with
-        the shape (n, d) where n is the number of data points and d is the
-        dimension (between 1 and 3).
-    end : 2D ndarray
-        The end points of the lines to be reflected. Must be a 2D array with
-        the shape (n, d) where n is the number of data points and d is the
-        dimension (between 1 and 3).
-    limits : dict
-        A dictionary containing the box limits. Cancontain the keys 'x' for
-        the lower and upper limits on the x coordinate, 'y' for the lower and
-        upper limits on the y coordinate, and 'z' for the lower and upper
-        limits on the z coordinate, all given as a list or ndarray with two
-        entries. Must cover at least the dimensions given in start and end.
-
-
-    Returns
-    -------
-    re_box : list of ndarrays
-        The coordinates of the reflection points on the box limits. The list
-        contains n elements and each element is a 2D ndarray with the
-        coordinates.
-    final : ndarray
-        The coordinates of the final end points after all reflections. Has the
-        same shape like start and end.
-
-    """
-    # The datapoints defining the lines to be reflected
-    start = np.asarray(start, dtype='float')
-    end = np.asarray(end, dtype='float')
-    if start.shape == end.shape:
-        dimensions = start.shape[1]
-    else:
-        raise ValueError(
-            'Arrays for start and end point must have the same shapes.')
-
-    # characteristics of the datapoints defining the lines to be reflected
-    # on the borders of the allowed space
-    point_diff = end - start
-    direction = np.sign(point_diff).astype('int')
-
-    # characteristics of the box limiting the allowed space
-    limits = np.array([limits[ii] for ii in ['x', 'y', 'z'][:dimensions]]).T
-    box_diff = np.zeros(dimensions)
-    for curr_dim in range(dimensions):
-        if np.all(limits[:, curr_dim]):
-            box_diff[curr_dim] = np.abs(
-                limits[1, curr_dim] - limits[0, curr_dim])
-            if box_diff[curr_dim] == 0:
-                raise ValueError(
-                    'Upper and lower limits for dimension {} are equal. '
-                    'They must be different or one or both must be None.'
-                    ''.format(curr_dim+1))
-        if np.any((start[:, curr_dim] > limits[1, curr_dim]) |
-                  (start[:, curr_dim] < limits[0, curr_dim])):
-            raise ValueError(
-                'At least one of the start points is not within the '
-                'limits.')
-
-    # coordinates of the reflection points and the coordinate limit that
-    # causes reflection
-    reflect = [[[] for _ in range(dimensions)]
-               for _ in range(start.shape[0])]
-    reflect_type = [[] for _ in range(start.shape[0])]
-
-    # calculate the intersection of the line between the points with the
-    # lines of a grid formed by repeating the box limiting the allowed
-    # space. This gives the coordinates of reflection points.
-    for ii in range(dimensions):
-        # if box_diff[ii] > 0:
-        n = np.abs(direction[:, ii]) * (1/2*direction[:, ii]+1/2).astype(
-            'int')
-        grid = limits[0, ii] + n*box_diff[ii]
-        for curr_point in range(start.shape[0]):
-            while ((grid[curr_point] < end[curr_point, ii]) &
-                   (direction[curr_point, ii] == 1) or
-                   (grid[curr_point] > end[curr_point, ii]) &
-                   (direction[curr_point, ii] == -1)):
-                lambd = ((grid[curr_point] - end[curr_point, ii]) /
-                         point_diff[curr_point, ii])
-                for jj in range(dimensions):
-                    if jj != ii:
-                        reflect[curr_point][jj].append(
-                            end[curr_point, jj] +
-                            lambd*point_diff[curr_point, jj])
-                    else:
-                        reflect[curr_point][ii].append(grid[curr_point])
-                reflect_type[curr_point].append(ii)
-                n[curr_point] += direction[curr_point, ii]
-                grid[curr_point] = (limits[0, ii] +
-                                    n[curr_point]*box_diff[ii])
-
-    # sort the reflection coordinates
-    sort_idx = [
-        np.argsort(reflect[curr_point][0])[::direction[curr_point, 0]]
-        for curr_point in range(start.shape[0])]
-    reflect = [[np.array(reflect[curr_point][ii])[sort_idx[curr_point]]
-                for ii in range(dimensions)]
-               for curr_point in range(start.shape[0])]
-    reflect_type = [
-        np.array(reflect_type[curr_point])[sort_idx[curr_point]]
-        for curr_point in range(start.shape[0])]
-
-    # Calculate the reflection points on the box faces
-    re_box = [[reflect[curr_point][ii].copy() for ii in range(dimensions)]
-              for curr_point in range(start.shape[0])]
-    for curr_point in range(start.shape[0]):
-        if reflect[curr_point][0].size != 0:
-            for ii, r_type in enumerate(reflect_type[curr_point][:-1]):
-                re_box[curr_point][r_type][ii+1:] = -(
-                    re_box[curr_point][r_type][ii+1:] -
-                    re_box[curr_point][r_type][ii]
-                    ) + re_box[curr_point][r_type][ii]
-
-    re_box = [np.array(curr_re_box) for curr_re_box in re_box]
-
-    # calculate the final coordinates
-    final = np.zeros_like(start)
-    for curr_point in range(start.shape[0]):
-        if reflect_type[curr_point].size != 0:
-            for ii in range(dimensions):
-                if any(reflect_type[curr_point] == ii):
-                    coords = re_box[curr_point][ii][
-                        reflect_type[curr_point] == ii]
-                    rest = abs(point_diff[curr_point, ii]) - (
-                        (reflect_type[curr_point] == ii).sum()-1
-                        )*box_diff[ii] - abs(
-                            start[curr_point, ii]-coords[0])
-                    if coords[-1] == limits[0, ii]:
-                        final[curr_point, ii] = limits[0, ii] + rest
-                    else:
-                        final[curr_point, ii] = limits[1, ii] - rest
-                else:
-                    final[curr_point, ii] = end[curr_point, ii]
-
-    return (re_box, final)
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Jan 27 19:12:39 2022
+
+@author: Alexander Southan
+"""
+
+import numpy as np
+from matplotlib.patches import Polygon
+
+
+def point_inside_circle(
+        x_values, y_values, z_values=None, x_c=0, y_c=0, z_c=None, r=1):
+    """
+    Calculate if a set of points is inside a circle.
+
+    The circle can be 2D or 3D (a sphere). This function could be easily
+    adapted to be usable for n-dimensional spheres.
+
+    Parameters
+    ----------
+    x_values : float or ndarray
+        The x coordinates of the points.
+    y_values : float or ndarray
+        The y coordinates of the points. Must have the same length like
+        x_values.
+    z_values : float or ndarray, optional
+        The z coordinates of the points. Must have the same length like
+        x_values. The default is None so that calculations are done in 2D.
+    x_c : float, optional
+        The x coordinate of the circle center. The default is 0.
+    y_c : float, optional
+        The y coordinate of the circle center. The default is 0.
+    z_c : float or None, optional
+        The z coordinate of the circle center. Default is None so that
+        calculations are done in 2D.
+    r : float, optinal
+        The radius of the circle. The default is 1.
+
+    Returns
+    -------
+    bool or ndarray
+        A boolean or an array of booleans stating if the points are within the
+        circle. Has the same shape like x_values and y_values.
+
+    """
+    if (z_c is None) or (z_values is None):
+        params = np.asarray([x_values-x_c, y_values-y_c])
+    else:
+        params = np.asarray([x_values-x_c, y_values-y_c, z_values-z_c])
+
+    return ((params)**2).sum(axis=0) <= r**2
+
+
+def point_inside_polygon(x_values, y_values, polygon_x, polygon_y):
+    """
+    Calculate if a set of points is inside a polygon.
+
+    This function works fully in 2D, so the corresponding matplotlib method
+    can be used directly, making the code very short.
+
+    Parameters
+    ----------
+    x_values : float or ndarray
+        The x coordinates of the points.
+    y_values : float or ndarray
+        The y coordinates of the points. Must have the same length like
+        x_values.
+    polygon_x : ndarray
+        An array with n elements, giving the x coordinates of the n points that
+        form the polygon.
+    polygon_y : ndarray
+        An array with n elements, giving the y coordinates of the n points that
+        form the polygon.
+
+    Returns
+    -------
+    bool or ndarray
+        A boolean or an array of booleans stating if the points are within the
+        polygon. Has the same shape like x_values and y_values.
+
+    """
+    coords = np.asarray([x_values, y_values]).T
+    polygon = Polygon(np.array([polygon_x, polygon_y]).T, closed=True)
+    return polygon.contains_points(coords)
+
+
+def point_inside_cartesianbox(
+        x_values, y_values=None, z_values=None, x_limits=[-1, 1],
+        y_limits=[-1, 1], z_limits=[-1, 1]):
+    """
+    Calculate if points are inside of a cartesian box.
+
+    The cartesian box can be a 1D, 2D or 3D box. The 2D box is a rectangle and
+    the 3D box a rectangular prism.
+
+    Parameters
+    ----------
+    x_values : float or ndarray
+        The x coordinates of the points.
+    y_values : float or ndarray, optional
+        The y coordinates of the points. Must have the same length like
+        x_values. The default is None.
+    z_values : float or ndarray, optional
+        The z coordinates of the points. Must have the same length like
+        x_values. The default is None.
+    x_limits : ndarray or None, optional
+        Contains two elements, first the lower limit and second the upper limit
+        allowed for the x coordinate. Each value can be None, so that the
+        corresponding limit does not exist. The default is [-1, 1].
+    y_limits : ndarray or None, optional
+        Contains two elements, first the lower limit and second the upper limit
+        allowed for the y coordinate. Each value can be None, so that the
+        corresponding limit does not exist. The default is [-1, 1].
+    z_limits : ndarray or None, optional
+        Contains two elements, first the lower limit and second the upper limit
+        allowed for the z coordinate. Each value can be None, so that the
+        corresponding limit does not exist. The default is [-1, 1].
+
+    Returns
+    -------
+    ndarray or bool
+        A boolean ndarray or a signle boolean value in the shape of x_values,
+        stating if the points are within the box or not.
+
+    """
+    if (y_values is None) and (z_values is None):
+        dims = 1
+    elif z_values is None:
+        dims = 2
+    else:
+        dims = 3
+
+    limits = np.asarray([curr_lims for curr_lims
+                         in [x_limits, y_limits, z_limits][:dims]])
+    coords = np.asarray([curr_coords for curr_coords in
+                         [x_values, y_values, z_values][:dims]])
+
+    inside_box = np.empty_like(coords, dtype='bool')
+
+    for curr_idx, (curr_values, curr_limits) in enumerate(zip(coords, limits)):
+        if (curr_limits is None) or (curr_limits[0] is None):
+            below_lower = np.full_like(curr_values, False, dtype='bool')
+        else:
+            below_lower = curr_values < curr_limits[0]
+
+        if (curr_limits is None) or (curr_limits[1] is None):
+            above_upper = np.full_like(curr_values, False, dtype='bool')
+        else:
+            above_upper = curr_values > curr_limits[1]
+
+        inside_box[curr_idx] = ~(below_lower | above_upper)
+
+    return np.all(inside_box, axis=0)
+
+
+def line_through_box(x_values, y_values, box={'x': [-1, 1], 'y': [-1, 1]}):
+    """
+    Calculate if a line defined by two points passes through a rectangular box.
+
+    The two points define an endless line in two dimensions and it is
+    calculated if this endless line travels through the box. So it is totally
+    irrelevant where exactly the two points are.
+
+    Parameters
+    ----------
+    x_values : list or ndarray
+        A list containing two values which are the x coodinates of the two
+        data points.
+    y_values : list or ndarray
+        A list containing two values which are the y coodinates of the two
+        data points.
+    box : dict, optional
+        A dictionary containing the box limits. Must contain the keys 'x' for
+        the lower and upper limits on the x coordinate and 'y' for the lower
+        and upper limits on the y coordinate, both given as a list or ndarray
+        with two entries. The default is {'x': [-1, 1], 'y': [-1, 1]}.
+
+    Returns
+    -------
+    float
+        The distance the line travels through the box.
+    list
+        The two x coordinates where the line intersects the box walls.
+    list
+        The two y coordinates where the line intersects the box walls.
+
+    """
+    slope = (y_values[1]-y_values[0])/(x_values[1]-x_values[0])
+    intercept = y_values[0] - slope*x_values[0]
+
+    if slope != 0:
+        intersect_x = np.sort((box['y']-intercept)/slope)
+        overlap_x = [max(intersect_x[0], box['x'][0]),
+                     min(intersect_x[1], box['x'][1])]
+        overlap_x = overlap_x if overlap_x[0] < overlap_x[1] else []
+    else:
+        if ((y_values[0] > box['y'][0]) & (y_values[0] < box['y'][1])):
+            overlap_x = box['x']
+        else:
+            overlap_x = []
+
+    if overlap_x:
+        overlap_y = [slope*curr_x+intercept for curr_x in overlap_x]
+        score = np.sqrt((overlap_x[1]-overlap_x[0])**2 +
+                        (overlap_y[1]-overlap_y[0])**2)
+        return (score, overlap_x, overlap_y)
+    else:
+        return (0, [], [])
+
+
+def reflect_line_in_box(start, end, limits):
+    """
+    Reflect a line defined by two points within a one- to threedimensional box.
+
+    Parameters
+    ----------
+    start : 2D ndarray
+        The start points of the lines to be reflected. Must be a 2D array with
+        the shape (n, d) where n is the number of data points and d is the
+        dimension (between 1 and 3).
+    end : 2D ndarray
+        The end points of the lines to be reflected. Must be a 2D array with
+        the shape (n, d) where n is the number of data points and d is the
+        dimension (between 1 and 3).
+    limits : dict
+        A dictionary containing the box limits. Cancontain the keys 'x' for
+        the lower and upper limits on the x coordinate, 'y' for the lower and
+        upper limits on the y coordinate, and 'z' for the lower and upper
+        limits on the z coordinate, all given as a list or ndarray with two
+        entries. Must cover at least the dimensions given in start and end.
+
+
+    Returns
+    -------
+    re_box : list of ndarrays
+        The coordinates of the reflection points on the box limits. The list
+        contains n elements and each element is a 2D ndarray with the
+        coordinates.
+    final : ndarray
+        The coordinates of the final end points after all reflections. Has the
+        same shape like start and end.
+
+    """
+    # The datapoints defining the lines to be reflected
+    start = np.asarray(start, dtype='float')
+    end = np.asarray(end, dtype='float')
+    if start.shape == end.shape:
+        dimensions = start.shape[1]
+    else:
+        raise ValueError(
+            'Arrays for start and end point must have the same shapes.')
+
+    # characteristics of the datapoints defining the lines to be reflected
+    # on the borders of the allowed space
+    point_diff = end - start
+    direction = np.sign(point_diff).astype('int')
+
+    # characteristics of the box limiting the allowed space
+    limits = np.array([limits[ii] for ii in ['x', 'y', 'z'][:dimensions]]).T
+    box_diff = np.zeros(dimensions)
+    for curr_dim in range(dimensions):
+        if np.all(limits[:, curr_dim]):
+            box_diff[curr_dim] = np.abs(
+                limits[1, curr_dim] - limits[0, curr_dim])
+            if box_diff[curr_dim] == 0:
+                raise ValueError(
+                    'Upper and lower limits for dimension {} are equal. '
+                    'They must be different or one or both must be None.'
+                    ''.format(curr_dim+1))
+        if np.any((start[:, curr_dim] > limits[1, curr_dim]) |
+                  (start[:, curr_dim] < limits[0, curr_dim])):
+            raise ValueError(
+                'At least one of the start points is not within the '
+                'limits.')
+
+    # coordinates of the reflection points and the coordinate limit that
+    # causes reflection
+    reflect = [[[] for _ in range(dimensions)]
+               for _ in range(start.shape[0])]
+    reflect_type = [[] for _ in range(start.shape[0])]
+
+    # calculate the intersection of the line between the points with the
+    # lines of a grid formed by repeating the box limiting the allowed
+    # space. This gives the coordinates of reflection points.
+    for ii in range(dimensions):
+        # if box_diff[ii] > 0:
+        n = np.abs(direction[:, ii]) * (1/2*direction[:, ii]+1/2).astype(
+            'int')
+        grid = limits[0, ii] + n*box_diff[ii]
+        for curr_point in range(start.shape[0]):
+            while ((grid[curr_point] < end[curr_point, ii]) &
+                   (direction[curr_point, ii] == 1) or
+                   (grid[curr_point] > end[curr_point, ii]) &
+                   (direction[curr_point, ii] == -1)):
+                lambd = ((grid[curr_point] - end[curr_point, ii]) /
+                         point_diff[curr_point, ii])
+                for jj in range(dimensions):
+                    if jj != ii:
+                        reflect[curr_point][jj].append(
+                            end[curr_point, jj] +
+                            lambd*point_diff[curr_point, jj])
+                    else:
+                        reflect[curr_point][ii].append(grid[curr_point])
+                reflect_type[curr_point].append(ii)
+                n[curr_point] += direction[curr_point, ii]
+                grid[curr_point] = (limits[0, ii] +
+                                    n[curr_point]*box_diff[ii])
+
+    # sort the reflection coordinates
+    sort_idx = [
+        np.argsort(reflect[curr_point][0])[::direction[curr_point, 0]]
+        for curr_point in range(start.shape[0])]
+    reflect = [[np.array(reflect[curr_point][ii])[sort_idx[curr_point]]
+                for ii in range(dimensions)]
+               for curr_point in range(start.shape[0])]
+    reflect_type = [
+        np.array(reflect_type[curr_point])[sort_idx[curr_point]]
+        for curr_point in range(start.shape[0])]
+
+    # Calculate the reflection points on the box faces
+    re_box = [[reflect[curr_point][ii].copy() for ii in range(dimensions)]
+              for curr_point in range(start.shape[0])]
+    for curr_point in range(start.shape[0]):
+        if reflect[curr_point][0].size != 0:
+            for ii, r_type in enumerate(reflect_type[curr_point][:-1]):
+                re_box[curr_point][r_type][ii+1:] = -(
+                    re_box[curr_point][r_type][ii+1:] -
+                    re_box[curr_point][r_type][ii]
+                    ) + re_box[curr_point][r_type][ii]
+
+    re_box = [np.array(curr_re_box) for curr_re_box in re_box]
+
+    # calculate the final coordinates
+    final = np.zeros_like(start)
+    for curr_point in range(start.shape[0]):
+        if reflect_type[curr_point].size != 0:
+            for ii in range(dimensions):
+                if any(reflect_type[curr_point] == ii):
+                    coords = re_box[curr_point][ii][
+                        reflect_type[curr_point] == ii]
+                    rest = abs(point_diff[curr_point, ii]) - (
+                        (reflect_type[curr_point] == ii).sum()-1
+                        )*box_diff[ii] - abs(
+                            start[curr_point, ii]-coords[0])
+                    if coords[-1] == limits[0, ii]:
+                        final[curr_point, ii] = limits[0, ii] + rest
+                    else:
+                        final[curr_point, ii] = limits[1, ii] - rest
+                else:
+                    final[curr_point, ii] = end[curr_point, ii]
+
+    return (re_box, final)
```

### Comparing `little_helpers-0.0.5/src/little_helpers/hydrogel_conversions.py` & `little_helpers-0.0.6/src/little_helpers/hydrogel_conversions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Sep 23 20:24:31 2021
-
-@author: Alexander Southan
-"""
-
-import numpy as np
-
-
-def eds_to_volume_fraction(eds, rho_polymer=1, rho_swelling=1,
-                           eds_mode='subtracted', output='polymer'):
-    """
-    Equilibrium degree of swelling to polymer or solvent volume fraction.
-
-    Additivity of volumes is assumed, i.e. there is no volume contraction or
-    other similar mixing effects during swelling.
-
-    Parameters
-    ----------
-    eds : float or ndarray
-        The measured equilibrium degree(s) of swelling. Can be a float for a
-        single value or an ndarray for multiple values.
-    rho_polymer : float, optional
-        The density of the polymer in the dry state. The default is 1.
-    rho_h2o : float, optional
-        The density of the swelling medium. The default is 1.
-    eds_mode : string, optional
-        The way the eds was calculated.
-        'subtracted' means:
-            eds = (swollen_mass-dry_mass)/dry_mass
-        'plain' means:
-            eds = swollen_mass/dry_mass
-        The default is 'subtracted'.
-    output : string, optional
-        The value that will be returned. With 'polymer', the polymer volume
-        fraction will be returned, with 'solvent' the volume fraction of the
-        swelling medium. The default is 'polymer'.
-
-    Returns
-    -------
-    float or ndarray
-        The polymer volume fraction in the swollen material.
-
-    """
-    eds = np.asarray(eds)
-
-    if eds_mode == 'subtracted':
-        eds = eds
-    elif eds_mode == 'plain':
-        eds = eds.copy() - 1
-    else:
-        raise ValueError('No valid value for eds_mode given.')
-
-    v_2s = 1/(eds*rho_swelling/rho_polymer+1)
-    if output == 'polymer':
-        return v_2s
-    elif output == 'solvent':
-        return 1-v_2s
-    else:
-        raise ValueError('No valid value for output given.')
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Sep 23 20:24:31 2021
+
+@author: Alexander Southan
+"""
+
+import numpy as np
+
+
+def eds_to_volume_fraction(eds, rho_polymer=1, rho_swelling=1,
+                           eds_mode='subtracted', output='polymer'):
+    """
+    Equilibrium degree of swelling to polymer or solvent volume fraction.
+
+    Additivity of volumes is assumed, i.e. there is no volume contraction or
+    other similar mixing effects during swelling.
+
+    Parameters
+    ----------
+    eds : float or ndarray
+        The measured equilibrium degree(s) of swelling. Can be a float for a
+        single value or an ndarray for multiple values.
+    rho_polymer : float, optional
+        The density of the polymer in the dry state. The default is 1.
+    rho_h2o : float, optional
+        The density of the swelling medium. The default is 1.
+    eds_mode : string, optional
+        The way the eds was calculated.
+        'subtracted' means:
+            eds = (swollen_mass-dry_mass)/dry_mass
+        'plain' means:
+            eds = swollen_mass/dry_mass
+        The default is 'subtracted'.
+    output : string, optional
+        The value that will be returned. With 'polymer', the polymer volume
+        fraction will be returned, with 'solvent' the volume fraction of the
+        swelling medium. The default is 'polymer'.
+
+    Returns
+    -------
+    float or ndarray
+        The polymer volume fraction in the swollen material.
+
+    """
+    eds = np.asarray(eds)
+
+    if eds_mode == 'subtracted':
+        eds = eds
+    elif eds_mode == 'plain':
+        eds = eds.copy() - 1
+    else:
+        raise ValueError('No valid value for eds_mode given.')
+
+    v_2s = 1/(eds*rho_polymer/rho_swelling+1)
+    if output == 'polymer':
+        return v_2s
+    elif output == 'solvent':
+        return 1-v_2s
+    else:
+        raise ValueError('No valid value for output given.')
```

### Comparing `little_helpers-0.0.5/src/little_helpers/math_functions.py` & `little_helpers-0.0.6/src/little_helpers/math_functions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,506 +1,506 @@
-# -*- coding: utf-8 -*-
-
-import numpy as np
-from scipy import integrate
-from scipy.special import erf
-
-from .array_tools import segment_xy_values
-
-def langmuir_isotherm(c_e, q_m, K_s):
-    """
-    Calculate the q_e values of a Langmuir isotherm.
-
-    Parameters
-    ----------
-    c_e : ndarray
-        The equilibrium concentrations in the liquid phase. Can have any shape,
-        so an (M, N) array may be interpreted as M data rows with N data
-        points.
-    q_m : float
-        The adsorption capacity of the adsorber.
-    K_s : float
-        The equilibrium constant of adsorption and desorption.
-
-    Returns
-    -------
-    ndarray
-        The equilibrium concentrations q_e in the adsorber. Has the same shape
-        like c_e.
-
-    """
-    c_e = np.asarray(c_e)
-
-    return q_m * c_e * K_s/(1 + c_e * K_s)
-
-def langmuir_isotherm_hydrogel(c_e, q_m, K_s, phi_h2o, rho_hydrogel=1):
-    """
-    Calculate the a_e values of a Langmuir isotherm in a hydrogel.
-
-    Parameters
-    ----------
-    c_e : ndarray
-        The equilibrium concentrations in the liquid phase. Can have any shape,
-        so an (M, N) array may be interpreted as M data rows with N data
-        points. It is assumed that the aqueous phase within the hydrogel has
-        the same concentration like c_e.
-    q_m : float
-        The adsorption capacity of the polymer network within the hydrogel.
-    K_s : float
-        The equilibrium constant of adsorption and desorption.
-    phi_h2o : float
-        The volume fraction of water inside the hydrogel.
-    rho_hydrogel : float, optional
-        The density of the hydrogel in g/mL. The default is 1.
-
-    Returns
-    -------
-        The equilibrium concentrations a_e in the adsorber. Has the same shape
-        like c_e.
-
-    """
-    c_e = np.asarray(c_e)
-
-    return c_e*phi_h2o/rho_hydrogel + q_m * c_e * K_s/(1 + c_e * K_s)
-
-def langmuir_comp(c_e_1, c_e_2, q_m, K_s_1, K_s_2):
-    """
-    Calculate the q_e values of a Langmuir isotherm for competitive adsorption.
-
-    Parameters
-    ----------
-    c_e_1 : ndarray
-        The equilibrium concentrations of adsorbat 1 in the liquid phase. Can 
-        have any shape,so an (M, N) array may be interpreted as M data rows
-        with N data points.
-    c_e_2 : ndarray
-        The equilibrium concentrations of adsorbat 2 in the liquid phase. Can 
-        have any shape,so an (M, N) array may be interpreted as M data rows
-        with N data points.
-    q_m : float
-        The adsorption capacity of the adsorber.
-    K_s_1 : float
-        The equilibrium constant of adsorption and desorption of adsorbat 1.
-    K_s_2 : float
-        The equilibrium constant of adsorption and desorption of adsorbat 2.
-
-    Returns
-    -------
-    ndarray
-        The equilibrium concentrations q_e in the adsorber. Has the same shape
-        like c_e.
-
-    """
-    c_e_1 = np.asarray(c_e_1)
-    c_e_2 = np.asarray(c_e_2)
-
-    return q_m * c_e_1 * K_s_1/(1 + c_e_1 * K_s_1 + c_e_2 * K_s_2)
-
-def langmuir_comp_hydrogel(
-        c_e_1, c_e_2, q_m, K_s_1, K_s_2, phi_h2o, rho_hydrogel=1):
-    """
-    Calculate the q_e values of a Langmuir isotherm for competitive adsorption.
-
-    Contains an extra term that takes the free water in the hydrogel into
-    account.
-
-    Parameters
-    ----------
-    c_e_1 : ndarray
-        The equilibrium concentrations of adsorbat 1 in the liquid phase. Can 
-        have any shape,so an (M, N) array may be interpreted as M data rows
-        with N data points.
-    c_e_2 : ndarray
-        The equilibrium concentrations of adsorbat 2 in the liquid phase. Can 
-        have any shape,so an (M, N) array may be interpreted as M data rows
-        with N data points.
-    q_m : float
-        The adsorption capacity of the adsorber.
-    K_s_1 : float
-        The equilibrium constant of adsorption and desorption of adsorbat 1.
-    K_s_2 : float
-        The equilibrium constant of adsorption and desorption of adsorbat 2.
-    phi_h2o : float
-        The volume fraction of water inside the hydrogel.
-    rho_hydrogel : float, optional
-        The density of the hydrogel in g/mL. The default is 1.
-
-    Returns
-    -------
-    ndarray
-        The equilibrium concentrations q_e in the adsorber. Has the same shape
-        like c_e.
-
-    """
-    c_e_1 = np.asarray(c_e_1)
-    c_e_2 = np.asarray(c_e_2)
-
-    return (c_e_1*phi_h2o/rho_hydrogel +
-            q_m * c_e_1 * K_s_1/(1 + c_e_1 * K_s_1 + c_e_2 * K_s_2))
-
-def conductivity_hydrogel(c_e_1, c_e_2, sigma0, m1, m2, qm1, qm2, ks1_1, ks1_2,
-                          ks2_1, ks2_2, phi_h2o, rho_hydrogel):
-    c_e_1 = np.asarray(c_e_1)
-    c_e_2 = np.asarray(c_e_2)
-
-    sigma = (sigma0 +
-             m1 * langmuir_comp_hydrogel(
-                 c_e_1, c_e_2, qm1, ks1_1, ks1_2, phi_h2o,
-                 rho_hydrogel=rho_hydrogel) + 
-             m2 * langmuir_comp_hydrogel(
-                 c_e_2, c_e_1, qm2, ks2_1, ks2_2, phi_h2o,
-                 rho_hydrogel=rho_hydrogel))
-
-    return sigma
-
-def triangle(x, start_left, start_right, x_max, y_max, y_offset=0):
-    """
-    Calculate a triangle function. 
-    
-    The triangle function is zero outside of the triangle and different slopes
-    on both sides of the triangle are possible.
-
-    Parameters
-    ----------
-    x : ndarray
-        The x values used for the calculation. Can be any shape, but the
-        triangle will always be produced in the last dimension. An (M, N) array
-        can therefore be interpreted as M data rows with potentially different
-        x values while the triangles are always created at the same x values.
-    start_left : float
-        The x value where the triangle starts, i.e. the left edge of the
-        tiangle.
-    start_right : float
-        The x value where the triangle stops, i.e. the right edge of the
-        triangle.
-    x_max : float
-        The x value of the triangle maximum/minimum, must be between start_left
-        and start_right, otherwise odd results will occur.
-    y_max : float
-        The y value of the triangle maximum/minimum.
-    y_offset : float, optional
-        The y value outside of the triangle. Default is 0. If y_offset is
-        greater than y_max, the triangle will point downwards, otherwise
-        upwards.
-
-    Returns
-    -------
-    triangle : ndarray
-        An array containing the funtion values of the triangle functions. Has
-        the same shape like x.
-
-    """
-    x = np.asarray(x)
-
-    left_mask = np.logical_and(
-        x >= min(start_left, x_max),
-        x <= max(start_left, x_max))
-    right_mask = np.logical_and(
-        x > min(x_max, start_right),
-        x <= max(x_max, start_right))
-
-    left_slope = (y_max-y_offset)/(x_max - start_left)
-    right_slope = -(y_max-y_offset)/(start_right - x_max)
-
-    triangle = np.full_like(x, y_offset, dtype='float')
-    triangle[left_mask] += left_slope * (x[left_mask] - start_left)
-    triangle[right_mask] += right_slope * (x[right_mask] - start_right)
-    return triangle
-
-def gaussian(x, amp, x_offset, y_offset, sigma):
-    """
-    Calculate one or a superposition of Gaussian normal distributions.
-
-    Parameters
-    ----------
-    x : ndarray
-        A one-dimensional array with the x values used for calculations.
-    amp : float or list of float
-        The amplitudes, i.e. the maximum values of the calculated Gauss curve.
-        If a single value is given, a single peak is created. If a list of
-        values is given, a superposition of several Gauss curves will be
-        calculated.
-    x_offset : float or list of float
-        The x position of the maximum value defined by amp. Must be the same
-        shape like amp.
-    y_offset : float or list of float
-        The y value of the baseline of the Gauss curve. Must be the same shape
-        like amp.
-    sigma : float or list of float
-        The with of the Gauss curve. The full width at half maximum is given by
-        2*sqrt(2*ln(2))*sigma. Must be the same shape like amp.
-
-    Returns
-    -------
-    ndarray
-        An array containing the function values of the (superimposed) Gauss
-        curves. Has the same shape like x.
-
-    """
-    amp = np.array(amp, ndmin=1)
-    x_offset = np.array(x_offset, ndmin=1)
-    y_offset = np.array(y_offset, ndmin=1)
-    sigma = np.array(sigma, ndmin=1)
-    return np.sum(
-        amp[:, np.newaxis] * np.exp(
-            (x - x_offset[:, np.newaxis])**2 /
-            (-2 * sigma[:, np.newaxis]**2)) +
-        y_offset[:, np.newaxis], axis=0)
-
-def boxcar(x, boxcar_start, boxcar_end, y_offset=0, amp=1):
-    """
-    Calculate a boxcar function.
-
-    The boxcar function has a constant value inside the box and another value,
-    typically zero, outside of the box.
-
-    Parameters
-    ----------
-    x : ndarray
-        A one-dimensional array with the x values used for calculations.
-    boxcar_start : float
-        The left edge value of the box, must be smaller than boxcar_end.
-    boxcar_end : float
-        The right edge value of the box, must be greater than boxcar_start.
-    y_offset : float, optional
-        The value of the boxcar function outside of the box. The default is 0.
-    amp : float, optional
-        The value of the boxcar function inside the box. The default is 1.
-
-    Returns
-    -------
-    y_boxcar : ndarray
-        An array containing the function values of the boxcar function. Has the
-        same shape like x.
-
-    """
-    x = np.asarray(x)
-
-    boxcar_mask = np.logical_and(
-        x >= min(boxcar_start, boxcar_end),
-        x <= max(boxcar_start, boxcar_end))
-    y_boxcar = np.full_like(x, y_offset)
-    y_boxcar[boxcar_mask] = amp
-    return y_boxcar
-
-def boxcar_convolution(x, boxcar_start, boxcar_end, convolution_function,
-                       con_func_params, y_offset=0):
-    """
-    Calculate a convolution of a boxcar function and another function.
-
-    This useful for example to estimate the intensity distribution when a
-    Gaussian focus is moved through a layer with constant thickness, e.g. in
-    confocal fluorescence or Raman microscopy. In this case,
-    concolution_function would be gaussian.
-
-    Parameters
-    ----------
-    x : ndarray
-        A one-dimensional array with the x values used for calculations.
-    boxcar_start : float
-        The left edge value of the box, must be smaller than boxcar_end.
-    boxcar_end : float
-        The right edge value of the box, must be greater than boxcar_start.
-    convolution_function : callable
-        A callable function that takes x as the first parameter and
-        con_func_params as additional arguments.
-    con_func_params : list of float
-        Additional parameters passed to convolution_function.
-    y_offset : float, optional
-        The value the convoluted function is shifted upwards after calculation.
-        The default is 0.
-
-    Returns
-    -------
-    function_values : ndarray
-        An array containing the function values of the convoluted function.
-        Has the same shape like x.
-
-    """
-    x_spacing = np.abs(x[1]-x[0])
-    x_min = x[0]
-    x_max = x[-1]
-    boxcar_width = abs(boxcar_start - boxcar_end)
-
-    x_addition_datapoints = np.around(
-        boxcar_width/(2*x_spacing)).astype(np.uint32)
-    x_addition = x_addition_datapoints * x_spacing
-    x_min_convolution = x_min - x_addition
-    x_max_convolution = x_max + x_addition
-
-    x_values_convolution = np.arange(
-        x_min_convolution, x_max_convolution+x_spacing/2, x_spacing)
-
-    y_con_func = convolution_function(x_values_convolution, *con_func_params)
-    y_con_func_integral = integrate.cumtrapz(y_con_func, x_values_convolution,
-                                             initial=0)
-
-    function_values = (y_con_func_integral[2*x_addition_datapoints:] -
-                       y_con_func_integral[
-                           :len(x_values_convolution) -
-                           2*x_addition_datapoints] +
-                       y_offset)
-    return function_values
-
-def piecewise_polynomial(x_values, coefs, segment_borders=[]):
-    """
-    Calculate the y values of a piecewise polynomial.
-
-    Can also calculate a simple polynomial.
-
-    Parameters
-    ----------
-    x_values : ndarray
-        A 1D array with the length M holding the independent varibale used for
-        calculation of the piecewise polynomial.
-    coefs : list of ndarray
-        A list containing the coefficient vectors of the polynomial equations
-        for the data segments. Each list entry must be in a format so that it
-        can be passed directly to np.polynomial.polynomial.polyval to calculate
-        the polynomial values. If segment borders is left at the default value,
-        still a list with only one coefficient vector must be given.
-    segment_borders : list of int or float, optional
-        The values with respect to x_values at which the data is divided into
-        segments. An arbitrary number of segment borders may be given, but it
-        is recommended to provide a sorted list in order to avoid confusion.
-        If the list is not sorted, it will be sorted. The default is [] meaning
-        that only a simple polynomial is calculated.
-
-    Returns
-    -------
-    ndarray
-        The y values of the piecewise polynomial, an array with the same length
-        as x_values.
-
-    """
-
-    segment_borders = np.array(segment_borders, ndmin=1)
-
-    if segment_borders.size > 0:
-        x_segments = segment_xy_values(x_values, segment_borders)
-    else:
-        x_segments = [x_values]
-
-    curve_segments = []
-    for curr_x, curr_coefs in zip(x_segments, coefs):
-        poly_vals = np.polynomial.polynomial.polyval(curr_x, curr_coefs)
-        curve_segments.append(poly_vals
-                              if len(curve_segments) == len(x_segments)-1
-                              else poly_vals[:-1])
-
-    return np.concatenate(curve_segments)
-
-def flory_rehner(v_2s, M_n, v_2r, chi, rho_swelling=1, rho_polymer=1,
-                 molar_mass_swelling=18):
-    """
-    Calculate 1/M_c according to the Flory-Rehner equation.
-
-    Parameters
-    ----------
-    v_2s : ndarray
-        The polymer volume fractions in a hydrogel after swelling to
-        equilibrium.
-    M_n : float
-        Number average molar mass of the polymer before cross-linking.
-    v_2r : float
-        The polymer volume fraction in the hydrogel after cross-linking but
-        before swelling in additional solvent. Often approximated with the
-        polymer volume fraction in the solution state before cross-linking.
-    chi : float
-        The Flory-Huggins interaction parameter for the polymer-solvent pair
-        used.
-    rho_swelling : float, optional
-        The density of the swelling medium in g/mL. Default is 1.
-    rho_polymer : float, optional
-        The density of the polymer in g/mL. Default is 1.
-    molar_mass_swelling : float, optional
-        The molar mass of the swelling medium in g/mol. Default is 18.
-
-    Returns
-    -------
-    ndarray
-        The 1/M_c values of the hydrogels, has the same length like v_2s.
-
-    """
-    v_2s = np.asarray(v_2s)
-
-    return (
-        2/M_n -
-        rho_swelling/rho_polymer/molar_mass_swelling*
-        (np.log(1-v_2s)+v_2s+chi*v_2s**2)/
-        (v_2r*((v_2s/v_2r)**(1/3)-0.5*v_2s/v_2r))
-        )
-
-def Herschel_Bulkley(x, yield_stress, k, n):
-    x = np.asarray(x)
-
-    return yield_stress + k * x**n
-
-def cum_dist_normal(x_values, sigma, x_offset, amp=1):
-    """
-    Cumulative distribution function for the normal distribution.
-
-    Parameters
-    ----------
-    x_values : ndarray
-        The x_values used for the calculation. Can have any shape.
-    sigma : float
-        The standard deviation of the normal distribution.
-    x_offset : float
-        The expected value of the normal distribution.
-    amp : float, optional
-        The amplitude, i.e. the total integral of the normal distribution.
-        The default is 1.
-
-    Returns
-    -------
-    ndarray
-        The cumulative distribution function of a normal distribution. Has the
-        same shape like x_values.
-
-    """
-    x_values = np.asarray(x_values)
-
-    return amp*1/2*(1+erf((x_values-x_offset)/np.sqrt(2*sigma**2)))
-
-def cum_dist_normal_with_rise(x_values, sigma, x_offset, slope, amp=1,
-                              linear_rise='full'):
-    """
-    Superposition of cum_dist_normal and a linear function through the origin.
-
-    Parameters
-    ----------
-    x_values : ndarray
-        The x_values used for the calculation.
-    sigma : float
-        See docstring of cum_dist_normal.
-    x_offset : float
-        See docstring of cum_dist_normal.
-    slope : float
-        The slope of the linear function.
-    amp : float, optional
-        See docstring of cum_dist_normal. The default is 1.
-    linear_rise : string, optional
-        Allowed values are 'full' (linear rise over the entire x_values range),
-        'left' (linear rise only left of x_offset) and 'right' (linear rise
-        only right of x_offset). The default is 'full'.
-
-    Returns
-    -------
-    function_values : ndarray
-        The calculated function values.
-
-    """
-    x_values = np.asarray(x_values)
-
-    function_values = cum_dist_normal(x_values, sigma, x_offset, amp=amp)
-    if linear_rise == 'full':
-        function_values += slope * x_values
-    else:
-        linear_part = np.zeros_like(function_values)
-        if linear_rise == 'left':
-            linear_mask = x_values<=x_offset
-        elif linear_rise == 'right':
-            linear_mask = x_values>=x_offset
-        linear_part[linear_mask] = (x_values[linear_mask]-x_offset)*slope
-        function_values += linear_part
-    return function_values
+# -*- coding: utf-8 -*-
+
+import numpy as np
+from scipy import integrate
+from scipy.special import erf
+
+from .array_tools import segment_xy_values
+
+def langmuir_isotherm(c_e, q_m, K_s):
+    """
+    Calculate the q_e values of a Langmuir isotherm.
+
+    Parameters
+    ----------
+    c_e : ndarray
+        The equilibrium concentrations in the liquid phase. Can have any shape,
+        so an (M, N) array may be interpreted as M data rows with N data
+        points.
+    q_m : float
+        The adsorption capacity of the adsorber.
+    K_s : float
+        The equilibrium constant of adsorption and desorption.
+
+    Returns
+    -------
+    ndarray
+        The equilibrium concentrations q_e in the adsorber. Has the same shape
+        like c_e.
+
+    """
+    c_e = np.asarray(c_e)
+
+    return q_m * c_e * K_s/(1 + c_e * K_s)
+
+def langmuir_isotherm_hydrogel(c_e, q_m, K_s, phi_h2o, rho_hydrogel=1):
+    """
+    Calculate the a_e values of a Langmuir isotherm in a hydrogel.
+
+    Parameters
+    ----------
+    c_e : ndarray
+        The equilibrium concentrations in the liquid phase. Can have any shape,
+        so an (M, N) array may be interpreted as M data rows with N data
+        points. It is assumed that the aqueous phase within the hydrogel has
+        the same concentration like c_e.
+    q_m : float
+        The adsorption capacity of the polymer network within the hydrogel.
+    K_s : float
+        The equilibrium constant of adsorption and desorption.
+    phi_h2o : float
+        The volume fraction of water inside the hydrogel.
+    rho_hydrogel : float, optional
+        The density of the hydrogel in g/mL. The default is 1.
+
+    Returns
+    -------
+        The equilibrium concentrations a_e in the adsorber. Has the same shape
+        like c_e.
+
+    """
+    c_e = np.asarray(c_e)
+
+    return c_e*phi_h2o/rho_hydrogel + q_m * c_e * K_s/(1 + c_e * K_s)
+
+def langmuir_comp(c_e_1, c_e_2, q_m, K_s_1, K_s_2):
+    """
+    Calculate the q_e values of a Langmuir isotherm for competitive adsorption.
+
+    Parameters
+    ----------
+    c_e_1 : ndarray
+        The equilibrium concentrations of adsorbat 1 in the liquid phase. Can 
+        have any shape,so an (M, N) array may be interpreted as M data rows
+        with N data points.
+    c_e_2 : ndarray
+        The equilibrium concentrations of adsorbat 2 in the liquid phase. Can 
+        have any shape,so an (M, N) array may be interpreted as M data rows
+        with N data points.
+    q_m : float
+        The adsorption capacity of the adsorber.
+    K_s_1 : float
+        The equilibrium constant of adsorption and desorption of adsorbat 1.
+    K_s_2 : float
+        The equilibrium constant of adsorption and desorption of adsorbat 2.
+
+    Returns
+    -------
+    ndarray
+        The equilibrium concentrations q_e in the adsorber. Has the same shape
+        like c_e.
+
+    """
+    c_e_1 = np.asarray(c_e_1)
+    c_e_2 = np.asarray(c_e_2)
+
+    return q_m * c_e_1 * K_s_1/(1 + c_e_1 * K_s_1 + c_e_2 * K_s_2)
+
+def langmuir_comp_hydrogel(
+        c_e_1, c_e_2, q_m, K_s_1, K_s_2, phi_h2o, rho_hydrogel=1):
+    """
+    Calculate the q_e values of a Langmuir isotherm for competitive adsorption.
+
+    Contains an extra term that takes the free water in the hydrogel into
+    account.
+
+    Parameters
+    ----------
+    c_e_1 : ndarray
+        The equilibrium concentrations of adsorbat 1 in the liquid phase. Can 
+        have any shape,so an (M, N) array may be interpreted as M data rows
+        with N data points.
+    c_e_2 : ndarray
+        The equilibrium concentrations of adsorbat 2 in the liquid phase. Can 
+        have any shape,so an (M, N) array may be interpreted as M data rows
+        with N data points.
+    q_m : float
+        The adsorption capacity of the adsorber.
+    K_s_1 : float
+        The equilibrium constant of adsorption and desorption of adsorbat 1.
+    K_s_2 : float
+        The equilibrium constant of adsorption and desorption of adsorbat 2.
+    phi_h2o : float
+        The volume fraction of water inside the hydrogel.
+    rho_hydrogel : float, optional
+        The density of the hydrogel in g/mL. The default is 1.
+
+    Returns
+    -------
+    ndarray
+        The equilibrium concentrations q_e in the adsorber. Has the same shape
+        like c_e.
+
+    """
+    c_e_1 = np.asarray(c_e_1)
+    c_e_2 = np.asarray(c_e_2)
+
+    return (c_e_1*phi_h2o/rho_hydrogel +
+            q_m * c_e_1 * K_s_1/(1 + c_e_1 * K_s_1 + c_e_2 * K_s_2))
+
+def conductivity_hydrogel(c_e_1, c_e_2, sigma0, m1, m2, qm1, qm2, ks1_1, ks1_2,
+                          ks2_1, ks2_2, phi_h2o, rho_hydrogel):
+    c_e_1 = np.asarray(c_e_1)
+    c_e_2 = np.asarray(c_e_2)
+
+    sigma = (sigma0 +
+             m1 * langmuir_comp_hydrogel(
+                 c_e_1, c_e_2, qm1, ks1_1, ks1_2, phi_h2o,
+                 rho_hydrogel=rho_hydrogel) + 
+             m2 * langmuir_comp_hydrogel(
+                 c_e_2, c_e_1, qm2, ks2_1, ks2_2, phi_h2o,
+                 rho_hydrogel=rho_hydrogel))
+
+    return sigma
+
+def triangle(x, start_left, start_right, x_max, y_max, y_offset=0):
+    """
+    Calculate a triangle function. 
+    
+    The triangle function is zero outside of the triangle and different slopes
+    on both sides of the triangle are possible.
+
+    Parameters
+    ----------
+    x : ndarray
+        The x values used for the calculation. Can be any shape, but the
+        triangle will always be produced in the last dimension. An (M, N) array
+        can therefore be interpreted as M data rows with potentially different
+        x values while the triangles are always created at the same x values.
+    start_left : float
+        The x value where the triangle starts, i.e. the left edge of the
+        tiangle.
+    start_right : float
+        The x value where the triangle stops, i.e. the right edge of the
+        triangle.
+    x_max : float
+        The x value of the triangle maximum/minimum, must be between start_left
+        and start_right, otherwise odd results will occur.
+    y_max : float
+        The y value of the triangle maximum/minimum.
+    y_offset : float, optional
+        The y value outside of the triangle. Default is 0. If y_offset is
+        greater than y_max, the triangle will point downwards, otherwise
+        upwards.
+
+    Returns
+    -------
+    triangle : ndarray
+        An array containing the funtion values of the triangle functions. Has
+        the same shape like x.
+
+    """
+    x = np.asarray(x)
+
+    left_mask = np.logical_and(
+        x >= min(start_left, x_max),
+        x <= max(start_left, x_max))
+    right_mask = np.logical_and(
+        x > min(x_max, start_right),
+        x <= max(x_max, start_right))
+
+    left_slope = (y_max-y_offset)/(x_max - start_left)
+    right_slope = -(y_max-y_offset)/(start_right - x_max)
+
+    triangle = np.full_like(x, y_offset, dtype='float')
+    triangle[left_mask] += left_slope * (x[left_mask] - start_left)
+    triangle[right_mask] += right_slope * (x[right_mask] - start_right)
+    return triangle
+
+def gaussian(x, amp, x_offset, y_offset, sigma):
+    """
+    Calculate one or a superposition of Gaussian normal distributions.
+
+    Parameters
+    ----------
+    x : ndarray
+        A one-dimensional array with the x values used for calculations.
+    amp : float or list of float
+        The amplitudes, i.e. the maximum values of the calculated Gauss curve.
+        If a single value is given, a single peak is created. If a list of
+        values is given, a superposition of several Gauss curves will be
+        calculated.
+    x_offset : float or list of float
+        The x position of the maximum value defined by amp. Must be the same
+        shape like amp.
+    y_offset : float or list of float
+        The y value of the baseline of the Gauss curve. Must be the same shape
+        like amp.
+    sigma : float or list of float
+        The with of the Gauss curve. The full width at half maximum is given by
+        2*sqrt(2*ln(2))*sigma. Must be the same shape like amp.
+
+    Returns
+    -------
+    ndarray
+        An array containing the function values of the (superimposed) Gauss
+        curves. Has the same shape like x.
+
+    """
+    amp = np.array(amp, ndmin=1)
+    x_offset = np.array(x_offset, ndmin=1)
+    y_offset = np.array(y_offset, ndmin=1)
+    sigma = np.array(sigma, ndmin=1)
+    return np.sum(
+        amp[:, np.newaxis] * np.exp(
+            (x - x_offset[:, np.newaxis])**2 /
+            (-2 * sigma[:, np.newaxis]**2)) +
+        y_offset[:, np.newaxis], axis=0)
+
+def boxcar(x, boxcar_start, boxcar_end, y_offset=0, amp=1):
+    """
+    Calculate a boxcar function.
+
+    The boxcar function has a constant value inside the box and another value,
+    typically zero, outside of the box.
+
+    Parameters
+    ----------
+    x : ndarray
+        A one-dimensional array with the x values used for calculations.
+    boxcar_start : float
+        The left edge value of the box, must be smaller than boxcar_end.
+    boxcar_end : float
+        The right edge value of the box, must be greater than boxcar_start.
+    y_offset : float, optional
+        The value of the boxcar function outside of the box. The default is 0.
+    amp : float, optional
+        The value of the boxcar function inside the box. The default is 1.
+
+    Returns
+    -------
+    y_boxcar : ndarray
+        An array containing the function values of the boxcar function. Has the
+        same shape like x.
+
+    """
+    x = np.asarray(x)
+
+    boxcar_mask = np.logical_and(
+        x >= min(boxcar_start, boxcar_end),
+        x <= max(boxcar_start, boxcar_end))
+    y_boxcar = np.full_like(x, y_offset)
+    y_boxcar[boxcar_mask] = amp
+    return y_boxcar
+
+def boxcar_convolution(x, boxcar_start, boxcar_end, convolution_function,
+                       con_func_params, y_offset=0):
+    """
+    Calculate a convolution of a boxcar function and another function.
+
+    This useful for example to estimate the intensity distribution when a
+    Gaussian focus is moved through a layer with constant thickness, e.g. in
+    confocal fluorescence or Raman microscopy. In this case,
+    concolution_function would be gaussian.
+
+    Parameters
+    ----------
+    x : ndarray
+        A one-dimensional array with the x values used for calculations.
+    boxcar_start : float
+        The left edge value of the box, must be smaller than boxcar_end.
+    boxcar_end : float
+        The right edge value of the box, must be greater than boxcar_start.
+    convolution_function : callable
+        A callable function that takes x as the first parameter and
+        con_func_params as additional arguments.
+    con_func_params : list of float
+        Additional parameters passed to convolution_function.
+    y_offset : float, optional
+        The value the convoluted function is shifted upwards after calculation.
+        The default is 0.
+
+    Returns
+    -------
+    function_values : ndarray
+        An array containing the function values of the convoluted function.
+        Has the same shape like x.
+
+    """
+    x_spacing = np.abs(x[1]-x[0])
+    x_min = x[0]
+    x_max = x[-1]
+    boxcar_width = abs(boxcar_start - boxcar_end)
+
+    x_addition_datapoints = np.around(
+        boxcar_width/(2*x_spacing)).astype(np.uint32)
+    x_addition = x_addition_datapoints * x_spacing
+    x_min_convolution = x_min - x_addition
+    x_max_convolution = x_max + x_addition
+
+    x_values_convolution = np.arange(
+        x_min_convolution, x_max_convolution+x_spacing/2, x_spacing)
+
+    y_con_func = convolution_function(x_values_convolution, *con_func_params)
+    y_con_func_integral = integrate.cumtrapz(y_con_func, x_values_convolution,
+                                             initial=0)
+
+    function_values = (y_con_func_integral[2*x_addition_datapoints:] -
+                       y_con_func_integral[
+                           :len(x_values_convolution) -
+                           2*x_addition_datapoints] +
+                       y_offset)
+    return function_values
+
+def piecewise_polynomial(x_values, coefs, segment_borders=[]):
+    """
+    Calculate the y values of a piecewise polynomial.
+
+    Can also calculate a simple polynomial.
+
+    Parameters
+    ----------
+    x_values : ndarray
+        A 1D array with the length M holding the independent varibale used for
+        calculation of the piecewise polynomial.
+    coefs : list of ndarray
+        A list containing the coefficient vectors of the polynomial equations
+        for the data segments. Each list entry must be in a format so that it
+        can be passed directly to np.polynomial.polynomial.polyval to calculate
+        the polynomial values. If segment borders is left at the default value,
+        still a list with only one coefficient vector must be given.
+    segment_borders : list of int or float, optional
+        The values with respect to x_values at which the data is divided into
+        segments. An arbitrary number of segment borders may be given, but it
+        is recommended to provide a sorted list in order to avoid confusion.
+        If the list is not sorted, it will be sorted. The default is [] meaning
+        that only a simple polynomial is calculated.
+
+    Returns
+    -------
+    ndarray
+        The y values of the piecewise polynomial, an array with the same length
+        as x_values.
+
+    """
+
+    segment_borders = np.array(segment_borders, ndmin=1)
+
+    if segment_borders.size > 0:
+        x_segments = segment_xy_values(x_values, segment_borders)
+    else:
+        x_segments = [x_values]
+
+    curve_segments = []
+    for curr_x, curr_coefs in zip(x_segments, coefs):
+        poly_vals = np.polynomial.polynomial.polyval(curr_x, curr_coefs)
+        curve_segments.append(poly_vals
+                              if len(curve_segments) == len(x_segments)-1
+                              else poly_vals[:-1])
+
+    return np.concatenate(curve_segments)
+
+def flory_rehner(v_2s, M_n, v_2r, chi, rho_swelling=1, rho_polymer=1,
+                 molar_mass_swelling=18):
+    """
+    Calculate 1/M_c according to the Flory-Rehner equation.
+
+    Parameters
+    ----------
+    v_2s : ndarray
+        The polymer volume fractions in a hydrogel after swelling to
+        equilibrium.
+    M_n : float
+        Number average molar mass of the polymer before cross-linking.
+    v_2r : float
+        The polymer volume fraction in the hydrogel after cross-linking but
+        before swelling in additional solvent. Often approximated with the
+        polymer volume fraction in the solution state before cross-linking.
+    chi : float
+        The Flory-Huggins interaction parameter for the polymer-solvent pair
+        used.
+    rho_swelling : float, optional
+        The density of the swelling medium in g/mL. Default is 1.
+    rho_polymer : float, optional
+        The density of the polymer in g/mL. Default is 1.
+    molar_mass_swelling : float, optional
+        The molar mass of the swelling medium in g/mol. Default is 18.
+
+    Returns
+    -------
+    ndarray
+        The 1/M_c values of the hydrogels, has the same length like v_2s.
+
+    """
+    v_2s = np.asarray(v_2s)
+
+    return (
+        2/M_n -
+        rho_swelling/rho_polymer/molar_mass_swelling*
+        (np.log(1-v_2s)+v_2s+chi*v_2s**2)/
+        (v_2r*((v_2s/v_2r)**(1/3)-0.5*v_2s/v_2r))
+        )
+
+def Herschel_Bulkley(x, yield_stress, k, n):
+    x = np.asarray(x)
+
+    return yield_stress + k * x**n
+
+def cum_dist_normal(x_values, sigma, x_offset, amp=1):
+    """
+    Cumulative distribution function for the normal distribution.
+
+    Parameters
+    ----------
+    x_values : ndarray
+        The x_values used for the calculation. Can have any shape.
+    sigma : float
+        The standard deviation of the normal distribution.
+    x_offset : float
+        The expected value of the normal distribution.
+    amp : float, optional
+        The amplitude, i.e. the total integral of the normal distribution.
+        The default is 1.
+
+    Returns
+    -------
+    ndarray
+        The cumulative distribution function of a normal distribution. Has the
+        same shape like x_values.
+
+    """
+    x_values = np.asarray(x_values)
+
+    return amp*1/2*(1+erf((x_values-x_offset)/np.sqrt(2*sigma**2)))
+
+def cum_dist_normal_with_rise(x_values, sigma, x_offset, slope, amp=1,
+                              linear_rise='full'):
+    """
+    Superposition of cum_dist_normal and a linear function through the origin.
+
+    Parameters
+    ----------
+    x_values : ndarray
+        The x_values used for the calculation.
+    sigma : float
+        See docstring of cum_dist_normal.
+    x_offset : float
+        See docstring of cum_dist_normal.
+    slope : float
+        The slope of the linear function.
+    amp : float, optional
+        See docstring of cum_dist_normal. The default is 1.
+    linear_rise : string, optional
+        Allowed values are 'full' (linear rise over the entire x_values range),
+        'left' (linear rise only left of x_offset) and 'right' (linear rise
+        only right of x_offset). The default is 'full'.
+
+    Returns
+    -------
+    function_values : ndarray
+        The calculated function values.
+
+    """
+    x_values = np.asarray(x_values)
+
+    function_values = cum_dist_normal(x_values, sigma, x_offset, amp=amp)
+    if linear_rise == 'full':
+        function_values += slope * x_values
+    else:
+        linear_part = np.zeros_like(function_values)
+        if linear_rise == 'left':
+            linear_mask = x_values<=x_offset
+        elif linear_rise == 'right':
+            linear_mask = x_values>=x_offset
+        linear_part[linear_mask] = (x_values[linear_mask]-x_offset)*slope
+        function_values += linear_part
+    return function_values
```

### Comparing `little_helpers-0.0.5/src/little_helpers.egg-info/PKG-INFO` & `little_helpers-0.0.6/src/little_helpers.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,49 @@
-Metadata-Version: 2.1
-Name: little-helpers
-Version: 0.0.5
-Summary: little helper functions
-Home-page: https://github.com/AlexanderSouthan/little_helpers
-Author: Alexander Southan
-Author-email: alexander.southan@web.de
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/little_helpers/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![build workflow](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/AlexanderSouthan/little_helpers/branch/main/graph/badge.svg?token=W7O1I2YKGO)](https://codecov.io/gh/AlexanderSouthan/little_helpers)
-
-# little_helpers
-Some helpful functions that keep being used in various of my repositories, install via:
-```
-pip install little_helpers
-```
-
-## array_tools.py
-* y_at_y: Find values in y_values that belongs to the values in x_values clostest to x.
-* closest_index: Find the index of a value in array x_values that is clostest to x.
-* segment_xy_values: Segment the x_values and y_values according to segment borders.
-
-## math_functions.py
-* langmuir_isotherm: Calculate the q_e values of a simple Langmuir isotherm.
-* langmuir_isotherm_hydrogel: Calculate the adsotpion inside a hydrogel based on a Langmuir model taking the swelling into account.
-* langmuir_comp: Calculate the q_e values of a Langmuir isotherm taking into account competetive adsorption of two species.
-* triangle: Calculate a triangle function.
-* gaussian: Calculate one or a superposition of Gaussian normal distributions.
-* boxcar: Calculate a boxcar function.
-* boxcar_convolution: Calculate the convolution of a boxcar function with another function.
-* piecewise_polynomial: Calculate the y values of a piecewise polynomial.
-* flory_rehner: Calculate 1/M_c according to the Flory-Rehner equation.
-* Herschel_Bulkley: Calculate the stress according tot he Herschel-Bulkley model.
-* cum_dist_normal: Cumulative distribution function for the normal distribution.
-* cum_dist_normal_with_rise: Superposition of cum_dist_normal and a linear function through the origin.
-
-## num_derive.py
-A simple method to calculate the derivative of discrete data.
-
-## statsmodel_wrapper.py
-A universal sklearn-style wrapper for statsmodels regressors.
-
-
+Metadata-Version: 2.1
+Name: little-helpers
+Version: 0.0.6
+Summary: little helper functions
+Home-page: https://github.com/AlexanderSouthan/little_helpers
+Author: Alexander Southan
+Author-email: alexander.southan@web.de
+Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/little_helpers/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![build workflow](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/little_helpers/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/AlexanderSouthan/little_helpers/branch/main/graph/badge.svg?token=W7O1I2YKGO)](https://codecov.io/gh/AlexanderSouthan/little_helpers)
+
+# little_helpers
+Some helpful functions that keep being used in various of my repositories, install via:
+```
+pip install little_helpers
+```
+
+## array_tools.py
+* y_at_y: Find values in y_values that belongs to the values in x_values clostest to x.
+* closest_index: Find the index of a value in array x_values that is clostest to x.
+* segment_xy_values: Segment the x_values and y_values according to segment borders.
+
+## math_functions.py
+* langmuir_isotherm: Calculate the q_e values of a simple Langmuir isotherm.
+* langmuir_isotherm_hydrogel: Calculate the adsotpion inside a hydrogel based on a Langmuir model taking the swelling into account.
+* langmuir_comp: Calculate the q_e values of a Langmuir isotherm taking into account competetive adsorption of two species.
+* triangle: Calculate a triangle function.
+* gaussian: Calculate one or a superposition of Gaussian normal distributions.
+* boxcar: Calculate a boxcar function.
+* boxcar_convolution: Calculate the convolution of a boxcar function with another function.
+* piecewise_polynomial: Calculate the y values of a piecewise polynomial.
+* flory_rehner: Calculate 1/M_c according to the Flory-Rehner equation.
+* Herschel_Bulkley: Calculate the stress according tot he Herschel-Bulkley model.
+* cum_dist_normal: Cumulative distribution function for the normal distribution.
+* cum_dist_normal_with_rise: Superposition of cum_dist_normal and a linear function through the origin.
+
+## num_derive.py
+A simple method to calculate the derivative of discrete data.
+
+## statsmodel_wrapper.py
+A universal sklearn-style wrapper for statsmodels regressors.
```

### Comparing `little_helpers-0.0.5/src/little_helpers.egg-info/SOURCES.txt` & `little_helpers-0.0.6/src/little_helpers.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,8 +11,13 @@
 src/little_helpers/math_to_word.py
 src/little_helpers/num_derive.py
 src/little_helpers/statsmodel_wrapper.py
 src/little_helpers.egg-info/PKG-INFO
 src/little_helpers.egg-info/SOURCES.txt
 src/little_helpers.egg-info/dependency_links.txt
 src/little_helpers.egg-info/requires.txt
-src/little_helpers.egg-info/top_level.txt
+src/little_helpers.egg-info/top_level.txt
+tests/test_array_tools.py
+tests/test_hydrogel_conversions.py
+tests/test_math_functions.py
+tests/test_num_derive.py
+tests/test_statsmodel_wrapper.py
```

