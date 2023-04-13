# Comparing `tmp/keypoint-moseq-0.0.2.tar.gz` & `tmp/keypoint-moseq-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.0.2.tar", last modified: Fri Apr  7 22:26:29 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.0.3.tar", last modified: Thu Apr 13 22:33:32 2023, max compression
```

## Comparing `keypoint-moseq-0.0.2.tar` & `keypoint-moseq-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-07 22:26:29.017337 keypoint-moseq-0.0.2/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.2/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.2/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-07 22:26:29.017483 keypoint-moseq-0.0.2/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4694 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.2/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-07 22:26:29.015037 keypoint-moseq-0.0.2/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      633 2023-02-25 00:06:15.000000 keypoint-moseq-0.0.2/keypoint_moseq/__init__.py
--rw-rw-r--   0 calebweinreb   (501) staff       (20)    21235 2022-12-01 15:26:20.000000 keypoint-moseq-0.0.2/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17620 2023-02-10 16:07:10.000000 keypoint-moseq-0.0.2/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    16129 2023-03-11 00:23:09.000000 keypoint-moseq-0.0.2/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    32763 2023-04-07 22:25:29.000000 keypoint-moseq-0.0.2/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28233 2023-04-07 22:25:29.000000 keypoint-moseq-0.0.2/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    60436 2023-04-07 22:25:29.000000 keypoint-moseq-0.0.2/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-07 22:26:29.017011 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-07 22:26:28.000000 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      414 2023-04-07 22:26:28.000000 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-04-07 22:26:28.000000 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      124 2023-04-07 22:26:28.000000 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-04-07 22:26:28.000000 keypoint-moseq-0.0.2/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-04-07 22:26:29.018123 keypoint-moseq-0.0.2/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      807 2023-04-07 22:25:29.000000 keypoint-moseq-0.0.2/setup.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-13 22:33:32.435466 keypoint-moseq-0.0.3/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.3/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.3/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-13 22:33:32.435588 keypoint-moseq-0.0.3/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4694 2023-04-04 16:59:53.000000 keypoint-moseq-0.0.3/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-13 22:33:32.432396 keypoint-moseq-0.0.3/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      659 2023-04-13 16:52:36.000000 keypoint-moseq-0.0.3/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-04-13 16:52:36.000000 keypoint-moseq-0.0.3/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17686 2023-04-13 16:52:36.000000 keypoint-moseq-0.0.3/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    16272 2023-04-13 16:52:36.000000 keypoint-moseq-0.0.3/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    32764 2023-04-13 16:54:16.000000 keypoint-moseq-0.0.3/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    30075 2023-04-13 16:52:36.000000 keypoint-moseq-0.0.3/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    60436 2023-04-07 22:25:29.000000 keypoint-moseq-0.0.3/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-13 22:33:32.435139 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-13 22:33:32.000000 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      414 2023-04-13 22:33:32.000000 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-04-13 22:33:32.000000 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      124 2023-04-13 22:33:32.000000 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-04-13 22:33:32.000000 keypoint-moseq-0.0.3/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-04-13 22:33:32.436096 keypoint-moseq-0.0.3/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      807 2023-04-13 22:32:55.000000 keypoint-moseq-0.0.3/setup.py
```

### Comparing `keypoint-moseq-0.0.2/LICENSE.md` & `keypoint-moseq-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.2/NOTICE.md` & `keypoint-moseq-0.0.3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.2/README.md` & `keypoint-moseq-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.2/keypoint_moseq/__init__.py` & `keypoint-moseq-0.0.3/keypoint_moseq/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,13 +26,14 @@
 from .analysis import (
     compute_moseq_df, 
     compute_stats_df, 
     plotting_fingerprint,
     create_fingerprint_dataframe, 
     plot_syll_stats_with_sem,
     get_group_trans_mats,
+    changepoint_analysis,
 )
 
 from jax_moseq.models.keypoint_slds import (
     fit_pca, 
     init_model
 )
```

### Comparing `keypoint-moseq-0.0.2/keypoint_moseq/analysis.py` & `keypoint-moseq-0.0.3/keypoint_moseq/analysis.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.gridspec import GridSpec
 import matplotlib.lines as mlines
 from tqdm import tqdm
