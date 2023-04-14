# Comparing `tmp/visualime-0.0.5.tar.gz` & `tmp/visualime-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualime-0.0.5.tar", last modified: Sun Jan  1 15:09:25 2023, max compression
+gzip compressed data, was "visualime-0.0.6.tar", last modified: Fri Apr 14 08:34:30 2023, max compression
```

## Comparing `visualime-0.0.5.tar` & `visualime-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:09:25.107846 visualime-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-01-01 15:09:15.000000 visualime-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-01 15:09:15.000000 visualime-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-01-01 15:09:25.107846 visualime-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-01-01 15:09:15.000000 visualime-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-01 15:09:15.000000 visualime-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-01 15:09:15.000000 visualime-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-01 15:09:25.107846 visualime-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:09:25.107846 visualime-0.0.5/visualime/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-01 15:09:15.000000 visualime-0.0.5/visualime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-01-01 15:09:15.000000 visualime-0.0.5/visualime/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-01-01 15:09:15.000000 visualime-0.0.5/visualime/baylime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-01-01 15:09:15.000000 visualime-0.0.5/visualime/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-01-01 15:09:15.000000 visualime-0.0.5/visualime/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-01-01 15:09:15.000000 visualime-0.0.5/visualime/lime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-01-01 15:09:15.000000 visualime-0.0.5/visualime/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-01-01 15:09:15.000000 visualime-0.0.5/visualime/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:09:25.107846 visualime-0.0.5/visualime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-01-01 15:09:25.000000 visualime-0.0.5/visualime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-01-01 15:09:25.000000 visualime-0.0.5/visualime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-01 15:09:25.000000 visualime-0.0.5/visualime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-01 15:09:25.000000 visualime-0.0.5/visualime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-01 15:09:25.000000 visualime-0.0.5/visualime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:34:30.235718 visualime-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-14 08:34:15.000000 visualime-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 08:34:15.000000 visualime-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-14 08:34:30.235718 visualime-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-04-14 08:34:15.000000 visualime-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-14 08:34:15.000000 visualime-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 08:34:15.000000 visualime-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:34:30.235718 visualime-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:34:30.231717 visualime-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-14 08:34:15.000000 visualime-0.0.6/tests/test_baylime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-14 08:34:15.000000 visualime-0.0.6/tests/test_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-14 08:34:15.000000 visualime-0.0.6/tests/test_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-14 08:34:15.000000 visualime-0.0.6/tests/test_lime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-14 08:34:15.000000 visualime-0.0.6/tests/test_visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:34:30.231717 visualime-0.0.6/visualime/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/baylime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/lime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14849 2023-04-14 08:34:15.000000 visualime-0.0.6/visualime/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:34:30.235718 visualime-0.0.6/visualime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-14 08:34:30.000000 visualime-0.0.6/visualime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-14 08:34:30.000000 visualime-0.0.6/visualime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:34:30.000000 visualime-0.0.6/visualime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 08:34:30.000000 visualime-0.0.6/visualime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 08:34:30.000000 visualime-0.0.6/visualime.egg-info/top_level.txt
```

### Comparing `visualime-0.0.5/LICENSE` & `visualime-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `visualime-0.0.5/PKG-INFO` & `visualime-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualime
-Version: 0.0.5
+Version: 0.0.6
 Summary: Implementation of LIME focused on producing user-centric local explanations for image classifiers.
 Author-email: Kilian Kluge <dev@kluge.ai>, The VisuaLIME developers <xai.demonstrator@gmail.com>
 License: Apache 2.0 License
 Project-URL: Documentation, https://visualime.readthedocs.io/
 Project-URL: Repository, https://github.com/xai-demonstrator/visualime
 Project-URL: Bug Tracker, https://github.com/xai-demonstrator/visualime/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `visualime-0.0.5/README.md` & `visualime-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `visualime-0.0.5/pyproject.toml` & `visualime-0.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -27,7 +27,23 @@
 
 [tool.setuptools]
 packages = ["visualime"]
 
 [tool.setuptools.dynamic]
 version = { attr = "visualime.__version__" }
 dependencies = { file = "requirements.txt" }
+
+[tool.mypy]
+python_version = "3.10"
+warn_return_any = false
+plugins = ["numpy.typing.mypy_plugin"]
+
+[[tool.mypy.overrides]]
+module = [
+    "sklearn",
+    "sklearn.*",
+    "skimage",
+    "skimage.*",
+    "PIL",
+    "PIL.*"
+]
+ignore_missing_imports = true
```

