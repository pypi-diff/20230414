# Comparing `tmp/gmltools-0.0.52.tar.gz` & `tmp/gmltools-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.52.tar", last modified: Thu Apr 13 11:45:59 2023, max compression
+gzip compressed data, was "gmltools-0.0.53.tar", last modified: Fri Apr 14 07:56:53 2023, max compression
```

## Comparing `gmltools-0.0.52.tar` & `gmltools-0.0.53.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:45:59.218582 gmltools-0.0.52/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.52/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.52/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-13 11:45:59.218582 gmltools-0.0.52/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.52/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 11:45:59.132459 gmltools-0.0.52/dist/
--rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.52/dist/gmltools-0.0.24.tar.gz
--rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.52/dist/gmltools-0.0.25.tar.gz
--rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.52/dist/gmltools-0.0.26.tar.gz
--rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.52/dist/gmltools-0.0.27.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.52/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.52/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-13 11:45:30.000000 gmltools-0.0.52/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 11:45:59.218582 gmltools-0.0.52/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-13 11:45:22.000000 gmltools-0.0.52/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:45:59.090205 gmltools-0.0.52/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 11:45:59.136766 gmltools-0.0.52/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.52/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.52/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:45:59.191079 gmltools-0.0.52/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.52/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.52/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:45:59.210851 gmltools-0.0.52/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.52/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.52/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.52/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0   118688 2023-04-12 11:41:49.000000 gmltools-0.0.52/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.52/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0     9739 2023-04-13 11:45:08.000000 gmltools-0.0.52/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:45:59.214043 gmltools-0.0.52/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.52/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.52/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.52/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:45:59.217565 gmltools-0.0.52/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.52/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.52/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.52/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.52/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:45:59.186091 gmltools-0.0.52/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-13 11:45:58.000000 gmltools-0.0.52/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-13 11:45:58.000000 gmltools-0.0.52/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:45:58.000000 gmltools-0.0.52/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-13 11:45:58.000000 gmltools-0.0.52/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 11:45:58.000000 gmltools-0.0.52/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 07:56:53.782594 gmltools-0.0.53/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.53/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.53/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-14 07:56:53.781597 gmltools-0.0.53/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.53/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 07:56:53.595620 gmltools-0.0.53/dist/
+-rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.53/dist/gmltools-0.0.24.tar.gz
+-rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.53/dist/gmltools-0.0.25.tar.gz
+-rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.53/dist/gmltools-0.0.26.tar.gz
+-rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.53/dist/gmltools-0.0.27.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.53/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.53/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-14 07:56:29.000000 gmltools-0.0.53/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 07:56:53.782594 gmltools-0.0.53/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-14 07:56:20.000000 gmltools-0.0.53/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:56:53.496273 gmltools-0.0.53/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 07:56:53.604974 gmltools-0.0.53/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.53/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.53/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:56:53.659562 gmltools-0.0.53/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.53/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.53/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:56:53.722976 gmltools-0.0.53/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.53/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.53/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.53/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0   118688 2023-04-12 11:41:49.000000 gmltools-0.0.53/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.53/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    11555 2023-04-14 07:55:01.000000 gmltools-0.0.53/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:56:53.752058 gmltools-0.0.53/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.53/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.53/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.53/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:56:53.780682 gmltools-0.0.53/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.53/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.53/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.53/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.53/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:56:53.647699 gmltools-0.0.53/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-14 07:56:52.000000 gmltools-0.0.53/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-14 07:56:53.000000 gmltools-0.0.53/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 07:56:52.000000 gmltools-0.0.53/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-14 07:56:52.000000 gmltools-0.0.53/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 07:56:52.000000 gmltools-0.0.53/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.52/LICENSE` & `gmltools-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/Models.ipynb` & `gmltools-0.0.53/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/PKG-INFO` & `gmltools-0.0.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.52
+Version: 0.0.53
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.52/README.md` & `gmltools-0.0.53/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/dist/gmltools-0.0.24.tar.gz` & `gmltools-0.0.53/dist/gmltools-0.0.24.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/dist/gmltools-0.0.25.tar.gz` & `gmltools-0.0.53/dist/gmltools-0.0.25.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/dist/gmltools-0.0.26.tar.gz` & `gmltools-0.0.53/dist/gmltools-0.0.26.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/dist/gmltools-0.0.27.tar.gz` & `gmltools-0.0.53/dist/gmltools-0.0.27.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/gmltools.yml` & `gmltools-0.0.53/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/mltools.yml` & `gmltools-0.0.53/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/pyproject.toml` & `gmltools-0.0.53/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.52"
+version = "0.0.53"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.52/setup.py` & `gmltools-0.0.53/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.52',
+    'version': '0.0.53',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.52/src/gmltools/To_Do.txt` & `gmltools-0.0.53/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools/eda/eda.py` & `gmltools-0.0.53/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools/models/bayes.py` & `gmltools-0.0.53/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.53/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools/models/model.py` & `gmltools-0.0.53/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools/models/models_info.py` & `gmltools-0.0.53/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.53/src/gmltools/models/timeseriesplit.py`

 * *Files 11% similar despite different names*

```diff
@@ -159,15 +159,35 @@
                     break
                 else:
                     yield (
                         indices[:test_start+ intra_gap],
                         indices[test_start + gap + intra_gap: test_start + intra_gap + increment_size + gap],
                     )
 