-
 import uuid
 from collections import defaultdict
 from sklearn.preprocessing import LabelEncoder, MinMaxScaler, StandardScaler
-
 from collections import defaultdict, OrderedDict
 from copy import deepcopy
 from cytoolz import sliding_window
-from keypoint_moseq.util import filter_angle
 import seaborn as sns
 
+# imports for changepoint analysis
+from statsmodels.stats.multitest import fdrcorrection
+from scipy.ndimage import gaussian_filter1d, convolve1d
+from scipy.signal import argrelextrema
+from keypoint_moseq.util import filter_angle, filtered_derivative, permute_cyclic
+from keypoint_moseq.io import format_data
+from jax_moseq.models.keypoint_slds import align_egocentric
+from jax_moseq.utils import unbatch
+na = np.newaxis
+
+
+
 def compute_moseq_df(results_dict, *, use_bodyparts, smooth_heading=True, **kwargs):
     session_name = []
     centroid = []
     velocity = []
     estimated_coordinates = []
     heading = []
     syllables = []
@@ -515,8 +524,166 @@
         trans_mats.append(get_transition_matrix(use_labels,
                                                 normalize=normalize,
                                                 combine=True,
                                                 max_syllable=max_sylls))
 
         # Getting frequency information for node scaling
         frequencies.append(get_syllable_statistics(use_labels, max_syllable=max_sylls)[0])
