# Comparing `tmp/nobias-0.1.51.tar.gz` & `tmp/nobias-0.1.6.tar.gz`

## Comparing `nobias-0.1.51.tar` & `nobias-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nobias-0.1.51/.readthedocs.yaml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 nobias-0.1.51/HowTo.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nobias-0.1.51/Makefile
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 nobias-0.1.51/README.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nobias-0.1.51/lumache.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nobias-0.1.51/requirements.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nobias-0.1.51/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nobias-0.1.51/docs/make.bat
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nobias-0.1.51/docs/source/api.rst
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 nobias-0.1.51/docs/source/conf.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 nobias-0.1.51/docs/source/explanation.rst
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 nobias-0.1.51/docs/source/index.rst
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 nobias-0.1.51/docs/source/installation.rst
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nobias-0.1.51/docs/source/modules.rst
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 nobias-0.1.51/docs/source/nobias.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 nobias-0.1.51/nobias/__init__.py
--rw-r--r--   0        0        0     8503 2020-02-02 00:00:00.000000 nobias-0.1.51/nobias/audits.py
--rw-r--r--   0        0        0    10123 2020-02-02 00:00:00.000000 nobias-0.1.51/nobias/distributionshift.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 nobias-0.1.51/nobias/explanation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nobias-0.1.51/tests/__init__.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 nobias-0.1.51/tests/test_audit.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 nobias-0.1.51/tests/test_explanation.py
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 nobias-0.1.51/tests/test_explanationshift.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 nobias-0.1.51/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nobias-0.1.51/LICENSE
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nobias-0.1.51/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nobias-0.1.51/pyproject.toml
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 nobias-0.1.51/PKG-INFO
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nobias-0.1.6/.readthedocs.yaml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 nobias-0.1.6/HowTo.md
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nobias-0.1.6/Makefile
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 nobias-0.1.6/README.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 nobias-0.1.6/requirements.txt
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 nobias-0.1.6/tutorial.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/make.bat
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/source/api.rst
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/source/auditTutorial.rst
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/source/audits.rst
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/source/conf.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/source/index.rst
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/source/installation.rst
+-rw-r--r--   0        0        0    26256 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/source/images/folksShapLocal.png
+-rw-r--r--   0        0        0    25479 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/source/images/folksShapLocal2.png
+-rw-r--r--   0        0        0    17265 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/source/images/folkstShapGlobal.png
+-rw-r--r--   0        0        0    17175 2020-02-02 00:00:00.000000 nobias-0.1.6/docs/source/images/folkstShapGlobal2.png
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 nobias-0.1.6/nobias/__init__.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 nobias-0.1.6/nobias/audits.py
+-rw-r--r--   0        0        0    10123 2020-02-02 00:00:00.000000 nobias-0.1.6/nobias/distributionshift.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 nobias-0.1.6/nobias/explanation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nobias-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 nobias-0.1.6/tests/test_audit.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 nobias-0.1.6/tests/test_explanation.py
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 nobias-0.1.6/tests/test_explanationshift.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 nobias-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 nobias-0.1.6/LICENSE
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nobias-0.1.6/README.md
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nobias-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 nobias-0.1.6/PKG-INFO
```

### Comparing `nobias-0.1.51/HowTo.md` & `nobias-0.1.6/HowTo.md`

 * *Files identical despite different names*

### Comparing `nobias-0.1.51/docs/Makefile` & `nobias-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nobias-0.1.51/docs/make.bat` & `nobias-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nobias-0.1.51/docs/source/conf.py` & `nobias-0.1.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nobias-0.1.51/docs/source/installation.rst` & `nobias-0.1.6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nobias-0.1.51/nobias/audits.py` & `nobias-0.1.6/nobias/distributionshift.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,238 +1,268 @@
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import roc_auc_score
-import shap
 import pandas as pd
