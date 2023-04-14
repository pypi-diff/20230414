# Comparing `tmp/kinisi-0.6.2.tar.gz` & `tmp/kinisi-0.6.3.tar.gz`

## Comparing `kinisi-0.6.2.tar` & `kinisi-0.6.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/analyze.py
--rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/analyzer.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/arrhenius.py
--rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/conductivity_analyzer.py
--rw-r--r--   0        0        0    30920 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/diffusion.py
--rw-r--r--   0        0        0    11010 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/diffusion_analyzer.py
--rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/jump_diffusion_analyzer.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/matrix.py
--rw-r--r--   0        0        0    23411 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/tests/__init__.py
--rw-r--r--   0        0        0    15452 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/tests/test_analyze.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/tests/test_arrhenius.py
--rw-r--r--   0        0        0    38487 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/tests/test_diffusion.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/tests/test_matrix.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/tests/test_parser.py
--rw-r--r--   0        0        0    46919 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/tests/inputs/example_LAMMPS.data
--rw-r--r--   0        0        0   630756 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/tests/inputs/example_LAMMPS.dcd
--rw-r--r--   0        0        0   842426 2020-02-02 00:00:00.000000 kinisi-0.6.2/kinisi/tests/inputs/example_XDATCAR.gz
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kinisi-0.6.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 kinisi-0.6.2/LICENSE
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 kinisi-0.6.2/README.md
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 kinisi-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 kinisi-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/analyze.py
+-rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/analyzer.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/arrhenius.py
+-rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/conductivity_analyzer.py
+-rw-r--r--   0        0        0    34673 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/diffusion.py
+-rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/diffusion_analyzer.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/jump_diffusion_analyzer.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/matrix.py
+-rw-r--r--   0        0        0    23518 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/__init__.py
+-rw-r--r--   0        0        0    14904 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/test_analyze.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/test_arrhenius.py
+-rw-r--r--   0        0        0    38583 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/test_diffusion.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/test_matrix.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/test_parser.py
+-rw-r--r--   0        0        0    46919 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/inputs/example_LAMMPS.data
+-rw-r--r--   0        0        0   630756 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/inputs/example_LAMMPS.dcd
+-rw-r--r--   0        0        0   842426 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/inputs/example_XDATCAR.gz
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kinisi-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 kinisi-0.6.3/LICENSE
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 kinisi-0.6.3/README.md
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 kinisi-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 kinisi-0.6.3/PKG-INFO
```

### Comparing `kinisi-0.6.2/kinisi/analyze.py` & `kinisi-0.6.3/kinisi/analyze.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/kinisi/analyzer.py` & `kinisi-0.6.3/kinisi/analyzer.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/kinisi/arrhenius.py` & `kinisi-0.6.3/kinisi/arrhenius.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/kinisi/conductivity_analyzer.py` & `kinisi-0.6.3/kinisi/conductivity_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             average from the data.
         """
         return self._diff.n
 
     @property
     def mscd_std(self) -> np.ndarray:
         """
-        :return: MSCD standard deviations values for the input trajectories.
+        :return: MSCD standard deviation values for the input trajectories (a single standard deviation).
         """
         return self._diff.s
 
     @property
     def sigma(self) -> 'uravu.distribution.Distribution':
         """
         :returns: Conductivity, in mS^{1}cm^{-1}.
```

### Comparing `kinisi-0.6.2/kinisi/diffusion.py` & `kinisi-0.6.3/kinisi/diffusion.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 # Copyright (c) Andrew R. McCluskey and Benjamin J. Morgan
 # Distributed under the terms of the MIT License
 # author: Andrew R. McCluskey (arm61)
 
 import warnings
-from typing import List, Union
+from typing import List, Union, Any
 import numpy as np
 from scipy.stats import normaltest, linregress
 from scipy.linalg import pinvh
 from scipy.optimize import minimize, curve_fit
 import scipy.constants as const
 import tqdm
 from uravu.distribution import Distribution
@@ -61,14 +61,17 @@
         self._delta_t = np.array(delta_t[::sub_sample_dt])
         self._max_obs = self._displacements[0].shape[1]
         self._distributions = []
         self._dt = np.array([])
         self._n = np.array([])
         self._s = np.array([])
         self._v = np.array([])
+        self._n_bootstrap = np.array([])
+        self._s_bootstrap = np.array([])
+        self._v_bootstrap = np.array([])
         self._n_o = n_o
         self._ngp = np.array([])
         self._sub_sample_dt = sub_sample_dt
         self._dimension = dimension
         self._euclidian_displacements = []
         self._diffusion_coefficient = None
         self._jump_diffusion_coefficient = None