-    return trans_mats, frequencies
+    return trans_mats, frequencies
+
+def changepoint_analysis(coordinates, *, anterior_bodyparts, posterior_bodyparts, 
+                         bodyparts=None, use_bodyparts=None, alpha=0.1, 
+                         derivative_ksize=3, gaussian_ksize=1, num_thresholds=20,
+                         verbose=True, **kwargs):
+    """
+    Find changepoints in keypoint data. 
+    
+    Changepoints are peaks in a change score that is computed by:
+
+        1. Differentiating (egocentrically aligned) keypoint coordinates
+        2. Z-scoring the absolute values of each derivative
+        3. Counting the number keypoint-coordinate pairs where the 
+           Z-score crosses a threshold (in each frame).
+        4. Computing a p-value for the number of threshold-crossings
+           using a temporally shuffled null distribution
+        5. Smoothing the resulting significance score across time
+        
+    Steps (3-5) are performed for a range of threshold values, and 
+    the final outputs are based on the threshold that yields the 
+    highest changepoint frequency.
+
+    Parameters
+    ----------
+    coordinates : dict
+        Keypoint observations as a dictionary mapping session names to
+        ndarrays of shape (num_frames, num_keypoints, dim)
+
+    anterior_bodyparts : iterable of str or int
+        Anterior keypoints for egocentric alignment, either as indices
+        or as strings if ``bodyparts`` is provided.
+
+    posterior_bodyparts : iterable of str or int
+        Posterior keypoints for egocentric alignment, either as indices
+        or as strings if ``bodyparts`` is provided.
+
+    bodyparts : iterable of str, optional
+        Names of keypoints. Required for subsetting keypoints using
+        ``use_bodyparts`` or if ``anterior_bodyparts`` and
+        ``posterior_bodyparts`` are specified as strings.
+
+    use_bodyparts : iterable of str, optional
+        Subset of keypoints to use for changepoint analysis. If not
+        provided, all keypoints are used.
+
+    alpha : float, default=0.1
+        False-discovery rate for statistical significance testing. Only
+         changepoints with ``p < alpha`` are considered significant.
+
+    derivative_ksize : int, default=3
+        Size of the kernel used to differentiate keypoint coordinates. 
+        For example if ``derivative_ksize=3``, the derivative would be
+
+        .. math::
+
+            \dot{y_t} = \frac{1}{3}( x_{t+3}+x_{t+2}+x_{t+1}-x_{t-1}-x_{t-2}-x_{t-3})
+
+    gaussian_ksize : int, default=1
+        Size of the kernel used to smooth the change score. 
+        
+    num_thresholds : int, default=20
+        Number of thresholds to test.
+        
+    verbose : bool, default=True
+        Print progress messages.
+
+    Returns
+    -------
+    changepoints : dict
+        Changepoints as a dictionary with the same keys as ``coordinates``.
+
+    changescores : dict
+        Change scores as a dictionary with the same keys as ``coordinates``.
+
+    coordinates_ego: dict
+        Keypoints in egocentric coordinates, in the same format as 
+        ``coordinates``.
+
+    derivatives : dict
+        Z-scored absolute values of the derivatives for each egocentic 
+        keypoint coordinate, in the same format as ``coordinates``
+
+    threshold: float
+        Threshold used to binarize Z-scored derivatives. 
+    """
+    if use_bodyparts is None and bodyparts is not None:
+        use_bodyparts = bodyparts
+    
+    if isinstance(anterior_bodyparts[0], str):
+        assert use_bodyparts is not None, fill(
+            "Must provide `bodyparts` or `use_bodyparts` if `anterior_bodyparts` is a list of strings")
+        anterior_idxs = [use_bodyparts.index(bp) for bp in anterior_bodyparts]
+    else: anterior_idxs = anterior_bodyparts
+
+    if isinstance(posterior_bodyparts[0], str):
+        assert use_bodyparts is not None, fill(
+            "Must provide `bodyparts` or `use_bodyparts` if `posterior_bodyparts` is a list of strings")
+        posterior_idxs = [use_bodyparts.index(bp) for bp in posterior_bodyparts]
+    else: posterior_idxs = posterior_bodyparts
+    
+    # Differentiating (egocentrically aligned) keypoint coordinates
+    if verbose: print('Aligning keypoints')
+    data, labels = format_data(coordinates, bodyparts=bodyparts, use_bodyparts=use_bodyparts)
+    Y_ego,_,_ = align_egocentric(data['Y'], anterior_idxs, posterior_idxs)
+    Y_flat = np.array(Y_ego).reshape(*Y_ego.shape[:2], -1)
+    
+    if verbose: print('Differentiating and z-scoring')
+    dy = np.abs(filtered_derivative(Y_flat, derivative_ksize, axis=1))
+    mask = np.broadcast_to(np.array(data['mask'])[:,:,na], dy.shape)>0
+    means = (dy * mask).sum(1) / mask.sum(1)
+    dy_centered = dy - means[:,na,:]
+    stds = np.sqrt((dy_centered**2 * mask).sum(1) / mask.sum(1))
+    dy_zscored = dy_centered / (stds[:,na,:]+1e-8)
+
+    # Count threshold crossings
+    thresholds = np.linspace(
+        np.percentile(dy_zscored,1), 
+        np.percentile(dy_zscored,99), 
+        num_thresholds)
+    
+    def get_changepoints(score, pvals, alpha):
+        pts = argrelextrema(score, np.greater, order=1)[0]
+        return pts[pvals[pts] < alpha]
+    
+    # get changescores for each threshold
+    all_changescores, all_changepoints = [],[]
+    for threshold in tqdm(thresholds, disable=(not verbose), desc='Testing thresholds'):
+
+        # permute within-session then combine across sessions
+        crossings = (dy_zscored > threshold).sum(2)[mask[:,:,0]]
+        crossings_shuff = permute_cyclic(dy_zscored > threshold, mask, axis=1).sum(2)[mask[:,:,0]]
+        crossings_shuff = crossings_shuff + np.random.uniform(-.1,.1,crossings_shuff.shape)
+
+        # get significance score
+        ps_combined = 1-(np.sort(crossings_shuff).searchsorted(crossings)-1)/len(crossings)
+        ps_combined = fdrcorrection(ps_combined, alpha=alpha)[1]
+
+        # separate back into sessions
+        pvals = np.zeros(mask[:,:,0].shape)
+        pvals[mask[:,:,0]] = ps_combined
+        pvals = unbatch(pvals, labels)
+
+        changescores = {k:gaussian_filter1d(-np.log10(ps),gaussian_ksize) for k,ps in pvals.items()}
+        changepoints = {k:get_changepoints(changescores[k],ps,alpha) for k,ps in pvals.items()}
+        all_changescores.append(changescores)
+        all_changepoints.append(changepoints)
+        
+    # pick threshold with most changepoints 
+    num_changepoints = [sum(map(len,d.values())) for d in all_changepoints]
+    changescores = all_changescores[np.argmax(num_changepoints)]
+    changepoints = all_changepoints[np.argmax(num_changepoints)]
+    threshold = thresholds[np.argmax(num_changepoints)]
+
+    coordinates_ego = unbatch(np.array(Y_ego), labels)
+    derivatives = unbatch(dy_zscored.reshape(Y_ego.shape), labels)
+    return changepoints, changescores, coordinates_ego, derivatives, threshold
+
+
```

### Comparing `keypoint-moseq-0.0.2/keypoint_moseq/calibration.py` & `keypoint-moseq-0.0.3/keypoint_moseq/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,17 +170,18 @@
                   intercept=float(estimator.intercept))
 
 
 def _confs_and_dists_from_annotations(coordinates, confidences, 
                                       annotations, bodyparts):
     confs,dists = [],[]
     for (key,frame,bodypart),xy in annotations.items():
