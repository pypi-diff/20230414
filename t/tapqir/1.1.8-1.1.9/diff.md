# Comparing `tmp/tapqir-1.1.8.tar.gz` & `tmp/tapqir-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapqir-1.1.8.tar", last modified: Thu Nov  3 12:44:59 2022, max compression
+gzip compressed data, was "tapqir-1.1.9.tar", last modified: Mon Nov  7 18:17:00 2022, max compression
```

## Comparing `tapqir-1.1.8.tar` & `tapqir-1.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:59.226495 tapqir-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-03 12:44:50.000000 tapqir-1.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-03 12:44:50.000000 tapqir-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-11-03 12:44:59.226495 tapqir-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-11-03 12:44:50.000000 tapqir-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-11-03 12:44:59.226495 tapqir-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-11-03 12:44:50.000000 tapqir-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:59.226495 tapqir-1.1.8/tapqir/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-03 12:44:59.226495 tapqir-1.1.8/tapqir/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/app.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:59.222495 tapqir-1.1.8/tapqir/distributions/
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/distributions/affine_beta.py
--rw-r--r--   0 runner    (1001) docker     (121)     9025 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/distributions/ksmogn.py
--rw-r--r--   0 runner    (1001) docker     (121)     6454 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/distributions/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    41089 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/gui.py
--rw-r--r--   0 runner    (1001) docker     (121)    11581 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:59.222495 tapqir-1.1.8/tapqir/imscroll/
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/imscroll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18517 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/imscroll/glimpse_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:59.226495 tapqir-1.1.8/tapqir/infer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/infer/elbo.py
--rw-r--r--   0 runner    (1001) docker     (121)    14716 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/infer/sum_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    41162 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:59.226495 tapqir-1.1.8/tapqir/models/
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27843 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/models/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (121)    21914 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/models/crosstalk.py
--rw-r--r--   0 runner    (1001) docker     (121)    25444 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/models/hmm.py
--rw-r--r--   0 runner    (1001) docker     (121)    13202 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:59.226495 tapqir-1.1.8/tapqir/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5585 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     9024 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/utils/imscroll.py
--rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/utils/mle_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     5070 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/utils/simulate.py
--rw-r--r--   0 runner    (1001) docker     (121)    12706 2022-11-03 12:44:50.000000 tapqir-1.1.8/tapqir/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:59.222495 tapqir-1.1.8/tapqir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-11-03 12:44:59.000000 tapqir-1.1.8/tapqir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-11-03 12:44:59.000000 tapqir-1.1.8/tapqir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 12:44:59.000000 tapqir-1.1.8/tapqir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-03 12:44:59.000000 tapqir-1.1.8/tapqir.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-11-03 12:44:59.000000 tapqir-1.1.8/tapqir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-03 12:44:59.000000 tapqir-1.1.8/tapqir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:59.226495 tapqir-1.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 12:44:50.000000 tapqir-1.1.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3266 2022-11-03 12:44:50.000000 tapqir-1.1.8/test/test_imscroll.py
--rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-11-03 12:44:50.000000 tapqir-1.1.8/test/test_tapqir.py
--rw-r--r--   0 runner    (1001) docker     (121)    68838 2022-11-03 12:44:50.000000 tapqir-1.1.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:17:00.088532 tapqir-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-07 18:16:47.000000 tapqir-1.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-07 18:16:47.000000 tapqir-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-11-07 18:17:00.088532 tapqir-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-11-07 18:16:47.000000 tapqir-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-11-07 18:17:00.088532 tapqir-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-11-07 18:16:47.000000 tapqir-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:17:00.088532 tapqir-1.1.9/tapqir/
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-07 18:17:00.088532 tapqir-1.1.9/tapqir/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/app.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:17:00.084532 tapqir-1.1.9/tapqir/distributions/
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/distributions/affine_beta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9025 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/distributions/ksmogn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6454 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/distributions/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41089 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/gui.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11581 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:17:00.084532 tapqir-1.1.9/tapqir/imscroll/
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/imscroll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18517 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/imscroll/glimpse_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:17:00.088532 tapqir-1.1.9/tapqir/infer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/infer/elbo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14716 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/infer/sum_product.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41162 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:17:00.088532 tapqir-1.1.9/tapqir/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27843 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/models/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21914 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/models/crosstalk.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25444 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/models/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13502 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:17:00.088532 tapqir-1.1.9/tapqir/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5585 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9024 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/utils/imscroll.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/utils/mle_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5070 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/utils/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12706 2022-11-07 18:16:47.000000 tapqir-1.1.9/tapqir/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:17:00.084532 tapqir-1.1.9/tapqir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-11-07 18:17:00.000000 tapqir-1.1.9/tapqir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-11-07 18:17:00.000000 tapqir-1.1.9/tapqir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 18:17:00.000000 tapqir-1.1.9/tapqir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-07 18:17:00.000000 tapqir-1.1.9/tapqir.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      659 2022-11-07 18:17:00.000000 tapqir-1.1.9/tapqir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-07 18:17:00.000000 tapqir-1.1.9/tapqir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 18:17:00.088532 tapqir-1.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 18:16:47.000000 tapqir-1.1.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3266 2022-11-07 18:16:47.000000 tapqir-1.1.9/test/test_imscroll.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-11-07 18:16:47.000000 tapqir-1.1.9/test/test_tapqir.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68838 2022-11-07 18:16:47.000000 tapqir-1.1.9/versioneer.py
```

### Comparing `tapqir-1.1.8/LICENSE.md` & `tapqir-1.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/PKG-INFO` & `tapqir-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapqir
-Version: 1.1.8
+Version: 1.1.9
 Summary: Bayesian analysis of co-localization single-molecule microscopy image data
 Home-page: https://tapqir.readthedocs.io
 Author: Yerdos Ordabayev
 Author-email: ordabayev@brandeis.edu
 License: Apache 2.0
 Project-URL: Documentation, https://tapqir.readthedocs.io
 Project-URL: Source, https://github.com/gelles-brandeis/tapqir
