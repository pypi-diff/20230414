# Comparing `tmp/cyclic_boosting-0.1.0.tar.gz` & `tmp/cyclic_boosting-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclic_boosting-0.1.0.tar", max compression
+gzip compressed data, was "cyclic_boosting-1.0.0.tar", max compression
```

## Comparing `cyclic_boosting-0.1.0.tar` & `cyclic_boosting-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    14197 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/LICENSE
--rw-r--r--   0        0        0     1268 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/README.md
--rw-r--r--   0        0        0     3489 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/GBSregression.py
--rw-r--r--   0        0        0     1943 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/__init__.py
--rw-r--r--   0        0        0    44776 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/base.py
--rw-r--r--   0        0        0      719 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/binning/__init__.py
--rw-r--r--   0        0        0    10628 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/binning/_binary_search.py
--rw-r--r--   0        0        0     2953 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/binning/_utils.py
--rw-r--r--   0        0        0     8282 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/binning/bin_number_transformer.py
--rw-r--r--   0        0        0    19266 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/binning/ecdf_transformer.py
--rw-r--r--   0        0        0     4896 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/classification.py
--rw-r--r--   0        0        0    12955 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/common_smoothers.py
--rw-r--r--   0        0        0    11607 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/features.py
--rw-r--r--   0        0        0    13132 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/flags.py
--rw-r--r--   0        0        0     2308 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/learning_rate.py
--rw-r--r--   0        0        0     2383 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/link.py
--rw-r--r--   0        0        0     8943 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/location.py
--rw-r--r--   0        0        0     8331 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/nbinom.py
--rw-r--r--   0        0        0     6831 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/observers.py
--rw-r--r--   0        0        0     6108 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/pipelines.py
--rw-r--r--   0        0        0    11070 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/plots/_1dplots.py
--rw-r--r--   0        0        0     7517 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/plots/_2dplots.py
--rw-r--r--   0        0        0    10899 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/plots/__init__.py
--rw-r--r--   0        0        0     7497 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/plots/plot_utils.py
--rw-r--r--   0        0        0    15702 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/price.py
--rw-r--r--   0        0        0     6953 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/regression.py
--rw-r--r--   0        0        0      529 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/__init__.py
--rw-r--r--   0        0        0     1185 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/base.py
--rw-r--r--   0        0        0     4737 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/extrapolate.py
--rw-r--r--   0        0        0    10724 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/meta_smoother.py
--rw-r--r--   0        0        0    14258 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/multidim.py
--rw-r--r--   0        0        0    26024 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/onedim.py
--rw-r--r--   0        0        0     4940 2023-04-13 16:16:00.143156 cyclic_boosting-0.1.0/cyclic_boosting/smoothing/orthofit.py
--rw-r--r--   0        0        0    30546 2023-04-13 16:16:00.147156 cyclic_boosting-0.1.0/cyclic_boosting/utils.py
--rw-r--r--   0        0        0     1394 2023-04-13 16:16:00.147156 cyclic_boosting-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2426 1970-01-01 00:00:00.000000 cyclic_boosting-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    14197 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1268 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/README.md
+-rw-r--r--   0        0        0     3489 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/GBSregression.py
+-rw-r--r--   0        0        0     1943 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/__init__.py
+-rw-r--r--   0        0        0    44776 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/base.py
+-rw-r--r--   0        0        0      719 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/binning/__init__.py
+-rw-r--r--   0        0        0    10628 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/binning/_binary_search.py
+-rw-r--r--   0        0        0     2953 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/binning/_utils.py
+-rw-r--r--   0        0        0     8282 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/binning/bin_number_transformer.py
+-rw-r--r--   0        0        0    19266 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/binning/ecdf_transformer.py
+-rw-r--r--   0        0        0     4896 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/classification.py
+-rw-r--r--   0        0        0    13130 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/common_smoothers.py
+-rw-r--r--   0        0        0    11607 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/features.py
+-rw-r--r--   0        0        0    13132 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/flags.py
+-rw-r--r--   0        0        0     2308 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/learning_rate.py
+-rw-r--r--   0        0        0     2383 2023-04-14 14:34:07.125378 cyclic_boosting-1.0.0/cyclic_boosting/link.py
+-rw-r--r--   0        0        0     8943 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/location.py
+-rw-r--r--   0        0        0     8331 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/nbinom.py
+-rw-r--r--   0        0        0     6831 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/observers.py
+-rw-r--r--   0        0        0     6108 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/pipelines.py
+-rw-r--r--   0        0        0    11070 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/plots/_1dplots.py
+-rw-r--r--   0        0        0     7517 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/plots/_2dplots.py
+-rw-r--r--   0        0        0    10899 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/plots/__init__.py
+-rw-r--r--   0        0        0     7497 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/plots/plot_utils.py
+-rw-r--r--   0        0        0    15702 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/price.py
+-rw-r--r--   0        0        0     6953 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/regression.py
+-rw-r--r--   0        0        0      529 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/__init__.py
+-rw-r--r--   0        0        0     1185 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/base.py
+-rw-r--r--   0        0        0     4737 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/extrapolate.py
+-rw-r--r--   0        0        0    10724 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/meta_smoother.py
+-rw-r--r--   0        0        0    14258 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/multidim.py
+-rw-r--r--   0        0        0    26024 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/onedim.py
+-rw-r--r--   0        0        0     4940 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/smoothing/orthofit.py
+-rw-r--r--   0        0        0    30546 2023-04-14 14:34:07.129378 cyclic_boosting-1.0.0/cyclic_boosting/utils.py
+-rw-r--r--   0        0        0     1394 2023-04-14 14:34:07.133379 cyclic_boosting-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2426 1970-01-01 00:00:00.000000 cyclic_boosting-1.0.0/PKG-INFO
```

### Comparing `cyclic_boosting-0.1.0/LICENSE` & `cyclic_boosting-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/README.md` & `cyclic_boosting-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/GBSregression.py` & `cyclic_boosting-1.0.0/cyclic_boosting/GBSregression.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/__init__.py` & `cyclic_boosting-1.0.0/cyclic_boosting/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/base.py` & `cyclic_boosting-1.0.0/cyclic_boosting/base.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/binning/__init__.py` & `cyclic_boosting-1.0.0/cyclic_boosting/binning/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/binning/_binary_search.py` & `cyclic_boosting-1.0.0/cyclic_boosting/binning/_binary_search.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/binning/_utils.py` & `cyclic_boosting-1.0.0/cyclic_boosting/binning/_utils.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/binning/bin_number_transformer.py` & `cyclic_boosting-1.0.0/cyclic_boosting/binning/bin_number_transformer.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/binning/ecdf_transformer.py` & `cyclic_boosting-1.0.0/cyclic_boosting/binning/ecdf_transformer.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/classification.py` & `cyclic_boosting-1.0.0/cyclic_boosting/classification.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/common_smoothers.py` & `cyclic_boosting-1.0.0/cyclic_boosting/common_smoothers.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,21 @@
         return flags.IS_UNORDERED
     elif flags.is_unordered_set(feature_property):
         return flags.IS_UNORDERED
     else:
         features = ""
         if feature_group is not None:
             features = "for feature {}".format(feature_group)
