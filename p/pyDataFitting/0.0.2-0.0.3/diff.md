# Comparing `tmp/pyDataFitting-0.0.2.tar.gz` & `tmp/pyDataFitting-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/almami/Alexander/Python_Skripte/00_packages/pyDataFitting/dist/tmpv24aexqv/pyDataFitting-0.0.2.tar", last modified: Wed Dec  1 18:37:03 2021, max compression
+gzip compressed data, was "pyDataFitting-0.0.3.tar", last modified: Fri Apr 14 12:37:04 2023, max compression
```

## Comparing `pyDataFitting-0.0.2.tar` & `pyDataFitting-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/
--rw-rw-r--   0 almami    (1000) almami    (1000)     1074 2021-10-18 20:58:37.000000 pyDataFitting-0.0.2/LICENSE
--rw-rw-r--   0 almami    (1000) almami    (1000)     4783 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/PKG-INFO
--rw-rw-r--   0 almami    (1000) almami    (1000)     4204 2021-11-06 19:01:14.000000 pyDataFitting-0.0.2/README.md
--rw-rw-r--   0 almami    (1000) almami    (1000)      104 2021-10-18 20:58:37.000000 pyDataFitting-0.0.2/pyproject.toml
--rw-rw-r--   0 almami    (1000) almami    (1000)      667 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/setup.cfg
--rw-rw-r--   0 almami    (1000) almami    (1000)      256 2021-12-01 18:36:39.000000 pyDataFitting-0.0.2/setup.py
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/src/
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/src/pyDataFitting/
--rw-rw-r--   0 almami    (1000) almami    (1000)      165 2021-10-18 20:58:37.000000 pyDataFitting-0.0.2/src/pyDataFitting/__init__.py
--rw-rw-r--   0 almami    (1000) almami    (1000)     4067 2021-10-18 20:58:37.000000 pyDataFitting-0.0.2/src/pyDataFitting/linear_regression.py
--rw-rw-r--   0 almami    (1000) almami    (1000)    57094 2021-10-18 20:58:37.000000 pyDataFitting-0.0.2/src/pyDataFitting/multivariate_regression.py
--rw-rw-r--   0 almami    (1000) almami    (1000)     8013 2021-10-18 20:58:37.000000 pyDataFitting-0.0.2/src/pyDataFitting/nonlinear_regression.py
--rwxrwxr-x   0 almami    (1000) almami    (1000)    20683 2021-10-19 21:22:34.000000 pyDataFitting-0.0.2/src/pyDataFitting/polynomial_regression.py
-drwxrwxr-x   0 almami    (1000) almami    (1000)        0 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/src/pyDataFitting.egg-info/
--rw-rw-r--   0 almami    (1000) almami    (1000)     4783 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/src/pyDataFitting.egg-info/PKG-INFO
--rw-rw-r--   0 almami    (1000) almami    (1000)      454 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/src/pyDataFitting.egg-info/SOURCES.txt
--rw-rw-r--   0 almami    (1000) almami    (1000)        1 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/src/pyDataFitting.egg-info/dependency_links.txt
--rw-rw-r--   0 almami    (1000) almami    (1000)       70 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/src/pyDataFitting.egg-info/requires.txt
--rw-rw-r--   0 almami    (1000) almami    (1000)       14 2021-12-01 18:37:03.000000 pyDataFitting-0.0.2/src/pyDataFitting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 12:37:04.730266 pyDataFitting-0.0.3/
+-rw-rw-rw-   0        0        0     1095 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5091 2023-04-14 12:37:05.533467 pyDataFitting-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4506 2023-04-14 10:10:48.000000 pyDataFitting-0.0.3/README.md
+-rw-rw-rw-   0        0        0      110 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      722 2023-04-14 12:37:05.543903 pyDataFitting-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      273 2023-04-14 12:32:37.000000 pyDataFitting-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:37:04.802267 pyDataFitting-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 12:37:04.802267 pyDataFitting-0.0.3/src/pyDataFitting/
+-rw-rw-rw-   0        0        0      208 2023-04-14 09:55:23.000000 pyDataFitting-0.0.3/src/pyDataFitting/__init__.py
+-rw-rw-rw-   0        0        0     4067 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/src/pyDataFitting/linear_regression.py
+-rw-rw-rw-   0        0        0     1669 2023-04-14 09:13:47.000000 pyDataFitting-0.0.3/src/pyDataFitting/model_diagnostics.py
+-rw-rw-rw-   0        0        0    13711 2023-04-14 11:10:40.000000 pyDataFitting-0.0.3/src/pyDataFitting/model_tools.py
+-rw-rw-rw-   0        0        0    58327 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/src/pyDataFitting/multivariate_regression.py
+-rw-rw-rw-   0        0        0     6063 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/src/pyDataFitting/nonlinear_regression.py
+-rw-rw-rw-   0        0        0    23760 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/src/pyDataFitting/polynomial_regression.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:37:04.810267 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/
+-rw-rw-rw-   0        0        0     5091 2023-04-14 12:37:04.000000 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2023-04-14 12:37:04.000000 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:37:04.000000 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-04-14 12:37:04.000000 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 12:37:04.000000 pyDataFitting-0.0.3/src/pyDataFitting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 12:37:04.814267 pyDataFitting-0.0.3/tests/
+-rw-rw-rw-   0        0        0     2989 2023-04-14 11:51:38.000000 pyDataFitting-0.0.3/tests/test_model_tools.py
+-rw-rw-rw-   0        0        0     2367 2023-04-14 12:16:08.000000 pyDataFitting-0.0.3/tests/test_nonlinear_regresssion.py
+-rw-rw-rw-   0        0        0     3959 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/tests/test_piecewise_polynomial_fit.py
+-rw-rw-rw-   0        0        0     3387 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/tests/test_polynomial_regression.py
+-rw-rw-rw-   0        0        0     2413 2023-01-17 12:23:36.000000 pyDataFitting-0.0.3/tests/test_principal_component_regression.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyDataFitting-0.0.2/LICENSE` & `pyDataFitting-0.0.3/LICENSE`

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

### Comparing `pyDataFitting-0.0.2/PKG-INFO` & `pyDataFitting-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,73 @@
-Metadata-Version: 2.1
-Name: pyDataFitting
-Version: 0.0.2
-Summary: package for specialized regression
-Home-page: https://github.com/AlexanderSouthan/pyDataFitting
-Author: Alexander Southan
-Author-email: alexander.southan@web.de
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyDataFitting/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![build workflow](https://github.com/AlexanderSouthan/pyDataFitting/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/pyDataFitting/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/AlexanderSouthan/pyDataFitting/branch/master/graph/badge.svg?token=NYWF752QP0)](https://codecov.io/gh/AlexanderSouthan/pyDataFitting)
-
-# pyDataFitting
-Linear and nonlinear fit functions that can be used *e.g.* for curve fitting.
-Is not meant to duplicate methods already implemented *e.g.* in NumPy or SciPy,
-but to provide additional, specialized regression methods or higher computation
-speed. You will need certain functions of my little_helpers repository and
-quite a few other, external packages like Numpy, Pandas, matplotlib,
-scikit-learn, statsmodels, Scipy.
-
-Install with:
-```
-pip install pyDataFitting
-```
-
-## Linear regression (in linear_regression.py)
-* dataset_regression: Does a classical linear least squares regression. Treats
-the input data as a linear combination of the different components from
-reference data. Can be used for example to fit spectra of mixtures with spectra
-of pure components. Produces the same result like, but much faster than using
-sklearn.linear_model.LinearRegression().fit(...).
-* lin_reg_all_sections: Does linear regressions on a dataset starting with the
-first two datapoints and expands the segment by one for each iteration. The
-regression metrics are useful to determine if a dataset behaves linearly at its
-beginning or not, and when a transition to nonlinear behavior occurs.
-
-## Polynomial regression (in polynomial_regression.py)
-* polynomial_fit: Allows to perform polynomial fits by minimizing the sum of
-the squared residuals while also taking equality constaints into account via
-Lagrange multiplicators. This can be used to force the regression function
-through certain points or to force it to have certain slopes at a given points.
-Also does unconstrained polynomial fits, but is slower than the corresponding
-Numpy functions.
-* piecewise_polynomial_fit: Allows to do a picewise polynomial fit on a dataset,
-*i.e.* the data is divided into segments that are then each fitted with an own
-polynomial function. The segments can be fitted with polynomials of different
-orders. It is possible to use equality constraints on the segment borders, so
-that the segments *e.g.* are forced to have the same y values at the borders or
-the same slopes.
-* segment_regression: Does a piecewise polynomial fit with the segment borders,
-y values at the segment borders, or the slopes at the segment borders as
-additional fit parameters. The additional fit parameters are estimated with an
-evolutionary fitting algorithm which calls picewise_polynomial_fit several
-times in each iteration, so the whole procedure is rather slow (albeit still
-very usable).
-
-## General nonlinear regression (in nonlinear_regression.py)
-* nonlinear_regression: Does nonlinear regressions by minimizing the sum of the
-squared residuals. Basically utilizes differential_evolution from
-scipy.optimize to estimatze the parameters of complex regression functions. The
-functions must be included in calc_functions, but can be added easily there. 
-This is not a particularly fast method, so use methods from other packages for
-simple problems.
-* nonlinear_regression_3D: Does the same like nonlinear_regression, but on 3D
-datasets. Also here, the regression function must be included in
-calc_function_3D.
-
-## Principal component regression and partial least squares regression (in multivariate_regression.py)
-* principal_component_regression: A class for a principal component regression
-(PCR). Does a principal component analysis of the dataset and a multilinear
-regression on the resulting scores with one or several responses in order to
-generate a model to predict the responses from future data. The PCR parts work
-quite well, the methods included for generating various plots still need
-improving.
-* pls_regression: A class to help with using the partial least squares
-regression class from scikit-learn. It is usable, but could do with some
-redesigning.
-
-
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![build workflow](https://github.com/AlexanderSouthan/pyDataFitting/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/pyDataFitting/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/AlexanderSouthan/pyDataFitting/branch/master/graph/badge.svg?token=NYWF752QP0)](https://codecov.io/gh/AlexanderSouthan/pyDataFitting)
+
+# pyDataFitting
+Linear and nonlinear fit functions that can be used *e.g.* for curve fitting.
+Is not meant to duplicate methods already implemented *e.g.* in NumPy or SciPy,
+but to provide additional, specialized regression methods, higher computation
+speed, or help with methods from well-known packages. You will need certain
+functions of my little_helpers repository and quite a few other, external
+packages like Numpy, Pandas, matplotlib, scikit-learn, statsmodels, Scipy.
+
+Install with:
+```
+pip install pyDataFitting
+```
+
+## Linear regression (in linear_regression.py)
+* dataset_regression: Does a classical linear least squares regression. Treats
+the input data as a linear combination of the different components from
+reference data. Can be used for example to fit spectra of mixtures with spectra
+of pure components. Produces the same result like, but much faster than using
+sklearn.linear_model.LinearRegression().fit(...).
+* lin_reg_all_sections: Does linear regressions on a dataset starting with the
+first two datapoints and expands the segment by one for each iteration. The
+regression metrics are useful to determine if a dataset behaves linearly at its
+beginning or not, and when a transition to nonlinear behavior occurs.
+
+## Polynomial regression (in polynomial_regression.py)
+* polynomial_fit: Allows to perform polynomial fits by minimizing the sum of
+the squared residuals while also taking equality constaints into account via
+Lagrange multiplicators. This can be used to force the regression function
+through certain points or to force it to have certain slopes at a given points.
+Also does unconstrained polynomial fits, but is slower than the corresponding
+Numpy functions.
+* piecewise_polynomial_fit: Allows to do a picewise polynomial fit on a dataset,
+*i.e.* the data is divided into segments that are then each fitted with an own
+polynomial function. The segments can be fitted with polynomials of different
+orders. It is possible to use equality constraints on the segment borders, so
+that the segments *e.g.* are forced to have the same y values at the borders or
+the same slopes.
+* segment_regression: Does a piecewise polynomial fit with the segment borders,
+y values at the segment borders, or the slopes at the segment borders as
+additional fit parameters. The additional fit parameters are estimated with an
+evolutionary fitting algorithm which calls picewise_polynomial_fit several
+times in each iteration, so the whole procedure is rather slow (albeit still
+very usable).
+
+## General nonlinear regression (in nonlinear_regression.py)
+* nonlinear_regression: Does nonlinear regressions by minimizing the sum of the
+squared residuals. Basically utilizes the minimize method from lmfit to
+estimatze the parameters of complex regression functions. The functions
+calculating the function values must be written externally, but this is pretty
+straight forward. 
+
+## Principal component regression and partial least squares regression (in multivariate_regression.py)
+* principal_component_regression: A class for a principal component regression
+(PCR). Does a principal component analysis of the dataset and a multilinear
+regression on the resulting scores with one or several responses in order to
+generate a model to predict the responses from future data. The PCR parts work
+quite well, the methods included for generating various plots still need
+improving.
+* pls_regression: A class to help with using the partial least squares
+regression class from scikit-learn. It is usable, but could do with some
+redesigning.
+
+## Tools for supporting the use of ols from statsmodels.formula.api (in model_tools.py)
+* Provides simple methods to generate the model string for different simple
+models (linear, two-factor interaction, quadratic, etc.). 
+* Provides a method to easily adapt the included parameters in the model string
+and a method to ensure model hierarchy.
+* Allows the calculation of model values if the model coefficients are
+provided.
```

### Comparing `pyDataFitting-0.0.2/src/pyDataFitting/linear_regression.py` & `pyDataFitting-0.0.3/src/pyDataFitting/linear_regression.py`

 * *Files identical despite different names*

### Comparing `pyDataFitting-0.0.2/src/pyDataFitting/multivariate_regression.py` & `pyDataFitting-0.0.3/src/pyDataFitting/multivariate_regression.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1240 +1,1240 @@
-# -*- coding: utf-8 -*-
-"""Multivariate regression objects for data analysis."""
-
-import numpy as np
-import pandas as pd
-import matplotlib.pyplot as plt
-import matplotlib.ticker as ticker
-from matplotlib.cm import rainbow
-from mpl_toolkits.mplot3d import Axes3D
-from sklearn.decomposition import PCA
-from sklearn.cross_decomposition import PLSRegression
-from sklearn.preprocessing import StandardScaler
-from sklearn.model_selection import cross_val_predict
-from sklearn.metrics import mean_squared_error, r2_score
-import statsmodels.api as sm
-
-from little_helpers.statsmodel_wrapper import statsmodel_wrapper
-
-
-class principal_component_regression():
-    """Class for performing principal component regression."""
-
-    def __init__(self, x, y=None, x_names=None, y_names=None,
-                 sample_names=None, scale_std=False):
-        """
-        Store input data and initialize results DataFrame.
-
-        Parameters
-        ----------
-        x : ndarray or pandas DataFrame
-            Sample training data in the shape (n_samples, n_variables). Data is
-            mean centered automatically, so it is not necessary to do that
-            before. If a pandas DataFrame, the index is used for sample naming
-            and the columns for variable naming, so potentially given values by
-            x_names and sample_names are ignored.
-        y : ndarray, pandas DataFrame or None, optional
-            Target values in the shape (n_samples,) for a single target or
-            (n_samples, n_targets) for multiple targets. Must be given if a
-            regression is to be performed, otherwise only a PCA on x makes
-            sense. Default is None in which case the regression results are
-            empty and meaningless. If a pandas DataFrame, the columns are used
-            for target naming, so potentially given values by y_names are
-            ignored.
-        x_names : list of str or None, optional
-            A list containing the names of the n_variables factors. Default is
-            None which results in numbered variables.
-        y_names : list of str or None, optional
-            A list containing the names of the n_targets responses. Default is
-            None which results in response names of 'response_1', 'response_2'
-            etc.
-        sample_names : list of str or None, optional
-            A list containing the n_samples sample names. Default is None which
-            results in sample names of 'sample_1', 'sample_2' etc.
-        scale_std : bool, optional
-            True means the data will be scaled to unit variance. Default is
-            False.
-
-        Returns
-        -------
-        None.
-
-        """
-        self.scale_std = scale_std
-        self.n_samples, self.n_variables = x.shape
-        if y is None:
-            self.n_responses = 0
-        elif (y is not None) and (len(np.squeeze(y).shape) == 1):
-            self.n_responses = 1
-        else:
-            self.n_responses = y.shape[1]
-
-        if isinstance(y, np.ndarray) or (y is None):
-            if (y_names is not None) and (len(y_names) == self.n_responses):
-                self.y_names = y_names
-            elif y_names is None:
-                self.y_names = ['response_{}'.format(ii) for ii in np.arange(
-                    1, self.n_responses+1)]
-            else:
-                raise ValueError(
-                    'Number of response names does not match number of '
-                    'responses. Number of responses is {} and response name '
-                    'number is {}.'.format(self.n_responses, len(x_names)))
-
-            self.response_index = pd.Index(self.y_names, name='Response name')
-        elif isinstance(y, pd.DataFrame):
-            self.y_names = y.columns.to_numpy()
-            self.response_index = y.columns
-        else:
-            raise TypeError('y must either be np.ndarray or '
-                            'pd.DataFrame or None.')
-
-        if isinstance(x, np.ndarray):
-            if (x_names is not None) and (len(x_names) == self.n_variables):
-                self.x_names = x_names
-            elif x_names is None:
-                self.x_names = ['factor_{}'.format(ii) for ii in np.arange(
-                    1, self.n_variables+1)]
-            else:
-                raise ValueError(
-                    'Number of factor names does not match number of factors. '
-                    'Number of factors is {} and factor name number is '
-                    '{}.'.format(self.n_variables, len(x_names)))
-
-            if (sample_names is not None) and (
-                    len(sample_names) == self.n_samples):
-                self.sample_names = sample_names
-            elif sample_names is None:
-                self.sample_names = [
-                    'sample_{}'.format(ii) for ii in np.arange(
-                        1, self.n_samples+1)]
-            else:
-                raise ValueError(
-                    'Number of sample names does not match number of samples. '
-                    'Number of samples is {} and sample name number is {}'
-                    '.'.format(self.n_samples, len(sample_names)))
-
-            # Construct indices for later use in the DataFrames that collect
-            # the different PCA and PCR results
-            self.sample_index = pd.Index(self.sample_names, name='Sample name')
-            self.var_index = pd.Index(self.x_names, name='Variable name')
-        elif isinstance(x, pd.DataFrame):
-            self.sample_index = x.index
-            self.var_index = x.columns
-        else:
-            raise TypeError('x must either be np.ndarray or '
-                            'pd.DataFrame.')
-
-        y_c_index = pd.MultiIndex.from_product(
-            [self.response_index, self.sample_index.values],
-            names=['response name', 'sample number'])
-        metrics_index = pd.MultiIndex.from_product(
-            [self.response_index, ['r2_c', 'r2_cv', 'rmse_c', 'rmse_cv']],
-            names=['response name', 'metrics type'])
-
-        self.scaler = StandardScaler(with_std=self.scale_std)
-        self.x = pd.DataFrame(self.scaler.fit_transform(x),
-                              index=self.sample_index, columns=self.var_index)
-
-        if (y is not None) and (len(y) == len(x)):
-            self.y = pd.DataFrame(
-                y, index=self.sample_index, columns=self.response_index)
-        elif y is None:
-            self.y = None
-        else:
-            raise ValueError(
-                'Number of responses does not match number of samples. '
-                'Number of responses is {} and sample number is {}.'.format(
-                    self.n_responses, self.n_samples))
-
-        # List that will collect PCA component numbers that already
-        # were calculated
-        self.computed_components = [0]
-
-        self.pca_objects = pd.Series([], dtype='object')
-        self.pca_scores = pd.DataFrame([])
-        self.pca_eigenvalues = pd.Series([], dtype='float64')
-        self.pca_eigenvectors = pd.DataFrame([])
-        self.pca_loadings = pd.DataFrame([])
-        self.pca_explained_variance = pd.DataFrame([], columns=['each', 'cum'])
-        self.pca_results = pd.DataFrame([],
-                                        index=['Hotelling_T2', 'Q_residuals'])
-        self.pcr_models = pd.DataFrame([], dtype='object',
-                                       columns=self.response_index)
-        self.pcr_params = pd.DataFrame([], dtype='object',
-                                       columns=self.response_index)
-        self.pcr_used_pcs = pd.DataFrame([], dtype='object',
-                                         columns=self.response_index)
-        self.pcr_corr_coef = pd.DataFrame([], columns=self.response_index)
-        self.pcr_y_c = pd.DataFrame([], index=y_c_index)
-        self.pcr_y_cv = pd.DataFrame([], index=y_c_index)
-        self.pcr_metrics = pd.DataFrame([], index=metrics_index)
-
-    def perform_pca(self, n_components, **kwargs):
-        """
-        Actually perform the principal component analysis.
-
-        Parameters
-        ----------
-        n_components : int
-            Number of components kept after principal component analysis.
-        **kwargs :
-            All **kwargs from sklearn.decomposition.PCA are allowed, see the
-            documentation of that class for details.
-
-        Returns
-        -------
-        None.
-
-        """
-        # Check if PCA with n_components was already done before. If so, no
-        # calculation is performed because the data is already there.
-        if n_components not in self.computed_components:
-            self.pca_objects[n_components] = PCA(
-                n_components=n_components, **kwargs)
-            curr_scores = self.pca_objects[
-                    n_components].fit_transform(self.x)
-
-            # Check if any new information is generated by the calculations.
-            # If that is the case, scores, loadings, etc. are stored in the
-            # corresponding attributes.
-            if n_components > max(self.computed_components):
-                pc_index = pd.Index(np.arange(1, n_components+1),
-                                    name='PC number')
-
-                self.pca_scores = pd.DataFrame(curr_scores,
-                                               index=self.sample_index,
-                                               columns=pc_index)
-                self.pca_eigenvalues = pd.Series(
-                    self.pca_objects[n_components].explained_variance_,
-                    index=pc_index)
-                self.pca_eigenvectors = pd.DataFrame(
-                    self.pca_objects[n_components].components_.T,
-                    index=self.var_index,
-                    columns=pc_index)
-                self.pca_loadings = self.pca_eigenvectors * np.sqrt(
-                    self.pca_eigenvalues)
-                self.pca_explained_variance = pd.DataFrame(
-                    self.pca_objects[n_components].explained_variance_ratio_,
-                    columns=['each'], index=pc_index)
-                self.pca_explained_variance['cum'] = (
-                    self.pca_explained_variance['each'].cumsum())
-
-            self.pca_results[n_components] = pd.Series([], dtype='object')
-            # self.pc_loadings = self.components_.T
-            # * np.sqrt(pca.explained_variance_)
-
-            # Some PCA metrics are calculated. The results should be checked,
-            # calculation is still experimental. Also the attribute pca_results
-            # should be improved in the future.
-            # self.pca_results.at['Hotelling_T2', n_components] = np.array(
-            #     [sample.dot(self.pca_eigenvectors.loc[:, :n_components]).dot(
-            #         np.diag(self.pca_eigenvalues ** -1)).dot(
-            #             self.pca_eigenvectors.loc[:, :n_components].T).dot(
-            #                 sample.T) for sample in self.x])
-            # self.pca_results.at['Q_residuals', n_components] = np.array(
-            #     [sample.dot(np.identity(self.x.shape[1])-self.pca_eigenvectors.loc[
-            #         :, :n_components].dot(self.pca_eigenvectors.loc[
-            #             :, :n_components].T)).dot(
-            #                 sample.T) for sample in self.x])
-
-            self.computed_components.append(n_components)
-
-    def reconstruct_input(self):
-        """
-        Reconstruct the original input data.
-
-        The input data are reconstructed from the scaled data using the
-        standard deviation (if self.scale.std == true) and the
-        mean data from self.scaler. The input data is not needed within this
-        class, so the input data is not stored in order to save memory.
-
-        Returns
-        -------
-        reconstructed_input : pandas DataFrame
-            A DataFrame in the same format as self.x containing the input data.
-
-        """
-        reconstructed_input = pd.DataFrame(
-            self.scaler.inverse_transform(self.x.copy()),
-            index=self.x.index, columns=self.x.columns)
-        return reconstructed_input
-
-    def reconstruct_data(self, used_pcs):
-        """
-        Reconstruct the data from scores and eigenvectors.
-
-        The result is the original data without the contents of the PCA error
-        matrix, so can also be understood as a PCA based smoothing.
-
-        Parameters
-        ----------
-        used_pcs : int or list of int
-            If an int is given, the according number of principal components
-            is used for data reconstruction based on the order of explained
-            variance. If a list of int is given, the pricipal components given
-            in the list will be used for data reconstruction, based on the
-            explained variance ordering and the first PC having number 1.
-
-        Returns
-        -------
-        reconstructed_data : pandas DataFrame
-            The recomstructed data in the same format as self.x.
-
-        """
-        if isinstance(used_pcs, int):
-            max_component = used_pcs
-            pc_list = np.arange(1, used_pcs+1)
-        elif isinstance(used_pcs, list) and all(
-                [isinstance(ii, int) for ii in used_pcs]):
-            max_component = max(used_pcs)
-            pc_list = used_pcs
-        else:
-            raise TypeError('No valid value for used_pcs given. Allowed '
-                            'inputs are an integer or a list of integers.')
-
-        if max_component > max(self.computed_components):
-            self.perform_pca(max_component)
-
-        reconstructed_data = np.dot(
-            self.pca_scores.loc[:, pc_list],
-            self.pca_eigenvectors.loc[:, pc_list].T)
-
-        reconstructed_data = pd.DataFrame(
-            self.scaler.inverse_transform(reconstructed_data),
-            index=self.x.index, columns=self.x.columns)
-
-        return reconstructed_data
-
-    def pcr_fit(self, cv_percentage=20, mode='exp_var',
-                **kwargs):
-        """
-        Perform principal component regression for one number of components.
-
-        One PCA object is generated for every number of components.
-        This is necessary in order to be able to use the PCA transform method
-        in self.predict. For example, the predicted sample values ('y') of the
-        training data ('c'), the corresponding predictions ('y') after
-        cross-validation ('cv'), the coefficient of determination ('r2') for
-        'c' and 'cv', and the root mean squared error ('rmse') for 'c' and 'cv'
-        are calculated.
-
-        Parameters
-        ----------
-        cv_percentage : float, optional
-            Percentage of data used for cross-validation. The default is 20.
-        mode : str, optional
-            Determines if PCs used for regression are selected based on
-            explained variance only ('exp_var'), only based on corellation
-            with the data in self.y ('corr_coef'), or are given in a list based
-            on the exlained variance order ('list'). Default is 'exp_var'.
-        **kwargs :
-            All **kwargs from sklearn.decomposition.PCA are allowed, see the
-            documentation of that class for details.
-        **kwargs if mode=='exp_var':
-            n_components : int
-                The number of principal components used for the regression.
-        **kwargs if mode=='corr_coef':
-            n_components : int
-                See above.
-            max_components : int
-                The number of components ordered by increasing explained
-                variance which are used for calculation of corellation
-                coefficients. Default is 10.
-        **kwargs if mode=='list'
-            used_pcs : list of int
-                Gives the principal components used for regression based on the
-                order of explained variance.
-
-        Returns
-        -------
-        None
-
-        """
-        # PCA options
-        copy = kwargs.get('copy', True)
-        whiten = kwargs.get('whiten', False)
-        svd_solver = kwargs.get('svd_solver', 'auto')
-        tol = kwargs.get('tol', 0.0)
-        iterated_power = kwargs.get('iterated_power', 'auto')
-        random_state = kwargs.get('random_state', None)
-
-        # # LinearRegression options
-        # fit_intercept = kwargs.get('fit_intercept', True)
-        # normalize = kwargs.get('normalize', False)
-        # copy_X = kwargs.get('copy_X', True)
-        # n_jobs = kwargs.get('n_jobs', None)
-
-        if (mode == 'exp_var') or (mode == 'corr_coef'):
-            n_components = kwargs.get('n_components')
-        elif mode == 'list':
-            pc_list = kwargs.get('used_pcs')
-            n_components = max(pc_list)
-        else:
-            raise ValueError('Missing info on the number of components.')
-
-        # Perform the actual PCA
-        self.perform_pca(n_components, copy=copy, whiten=whiten,
-                         svd_solver=svd_solver, tol=tol,
-                         iterated_power=iterated_power,
-                         random_state=random_state)
-
-        # The number of components used for the calulation of the correlation
-        # coefficients can be bigger than the number of components used for
-        # the regression afterwards. Thus, e.g. a regression using 5 components
-        # can include e.g. the 10th component based on the explained variance
-        # ordering if max_components allows it.
-        if mode == 'corr_coef':
-            max_components = kwargs.get('max_components', 10)
-            self.perform_pca(max_components, copy=copy, whiten=whiten,
-                             svd_solver=svd_solver, tol=tol,
-                             iterated_power=iterated_power,
-                             random_state=random_state)
-
-        # In each iteration in the following for loop, a multilinear regression
-        # with the scores and only one of the responses given is performed. So
-        # the loop iterates over the individual responses. This results in
-        # one call of the fit and predict methods from the linear model objects
-        # per iteration. This is necessary for mode=='coord_coef' because for
-        # each response, different components may be used for regression.
-        for curr_y in self.y_names:
-            for curr_index, curr_scores in enumerate(
-                    self.pca_scores.values.T):
-                self.pcr_corr_coef.at[curr_index+1, curr_y] = np.abs(
-                    np.corrcoef(
-                        curr_scores, self.y[curr_y])[0, 1])
-
-            # Select score values to be used for the regression based on the
-            # mode given.
-            if mode == 'exp_var':
-                self.pcr_used_pcs.at[n_components, curr_y] = np.arange(
-                    1, n_components+1)
-            elif mode == 'corr_coef':
-                self.pcr_used_pcs.at[n_components, curr_y] = np.flip(
-                    np.argsort(self.pcr_corr_coef.loc[:, curr_y].values)[
-                        -n_components:])+1
-            elif mode == 'list':
-                self.pcr_used_pcs.at[n_components, curr_y] = np.array(pc_list)
-
-            fit_scores = self.pca_scores.loc[
-                :, self.pcr_used_pcs.at[n_components, curr_y]].values
-
-            # Build linear model
-            fit_scores = sm.add_constant(fit_scores)
-            self.pcr_models.at[n_components, curr_y] = sm.OLS(
-                self.y[curr_y], fit_scores)
-            self.pcr_params.at[n_components, curr_y] = (
-                self.pcr_models.at[n_components, curr_y].fit())
-            # Predict sample values according to PCR model
-            idx = pd.IndexSlice
-            self.pcr_y_c.loc[idx[curr_y, :], n_components] = (
-                self.pcr_models.at[n_components, curr_y].predict(
-                    self.pcr_params.at[n_components, curr_y].params,
-                    fit_scores))
-            # Cross-validate the PCR model
-            self.pcr_y_cv.loc[idx[curr_y, :], n_components] = (
-                cross_val_predict(statsmodel_wrapper(sm.OLS),
-                                  fit_scores, self.y[curr_y],
-                                  cv=round(100/cv_percentage)))
-            # Calculate metrics for PCR model
-            self.pcr_metrics.at[(curr_y, 'r2_c'), n_components] = r2_score(
-                self.y[curr_y], self.pcr_y_c.loc[
-                    idx[curr_y, :], n_components], multioutput='raw_values')
-            self.pcr_metrics.at[(curr_y, 'r2_cv'), n_components] = r2_score(
-                self.y[curr_y], self.pcr_y_cv.loc[
-                    idx[curr_y, :], n_components], multioutput='raw_values')
-            self.pcr_metrics.at[(curr_y, 'rmse_c'), n_components] = (
-                mean_squared_error(self.y[curr_y],
-                                   self.pcr_y_c.loc[idx[curr_y, :],
-                                                    n_components],
-                                   multioutput='raw_values', squared=False))
-            self.pcr_metrics.at[(curr_y, 'rmse_cv'), n_components] = (
-                mean_squared_error(self.y[curr_y],
-                                   self.pcr_y_cv.loc[idx[curr_y, :],
-                                                     n_components],
-                                   multioutput='raw_values', squared=False))
-
-    def pcr_sweep(self, sweep_components=20, cv_percentage=20, mode='exp_var',
-                  **kwargs):
-        """
-        Perform PCR for all number of components between 1 and n_components.
-
-        Parameters
-        ----------
-        sweep_components : int, optional
-            The upper limit of components used for PCR. The default is 20.
-        cv_percentage : float, optional
-            Percentage of data used for cross-validation. The default is 10.
-        mode : str, optional
-            Determines if PCs used for regression are selected based on
-            explained variance only ('exp_var'), only based on corellation
-            with the data in self.y ('corr_coef'), or are given in a list based
-            on the explained variance order ('list'). Default is 'exp_var'.
-        **kwargs :
-            The same **kwargs as in self.pcr_fit, only n_components must be
-            left out because that is controlled by the iterator of the loop
-            that repeatately calls self.pcr_fit.
-
-        Returns
-        -------
-        DataFrame
-            See Docstring of self.pcr_fit.
-
-        """
-        assert mode in ['exp_var', 'corr_coef'], (
-            'No valid option for mode given. Remember that \'list\' is not '
-            'allowed for this method because in this case information about '
-            'the PCs used must already be known.')
-
-        for ii in reversed(range(1, sweep_components+1)):
-            self.pcr_fit(cv_percentage=cv_percentage, mode=mode,
-                         n_components=ii, **kwargs)
-        # return self.pcr_results
-
-    def predict(self, samples, n_components, sample_names=None):
-        """
-        Predict unknown sample target values.
-
-        Currently works correct only for mode=='exp_var'. For
-        mode=='corr_coef', the tranformation has to be implemented independent
-        of the PCA object method.
-
-        Parameters
-        ----------
-        samples : ndarray
-            Sample data in the shape (n_samples, n_variables).
-        n_components : int
-            Number of components used in the PCR model for the prediction.
-        sample_names : list of str, optional
-            The names of the samples passed to the function for prediction.
-            Default is None resulting in numbered sample names.
-
-        Returns
-        -------
-        prediction : ndarray
-            Predicted target values in the shape (n_samples,) for a single
-            target or (n_samples, n_targets) for multiple targets.
-
-        """
-        if sample_names is None:
-            sample_names = ['Sample {}'.format(curr_idx)
-                            for curr_idx in range(len(samples))]
-
-        transformed_samples = self.pca_objects.at[n_components].transform(
-            self.scaler.transform(samples))
-
-        transformed_samples = sm.add_constant(transformed_samples)
-        self.test = transformed_samples
-
-        prediction = pd.DataFrame([], columns=self.y_names, index=sample_names)
-        for curr_y in self.y_names:
-            prediction[curr_y] = (
-                self.pcr_models.at[n_components, curr_y].predict(
-                    self.pcr_params.at[n_components, curr_y].params,
-                    transformed_samples))
-        return prediction
-
-    def results_to_csv(self, folder=None):
-        if folder is None:
-            folder = ''
-        self.pca_loadings.to_csv(folder + '/pca_loadings.txt', sep='\t')
-        self.pca_explained_variance.to_csv(
-            folder + '/pca_explained_variance.txt', sep='\t')
-        self.pca_scores.to_csv(folder + '/pca_scores.txt', sep='\t')
-        self.pcr_corr_coef.to_csv(folder + '/pcr_corr_coef.txt', sep='\t')
-        self.pcr_metrics.to_csv(folder + '/pcr_metrics.txt', sep='\t')
-        self.pcr_used_pcs.to_csv(folder + '/pcr_used_pcs.txt', sep='\t')
-        self.pcr_y_c.to_csv(folder + '/pcr_y_c.txt', sep='\t')
-        self.pcr_y_cv.to_csv(folder + '/pcr_y_cv.txt', sep='\t')
-
-    def pca_biplot(self, pc_numbers=[1, 2], grouping=[None, None, None],
-                   scores_only=False, **kwargs):
-        """
-        Make a plot containing both the PCA loadings and scores.
-
-        Parameters
-        ----------
-        pc_numbers : list of int, optional, optional
-            Contains two entries giving the component indices to be used for
-            plotting, starting with 1 for the first principal component. The
-            default is [0,1].
-        grouping : list of str or None, optional
-            Contains three elements that must either be an element from
-            self.y_names or None. Defines a color (first entry), symbol
-            (second entry) and symbol fill style grouping (third entry) of
-            plotted scores based on the given targets. Default is [None, None,
-            None] where there is no grouping and only one color and one symbol
-            is used.
-        scores_only : boolean, optional
-            If True, the loadings will not be plotted, but only the scores.
-            Default is False.
-        **kwargs :
-            colors : list of matplotlib color codes
-                Must contain as many elements as levels present in the target
-                used for the color grouping. By default, the colors are given
-                by the matplotlib rainbow colormap.
-            markers : list og matplotlib markers, optional
-                Must contain as many elements as levels present in the target
-                used for symbol grouping. By default, a modified list obtained
-                by matplotlib.lines.Line2D.markers.keys() is used.
-            fill_styles : list of matplotlib marker fill styles, optional
-                Must contain as many elements as levels present in the target
-                used for fill style grouping. By default, a modified list
-                obtained by matplotlib.lines.Line2D.fillStyles is used.
-
-        Raises
-        ------
-        ValueError
-            DESCRIPTION.
-
-        Returns
-        -------
-        None.
-
-        """
-        # Define plot deltails
-        SMALL_SIZE = 6
-        MEDIUM_SIZE = 8
-        BIGGER_SIZE = 10
-        FIGSIZE = (3.1496, 2.3622)
-        DPI = 600
-        MARKERSIZE = 4
-
-        plt.rc('font', size=MEDIUM_SIZE)  # controls default text sizes
-        plt.rc('axes', titlesize=MEDIUM_SIZE)  # fontsize of the axes title
-        plt.rc('axes', labelsize=MEDIUM_SIZE)  # fontsize of the x and y labels
-        plt.rc('xtick', labelsize=MEDIUM_SIZE)  # fontsize of the tick labels
-        plt.rc('ytick', labelsize=MEDIUM_SIZE)  # fontsize of the tick labels
-        plt.rc('legend', fontsize=SMALL_SIZE)  # legend fontsize
-        plt.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
-
-        # First produce axis with two circles and the coordinate axes as dotted
-        # lines. This axis will be used to plot the PCA loadings.
-        fig1, ax1 = plt.subplots(1, figsize=FIGSIZE, dpi=DPI)
-        if not scores_only:
-            circle1 = plt.Circle((0, 0), 1, color='k', linestyle='--',
-                                 fill=False)
-            circle2 = plt.Circle((0, 0), np.sqrt(0.5), color='k',
-                                 linestyle='dotted', fill=False)
-            ax1.add_artist(circle1)
-            ax1.add_artist(circle2)
-            ax1.axhline(0, color='k', linestyle='dotted')
-            ax1.axvline(0, color='k', linestyle='dotted')
-            # Draw arrows starting at the origin for the PCA loadings and
-            # annotate them with the name of the corresponding target from
-            # self.y.
-            for (curr_loading1, curr_loading2, curr_var) in zip(
-                    self.pca_loadings[pc_numbers[0]],
-                    self.pca_loadings[pc_numbers[1]],
-                    self.pca_loadings.index.values):
-                ax1.arrow(0, 0, curr_loading1, curr_loading2, color='b',
-                          head_width=0.05, length_includes_head=True)
-                if curr_loading1 >= 0:
-                    ha = 'left'
-                else:
-                    ha = 'right'
-                # rotation = np.arctan(curr_loading2/curr_loading1)/(2*np.pi)*360
-                ax1.text(curr_loading1, curr_loading2, curr_var, ha=ha,
-                         va='center', rotation=0)
-            # Set limits and labels
-            ax1.set_xlim(-1.1, 1.1)
-            ax1.set_ylim(-1.1, 1.1)
-            ax1.set_xlabel('PC{} loadings'.format(pc_numbers[0]))
-            ax1.set_ylabel('PC{} loadings'.format(pc_numbers[1]))
-            ax1.set_facecolor('lightgrey')
-
-            # Set x and y tick spacing
-            ax1.xaxis.set_major_locator(ticker.MultipleLocator(0.4))
-            ax1.xaxis.set_minor_locator(ticker.MultipleLocator(0.1))
-            ax1.yaxis.set_major_locator(ticker.MultipleLocator(0.4))
-            ax1.yaxis.set_minor_locator(ticker.MultipleLocator(0.1))
-
-        # Add another axis on top of the previous one. The new axis will hold
-        # the PCA scores.
-        ax2 = fig1.add_subplot(111)
-
-        # If no grouping by color and/or symbol grouping contains only None
-        # so a simple scatter plot is made for the scores.
-        if not any(grouping):
-            ax2.plot(self.pca_scores[pc_numbers[0]],
-                     self.pca_scores[pc_numbers[1]],
-                     label='Scores', marker='o',
-                     markersize=MARKERSIZE, linestyle='none')
-            ax2.legend(loc='center right', bbox_to_anchor=(1.7, 0.5))
-
-        # If grouping by color and/or symbol the plotting procedure is a
-        # little more complicated, involves three nested for loops to
-        # accomodate the three grouping principles.
-        elif ((grouping[0] in self.y_names) or (grouping[0] is None)) and (
-                (grouping[1] in self.y_names) or (grouping[1] is None)) and (
-                    (grouping[2] in self.y_names) or (grouping[2] is None)):
-
-            # The values present in the y variables used for grouping are
-            # determined.
-            grouping_levels = []
-            grouping_levels.append(
-                self.y[grouping[0]].unique() if grouping[0] is not None
-                else None)
-            grouping_levels.append(
-                self.y[grouping[1]].unique() if grouping[1] is not None
-                else None)
-            grouping_levels.append(
-                self.y[grouping[2]].unique() if grouping[2] is not None
-                else None)
-
-            # Masks used for the later selection of data to be plotted are
-            # determined. This is done for one y variable used for grouping
-            # after the other (next three if-else statements).
-            grouping_masks = []
-            if grouping_levels[0] is not None:
-                grouping_masks.append([
-                    (self.y[grouping[0]] == curr_level).values
-                    for curr_level in grouping_levels[0]])
-            else:
-                grouping_masks.append(
-                    [np.full_like(self.y.index.values, True,
-                                  dtype='bool')])
-
-            if grouping_levels[1] is not None:
-                grouping_masks.append([
-                    (self.y[grouping[1]] == curr_level).values
-                    for curr_level in grouping_levels[1]])
-            else:
-                grouping_masks.append([np.full_like(
-                    self.y.index.values, True, dtype='bool')])
-
-            if grouping_levels[2] is not None:
-                grouping_masks.append([
-                    (self.y[grouping[2]] == curr_level).values
-                    for curr_level in grouping_levels[2]])
-            else:
-                grouping_masks.append([np.full_like(
-                    self.y.index.values, True, dtype='bool')])
-
-            # The 1D grouping masks from before are mixed together in one 3D
-            # array that is iterated over while plotting later on.
-            grouping_masks_all = (
-                np.array(grouping_masks[0]) *
-                np.array(grouping_masks[1])[:, np.newaxis]) * np.array(
-                    grouping_masks[2])[:, np.newaxis, np.newaxis]
-
-            # Colors, symbols and fill styles used for grouping are determined.
-            grouping_colors = kwargs.get(
-                'colors',
-                [rainbow(x) for x in np.linspace(0, 1,
-                                                 len(grouping_masks_all))])
-            grouping_symbols = kwargs.get(
-                'markers',
-                ['o', 'v', 'P', 'X', 'H', '<', '>', '1', '2', '3', '4',
-                 '8', 's', 'p', '*', 'h', '^', '+', 'x', 'D', 'd', '|',
-                 '_', '.', ',', 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11])
-            grouping_fillstyles = kwargs.get(
-                'fill_styles',
-                ['full', 'none', 'top', 'bottom', 'left', 'right'])
-
-            # Now the actual plotting starts by iterating through the
-            # previously calculated 3D mask array with three nested for loops.
-            idx = np.empty(3, dtype='int')
-            for idx[2], (curr_mask_2, curr_fillstyle) in enumerate(zip(
-                    grouping_masks_all, grouping_fillstyles)):
-                for idx[1], (curr_mask_1, curr_symbol) in enumerate(zip(
-                        curr_mask_2, grouping_symbols)):
-                    for idx[0], (curr_mask_0, curr_color) in enumerate(zip(
-                            curr_mask_1, grouping_colors)):
-
-                        label = ''
-                        for ii, curr_levels in enumerate(grouping_levels):
-                            if curr_levels is not None:
-                                label = label + str(curr_levels[idx[ii]]) + ', '
-                        label = label[:-2]
-                        # if grouping_levels[0] is None:
-                        #     label = str(grouping_levels[1][idx_0])
-                        # elif grouping_levels[1] is None:
-                        #     label = str(grouping_levels[0][idx_1])
-                        # elif grouping_levels[2] is None:
-                        #     label = str(grouping_levels[0][idx_2])
-                        # else:
-                        #     label = str(grouping_levels[0][idx_1])+', '+str(grouping_levels[1][idx_0])
-    
-                        ax2.plot(self.pca_scores.loc[curr_mask_0, pc_numbers[0]],
-                                 self.pca_scores.loc[curr_mask_0, pc_numbers[1]],
-                                 color=curr_color, marker=curr_symbol, label=label,
-                                 fillstyle=curr_fillstyle, linestyle='none',
-                                 markersize=MARKERSIZE)
-
-            legend_title = ''
-            for idx, curr_levels in enumerate(grouping_levels):
-                if curr_levels is not None:
-                    legend_title = legend_title + grouping[idx] + ', '
-            legend_title = legend_title[:-2]
-            ax2.legend(loc='center right', bbox_to_anchor= (1.8, 0.5), title=legend_title)
-        else:
-            raise ValueError('No valid grouping. Allowed values must be in'
-                             ' {} or None, but \'{}\' was given.'.format(
-                                 self.y_names, grouping))
-
-        # Score plot axis labels and positions are fixed and the top layer
-        # background is set to tranparent.
-        ax2.yaxis.set_ticks_position('right')
-        ax2.xaxis.set_ticks_position('top')
-        ax2.yaxis.set_label_position('right')
-        ax2.xaxis.set_label_position('top')
-        ax2.set_xlabel('PC{} scores'.format(pc_numbers[0]))
-        ax2.set_ylabel('PC{} scores'.format(pc_numbers[1]))
-        ax2.patch.set_alpha(0)
-
-        return fig1
-
-    def generate_plots(self, plot_names, response_number=0, **kwargs):
-        """
-        Generate some basic plots of principal component regression results.
-
-        Parameters
-        ----------
-        plot_names : list of str
-            List of plots to be generated. Allowed entries are
-            'actual_vs_pred' (actual target values vs. predicted values),
-            'r2_vs_comp' (coefficient of determination vs. number of
-            components), 'mse_vs_comp' (mean squared error vs. number of
-            components), 'biplot' (PCA loadings and scores in one plot),
-            'scoreplot_3D' (a 3D score plot using three principal components).
-        response_number : int, optional
-            Defines the index of the response from self.y to be plotted.
-            Default is 0.
-        **kwargs :
-            n_components : int
-                Needed for plot_name 'actual_vs_pred'. Currently, there is one
-                difficulty when using mode=='list' for self.pcr_fit. In this
-                case, the value for n_components has to be the highest number
-                in the list, otherwise a KeyError occurs.
-            cv : boolean
-                State if cross-validation data should be plotted, too.
-                Default is False.
-
-        Returns
-        -------
-        plots : matplotlib plots
-            Plot objects, I do not know if anything can be done with this.
-
-        """
-        plots = []
-        plot_cv_data = kwargs.get('cv', False)
-        idx = pd.IndexSlice
-        if 'actual_vs_pred' in plot_names:
-            n_components = kwargs.get('n_components')
-            curr_y = self.y[self.y_names[response_number]]
-            curr_c = self.pcr_y_c.loc[idx[self.y_names[response_number], :],
-                                      n_components]
-            curr_cv = self.pcr_y_cv.loc[idx[self.y_names[response_number], :],
-                                        n_components]
-            z_c = np.polyfit(
-                curr_y, curr_c, 1)
-            z_cv = np.polyfit(
-                curr_y, curr_cv, 1)
-            with plt.style.context(('ggplot')):
-                fig1, ax1 = plt.subplots(figsize=(9, 5))
-                ax1.scatter(curr_y, curr_c, c='red', edgecolors='k')
-                if plot_cv_data:
-                    ax1.scatter(curr_y, curr_cv, c='blue', edgecolors='k')
-                    ax1.plot(curr_y, z_cv[1]+z_cv[0]*curr_y, c='blue',
-                             linewidth=1)
-                ax1.plot(curr_y, z_c[1]+z_c[0]*curr_y, c='red', linewidth=1)
-                ax1.plot(curr_y, curr_y, color='green', linewidth=1)
-                plt.title('$R^{2}$ (CV): '+str(
-                    self.pcr_metrics.at[(self.y_names[response_number],
-                                         'r2_cv'), n_components]))
-                plt.xlabel('Measured')
-                plt.ylabel('Predicted')
-            plots.append(fig1)
-        if 'r2_vs_comp' in plot_names:
-            curr_c_r2 = self.pcr_metrics.loc[(self.y_names[response_number],
-                                              'r2_c')]
-            curr_cv_r2 = self.pcr_metrics.loc[(self.y_names[response_number],
-                                               'r2_cv')]
-
-            with plt.style.context(('ggplot')):
-                fig2, ax2 = plt.subplots(figsize=(9, 5))
-                ax2.plot(
-                    curr_c_r2, linestyle='--', marker='o')
-                if plot_cv_data:
-                    ax2.plot(
-                        curr_cv_r2, linestyle='--', marker='o')
-                plt.ylabel('$R^{2}$')
-                plt.xlabel('Number of components')
-            plots.append(fig2)
-        if 'mse_vs_comp' in plot_names:
-            curr_c_rmse = self.pcr_metrics.loc[(self.y_names[response_number],
-                                                'rmse_c')]
-            curr_cv_rmse = self.pcr_metrics.loc[(self.y_names[response_number],
-                                                 'rmse_cv')]
-
-            with plt.style.context(('ggplot')):
-                fig3, ax3 = plt.subplots(figsize=(9, 5))
-                ax3.plot(
-                    curr_c_rmse, linestyle='--', marker='o')
-                if plot_cv_data:
-                    ax3.plot(
-                        curr_cv_rmse, linestyle='--', marker='o')
-                plt.ylabel('RMSE')
-                plt.xlabel('Number of components')
-            plots.append(fig3)
-        if 'expvar_vs_corrcoef' in plot_names:
-            curr_expvar = self.pca_explained_variance['each']
-            curr_corrcoef = self.pcr_corr_coef[self.y_names[response_number]]
-
-            with plt.style.context(('ggplot')):
-                fig4, ax4 = plt.subplots(figsize=(9, 5))
-                ax4.scatter(
-                    curr_expvar, curr_corrcoef)
-                for ii, txt in enumerate(curr_expvar.index):
-                    ax4.annotate(txt, (curr_expvar[ii+1], curr_corrcoef[ii+1]))
-                ax4.set_yscale('log')
-                ax4.set_xscale('log')
-                plt.ylabel('Correlation coefficients')
-                plt.xlabel('Explained variance')
-                plt.title(self.y_names[response_number])
-            plots.append(fig4)
-        if 'scoreplot_3D' in plot_names:
-            pc_numbers = kwargs.get('pc_numbers', [0, 1, 2])
-            grouping = kwargs.get('grouping', [None, None])
-            fig1 = plt.figure()
-            ax2 = Axes3D(fig1)
-            marker_size = 200
-            # If no grouping by color and/or symbol grouping contains only None
-            # so a simple scatter plot is made for the scores.
-            if not any(grouping):
-                ax2.scatter(self.pca_scores[pc_numbers[0]],
-                            self.pca_scores[pc_numbers[1]],
-                            self.pca_scores[pc_numbers[2]],
-                            label='Scores', s=marker_size)
-                ax2.legend(loc='lower left', bbox_to_anchor= (1.1, 0))
-            # If grouping by color and/or symbol the plotting procedure is a
-            # little more complicated, involves two nested for loops to
-            # accomodate the two grouping principles.
-            elif ((grouping[0] in self.y_names) or (grouping[0] is None)) and (
-                    (grouping[1] in self.y_names) or (grouping[1] is None)):
-                grouping_levels_0 = self.y[grouping[0]].unique() if grouping[0] is not None else None
-                grouping_levels_1 = self.y[grouping[1]].unique() if grouping[1] is not None else None
-
-                if grouping_levels_0 is not None:
-                    grouping_masks_0 = [
-                        (self.y[grouping[0]]==curr_level).values
-                        for curr_level in grouping_levels_0]
-                else:
-                    grouping_masks_0 = [np.full_like(self.y.index.values, True, dtype='bool')]
-
-                if grouping_levels_1 is not None:
-                    grouping_masks_1 = [
-                        (self.y[grouping[1]]==curr_level).values
-                        for curr_level in grouping_levels_1]
-                else:
-                    grouping_masks_1 = [np.full_like(self.y.index.values, True, dtype='bool')]
-
-                grouping_masks_all = np.array(grouping_masks_1) * np.array(grouping_masks_0)[:, np.newaxis]
-                grouping_colors = kwargs.get(
-                    'colors',
-                    [rainbow(x) for x in np.linspace(0, 1,
-                                                     len(grouping_masks_all))])
-                #['k', 'b', 'r']
-                grouping_symbols = kwargs.get(
-                    'markers',
-                    ['o', 'v', 'P', 'X', 'H', '<', '>', '1', '2', '3', '4',
-                     '8', 's', 'p', '*', 'h', '^', '+', 'x', 'D', 'd', '|',
-                     '_', '.', ',', 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11])
-                for idx_1, (curr_mask_1, curr_color) in enumerate(zip(
-                        grouping_masks_all, grouping_colors)):
-                    for idx_0, (curr_mask_0, curr_symbol) in enumerate(zip(
-                            curr_mask_1, grouping_symbols)):
-
-                        if grouping_levels_0 is None:
-                            label = str(grouping_levels_1[idx_0])
-                            legend_title = grouping[1]
-                        elif grouping_levels_1 is None:
-                            label = str(grouping_levels_0[idx_1])
-                            legend_title = grouping[0]
-                        else:
-                            label = str(grouping_levels_0[idx_1])+', '+str(grouping_levels_1[idx_0])
-                            legend_title = grouping[0]+', '+grouping[1]
-
-                        ax2.scatter(self.pca_scores.loc[curr_mask_0, pc_numbers[0]],
-                                    self.pca_scores.loc[curr_mask_0, pc_numbers[1]],
-                                    self.pca_scores.loc[curr_mask_0, pc_numbers[2]],
-                                    color=curr_color, marker=curr_symbol,
-                                    s=marker_size, label=label)
-
-                        ax2.legend(loc='upper left', bbox_to_anchor= (1.15, 1), title=legend_title)
-            else:
-                raise ValueError('No valid grouping. Allowed values must be in'
-                                 ' {} or None, but \'{}\' was given.'.format(
-                                     self.y_names, grouping))
-            ax2.yaxis.set_ticks_position('top')
-            ax2.xaxis.set_ticks_position('top')
-            ax2.yaxis.set_label_position('top')
-            ax2.xaxis.set_label_position('top')
-            ax2.set_xlabel('PC{} scores'.format(pc_numbers[0]))
-            ax2.set_ylabel('PC{} scores'.format(pc_numbers[1]))
-            ax2.set_zlabel('PC{} scores'.format(pc_numbers[2]))
-            ax2.patch.set_alpha(0)
-
-        return plots
-
-
-class pls_regression():
-    """Class for performing principal component regression."""
-
-    def __init__(self, x, y, scale_std=False):
-        """
-        Store input data and initialize results DataFrame.
-
-        Parameters
-        ----------
-        x : ndarray
-            Sample training data in the shape (n_samples, n_variables).
-        y : ndarray
-            Target values in the shape (n_samples,) for a single target or
-            (n_samples, n_targets) for multiple targets.
-
-        Returns
-        -------
-        None.
-
-        """
-        self.x_raw = x
-        self.y = y
-        self.scale_std = scale_std
-
-        self.scaler = StandardScaler(with_std=self.scale_std)
-        self.x = self.scaler.fit_transform(self.x_raw)
-
-        results_index = pd.MultiIndex.from_product(
-            [['plsr_objects', 'y', 'r2', 'mse', 'Hotelling_T2'], ['c', 'cv']],
-            names=['result_name', 'cal_or_crossval'])
-        results_columns = pd.Index(
-            [], name='n_components')
-        self.plsr_results = pd.DataFrame([], index=results_index,
-                                         columns=results_columns, dtype='object')
-
-    def plsr_fit(self, n_components, cv_percentage=10, **kwargs):
-        """
-        Perform partial least squares regression for one number of components.
-
-        Currently, one PLSR object is generated for every number of components.
-        I do not know if this is necessary, might be checked in the future.
-
-        Parameters
-        ----------
-        n_components : int
-            Number of components kept after PLSR.
-        cv_percentage : float, optional
-            Percentage of data used for cross-validation. The default is 10.
-        **kwargs :
-            All **kwargs from sklearn.cross_decomposition.PLSRegression are
-            allowed, see the documentation of those classes for details.
-
-        Returns
-        -------
-        DataFrame
-            Contains the predicted sample values ('y') of the training data
-            ('c'), the corresponding predictions ('y') after cross-validation
-            ('cv'), the coefficient of determination ('r2') for 'c' and 'cv',
-            and the mean squared error ('mse') for 'c' and 'cv' (given in the
-            DataFrame index). The DataFrame columns give the number of
-            components used to calculate the values.
-
-        """
-        # Create PLSR models
-        self.plsr_results.at[('plsr_objects', 'c'), n_components] = PLSRegression(
-            n_components=n_components, **kwargs)
-        self.plsr_results.at[('plsr_objects', 'c'), n_components].fit_transform(self.x, y=self.y)
-        # Predict sample values according to PLSR model
-        self.plsr_results.at[('y', 'c'), n_components] = self.predict(
-            self.x, n_components, scale=False)
-        # Cross-validate the PCR model
-        self.plsr_results.at[('y', 'cv'), n_components] = np.squeeze(
-            cross_val_predict(
-                self.plsr_results.at[('plsr_objects', 'c'), n_components], self.x, self.y,
-                cv=round(100/cv_percentage)))
-
-        # Calculate metrics for PLSR model
-        self.plsr_results.at[('r2', 'c'), n_components] = r2_score(
-            self.y, self.plsr_results.at[('y', 'c'), n_components],
-            multioutput='raw_values')
-        self.plsr_results.at[('r2', 'cv'), n_components] = r2_score(
-            self.y, self.plsr_results.at[('y', 'cv'), n_components],
-            multioutput='raw_values')
-        self.plsr_results.at[('mse', 'c'), n_components] = mean_squared_error(
-            self.y, self.plsr_results.at[('y', 'c'), n_components],
-            multioutput='raw_values')
-        self.plsr_results.at[('mse', 'cv'), n_components] = mean_squared_error(
-            self.y, self.plsr_results.at[('y', 'cv'), n_components],
-            multioutput='raw_values')
-
-        return self.plsr_results
-
-    def plsr_sweep(self, max_components=20, **kwargs):
-        """
-        Perform PLSR for all number of components between 1 and max_components.
-
-        Parameters
-        ----------
-        max_components : int, optional
-            The upper limit of components used for PLSR. The default is 20.
-        **kwargs :
-            The same **kwargs as in self.plsr_fit.
-
-        Returns
-        -------
-        DataFrame
-            See Docstring of self.plsr_fit.
-
-        """
-        for ii in range(1, max_components+1):
-            self.plsr_fit(ii, **kwargs)
-        return self.plsr_results
-
-    def predict(self, samples, n_components, scale=True):
-        """
-        Predict unknown sample target values.
-
-        Parameters
-        ----------
-        samples : ndarray
-            Sample data in the shape (n_samples, n_variables).
-        n_components : int
-            Number of components used in the PLSR model for the prediction.
-        scale : bool, optional
-            Defines if the sample data is scaled like the input data or not.
-            If called from within the class, should be False. Default is True.
-
-        Returns
-        -------
-        prediction : ndarray
-            Predicted target values in the shape (n_samples,) for a single
-            target or (n_samples, n_targets) for multiple targets.
-
-        """
-        if scale:
-            samples = self.scaler.transform(samples)
-
-        return np.squeeze(
-            self.plsr_results.at[('plsr_objects', 'c'), n_components].predict(samples))
-
-    def generate_plots(self, plot_names, response_number=0, **kwargs):
-        """
-        Generate some basic plots of partial least squares regression results.
-
-        Parameters
-        ----------
-        plot_names : list of str
-            List of plots to be generated. Allowed entries are
-            'actual_vs_pred' (actual target values vs. predicted values),
-            'r2_vs_comp' (coefficient of determination vs. number of
-            components), 'mse_vs_comp' (mean squared error vs. number of
-            components).
-        response_number : int, optional
-            Defines the index of the response from self.y to be plotted. 
-            Default is 0.
-        **kwargs :
-            n_components : int
-                Needed for plot_name 'actual_vs_pred'.
-            cv : boolean
-                State if cross-validation data should be plotted, too.
-                Default is False.
-        Returns
-        -------
-        plots : matplotlib plots
-            Plot objects, I do not know if anything can be done with this.
-
-        """
-        plots = []
-        plot_cv_data = kwargs.get('cv', False)
-        if 'actual_vs_pred' in plot_names:
-            n_components = kwargs.get('n_components')
-
-            if len(self.y.shape) == 1:
-                curr_y = self.y
-            else:
-                curr_y = self.y[:, response_number]
-                
-            if len(self.plsr_results.at[('y', 'c'), n_components].shape) == 1:
-                curr_c = self.plsr_results.at[('y', 'c'), n_components]
-            else:
-                curr_c = self.plsr_results.at[('y', 'c'), n_components][
-                    :, response_number]
-                
-            if len(self.plsr_results.at[('y', 'cv'), n_components].shape) == 1:
-                curr_cv = self.plsr_results.at[('y', 'cv'), n_components]
-            else:
-                curr_cv = self.plsr_results.at[('y', 'cv'), n_components][
-                    :, response_number]
-
-            z_c = np.polyfit(
-                curr_y, curr_c, 1)
-            z_cv = np.polyfit(
-                curr_y, curr_cv, 1)
-            with plt.style.context(('ggplot')):
-                fig1, ax1 = plt.subplots(figsize=(9, 5))
-                ax1.scatter(curr_y, curr_c, c='red', edgecolors='k')
-                if plot_cv_data:
-                    ax1.scatter(curr_y, curr_cv, c='blue', edgecolors='k')
-                    ax1.plot(curr_y, z_cv[1]+z_cv[0]*curr_y, c='blue',
-                             linewidth=1)
-                ax1.plot(curr_y, z_c[1]+z_c[0]*curr_y, c='red', linewidth=1)
-                ax1.plot(curr_y, curr_y, color='green', linewidth=1)
-                plt.title('$R^{2}$ (CV): '+str(
-                    self.plsr_results.loc[('r2', 'cv'), n_components]))
-                plt.xlabel('Measured')
-                plt.ylabel('Predicted')
-            plots.append(fig1)
-        if 'r2_vs_comp' in plot_names:
-            if len(self.plsr_results.loc['r2', 'c'][1]) == 1:
-                curr_c_r2 = self.plsr_results.loc['r2', 'c']
-            else:
-                curr_c_r2 = pd.DataFrame(
-                    self.plsr_results.loc['r2', 'c'].tolist()
-                    ).iloc[:, response_number]
-
-            if len(self.plsr_results.loc['r2', 'cv'][1]) == 1:
-                curr_cv_r2 = self.plsr_results.loc['r2', 'cv']
-            else:
-                curr_cv_r2 = pd.DataFrame(
-                    self.plsr_results.loc['r2', 'cv'].tolist()
-                    ).iloc[:, response_number]
-
-            with plt.style.context(('ggplot')):
-                fig2, ax2 = plt.subplots(figsize=(9, 5))
-                ax2.plot(
-                    curr_c_r2, linestyle='--', marker='o')
-                if plot_cv_data:
-                    ax2.plot(
-                        curr_cv_r2, linestyle='--', marker='o')
-                plt.ylabel('$R^{2}$')
-                plt.xlabel('Number of components')
-            plots.append(fig2)
-        if 'mse_vs_comp' in plot_names:
-            if len(self.plsr_results.loc['mse', 'c'][1]) == 1:
-                curr_c_mse = self.plsr_results.loc['mse', 'c']
-            else:
-                curr_c_mse = pd.DataFrame(
-                    self.plsr_results.loc['mse', 'c'].tolist()
-                    ).iloc[:, response_number]
-
-            if len(self.plsr_results.loc['mse', 'cv'][1]) == 1:
-                curr_cv_mse = self.plsr_results.loc['mse', 'cv']
-            else:
-                curr_cv_mse = pd.DataFrame(
-                    self.plsr_results.loc['mse', 'cv'].tolist()
-                    ).iloc[:, response_number]
-            
-            with plt.style.context(('ggplot')):
-                fig3, ax3 = plt.subplots(figsize=(9, 5))
-                ax3.plot(
-                    curr_c_mse, linestyle='--', marker='o')
-                if plot_cv_data:
-                    ax3.plot(
-                        curr_cv_mse, linestyle='--', marker='o')
-                plt.ylabel('MSE')
-                plt.xlabel('Number of components')
-            plots.append(fig3)
-
-        return plots
+# -*- coding: utf-8 -*-
+"""Multivariate regression objects for data analysis."""
+
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+import matplotlib.ticker as ticker
+from matplotlib.cm import rainbow
+from mpl_toolkits.mplot3d import Axes3D
+from sklearn.decomposition import PCA
+from sklearn.cross_decomposition import PLSRegression
+from sklearn.preprocessing import StandardScaler
+from sklearn.model_selection import cross_val_predict
+from sklearn.metrics import mean_squared_error, r2_score
+import statsmodels.api as sm
+
+from little_helpers.statsmodel_wrapper import statsmodel_wrapper
+
+
+class principal_component_regression():
+    """Class for performing principal component regression."""
+
+    def __init__(self, x, y=None, x_names=None, y_names=None,
+                 sample_names=None, scale_std=False):
+        """
+        Store input data and initialize results DataFrame.
+
+        Parameters
+        ----------
+        x : ndarray or pandas DataFrame
+            Sample training data in the shape (n_samples, n_variables). Data is
+            mean centered automatically, so it is not necessary to do that
+            before. If a pandas DataFrame, the index is used for sample naming
+            and the columns for variable naming, so potentially given values by
+            x_names and sample_names are ignored.
+        y : ndarray, pandas DataFrame or None, optional
+            Target values in the shape (n_samples,) for a single target or
+            (n_samples, n_targets) for multiple targets. Must be given if a
+            regression is to be performed, otherwise only a PCA on x makes
+            sense. Default is None in which case the regression results are
+            empty and meaningless. If a pandas DataFrame, the columns are used
+            for target naming, so potentially given values by y_names are
+            ignored.
+        x_names : list of str or None, optional
+            A list containing the names of the n_variables factors. Default is
+            None which results in numbered variables.
+        y_names : list of str or None, optional
+            A list containing the names of the n_targets responses. Default is
+            None which results in response names of 'response_1', 'response_2'
+            etc.
+        sample_names : list of str or None, optional
+            A list containing the n_samples sample names. Default is None which
+            results in sample names of 'sample_1', 'sample_2' etc.
+        scale_std : bool, optional
+            True means the data will be scaled to unit variance. Default is
+            False.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.scale_std = scale_std
+        self.n_samples, self.n_variables = x.shape
+        if y is None:
+            self.n_responses = 0
+        elif (y is not None) and (len(np.squeeze(y).shape) == 1):
+            self.n_responses = 1
+        else:
+            self.n_responses = y.shape[1]
+
+        if isinstance(y, np.ndarray) or (y is None):
+            if (y_names is not None) and (len(y_names) == self.n_responses):
+                self.y_names = y_names
+            elif y_names is None:
+                self.y_names = ['response_{}'.format(ii) for ii in np.arange(
+                    1, self.n_responses+1)]
+            else:
+                raise ValueError(
+                    'Number of response names does not match number of '
+                    'responses. Number of responses is {} and response name '
+                    'number is {}.'.format(self.n_responses, len(y_names)))
+
+            self.response_index = pd.Index(self.y_names, name='Response name')
+        elif isinstance(y, pd.DataFrame):
+            self.y_names = y.columns.to_numpy()
+            self.response_index = y.columns
+        else:
+            raise TypeError('y must either be np.ndarray or '
+                            'pd.DataFrame or None.')
+
+        if isinstance(x, np.ndarray):
+            if (x_names is not None) and (len(x_names) == self.n_variables):
+                self.x_names = x_names
+            elif x_names is None:
+                self.x_names = ['factor_{}'.format(ii) for ii in np.arange(
+                    1, self.n_variables+1)]
+            else:
+                raise ValueError(
+                    'Number of factor names does not match number of factors. '
+                    'Number of factors is {} and factor name number is '
+                    '{}.'.format(self.n_variables, len(x_names)))
+
+            if (sample_names is not None) and (
+                    len(sample_names) == self.n_samples):
+                self.sample_names = sample_names
+            elif sample_names is None:
+                self.sample_names = [
+                    'sample_{}'.format(ii) for ii in np.arange(
+                        1, self.n_samples+1)]
+            else:
+                raise ValueError(
+                    'Number of sample names does not match number of samples. '
+                    'Number of samples is {} and sample name number is {}'
+                    '.'.format(self.n_samples, len(sample_names)))
+
+            # Construct indices for later use in the DataFrames that collect
+            # the different PCA and PCR results
+            self.sample_index = pd.Index(self.sample_names, name='Sample name')
+            self.var_index = pd.Index(self.x_names, name='Variable name')
+        elif isinstance(x, pd.DataFrame):
+            self.sample_index = x.index
+            self.var_index = x.columns
+        else:
+            raise TypeError('x must either be np.ndarray or '
+                            'pd.DataFrame.')
+
+        y_c_index = pd.MultiIndex.from_product(
+            [self.response_index, self.sample_index.values],
+            names=['response name', 'sample number'])
+        metrics_index = pd.MultiIndex.from_product(
+            [self.response_index, ['r2_c', 'r2_cv', 'rmse_c', 'rmse_cv']],
+            names=['response name', 'metrics type'])
+
+        self.scaler = StandardScaler(with_std=self.scale_std)
+        self.x = pd.DataFrame(self.scaler.fit_transform(x),
+                              index=self.sample_index, columns=self.var_index)
+
+        if (y is not None) and (len(y) == len(x)):
+            self.y = pd.DataFrame(
+                y, index=self.sample_index, columns=self.response_index)
+        elif y is None:
+            self.y = None
+        else:
+            raise ValueError(
+                'Number of responses does not match number of samples. '
+                'Number of responses is {} and sample number is {}.'.format(
+                    self.n_responses, self.n_samples))
+
+        # List that will collect PCA component numbers that already
+        # were calculated
+        self.computed_components = [0]
+
+        self.pca_objects = pd.Series([], dtype='object')
+        self.pca_scores = pd.DataFrame([])
+        self.pca_eigenvalues = pd.Series([], dtype='float64')
+        self.pca_eigenvectors = pd.DataFrame([])
+        self.pca_loadings = pd.DataFrame([])
+        self.pca_explained_variance = pd.DataFrame([], columns=['each', 'cum'])
+        self.pca_results = pd.DataFrame([],
+                                        index=['Hotelling_T2', 'Q_residuals'])
+        self.pcr_models = pd.DataFrame([], dtype='object',
+                                       columns=self.response_index)
+        self.pcr_params = pd.DataFrame([], dtype='object',
+                                       columns=self.response_index)
+        self.pcr_used_pcs = pd.DataFrame([], dtype='object',
+                                         columns=self.response_index)
+        self.pcr_corr_coef = pd.DataFrame([], columns=self.response_index)
+        self.pcr_y_c = pd.DataFrame([], index=y_c_index)
+        self.pcr_y_cv = pd.DataFrame([], index=y_c_index)
+        self.pcr_metrics = pd.DataFrame([], index=metrics_index)
+
+    def perform_pca(self, n_components, **kwargs):
+        """
+        Actually perform the principal component analysis.
+
+        Parameters
+        ----------
+        n_components : int
+            Number of components kept after principal component analysis.
+        **kwargs :
+            All **kwargs from sklearn.decomposition.PCA are allowed, see the
+            documentation of that class for details.
+
+        Returns
+        -------
+        None.
+
+        """
+        # Check if PCA with n_components was already done before. If so, no
+        # calculation is performed because the data is already there.
+        if n_components not in self.computed_components:
+            self.pca_objects[n_components] = PCA(
+                n_components=n_components, **kwargs)
+            curr_scores = self.pca_objects[
+                    n_components].fit_transform(self.x)
+
+            # Check if any new information is generated by the calculations.
+            # If that is the case, scores, loadings, etc. are stored in the
+            # corresponding attributes.
+            if n_components > max(self.computed_components):
+                pc_index = pd.Index(np.arange(1, n_components+1),
+                                    name='PC number')
+
+                self.pca_scores = pd.DataFrame(curr_scores,
+                                               index=self.sample_index,
+                                               columns=pc_index)
+                self.pca_eigenvalues = pd.Series(
+                    self.pca_objects[n_components].explained_variance_,
+                    index=pc_index)
+                self.pca_eigenvectors = pd.DataFrame(
+                    self.pca_objects[n_components].components_.T,
+                    index=self.var_index,
+                    columns=pc_index)
+                self.pca_loadings = self.pca_eigenvectors * np.sqrt(
+                    self.pca_eigenvalues)
+                self.pca_explained_variance = pd.DataFrame(
+                    self.pca_objects[n_components].explained_variance_ratio_,
+                    columns=['each'], index=pc_index)
+                self.pca_explained_variance['cum'] = (
+                    self.pca_explained_variance['each'].cumsum())
+
+            self.pca_results[n_components] = pd.Series([], dtype='object')
+            # self.pc_loadings = self.components_.T
+            # * np.sqrt(pca.explained_variance_)
+
+            # Some PCA metrics are calculated. The results should be checked,
+            # calculation is still experimental. Also the attribute pca_results
+            # should be improved in the future.
+            # self.pca_results.at['Hotelling_T2', n_components] = np.array(
+            #     [sample.dot(self.pca_eigenvectors.loc[:, :n_components]).dot(
+            #         np.diag(self.pca_eigenvalues ** -1)).dot(
+            #             self.pca_eigenvectors.loc[:, :n_components].T).dot(
+            #                 sample.T) for sample in self.x])
+            # self.pca_results.at['Q_residuals', n_components] = np.array(
+            #     [sample.dot(np.identity(self.x.shape[1])-self.pca_eigenvectors.loc[
+            #         :, :n_components].dot(self.pca_eigenvectors.loc[
+            #             :, :n_components].T)).dot(
+            #                 sample.T) for sample in self.x])
+
+            self.computed_components.append(n_components)
+
+    def reconstruct_input(self):
+        """
+        Reconstruct the original input data.
+
+        The input data are reconstructed from the scaled data using the
+        standard deviation (if self.scale.std == true) and the
+        mean data from self.scaler. The input data is not needed within this
+        class, so the input data is not stored in order to save memory.
+
+        Returns
+        -------
+        reconstructed_input : pandas DataFrame
+            A DataFrame in the same format as self.x containing the input data.
+
+        """
+        reconstructed_input = pd.DataFrame(
+            self.scaler.inverse_transform(self.x.copy()),
+            index=self.x.index, columns=self.x.columns)
+        return reconstructed_input
+
+    def reconstruct_data(self, used_pcs):
+        """
+        Reconstruct the data from scores and eigenvectors.
+
+        The result is the original data without the contents of the PCA error
+        matrix, so can also be understood as a PCA based smoothing.
+
+        Parameters
+        ----------
+        used_pcs : int or list of int
+            If an int is given, the according number of principal components
+            is used for data reconstruction based on the order of explained
+            variance. If a list of int is given, the pricipal components given
+            in the list will be used for data reconstruction, based on the
+            explained variance ordering and the first PC having number 1.
+
+        Returns
+        -------
+        reconstructed_data : pandas DataFrame
+            The recomstructed data in the same format as self.x.
+
+        """
+        if isinstance(used_pcs, int):
+            max_component = used_pcs
+            pc_list = np.arange(1, used_pcs+1)
+        elif isinstance(used_pcs, list) and all(
+                [isinstance(ii, int) for ii in used_pcs]):
+            max_component = max(used_pcs)
+            pc_list = used_pcs
+        else:
+            raise TypeError('No valid value for used_pcs given. Allowed '
+                            'inputs are an integer or a list of integers.')
+
+        if max_component > max(self.computed_components):
+            self.perform_pca(max_component)
+
+        reconstructed_data = np.dot(
+            self.pca_scores.loc[:, pc_list],
+            self.pca_eigenvectors.loc[:, pc_list].T)
+
+        reconstructed_data = pd.DataFrame(
+            self.scaler.inverse_transform(reconstructed_data),
+            index=self.x.index, columns=self.x.columns)
+
+        return reconstructed_data
+
+    def pcr_fit(self, cv_percentage=20, mode='exp_var',
+                **kwargs):
+        """
+        Perform principal component regression for one number of components.
+
+        One PCA object is generated for every number of components.
+        This is necessary in order to be able to use the PCA transform method
+        in self.predict. For example, the predicted sample values ('y') of the
+        training data ('c'), the corresponding predictions ('y') after
+        cross-validation ('cv'), the coefficient of determination ('r2') for
+        'c' and 'cv', and the root mean squared error ('rmse') for 'c' and 'cv'
+        are calculated.
+
+        Parameters
+        ----------
+        cv_percentage : float, optional
+            Percentage of data used for cross-validation. The default is 20.
+        mode : str, optional
+            Determines if PCs used for regression are selected based on
+            explained variance only ('exp_var'), only based on corellation
+            with the data in self.y ('corr_coef'), or are given in a list based
+            on the exlained variance order ('list'). Default is 'exp_var'.
+        **kwargs :
+            All **kwargs from sklearn.decomposition.PCA are allowed, see the
+            documentation of that class for details.
+        **kwargs if mode=='exp_var':
+            n_components : int
+                The number of principal components used for the regression.
+        **kwargs if mode=='corr_coef':
+            n_components : int
+                See above.
+            max_components : int
+                The number of components ordered by increasing explained
+                variance which are used for calculation of corellation
+                coefficients. Default is 10.
+        **kwargs if mode=='list'
+            used_pcs : list of int
+                Gives the principal components used for regression based on the
+                order of explained variance.
+
+        Returns
+        -------
+        None
+
+        """
+        # PCA options
+        copy = kwargs.get('copy', True)
+        whiten = kwargs.get('whiten', False)
+        svd_solver = kwargs.get('svd_solver', 'auto')
+        tol = kwargs.get('tol', 0.0)
+        iterated_power = kwargs.get('iterated_power', 'auto')
+        random_state = kwargs.get('random_state', None)
+
+        # # LinearRegression options
+        # fit_intercept = kwargs.get('fit_intercept', True)
+        # normalize = kwargs.get('normalize', False)
+        # copy_X = kwargs.get('copy_X', True)
+        # n_jobs = kwargs.get('n_jobs', None)
+
+        if (mode == 'exp_var') or (mode == 'corr_coef'):
+            n_components = kwargs.get('n_components')
+        elif mode == 'list':
+            pc_list = kwargs.get('used_pcs')
+            n_components = max(pc_list)
+        else:
+            raise ValueError('Missing info on the number of components.')
+
+        # Perform the actual PCA
+        self.perform_pca(n_components, copy=copy, whiten=whiten,
+                         svd_solver=svd_solver, tol=tol,
+                         iterated_power=iterated_power,
+                         random_state=random_state)
+
+        # The number of components used for the calulation of the correlation
+        # coefficients can be bigger than the number of components used for
+        # the regression afterwards. Thus, e.g. a regression using 5 components
+        # can include e.g. the 10th component based on the explained variance
+        # ordering if max_components allows it.
+        if mode == 'corr_coef':
+            max_components = kwargs.get('max_components', 10)
+            self.perform_pca(max_components, copy=copy, whiten=whiten,
+                             svd_solver=svd_solver, tol=tol,
+                             iterated_power=iterated_power,
+                             random_state=random_state)
+
+        # In each iteration in the following for loop, a multilinear regression
+        # with the scores and only one of the responses given is performed. So
+        # the loop iterates over the individual responses. This results in
+        # one call of the fit and predict methods from the linear model objects
+        # per iteration. This is necessary for mode=='coord_coef' because for
+        # each response, different components may be used for regression.
+        for curr_y in self.y_names:
+            for curr_index, curr_scores in enumerate(
+                    self.pca_scores.values.T):
+                self.pcr_corr_coef.at[curr_index+1, curr_y] = np.abs(
+                    np.corrcoef(
+                        curr_scores, self.y[curr_y])[0, 1])
+
+            # Select score values to be used for the regression based on the
+            # mode given.
+            if mode == 'exp_var':
+                self.pcr_used_pcs.at[n_components, curr_y] = np.arange(
+                    1, n_components+1)
+            elif mode == 'corr_coef':
+                self.pcr_used_pcs.at[n_components, curr_y] = np.flip(
+                    np.argsort(self.pcr_corr_coef.loc[:, curr_y].values)[
+                        -n_components:])+1
+            elif mode == 'list':
+                self.pcr_used_pcs.at[n_components, curr_y] = np.array(pc_list)
+
+            fit_scores = self.pca_scores.loc[
+                :, self.pcr_used_pcs.at[n_components, curr_y]].values
+
+            # Build linear model
+            fit_scores = sm.add_constant(fit_scores)
+            self.pcr_models.at[n_components, curr_y] = sm.OLS(
+                self.y[curr_y], fit_scores)
+            self.pcr_params.at[n_components, curr_y] = (
+                self.pcr_models.at[n_components, curr_y].fit())
+            # Predict sample values according to PCR model
+            idx = pd.IndexSlice
+            self.pcr_y_c.loc[idx[curr_y, :], n_components] = (
+                self.pcr_models.at[n_components, curr_y].predict(
+                    self.pcr_params.at[n_components, curr_y].params,
+                    fit_scores))
+            # Cross-validate the PCR model
+            self.pcr_y_cv.loc[idx[curr_y, :], n_components] = (
+                cross_val_predict(statsmodel_wrapper(sm.OLS),
+                                  fit_scores, self.y[curr_y],
+                                  cv=round(100/cv_percentage)))
+            # Calculate metrics for PCR model
+            self.pcr_metrics.at[(curr_y, 'r2_c'), n_components] = r2_score(
+                self.y[curr_y], self.pcr_y_c.loc[
+                    idx[curr_y, :], n_components], multioutput='raw_values')
+            self.pcr_metrics.at[(curr_y, 'r2_cv'), n_components] = r2_score(
+                self.y[curr_y], self.pcr_y_cv.loc[
+                    idx[curr_y, :], n_components], multioutput='raw_values')
+            self.pcr_metrics.at[(curr_y, 'rmse_c'), n_components] = (
+                mean_squared_error(self.y[curr_y],
+                                   self.pcr_y_c.loc[idx[curr_y, :],
+                                                    n_components],
+                                   multioutput='raw_values', squared=False))
+            self.pcr_metrics.at[(curr_y, 'rmse_cv'), n_components] = (
+                mean_squared_error(self.y[curr_y],
+                                   self.pcr_y_cv.loc[idx[curr_y, :],
+                                                     n_components],
+                                   multioutput='raw_values', squared=False))
+
+    def pcr_sweep(self, sweep_components=20, cv_percentage=20, mode='exp_var',
+                  **kwargs):
+        """
+        Perform PCR for all number of components between 1 and n_components.
+
+        Parameters
+        ----------
+        sweep_components : int, optional
+            The upper limit of components used for PCR. The default is 20.
+        cv_percentage : float, optional
+            Percentage of data used for cross-validation. The default is 10.
+        mode : str, optional
+            Determines if PCs used for regression are selected based on
+            explained variance only ('exp_var'), only based on corellation
+            with the data in self.y ('corr_coef'), or are given in a list based
+            on the explained variance order ('list'). Default is 'exp_var'.
+        **kwargs :
+            The same **kwargs as in self.pcr_fit, only n_components must be
+            left out because that is controlled by the iterator of the loop
+            that repeatately calls self.pcr_fit.
+
+        Returns
+        -------
+        DataFrame
+            See Docstring of self.pcr_fit.
+
+        """
+        assert mode in ['exp_var', 'corr_coef'], (
+            'No valid option for mode given. Remember that \'list\' is not '
+            'allowed for this method because in this case information about '
+            'the PCs used must already be known.')
+
+        for ii in reversed(range(1, sweep_components+1)):
+            self.pcr_fit(cv_percentage=cv_percentage, mode=mode,
+                         n_components=ii, **kwargs)
+        # return self.pcr_results
+
+    def predict(self, samples, n_components, sample_names=None):
+        """
+        Predict unknown sample target values.
+
+        Currently works correct only for mode=='exp_var'. For
+        mode=='corr_coef', the tranformation has to be implemented independent
+        of the PCA object method.
+
+        Parameters
+        ----------
+        samples : ndarray
+            Sample data in the shape (n_samples, n_variables).
+        n_components : int
+            Number of components used in the PCR model for the prediction.
+        sample_names : list of str, optional
+            The names of the samples passed to the function for prediction.
+            Default is None resulting in numbered sample names.
+
+        Returns
+        -------
+        prediction : ndarray
+            Predicted target values in the shape (n_samples,) for a single
+            target or (n_samples, n_targets) for multiple targets.
+
+        """
+        if sample_names is None:
+            sample_names = ['Sample {}'.format(curr_idx)
+                            for curr_idx in range(len(samples))]
+
+        transformed_samples = self.pca_objects.at[n_components].transform(
+            self.scaler.transform(samples))
+
+        transformed_samples = sm.add_constant(
+            transformed_samples, has_constant='add')
+
+        prediction = pd.DataFrame([], columns=self.y_names, index=sample_names)
+        for curr_y in self.y_names:
+            prediction[curr_y] = (
+                self.pcr_models.at[n_components, curr_y].predict(
+                    self.pcr_params.at[n_components, curr_y].params,
+                    transformed_samples))
+        return prediction
+
+    def results_to_csv(self, folder=None):
+        if folder is None:
+            folder = ''
+        self.pca_loadings.to_csv(folder + '/pca_loadings.txt', sep='\t')
+        self.pca_explained_variance.to_csv(
+            folder + '/pca_explained_variance.txt', sep='\t')
+        self.pca_scores.to_csv(folder + '/pca_scores.txt', sep='\t')
+        self.pcr_corr_coef.to_csv(folder + '/pcr_corr_coef.txt', sep='\t')
+        self.pcr_metrics.to_csv(folder + '/pcr_metrics.txt', sep='\t')
+        self.pcr_used_pcs.to_csv(folder + '/pcr_used_pcs.txt', sep='\t')
+        self.pcr_y_c.to_csv(folder + '/pcr_y_c.txt', sep='\t')
+        self.pcr_y_cv.to_csv(folder + '/pcr_y_cv.txt', sep='\t')
+
+    def pca_biplot(self, pc_numbers=[1, 2], grouping=[None, None, None],
+                   scores_only=False, **kwargs):
+        """
+        Make a plot containing both the PCA loadings and scores.
+
+        Parameters
+        ----------
+        pc_numbers : list of int, optional, optional
+            Contains two entries giving the component indices to be used for
+            plotting, starting with 1 for the first principal component. The
+            default is [0,1].
+        grouping : list of str or None, optional
+            Contains three elements that must either be an element from
+            self.y_names or None. Defines a color (first entry), symbol
+            (second entry) and symbol fill style grouping (third entry) of
+            plotted scores based on the given targets. Default is [None, None,
+            None] where there is no grouping and only one color and one symbol
+            is used.
+        scores_only : boolean, optional
+            If True, the loadings will not be plotted, but only the scores.
+            Default is False.
+        **kwargs :
+            colors : list of matplotlib color codes
+                Must contain as many elements as levels present in the target
+                used for the color grouping. By default, the colors are given
+                by the matplotlib rainbow colormap.
+            markers : list og matplotlib markers, optional
+                Must contain as many elements as levels present in the target
+                used for symbol grouping. By default, a modified list obtained
+                by matplotlib.lines.Line2D.markers.keys() is used.
+            fill_styles : list of matplotlib marker fill styles, optional
+                Must contain as many elements as levels present in the target
+                used for fill style grouping. By default, a modified list
+                obtained by matplotlib.lines.Line2D.fillStyles is used.
+
+        Raises
+        ------
+        ValueError
+            DESCRIPTION.
+
+        Returns
+        -------
+        None.
+
+        """
+        # Define plot deltails
+        SMALL_SIZE = 6
+        MEDIUM_SIZE = 8
+        BIGGER_SIZE = 10
+        FIGSIZE = (3.1496, 2.3622)
+        DPI = 600
+        MARKERSIZE = 4
+
+        plt.rc('font', size=MEDIUM_SIZE)  # controls default text sizes
+        plt.rc('axes', titlesize=MEDIUM_SIZE)  # fontsize of the axes title
+        plt.rc('axes', labelsize=MEDIUM_SIZE)  # fontsize of the x and y labels
+        plt.rc('xtick', labelsize=MEDIUM_SIZE)  # fontsize of the tick labels
+        plt.rc('ytick', labelsize=MEDIUM_SIZE)  # fontsize of the tick labels
+        plt.rc('legend', fontsize=SMALL_SIZE)  # legend fontsize
+        plt.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
+
+        # First produce axis with two circles and the coordinate axes as dotted
+        # lines. This axis will be used to plot the PCA loadings.
+        fig1, ax1 = plt.subplots(1, figsize=FIGSIZE, dpi=DPI)
+        if not scores_only:
+            circle1 = plt.Circle((0, 0), 1, color='k', linestyle='--',
+                                 fill=False)
+            circle2 = plt.Circle((0, 0), np.sqrt(0.5), color='k',
+                                 linestyle='dotted', fill=False)
+            ax1.add_artist(circle1)
+            ax1.add_artist(circle2)
+            ax1.axhline(0, color='k', linestyle='dotted')
+            ax1.axvline(0, color='k', linestyle='dotted')
+            # Draw arrows starting at the origin for the PCA loadings and
+            # annotate them with the name of the corresponding target from
+            # self.y.
+            for (curr_loading1, curr_loading2, curr_var) in zip(
+                    self.pca_loadings[pc_numbers[0]],
+                    self.pca_loadings[pc_numbers[1]],
+                    self.pca_loadings.index.values):
+                ax1.arrow(0, 0, curr_loading1, curr_loading2, color='b',
+                          head_width=0.05, length_includes_head=True)
+                if curr_loading1 >= 0:
+                    ha = 'left'
+                else:
+                    ha = 'right'
+                # rotation = np.arctan(curr_loading2/curr_loading1)/(2*np.pi)*360
+                ax1.text(curr_loading1, curr_loading2, curr_var, ha=ha,
+                         va='center', rotation=0)
+            # Set limits and labels
+            ax1.set_xlim(-1.1, 1.1)
+            ax1.set_ylim(-1.1, 1.1)
+            ax1.set_xlabel('PC{} loadings'.format(pc_numbers[0]))
+            ax1.set_ylabel('PC{} loadings'.format(pc_numbers[1]))
+            ax1.set_facecolor('lightgrey')
+
+            # Set x and y tick spacing
+            ax1.xaxis.set_major_locator(ticker.MultipleLocator(0.4))
+            ax1.xaxis.set_minor_locator(ticker.MultipleLocator(0.1))
+            ax1.yaxis.set_major_locator(ticker.MultipleLocator(0.4))
+            ax1.yaxis.set_minor_locator(ticker.MultipleLocator(0.1))
+
+        # Add another axis on top of the previous one. The new axis will hold
+        # the PCA scores.
+        ax2 = fig1.add_subplot(111)
+
+        # If no grouping by color and/or symbol grouping contains only None
+        # so a simple scatter plot is made for the scores.
+        if not any(grouping):
+            ax2.plot(self.pca_scores[pc_numbers[0]],
+                     self.pca_scores[pc_numbers[1]],
+                     label='Scores', marker='o',
+                     markersize=MARKERSIZE, linestyle='none')
+            ax2.legend(loc='center right', bbox_to_anchor=(1.7, 0.5))
+
+        # If grouping by color and/or symbol the plotting procedure is a
+        # little more complicated, involves three nested for loops to
+        # accomodate the three grouping principles.
+        elif ((grouping[0] in self.y_names) or (grouping[0] is None)) and (
+                (grouping[1] in self.y_names) or (grouping[1] is None)) and (
+                    (grouping[2] in self.y_names) or (grouping[2] is None)):
+
+            # The values present in the y variables used for grouping are
+            # determined.
+            grouping_levels = []
+            grouping_levels.append(
+                self.y[grouping[0]].unique() if grouping[0] is not None
+                else None)
+            grouping_levels.append(
+                self.y[grouping[1]].unique() if grouping[1] is not None
+                else None)
+            grouping_levels.append(
+                self.y[grouping[2]].unique() if grouping[2] is not None
+                else None)
+
+            # Masks used for the later selection of data to be plotted are
+            # determined. This is done for one y variable used for grouping
+            # after the other (next three if-else statements).
+            grouping_masks = []
+            if grouping_levels[0] is not None:
+                grouping_masks.append([
+                    (self.y[grouping[0]] == curr_level).values
+                    for curr_level in grouping_levels[0]])
+            else:
+                grouping_masks.append(
+                    [np.full_like(self.y.index.values, True,
+                                  dtype='bool')])
+
+            if grouping_levels[1] is not None:
+                grouping_masks.append([
+                    (self.y[grouping[1]] == curr_level).values
+                    for curr_level in grouping_levels[1]])
+            else:
+                grouping_masks.append([np.full_like(
+                    self.y.index.values, True, dtype='bool')])
+
+            if grouping_levels[2] is not None:
+                grouping_masks.append([
+                    (self.y[grouping[2]] == curr_level).values
+                    for curr_level in grouping_levels[2]])
+            else:
+                grouping_masks.append([np.full_like(
+                    self.y.index.values, True, dtype='bool')])
+
+            # The 1D grouping masks from before are mixed together in one 3D
+            # array that is iterated over while plotting later on.
+            grouping_masks_all = (
+                np.array(grouping_masks[0]) *
+                np.array(grouping_masks[1])[:, np.newaxis]) * np.array(
+                    grouping_masks[2])[:, np.newaxis, np.newaxis]
+
+            # Colors, symbols and fill styles used for grouping are determined.
+            grouping_colors = kwargs.get(
+                'colors',
+                [rainbow(x) for x in np.linspace(0, 1,
+                                                 len(grouping_masks_all))])
+            grouping_symbols = kwargs.get(
+                'markers',
+                ['o', 'v', 'P', 'X', 'H', '<', '>', '1', '2', '3', '4',
+                 '8', 's', 'p', '*', 'h', '^', '+', 'x', 'D', 'd', '|',
+                 '_', '.', ',', 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11])
+            grouping_fillstyles = kwargs.get(
+                'fill_styles',
+                ['full', 'none', 'top', 'bottom', 'left', 'right'])
+
+            # Now the actual plotting starts by iterating through the
+            # previously calculated 3D mask array with three nested for loops.
+            idx = np.empty(3, dtype='int')
+            for idx[2], (curr_mask_2, curr_fillstyle) in enumerate(zip(
+                    grouping_masks_all, grouping_fillstyles)):
+                for idx[1], (curr_mask_1, curr_symbol) in enumerate(zip(
+                        curr_mask_2, grouping_symbols)):
+                    for idx[0], (curr_mask_0, curr_color) in enumerate(zip(
+                            curr_mask_1, grouping_colors)):
+
+                        label = ''
+                        for ii, curr_levels in enumerate(grouping_levels):
+                            if curr_levels is not None:
+                                label = label + str(curr_levels[idx[ii]]) + ', '
+                        label = label[:-2]
+                        # if grouping_levels[0] is None:
+                        #     label = str(grouping_levels[1][idx_0])
+                        # elif grouping_levels[1] is None:
+                        #     label = str(grouping_levels[0][idx_1])
+                        # elif grouping_levels[2] is None:
+                        #     label = str(grouping_levels[0][idx_2])
+                        # else:
+                        #     label = str(grouping_levels[0][idx_1])+', '+str(grouping_levels[1][idx_0])
+    
+                        ax2.plot(self.pca_scores.loc[curr_mask_0, pc_numbers[0]],
+                                 self.pca_scores.loc[curr_mask_0, pc_numbers[1]],
+                                 color=curr_color, marker=curr_symbol, label=label,
+                                 fillstyle=curr_fillstyle, linestyle='none',
+                                 markersize=MARKERSIZE)
+
+            legend_title = ''
+            for idx, curr_levels in enumerate(grouping_levels):
+                if curr_levels is not None:
+                    legend_title = legend_title + grouping[idx] + ', '
+            legend_title = legend_title[:-2]
+            ax2.legend(loc='center right', bbox_to_anchor= (1.8, 0.5), title=legend_title)
+        else:
+            raise ValueError('No valid grouping. Allowed values must be in'
+                             ' {} or None, but \'{}\' was given.'.format(
+                                 self.y_names, grouping))
+
+        # Score plot axis labels and positions are fixed and the top layer
+        # background is set to tranparent.
+        ax2.yaxis.set_ticks_position('right')
+        ax2.xaxis.set_ticks_position('top')
+        ax2.yaxis.set_label_position('right')
+        ax2.xaxis.set_label_position('top')
+        ax2.set_xlabel('PC{} scores'.format(pc_numbers[0]))
+        ax2.set_ylabel('PC{} scores'.format(pc_numbers[1]))
+        ax2.patch.set_alpha(0)
+
+        return fig1
+
+    def generate_plots(self, plot_names, response_number=0, **kwargs):
+        """
+        Generate some basic plots of principal component regression results.
+
+        Parameters
+        ----------
+        plot_names : list of str
+            List of plots to be generated. Allowed entries are
+            'actual_vs_pred' (actual target values vs. predicted values),
+            'r2_vs_comp' (coefficient of determination vs. number of
+            components), 'mse_vs_comp' (mean squared error vs. number of
+            components), 'biplot' (PCA loadings and scores in one plot),
+            'scoreplot_3D' (a 3D score plot using three principal components).
+        response_number : int, optional
+            Defines the index of the response from self.y to be plotted.
+            Default is 0.
+        **kwargs :
+            n_components : int
+                Needed for plot_name 'actual_vs_pred'. Currently, there is one
+                difficulty when using mode=='list' for self.pcr_fit. In this
+                case, the value for n_components has to be the highest number
+                in the list, otherwise a KeyError occurs.
+            cv : boolean
+                State if cross-validation data should be plotted, too.
+                Default is False.
+
+        Returns
+        -------
+        plots : matplotlib plots
+            Plot objects, I do not know if anything can be done with this.
+
+        """
+        plots = []
+        plot_cv_data = kwargs.get('cv', False)
+        idx = pd.IndexSlice
+        if 'actual_vs_pred' in plot_names:
+            n_components = kwargs.get('n_components')
+            curr_y = self.y[self.y_names[response_number]]
+            curr_c = self.pcr_y_c.loc[idx[self.y_names[response_number], :],
+                                      n_components]
+            curr_cv = self.pcr_y_cv.loc[idx[self.y_names[response_number], :],
+                                        n_components]
+            z_c = np.polyfit(
+                curr_y, curr_c, 1)
+            z_cv = np.polyfit(
+                curr_y, curr_cv, 1)
+            with plt.style.context(('ggplot')):
+                fig1, ax1 = plt.subplots(figsize=(9, 5))
+                ax1.scatter(curr_y, curr_c, c='red', edgecolors='k')
+                if plot_cv_data:
+                    ax1.scatter(curr_y, curr_cv, c='blue', edgecolors='k')
+                    ax1.plot(curr_y, z_cv[1]+z_cv[0]*curr_y, c='blue',
+                             linewidth=1)
+                ax1.plot(curr_y, z_c[1]+z_c[0]*curr_y, c='red', linewidth=1)
+                ax1.plot(curr_y, curr_y, color='green', linewidth=1)
+                plt.title('$R^{2}$ (CV): '+str(
+                    self.pcr_metrics.at[(self.y_names[response_number],
+                                         'r2_cv'), n_components]))
+                plt.xlabel('Measured')
+                plt.ylabel('Predicted')
+            plots.append(fig1)
+        if 'r2_vs_comp' in plot_names:
+            curr_c_r2 = self.pcr_metrics.loc[(self.y_names[response_number],
+                                              'r2_c')]
+            curr_cv_r2 = self.pcr_metrics.loc[(self.y_names[response_number],
+                                               'r2_cv')]
+
+            with plt.style.context(('ggplot')):
+                fig2, ax2 = plt.subplots(figsize=(9, 5))
+                ax2.plot(
+                    curr_c_r2, linestyle='--', marker='o')
+                if plot_cv_data:
+                    ax2.plot(
+                        curr_cv_r2, linestyle='--', marker='o')
+                plt.ylabel('$R^{2}$')
+                plt.xlabel('Number of components')
+            plots.append(fig2)
+        if 'mse_vs_comp' in plot_names:
+            curr_c_rmse = self.pcr_metrics.loc[(self.y_names[response_number],
+                                                'rmse_c')]
+            curr_cv_rmse = self.pcr_metrics.loc[(self.y_names[response_number],
+                                                 'rmse_cv')]
+
+            with plt.style.context(('ggplot')):
+                fig3, ax3 = plt.subplots(figsize=(9, 5))
+                ax3.plot(
+                    curr_c_rmse, linestyle='--', marker='o')
+                if plot_cv_data:
+                    ax3.plot(
+                        curr_cv_rmse, linestyle='--', marker='o')
+                plt.ylabel('RMSE')
+                plt.xlabel('Number of components')
+            plots.append(fig3)
+        if 'expvar_vs_corrcoef' in plot_names:
+            curr_expvar = self.pca_explained_variance['each']
+            curr_corrcoef = self.pcr_corr_coef[self.y_names[response_number]]
+
+            with plt.style.context(('ggplot')):
+                fig4, ax4 = plt.subplots(figsize=(9, 5))
+                ax4.scatter(
+                    curr_expvar, curr_corrcoef)
+                for ii, txt in enumerate(curr_expvar.index):
+                    ax4.annotate(txt, (curr_expvar[ii+1], curr_corrcoef[ii+1]))
+                ax4.set_yscale('log')
+                ax4.set_xscale('log')
+                plt.ylabel('Correlation coefficients')
+                plt.xlabel('Explained variance')
+                plt.title(self.y_names[response_number])
+            plots.append(fig4)
+        if 'scoreplot_3D' in plot_names:
+            pc_numbers = kwargs.get('pc_numbers', [0, 1, 2])
+            grouping = kwargs.get('grouping', [None, None])
+            fig1 = plt.figure()
+            ax2 = Axes3D(fig1)
+            marker_size = 200
+            # If no grouping by color and/or symbol grouping contains only None
+            # so a simple scatter plot is made for the scores.
+            if not any(grouping):
+                ax2.scatter(self.pca_scores[pc_numbers[0]],
+                            self.pca_scores[pc_numbers[1]],
+                            self.pca_scores[pc_numbers[2]],
+                            label='Scores', s=marker_size)
+                ax2.legend(loc='lower left', bbox_to_anchor= (1.1, 0))
+            # If grouping by color and/or symbol the plotting procedure is a
+            # little more complicated, involves two nested for loops to
+            # accomodate the two grouping principles.
+            elif ((grouping[0] in self.y_names) or (grouping[0] is None)) and (
+                    (grouping[1] in self.y_names) or (grouping[1] is None)):
+                grouping_levels_0 = self.y[grouping[0]].unique() if grouping[0] is not None else None
+                grouping_levels_1 = self.y[grouping[1]].unique() if grouping[1] is not None else None
+
+                if grouping_levels_0 is not None:
+                    grouping_masks_0 = [
+                        (self.y[grouping[0]]==curr_level).values
+                        for curr_level in grouping_levels_0]
+                else:
+                    grouping_masks_0 = [np.full_like(self.y.index.values, True, dtype='bool')]
+
+                if grouping_levels_1 is not None:
+                    grouping_masks_1 = [
+                        (self.y[grouping[1]]==curr_level).values
+                        for curr_level in grouping_levels_1]
+                else:
+                    grouping_masks_1 = [np.full_like(self.y.index.values, True, dtype='bool')]
+
+                grouping_masks_all = np.array(grouping_masks_1) * np.array(grouping_masks_0)[:, np.newaxis]
+                grouping_colors = kwargs.get(
+                    'colors',
+                    [rainbow(x) for x in np.linspace(0, 1,
+                                                     len(grouping_masks_all))])
+                #['k', 'b', 'r']
+                grouping_symbols = kwargs.get(
+                    'markers',
+                    ['o', 'v', 'P', 'X', 'H', '<', '>', '1', '2', '3', '4',
+                     '8', 's', 'p', '*', 'h', '^', '+', 'x', 'D', 'd', '|',
+                     '_', '.', ',', 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11])
+                for idx_1, (curr_mask_1, curr_color) in enumerate(zip(
+                        grouping_masks_all, grouping_colors)):
+                    for idx_0, (curr_mask_0, curr_symbol) in enumerate(zip(
+                            curr_mask_1, grouping_symbols)):
+
+                        if grouping_levels_0 is None:
+                            label = str(grouping_levels_1[idx_0])
+                            legend_title = grouping[1]
+                        elif grouping_levels_1 is None:
+                            label = str(grouping_levels_0[idx_1])
+                            legend_title = grouping[0]
+                        else:
+                            label = str(grouping_levels_0[idx_1])+', '+str(grouping_levels_1[idx_0])
+                            legend_title = grouping[0]+', '+grouping[1]
+
+                        ax2.scatter(self.pca_scores.loc[curr_mask_0, pc_numbers[0]],
+                                    self.pca_scores.loc[curr_mask_0, pc_numbers[1]],
+                                    self.pca_scores.loc[curr_mask_0, pc_numbers[2]],
+                                    color=curr_color, marker=curr_symbol,
+                                    s=marker_size, label=label)
+
+                        ax2.legend(loc='upper left', bbox_to_anchor= (1.15, 1), title=legend_title)
+            else:
+                raise ValueError('No valid grouping. Allowed values must be in'
+                                 ' {} or None, but \'{}\' was given.'.format(
+                                     self.y_names, grouping))
+            ax2.yaxis.set_ticks_position('top')
+            ax2.xaxis.set_ticks_position('top')
+            ax2.yaxis.set_label_position('top')
+            ax2.xaxis.set_label_position('top')
+            ax2.set_xlabel('PC{} scores'.format(pc_numbers[0]))
+            ax2.set_ylabel('PC{} scores'.format(pc_numbers[1]))
+            ax2.set_zlabel('PC{} scores'.format(pc_numbers[2]))
+            ax2.patch.set_alpha(0)
+
+        return plots
+
+
+class pls_regression():
+    """Class for performing principal component regression."""
+
+    def __init__(self, x, y, scale_std=False):
+        """
+        Store input data and initialize results DataFrame.
+
+        Parameters
+        ----------
+        x : ndarray
+            Sample training data in the shape (n_samples, n_variables).
+        y : ndarray
+            Target values in the shape (n_samples,) for a single target or
+            (n_samples, n_targets) for multiple targets.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.x_raw = x
+        self.y = y
+        self.scale_std = scale_std
+
+        self.scaler = StandardScaler(with_std=self.scale_std)
+        self.x = self.scaler.fit_transform(self.x_raw)
+
+        results_index = pd.MultiIndex.from_product(
+            [['plsr_objects', 'y', 'r2', 'mse', 'Hotelling_T2'], ['c', 'cv']],
+            names=['result_name', 'cal_or_crossval'])
+        results_columns = pd.Index(
+            [], name='n_components')
+        self.plsr_results = pd.DataFrame([], index=results_index,
+                                         columns=results_columns, dtype='object')
+
+    def plsr_fit(self, n_components, cv_percentage=10, **kwargs):
+        """
+        Perform partial least squares regression for one number of components.
+
+        Currently, one PLSR object is generated for every number of components.
+        I do not know if this is necessary, might be checked in the future.
+
+        Parameters
+        ----------
+        n_components : int
+            Number of components kept after PLSR.
+        cv_percentage : float, optional
+            Percentage of data used for cross-validation. The default is 10.
+        **kwargs :
+            All **kwargs from sklearn.cross_decomposition.PLSRegression are
+            allowed, see the documentation of those classes for details.
+
+        Returns
+        -------
+        DataFrame
+            Contains the predicted sample values ('y') of the training data
+            ('c'), the corresponding predictions ('y') after cross-validation
+            ('cv'), the coefficient of determination ('r2') for 'c' and 'cv',
+            and the mean squared error ('mse') for 'c' and 'cv' (given in the
+            DataFrame index). The DataFrame columns give the number of
+            components used to calculate the values.
+
+        """
+        # Create PLSR models
+        self.plsr_results.at[('plsr_objects', 'c'), n_components] = PLSRegression(
+            n_components=n_components, **kwargs)
+        self.plsr_results.at[('plsr_objects', 'c'), n_components].fit_transform(self.x, y=self.y)
+        # Predict sample values according to PLSR model
+        self.plsr_results.at[('y', 'c'), n_components] = self.predict(
+            self.x, n_components, scale=False)
+        # Cross-validate the PCR model
+        self.plsr_results.at[('y', 'cv'), n_components] = np.squeeze(
+            cross_val_predict(
+                self.plsr_results.at[('plsr_objects', 'c'), n_components], self.x, self.y,
+                cv=round(100/cv_percentage)))
+
+        # Calculate metrics for PLSR model
+        self.plsr_results.at[('r2', 'c'), n_components] = r2_score(
+            self.y, self.plsr_results.at[('y', 'c'), n_components],
+            multioutput='raw_values')
+        self.plsr_results.at[('r2', 'cv'), n_components] = r2_score(
+            self.y, self.plsr_results.at[('y', 'cv'), n_components],
+            multioutput='raw_values')
+        self.plsr_results.at[('mse', 'c'), n_components] = mean_squared_error(
+            self.y, self.plsr_results.at[('y', 'c'), n_components],
+            multioutput='raw_values')
+        self.plsr_results.at[('mse', 'cv'), n_components] = mean_squared_error(
+            self.y, self.plsr_results.at[('y', 'cv'), n_components],
+            multioutput='raw_values')
+
+        return self.plsr_results
+
+    def plsr_sweep(self, max_components=20, **kwargs):
+        """
+        Perform PLSR for all number of components between 1 and max_components.
+
+        Parameters
+        ----------
+        max_components : int, optional
+            The upper limit of components used for PLSR. The default is 20.
+        **kwargs :
+            The same **kwargs as in self.plsr_fit.
+
+        Returns
+        -------
+        DataFrame
+            See Docstring of self.plsr_fit.
+
+        """
+        for ii in range(1, max_components+1):
+            self.plsr_fit(ii, **kwargs)
+        return self.plsr_results
+
+    def predict(self, samples, n_components, scale=True):
+        """
+        Predict unknown sample target values.
+
+        Parameters
+        ----------
+        samples : ndarray
+            Sample data in the shape (n_samples, n_variables).
+        n_components : int
+            Number of components used in the PLSR model for the prediction.
+        scale : bool, optional
+            Defines if the sample data is scaled like the input data or not.
+            If called from within the class, should be False. Default is True.
+
+        Returns
+        -------
+        prediction : ndarray
+            Predicted target values in the shape (n_samples,) for a single
+            target or (n_samples, n_targets) for multiple targets.
+
+        """
+        if scale:
+            samples = self.scaler.transform(samples)
+
+        return np.squeeze(
+            self.plsr_results.at[('plsr_objects', 'c'), n_components].predict(samples))
+
+    def generate_plots(self, plot_names, response_number=0, **kwargs):
+        """
+        Generate some basic plots of partial least squares regression results.
+
+        Parameters
+        ----------
+        plot_names : list of str
+            List of plots to be generated. Allowed entries are
+            'actual_vs_pred' (actual target values vs. predicted values),
+            'r2_vs_comp' (coefficient of determination vs. number of
+            components), 'mse_vs_comp' (mean squared error vs. number of
+            components).
+        response_number : int, optional
+            Defines the index of the response from self.y to be plotted. 
+            Default is 0.
+        **kwargs :
+            n_components : int
+                Needed for plot_name 'actual_vs_pred'.
+            cv : boolean
+                State if cross-validation data should be plotted, too.
+                Default is False.
+        Returns
+        -------
+        plots : matplotlib plots
+            Plot objects, I do not know if anything can be done with this.
+
+        """
+        plots = []
+        plot_cv_data = kwargs.get('cv', False)
+        if 'actual_vs_pred' in plot_names:
+            n_components = kwargs.get('n_components')
+
+            if len(self.y.shape) == 1:
+                curr_y = self.y
+            else:
+                curr_y = self.y[:, response_number]
+                
+            if len(self.plsr_results.at[('y', 'c'), n_components].shape) == 1:
+                curr_c = self.plsr_results.at[('y', 'c'), n_components]
+            else:
+                curr_c = self.plsr_results.at[('y', 'c'), n_components][
+                    :, response_number]
+                
+            if len(self.plsr_results.at[('y', 'cv'), n_components].shape) == 1:
+                curr_cv = self.plsr_results.at[('y', 'cv'), n_components]
+            else:
+                curr_cv = self.plsr_results.at[('y', 'cv'), n_components][
+                    :, response_number]
+
+            z_c = np.polyfit(
+                curr_y, curr_c, 1)
+            z_cv = np.polyfit(
+                curr_y, curr_cv, 1)
+            with plt.style.context(('ggplot')):
+                fig1, ax1 = plt.subplots(figsize=(9, 5))
+                ax1.scatter(curr_y, curr_c, c='red', edgecolors='k')
+                if plot_cv_data:
+                    ax1.scatter(curr_y, curr_cv, c='blue', edgecolors='k')
+                    ax1.plot(curr_y, z_cv[1]+z_cv[0]*curr_y, c='blue',
+                             linewidth=1)
+                ax1.plot(curr_y, z_c[1]+z_c[0]*curr_y, c='red', linewidth=1)
+                ax1.plot(curr_y, curr_y, color='green', linewidth=1)
+                plt.title('$R^{2}$ (CV): '+str(
+                    self.plsr_results.loc[('r2', 'cv'), n_components]))
+                plt.xlabel('Measured')
+                plt.ylabel('Predicted')
+            plots.append(fig1)
+        if 'r2_vs_comp' in plot_names:
+            if len(self.plsr_results.loc['r2', 'c'][1]) == 1:
+                curr_c_r2 = self.plsr_results.loc['r2', 'c']
+            else:
+                curr_c_r2 = pd.DataFrame(
+                    self.plsr_results.loc['r2', 'c'].tolist()
+                    ).iloc[:, response_number]
+
+            if len(self.plsr_results.loc['r2', 'cv'][1]) == 1:
+                curr_cv_r2 = self.plsr_results.loc['r2', 'cv']
+            else:
+                curr_cv_r2 = pd.DataFrame(
+                    self.plsr_results.loc['r2', 'cv'].tolist()
+                    ).iloc[:, response_number]
+
+            with plt.style.context(('ggplot')):
+                fig2, ax2 = plt.subplots(figsize=(9, 5))
+                ax2.plot(
+                    curr_c_r2, linestyle='--', marker='o')
+                if plot_cv_data:
+                    ax2.plot(
+                        curr_cv_r2, linestyle='--', marker='o')
+                plt.ylabel('$R^{2}$')
+                plt.xlabel('Number of components')
+            plots.append(fig2)
+        if 'mse_vs_comp' in plot_names:
+            if len(self.plsr_results.loc['mse', 'c'][1]) == 1:
+                curr_c_mse = self.plsr_results.loc['mse', 'c']
+            else:
+                curr_c_mse = pd.DataFrame(
+                    self.plsr_results.loc['mse', 'c'].tolist()
+                    ).iloc[:, response_number]
+
+            if len(self.plsr_results.loc['mse', 'cv'][1]) == 1:
+                curr_cv_mse = self.plsr_results.loc['mse', 'cv']
+            else:
+                curr_cv_mse = pd.DataFrame(
+                    self.plsr_results.loc['mse', 'cv'].tolist()
+                    ).iloc[:, response_number]
+            
+            with plt.style.context(('ggplot')):
+                fig3, ax3 = plt.subplots(figsize=(9, 5))
+                ax3.plot(
+                    curr_c_mse, linestyle='--', marker='o')
+                if plot_cv_data:
+                    ax3.plot(
+                        curr_cv_mse, linestyle='--', marker='o')
+                plt.ylabel('MSE')
+                plt.xlabel('Number of components')
+            plots.append(fig3)
+
+        return plots
```

### Comparing `pyDataFitting-0.0.2/src/pyDataFitting/polynomial_regression.py` & `pyDataFitting-0.0.3/src/pyDataFitting/polynomial_regression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,481 +1,516 @@
-# -*- coding: utf-8 -*-
-
-import numpy as np
-from scipy.optimize import differential_evolution
-
-from little_helpers.array_tools import segment_xy_values
-
-
-def segment_regression(x_values, y_values, poly_orders, border_bounds,
-                       y_bounds=None, slope_bounds=None, max_iter=1000):
-    """
-    Do a regression with a piecewise polynomial fit on the segmentation points.
-
-    This method is useful if the segmentation points for a piecewise polynomial
-    fit are not exactly known, but can be guessed to some extent. Generally, it
-    is possible to give the whole data range as boundaries, so effectively no
-    boundary conditions are passed to the fit, however this is not recommended
-    and may result in an error message. It is better to provide separated
-    boundaries for the segmentation points.
-
-    Parameters
-    ----------
-    x_values : ndarray
-        A 1D array with the length M holding the independent varibale used for
-        the fit.
-    y_values : ndarray
-        A 1D array with the length M holding the dependent varibale used for
-        the fit.
-    poly_orders : list of int
-        A list containing the polynomial orders used for the fit. Must contain
-        one more element than border_bounds.
-    border_bounds : list of tuples
-        The range the fit varies the x values of the segmentation points. Each
-        tuple has two entries and defines the range for one segmentation point,
-        so the list has as many tuples as segmentation points are present. The
-        first value in the tuple is the lower boundary, the second the upper
-        boundary for the respective segmentation point.
-    y_bounds : None, or list of tuples or None, optional
-        The range the fit varies the y values of the segmentation points. Each
-        tuple has two entries and defines the range for one segmentation point,
-        so the list has as many tuples or None as segmentation points are
-        present. The first value in the tuple is the lower boundary, the second
-        the upper boundary for the respective segmentation point. Default is
-        None which means no point constraint at the segmentation point.
-    slope_bounds : None, or list of tuples or None, optional
-        The range the fit varies the slope values at the segmentation points.
-        Each tuple has two entries and defines the range for one segmentation
-        point, so the list has as many tuples or None as segmentation points
-        are present. The first value in the tuple is the lower boundary, the
-        second the upper boundary for the respective segmentation point.
-        Default is None which means no point constraint at the segmentation
-        point.
-    max_iter : int, optional
-        The maximum numer of iterations performed in the iterative fit
-        algorithm (currently differential evolution). The default is 1000.
-
-    Returns
-    -------
-    y_fit : ndarray
-        A 1D array containing the y values of the fit at the x values given in
-        x_values.
-    coefs : list of ndarray
-        A list containing the coefficient vectors of the polynomial equations
-        for the data segments. Each list entry can be passed directly to
-        np.polynomial.polynomial.polyval to calculate the polynomial values.
-    evo_fit : scipy.optimize.OptimizeResult
-        The result of the differential evolution fit.
-
-    """
-    # border_bounds, y_bounds and slope_bounds are mixed together in boundaries
-    # because the parameters for differential_evolution have to be one 1D
-    # array. constraint_types passes a key to sum_of_squared_residuals to
-    # identify which parameter is which kind of constraint.
-    boundaries = []
-    constraint_types = []
-    for idx, curr_border_bounds in enumerate(border_bounds):
-        boundaries.append(curr_border_bounds)
-        constraint_types.append('b')
-        if (y_bounds is not None) and (y_bounds[idx] is not None):
-            boundaries.append(y_bounds[idx])
-            constraint_types.append('y')
-        if (slope_bounds is not None) and (slope_bounds[idx] is not None):
-            boundaries.append(slope_bounds[idx])
-            constraint_types.append('s')
-
-    # The evolutionary fit itself.
-    evo_fit = differential_evolution(
-        sum_of_squared_residuals, bounds=boundaries,
-        args=(x_values, y_values, poly_orders, constraint_types),
-        maxiter=max_iter)
-
-    # segment_borders and y_at_borders are extracted from the 1D evo_fit
-    # array so that they can be used in the calculation of the fit curve.
-    segment_borders, y_at_borders, slope_at_borders = decode_fit_par(
-        evo_fit.x, constraint_types)
-
-    y_fit, coefs = piecewise_polynomial_fit(
-        x_values, y_values, segment_borders, poly_orders,
-        y_at_borders=y_at_borders, slope_at_borders=slope_at_borders)
-
-    return (y_fit, coefs, evo_fit)
-
-
-def sum_of_squared_residuals(fit_par, x_values, y_values, poly_orders,
-                             constraint_types):
-    """
-    Objective function to be minimized during segment_regression.
-
-    The function is called by differential_evolution.
-
-    Parameters
-    ----------
-    fit_par : ndarray
-        A 1D array containing the fit parameters. Contains segment_borders,
-        and possibly y_at_borders and slope at borders directly following the
-        corresponding segment border.
-    x_values : ndarray
-        A 1D array with the length M holding the independent varibale used for
-        the fit.
-    y_values : ndarray
-        A 1D array with the length M holding the dependent varibale used for
-        the fit.
-    poly_orders : list of int
-        A list containing the polynomial orders used for the fit. Must contain
-        one more element than segment_borers contained in fit_par.
-    constraint_types : list of str
-        Encodes which value in fit_par is which kind of constraint. 'b' means
-        segmentation border, 'y' means a common y value of adjacent segments,
-        and 's' means a common slope of adjacent segments.
-
-    Returns
-    -------
-    sum of squared residuals
-        The value to be minimized during the fit.
-
-    """
-    segment_borders, y_at_borders, slope_at_borders = decode_fit_par(
-        fit_par, constraint_types)
-
-    curr_values, curr_coefs = piecewise_polynomial_fit(
-        x_values, y_values, segment_borders, poly_orders,
-        y_at_borders=y_at_borders, slope_at_borders=slope_at_borders)
-
-    return np.sum((curr_values - y_values)**2)
-
-
-def decode_fit_par(fit_par, constraint_types):
-    """
-    Translate the 1D array of fit parameters to individual lists.
-
-    The fit paramters are sorted into the lists segment_borders, y_at_borders
-    slope_at_borders based on the strings given in constraint_types. The three
-    lists are used as arguments in piecewise_polynomial_fit called in the
-    functions sum_of_squared_residuals and segment_regression.
-
-    Parameters
-    ----------
-    fit_par : ndarray
-        A 1D array containing the fit parameters. Contains segment_borders,
-        and possibly y_at_borders and slope at borders directly following the
-        corresponding segment border.
-    constraint_types : list of str
-        Encodes which value in fit_par is which kind of constraint. 'b' means
-        segmentation border, 'y' means a common y value of adjacent segments,
-        and 's' means a common slope of adjacent segments.
-
-    Returns
-    -------
-    segment_borders, y_at_borders, slope_at_borders
-        The arguments used for piecewise_polynomial_fit, see its docstring for
-        details.
-
-    """
-    # Fit parameters from segment_regression and sum_of_squared_residuals are
-    # reordered to be understood by piecewise_polynomial_fit.
-    segment_borders = []
-    y_at_borders = []
-    slope_at_borders = []
-    for idx, curr_type in enumerate(constraint_types):
-        if curr_type == 'b':
-            segment_borders.append(fit_par[idx])
-            y_at_borders.append(None)
-            slope_at_borders.append(None)
-        if curr_type == 'y':
-            y_at_borders[-1] = fit_par[idx]
-        if curr_type == 's':
-            slope_at_borders[-1] = fit_par[idx]
-
-    return (segment_borders, y_at_borders, slope_at_borders)
-
-
-def piecewise_polynomial_fit(x_values, y_values, segment_borders,
-                             poly_orders, y_at_borders=None,
-                             slope_at_borders=None):
-    """
-    Piecewise polynomial fit using polynomial_fit for the data segments.
-
-    Since polynomial_fit allows constraints such as fixed points or fixed
-    slopes, this can be used for the piecewise polynomial fit as well. By
-    default, the data is divided into segments at the values given in
-    segment_borders and the segments are fitted each by a polynomial fit using
-    the least squares method. Thus, discontinuities will arise at the segment
-    borders between the fits of the segments. These discontinuities can be
-    suppressed by applying equality constraints to the fits that force the fit
-    curves through specific points or to have specific slopes. The method
-    allows to use polynomials of different orders for the different segments.
-
-    Parameters
-    ----------
-    x_values : ndarray
-        A 1D array with the length M holding the independent varibale used for
-        the fit.
-    y_values : ndarray
-        A 1D array with the length M holding the dependent varibale used for
-        the fit.
-    segment_borders : list of int or float
-        The values with respect to x_values at which the data is divided into
-        segments. An arbitrary number of segment borders may be given, but it
-        is recommended to provide a sorted list in order to avoid confusion.
-        If the list is not sorted, it will be sorted and the sorting is also
-        applied to y_at_borders and slope_at_borders (if they are given), but
-        not to poly_orders.
-    poly_orders : list of int
-        A list containing the polynomial orders used for the fit. Must contain
-        one more element than segment_borders.
-    y_at_borders : None, or list of float or None, optional
-        May contain dependent variable values used as equality constraints at
-        the segment borders. The fits of both touching segments are forced
-        through the point given by the pair (segment border, y_at_border). The
-        list entries may also be None to state that at a certain segment
-        border, no constraint is to be applied. The default is None which means
-        that no contraints are applied for any segment border.
-    slope_at_borders : None, or list of float or None, optional
-        Analogous to y_at_borders, with the difference that here, fixed slopes
-        at the segment borders are given. The default is None.
-
-    Returns
-    -------
-    y_fit : ndarray
-        A 1D array containing the y values of the fit at the x values given in
-        x_values.
-    coefs : list of ndarray
-        A list containing the coefficient vectors of the polynomial equations
-        for the data segments. Each list entry can be passed directly to
-        np.polynomial.polynomial.polyval to calculate the polynomial values.
-
-    """
-
-    sort_order = np.argsort(segment_borders)
-    segment_borders = np.array(segment_borders)[sort_order]
-
-    # Fixed points are given by the x values in segment_borders and the y
-    # values given in y_at_borders and are collected in tuples of the two
-    # numbers or in empty tuples if no fixed point is used for the given
-    # segment border.
-    if y_at_borders is not None:
-        y_at_borders = np.array(y_at_borders)[sort_order]
-        fixed_points = [()]  # for left edge
-        for x, y in zip(segment_borders, y_at_borders):
-            curr_point = (x, y) if y is not None else ()
-            fixed_points.append(curr_point)
-        fixed_points.append(())  # for right edge
-    else:
-        fixed_points = [()] * (len(segment_borders) + 2)
-
-    # Fixed slopes are given by the x values in segment_borders and the slope
-    # values given in slope_at_borders and are collected in tuples of the two
-    # numbers or in empty tuples if no fixed slope is used for the given
-    # segment border.
-    if slope_at_borders is not None:
-        fixed_slopes = [()]  # for left edge
-        for x, slope in zip(segment_borders, slope_at_borders):
-            curr_slope = (x, slope) if slope is not None else ()
-            fixed_slopes.append(curr_slope)
-        fixed_slopes.append(())  # for right edge
-    else:
-        fixed_slopes = [()] * (len(segment_borders) + 2)
-
-    x_segments, y_segments = segment_xy_values(x_values, segment_borders,
-                                               y_values=y_values)
-
-    fit_segments = []
-    coefs = []
-    # In the loop, the segments are fitted individually, one in each iteration.
-    for curr_x, curr_y, curr_order, left_fix, right_fix, left_slope, right_slope in zip(
-            x_segments, y_segments, poly_orders, fixed_points[:-1],
-            fixed_points[1:], fixed_slopes[:-1], fixed_slopes[1:]):
-        # The fixed points and slopes are translated into the syntax understood
-        # by polynomial_fit.
-        curr_fixed = []
-        if left_fix:
-            curr_fixed.append(left_fix)
-        if right_fix:
-            curr_fixed.append(right_fix)
-        if not curr_fixed:
-            curr_fixed = None
-        curr_slope = []
-        if left_slope:
-            curr_slope.append(left_slope)
-        if right_slope:
-            curr_slope.append(right_slope)
-        if not curr_slope:
-            curr_slope = None
-
-        # The polynomial fit itself.
-        curr_segment, curr_coefs = polynomial_fit(
-            curr_x, curr_y, curr_order, fixed_points=curr_fixed,
-            fixed_slopes=curr_slope)
-
-        # Fit results of the segments are collected in two lists.
-        fit_segments.append(
-            curr_segment if len(fit_segments) == len(x_segments)-1
-            else curr_segment[:-1])
-        coefs.append(curr_coefs)
-
-    # The fit curves of the segments are stitched together.
-    y_fit = np.concatenate(fit_segments)
-
-    return (y_fit, coefs)
-
-
-def polynomial_fit(x_values, y_values, poly_order, fixed_points=None,
-                   fixed_slopes=None):
-    """
-    Fit a dataset with a polynomial function including constraints.
-
-    The fit uses Lagrange multiplicators to introduce equality
-    constraints after formulating the polynomial fit as a
-    multilinear fit problem. The least squares of the residuals
-    is minimized upon the fit. The fit polynomial is described by
-    the following expression:
-
-        y_f = a0 + a1*x + a2*x^2 + a3*x^3 + ... + an*x^n
-            = [1   x   x^2   x^3  ...  x^n]*[ a0 ]
-                                            [ a1 ]
-                                            [ a2 ]
-                                            [ a3 ]
-                                            [....]
-                                            [ an ]
-
-    The minimization problem of the unconstrained fit is:
-        d(X*a-y)^2 = 0
-    with X as a matrix containing as many rows as data points to be
-    fitted, given by the vector y:
-        X = [1   x   x^2   x^3  ...  x^n]
-            [1   x   x^2   x^3  ...  x^n]
-            [... ... ...   ...       ...]
-            [1   x   x^2   x^3  ...  x^n]
-    The set of linear equations to be solved for a is then given by:
-        X(T)*X*a = X(T)*y
-    with (T) meaning the transposed matrix.
-
-    Constraints are introduced by:
-        y_c = C*a
-    with y_c as a vector of y values and C as the matrix to
-    calculate y_c with a. The Lagrangian with Lagrange
-    multiplicators lambda is constructed and its minimum is found
-    by:
-        [2*X(T)*X   C(T)] * [  a   ] = [2*X(T)*y]
-        [  C          0 ]   [lambda]   [   b    ]
-
-    The maximum number of constraints that can be introduced is
-    given by poly_order+1.
-
-    There is currently a small problem that occurred during testing with a
-    random input for x_values. The result was not numerically stable, slightly
-    different fit curves were obtained with different random points.
-
-    Parameters
-    ----------
-    x_values : ndarray
-        The x values (independent variable) used for the fit. Must
-        be a 1D array.
-    y_values : ndarray
-        The y values (dependent variable) used for the fit. Must be
-        a 1D array with the same length as x_values.
-    poly_order : int
-        The polynomial order used for the fit.
-    fixed_points : list of tuples or None, optional
-        Contains constraints for points that the fit functions must
-        pass through. Each point is given by a tuple of two numbers,
-        the x and the y corrdinate of the point. If no point
-        constraints are to be applied, this must be None. The
-        default is None.
-    fixed_slopes : list of tuples or None, optional
-        Contains constraints for slopes that the fit functions must
-        have at specific x values. Each slope is given by a tuple of
-        two numbers, the x value and the slope. If no slope
-        constraints are to be applied, this must be None. The
-        default is None.
-
-    Returns
-    -------
-    y_fit : ndarray
-        A 1D array containing the y values at the x values in
-        x_values.
-    coefs : ndarray
-        The vector a from the linear equations given above. Can be
-        passed directly to np.polynomial.polynomial.polyval to
-        calculate the polynomial values.
-
-    """
-    # Sort x and y values given in tuples from fixed_points into
-    # individual arrays. The numbers are converted to float64 explicitly to
-    # avoid problems with higher order polynomials where the numbers quickly
-    # are too big e.g. for int32 which is automatically used for integer
-    # constraints.
-    if fixed_points is not None:
-        x_points = np.array(
-            [curr_point[0] for curr_point in fixed_points]).astype('float64')
-        y_points = np.array(
-            [curr_point[1] for curr_point in fixed_points]).astype('float64')
-    else:
-        x_points = np.array([])
-        y_points = np.array([])
-
-    # Sort x and slope values given in tuples from fixed_slopes into
-    # individual arrays
-    if fixed_slopes is not None:
-        x_slopes = np.array(
-            [curr_slope[0] for curr_slope in fixed_slopes])
-        slopes = np.array(
-            [curr_slope[1] for curr_slope in fixed_slopes])
-    else:
-        x_slopes = np.array([])
-        slopes = np.array([])
-
-    # The number of constraints and the unknown coefficients in the
-    # polynomial fit function
-    # constraint_number = len(x_slopes) + len(x_points)
-    coef_number = poly_order + 1
-
-    # A matrix with len(x_values) rows and poly_order columns
-    # containing the x_values to the power of all exponents included
-    # by poly_order
-    x_matrix = x_values[:, np.newaxis]**np.arange(coef_number)
-
-    # The upper left part of the matrix in the equation system to be
-    # solved later on
-    ul_matrix = 2*np.dot(x_matrix.T, x_matrix)
-
-    # A matrix containing the factors in front of the polynomial
-    # coefficients for the constraints...
-    # ...in case of point constraints the fixed x values to the
-    # power of all exponents included in poly_order
-    constraints_matrix = x_points[:, np.newaxis]**np.arange(coef_number)
-    # ...in case of slope constraints the x_slopes multiplied with
-    # the exponents and with the x_values to power of the
-    # exponents-1.
-    constraints_matrix = np.append(
-        constraints_matrix,
-        np.arange(coef_number) * x_slopes[:, np.newaxis] **
-        np.insert(np.arange(coef_number-1), 0, 0),
-        axis=0)
-
-    # The combined matrix used for calculation of the least squares
-    # solution
-    combined_matrix = np.zeros(
-        (len(ul_matrix)+len(constraints_matrix),
-         len(ul_matrix)+len(constraints_matrix)))
-    combined_matrix[:coef_number, :coef_number] = ul_matrix
-    combined_matrix[:coef_number:, coef_number:] = constraints_matrix.T
-    combined_matrix[coef_number:, :coef_number] = constraints_matrix
-
-    # The upper part of the vector used for calculating the least
-    # squares solution.
-    upper_vector = 2 * np.dot(x_matrix.T, y_values)
-
-    # The combined vector used for calulating the least squares
-    # solution.
-    combined_vector = np.concatenate(
-        [upper_vector, y_points, slopes])
-
-    # Solution of the set of linear equations leading to the
-    # polynomial coefficients with minimized least squares of the
-    # residuals, possibly with constraints.
-    coefs = np.linalg.solve(
-        combined_matrix, combined_vector)[:coef_number]
-    y_fit = np.polynomial.polynomial.polyval(x_values, coefs)
-
-    return (y_fit, coefs)
+# -*- coding: utf-8 -*-
+
+import warnings
+import numpy as np
+from scipy.optimize import differential_evolution
+
+from little_helpers.array_tools import segment_xy_values
+
+
+def segment_regression(x_values, y_values, poly_orders, border_bounds,
+                       y_bounds=None, slope_bounds=None, max_iter=1000):
+    """
+    Do a regression with a piecewise polynomial fit on the segmentation points.
+
+    This method is useful if the segmentation points for a piecewise polynomial
+    fit are not exactly known, but can be guessed to some extent. Generally, it
+    is possible to give the whole data range as boundaries, so effectively no
+    boundary conditions are passed to the fit, however this is not recommended
+    and may result in an error message. It is better to provide separated
+    boundaries for the segmentation points.
+
+    Parameters
+    ----------
+    x_values : ndarray
+        A 1D array with the length M holding the independent varibale used for
+        the fit.
+    y_values : ndarray
+        A 1D array with the length M holding the dependent varibale used for
+        the fit.
+    poly_orders : list of int
+        A list containing the polynomial orders used for the fit. Must contain
+        one more element than border_bounds.
+    border_bounds : list of tuples
+        The range the fit varies the x values of the segmentation points. Each
+        tuple has two entries and defines the range for one segmentation point,
+        so the list has as many tuples as segmentation points are present. The
+        first value in the tuple is the lower boundary, the second the upper
+        boundary for the respective segmentation point.
+    y_bounds : None, or list of tuples or None, optional
+        The range the fit varies the y values of the segmentation points. Each
+        tuple has two entries and defines the range for one segmentation point,
+        so the list has as many tuples or None as segmentation points are
+        present. The first value in the tuple is the lower boundary, the second
+        the upper boundary for the respective segmentation point. Default is
+        None which means no point constraint at the segmentation point.
+    slope_bounds : None, or list of tuples or None, optional
+        The range the fit varies the slope values at the segmentation points.
+        Each tuple has two entries and defines the range for one segmentation
+        point, so the list has as many tuples or None as segmentation points
+        are present. The first value in the tuple is the lower boundary, the
+        second the upper boundary for the respective segmentation point.
+        Default is None which means no point constraint at the segmentation
+        point.
+    max_iter : int, optional
+        The maximum numer of iterations performed in the iterative fit
+        algorithm (currently differential evolution). The default is 1000.
+
+    Returns
+    -------
+    y_fit : ndarray
+        A 1D array containing the y values of the fit at the x values given in
+        x_values.
+    coefs : list of ndarray
+        A list containing the coefficient vectors of the polynomial equations
+        for the data segments. Each list entry can be passed directly to
+        np.polynomial.polynomial.polyval to calculate the polynomial values.
+    evo_fit : scipy.optimize.OptimizeResult
+        The result of the differential evolution fit.
+
+    """
+    # border_bounds, y_bounds and slope_bounds are mixed together in boundaries
+    # because the parameters for differential_evolution have to be one 1D
+    # array. constraint_types passes a key to sum_of_squared_residuals to
+    # identify which parameter is which kind of constraint.
+    boundaries = []
+    constraint_types = []
+    for idx, curr_border_bounds in enumerate(border_bounds):
+        boundaries.append(curr_border_bounds)
+        constraint_types.append('b')
+        if (y_bounds is not None) and (y_bounds[idx] is not None):
+            boundaries.append(y_bounds[idx])
+            constraint_types.append('y')
+        if (slope_bounds is not None) and (slope_bounds[idx] is not None):
+            boundaries.append(slope_bounds[idx])
+            constraint_types.append('s')
+
+    # The evolutionary fit itself.
+    evo_fit = differential_evolution(
+        sum_of_squared_residuals, bounds=boundaries,
+        args=(x_values, y_values, poly_orders, constraint_types),
+        maxiter=max_iter)
+
+    # segment_borders and y_at_borders are extracted from the 1D evo_fit
+    # array so that they can be used in the calculation of the fit curve.
+    segment_borders, y_at_borders, slope_at_borders = decode_fit_par(
+        evo_fit.x, constraint_types)
+
+    y_fit, coefs = piecewise_polynomial_fit(
+        x_values, y_values, segment_borders, poly_orders,
+        y_at_borders=y_at_borders, slope_at_borders=slope_at_borders)
+
+    return (y_fit, coefs, evo_fit)
+
+
+def sum_of_squared_residuals(fit_par, x_values, y_values, poly_orders,
+                             constraint_types):
+    """
+    Objective function to be minimized during segment_regression.
+
+    The function is called by differential_evolution.
+
+    Parameters
+    ----------
+    fit_par : ndarray
+        A 1D array containing the fit parameters. Contains segment_borders,
+        and possibly y_at_borders and slope at borders directly following the
+        corresponding segment border.
+    x_values : ndarray
+        A 1D array with the length M holding the independent varibale used for
+        the fit.
+    y_values : ndarray
+        A 1D array with the length M holding the dependent varibale used for
+        the fit.
+    poly_orders : list of int
+        A list containing the polynomial orders used for the fit. Must contain
+        one more element than segment_borers contained in fit_par.
+    constraint_types : list of str
+        Encodes which value in fit_par is which kind of constraint. 'b' means
+        segmentation border, 'y' means a common y value of adjacent segments,
+        and 's' means a common slope of adjacent segments.
+
+    Returns
+    -------
+    sum of squared residuals
+        The value to be minimized during the fit.
+
+    """
+    segment_borders, y_at_borders, slope_at_borders = decode_fit_par(
+        fit_par, constraint_types)
+
+    curr_values, curr_coefs = piecewise_polynomial_fit(
+        x_values, y_values, segment_borders, poly_orders,
+        y_at_borders=y_at_borders, slope_at_borders=slope_at_borders)
+
+    return np.sum((curr_values - y_values)**2)
+
+
+def decode_fit_par(fit_par, constraint_types):
+    """
+    Translate the 1D array of fit parameters to individual lists.
+
+    The fit paramters are sorted into the lists segment_borders, y_at_borders
+    slope_at_borders based on the strings given in constraint_types. The three
+    lists are used as arguments in piecewise_polynomial_fit called in the
+    functions sum_of_squared_residuals and segment_regression.
+
+    Parameters
+    ----------
+    fit_par : ndarray
+        A 1D array containing the fit parameters. Contains segment_borders,
+        and possibly y_at_borders and slope at borders directly following the
+        corresponding segment border.
+    constraint_types : list of str
+        Encodes which value in fit_par is which kind of constraint. 'b' means
+        segmentation border, 'y' means a common y value of adjacent segments,
+        and 's' means a common slope of adjacent segments.
+
+    Returns
+    -------
+    segment_borders, y_at_borders, slope_at_borders
+        The arguments used for piecewise_polynomial_fit, see its docstring for
+        details.
+
+    """
+    # Fit parameters from segment_regression and sum_of_squared_residuals are
+    # reordered to be understood by piecewise_polynomial_fit.
+    segment_borders = []
+    y_at_borders = []
+    slope_at_borders = []
+    for idx, curr_type in enumerate(constraint_types):
+        if curr_type == 'b':
+            segment_borders.append(fit_par[idx])
+            y_at_borders.append(None)
+            slope_at_borders.append(None)
+        if curr_type == 'y':
+            y_at_borders[-1] = fit_par[idx]
+        if curr_type == 's':
+            slope_at_borders[-1] = fit_par[idx]
+
+    return (segment_borders, y_at_borders, slope_at_borders)
+
+
+def piecewise_polynomial_fit(x_values, y_values, segment_borders,
+                             poly_orders, y_at_borders=None,
+                             slope_at_borders=None):
+    """
+    Piecewise polynomial fit using polynomial_fit for the data segments.
+
+    Since polynomial_fit allows constraints such as fixed points or fixed
+    slopes, this can be used for the piecewise polynomial fit as well. By
+    default, the data is divided into segments at the values given in
+    segment_borders and the segments are fitted each by a polynomial fit using
+    the least squares method. Thus, discontinuities will arise at the segment
+    borders between the fits of the segments. These discontinuities can be
+    suppressed by applying equality constraints to the fits that force the fit
+    curves through specific points or to have specific slopes. The method
+    allows to use polynomials of different orders for the different segments.
+
+    Parameters
+    ----------
+    x_values : ndarray
+        A 1D array with the length M holding the independent varibale used for
+        the fit.
+    y_values : ndarray
+        A 1D array with the length M holding the dependent varibale used for
+        the fit.
+    segment_borders : list of int or float
+        The values with respect to x_values at which the data is divided into
+        segments. An arbitrary number of segment borders may be given, but it
+        is recommended to provide a sorted list in order to avoid confusion.
+        If the list is not sorted, it will be sorted and the sorting is also
+        applied to y_at_borders and slope_at_borders (if they are given), but
+        not to poly_orders.
+    poly_orders : list of int
+        A list containing the polynomial orders used for the fit. Must contain
+        one more element than segment_borders.
+    y_at_borders : None, or list of float or None, optional
+        May contain dependent variable values used as equality constraints at
+        the segment borders. The fits of both touching segments are forced
+        through the point given by the pair (segment border, y_at_border). The
+        list entries may also be None to state that at a certain segment
+        border, no constraint is to be applied. The default is None which means
+        that no contraints are applied for any segment border.
+    slope_at_borders : None, or list of float or None, optional
+        Analogous to y_at_borders, with the difference that here, fixed slopes
+        at the segment borders are given. The default is None.
+
+    Returns
+    -------
+    y_fit : ndarray
+        A 1D array containing the y values of the fit at the x values given in
+        x_values.
+    coefs : list of ndarray
+        A list containing the coefficient vectors of the polynomial equations
+        for the data segments. Each list entry can be passed directly to
+        np.polynomial.polynomial.polyval to calculate the polynomial values.
+
+    """
+
+    sort_order = np.argsort(segment_borders)
+    segment_borders = np.array(segment_borders)[sort_order]
+
+    # Fixed points are given by the x values in segment_borders and the y
+    # values given in y_at_borders and are collected in tuples of the two
+    # numbers or in empty tuples if no fixed point is used for the given
+    # segment border.
+    if y_at_borders is not None:
+        y_at_borders = np.array(y_at_borders)[sort_order]
+        fixed_points = [()]  # for left edge
+        for x, y in zip(segment_borders, y_at_borders):
+            curr_point = (x, y) if y is not None else ()
+            fixed_points.append(curr_point)
+        fixed_points.append(())  # for right edge
+    else:
+        fixed_points = [()] * (len(segment_borders) + 2)
+
+    # Fixed slopes are given by the x values in segment_borders and the slope
+    # values given in slope_at_borders and are collected in tuples of the two
+    # numbers or in empty tuples if no fixed slope is used for the given
+    # segment border.
+    if slope_at_borders is not None:
+        fixed_slopes = [()]  # for left edge
+        for x, slope in zip(segment_borders, slope_at_borders):
+            curr_slope = (x, slope) if slope is not None else ()
+            fixed_slopes.append(curr_slope)
+        fixed_slopes.append(())  # for right edge
+    else:
+        fixed_slopes = [()] * (len(segment_borders) + 2)
+
+    x_segments, y_segments = segment_xy_values(x_values, segment_borders,
+                                               y_values=y_values)
+
+    fit_segments = []
+    coefs = []
+    # In the loop, the segments are fitted individually, one in each iteration.
+    for curr_x, curr_y, curr_order, left_fix, right_fix, left_slope, right_slope in zip(
+            x_segments, y_segments, poly_orders, fixed_points[:-1],
+            fixed_points[1:], fixed_slopes[:-1], fixed_slopes[1:]):
+        # The fixed points and slopes are translated into the syntax understood
+        # by polynomial_fit.
+        curr_fixed = []
+        if left_fix:
+            curr_fixed.append(left_fix)
+        if right_fix:
+            curr_fixed.append(right_fix)
+        if not curr_fixed:
+            curr_fixed = None
+        curr_slope = []
+        if left_slope:
+            curr_slope.append(left_slope)
+        if right_slope:
+            curr_slope.append(right_slope)
+        if not curr_slope:
+            curr_slope = None
+
+        # The polynomial fit itself.
+        curr_segment, curr_coefs = polynomial_fit(
+            curr_x, curr_y, curr_order, fixed_points=curr_fixed,
+            fixed_slopes=curr_slope)
+
+        # Fit results of the segments are collected in two lists.
+        fit_segments.append(
+            curr_segment if len(fit_segments) == len(x_segments)-1
+            else curr_segment[:-1])
+        coefs.append(curr_coefs)
+
+    # The fit curves of the segments are stitched together.
+    y_fit = np.concatenate(fit_segments)
+
+    return (y_fit, coefs)
+
+
+def polynomial_fit(x_values, y_values, poly_order, fixed_points=None,
+                   fixed_slopes=None, fixed_curvs=None):
+    """
+    Fit a dataset with a polynomial function including constraints.
+
+    The fit uses Lagrange multiplicators to introduce equality
+    constraints after formulating the polynomial fit as a
+    multilinear fit problem. The least squares of the residuals
+    is minimized upon the fit. The fit polynomial is described by
+    the following expression:
+
+        y_f = a0 + a1*x + a2*x^2 + a3*x^3 + ... + an*x^n
+            = [1   x   x^2   x^3  ...  x^n]*[ a0 ]
+                                            [ a1 ]
+                                            [ a2 ]
+                                            [ a3 ]
+                                            [....]
+                                            [ an ]
+
+    The minimization problem of the unconstrained fit is:
+        d(X*a-y)^2 = 0
+    with X as a matrix containing as many rows as data points to be
+    fitted, given by the vector y:
+        X = [1   x   x^2   x^3  ...  x^n]
+            [1   x   x^2   x^3  ...  x^n]
+            [... ... ...   ...       ...]
+            [1   x   x^2   x^3  ...  x^n]
+    The set of linear equations to be solved for a is then given by:
+        X(T)*X*a = X(T)*y
+    with (T) meaning the transposed matrix.
+
+    Constraints are introduced by:
+        y_c = C*a
+    with y_c as a vector of y values and C as the matrix to
+    calculate y_c with a. The Lagrangian with Lagrange
+    multiplicators lambda is constructed and its minimum is found
+    by:
+        [2*X(T)*X   C(T)] * [  a   ] = [2*X(T)*y]
+        [  C          0 ]   [lambda]   [   b    ]
+
+    The maximum number of constraints that can be introduced is
+    given by poly_order+1.
+
+    There is currently a small problem that occurred during testing with a
+    random input for x_values. Slightly different fit curves were obtained
+    with different random points. This might be caused by the different
+    least squares problems, but maybe also due to numerically instable
+    behavior. Should be checked in the future.
+
+    Parameters
+    ----------
+    x_values : ndarray
+        The x values (independent variable) used for the fit. Must
+        be a 1D array.
+    y_values : ndarray
+        The y values (dependent variable) used for the fit. Must be
+        a 1D array with the same length as x_values.
+    poly_order : int
+        The polynomial order used for the fit.
+    fixed_points : list of tuples or None, optional
+        Contains constraints for points that the fit functions must
+        pass through. Each point is given by a tuple of two numbers,
+        the x and the y corrdinate of the point. If no point
+        constraints are to be applied, this must be None. The
+        default is None.
+    fixed_slopes : list of tuples or None, optional
+        Contains constraints for slopes that the fit functions must
+        have at specific x values. Each slope is given by a tuple of
+        two numbers, the x value and the slope. If no slope
+        constraints are to be applied, this must be None. The
+        default is None.
+    fixed_curvs : list of tuples or None, optional
+        Contains constraints for curvatures that the fit functions must
+        have at specific x values. Each curvature is given by a tuple of
+        two numbers, the x value and the curvature. If no curvature
+        constraints are to be applied, this must be None. The
+        default is None.
+
+    Returns
+    -------
+    y_fit : ndarray
+        A 1D array containing the y values at the x values in
+        x_values.
+    coefs : ndarray
+        The vector a from the linear equations given above. Can be
+        passed directly to np.polynomial.polynomial.polyval to
+        calculate the polynomial values.
+
+    """
+    # Sort x and y values given in tuples from fixed_points, fixed_slopes and
+    # fixed_curvs into individual arrays. The numbers are converted to float64
+    # explicitly to avoid problems with higher order polynomials where the
+    # numbers quickly are too big e.g. for int32 which is automatically used
+    # for integer constraints.
+    const_x = []
+    const_y = []
+    constraint_number = 0
+    # The number of the unknown coefficients in the polynomial fit function
+    coef_number = poly_order + 1
+    for ii, curr_const in enumerate([fixed_points, fixed_slopes, fixed_curvs]):
+        if curr_const is not None:
+            const_x.append([curr_point[0] for curr_point in curr_const])
+            const_y.append([curr_point[1] for curr_point in curr_const])
+            constraint_number += len(const_x[-1])
+
+            # Make sure that no x value has two conflicting constraints of the
+            # same kind.
+            if len(const_x[-1]) != len(set(const_x[-1])):
+                raise Exception('More than one constraint of the same kind '
+                                'for one of the x values given.')
+
+            # Make sure that the number of constraints does not exceed the
+            # degrees of freedom of the respective polynomials.
+            if coef_number-ii < len(const_x[-1]):
+                if poly_order-ii < 0:
+                    error_end = 'zero, so no constraint can be applied.'
+                elif poly_order-ii == 0:
+                    error_end = ('a constant, so the maximum number of '
+                                 'constraints is 1.')
+                else:
+                    error_end = ('a polynomial with a degree of {}, so the '
+                                 'maximum number of constraints is {}.'.format(
+                                     poly_order-ii, poly_order-ii+1))
+                raise Exception(
+                    'Too many constraints ({0}) are applied on derivative of '
+                    'order {1}. With a poly_order of {2}, the derivative of '
+                    'order {1} is {3}'.format(
+                        len(const_x[-1]), ii, poly_order, error_end))
+        else:
+            const_x.append([])
+            const_y.append([])
+
+    # Make sure that the total number of constraints does not exceed the
+    # degrees of freedom of polynomial with order of poly_order.
+    if constraint_number > coef_number:
+        raise ValueError('Number of constraints ({}) must be smaller than '
+                         'poly_order + 1 ({}).'.format(
+                             constraint_number, poly_order+1))
+    elif constraint_number == coef_number:
+        warnings.warn('Constraint number equals the number of degrees of '
+                      'freedom for the regression, so the polynomial is fully '
+                      'defined already only by the constraints.')
+
+    # A matrix with len(x_values) rows and poly_order columns
+    # containing the x_values to the power of all exponents included
+    # by poly_order
+    x_matrix = np.polynomial.polynomial.polyvander(x_values, poly_order)
+
+    # A matrix containing the factors in front of the polynomial
+    # coefficients for the constraints...
+    # ...in case of point constraints the fixed x values to the power of the
+    # exponents.
+    # ...in case of slope constraints the x_slopes multiplied with
+    # the exponents and with the x_values to power of the
+    # exponents-1.
+    # ...in case of curvature constraints the x_curvs multiplied with
+    # the exponents-1 and with the x_values to power of the
+    # exponents-2.
+    constraints_matrix = np.zeros((constraint_number, coef_number))
+    start_idx = 0
+    for ii, curr_const in enumerate(const_x):
+        if curr_const:
+            ff = 1 if ii==0 else np.arange(ii, coef_number)
+            constraints_matrix[start_idx:start_idx+len(curr_const)] = (
+                np.insert(ff * np.polynomial.polynomial.polyvander(
+                    curr_const, poly_order-ii), [0]*ii, 0, axis=1))
+            start_idx += len(curr_const)
+
+    # The combined matrix used for calculation of the least squares solution
+    combined_matrix = np.zeros(
+        (coef_number + constraint_number,)*2)
+    combined_matrix[:coef_number:, coef_number:] = constraints_matrix.T
+    combined_matrix[coef_number:, :coef_number] = constraints_matrix
+    # The upper left part of the matrix in the equation system to be
+    # solved later on
+    combined_matrix[:coef_number, :coef_number] = 2*np.dot(
+        x_matrix.T, x_matrix)
+
+    # The combined vector used for calulating the least squares solution.
+    combined_vector = np.zeros(coef_number + constraint_number)
+    # The upper part of the vector used for calculating the least squares
+    # solution.
+    combined_vector[:coef_number] = 2 * np.dot(x_matrix.T, y_values)
+    # The combined vector used for calulating the least squares solution.
+    combined_vector[coef_number:] = np.concatenate(const_y)
+
+    # Solution of the set of linear equations leading to the
+    # polynomial coefficients with minimized least squares of the
+    # residuals, possibly with constraints.
+    coefs = np.linalg.solve(
+        combined_matrix, combined_vector)[:coef_number]
+    y_fit = np.polynomial.polynomial.polyval(x_values, coefs)
+
+    return (y_fit, coefs)
```

### Comparing `pyDataFitting-0.0.2/src/pyDataFitting.egg-info/PKG-INFO` & `pyDataFitting-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-Metadata-Version: 2.1
-Name: pyDataFitting
-Version: 0.0.2
-Summary: package for specialized regression
-Home-page: https://github.com/AlexanderSouthan/pyDataFitting
-Author: Alexander Southan
-Author-email: alexander.southan@web.de
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyDataFitting/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![build workflow](https://github.com/AlexanderSouthan/pyDataFitting/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/pyDataFitting/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/AlexanderSouthan/pyDataFitting/branch/master/graph/badge.svg?token=NYWF752QP0)](https://codecov.io/gh/AlexanderSouthan/pyDataFitting)
-
-# pyDataFitting
-Linear and nonlinear fit functions that can be used *e.g.* for curve fitting.
-Is not meant to duplicate methods already implemented *e.g.* in NumPy or SciPy,
-but to provide additional, specialized regression methods or higher computation
-speed. You will need certain functions of my little_helpers repository and
-quite a few other, external packages like Numpy, Pandas, matplotlib,
-scikit-learn, statsmodels, Scipy.
-
-Install with:
-```
-pip install pyDataFitting
-```
-
-## Linear regression (in linear_regression.py)
-* dataset_regression: Does a classical linear least squares regression. Treats
-the input data as a linear combination of the different components from
-reference data. Can be used for example to fit spectra of mixtures with spectra
-of pure components. Produces the same result like, but much faster than using
-sklearn.linear_model.LinearRegression().fit(...).
-* lin_reg_all_sections: Does linear regressions on a dataset starting with the
-first two datapoints and expands the segment by one for each iteration. The
-regression metrics are useful to determine if a dataset behaves linearly at its
-beginning or not, and when a transition to nonlinear behavior occurs.
-
-## Polynomial regression (in polynomial_regression.py)
-* polynomial_fit: Allows to perform polynomial fits by minimizing the sum of
-the squared residuals while also taking equality constaints into account via
-Lagrange multiplicators. This can be used to force the regression function
-through certain points or to force it to have certain slopes at a given points.
-Also does unconstrained polynomial fits, but is slower than the corresponding
-Numpy functions.
-* piecewise_polynomial_fit: Allows to do a picewise polynomial fit on a dataset,
-*i.e.* the data is divided into segments that are then each fitted with an own
-polynomial function. The segments can be fitted with polynomials of different
-orders. It is possible to use equality constraints on the segment borders, so
-that the segments *e.g.* are forced to have the same y values at the borders or
-the same slopes.
-* segment_regression: Does a piecewise polynomial fit with the segment borders,
-y values at the segment borders, or the slopes at the segment borders as
-additional fit parameters. The additional fit parameters are estimated with an
-evolutionary fitting algorithm which calls picewise_polynomial_fit several
-times in each iteration, so the whole procedure is rather slow (albeit still
-very usable).
-
-## General nonlinear regression (in nonlinear_regression.py)
-* nonlinear_regression: Does nonlinear regressions by minimizing the sum of the
-squared residuals. Basically utilizes differential_evolution from
-scipy.optimize to estimatze the parameters of complex regression functions. The
-functions must be included in calc_functions, but can be added easily there. 
-This is not a particularly fast method, so use methods from other packages for
-simple problems.
-* nonlinear_regression_3D: Does the same like nonlinear_regression, but on 3D
-datasets. Also here, the regression function must be included in
-calc_function_3D.
-
-## Principal component regression and partial least squares regression (in multivariate_regression.py)
-* principal_component_regression: A class for a principal component regression
-(PCR). Does a principal component analysis of the dataset and a multilinear
-regression on the resulting scores with one or several responses in order to
-generate a model to predict the responses from future data. The PCR parts work
-quite well, the methods included for generating various plots still need
-improving.
-* pls_regression: A class to help with using the partial least squares
-regression class from scikit-learn. It is usable, but could do with some
-redesigning.
-
-
+Metadata-Version: 2.1
+Name: pyDataFitting
+Version: 0.0.3
+Summary: package for specialized regression
+Home-page: https://github.com/AlexanderSouthan/pyDataFitting
+Author: Alexander Southan
+Author-email: 72788772+AlexanderSouthan@users.noreply.github.com
+Project-URL: Bug Tracker, https://github.com/AlexanderSouthan/pyDataFitting/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![build workflow](https://github.com/AlexanderSouthan/pyDataFitting/actions/workflows/main.yml/badge.svg)](https://github.com/AlexanderSouthan/pyDataFitting/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/AlexanderSouthan/pyDataFitting/branch/master/graph/badge.svg?token=NYWF752QP0)](https://codecov.io/gh/AlexanderSouthan/pyDataFitting)
+
+# pyDataFitting
+Linear and nonlinear fit functions that can be used *e.g.* for curve fitting.
+Is not meant to duplicate methods already implemented *e.g.* in NumPy or SciPy,
+but to provide additional, specialized regression methods, higher computation
+speed, or help with methods from well-known packages. You will need certain
+functions of my little_helpers repository and quite a few other, external
+packages like Numpy, Pandas, matplotlib, scikit-learn, statsmodels, Scipy.
+
+Install with:
+```
+pip install pyDataFitting
+```
+
+## Linear regression (in linear_regression.py)
+* dataset_regression: Does a classical linear least squares regression. Treats
+the input data as a linear combination of the different components from
+reference data. Can be used for example to fit spectra of mixtures with spectra
+of pure components. Produces the same result like, but much faster than using
+sklearn.linear_model.LinearRegression().fit(...).
+* lin_reg_all_sections: Does linear regressions on a dataset starting with the
+first two datapoints and expands the segment by one for each iteration. The
+regression metrics are useful to determine if a dataset behaves linearly at its
+beginning or not, and when a transition to nonlinear behavior occurs.
+
+## Polynomial regression (in polynomial_regression.py)
+* polynomial_fit: Allows to perform polynomial fits by minimizing the sum of
+the squared residuals while also taking equality constaints into account via
+Lagrange multiplicators. This can be used to force the regression function
+through certain points or to force it to have certain slopes at a given points.
+Also does unconstrained polynomial fits, but is slower than the corresponding
+Numpy functions.
+* piecewise_polynomial_fit: Allows to do a picewise polynomial fit on a dataset,
+*i.e.* the data is divided into segments that are then each fitted with an own
+polynomial function. The segments can be fitted with polynomials of different
+orders. It is possible to use equality constraints on the segment borders, so
+that the segments *e.g.* are forced to have the same y values at the borders or
+the same slopes.
+* segment_regression: Does a piecewise polynomial fit with the segment borders,
+y values at the segment borders, or the slopes at the segment borders as
+additional fit parameters. The additional fit parameters are estimated with an
+evolutionary fitting algorithm which calls picewise_polynomial_fit several
+times in each iteration, so the whole procedure is rather slow (albeit still
+very usable).
+
+## General nonlinear regression (in nonlinear_regression.py)
+* nonlinear_regression: Does nonlinear regressions by minimizing the sum of the
+squared residuals. Basically utilizes the minimize method from lmfit to
+estimatze the parameters of complex regression functions. The functions
+calculating the function values must be written externally, but this is pretty
+straight forward. 
+
+## Principal component regression and partial least squares regression (in multivariate_regression.py)
+* principal_component_regression: A class for a principal component regression
+(PCR). Does a principal component analysis of the dataset and a multilinear
+regression on the resulting scores with one or several responses in order to
+generate a model to predict the responses from future data. The PCR parts work
+quite well, the methods included for generating various plots still need
+improving.
+* pls_regression: A class to help with using the partial least squares
+regression class from scikit-learn. It is usable, but could do with some
+redesigning.
+
+## Tools for supporting the use of ols from statsmodels.formula.api (in model_tools.py)
+* Provides simple methods to generate the model string for different simple
+models (linear, two-factor interaction, quadratic, etc.). 
+* Provides a method to easily adapt the included parameters in the model string
+and a method to ensure model hierarchy.
+* Allows the calculation of model values if the model coefficients are
+provided.
```

