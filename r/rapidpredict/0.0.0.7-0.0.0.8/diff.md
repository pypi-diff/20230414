# Comparing `tmp/rapidpredict-0.0.0.7.tar.gz` & `tmp/rapidpredict-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpredict-0.0.0.7.tar", last modified: Tue Apr 11 03:34:33 2023, max compression
+gzip compressed data, was "rapidpredict-0.0.0.8.tar", last modified: Fri Apr 14 02:46:52 2023, max compression
```

## Comparing `rapidpredict-0.0.0.7.tar` & `rapidpredict-0.0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 03:34:33.977957 rapidpredict-0.0.0.7/
--rw-rw-rw-   0        0        0     4574 2023-04-11 03:34:33.977957 rapidpredict-0.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3752 2023-04-10 22:29:36.000000 rapidpredict-0.0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 03:34:33.963206 rapidpredict-0.0.0.7/rapidpredict/
--rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.7/rapidpredict/__init__.py
--rw-rw-rw-   0        0        0    21678 2023-04-11 03:32:56.000000 rapidpredict-0.0.0.7/rapidpredict/supervised.py
-drwxrwxrwx   0        0        0        0 2023-04-11 03:34:33.975460 rapidpredict-0.0.0.7/rapidpredict.egg-info/
--rw-rw-rw-   0        0        0     4574 2023-04-11 03:34:33.000000 rapidpredict-0.0.0.7/rapidpredict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-11 03:34:33.000000 rapidpredict-0.0.0.7/rapidpredict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 03:34:33.000000 rapidpredict-0.0.0.7/rapidpredict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-04-11 03:34:33.000000 rapidpredict-0.0.0.7/rapidpredict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 03:34:33.000000 rapidpredict-0.0.0.7/rapidpredict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 03:34:33.977957 rapidpredict-0.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1810 2023-04-11 03:34:25.000000 rapidpredict-0.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 02:46:52.335807 rapidpredict-0.0.0.8/
+-rw-rw-rw-   0        0        0     5023 2023-04-14 02:46:52.335807 rapidpredict-0.0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4177 2023-04-14 02:44:31.000000 rapidpredict-0.0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 02:46:52.329807 rapidpredict-0.0.0.8/rapidpredict/
+-rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.8/rapidpredict/__init__.py
+-rw-rw-rw-   0        0        0    22122 2023-04-14 02:14:16.000000 rapidpredict-0.0.0.8/rapidpredict/supervised.py
+drwxrwxrwx   0        0        0        0 2023-04-14 02:46:52.334806 rapidpredict-0.0.0.8/rapidpredict.egg-info/
+-rw-rw-rw-   0        0        0     5023 2023-04-14 02:46:52.000000 rapidpredict-0.0.0.8/rapidpredict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-14 02:46:52.000000 rapidpredict-0.0.0.8/rapidpredict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 02:46:52.000000 rapidpredict-0.0.0.8/rapidpredict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-04-14 02:46:52.000000 rapidpredict-0.0.0.8/rapidpredict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 02:46:52.000000 rapidpredict-0.0.0.8/rapidpredict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 02:46:52.335807 rapidpredict-0.0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1806 2023-04-14 02:46:20.000000 rapidpredict-0.0.0.8/setup.py
```

### Comparing `rapidpredict-0.0.0.7/PKG-INFO` & `rapidpredict-0.0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rapidpredict
-Version: 0.0.0.7
+Version: 0.0.0.8
 Summary: rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.
 Author: Synthetic Dataset AI Team
 Author-email: <nematiusa@gmail.com>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: Free To Use But Restricted
-Requires-Python: >=3.8.1.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 # RapidPredict
 RapidPredict is a Python library that simplifies the process of fitting and evaluating multiple machine learning models from scikit-learn. It's designed to provide a quick way to test various algorithms on a given dataset and compare their performance. 
 
 
@@ -34,26 +34,26 @@
 
 
 
 ## Classification
 
 Example :
 