@@ -89,25 +92,30 @@
             'delta_t': self._delta_t,
             'n_o': self._n_o,
             'max_obs': self._max_obs,
             'dt': self._dt,
             'n': self._n,
             's': self._s,
             'v': self._v,
+            'n_bootstrap': self._n_bootstrap,
+            's_bootstrap': self._s_bootstrap,
+            'v_bootstrap': self._v_bootstrap,
             'sub_sample_dt': self._sub_sample_dt,
             'dimension': self._dimension,
             'ngp': self._ngp,
             'covariance_matrix': self._covariance_matrix,
+            'distributions': None,
             'diffusion_coefficient': None,
             'jump_diffusion_coefficient': None,
             'sigma': None,
             'intercept': None,
             'gradient': None
         }
-        my_dict['distributions'] = [d.to_dict() for d in self._distributions]
+        if len(self._distributions) != 0:
+            my_dict['distributions'] = [d.to_dict() for d in self._distributions]
         my_dict['euclidian_displacements'] = [d.to_dict() for d in self._euclidian_displacements]
         if self._diffusion_coefficient is not None:
             my_dict['diffusion_coefficient'] = self._diffusion_coefficient.to_dict()
         if self._jump_diffusion_coefficient is not None:
             my_dict['jump_diffusion_coefficient'] = self._jump_diffusion_coefficient.to_dict()
         if self._sigma is not None:
             my_dict['sigma'] = self._sigma.to_dict()
@@ -129,22 +137,26 @@
         """
         boot = cls(my_dict['delta_t'],
                    my_dict['displacements'],
                    my_dict['n_o'],
                    sub_sample_dt=my_dict['sub_sample_dt'],
                    dimension=my_dict['dimension'])
         boot._max_obs = my_dict['max_obs']
-        boot._distributions = [Distribution.from_dict(d) for d in my_dict['distributions']]
         boot._euclidian_displacements = [Distribution.from_dict(d) for d in my_dict['euclidian_displacements']]
         boot._dt = my_dict['dt']
         boot._n = my_dict['n']
         boot._s = my_dict['s']
         boot._v = my_dict['v']
+        boot._n_bootstrap = my_dict['n_bootstrap']
+        boot._s_bootstrap = my_dict['s_bootstrap']
+        boot._v_bootstrap = my_dict['v_bootstrap']
         boot._n_o = my_dict['n_o']
         boot._ngp = my_dict['ngp']
+        if my_dict['distributions'] is not None:
+            boot._distributions = [Distribution.from_dict(d) for d in my_dict['distributions']]
         if my_dict['diffusion_coefficient'] is not None:
             boot._diffusion_coefficient = Distribution.from_dict(my_dict['diffusion_coefficient'])
         if my_dict['jump_diffusion_coefficient'] is not None:
             boot._jump_diffusion_coefficient = Distribution.from_dict(my_dict['jump_diffusion_coefficient'])
         if my_dict['sigma'] is not None:
             boot._sigma = Distribution.from_dict(my_dict['sigma'])
         if my_dict['intercept'] is not None:
@@ -227,20 +239,20 @@
 
         :param progress: Should :py:mod:`tqdm` be used to give a progress bar.
         :param loop: The object that should be looped over.
 
         :return: Iterator object.
         """
         if progress:
-            return tqdm.tqdm(loop, desc='Bootstrapping Displacements')
+            return tqdm.tqdm(loop, desc='Finding Means and Variances')
         return loop
 
     @staticmethod
     def sample_until_normal(array: np.ndarray,
-                            n_samples: int,
+                            n_samples: float,
                             n_resamples: int,
                             max_resamples: int,
                             alpha: float = 1e-3,
                             random_state: np.random.mtrand.RandomState = None) -> Distribution:
         """
         Resample from the distribution until a normal distribution is obtained or a maximum is reached.
 
@@ -252,17 +264,19 @@
         :param alpha: Level that p-value should be below in :py:func:`scipy.stats.normaltest` for the distribution
             to be normal. Optional, default is :py:attr:`1e-3`.
         :param random_state: A :py:attr:`RandomState` object to be used to ensure reproducibility. Optional,
             default is :py:attr:`None`.
 
         :return: The resampled distribution.
         """
+        # values = _bayesian_bootstrap(array, n_samples, n_resamples, random_state)
         values = _bootstrap(array, n_samples, n_resamples, random_state)
         p_value = normaltest(values)[1]
         while p_value < alpha and len(values) < max_resamples:
