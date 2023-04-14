# Comparing `tmp/PxMCMC-0.1.4.tar.gz` & `tmp/pxmcmc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PxMCMC-0.1.4.tar", max compression
+gzip compressed data, was "pxmcmc-0.1.5.tar", max compression
```

## Comparing `PxMCMC-0.1.4.tar` & `pxmcmc-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    35149 2021-07-22 08:20:25.513019 PxMCMC-0.1.4/LICENSE
--rw-r--r--   0        0        0      935 2022-06-06 09:33:25.280600 PxMCMC-0.1.4/README.md
--rw-r--r--   0        0        0       22 2022-06-06 09:33:25.282836 PxMCMC-0.1.4/pxmcmc/__init__.py
--rw-r--r--   0        0        0     5518 2022-10-11 09:57:40.987916 PxMCMC-0.1.4/pxmcmc/forward.py
--rw-r--r--   0        0        0    12744 2022-06-13 08:58:38.009082 PxMCMC-0.1.4/pxmcmc/mcmc.py
--rw-r--r--   0        0        0     8463 2022-06-13 08:58:38.009287 PxMCMC-0.1.4/pxmcmc/measurements.py
--rw-r--r--   0        0        0     6354 2022-06-13 08:58:38.009458 PxMCMC-0.1.4/pxmcmc/plotting.py
--rw-r--r--   0        0        0     2617 2022-06-06 09:33:25.284200 PxMCMC-0.1.4/pxmcmc/prior.py
--rw-r--r--   0        0        0     1757 2021-06-28 20:26:37.306610 PxMCMC-0.1.4/pxmcmc/saving.py
--rw-r--r--   0        0        0     4931 2022-06-13 08:58:38.009771 PxMCMC-0.1.4/pxmcmc/transforms.py
--rw-r--r--   0        0        0     2115 2021-06-28 20:26:37.313172 PxMCMC-0.1.4/pxmcmc/uncertainty.py
--rw-r--r--   0        0        0    10289 2022-06-13 08:58:38.010029 PxMCMC-0.1.4/pxmcmc/utils.py
--rw-r--r--   0        0        0     1016 2022-10-11 12:45:58.051099 PxMCMC-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 PxMCMC-0.1.4/setup.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 PxMCMC-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-07-22 08:20:25.513019 pxmcmc-0.1.5/LICENSE
+-rw-r--r--   0        0        0      935 2022-06-06 09:33:25.280600 pxmcmc-0.1.5/README.md
+-rw-r--r--   0        0        0       22 2022-06-06 09:33:25.282836 pxmcmc-0.1.5/pxmcmc/__init__.py
+-rw-r--r--   0        0        0     5518 2023-03-30 05:07:33.968909 pxmcmc-0.1.5/pxmcmc/forward.py
+-rw-r--r--   0        0        0    13473 2023-04-14 06:38:56.774037 pxmcmc-0.1.5/pxmcmc/mcmc.py
+-rw-r--r--   0        0        0     8463 2022-06-13 08:58:38.009287 pxmcmc-0.1.5/pxmcmc/measurements.py
+-rw-r--r--   0        0        0     6354 2023-03-30 05:07:33.971536 pxmcmc-0.1.5/pxmcmc/plotting.py
+-rw-r--r--   0        0        0     5447 2023-04-14 06:53:29.509093 pxmcmc-0.1.5/pxmcmc/prior.py
+-rw-r--r--   0        0        0     1757 2021-06-28 20:26:37.306610 pxmcmc-0.1.5/pxmcmc/saving.py
+-rw-r--r--   0        0        0     4931 2023-03-30 05:07:33.973061 pxmcmc-0.1.5/pxmcmc/transforms.py
+-rw-r--r--   0        0        0     2115 2021-06-28 20:26:37.313172 pxmcmc-0.1.5/pxmcmc/uncertainty.py
+-rw-r--r--   0        0        0    10289 2023-03-30 05:07:33.973877 pxmcmc-0.1.5/pxmcmc/utils.py
+-rw-r--r--   0        0        0     1060 2023-04-14 06:55:06.772156 pxmcmc-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2246 1970-01-01 00:00:00.000000 pxmcmc-0.1.5/PKG-INFO
```

### Comparing `PxMCMC-0.1.4/LICENSE` & `pxmcmc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PxMCMC-0.1.4/README.md` & `pxmcmc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `PxMCMC-0.1.4/pxmcmc/forward.py` & `pxmcmc-0.1.5/pxmcmc/forward.py`

 * *Files identical despite different names*