-    def get_n_splits(self, X, y=None, groups=None):
+    def get_n_splits(self, X, y=None, groups=None)->int:
+        """
+        Returns the number of splitting iterations in the cross-validator
+
+        Parameters
+        ----------
+        
+        X : array-like of shape (n_samples, n_features)
+            Training data, where `n_samples` is the number of samples
+            and `n_features` is the number of features.
+
+        y : array-like of shape (n_samples,), default=None
+            The target variable for supervised learning problems.
+        
+        groups : array-like of shape (n_samples,), default=None
+            Group labels for the samples used while splitting the dataset into
+
+        Returns
+        -------
+        n_splits : int
+        """
 
         n_samples = len(X)
 
         # Make sure we have enough samples for the given split parameters
         if self.initial > n_samples:
             raise ValueError(
                 f"Cannot have number of initial_size={self.initial} greater"
@@ -178,15 +198,46 @@
                 f"Size of initial + increment_size + gap too large given sample"
                 f"={n_samples} with initial={self.initial} increment_size={self.increment_size} and gap={self.gap}."
             )
         n_splits=0
         for train_index, test_index in self.split(X):
             n_splits +=1
         return n_splits
+    
+    def get_index_splits(self,X,y=None,groups=None):
+        """
+        Returns the index of the train and test sets for each split
+
+        Parameters
+        ----------
+
+        X : array-like of shape (n_samples, n_features)
+            Training data, where `n_samples` is the number of samples
+            and `n_features` is the number of features.
+
+        y : array-like of shape (n_samples,), default=None
+            The target variable for supervised learning problems.
+
+        groups : array-like of shape (n_samples,), default=None
+            Group labels for the samples used while splitting the dataset into
+
+        Returns
+        -------
+        X_train_date : list
+            List of the index of the train set for each split
+        X_test_date : list
+            List of the index of the test set for each split
+        """
+        X_train_date=[]
+        X_test_date=[]
+        for train_index, test_index in self.split(X):
+            X_train_date.append(X.index[train_index])
+            X_test_date.append(X.index[test_index])
 
+        return train_index,test_index
 
 def plot_timesplit(n_splits, n_samples,test_size=None , min_train_size=None, text=False,figsize=(20,10)):
 
     """
     Plot the train and test size depending on the number of splits for TimeSeriesSplit
 
     Parameters
```

### Comparing `gmltools-0.0.52/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.53/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.53/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.53/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.53/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.53/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.52/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.53/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.52
+Version: 0.0.53
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.52/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.53/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