-    from rapidpredict import classification as rp
-    from sklearn.datasets import load_breast_cancer
+    from rapidpredict.supervised import *
     from sklearn.model_selection import train_test_split
-
+    from sklearn.datasets import load_breast_cancer
     data = load_breast_cancer()
     X = data.data
     y= data.target
 
-    X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.5,random_state =123)
+    X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.25,random_state =123)
 
-    clf = rp(verbose=0,ignore_warnings=True, custom_metric=None)
-    models,predictions = clf.fit(X_train, X_test, y_train, y_test)
+
+    clf = rapidclassifier(verbose= 0,ignore_warnings=True, custom_metric=None)
+    models , predictions = clf.fit(X_train, X_test, y_train, y_test)
 
 
 
     |Model |Accuracy	 |Balanced Accuracy |	ROC | AUC |	Recall |	Precision | F1 Score |	5 Fold F1 |	Time  Taken |
     |-------------------------------|------|------|------|------|------|------|------|------|
     | QuadraticDiscriminantAnalysis | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.96 | 0.09 |
     | RandomForestClassifier        | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.96 | 1.21 |
@@ -80,8 +80,36 @@
     | NearestCentroid               | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.94 | 0.08 |
     | GaussianNB                    | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.94 | 0.08 |
     | ExtraTreeClassifier           | 0.94 | 0.94 | 0.94 | 0.94 | 0.94 | 0.94 | 0.93 | 0.08 |
     | DummyClassifier               | 0.62 | 0.50 | 0.50 | 0.62 | 0.39 | 0.48 | 0.77 | 0.08 |
 
 
 
+## Plot Target values
+
+    plot_target(y)
+
+![plot target](./image/plot_target.png)
+
+
+
+## Comparing models suing bar graph
+ 
+  compareModels_bargraph(predictions["F1 Score"] ,models.index)
+ 
+
+![](./image/compareModels_bargraph.png)  
+
+
+## Comparing models suing box plot
+ 
+    compareModels_boxplot(predictions["F1 Score"] ,models.index)
+
+
+![](./image/compareModels_boxplot.png)
+
+
+    
+
+
+
 This code updated from github  ["Lazypredic-Shankar Rao Pandala"](https://github.com/shankarpandala/lazypredict)
```

### Comparing `rapidpredict-0.0.0.7/README.md` & `rapidpredict-0.0.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 
 
 
 ## Classification
 
 Example :
 
-    from rapidpredict import classification as rp
-    from sklearn.datasets import load_breast_cancer
+    from rapidpredict.supervised import *
     from sklearn.model_selection import train_test_split
-
+    from sklearn.datasets import load_breast_cancer
     data = load_breast_cancer()
     X = data.data
     y= data.target
 
-    X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.5,random_state =123)
+    X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.25,random_state =123)
 
-    clf = rp(verbose=0,ignore_warnings=True, custom_metric=None)
-    models,predictions = clf.fit(X_train, X_test, y_train, y_test)
+
+    clf = rapidclassifier(verbose= 0,ignore_warnings=True, custom_metric=None)
+    models , predictions = clf.fit(X_train, X_test, y_train, y_test)
 
 
 
     |Model |Accuracy	 |Balanced Accuracy |	ROC | AUC |	Recall |	Precision | F1 Score |	5 Fold F1 |	Time  Taken |
     |-------------------------------|------|------|------|------|------|------|------|------|
     | QuadraticDiscriminantAnalysis | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.96 | 0.09 |
     | RandomForestClassifier        | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.96 | 1.21 |
@@ -62,8 +62,36 @@
     | NearestCentroid               | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.94 | 0.08 |
     | GaussianNB                    | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.94 | 0.08 |
     | ExtraTreeClassifier           | 0.94 | 0.94 | 0.94 | 0.94 | 0.94 | 0.94 | 0.93 | 0.08 |
     | DummyClassifier               | 0.62 | 0.50 | 0.50 | 0.62 | 0.39 | 0.48 | 0.77 | 0.08 |
 
 
 