### Comparing `PxMCMC-0.1.4/pxmcmc/mcmc.py` & `pxmcmc-0.1.5/pxmcmc/mcmc.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,20 @@
     def __init__(self, forward, prior, mcmcparams=PxMCMCParams()):
         self.forward = forward
         self.prior = prior
         for attr in mcmcparams.__dict__.keys():
             setattr(self, attr, getattr(mcmcparams, attr))
         self._initialise_tracking_arrays()
 
-    def run(self):
+    def run(self, start_point=None):
+        """
+        Implementation of the MCMC
+
+        :param start_point: vector of model parameters for the start point of the chain (default :code:`None`).
+        """
         raise NotImplementedError
 
     def logpi(self, X, preds):
         """
         Calculates the log(posterior), L2-norm and prior-norm of a model.
 
         :param X: vector of model parameters
@@ -85,19 +90,27 @@
 
     def _print_progress(self, i, logpi, **kwargs):
         print(
             f"{i+1:,}/{self.nsamples:,} - logposterior: {logpi:.8e} - "
             + " - ".join([f"{k}: {kwargs[k]:.8e}" for k in kwargs]),
         )
 
-    def _initial_sample(self):
-        # TODO: flexibility for different priors
-        X_curr = laplace.rvs(size=self.forward.nparams)
-        if self.complex:
-            X_curr = X_curr + laplace.rvs(size=self.forward.nparams) * 1j
+    def _initial_sample(self, initial_sample=None):
+        if initial_sample is None:
+            # TODO: flexibility for different priors
+            X_curr = laplace.rvs(size=self.forward.nparams)
+            if self.complex:
+                X_curr = X_curr + laplace.rvs(size=self.forward.nparams) * 1j
+        else:
+            if not isinstance(initial_sample, np.ndarray) or np.ndim(initial_sample) != 1:
+                raise TypeError("Expected a 1D numpy array as an initial sample")
+            if initial_sample.size == self.forward.nparams:
+                X_curr = initial_sample
+            else:
+                raise ValueError("Inital sample given has incorrect size")
         curr_preds = self.forward.forward(X_curr)
         return X_curr, curr_preds
 
     def _initialise_tracking_arrays(self):
         if "logposterior" in self.track:
             self.logPi = np.zeros(self.nsamples)
         if "predictions" in self.track:
@@ -130,21 +143,21 @@
 class MYULA(PxMCMC):
     """
     Implements the MYULA chain
     """
     def __init__(self, forward, prox, mcmcparams=PxMCMCParams()):
         super().__init__(forward, prox, mcmcparams)
 
-    def run(self):
+    def run(self, start_point=None):
         """
         Run the algorithm
         """
         i = 0  # total samples
         j = 0  # saved samples (excludes burn-in and thinned samples)
-        X_curr, curr_preds = self._initial_sample()
+        X_curr, curr_preds = self._initial_sample(start_point)
         while j < self.nsamples:
             gradg = self.forward.calc_gradg(curr_preds)
             proxf = self.prior.proxf(X_curr)
             X_prop = self.chain_step(X_curr, proxf, gradg)
             prop_preds = self.forward.forward(X_prop)
 
             X_curr = X_prop
@@ -198,23 +211,23 @@
 
        Option to tune :code:`delta` to any desired acceptance probability.
     """
     def __init__(self, forward, prox, mcmcparams=PxMCMCParams(), tune_delta=True):
         super().__init__(forward, prox, mcmcparams)
         self.tune_delta = tune_delta
 
-    def run(self):
+    def run(self, start_point=None):
         """
         Run the algorithm
         """
         self.acceptance_trace = []
         self.deltas_trace = [self.delta]
         i = 0
         j = 0
-        X_curr, curr_preds = self._initial_sample()
+        X_curr, curr_preds = self._initial_sample(start_point)
         gradg_curr = self.forward.calc_gradg(curr_preds)
         proxf_curr = self.prior.proxf(X_curr)
         logpiXc, L2Xc, priorXc = self.logpi(X_curr, curr_preds)
         while j < self.nsamples:
             X_prop = self.chain_step(X_curr, proxf_curr, gradg_curr)
             prop_preds = self.forward.forward(X_prop)
             gradg_prop = self.forward.calc_gradg(prop_preds)
@@ -288,21 +301,21 @@
 
         super().__init__(forward, prox, mcmcparams=mcmcparams)
         self.eta = 0.05
         self.omega_0 = 1 + self.eta / (self.s * self.s)
         self.omega_1 = chebyshev1(self.omega_0, self.s) / cheb1der(self.omega_0, self.s)
         self._recursion_coefs()
 