-        k = bodyparts.index(bodypart)
-        confs.append(confidences[key][frame][k])
-        dists.append(np.sqrt(((coordinates[key][frame][k]-np.array(xy))**2).sum()))
+        if key in coordinates and key in confidences:
+            k = bodyparts.index(bodypart)
+            confs.append(confidences[key][frame][k])
+            dists.append(np.sqrt(((coordinates[key][frame][k]-np.array(xy))**2).sum()))
     return confs,dists
 
 
 def _noise_calibration_widget(project_dir, coordinates, confidences,
                               sample_keys, sample_images, annotations, *, 
                               keypoint_colormap, bodyparts, skeleton, 
                               error_estimator, conf_threshold, **kwargs):
```

### Comparing `keypoint-moseq-0.0.2/keypoint_moseq/fitting.py` & `keypoint-moseq-0.0.3/keypoint_moseq/fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
                           savefig=save_progress_figs, project_dir=project_dir)
 
         if save_every_n_iters>0 and (iteration%save_every_n_iters)==0:
             save_checkpoint(model, data, history, labels, iteration, name=name,
                             project_dir=project_dir,save_history=save_history, 
                             save_states=save_states, save_data=save_data)
             
-        try: model = resample_model(data, **model, ar_only=ar_only)
+        try: model = resample_model(data, **model, ar_only=ar_only, verbose=verbose)
         except KeyboardInterrupt: break
     
     return model, history, name
     
     
 def resume_fitting(*, params, hypparams, labels, iteration, mask,
                    Y, conf, seed, noise_prior=None, states=None, **kwargs):