+import shap
 
 
-class ExplanationAudit(BaseEstimator, ClassifierMixin):
+class ExplanationShiftDetector(BaseEstimator, ClassifierMixin):
     """
-    Given a model, a dataset, and the protected attribute, we want to know if the model violates demographic parity or not and what are the features pushing for it.
-    We do this by computing the shap values of the model, and then train a classifier to distinguish the protected attribute.
+    Given a model, and two datasets (source,test), we want to know if the behaviour of the model is different bt train and test.
+    We can do this by computing the shap values of the model on the two datasets, and then train a classifier to distinguish between the two datasets.
 
     Example
     -------
     >>> import pandas as pd
-    >>> import numpy as np
-    >>> from sklearn.linear_model import LogisticRegression
+    >>> from sklearn.model_selection import train_test_split
+    >>> from sklearn.datasets import make_blobs
+    >>> from tools.xaiUtils import ExplanationShiftDetector
     >>> from xgboost import XGBRegressor
-    >>> from fairtools.detector import ExplanationAudit
-    >>> N = 5_000
-    >>> x1 = np.random.normal(1, 1, size=N)
-    >>> x2 = np.random.normal(1, 1, size=N)
-    >>> x34 = np.random.multivariate_normal([1, 1], [[1, 0.5], [0.5, 1]], size=N)
-    >>> x3 = x34[:, 0]
-    >>> x4 = x34[:, 1]
-    >>> # Binarize protected attribute
-    >>> x4 = np.where(x4 > np.mean(x4), 1, 0)
-    >>> X = pd.DataFrame([x1, x2, x3, x4]).T
-    >>> X.columns = ["var%d" % (i + 1) for i in range(X.shape[1])]
-    >>> y = (x1 + x2 + x3) / 3
-    >>> y = 1 / (1 + np.exp(-y))
-    >>> detector = ExplanationAudit(model=XGBRegressor(), gmodel=LogisticRegression())
-    >>> detector.fit(X, y, Z="var4")
+    >>> from sklearn.linear_model import LogisticRegression
+
+    >>> X, y = make_blobs(n_samples=2000, centers=2, n_features=5, random_state=0)
+    >>> X_tr, X_te, y_tr, y_te = train_test_split(X, y, test_size=0.5, random_state=0)
+    >>> X_ood,y_ood = make_blobs(n_samples=1000, centers=1, n_features=5, random_state=0)
+
+    >>> detector = ExplanationShiftDetector(model=XGBRegressor(),gmodel=LogisticRegression())
+    >>> detector.fit(X_tr, y_tr, X_ood)
     >>> detector.get_auc_val()
+    # 0.76
+    >>> detector.fit(X_tr, y_tr, X_te)
+    >>> detector.get_auc_val()
+    # 0.5
     """
 
-    def __init__(self, model, gmodel):
+    def __init__(
+        self,
+        model,
+        gmodel,
+        space: str = "explanation",
+        algorithm: str = "auto",
+        masker: bool = False,
+    ):
+        """
+        Parameters
+        ----------
+        model : sklearn model
+            Model to be used to compute the shap values.
+        gmodel : sklearn model
+            Model to be used to distinguish between the two datasets.
+        space : str, optional
+            Space in which the gmodel is learned. Can be 'explanation' or 'input' or 'predictions'. Default is 'explanation'.
+
+        algorithm : "auto", "permutation", "partition", "tree", or "linear"
+                The algorithm used to estimate the Shapley values. There are many different algorithms that
+                can be used to estimate the Shapley values (and the related value for constrained games), each
+                of these algorithms have various tradeoffs and are preferrable in different situations. By
+                default the "auto" options attempts to make the best choice given the passed model and masker,
+                but this choice can always be overriden by passing the name of a specific algorithm. The type of
+                algorithm used will determine what type of subclass object is returned by this constructor, and
+                you can also build those subclasses directly if you prefer or need more fine grained control over
+                their options.
+
+        masker : bool,
+                The masker object is used to define the background distribution over which the Shapley values
+                are estimated. Is a boolean that indicates if the masker should be used or not. If True, the masker is used.
+                If False, the masker is not used. The background distribution is the same distribution as we are calculating the Shapley values.
+                TODO Decide which masker distribution is better to use, options are: train data, hold out data, ood data
+        """
+
         self.model = model
         self.gmodel = gmodel
         self.explainer = None
+        self.space = space
+        self.algorithm = algorithm
+        self.masker = masker
 