-        _logger.warning(
-            "Feature property {0} is not known {1}."
-            " Thus it is converted to IS_UNORDERED!".format(flags.flags_to_string(feature_property), features)
-        )
+        if flags.has_missing_set(feature_property):
+            _logger.info("No feature property set. Thus it is set to default IS_UNORDERED!")
+        else:
+            _logger.warning(
+                "Feature property {0} is not known {1}."
+                " Thus it is converted to IS_UNORDERED!".format(flags.flags_to_string(feature_property), features)
+            )
         return flags.IS_UNORDERED
 
 
 def _choice_fct_svd(feature_group, feature_prop, feature_type=None):
     if isinstance(feature_prop, tuple):
         feature_prop = tuple([_simplify_flags(fp, feature_group) for fp in feature_prop])
         return feature_prop
```

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/features.py` & `cyclic_boosting-1.0.0/cyclic_boosting/features.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/flags.py` & `cyclic_boosting-1.0.0/cyclic_boosting/flags.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/learning_rate.py` & `cyclic_boosting-1.0.0/cyclic_boosting/learning_rate.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/link.py` & `cyclic_boosting-1.0.0/cyclic_boosting/link.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/location.py` & `cyclic_boosting-1.0.0/cyclic_boosting/location.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/nbinom.py` & `cyclic_boosting-1.0.0/cyclic_boosting/nbinom.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/observers.py` & `cyclic_boosting-1.0.0/cyclic_boosting/observers.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/pipelines.py` & `cyclic_boosting-1.0.0/cyclic_boosting/pipelines.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/plots/_1dplots.py` & `cyclic_boosting-1.0.0/cyclic_boosting/plots/_1dplots.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/plots/_2dplots.py` & `cyclic_boosting-1.0.0/cyclic_boosting/plots/_2dplots.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/plots/__init__.py` & `cyclic_boosting-1.0.0/cyclic_boosting/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/plots/plot_utils.py` & `cyclic_boosting-1.0.0/cyclic_boosting/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/price.py` & `cyclic_boosting-1.0.0/cyclic_boosting/price.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/regression.py` & `cyclic_boosting-1.0.0/cyclic_boosting/regression.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/__init__.py` & `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/base.py` & `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/base.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/extrapolate.py` & `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/extrapolate.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/meta_smoother.py` & `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/meta_smoother.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/multidim.py` & `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/multidim.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/onedim.py` & `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/onedim.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/smoothing/orthofit.py` & `cyclic_boosting-1.0.0/cyclic_boosting/smoothing/orthofit.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/cyclic_boosting/utils.py` & `cyclic_boosting-1.0.0/cyclic_boosting/utils.py`

 * *Files identical despite different names*

### Comparing `cyclic_boosting-0.1.0/pyproject.toml` & `cyclic_boosting-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyclic-boosting"
-version = "0.1.0"
+version = "1.0.0"
 description = "Implementation of Cyclic Boosting machine learning algorithms"
 authors = ["Blue Yonder GmbH"]
 packages = [{include = "cyclic_boosting"}]
 readme = "README.md"
 classifiers = [
    "Topic :: Scientific/Engineering :: Artificial Intelligence",
    "Programming Language :: Python :: 3 :: Only",
```

### Comparing `cyclic_boosting-0.1.0/PKG-INFO` & `cyclic_boosting-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclic-boosting
-Version: 0.1.0
+Version: 1.0.0
 Summary: Implementation of Cyclic Boosting machine learning algorithms
 Author: Blue Yonder GmbH
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