+## Plot Target values
+
+    plot_target(y)
+
+![plot target](./image/plot_target.png)
+
+
+
+## Comparing models suing bar graph
+ 
+  compareModels_bargraph(predictions["F1 Score"] ,models.index)
+ 
+
+![](./image/compareModels_bargraph.png)  
+
+
+## Comparing models suing box plot
+ 
+    compareModels_boxplot(predictions["F1 Score"] ,models.index)
+
+
+![](./image/compareModels_boxplot.png)
+
+
+    
+
+
+
 This code updated from github  ["Lazypredic-Shankar Rao Pandala"](https://github.com/shankarpandala/lazypredict)
```

### Comparing `rapidpredict-0.0.0.7/rapidpredict/supervised.py` & `rapidpredict-0.0.0.8/rapidpredict/supervised.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,14 +86,17 @@
         ("encoding", OrdinalEncoder()),
     ]
 )
 
 
 # Helper function
 
+##################################################################
+##                    Helper function                           ##
+##################################################################
 
 def get_card_split(df, cols, n=11):
     """
     Splits categorical columns into 2 lists based on cardinality (i.e # of unique values)
     Parameters
     ----------
     df : Pandas DataFrame
@@ -111,14 +114,17 @@
     """
     cond = df[cols].nunique() > n
     card_high = cols[cond]
     card_low = cols[~cond]
     return card_low, card_high
 
 
+##################################################################
+##                    Class rapidclassifier                     ##
+##################################################################
 
 class rapidclassifier:
 
     def __init__(
         self,
         verbose=0,
         ignore_warnings=True,
@@ -391,34 +397,17 @@
 
         if len(self.models.keys()) == 0:
             self.fit(X_train, X_test, y_train, y_test) 
 
         return self.models
     
 
-
-# class plot_target:
-#     def __init__(self, dataset, target = "target"):
-#         self.dataset = dataset
-#         self.target = target
-#         self.plot()
-
-#     def plot(self):
-#         # Create a DataFrame containing the target column
-#         target_df = pd.DataFrame({self.target: self.dataset})
-#         fig, ax = plt.subplots(figsize=(4, 8))
-#         ax = sns.countplot(x=self.target, data=target_df)
-#         ax.set_title("Target Distribution")
-#         ax.set_xlabel("Target")
-#         ax.set_ylabel("Count")
-#         plt.show()
-
-#     def __repr__(self):
-#         return ''
-
+##################################################################
+##                    Class plot_target                         ##
+##################################################################
 
 class plot_target:
     def __init__(self, dataset, target="target"):
         self.dataset = dataset
         self.target = target
         self.plot()
 
@@ -446,15 +435,17 @@
     def __repr__(self):
         return ''
     
 
 
 
 
-
+##################################################################
+##                  class compareModels_bargraph                ##                    
+##################################################################
 
 
 class compareModels_bargraph:
     def __init__(self, model_names, model_metrics_flscore):
         self.model_names = model_names.to_list()
         self.model_metrics_flscore = model_metrics_flscore.to_list()
         self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_metrics_flscore})
@@ -490,14 +481,18 @@
             return ''
 
 
 
 
 
 
+##################################################################
+##                  class compareModels_boxplot                 ##                    
+##################################################################
+
 class compareModels_boxplot:
     def __init__(self, model_names, model_metrics_flscore):
         self.model_names = model_names.to_list()
         self.model_metrics_flscore = model_metrics_flscore.to_list()
         self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_metrics_flscore})
         self.plot()
 
@@ -570,7 +565,9 @@
 #         for i, row in df_sorted.iterrows():
 #             ax.text(row['F1 Score'], i, f"{row['F1 Score']:.2f}", color='black', ha="left", va="center")
 
 #         # Mention the best result
 #         ax.text(0.98, 0.02, f"Best result: {best_model} ({best_f1:.2f})", transform=ax.transAxes, ha="right", va="bottom", fontsize=12)
 
 #         plt.show()