-        # Supported F Models
-        self.supported_tree_models = [
-            "XGBClassifier",
-            "XGBRegressor",
-            "GradientBoostingRegressor",
-        ]
-        self.supported_linear_models = [
-            "LogisticRegression",
-            "LinearRegression",
-            "Ridge",
-            "Lasso",
-        ]
-        self.supported_models = (
-            self.supported_tree_models + self.supported_linear_models
-        )
-        # Supported detectors
-        self.supported_linear_detectors = [
-            "LogisticRegression",
-        ]
-        self.supported_tree_detectors = [
-            "XGBClassifier",
-            "GradientBoostingClassifier",
-            "RandomForestClassifier",
-        ]
-        self.supported_detectors = (
-            self.supported_linear_detectors + self.supported_tree_detectors
-        )
-
-        # Check if models are supported
-        if self.get_model_type() not in self.supported_models:
-            raise ValueError(
-                "Model not supported. Supported models are: {} got {}".format(
-                    self.supported_models, self.model.__class__.__name__
-                )
-            )
-        if self.get_gmodel_type() not in self.supported_detectors:
+        # Check if space is supported
+        if self.space not in ["explanation", "input", "prediction"]:
             raise ValueError(
-                "gmodel not supported. Supported models are: {} got {}".format(
-                    self.supported_detectors, self.gmodel.__class__.__name__
+                "space not supported. Supported spaces are: {} got {}".format(
+                    ["explanation", "input", "prediction"], self.space
                 )
             )
 
     def get_gmodel_type(self):
+        """
+        Returns the type of the gmodel
+        """
         if self.gmodel.__class__.__name__ == "Pipeline":
             return self.gmodel.steps[-1][1].__class__.__name__
         else:
             return self.gmodel.__class__.__name__
 
     def get_model_type(self):
         if self.model.__class__.__name__ == "Pipeline":
             return self.model.steps[-1][1].__class__.__name__
         else:
             return self.model.__class__.__name__
 
-    def get_split_data(self, X, y, Z, n1=0.6, n2=0.5):
-        self.X_tr, X_val, self.y_tr, y_val = train_test_split(
-            X, y, random_state=0, test_size=0.6, stratify=X[Z]
-        )
-        self.X_val, self.X_te, self.y_val, self.y_te = train_test_split(
-            X_val, y_val, random_state=0, test_size=0.5, stratify=X_val[Z]
-        )
-        # Check number of classes present in label
-        if len(set(self.y_tr)) <= 1:
-            raise ValueError("Train set has only one class")
-        if len(set(self.y_val)) <= 1:
-            raise ValueError("Validation set has only one class")
-        if len(set(self.y_te)) <= 1:
-            raise ValueError("Test set has only one class")
-
-        # Check number or protected groups
-        if len(set(self.X_tr[Z])) <= 1:
-            raise ValueError("Train set has only one protected group")
-        if len(set(self.X_val[Z])) <= 1:
-            raise ValueError("Validation set has only one protected group")
-        if len(set(self.X_te[Z])) <= 1:
-            raise ValueError("Test set has only one protected group")
-
-        return self.X_tr, self.X_val, self.X_te, self.y_tr, self.y_val, self.y_te
+    def fit(self, X_source, y_source, X_ood):
+        """
+        1. Fits the model F to the data by splitting the data into two equal parts.
+        2. Get the explanations of the model F on the validation set and OOD
+        3. Fit the inspector to the data to the data.
 
-    def fit(self, X, y, Z):
+        """
 
         # Check that X and y have correct shape
-        check_X_y(X, y)
-        self.Z = Z
-
-        # Split data intro train, validation and test
-        _ = self.get_split_data(X, y, Z)
+        check_X_y(X_source, y_source)
+        self.X_ood = X_ood
 
-        # Extract prottected att. and remove from data
-        self.Z_tr = self.X_tr[self.Z]
-        self.Z_val = self.X_val[self.Z]
-        self.Z_te = self.X_te[self.Z]
-        self.X_tr = self.X_tr.drop(self.Z, axis=1)
-        self.X_val = self.X_val.drop(self.Z, axis=1)
-        self.X_te = self.X_te.drop(self.Z, axis=1)
+        self.X_tr, self.X_val, self.y_tr, self.y_val = train_test_split(
+            X_source, y_source, random_state=0, test_size=0.5
+        )
 
         # Fit model F
         self.fit_model(self.X_tr, self.y_tr)
 
         # Get explanations
         self.S_val = self.get_explanations(self.X_val)
+        self.S_ood = self.get_explanations(self.X_ood)
 
-        # Fit model G
-        self.fit_audit_detector(self.S_val, self.Z_val)
+        # Create dataset for  explanation shift detector
+        self.S_val["label"] = False
+        self.S_ood["label"] = True
+
+        self.S = pd.concat([self.S_val, self.S_ood])
+
+        (
+            self.X_shap_tr,
+            self.X_shap_te,
+            self.y_shap_tr,
+            self.y_shap_te,
+        ) = train_test_split(
+            self.S.drop(columns="label"), self.S["label"], random_state=0, test_size=0.5
+        )
+        self.fit_explanation_shift(self.X_shap_tr, self.y_shap_tr)
 
         return self
 
     def predict(self, X):
-        if self.Z in X.columns:
-            X = X.drop(self.Z, axis=1)
         return self.gmodel.predict(self.get_explanations(X))
 
     def predict_proba(self, X):
-        if self.Z in X.columns:
-            X = X.drop(self.Z, axis=1)
         return self.gmodel.predict_proba(self.get_explanations(X))
 
     def explanation_predict(self, X):
         return self.gmodel.predict(X)
 
     def explanation_predict_proba(self, X):
         return self.gmodel.predict_proba(X)
 
     def fit_model(self, X, y):
         self.model.fit(X, y)
 
-    def fit_audit_detector(self, X, y):
+    def fit_explanation_shift(self, X, y):
         self.gmodel.fit(X, y)
 
-    def get_explanations(self, X):
-        # Determine the type of SHAP explainer to use
-        if self.get_model_type() in self.supported_tree_models:
-            self.explainer = shap.Explainer(self.model)
-        elif self.get_model_type() in self.supported_linear_models:
-            self.explainer = shap.LinearExplainer(
-                self.model, X, feature_dependence="correlation_dependent"
-            )
+    def get_explanations(self, X, data_masker=None):
+        if data_masker == None:
+            data_masker = self.X_tr
         else:
-            raise ValueError(
-                "Model not supported. Supported models are: {}, got {}".format(
-                    self.supported_models, self.model.__class__.__name__
+            data_masker = data_masker
+
+        if self.space == "explanation":
+            if self.masker:
+                self.explainer = shap.Explainer(
+                    self.model, algorithm=self.algorithm, masker=data_masker
                 )
+            else:
+                self.explainer = shap.Explainer(self.model, algorithm=self.algorithm)
+
+            shap_values = self.explainer(X)
+            # Name columns
+            if isinstance(X, pd.DataFrame):
+                columns_name = X.columns
+            else:
+                columns_name = ["Shap%d" % (i + 1) for i in range(X.shape[1])]
+
+            exp = pd.DataFrame(
+                data=shap_values.values,
+                columns=columns_name,
             )
+        if self.space == "input":
+            shap_values = X
+            # Name columns
+            if isinstance(X, pd.DataFrame):
+                exp = X
+            else:
+                columns_name = ["Shap%d" % (i + 1) for i in range(X.shape[1])]
 
-        shap_values = self.explainer(X)
-        # Name columns
-        if isinstance(X, pd.DataFrame):
-            columns_name = X.columns
-        else:
-            columns_name = ["Shap%d" % (i + 1) for i in range(X.shape[1])]
+                exp = pd.DataFrame(
+                    data=shap_values,
+                    columns=columns_name,
+                )
+        if self.space == "prediction":
+            try:
+                shap_values = self.model.predict_proba(X)[:, 1]
+            except:
+                shap_values = self.model.predict(X)
+
+            # Name columns
+            exp = pd.DataFrame(
+                data=shap_values,
+                columns=["preds"],
+            )
 
-        exp = pd.DataFrame(
-            data=shap_values.values,
-            columns=columns_name,
-        )
         return exp
 
-    def get_auc_f_val(self):
-        """
-        TODO Case of F being a classifier
-        """
-        return roc_auc_score(self.y_val, self.model.predict(self.X_val))
-
     def get_auc_val(self):
         """
-        Returns the AUC of the validation set
+        Returns the AUC of the explanation shift detector on the validation set of the explanation space
+        Example
+        -------
+        from sklearn.model_selection import train_test_split
+        from sklearn.datasets import make_blobs
+        from tools.xaiUtils import ExplanationShiftDetector
+        from xgboost import XGBRegressor
+        from sklearn.linear_model import LogisticRegression
+
+        # Create data
+        X, y = make_blobs(n_samples=2000, centers=2, n_features=5, random_state=0)
+        X_tr, X_te, y_tr, y_te = train_test_split(X, y, test_size=0.5, random_state=0)
+        X_ood,y_ood = make_blobs(n_samples=1000, centers=1, n_features=5, random_state=0)
+
+        detector = ExplanationShiftDetector(model=XGBRegressor(),gmodel=LogisticRegression())
+        detector.fit(X_tr, y_tr, X_ood)
+        detector.get_auc_val()
+        # 0.76
 
         """
-        return roc_auc_score(self.Z_te, self.predict_proba(self.X_te)[:, 1])
+        return roc_auc_score(
+            self.y_shap_te, self.explanation_predict_proba(self.X_shap_te)[:, 1]
+        )
 
     def get_coefs(self):
         if self.gmodel.__class__.__name__ == "Pipeline":
-            if (
-                self.gmodel.steps[-1][1].__class__.__name__
-                in self.supported_linear_models
-            ):
+            if "sklearn.linear_model" in self.gmodel.steps[-1][1].__module__:
                 return self.gmodel.steps[-1][1].coef_
             else:
                 raise ValueError(
-                    "Pipeline model not supported. Supported models are: {}, got {}".format(
-                        self.supported_linear_models,
-                        self.gmodel.steps[-1][1].__class__.__name__,
+                    "Coefficients can not be calculated. Supported models are linear: sklearn.linear_model, got {}".format(
+                        self.gmodel.steps[-1][1].__module__
                     )
                 )
         else:
             return self.get_linear_coefs()
 
     def get_linear_coefs(self):
-        if self.gmodel.__class__.__name__ in self.supported_linear_models:
-            return self.gmodel.coef_[0]
+        if "sklearn.linear_model" in self.gmodel.__module__:
+            return self.gmodel.coef_
         else:
             raise ValueError(
-                "Detector model not supported. Supported models ar linear: {}, got {}".format(
-                    self.supported_linear_detector, self.model.__class__.__name__
+                "Coefficients can not be calculated. Supported models are linear: sklearn.linear_model, got {}".format(
+                    self.gmodel.steps[-1][1].__module__
                 )
             )
+
+    def explain_detector(self):
+        if self.space == "prediction":
+            return
+        exp = shap.Explainer(self.model)
+
+        shap_values = exp.shap_values(self.S_ood.drop(columns="label"))
+        shap.summary_plot(
+            shap_values, self.S_ood.drop(columns="label"), plot_type="bar", show=False
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nobias-0.1.51/nobias/explanation.py` & `nobias-0.1.6/nobias/explanation.py`

 * *Files identical despite different names*

### Comparing `nobias-0.1.51/tests/test_explanation.py` & `nobias-0.1.6/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `nobias-0.1.51/tests/test_explanationshift.py` & `nobias-0.1.6/tests/test_explanationshift.py`

 * *Files identical despite different names*

### Comparing `nobias-0.1.51/.gitignore` & `nobias-0.1.6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -127,8 +127,9 @@
 
 # Pyre type checker
 .pyre/
 
 token.txt
 .vscode
 stupid.py
-.DS_Store
+.DS_Store
+data
```

### Comparing `nobias-0.1.51/LICENSE` & `nobias-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nobias-0.1.51/pyproject.toml` & `nobias-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "nobias"
-version = "0.01.51"
+version = "0.1.6"
 authors = [
   { name="Carlos Mougan", email="carmougan@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `nobias-0.1.51/PKG-INFO` & `nobias-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobias
-Version: 0.1.51
+Version: 0.1.6
 Summary: A small example package
 Project-URL: Homepage, https://github.com/nobias-project/nobias
 Project-URL: Bug Tracker, https://github.com/nobias-project/nobiasissues
 Author-email: Carlos Mougan <carmougan@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 NoBIAS ITN Project
```