@@ -182,15 +182,15 @@
                        noise_prior, seed, **kwargs)
 
     return fit_model(model, data, labels, start_iter=iteration+1, **kwargs)
 
 
 def apply_model(*, params, coordinates, confidences=None, num_iters=5, 
                 use_saved_states=True, states=None, mask=None, labels=None, 
-                noise_prior=None, ar_only=False, save_results=True, 
+                noise_prior=None, ar_only=False, save_results=True, verbose=False,
                 project_dir=None, name=None, results_path=None, **kwargs): 
     """
     Apply a model to data.
 
     There are two scenarios for applying this function:
         - The model is being applied to the same data it was fit to.
             This would useful if the the data was chunked into segments
@@ -252,14 +252,17 @@
 
     ar_only : bool, default=False
         See :py:func:`keypoint_moseq.fitting.fit_model`.
 
     save_results : bool, default=True
         If True, the model outputs will be saved to disk.
 
+    verbose : bool, default=False
+        Whether to print progress updates.
+
     project_dir : str, default=None
         Path to the project directory. Required if ``save_results=True``
         and ``results_path=None``.
 
     name : str, default=None
         Name of the model. Required if ``save_results=True``
         and ``results_path=None``.
@@ -304,19 +307,19 @@
             new_states[k] = v[:,padding:]
         states = new_states
         
     else: 
         states = None
         noise_prior = None
     
-    model = init_model(data, states, params, noise_prior=noise_prior, **kwargs)
+    model = init_model(data, states, params, noise_prior=noise_prior, verbose=verbose, **kwargs)
     
     if num_iters>0:
         for iteration in tqdm.trange(num_iters, desc='Applying model'):
-            model = resample_model(data, **model, ar_only=ar_only, states_only=True)
+            model = resample_model(data, **model, ar_only=ar_only, states_only=True, verbose=verbose)
 
     nlags = model['hypparams']['ar_hypparams']['nlags']
     states = jax.device_get(model['states'])                     
     estimated_coords = jax.device_get(estimate_coordinates(
         **model['states'], **model['params'], **data))
     z_reindexed = reindex_by_frequency(states['z'], np.array(data['mask']))
```

### Comparing `keypoint-moseq-0.0.2/keypoint_moseq/io.py` & `keypoint-moseq-0.0.3/keypoint_moseq/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import warnings
 import h5py
 import joblib
 import tqdm
 import yaml
 import os
 import cv2
-import tqdm
 import re
 import pandas as pd
 from datetime import datetime
 from textwrap import fill
 from vidio.read import OpenCVReader
 warnings.formatwarning = lambda msg, *a: str(msg)
 
@@ -67,15 +66,15 @@
         'use_bodyparts': ['BODYPART1','BODYPART2','BODYPART3'],
         'skeleton': [['BODYPART1','BODYPART2'], ['BODYPART2','BODYPART3']],
         'anterior_bodyparts': ['BODYPART1'],
         'posterior_bodyparts': ['BODYPART3']})
         
     other = _update_dict(kwargs, {
         'session_name_suffix': '',
-        'verbose':True,
+        'verbose':False,
         'conf_pseudocount': 1e-3,
         'video_dir': '',
         'keypoint_colormap': 'autumn',
         'whiten': True,
         'fix_heading': False,
         'seg_length': 10000 })
        
@@ -233,23 +232,23 @@
     To update model hyperparameters, just use the name of the 
     hyperparameter as the keyword argument. 
 
     Examples
     --------
     To update ``video_dir`` to ``/path/to/videos``::
 
-    >>> update_config(project_dir, video_dir='/path/to/videos')
-    >>> print(load_config(project_dir)['video_dir'])
-    /path/to/videos
+      >>> update_config(project_dir, video_dir='/path/to/videos')
+      >>> print(load_config(project_dir)['video_dir'])
+      /path/to/videos
 
     To update ``trans_hypparams['kappa']`` to ``100``::
 
-    >>> update_config(project_dir, kappa=100)
-    >>> print(load_config(project_dir)['trans_hypparams']['kappa'])
-    100
+      >>> update_config(project_dir, kappa=100)
+      >>> print(load_config(project_dir)['trans_hypparams']['kappa'])
+      100
     """
     config = load_config(project_dir, check_if_valid=False, build_indexes=False)
     config.update(kwargs)
     generate_config(project_dir, **config)
     
         
 def setup_project(project_dir, deeplabcut_config=None, sleap_file=None,
```

### Comparing `keypoint-moseq-0.0.2/keypoint_moseq/util.py` & `keypoint-moseq-0.0.3/keypoint_moseq/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import glob
 import tqdm
 from textwrap import fill
 import jax, jax.numpy as jnp, jax.random as jr
 from jax.tree_util import tree_map
 from itertools import groupby
 from functools import partial
-from scipy.ndimage import median_filter
+from scipy.ndimage import median_filter, convolve1d
 from sklearn.decomposition import PCA
 from sklearn.neighbors import NearestNeighbors
 from jaxlib.xla_extension import DeviceArray as jax_array
 from jax_moseq.models.keypoint_slds import inverse_rigid_transform
 na = jnp.newaxis
 
 
@@ -643,15 +643,14 @@
             c = np.array([centroids[key][s] for key,s,e in syllable_instances])[:,None]
             h = np.array([headings[key][s] for key,s,e in syllable_instances])[:,None]
             trajectories = np_io(inverse_rigid_transform)(trajectories,c,h)
 
     return trajectories
 
 
-
 def sample_instances(syllable_instances, num_samples, mode='random', 
                      pca_samples=50000, pca_dim=4, n_neighbors=50,
                      coordinates=None, pre=5, post=15, centroids=None, 
                      headings=None, filter_size=9):
     """
     Sample a fixed number of instances for each syllable.
 
@@ -664,18 +663,18 @@
     num_samples: int
         Number of samples return for each syllable
 
     mode: str, {'random', 'density'}, default='random'
         Sampling method to use. Options are:
         
         - 'random': Instances are chosen randomly (without replacement)
-        - 'density': For each syllable, a syllable-specific density function is
-          computed in trajectory space and compared to the overall
-          density across all syllables. An exemplar instance that 
-          maximizes this ratio is chosen for each syllable, and
+        - 'density': For each syllable, a syllable-specific density 
+          function is computed in trajectory space and compared to the 
+          overall density across all syllables. An exemplar instance
+          that maximizes this ratio is chosen for each syllable, and
           its nearest neighbors are randomly sampled. 
 
     pca_samples: int, default=50000
         Number of trajectories to sample when fitting a PCA model for 
         density estimation (used when ``mode='density'``)
 
     pca_dim: int, default=4
@@ -689,16 +688,16 @@
 
     coordinates, pre, pos, centroids, heading, filter_size
         Passed to :py:func:`keypoint_moseq.util.get_trajectories`
 
     Returns
     -------
     sampled_instances: dict
-        Dictionary in the same format as ``syllable_instances`` mapping
-        each syllable to a list of sampled instances.
+        Dictionary in the same format as ``syllable_instances`` 
+        mapping each syllable to a list of sampled instances.
     """
     assert mode in ['random','density']
     assert all([len(v)>=num_samples for v in syllable_instances.values()])
     assert n_neighbors>=num_samples
 
     if mode=='random':
         sampled_instances = {syllable: [instances[i] for i in np.random.choice(
@@ -802,7 +801,81 @@
     interpolated_coordinates = np.zeros_like(coordinates)
     for i in range(coordinates.shape[1]):
         interpolated_coordinates[:,i,:] = interpolate_along_axis(
             np.arange(coordinates.shape[0]),
             np.nonzero(~outliers[:,i])[0],
             coordinates[~outliers[:,i],i,:])
     return interpolated_coordinates
+
+
+
+def filtered_derivative(Y_flat, ksize, axis=0):
+    """
+    Compute the filtered derivative of a signal along a given axis.
+
+    When ``ksize=3``, for example, the filtered derivative is
+
+    .. math::
+
+        \dot{y_t} = \frac{1}{3}( x_{t+3}+x_{t+2}+x_{t+1}-x_{t-1}-x_{t-2}-x_{t-3})
+
+    Parameters
+    ----------
+    Y_flat: ndarray
+        The signal to differentiate
+
+    ksize: int
+        The size of the filter. Must be odd.
+
+    axis: int, default=0
+        The axis along which to differentiate
+
+    Returns
+    -------
+    dY: ndarray
+        The filtered derivative of the signal
+    """
+    kernel = np.ones(ksize+1)/(ksize+1)
+    pre = convolve1d(Y_flat, kernel, origin=-(ksize+1)//2, axis=axis)
+    post = convolve1d(Y_flat, kernel, origin=ksize//2, axis=axis)
+    return post-pre
+
+
+def permute_cyclic(arr, mask=None, axis=0):
+    """
+    Cyclically permute an array along a given axis.
+
+    Parameters
+    ----------
+    arr: ndarray
+        The array to permute
+
+    mask: ndarray, optional
+        A boolean mask indicating which elements to permute. If None,
+        all elements are permuted.
+
+    axis: int, default=0
+        The axis along which to permute
+
+    Returns
+    -------
+    arr_permuted: ndarray
+        The permuted array
+    """
+    if mask is None: 
+        mask = np.ones_like(arr)
+
+    arr = np.moveaxis(arr, axis, 0)
+    mask = np.moveaxis(mask, axis, 0)
+    
+    shape = arr.shape
+    arr = arr.reshape(arr.shape[0],-1)
+    mask = mask.reshape(mask.shape[0],-1)
+
+    arr_permuted = np.zeros_like(arr)
+    for i in range(arr.shape[1]):
+        arr_permuted[mask[:,i]>0,i] = np.roll(
+            arr[mask[:,i]>0,i], np.random.randint(0,mask[:,i].sum()))
+        
+    arr_permuted = arr_permuted.reshape(shape)
+    arr_permuted = np.moveaxis(arr_permuted, 0, axis)
+    return arr_permuted
```

### Comparing `keypoint-moseq-0.0.2/keypoint_moseq/viz.py` & `keypoint-moseq-0.0.3/keypoint_moseq/viz.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.2/setup.py` & `keypoint-moseq-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='keypoint-moseq',
-    version='0.0.2',
+    version='0.0.3',
     author='Caleb Weinreb',
     author_email='calebsw@gmail.com',
     include_package_data=True,
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent'
```

