# Comparing `tmp/statscend-0.1.5.tar.gz` & `tmp/statscend-0.1.6.tar.gz`

## Comparing `statscend-0.1.5.tar` & `statscend-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.5/.DS_Store
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/__init__.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/bn_logistic_regression.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/datasets.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/linear_regression.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/mn_logistic_regression.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/ordinal_regression.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.5/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.5/LICENSE
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 statscend-0.1.5/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 statscend-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.6/.DS_Store
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/__init__.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/bn_logistic_regression.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/datasets.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/linear_regression.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/mn_logistic_regression.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 statscend-0.1.6/statscend/ordinal_regression.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.6/LICENSE
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 statscend-0.1.6/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 statscend-0.1.6/PKG-INFO
```

### Comparing `statscend-0.1.5/.DS_Store` & `statscend-0.1.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `statscend-0.1.5/statscend/bn_logistic_regression.py` & `statscend-0.1.6/statscend/bn_logistic_regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     cmdf['%Correct'] = ""
     cmdf.iloc[0, 2] = (
         (cmdf.iloc[0, 0]/(cmdf.iloc[0, 0] + cmdf.iloc[0, 1])) * 100).round(3)
     cmdf.iloc[1, 2] = (
         (cmdf.iloc[1, 1]/(cmdf.iloc[1, 0] + cmdf.iloc[1, 1])) * 100).round(3)
 
     # Calculate predictive measures from classification table
-    accuracy = ((cmdf['%Correct'].mean())/100).round(3)
+    accuracy = ((cmdf.iloc[0, 0] + cmdf.iloc[1, 1]) / np.sum(cm)).round(3)
     specificity = ((cmdf['%Correct'][0])/100).round(3)
     sensitivity = ((cmdf['%Correct'][1])/100).round(3)
 
     predictive_measures = {
         'Accuracy': [accuracy],
         'Specificity': [specificity],
         'Sensitivity': [sensitivity]
```

### Comparing `statscend-0.1.5/statscend/datasets.py` & `statscend-0.1.6/statscend/datasets.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.5/statscend/linear_regression.py` & `statscend-0.1.6/statscend/linear_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.5/statscend/mn_logistic_regression.py` & `statscend-0.1.6/statscend/mn_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.5/statscend/ordinal_regression.py` & `statscend-0.1.6/statscend/ordinal_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.5/LICENSE` & `statscend-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `statscend-0.1.5/README.md` & `statscend-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `statscend-0.1.5/pyproject.toml` & `statscend-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statscend"
-version = "0.1.5"
+version = "0.1.6"
 license = {file = "LICENSE"}
 authors = [
   { name="Hashim Puthiyakath", email="hashputhiyakath@gmail.com" },
 ]
 description = "A Python package for performing various statistical analyses"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `statscend-0.1.5/PKG-INFO` & `statscend-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statscend
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python package for performing various statistical analyses
 Project-URL: Homepage, https://github.com/hashimputhiyakath/statscend
 Project-URL: Bug Tracker, https://github.com/hashimputhiyakath/statscend/issues
 Author-email: Hashim Puthiyakath <hashputhiyakath@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hashim Puthiyakath
```