+            # values += _bayesian_bootstrap(array, n_samples, 100, random_state)
             values += _bootstrap(array, n_samples, 100, random_state)
             p_value = normaltest(values)[1]
         if len(values) >= max_resamples:
             warnings.warn("The maximum number of resamples has been reached, and the distribution is not yet normal.")
         return Distribution(values)
 
     @staticmethod
@@ -458,14 +472,16 @@
     :param delta_t: An array of the timestep values, units of ps
     :param disp_3d: A list of arrays, where each array has the axes
         :code:`[atom, displacement observation, dimension]`. There is one array in the list for each
         delta_t value. Note: it is necessary to use a list of arrays as the number of observations is
         not necessary the same at each data point.
     :param n_o: Number of statistically independent observations of the MSD at each timestep.
     :param sub_sample_dt: The frequency in observations to be sampled. Default is :py:attr:`1` (every observation)
+    :param bootstrap: Should bootstrap resampling be used to estimate the observed MSD distribution.
+        Optional, default is :py:attr:`False`.
     :param n_resamples: The initial number of resamples to be performed. Default is :py:attr:`1000`
     :param max_resamples: The max number of resamples to be performed by the distribution is assumed to be normal.
         This is present to allow user control over the time taken for the resampling to occur. Default
         is :py:attr:`100000`
     :param dimension: Dimension/s to find the displacement along, this should be some subset of `'xyz'` indicating
         the axes of interest. Optional, defaults to `'xyz'`.
     :param alpha: Value that p-value for the normal test must be greater than to accept. Default is :py:attr:`1e-3`
@@ -475,14 +491,15 @@
     """
 
     def __init__(self,
                  delta_t: np.ndarray,
                  disp_3d: List[np.ndarray],
                  n_o: np.ndarray,
                  sub_sample_dt: int = 1,
+                 bootstrap: bool = False,
                  n_resamples: int = 1000,
                  max_resamples: int = 10000,
                  dimension: str = 'xyz',
                  alpha: float = 1e-3,
                  random_state: np.random.mtrand.RandomState = None,
                  progress: bool = True):
         super().__init__(delta_t, disp_3d, n_o, sub_sample_dt, dimension)
@@ -490,19 +507,23 @@
         for i in self._iterator:
             disp_slice = self._displacements[i][:, :, self._slice].reshape(self._displacements[i].shape[0],
                                                                            self._displacements[i].shape[1], self.dims)
             d_squared = np.sum(disp_slice**2, axis=-1)
             if d_squared.size <= 1:
                 continue
             self._euclidian_displacements.append(Distribution(np.sqrt(d_squared.flatten())))
-            distro = self.sample_until_normal(d_squared, int(n_o[i]), n_resamples, max_resamples, alpha, random_state)
-            self._distributions.append(distro)
+            if bootstrap:
+                distro = self.sample_until_normal(d_squared, n_o[i], n_resamples, max_resamples, alpha, random_state)
+                self._distributions.append(distro)
+                self._n_bootstrap = np.append(self._n_bootstrap, np.mean(distro.samples))
+                self._v_bootstrap = np.append(self._v_bootstrap, np.var(distro.samples, ddof=1))
+                self._s_bootstrap = np.append(self._s_bootstrap, np.std(distro.samples, ddof=1))
             self._n = np.append(self._n, d_squared.mean())
-            self._s = np.append(self._s, np.std(distro.samples, ddof=1))
-            self._v = np.append(self._v, np.var(distro.samples, ddof=1))
+            self._v = np.append(self._v, np.var(d_squared, ddof=1) / n_o[i])
+            self._s = np.append(self._s, np.sqrt(self._v[i]))
             self._ngp = np.append(self._ngp, self.ngp_calculation(d_squared))
             self._dt = np.append(self._dt, self._delta_t[i])
         self._n_o = self._n_o[:self._n.size]
 
 
 class TMSDBootstrap(Bootstrap):
     """
@@ -512,15 +533,17 @@
     :param delta_t: An array of the timestep values.
     :param disp_3d: A list of arrays, where each array has the axes
         :code:`[atom, displacement observation, dimension]`. There is one array in the list for each
         delta_t value. Note: it is necessary to use a list of arrays as the number of observations is
         not necessary the same at each data point.
     :param n_o: Number of statistically independent observations of the MSD at each timestep.
     :param sub_sample_dt: The frequency in observations to be sampled. Optional, default
