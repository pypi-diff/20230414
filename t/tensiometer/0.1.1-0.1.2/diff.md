# Comparing `tmp/tensiometer-0.1.1.tar.gz` & `tmp/tensiometer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tensiometer-0.1.1.tar", last modified: Wed May 26 14:18:42 2021, max compression
+gzip compressed data, was "tensiometer-0.1.2.tar", last modified: Fri Apr 14 15:56:09 2023, max compression
```

## Comparing `tensiometer-0.1.1.tar` & `tensiometer-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2021-05-26 14:18:42.000000 tensiometer-0.1.1/
--rw-r--r--   0 marco      (501) staff       (20)     3098 2021-05-10 14:11:00.000000 tensiometer-0.1.1/.material.py
--rw-r--r--   0 marco      (501) staff       (20)       32 2020-10-05 19:39:07.000000 tensiometer-0.1.1/MANIFEST.in
--rw-r--r--   0 marco      (501) staff       (20)     3539 2021-05-26 14:18:42.000000 tensiometer-0.1.1/PKG-INFO
--rw-r--r--   0 marco      (501) staff       (20)     2406 2021-05-10 14:11:00.000000 tensiometer-0.1.1/README.rst
--rw-r--r--   0 marco      (501) staff       (20)       38 2021-05-26 14:18:42.000000 tensiometer-0.1.1/setup.cfg
--rw-r--r--   0 marco      (501) staff       (20)     2749 2021-05-10 14:14:34.000000 tensiometer-0.1.1/setup.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2021-05-26 14:18:42.000000 tensiometer-0.1.1/tensiometer/
--rw-r--r--   0 marco      (501) staff       (20)      163 2021-05-26 14:13:25.000000 tensiometer-0.1.1/tensiometer/__init__.py
--rw-r--r--   0 marco      (501) staff       (20)    14904 2021-04-15 00:20:09.000000 tensiometer-0.1.1/tensiometer/chains_convergence.py
--rw-r--r--   0 marco      (501) staff       (20)    15767 2021-05-10 14:11:00.000000 tensiometer-0.1.1/tensiometer/cosmosis_interface.py
--rw-r--r--   0 marco      (501) staff       (20)     4211 2021-05-10 14:11:00.000000 tensiometer-0.1.1/tensiometer/experimental.py
--rw-r--r--   0 marco      (501) staff       (20)    51242 2021-05-10 14:11:00.000000 tensiometer-0.1.1/tensiometer/gaussian_tension.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2021-05-26 14:18:42.000000 tensiometer-0.1.1/tensiometer/mcmc_tension/
--rw-r--r--   0 marco      (501) staff       (20)     1111 2021-05-10 14:11:00.000000 tensiometer-0.1.1/tensiometer/mcmc_tension/__init__.py
--rw-r--r--   0 marco      (501) staff       (20)    26136 2021-05-26 14:12:55.000000 tensiometer-0.1.1/tensiometer/mcmc_tension/flow.py
--rw-r--r--   0 marco      (501) staff       (20)    43510 2021-05-10 14:11:00.000000 tensiometer-0.1.1/tensiometer/mcmc_tension/kde.py
--rw-r--r--   0 marco      (501) staff       (20)    12309 2021-05-10 14:11:00.000000 tensiometer-0.1.1/tensiometer/mcmc_tension/param_diff.py
--rw-r--r--   0 marco      (501) staff       (20)    25511 2021-05-10 14:11:00.000000 tensiometer-0.1.1/tensiometer/tensor_eigenvalues.py
--rw-r--r--   0 marco      (501) staff       (20)    15552 2021-05-10 14:11:00.000000 tensiometer-0.1.1/tensiometer/utilities.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2021-05-26 14:18:42.000000 tensiometer-0.1.1/tensiometer.egg-info/
--rw-r--r--   0 marco      (501) staff       (20)     3539 2021-05-26 14:18:42.000000 tensiometer-0.1.1/tensiometer.egg-info/PKG-INFO
--rw-r--r--   0 marco      (501) staff       (20)      604 2021-05-26 14:18:42.000000 tensiometer-0.1.1/tensiometer.egg-info/SOURCES.txt
--rw-r--r--   0 marco      (501) staff       (20)        1 2021-05-26 14:18:42.000000 tensiometer-0.1.1/tensiometer.egg-info/dependency_links.txt
--rw-r--r--   0 marco      (501) staff       (20)        1 2021-03-23 02:27:06.000000 tensiometer-0.1.1/tensiometer.egg-info/not-zip-safe
--rw-r--r--   0 marco      (501) staff       (20)      181 2021-05-26 14:18:42.000000 tensiometer-0.1.1/tensiometer.egg-info/requires.txt
--rw-r--r--   0 marco      (501) staff       (20)       12 2021-05-26 14:18:42.000000 tensiometer-0.1.1/tensiometer.egg-info/top_level.txt
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-04-14 15:56:09.647624 tensiometer-0.1.2/
+-rw-r--r--   0 marco      (501) staff       (20)     3098 2023-01-07 09:10:42.000000 tensiometer-0.1.2/.material.py
+-rw-r--r--   0 marco      (501) staff       (20)    34502 2023-01-07 09:10:42.000000 tensiometer-0.1.2/LICENSE
+-rw-r--r--   0 marco      (501) staff       (20)       32 2023-01-07 09:10:42.000000 tensiometer-0.1.2/MANIFEST.in
+-rw-r--r--   0 marco      (501) staff       (20)     3100 2023-04-14 15:56:09.647365 tensiometer-0.1.2/PKG-INFO
+-rw-r--r--   0 marco      (501) staff       (20)     2406 2023-01-07 09:10:42.000000 tensiometer-0.1.2/README.rst
+-rw-r--r--   0 marco      (501) staff       (20)       38 2023-04-14 15:56:09.647712 tensiometer-0.1.2/setup.cfg
+-rw-r--r--   0 marco      (501) staff       (20)     2749 2023-01-07 09:10:42.000000 tensiometer-0.1.2/setup.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-04-14 15:56:09.643563 tensiometer-0.1.2/tensiometer/
+-rw-r--r--   0 marco      (501) staff       (20)      163 2023-04-14 15:52:22.000000 tensiometer-0.1.2/tensiometer/__init__.py
+-rw-r--r--   0 marco      (501) staff       (20)    14904 2023-01-07 09:10:42.000000 tensiometer-0.1.2/tensiometer/chains_convergence.py
+-rw-r--r--   0 marco      (501) staff       (20)    15767 2023-01-07 09:10:42.000000 tensiometer-0.1.2/tensiometer/cosmosis_interface.py
+-rw-r--r--   0 marco      (501) staff       (20)     4211 2023-01-07 09:10:42.000000 tensiometer-0.1.2/tensiometer/experimental.py
+-rw-r--r--   0 marco      (501) staff       (20)    51242 2023-01-07 09:10:42.000000 tensiometer-0.1.2/tensiometer/gaussian_tension.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-04-14 15:56:09.646976 tensiometer-0.1.2/tensiometer/mcmc_tension/
+-rw-r--r--   0 marco      (501) staff       (20)     1111 2023-01-07 09:10:42.000000 tensiometer-0.1.2/tensiometer/mcmc_tension/__init__.py
+-rw-r--r--   0 marco      (501) staff       (20)    26170 2023-01-07 09:10:42.000000 tensiometer-0.1.2/tensiometer/mcmc_tension/flow.py
+-rw-r--r--   0 marco      (501) staff       (20)    43510 2023-01-07 09:10:42.000000 tensiometer-0.1.2/tensiometer/mcmc_tension/kde.py
+-rw-r--r--   0 marco      (501) staff       (20)    12497 2023-04-14 15:46:52.000000 tensiometer-0.1.2/tensiometer/mcmc_tension/param_diff.py
+-rw-r--r--   0 marco      (501) staff       (20)    25511 2023-01-07 09:10:42.000000 tensiometer-0.1.2/tensiometer/tensor_eigenvalues.py
+-rw-r--r--   0 marco      (501) staff       (20)    15552 2023-01-07 09:10:42.000000 tensiometer-0.1.2/tensiometer/utilities.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-04-14 15:56:09.645556 tensiometer-0.1.2/tensiometer.egg-info/
+-rw-r--r--   0 marco      (501) staff       (20)     3100 2023-04-14 15:56:09.000000 tensiometer-0.1.2/tensiometer.egg-info/PKG-INFO
+-rw-r--r--   0 marco      (501) staff       (20)      612 2023-04-14 15:56:09.000000 tensiometer-0.1.2/tensiometer.egg-info/SOURCES.txt
+-rw-r--r--   0 marco      (501) staff       (20)        1 2023-04-14 15:56:09.000000 tensiometer-0.1.2/tensiometer.egg-info/dependency_links.txt
+-rw-r--r--   0 marco      (501) staff       (20)        1 2023-04-14 15:49:41.000000 tensiometer-0.1.2/tensiometer.egg-info/not-zip-safe
+-rw-r--r--   0 marco      (501) staff       (20)      181 2023-04-14 15:56:09.000000 tensiometer-0.1.2/tensiometer.egg-info/requires.txt
+-rw-r--r--   0 marco      (501) staff       (20)       12 2023-04-14 15:56:09.000000 tensiometer-0.1.2/tensiometer.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tensiometer-0.1.1/.material.py` & `tensiometer-0.1.2/.material.py`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/PKG-INFO` & `tensiometer-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,78 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: tensiometer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tension tools for posterior distributions
 Home-page: https://tensiometer.readthedocs.io
 Author: Marco Raveri
 License: GPL
 Project-URL: Source, https://github.com/mraveri/tensiometer
 Project-URL: Tracker, https://github.com/mraveri/tensiometer/issues
 Project-URL: Reference, https://arxiv.org/abs/1806.04649
 Project-URL: Licensing, https://raw.githubusercontent.com/mraveri/tensiometer/master/LICENSE
-Description: ============
-        Tensiometer
-        ============
-        -------------------------------
-         Test a model until it breaks!
-        -------------------------------
-        :Tensiometer: utilities to understand concordance and discordance of posterior distributions
-        :Author: Marco Raveri and Cyrille Doux
-        :Homepage: https://tensiometer.readthedocs.io
-        :Source: https://github.com/mraveri/tensiometer
-        :References: https://arxiv.org/abs/2105.03324 (non-Gaussian metrics), https://arxiv.org/abs/1806.04649 and https://arxiv.org/abs/1912.04880 (Gaussian)
-        
-        .. image:: https://travis-ci.org/mraveri/tensiometer.svg?branch=master
-            :target: https://travis-ci.org/mraveri/tensiometer
-        .. image:: https://readthedocs.org/projects/tensiometer/badge/?version=latest
-           :target: https://tensiometer.readthedocs.org/en/latest
-        .. image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/mraveri/tensiometer/master?filepath=docs%2Fexample_notebooks%2Ftension_example.ipynb
-        .. image:: https://coveralls.io/repos/github/mraveri/tensiometer/badge.svg?branch=master
-           :target: https://coveralls.io/github/mraveri/tensiometer?branch=master
-        .. image:: https://img.shields.io/pypi/v/tensiometer.svg?style=flat
-           :target: https://pypi.python.org/pypi/tensiometer/
-        
-        Description
-        ============
-        
-        The tensiometer package is a collection of tools to test the level of
-        agreement/disagreement between different posterior distributions.
-        
-        The best way to get up to speed is to read through the worked example
-        `full worked example <https://tensiometer.readthedocs.org/en/latest/tension_example.html>`_
-        that you can `run online <https://mybinder.org/v2/gh/mraveri/tensiometer/master?filepath=docs%2Fexample_notebooks%2Ftension_example.ipynb>`_! There's also a documented example of
-        `non-Gaussian tension estimates between DES Y1 and Planck 18 <https://tensiometer.readthedocs.io/en/latest/non_gaussian_tension.html>`_.
-        
-        
-        Installation
-        =============
-        
-        The tensiometer package is available on PyPI and can be easily installed with::
-        
-          pip install tensiometer
-        
-        Alternatively one can download the source code from github::
-        
-          git clone https://github.com/mraveri/tensiometer.git
-        
-        and install it locally with the shortcut::
-        
-          make install
-        
-        You can test that the code is working properly by using::
-        
-          make test
-        
-        
-        Dependencies
-        
 Keywords: MCMC
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
+License-File: LICENSE
+
+============
+Tensiometer
+============
+-------------------------------
+ Test a model until it breaks!
+-------------------------------
+:Tensiometer: utilities to understand concordance and discordance of posterior distributions
+:Author: Marco Raveri and Cyrille Doux
+:Homepage: https://tensiometer.readthedocs.io
+:Source: https://github.com/mraveri/tensiometer
+:References: https://arxiv.org/abs/2105.03324 (non-Gaussian metrics), https://arxiv.org/abs/1806.04649 and https://arxiv.org/abs/1912.04880 (Gaussian)
+
+.. image:: https://travis-ci.org/mraveri/tensiometer.svg?branch=master
+    :target: https://travis-ci.org/mraveri/tensiometer
+.. image:: https://readthedocs.org/projects/tensiometer/badge/?version=latest
+   :target: https://tensiometer.readthedocs.org/en/latest
+.. image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/mraveri/tensiometer/master?filepath=docs%2Fexample_notebooks%2Ftension_example.ipynb
+.. image:: https://coveralls.io/repos/github/mraveri/tensiometer/badge.svg?branch=master
+   :target: https://coveralls.io/github/mraveri/tensiometer?branch=master
+.. image:: https://img.shields.io/pypi/v/tensiometer.svg?style=flat
+   :target: https://pypi.python.org/pypi/tensiometer/
+
+Description
+============
+
+The tensiometer package is a collection of tools to test the level of
+agreement/disagreement between different posterior distributions.
+
+The best way to get up to speed is to read through the worked example
+`full worked example <https://tensiometer.readthedocs.org/en/latest/tension_example.html>`_
+that you can `run online <https://mybinder.org/v2/gh/mraveri/tensiometer/master?filepath=docs%2Fexample_notebooks%2Ftension_example.ipynb>`_! There's also a documented example of
+`non-Gaussian tension estimates between DES Y1 and Planck 18 <https://tensiometer.readthedocs.io/en/latest/non_gaussian_tension.html>`_.
+
+
+Installation
+=============
+
+The tensiometer package is available on PyPI and can be easily installed with::
+
+  pip install tensiometer
+
+Alternatively one can download the source code from github::
+
+  git clone https://github.com/mraveri/tensiometer.git
+
+and install it locally with the shortcut::
+
+  make install
+
+You can test that the code is working properly by using::
+
+  make test
+
+
+Dependencies
```

### Comparing `tensiometer-0.1.1/README.rst` & `tensiometer-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/setup.py` & `tensiometer-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/tensiometer/chains_convergence.py` & `tensiometer-0.1.2/tensiometer/chains_convergence.py`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/tensiometer/cosmosis_interface.py` & `tensiometer-0.1.2/tensiometer/cosmosis_interface.py`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/tensiometer/experimental.py` & `tensiometer-0.1.2/tensiometer/experimental.py`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/tensiometer/gaussian_tension.py` & `tensiometer-0.1.2/tensiometer/gaussian_tension.py`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/tensiometer/mcmc_tension/__init__.py` & `tensiometer-0.1.2/tensiometer/mcmc_tension/__init__.py`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/tensiometer/mcmc_tension/flow.py` & `tensiometer-0.1.2/tensiometer/mcmc_tension/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,21 +245,21 @@
         test_idx, training_idx = indices[:n_split], indices[n_split:]
 
         # Training
         self.X = diff_chain.samples[training_idx, :][:, ind]
         self.weights = diff_chain.weights[training_idx]
         self.weights *= len(self.weights) / np.sum(self.weights)  # weights normalized to number of samples
         self.has_weights = np.any(self.weights != self.weights[0])
-        self.Y = np.array(self.Y2X_bijector.inverse(self.X))
+        self.Y = np.array(self.Y2X_bijector.inverse(self.X.astype(np.float32)))
         assert not np.any(np.isnan(self.Y))
         self.num_samples = len(self.X)
 
         # Test
         self.X_test = diff_chain.samples[test_idx, :][:, ind]
-        self.Y_test = np.array(self.Y2X_bijector.inverse(self.X_test))
+        self.Y_test = np.array(self.Y2X_bijector.inverse(self.X_test.astype(np.float32)))
         self.weights_test = diff_chain.weights[test_idx]
         self.weights_test *= len(self.weights_test) / np.sum(self.weights_test)  # weights normalized to number of samples
 
         # Training sample generator
         Y_ds = tf.data.Dataset.from_tensor_slices((self.Y.astype(np.float32),                     # input
                                                    np.zeros(self.num_samples, dtype=np.float32),  # output (dummy zero)
                                                    self.weights.astype(np.float32),))             # weights
@@ -509,14 +509,14 @@
     :type tol: float, optional
     :param max_iter: maximum number of sampling steps, defaults to 1000.
     :type max_iter: int, optional
     :param step: number of samples per step, defaults to 100000.
     :type step: int, optional
     :return: probability value and error estimate.
     """
-    
+
     # Callback/model handler
     diff_flow_callback = DiffFlowCallback(diff_chain, param_names=param_names, **kwargs)
     # Train model
     diff_flow_callback.train(epochs=epochs, batch_size=batch_size, steps_per_epoch=steps_per_epoch, callbacks=callbacks, verbose=verbose)
     # Compute tension
     return diff_flow_callback.estimate_shift(tol=tol, max_iter=max_iter, step=step)
```