```

### Comparing `tapqir-1.1.8/README.rst` & `tapqir-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/setup.py` & `tapqir-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/app.ipynb` & `tapqir-1.1.9/tapqir/app.ipynb`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/distributions/affine_beta.py` & `tapqir-1.1.9/tapqir/distributions/affine_beta.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/distributions/ksmogn.py` & `tapqir-1.1.9/tapqir/distributions/ksmogn.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/distributions/util.py` & `tapqir-1.1.9/tapqir/distributions/util.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/exceptions.py` & `tapqir-1.1.9/tapqir/exceptions.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/gui.py` & `tapqir-1.1.9/tapqir/gui.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/handlers.py` & `tapqir-1.1.9/tapqir/handlers.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/imscroll/glimpse_reader.py` & `tapqir-1.1.9/tapqir/imscroll/glimpse_reader.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/infer/elbo.py` & `tapqir-1.1.9/tapqir/infer/elbo.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/infer/sum_product.py` & `tapqir-1.1.9/tapqir/infer/sum_product.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/logger.py` & `tapqir-1.1.9/tapqir/logger.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/main.py` & `tapqir-1.1.9/tapqir/main.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/models/cosmos.py` & `tapqir-1.1.9/tapqir/models/cosmos.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/models/crosstalk.py` & `tapqir-1.1.9/tapqir/models/crosstalk.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/models/hmm.py` & `tapqir-1.1.9/tapqir/models/hmm.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/models/model.py` & `tapqir-1.1.9/tapqir/models/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,17 +290,24 @@
         )
 
         # save global parameters for tensorboard
         writer.add_scalar("-ELBO", self.iter_loss, self.iter)
         for name, val in pyro.get_param_store().items():
             if val.dim() == 0:
                 writer.add_scalar(name, val.item(), self.iter)
-            elif val.dim() == 1 and len(val) <= self.S + 1:
+            elif val.dim() == 1 and len(val) <= self.Q * 2:
                 scalars = {str(i): v.item() for i, v in enumerate(val)}
                 writer.add_scalars(name, scalars, self.iter)
+            elif val.dim() == 2 and len(val) <= self.Q * 2:
+                scalars = {
+                    f"{i}_{j}": k.item()
+                    for i, v in enumerate(val)
+                    for j, k in enumerate(v)
+                }
+                writer.add_scalars(name, scalars, self.iter)
 
         if False and self.data.labels is not None:
             pred_labels = (
                 self.pspecific_map[self.data.is_ontarget].cpu().numpy().ravel()
             )
             true_labels = self.data.labels["z"].ravel()
```

### Comparing `tapqir-1.1.8/tapqir/utils/dataset.py` & `tapqir-1.1.9/tapqir/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/utils/imscroll.py` & `tapqir-1.1.9/tapqir/utils/imscroll.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/utils/mle_analysis.py` & `tapqir-1.1.9/tapqir/utils/mle_analysis.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/utils/simulate.py` & `tapqir-1.1.9/tapqir/utils/simulate.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir/utils/stats.py` & `tapqir-1.1.9/tapqir/utils/stats.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir.egg-info/PKG-INFO` & `tapqir-1.1.9/tapqir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapqir
-Version: 1.1.8
+Version: 1.1.9
 Summary: Bayesian analysis of co-localization single-molecule microscopy image data
 Home-page: https://tapqir.readthedocs.io
 Author: Yerdos Ordabayev
 Author-email: ordabayev@brandeis.edu
 License: Apache 2.0
 Project-URL: Documentation, https://tapqir.readthedocs.io
 Project-URL: Source, https://github.com/gelles-brandeis/tapqir
```

### Comparing `tapqir-1.1.8/tapqir.egg-info/SOURCES.txt` & `tapqir-1.1.9/tapqir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/tapqir.egg-info/requires.txt` & `tapqir-1.1.9/tapqir.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/test/test_imscroll.py` & `tapqir-1.1.9/test/test_imscroll.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/test/test_tapqir.py` & `tapqir-1.1.9/test/test_tapqir.py`

 * *Files identical despite different names*

### Comparing `tapqir-1.1.8/versioneer.py` & `tapqir-1.1.9/versioneer.py`

 * *Files identical despite different names*