-        is :py:attr:`1` (every observation)
+        is :py:attr:`1` (every observation).
+    :param bootstrap: Should bootstrap resampling be used to estimate the observed MSD distribution.
+        Optional, default is :py:attr:`False`.
     :param n_resamples: The initial number of resamples to be performed. Optional, default
         is :py:attr:`1000`
     :param max_resamples: The max number of resamples to be performed by the distribution is assumed to be
         normal. This is present to allow user control over the time taken for the resampling to occur.
         Optional, default is :py:attr:`100000`
     :param dimension: Dimension/s to find the displacement along, this should be some subset of `'xyz'` indicating
         the axes of interest. Optional, defaults to `'xyz'`.
@@ -532,14 +555,15 @@
     """
 
     def __init__(self,
                  delta_t: np.ndarray,
                  disp_3d: List[np.ndarray],
                  n_o: np.ndarray,
                  sub_sample_dt: int = 1,
+                 bootstrap: bool = False,
                  n_resamples: int = 1000,
                  max_resamples: int = 10000,
                  dimension: str = 'xyz',
                  alpha: float = 1e-3,
                  random_state: np.random.mtrand.RandomState = None,
                  progress: bool = True):
         super().__init__(delta_t, disp_3d, n_o, sub_sample_dt, dimension)
@@ -547,22 +571,24 @@
         for i in self._iterator:
             disp_slice = self._displacements[i][:, :, self._slice].reshape(self._displacements[i].shape[0],
                                                                            self._displacements[i].shape[1], self.dims)
             d_squared = np.sum(disp_slice**2, axis=-1)
             coll_motion = np.sum(np.sum(disp_slice, axis=0)**2, axis=-1)
             if coll_motion.size <= 1:
                 continue
-            self._n_o = np.append(self._n_o, n_o[i])
             self._euclidian_displacements.append(Distribution(np.sqrt(d_squared.flatten())))
-            distro = self.sample_until_normal(coll_motion, int(n_o[i] / d_squared.shape[0]), n_resamples, max_resamples,
-                                              alpha, random_state)
-            self._distributions.append(distro)
-            self._n = np.append(self._n, distro.n)
-            self._s = np.append(self._s, np.std(distro.samples, ddof=1))
-            self._v = np.append(self._v, np.var(distro.samples, ddof=1))
+            if bootstrap:
+                distro = self.sample_until_normal(d_squared, n_o[i], n_resamples, max_resamples, alpha, random_state)
+                self._distributions.append(distro)
+                self._n_bootstrap = np.append(self._n_bootstrap, np.mean(distro.samples))
+                self._v_bootstrap = np.append(self._v_bootstrap, np.var(distro.samples, ddof=1))
+                self._s_bootstrap = np.append(self._s_bootstrap, np.std(distro.samples, ddof=1))
+            self._n = np.append(self._n, d_squared.mean())
+            self._v = np.append(self._v, np.var(d_squared, ddof=1) / n_o[i])
+            self._s = np.append(self._s, np.sqrt(self._v[i]))
             self._ngp = np.append(self._ngp, self.ngp_calculation(d_squared.flatten()))
             self._dt = np.append(self._dt, self._delta_t[i])
         self._n_o = self._n_o[:self._n.size]
 
 
 class MSCDBootstrap(Bootstrap):
     """
@@ -573,14 +599,16 @@
     :param disp_3d: A list of arrays, where each array has the axes
         :code:`[atom, displacement observation, dimension]`. There is one array in the list for each
         delta_t value. Note: it is necessary to use a list of arrays as the number of observations is
         not necessary the same at each data point.
     :param ionic_charge: The charge on the mobile ions, either an array with a value for each ion or a scalar
         if all values are the same.
     :param n_o: Number of statistically independent observations of the MSD at each timestep.
+    :param bootstrap: Should bootstrap resampling be used to estimate the observed MSD distribution.
+        Optional, default is :py:attr:`False`.
     :param sub_sample_dt: The frequency in observations to be sampled. Optional, default is :py:attr:`1`
         (every observation).
     :param n_resamples: The initial number of resamples to be performed. Optional, default is :py:attr:`1000`.
     :param max_resamples: The max number of resamples to be performed by the distribution is assumed to be normal.
         This is present to allow user control over the time taken for the resampling to occur. Optional, default
         is :py:attr:`100000`.
     :param dimension: Dimension/s to find the displacement along, this should be some subset of `'xyz'` indicating