### Comparing `tensiometer-0.1.1/tensiometer/mcmc_tension/kde.py` & `tensiometer-0.1.2/tensiometer/mcmc_tension/kde.py`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/tensiometer/mcmc_tension/param_diff.py` & `tensiometer-0.1.2/tensiometer/mcmc_tension/param_diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,19 +218,25 @@
     # get parameter indexes:
     indexes_1 = [chain_1.index[name] for name in param_names]
     indexes_2 = [chain_2.index[name] for name in param_names]
     # get separate chains:
     if not hasattr(chain_1, 'chain_offsets'):
         _chains_1 = [chain_1]
     else:
-        _chains_1 = chain_1.getSeparateChains()
+        if chain_1.chain_offsets is None:
+            _chains_1 = [chain_1]
+        else:
+            _chains_1 = chain_1.getSeparateChains()
     if not hasattr(chain_2, 'chain_offsets'):
         _chains_2 = [chain_2]
     else:
-        _chains_2 = chain_2.getSeparateChains()
+        if chain_2.chain_offsets is None:
+            _chains_2 = [chain_2]
+        else:
+            _chains_2 = chain_2.getSeparateChains()
     # set the boost:
     if chain_1.sampler == 'nested' \
        or chain_2.sampler == 'nested' or boost is None:
         chain_boost = max(len(_chains_1), len(_chains_2))
         sample_boost = None
     else:
         chain_boost = min(boost, max(len(_chains_1), len(_chains_2)))