-    def run(self):
+    def run(self, start_point=None):
         """
         Run the algorithm
         """
         i = 0  # total samples
         j = 0  # saved samples (excludes burn-in and thinned samples)
-        X_curr, curr_preds = self._initial_sample()
+        X_curr, curr_preds = self._initial_sample(start_point)
         while j < self.nsamples:
             X_prop = self.chain_step(X_curr)
             prop_preds = self.forward.forward(X_prop)
 
             X_curr = X_prop
             curr_preds = prop_preds
```

### Comparing `PxMCMC-0.1.4/pxmcmc/measurements.py` & `pxmcmc-0.1.5/pxmcmc/measurements.py`

 * *Files identical despite different names*

### Comparing `PxMCMC-0.1.4/pxmcmc/plotting.py` & `pxmcmc-0.1.5/pxmcmc/plotting.py`

 * *Files identical despite different names*

### Comparing `PxMCMC-0.1.4/pxmcmc/saving.py` & `pxmcmc-0.1.5/pxmcmc/saving.py`

 * *Files identical despite different names*

### Comparing `PxMCMC-0.1.4/pxmcmc/transforms.py` & `pxmcmc-0.1.5/pxmcmc/transforms.py`

 * *Files identical despite different names*

### Comparing `PxMCMC-0.1.4/pxmcmc/uncertainty.py` & `pxmcmc-0.1.5/pxmcmc/uncertainty.py`

 * *Files identical despite different names*

### Comparing `PxMCMC-0.1.4/pxmcmc/utils.py` & `pxmcmc-0.1.5/pxmcmc/utils.py`

 * *Files identical despite different names*

### Comparing `PxMCMC-0.1.4/pyproject.toml` & `pxmcmc-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [tool.poetry]
 name = "PxMCMC"
-version = "0.1.4"
+version = "0.1.5"
 authors = ["Auggie Marignier <augustin.marignier.14@ucl.ac.uk>"]
 description = "Proximal Markov Chain Monte Carlo"
 homepage = "https://github.com/auggiemarignier/pxmcmc"
 repository = "https://github.com/auggiemarignier/pxmcmc"
 license = "GPL-3.0-or-later"
 documentation = "https://pxmcmc.readthedocs.io/en/latest/index.html"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.8,<4.0"
 numpy = "^1.21.1"
 matplotlib = "^3.4.2"
 pyssht = "^1.4.0"
 pys2let = "^2.2.3"
 greatcirclepaths = "^1.1.0"
 h5py = "^3.3.0"
 Cartopy = {version = "^0.19.0", optional = true}
 sphinx = {version = "^4", optional = true}
 astropy = "^5.0.4"
 sphinx-rtd-theme = {version = "^1.0.0", optional = true}
 scipy = "^1.9.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+pytest = "^7.0"
 black = "^19.10b0"
 flake8 = "^3.7.9"
-pytest-cases = "^2.0.4"
+
+[tool.poetry.group.dev.dependencies]
+pytest-cases = "^3.6.13"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-rtd-theme"]
```

### Comparing `PxMCMC-0.1.4/PKG-INFO` & `pxmcmc-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: pxmcmc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Proximal Markov Chain Monte Carlo
 Home-page: https://github.com/auggiemarignier/pxmcmc
 License: GPL-3.0-or-later
 Author: Auggie Marignier
 Author-email: augustin.marignier.14@ucl.ac.uk
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cartopy
 Provides-Extra: docs
-Requires-Dist: Cartopy (>=0.19.0,<0.20.0); extra == "cartopy"
+Requires-Dist: Cartopy (>=0.19.0,<0.20.0) ; extra == "cartopy"
 Requires-Dist: astropy (>=5.0.4,<6.0.0)
 Requires-Dist: greatcirclepaths (>=1.1.0,<2.0.0)
 Requires-Dist: h5py (>=3.3.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.4.2,<4.0.0)
 Requires-Dist: numpy (>=1.21.1,<2.0.0)
 Requires-Dist: pys2let (>=2.2.3,<3.0.0)
 Requires-Dist: pyssht (>=1.4.0,<2.0.0)
 Requires-Dist: scipy (>=1.9.2,<2.0.0)
-Requires-Dist: sphinx (>=4,<5); extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0); extra == "docs"
+Requires-Dist: sphinx (>=4,<5) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs"
 Project-URL: Documentation, https://pxmcmc.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/auggiemarignier/pxmcmc
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/pxmcmc/badge/?version=latest)](https://pxmcmc.readthedocs.io/en/latest/?badge=latest)
 
 # Python ProxMCMC
```