@@ -594,14 +622,15 @@
 
     def __init__(self,
                  delta_t: np.ndarray,
                  disp_3d: List[np.ndarray],
                  ionic_charge: Union[np.ndarray, int],
                  n_o: np.ndarray,
                  sub_sample_dt: int = 1,
+                 bootstrap: bool = False,
                  n_resamples: int = 1000,
                  max_resamples: int = 10000,
                  dimension: str = 'xyz',
                  alpha: float = 1e-3,
                  random_state: np.random.mtrand.RandomState = None,
                  progress: bool = True):
         super().__init__(delta_t, disp_3d, n_o, sub_sample_dt, dimension)
@@ -613,46 +642,84 @@
         for i in self._iterator:
             disp_slice = self._displacements[i][:, :, self._slice].reshape(self._displacements[i].shape[0],
                                                                            self._displacements[i].shape[1], self.dims)
             d_squared = np.sum(disp_slice**2, axis=-1)
             sq_chg_motion = np.sum(np.sum((ionic_charge * self._displacements[i].T).T, axis=0)**2, axis=-1)
             if sq_chg_motion.size <= 1:
                 continue
-            self._n_o = np.append(self._n_o, n_o[i])
             self._euclidian_displacements.append(Distribution(np.sqrt(d_squared.flatten())))
-            distro = self.sample_until_normal(sq_chg_motion, int(n_o[i] / d_squared.shape[0]), n_resamples,
-                                              max_resamples, alpha, random_state)
-            self._distributions.append(distro)
-            self._n = np.append(self._n, distro.n)
-            self._s = np.append(self._s, np.std(distro.samples, ddof=1))
-            self._v = np.append(self._v, np.var(distro.samples, ddof=1))
+            if bootstrap:
+                distro = self.sample_until_normal(d_squared, n_o[i], n_resamples, max_resamples, alpha, random_state)
+                self._distributions.append(distro)
+                self._n_bootstrap = np.append(self._n_bootstrap, np.mean(distro.samples))
+                self._v_bootstrap = np.append(self._v_bootstrap, np.var(distro.samples, ddof=1))
+                self._s_bootstrap = np.append(self._s_bootstrap, np.std(distro.samples, ddof=1))
+            self._n = np.append(self._n, d_squared.mean())
+            self._v = np.append(self._v, np.var(d_squared, ddof=1) / n_o[i])
+            self._s = np.append(self._s, np.sqrt(self._v[i]))
             self._ngp = np.append(self._ngp, self.ngp_calculation(d_squared.flatten()))
             self._dt = np.append(self._dt, self._delta_t[i])
         self._n_o = self._n_o[:self._n.size]
 
 
-def _bootstrap(array: np.ndarray, n_samples: int, n_resamples: int, random_state: np.random.mtrand.RandomState = None):
+def _bootstrap(array: np.ndarray,
+               n_samples: int,
+               n_resamples: float,
+               random_state: np.random.mtrand.RandomState = None) -> List[float]:
     """
     Perform a set of resamples.
 
     :param array: The array to sample from.
     :param n_samples: Number of samples.
-    :param n_resamples: Number of resamples to perform initially.
-    :param dt: current timestep.
+    :param n_resamples: Number of resamples to perform.
     :param random_state: A :py:attr:`RandomState` object to be used to ensure reproducibility. Optional,
         default is :py:attr:`None`
 
-    :return: Resampled values from the array
+    :return: Simulated means from resampling the array.
     """
     return [
-        np.mean(resample(array.flatten(), n_samples=n_samples, random_state=random_state).flatten())
+        np.mean(resample(array.flatten(), n_samples=int(n_samples), random_state=random_state).flatten())
         for j in range(n_resamples)
     ]
 
 