```

### Comparing `tensiometer-0.1.1/tensiometer/tensor_eigenvalues.py` & `tensiometer-0.1.2/tensiometer/tensor_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/tensiometer/utilities.py` & `tensiometer-0.1.2/tensiometer/utilities.py`

 * *Files identical despite different names*

### Comparing `tensiometer-0.1.1/tensiometer.egg-info/PKG-INFO` & `tensiometer-0.1.2/tensiometer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,78 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: tensiometer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tension tools for posterior distributions
 Home-page: https://tensiometer.readthedocs.io
 Author: Marco Raveri
 License: GPL
 Project-URL: Source, https://github.com/mraveri/tensiometer
 Project-URL: Tracker, https://github.com/mraveri/tensiometer/issues
 Project-URL: Reference, https://arxiv.org/abs/1806.04649
 Project-URL: Licensing, https://raw.githubusercontent.com/mraveri/tensiometer/master/LICENSE
-Description: ============
-        Tensiometer
-        ============
-        -------------------------------
-         Test a model until it breaks!
-        -------------------------------
-        :Tensiometer: utilities to understand concordance and discordance of posterior distributions
-        :Author: Marco Raveri and Cyrille Doux
-        :Homepage: https://tensiometer.readthedocs.io
-        :Source: https://github.com/mraveri/tensiometer
-        :References: https://arxiv.org/abs/2105.03324 (non-Gaussian metrics), https://arxiv.org/abs/1806.04649 and https://arxiv.org/abs/1912.04880 (Gaussian)
-        
-        .. image:: https://travis-ci.org/mraveri/tensiometer.svg?branch=master
-            :target: https://travis-ci.org/mraveri/tensiometer
-        .. image:: https://readthedocs.org/projects/tensiometer/badge/?version=latest
-           :target: https://tensiometer.readthedocs.org/en/latest
-        .. image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/mraveri/tensiometer/master?filepath=docs%2Fexample_notebooks%2Ftension_example.ipynb
-        .. image:: https://coveralls.io/repos/github/mraveri/tensiometer/badge.svg?branch=master
-           :target: https://coveralls.io/github/mraveri/tensiometer?branch=master
-        .. image:: https://img.shields.io/pypi/v/tensiometer.svg?style=flat
-           :target: https://pypi.python.org/pypi/tensiometer/
-        
-        Description
-        ============
-        
-        The tensiometer package is a collection of tools to test the level of
-        agreement/disagreement between different posterior distributions.
-        
-        The best way to get up to speed is to read through the worked example
-        `full worked example <https://tensiometer.readthedocs.org/en/latest/tension_example.html>`_
-        that you can `run online <https://mybinder.org/v2/gh/mraveri/tensiometer/master?filepath=docs%2Fexample_notebooks%2Ftension_example.ipynb>`_! There's also a documented example of
-        `non-Gaussian tension estimates between DES Y1 and Planck 18 <https://tensiometer.readthedocs.io/en/latest/non_gaussian_tension.html>`_.
-        
-        
-        Installation
-        =============
-        
-        The tensiometer package is available on PyPI and can be easily installed with::
-        
-          pip install tensiometer
-        
-        Alternatively one can download the source code from github::
-        
-          git clone https://github.com/mraveri/tensiometer.git
-        
-        and install it locally with the shortcut::
-        
-          make install
-        
-        You can test that the code is working properly by using::
-        
-          make test
-        
-        
-        Dependencies
-        
 Keywords: MCMC
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
+License-File: LICENSE
+
+============
+Tensiometer
+============
+-------------------------------
+ Test a model until it breaks!
+-------------------------------
+:Tensiometer: utilities to understand concordance and discordance of posterior distributions
+:Author: Marco Raveri and Cyrille Doux
+:Homepage: https://tensiometer.readthedocs.io
+:Source: https://github.com/mraveri/tensiometer
+:References: https://arxiv.org/abs/2105.03324 (non-Gaussian metrics), https://arxiv.org/abs/1806.04649 and https://arxiv.org/abs/1912.04880 (Gaussian)
+
+.. image:: https://travis-ci.org/mraveri/tensiometer.svg?branch=master
+    :target: https://travis-ci.org/mraveri/tensiometer
+.. image:: https://readthedocs.org/projects/tensiometer/badge/?version=latest
+   :target: https://tensiometer.readthedocs.org/en/latest
+.. image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/mraveri/tensiometer/master?filepath=docs%2Fexample_notebooks%2Ftension_example.ipynb
+.. image:: https://coveralls.io/repos/github/mraveri/tensiometer/badge.svg?branch=master
+   :target: https://coveralls.io/github/mraveri/tensiometer?branch=master
+.. image:: https://img.shields.io/pypi/v/tensiometer.svg?style=flat
+   :target: https://pypi.python.org/pypi/tensiometer/
+
+Description
+============
+
+The tensiometer package is a collection of tools to test the level of
+agreement/disagreement between different posterior distributions.
+
+The best way to get up to speed is to read through the worked example
+`full worked example <https://tensiometer.readthedocs.org/en/latest/tension_example.html>`_
+that you can `run online <https://mybinder.org/v2/gh/mraveri/tensiometer/master?filepath=docs%2Fexample_notebooks%2Ftension_example.ipynb>`_! There's also a documented example of
+`non-Gaussian tension estimates between DES Y1 and Planck 18 <https://tensiometer.readthedocs.io/en/latest/non_gaussian_tension.html>`_.
+
+
+Installation
+=============
+
+The tensiometer package is available on PyPI and can be easily installed with::
+
+  pip install tensiometer
+
+Alternatively one can download the source code from github::
+
+  git clone https://github.com/mraveri/tensiometer.git
+
+and install it locally with the shortcut::
+
+  make install
+
+You can test that the code is working properly by using::
+
+  make test
+
+
+Dependencies
```

### Comparing `tensiometer-0.1.1/tensiometer.egg-info/SOURCES.txt` & `tensiometer-0.1.2/tensiometer.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .material.py
+LICENSE
 MANIFEST.in
 README.rst
 setup.py
 tensiometer/__init__.py
 tensiometer/chains_convergence.py
 tensiometer/cosmosis_interface.py
 tensiometer/experimental.py
```

