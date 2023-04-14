# Comparing `tmp/statscend-0.1.4.tar.gz` & `tmp/statscend-0.1.5.tar.gz`

## Comparing `statscend-0.1.4.tar` & `statscend-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.4/.DS_Store
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/bn_logistic_regression.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/datasets.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/linear_regression.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/mn_logistic_regression.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 statscend-0.1.4/statscend/ordinal_regression.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.4/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.4/LICENSE
--rw-r--r--   0        0        0     5399 2020-02-02 00:00:00.000000 statscend-0.1.4/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 statscend-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.5/.DS_Store
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/__init__.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/bn_logistic_regression.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/datasets.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/linear_regression.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/mn_logistic_regression.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 statscend-0.1.5/statscend/ordinal_regression.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.5/LICENSE
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 statscend-0.1.5/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 statscend-0.1.5/PKG-INFO
```

### Comparing `statscend-0.1.4/.DS_Store` & `statscend-0.1.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `statscend-0.1.4/statscend/bn_logistic_regression.py` & `statscend-0.1.5/statscend/bn_logistic_regression.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,26 @@
         'Accuracy': [accuracy],
         'Specificity': [specificity],
         'Sensitivity': [sensitivity]
     }
 
     predictive_measures_table = pd.DataFrame(predictive_measures)
 
+    overall_model_test = pd.DataFrame({
+        'Deviance': -2 * model.llf,
+        'AIC': model.aic,
+
+        'Chi Squared': [round(model.llr, 3)],
+        'df': [int(model.df_model)],
+        'p': [round(model.llr_pvalue, 4)],
+
+    })
+
     results_dict = {
-        "summary_table": summary_table,
+        "overall_model_test": overall_model_test,
         "coefficients_table": coefficients_table,
         "predictive_measures_table": predictive_measures_table,
-        "classification_table": cmdf
+        "classification_table": cmdf,
+        "summary_table": summary_table,
     }
 
     return results_dict
```

### Comparing `statscend-0.1.4/statscend/linear_regression.py` & `statscend-0.1.5/statscend/linear_regression.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,12 +46,28 @@
     summary_table.columns = ['Description', 'Value', 'Description', 'Value']
 
     # Table 3: Regression Diagnostics Table
     diagnostics_table = pd.read_html(
         model.summary().tables[2].as_html(), header=None, index_col=None)[0]
     diagnostics_table.columns = ['Statistic', 'Value', 'Statistic', 'Value']
 
+    # Table 4: overall model fit
+    fvalue = model.fvalue.round(3)
+    pvalue = model.f_pvalue.round(3)
+    df_model = int(model.df_model)
+    df_resid = int(model.df_resid)
+
+    r_squared = model.rsquared.round(3)
+    r = np.sqrt(r_squared).round(3)
+    r_squared_adj = model.rsquared_adj.round(3)
+
+    overall_model_fit = [['R', 'R-squared', 'Adj. R-squared', 'F-statistic', 'p-value', 'df-model', 'df-resid'],
+                         [r, r_squared, r_squared_adj, fvalue, pvalue, df_model, df_resid]]
+    overall_model_fit = pd.DataFrame(
+        overall_model_fit[1:], columns=overall_model_fit[0])
+
     results = {}
-    results['coefficients_table'] = coefficients_table.round(3)
+    results['overall_model_fit'] = overall_model_fit
     results['summary_table'] = summary_table.round(3)
+    results['coefficients_table'] = coefficients_table.round(3)
     results['diagnostics_table'] = diagnostics_table.round(3)
     return results
```

### Comparing `statscend-0.1.4/statscend/mn_logistic_regression.py` & `statscend-0.1.5/statscend/mn_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.4/statscend/ordinal_regression.py` & `statscend-0.1.5/statscend/ordinal_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.4/LICENSE` & `statscend-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `statscend-0.1.4/pyproject.toml` & `statscend-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statscend"
-version = "0.1.4"
+version = "0.1.5"
 license = {file = "LICENSE"}
 authors = [
   { name="Hashim Puthiyakath", email="hashputhiyakath@gmail.com" },
 ]
 description = "A Python package for performing various statistical analyses"
 readme = "README.md"
 requires-python = ">=3.7"
```