+def _bayesian_bootstrap(array: np.ndarray,
+                        n_samples: float,
+                        n_resamples: int,
+                        random_state: np.random.mtrand.RandomState = None) -> List[float]:
+    """
+    Performs a Bayesian bootstrap simulation of the posterior distribution of the mean of observed values,
+    using a sparse Dirichlet prior for sample weights.
+    
+    The sparsity of the Dirichlet prior for the sample weights is controlled by a concentration parameter
+    alpha, where alpha = k(N-1)/(k-1). k is the dimensionality of the array of observed values, and 
+    N can be considered an effective number of samples for each set of sample weights.
+    alpha has been chosen to vary linearly with N, and gives a flat Dirichlet prior when N=k,
+    and a uniform categorical prior when N=1.
+    
+    :param array: The array to sample from.
+    :param n_samples: The effective number of samples for each set of simulated weights.
+    :param n_resamples: Number of resamples to perform.
+    :param random_state: A :py:attr:`RandomState` object. Optional, default is :py:attr:`None`
+    
+    :return: Samples from the simulated posterior distribution of the mean of the array.
+    """
+    if random_state == None:
+        random_state = np.random.mtrand.RandomState()
+    values = array.flatten()
+    k = len(values)
+    alphak = (n_samples - 1) / (k - 1)
+    if alphak > 0:
+        weights = random_state.dirichlet(alpha=np.ones(k) * alphak, size=n_resamples)
+    else:
+        # Sample from a uniform categorical distribution, equivalent to Dirichlet([0,0,0,…])
+        weights = random_state.multinomial(n=1, pvals=np.ones(k) / k, size=n_resamples)
+    return list(np.sum(weights * values, axis=1))
+
+
 def _populate_covariance_matrix(variances: np.ndarray, n_samples: np.ndarray) -> np.ndarray:
     """
     Populate the covariance matrix for the generalised least squares methodology.
 
     :param variances: The variances for each timestep
     :param n_samples: Number of independent trajectories for each timestep
```

### Comparing `kinisi-0.6.2/kinisi/diffusion_analyzer.py` & `kinisi-0.6.3/kinisi/diffusion_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         average from the data.
         """
         return self._diff.n
 
     @property
     def msd_std(self) -> np.ndarray:
         """
-        :return: MSD standard deviations values for the input trajectories.
+        :return: MSD standard deviation values for the input trajectories (a single standard deviation).
         """
         return self._diff.s
 
     @property
     def D(self) -> 'uravu.distribution.Distribution':
         """
         :return: Diffusion coefficient distribution.
```

### Comparing `kinisi-0.6.2/kinisi/jump_diffusion_analyzer.py` & `kinisi-0.6.3/kinisi/jump_diffusion_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
             average from the data.
         """
         return self._diff.n
 
     @property
     def tmsd_std(self) -> np.ndarray:
         """
-        :return: MSD standard deviations values for the input trajectories.
+        :return: MSD standard deviation values for the input trajectories (a single standard deviation).
         """
         return self._diff.s
 
     @property
     def D_J(self) -> 'uravu.distribution.Distribution':
         """
         :return: Jump diffusion coefficient
```

### Comparing `kinisi-0.6.2/kinisi/matrix.py` & `kinisi-0.6.3/kinisi/matrix.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/kinisi/parser.py` & `kinisi-0.6.3/kinisi/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             return np.unique(np.geomspace(min_dt, max_dt, n_steps, dtype=int))
         else:
             raise ValueError("Only linear or logarithmic spacing is allowed.")
 
     def get_disps(self,
                   timesteps: np.ndarray,
                   drift_corrected: np.ndarray,
-                  progress: bool = True) -> Tuple[np.ndarray, np.ndarray]:
+                  progress: bool = True) -> Tuple[np.ndarray, List[np.ndarray], np.ndarray]:
         """
         Calculate the displacement at each timestep.
 
         :param timesteps: Smoothed timesteps.
         :param drift_corrected: Drift of framework corrected disp.
         :param progress: Print progress bars to screen. Defaults to :py:attr:`True`.
 
@@ -199,15 +199,16 @@
                                       axis=1)
                 if np.multiply(*disp[:, ::timestep].shape[:2]) <= 1:
                     continue
                 disp_3d.append(disp)
             else:
                 raise ValueError(f"The sampling option of {self.sampling} is unrecognized, "
                                  "please use 'multi-origin' or 'single-origin'.")