+
+
```

### Comparing `rapidpredict-0.0.0.7/rapidpredict.egg-info/PKG-INFO` & `rapidpredict-0.0.0.8/rapidpredict.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rapidpredict
-Version: 0.0.0.7
+Version: 0.0.0.8
 Summary: rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.
 Author: Synthetic Dataset AI Team
 Author-email: <nematiusa@gmail.com>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: Free To Use But Restricted
-Requires-Python: >=3.8.1.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 # RapidPredict
 RapidPredict is a Python library that simplifies the process of fitting and evaluating multiple machine learning models from scikit-learn. It's designed to provide a quick way to test various algorithms on a given dataset and compare their performance. 
 
 
@@ -34,26 +34,26 @@
 
 
 
 ## Classification
 
 Example :
 
-    from rapidpredict import classification as rp
-    from sklearn.datasets import load_breast_cancer
+    from rapidpredict.supervised import *
     from sklearn.model_selection import train_test_split
-
+    from sklearn.datasets import load_breast_cancer
     data = load_breast_cancer()
     X = data.data
     y= data.target
 
-    X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.5,random_state =123)
+    X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.25,random_state =123)
 
-    clf = rp(verbose=0,ignore_warnings=True, custom_metric=None)
-    models,predictions = clf.fit(X_train, X_test, y_train, y_test)
+
+    clf = rapidclassifier(verbose= 0,ignore_warnings=True, custom_metric=None)
+    models , predictions = clf.fit(X_train, X_test, y_train, y_test)
 
 
 
     |Model |Accuracy	 |Balanced Accuracy |	ROC | AUC |	Recall |	Precision | F1 Score |	5 Fold F1 |	Time  Taken |
     |-------------------------------|------|------|------|------|------|------|------|------|
     | QuadraticDiscriminantAnalysis | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.96 | 0.09 |
     | RandomForestClassifier        | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.96 | 1.21 |
@@ -80,8 +80,36 @@
     | NearestCentroid               | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.94 | 0.08 |
     | GaussianNB                    | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.94 | 0.08 |
     | ExtraTreeClassifier           | 0.94 | 0.94 | 0.94 | 0.94 | 0.94 | 0.94 | 0.93 | 0.08 |
     | DummyClassifier               | 0.62 | 0.50 | 0.50 | 0.62 | 0.39 | 0.48 | 0.77 | 0.08 |
 
 
 
+## Plot Target values
+
+    plot_target(y)
+
+![plot target](./image/plot_target.png)
+
+
+
+## Comparing models suing bar graph
+ 
+  compareModels_bargraph(predictions["F1 Score"] ,models.index)
+ 
+
+![](./image/compareModels_bargraph.png)  
+
+
+## Comparing models suing box plot
+ 
+    compareModels_boxplot(predictions["F1 Score"] ,models.index)
+
+
+![](./image/compareModels_boxplot.png)
+
+
+    
+
+
+
 This code updated from github  ["Lazypredic-Shankar Rao Pandala"](https://github.com/shankarpandala/lazypredict)
```

### Comparing `rapidpredict-0.0.0.7/setup.py` & `rapidpredict-0.0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.0.7'
+VERSION = '0.0.0.8'
 DESCRIPTION = 'rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.'
 LONG_DESCRIPTION = 'This repository contains a Python-based framework for rapid prediction of machine learning models\
       that simplifies the process of fitting and evaluating multiple machine learning models from scikit-learn.\
           It''s designed to provide a quick way to test various algorithms on a given dataset and compare their performance.'
 
 # Setting up
 setup(
@@ -23,15 +23,15 @@
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=["click", "scikit-learn", "pandas"  , "tqdm" , "joblib", \
                        "lightgbm" ,  "xgboost"  , "itables" ,"catboost" , "colorlover" , "seaborn"\
                           , "plotly" , "IPython"],
     keywords=['python', 'pandas', 'numpy', 'scikit-learn', 'scipy', 'matplotlib', 'seaborn'],
-    python_requires=">=3.8.1.7",
+    python_requires=">=3.7",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