### Comparing `visualime-0.0.5/visualime/_models.py` & `visualime-0.0.6/visualime/_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,23 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Literal, Optional
 
 from sklearn.linear_model import BayesianRidge, Lasso, LinearRegression, Ridge
 
 from .baylime import BayesianRidgeFixedAlphaLambda, BayesianRidgeFixedLambda
 
-LINEAR_MODELS = {
+LINEAR_MODEL_TYPES = Literal[
+    "linear_regression",
+    "lasso",
+    "ridge",
+    "bayesian_ridge",
+    "bayesian_ridge_fixed_lambda",
+    "bayesian_ridge_fixed_alpha_lambda",
+]
+
+LINEAR_MODELS: Dict[LINEAR_MODEL_TYPES, Any] = {
     "linear_regression": LinearRegression,
     "lasso": Lasso,
     "ridge": Ridge,
     "bayesian_ridge": BayesianRidge,
     "bayesian_ridge_fixed_lambda": BayesianRidgeFixedLambda,
     "bayesian_ridge_fixed_alpha_lambda": BayesianRidgeFixedAlphaLambda,
 }
@@ -26,15 +35,17 @@
         Parameters to pass to the model during instantiation.
 
         See the `scikit-learn documentation
         <https://scikit-learn.org/stable/modules/classes.html#module-sklearn.linear_model>`_
         for details on each of the models."""
 
 
-def instantiate_model(model_type: str, model_params: Optional[Dict[str, Any]] = None):
+def instantiate_model(
+    model_type: LINEAR_MODEL_TYPES, model_params: Optional[Dict[str, Any]] = None
+):
     model_params = model_params or {}
 
     try:
         return LINEAR_MODELS[model_type](**model_params)
     except KeyError:
         raise ValueError(
             f"Unknown model_type '{model_type}'. Available options: {', '.join(list(LINEAR_MODELS.keys()))}."
```

### Comparing `visualime-0.0.5/visualime/baylime.py` & `visualime-0.0.6/visualime/baylime.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     A warning will be issued if this amount is exceeded.
     To reduce the amount of change in lambda, increase `large_number`.
 
     See the documentation for :meth:`sklearn.linear_model.BayesianRidge` for a list
     of available parameters.
     """
 
-    def __init__(self, *, epsilon: float = 1e-6, large_number: int = 1e9, **kwargs):
+    def __init__(self, *, epsilon: float = 1e-6, large_number: float = 1e9, **kwargs):
         if "lambda_init" not in kwargs:
             raise ValueError("'lambda_init' must be set.")
 
         super().__init__(**kwargs)
 
         self.epsilon = epsilon
         self.large_number = large_number
@@ -60,15 +60,15 @@
     A warning will be issued if this amount is exceeded.
     To reduce the amount of change, increase `large_number`.
 
     See the documentation for :meth:`sklearn.linear_model.BayesianRidge` for a list
     of available parameters.
     """
 
-    def __init__(self, *, epsilon: float = 1e-6, large_number: int = 1e9, **kwargs):
+    def __init__(self, *, epsilon: float = 1e-6, large_number: float = 1e9, **kwargs):
         if "alpha_init" not in kwargs:
             raise ValueError("'alpha_init' must be set.")
         if "lambda_init" not in kwargs:
             raise ValueError("'lambda_init' must be set.")
 
         super().__init__(**kwargs)
```

### Comparing `visualime-0.0.5/visualime/explain.py` & `visualime-0.0.6/visualime/explain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 import numpy as np
 from PIL import Image
 from PIL.Image import Image as PIL_Image
 
+from ._models import LINEAR_MODEL_TYPES
 from .feature_selection import forward_selection, select_by_weight
+from .lime import SEGMENTATION_METHOD_TYPES  # noqa
 from .lime import (
     compute_distances,
     create_segments,
     generate_images,
     generate_samples,
     predict_images,
     weigh_segments,
@@ -16,15 +18,15 @@
 from .visualize import generate_overlay, scale_opacity, select_segments
 
 
 def explain_classification(
     image: np.ndarray,
     predict_fn: Callable[[np.ndarray], np.ndarray],
     label_idx: Optional[int] = None,
-    segmentation_method: str = "slic",
+    segmentation_method: SEGMENTATION_METHOD_TYPES = "slic",
     segmentation_settings: Optional[Dict[str, Any]] = None,
     num_of_samples: int = 64,
     p: float = 0.33,
     segment_selection_method: str = "by_weight",
     num_segments_to_select: Optional[int] = 0,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Explain why the classifier called through `predict_fn` classifies the `image` into
@@ -78,15 +80,15 @@
     segment_weights : np.ndarray
         A one-dimensional array whose length is equal to the number of segments.
 
     Examples
     --------
     TODO: Add end-to-end example
     """
-    model_type = "bayesian_ridge"
+    model_type: LINEAR_MODEL_TYPES = "bayesian_ridge"
 
     if label_idx is None:
         label_idx = int(np.argmax(predict_fn(image[None, :, :, :])))
 
     segment_mask = create_segments(
         image=image,
         segmentation_method=segmentation_method,
@@ -199,14 +201,15 @@
         )
 
         positive_overlay = scale_opacity(
             overlay=positive_overlay,
             segment_weights=segment_weights,
             segment_mask=segment_mask,
             segments_to_color=positive_segments,
+            max_opacity=opacity,
         )
 
         overlay_image = Image.fromarray(positive_overlay.astype(np.uint8), "RGBA")
         final_img.alpha_composite(overlay_image)
 
     if negative is not None:
         negative_segments = select_segments(
@@ -217,13 +220,14 @@
         )
 
         negative_overlay = scale_opacity(
             overlay=negative_overlay,
             segment_weights=segment_weights,
             segment_mask=segment_mask,
             segments_to_color=negative_segments,
+            max_opacity=opacity,
         )
 
         overlay_image = Image.fromarray(negative_overlay.astype(np.uint8), "RGBA")
         final_img.alpha_composite(overlay_image)
 
     return final_img
```

### Comparing `visualime-0.0.5/visualime/feature_selection.py` & `visualime-0.0.6/visualime/feature_selection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np
 from sklearn.feature_selection import SelectFromModel
 from sklearn.linear_model import lars_path
 
-from ._models import MODEL_TYPE_PARAMS_DOC, instantiate_model
+from ._models import LINEAR_MODEL_TYPES, MODEL_TYPE_PARAMS_DOC, instantiate_model
 from .lime import SAMPLES_PREDICTIONS_LABEL_IDX_DOC
 from .metrics import DISTANCES_KERNEL_DOC, cosine_distance, exponential_kernel
 
 
-def _get_num_segments(samples: np.ndarray, num_segments_to_select: Optional[int]):
+def _get_num_segments(
+    samples: np.ndarray, num_segments_to_select: Optional[int]
+) -> Tuple[int, int]:
     num_segments = samples.shape[1]
     num_segments_to_select = num_segments_to_select or num_segments
     if num_segments_to_select > num_segments:
         raise ValueError(
             f"Number of features to select ({num_segments_to_select}) cannot exceed "
             f"number of features in data ({num_segments})"
         )
     return num_segments, num_segments_to_select
 
 
 def select_by_weight(
     samples: np.ndarray,
     predictions: np.ndarray,
     label_idx: int,
-    model_type: str = "bayesian_ridge",
+    model_type: LINEAR_MODEL_TYPES = "bayesian_ridge",
     model_params: Optional[Dict[str, Any]] = None,
     distances: Optional[np.ndarray] = None,
     kernel: Callable[[np.ndarray], np.ndarray] = exponential_kernel,
     num_segments_to_select: Optional[int] = None,
 ) -> List[int]:
     num_segments, num_segments_to_select = _get_num_segments(
         samples, num_segments_to_select
@@ -72,15 +74,15 @@
 """
 
 
 def forward_selection(
     samples: np.ndarray,
     predictions: np.ndarray,
     label_idx: int,
-    model_type: str = "ridge",
+    model_type: LINEAR_MODEL_TYPES = "ridge",
     model_params: Optional[Dict[str, Any]] = None,
     distances: Optional[np.ndarray] = None,
     kernel: Callable[[np.ndarray], np.ndarray] = exponential_kernel,
     num_segments_to_select: Optional[int] = None,
 ) -> List[int]:
     num_segments, num_segments_to_select = _get_num_segments(
         samples, num_segments_to_select
@@ -90,28 +92,30 @@
         distances = cosine_distance(samples)
     sample_weight = kernel(distances)
 
     # TODO: Understand and account for the implications of regularization
     linear_model = instantiate_model(model_type=model_type, model_params=model_params)
 
     # TODO: Wait for https://github.com/scikit-learn/scikit-learn/issues/25236
-    def score(current_features: List[int], next_feature_idx: int):
+    def score(current_features: List[int], next_feature_idx: int) -> float:
         linear_model.fit(
             samples[:, current_features + [next_feature_idx]],
             predictions[:, label_idx],
             sample_weight=sample_weight,
         )
 
-        return linear_model.score(
-            samples[:, current_features + [next_feature_idx]],
-            predictions[:, label_idx],
-            sample_weight=sample_weight,
+        return float(
+            linear_model.score(
+                samples[:, current_features + [next_feature_idx]],
+                predictions[:, label_idx],
+                sample_weight=sample_weight,
+            )
         )
 
-    selected_segments = []
+    selected_segments: List[int] = []
     for _ in range(num_segments_to_select):
         selectable_segments = set(range(num_segments)) - set(selected_segments)
         scores = (
             (score(selected_segments, segment_idx), segment_idx)
             for segment_idx in selectable_segments
         )
         segment_with_highest_score = max(scores, key=lambda x: x[0])[1]
```

### Comparing `visualime-0.0.5/visualime/lime.py` & `visualime-0.0.6/visualime/lime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 from skimage.color import rgb2gray
 from skimage.filters import sobel
 from skimage.segmentation import felzenszwalb, quickshift, slic, watershed
 
 __all__ = [
@@ -10,15 +10,19 @@
     "generate_images",
     "generate_samples",
     "compute_distances",
     "predict_images",
     "weigh_segments",
 ]
 
-from visualime._models import MODEL_TYPE_PARAMS_DOC, instantiate_model
+from visualime._models import (
+    LINEAR_MODEL_TYPES,
+    MODEL_TYPE_PARAMS_DOC,
+    instantiate_model,
+)
 from visualime.metrics import DISTANCES_KERNEL_DOC, cosine_distance, exponential_kernel
 
 SAMPLES_PREDICTIONS_LABEL_IDX_DOC = """samples : np.ndarray
         The samples generated by :meth:`visualime.lime.generate_samples`:
         An array of shape `(num_of_samples, num_of_segments)`.
 
     predictions : np.ndarray
@@ -31,15 +35,19 @@
 
 
 def _watershed(image: np.ndarray, **kwargs):
     gradient = sobel(rgb2gray(image))
     return watershed(image=gradient, **kwargs)
 
 
-SEGMENTATION_METHODS = {
+SEGMENTATION_METHOD_TYPES = Literal["felzenszwalb", "slic", "quickshift", "watershed"]
+
+SEGMENTATION_METHODS: Dict[
+    SEGMENTATION_METHOD_TYPES, Tuple[Callable, Dict[str, Any]]
+] = {
     "felzenszwalb": (felzenszwalb, {"scale": 250, "sigma": 0.6, "min_size": 45}),
     "slic": (
         slic,
         {
             "n_segments": 250,
             "compactness": 2,
             "convert2lab": True,
@@ -50,15 +58,15 @@
     "quickshift": (quickshift, {"kernel_size": 5, "max_dist": 6, "ratio": 0.7}),
     "watershed": (_watershed, {"markers": 250, "compactness": 0.001}),
 }
 
 
 def create_segments(
     image: np.ndarray,
-    segmentation_method: str,
+    segmentation_method: SEGMENTATION_METHOD_TYPES,
     segmentation_settings: Optional[Dict[str, Any]] = None,
 ) -> np.ndarray:
     """Divide the image into segments (superpixels).
 
     Proper segmentation of the images is key to producing meaningful explanations with LIME.
     Which method and settings are appropriate is highly use-case specific.
 
@@ -216,15 +224,15 @@
     """
     return predict_fn(images)
 
 
 def compute_distances(
     image: np.ndarray,
     images: np.ndarray,
-    norm: Optional[Union[str, int]] = None,
+    norm: Optional[Union[Literal["fro", "nuc"], int]] = None,
     select: str = "sum",
 ) -> np.ndarray:
     """Calculate the distances between the original `image` and the generated `images`.
 
     Parameters
     ----------
     image : np.ndarray
@@ -271,15 +279,15 @@
         raise ValueError(f"Invalid value '{select}' for parameter 'select'.")
 
 
 def weigh_segments(
     samples: np.ndarray,
     predictions: np.ndarray,
     label_idx: int,
-    model_type: str = "bayesian_ridge",
+    model_type: LINEAR_MODEL_TYPES = "bayesian_ridge",
     model_params: Optional[Dict[str, Any]] = None,
     distances: Optional[np.ndarray] = None,
     kernel: Callable[[np.ndarray], np.ndarray] = exponential_kernel,
     segment_subset: Optional[List[int]] = None,
 ) -> np.ndarray:
     linear_model = instantiate_model(model_type=model_type, model_params=model_params)
```

### Comparing `visualime-0.0.5/visualime/metrics.py` & `visualime-0.0.6/visualime/metrics.py`

 * *Files identical despite different names*

### Comparing `visualime-0.0.5/visualime/visualize.py` & `visualime-0.0.6/visualime/visualize.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import List, Optional, Tuple, Union
+from typing import List, Literal, Optional, Tuple, Union
 
 import numpy as np
 from PIL.ImageColor import getrgb
 
 
 def select_segments(
     segment_weights: np.ndarray,
@@ -110,15 +110,15 @@
 
     ordered_segments = np.argsort(-segment_weights)
 
     if coverage is not None:
         coverage = min(coverage, max_coverage, 1.0)
         coverage = max(coverage, min_coverage, 0.0)
 
-        for i in range(max_segment_idx - 1):
+        for i in range(max_segment_idx):
             _selected_segments = ordered_segments[: i + 1]
             if np.isin(segment_mask, _selected_segments).sum() / _area >= coverage:
                 num_of_segments = i + 1
                 break
         else:
             warnings.warn(
                 f"Need to select all {max_num_of_segments} segments to reach desired "
@@ -229,15 +229,15 @@
 
 
 def scale_opacity(
     overlay: np.ndarray,
     segment_mask: np.ndarray,
     segment_weights: np.ndarray,
     segments_to_color: Union[np.ndarray, List[int]],
-    relative_to: Union[str, float] = "max",
+    relative_to: Union[Literal["max"], float] = "max",
     exponent: float = 1.0,
     max_opacity: float = 1.0,
 ) -> np.ndarray:
     """Set the opacity of each segment according to its weight.
 
     Segments with a higher (absolute) weight will be more opaque than segments with a lower weight.
 
@@ -314,14 +314,72 @@
     for segment_id in segments_to_color:
         mask = segment_mask == segment_id
         new_overlay[mask, 3] = new_opacity[segment_id]
 
     return new_overlay
 
 
+def mark_boundaries(
+    image: np.ndarray,
+    segment_mask: np.ndarray,
+    color: Union[str, Tuple[int, int, int]] = "red",
+    opacity: float = 1.0,
+) -> np.ndarray:
+    """Mark the boundaries of the segments in the image.
+
+    Parameters
+    ----------
+    image : np.ndarray
+        The image to mark the boundaries of the segments in.
+        The image must be an array of shape `(image_width, image_height, 3)`.
+        The image will be modified in-place.
+
+    segment_mask : np.ndarray
+        The mask generated by :meth:`visualime.lime.create_segments`:
+        An array of shape `(image_width, image_height)`.
+
+    color : str or int 3-tuple (RGB), default "red"
+        The color for the boundaries.
+        Can be given as a color name or an RGB tuple.
+
+        Color names are parsed through :meth:`PIL.ImageColor.getrgb`.
+        To obtain a list of available color names, run:
+
+        >>> from PIL.ImageColor import colormap, getrgb
+        >>> for name, code in colormap.items(): print(name, getrgb(code))
+
+        Note that while it is possible to pass an RGBA tuple, only the RGB values
+        will be considered, the opacity will be determined by the `opacity` parameter.
+
+    opacity : float, default 1.0
+        The opacity of the boundaries as a number between `0.0` and `1.0`.
+
+    Returns
+    -------
+    np.ndarray
+        An array of shape `(image_width, image_height, 3)` representing an RGB image.
+    """
+    rgb_color = _get_color(color, opacity)[:3]
+
+    if image.shape[:2] != segment_mask.shape:
+        raise ValueError(
+            f"The shape of the mask ({segment_mask.shape}) does not match "
+            f"the shape of the image ({image.shape[:2]})"
+        )
+
+    for i in range(1, image.shape[0]):
+        for j in range(1, image.shape[1]):
+            if segment_mask[i, j] != segment_mask[i - 1, j]:
+                image[i, j] = image[i, j] * (1 - opacity) + rgb_color * opacity
+            if segment_mask[i, j] != segment_mask[i, j - 1]:
+                image[i, j] = image[i, j] * (1 - opacity) + rgb_color * opacity
+
+    return image
+
+
 # TODO: Add more functions to normalize the segments weights, deal with outliers etc.
 
 
 def smooth_weights(segment_weights: np.ndarray) -> np.ndarray:
     """Smooth the `segment_weights` by applying the sigmoid function.
 
     Parameters
```

### Comparing `visualime-0.0.5/visualime.egg-info/PKG-INFO` & `visualime-0.0.6/visualime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualime
-Version: 0.0.5
+Version: 0.0.6
 Summary: Implementation of LIME focused on producing user-centric local explanations for image classifiers.
 Author-email: Kilian Kluge <dev@kluge.ai>, The VisuaLIME developers <xai.demonstrator@gmail.com>
 License: Apache 2.0 License
 Project-URL: Documentation, https://visualime.readthedocs.io/
 Project-URL: Repository, https://github.com/xai-demonstrator/visualime
 Project-URL: Bug Tracker, https://github.com/xai-demonstrator/visualime/issues
 Classifier: Development Status :: 3 - Alpha
```