-            n_samples = np.append(n_samples, np.multiply(*disp[:, ::timestep].shape[:2]))
+            # n_samples = np.append(n_samples, np.multiply(*disp[:, ::timestep].shape[:2]))
+            n_samples = np.append(n_samples, disp.shape[0] * timesteps[-1] / timestep)
         return delta_t, disp_3d, n_samples
 
 
 class PymatgenParser(Parser):
     """
     A parser for pymatgen structures.
```

### Comparing `kinisi-0.6.2/kinisi/tests/test_analyze.py` & `kinisi-0.6.3/kinisi/tests/test_analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,16 +209,14 @@
                                                     bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
             assert_almost_equal(a.tmsd, a._diff.n)
             assert_almost_equal(a.tmsd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
-            assert issubclass(w[0].category, UserWarning)
-            assert "maximum" in str(w[0].message)
 
     def test_diffusion(self):
         with warnings.catch_warnings(record=True) as w:
             a = JumpDiffusionAnalyzer.from_pymatgen(xd.structures,
                                                     parser_params=da_params,
                                                     bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
@@ -226,16 +224,14 @@
             assert_almost_equal(a.tmsd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
             a.jump_diffusion()
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.D_J, Distribution)
             assert a.flatchain.shape == (3200, 2)
-            assert issubclass(w[0].category, UserWarning)
-            assert "maximum" in str(w[0].message)
 
     def test_dictionary_roundtrip(self):
         with warnings.catch_warnings(record=True) as w:
             a = JumpDiffusionAnalyzer.from_pymatgen(xd.structures,
                                                     parser_params=da_params,
                                                     bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
@@ -243,15 +239,14 @@
             assert_almost_equal(a.tmsd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
             a.jump_diffusion()
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.D_J, Distribution)
             assert a.flatchain.shape == (3200, 2)
-            assert issubclass(w[0].category, UserWarning)
             b = JumpDiffusionAnalyzer.from_dict(a.to_dict())
             assert_equal(a.dt, b.dt)
             assert_equal(a.tmsd, b.tmsd)
             assert_equal(a.tmsd_std, b.tmsd_std)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, b.dr[i].samples)
             assert a.ngp_max == b.ngp_max
@@ -272,16 +267,14 @@
                                                    ionic_charge=1)
             assert_almost_equal(a.dt, a._diff.dt)
             assert_almost_equal(a.mscd, a._diff.n)
             assert_almost_equal(a.mscd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
-            assert issubclass(w[0].category, UserWarning)
-            assert "maximum" in str(w[0].message)
 
     def test_diffusion(self):
         with warnings.catch_warnings(record=True) as w:
             a = ConductivityAnalyzer.from_pymatgen(xd.structures,
                                                    parser_params=da_params,
                                                    bootstrap_params={'random_state': np.random.RandomState(0)},
                                                    ionic_charge=1)
@@ -290,16 +283,14 @@
             assert_almost_equal(a.mscd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
             a.conductivity(100)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.sigma, Distribution)
             assert a.flatchain.shape == (3200, 2)
-            assert issubclass(w[0].category, UserWarning)
-            assert "maximum" in str(w[0].message)
 
     def test_dictionary_roundtrip(self):
         with warnings.catch_warnings(record=True) as w:
             a = ConductivityAnalyzer.from_pymatgen(xd.structures,
                                                    parser_params=da_params,
                                                    bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
@@ -307,15 +298,14 @@
             assert_almost_equal(a.mscd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
             a.conductivity(100)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.sigma, Distribution)
             assert a.flatchain.shape == (3200, 2)
-            assert issubclass(w[0].category, UserWarning)
             b = ConductivityAnalyzer.from_dict(a.to_dict())
             assert_equal(a.dt, b.dt)
             assert_equal(a.mscd, b.mscd)
             assert_equal(a.mscd_std, b.mscd_std)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, b.dr[i].samples)
             assert a.ngp_max == b.ngp_max
```

### Comparing `kinisi-0.6.2/kinisi/tests/test_arrhenius.py` & `kinisi-0.6.3/kinisi/tests/test_arrhenius.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/kinisi/tests/test_diffusion.py` & `kinisi-0.6.3/kinisi/tests/test_diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,25 +190,25 @@
                 assert i.samples.size <= 110
 
     def test_initialisation_random_state(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs1 = MSDBootstrap(dt, disp_3d, n_o, random_state=np.random.RandomState(0))
+            bs1 = MSDBootstrap(dt, disp_3d, n_o, bootstrap=True, random_state=np.random.RandomState(0))
             assert bs1.n.shape == (10, )
             assert bs1.s.shape == (10, )
             assert_almost_equal(bs1.v, np.square(bs1.s))
             assert bs1.ngp.shape == (10, )
             assert len(bs1.euclidian_displacements) == 10
             for i in bs1.euclidian_displacements:
                 assert isinstance(i, Distribution)
             for i in bs1._distributions:
                 assert i.samples.size >= 1000
-            bs2 = MSDBootstrap(dt, disp_3d, n_o, random_state=np.random.RandomState(0))
+            bs2 = MSDBootstrap(dt, disp_3d, n_o, bootstrap=True, random_state=np.random.RandomState(0))
             assert bs1._distributions[-1].size == bs2._distributions[-1].size
             assert_almost_equal(bs1._distributions[-1].samples, bs2._distributions[-1].samples)
 
     def test_initialisation_progress(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
@@ -432,25 +432,25 @@
                 assert i.samples.size <= 110
 
     def test_initialisation_random_state(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs1 = TMSDBootstrap(dt, disp_3d, n_o, random_state=np.random.RandomState(0))
+            bs1 = TMSDBootstrap(dt, disp_3d, n_o, bootstrap=True, random_state=np.random.RandomState(0))
             assert bs1.n.shape == (5, )
             assert bs1.s.shape == (5, )
             assert_almost_equal(bs1.v, np.square(bs1.s))
             assert bs1.ngp.shape == (5, )
             assert len(bs1.euclidian_displacements) == 5
             for i in bs1.euclidian_displacements:
                 assert isinstance(i, Distribution)
             for i in bs1._distributions:
                 assert i.samples.size >= 1000
-            bs2 = TMSDBootstrap(dt, disp_3d, n_o, random_state=np.random.RandomState(0))
+            bs2 = TMSDBootstrap(dt, disp_3d, n_o, bootstrap=True, random_state=np.random.RandomState(0))
             assert bs1._distributions[-1].size == bs2._distributions[-1].size
             assert_almost_equal(bs1._distributions[-1].samples, bs2._distributions[-1].samples)
 
     def test_initialisation_progress(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
@@ -639,25 +639,25 @@
                 assert i.samples.size <= 110
 
     def test_initialisation_random_state(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs1 = MSCDBootstrap(dt, disp_3d, 1, n_o, random_state=np.random.RandomState(0))
+            bs1 = MSCDBootstrap(dt, disp_3d, 1, n_o, bootstrap=True, random_state=np.random.RandomState(0))
             assert bs1.n.shape == (5, )
             assert bs1.s.shape == (5, )
             assert_almost_equal(bs1.v, np.square(bs1.s))
             assert bs1.ngp.shape == (5, )
             assert len(bs1.euclidian_displacements) == 5
             for i in bs1.euclidian_displacements:
                 assert isinstance(i, Distribution)
             for i in bs1._distributions:
                 assert i.samples.size >= 1000
-            bs2 = MSCDBootstrap(dt, disp_3d, 1, n_o, random_state=np.random.RandomState(0))
+            bs2 = MSCDBootstrap(dt, disp_3d, 1, n_o, bootstrap=True, random_state=np.random.RandomState(0))
             assert bs1._distributions[-1].size == bs2._distributions[-1].size
             assert_almost_equal(bs1._distributions[-1].samples, bs2._distributions[-1].samples)
 
     def test_initialisation_progress(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
```

### Comparing `kinisi-0.6.2/kinisi/tests/test_matrix.py` & `kinisi-0.6.3/kinisi/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/kinisi/tests/test_parser.py` & `kinisi-0.6.3/kinisi/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/kinisi/tests/inputs/example_LAMMPS.data` & `kinisi-0.6.3/kinisi/tests/inputs/example_LAMMPS.data`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/kinisi/tests/inputs/example_LAMMPS.dcd` & `kinisi-0.6.3/kinisi/tests/inputs/example_LAMMPS.dcd`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/kinisi/tests/inputs/example_XDATCAR.gz` & `kinisi-0.6.3/kinisi/tests/inputs/example_XDATCAR.gz`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/LICENSE` & `kinisi-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/README.md` & `kinisi-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.2/pyproject.toml` & `kinisi-0.6.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Topic :: Scientific/Engineering',
     'Topic :: Scientific/Engineering :: Chemistry',
     'Topic :: Scientific/Engineering :: Physics'
 ]
-requires-python = ">=3.8,<3.11"
+requires-python = ">=3.8"
 dependencies = [
     'numpy',
     'scikit-learn',
     'scipy>=1.9.3',
     'tqdm',
     'uravu>=1.2.9'
 ]
```

### Comparing `kinisi-0.6.2/PKG-INFO` & `kinisi-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kinisi
-Version: 0.6.2
+Version: 0.6.3
 Summary: Efficient estimation of diffusion processes from molecular dynamics.
 Project-URL: homepage, https://github.com/bjmorgan/kinisi
 Project-URL: documentation, https://kinisi.rtfd.io
 Author-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, "Benjamin J. Morgan" <b.j.morgan@bath.ac.uk>
 Maintainer-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, "Benjamin J. Morgan" <b.j.morgan@bath.ac.uk>
 License-Expression: MIT
 License-File: LICENSE
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: scipy>=1.9.3
 Requires-Dist: tqdm
 Requires-Dist: uravu>=1.2.9
 Provides-Extra: dev
 Requires-Dist: codeclimate-test-reporter; extra == 'dev'
```

