# Comparing `tmp/rapidpredict-0.0.0.8.tar.gz` & `tmp/rapidpredict-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpredict-0.0.0.8.tar", last modified: Fri Apr 14 02:46:52 2023, max compression
+gzip compressed data, was "rapidpredict-0.0.0.9.tar", last modified: Fri Apr 14 03:43:14 2023, max compression
```

## Comparing `rapidpredict-0.0.0.8.tar` & `rapidpredict-0.0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 02:46:52.335807 rapidpredict-0.0.0.8/
--rw-rw-rw-   0        0        0     5023 2023-04-14 02:46:52.335807 rapidpredict-0.0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4177 2023-04-14 02:44:31.000000 rapidpredict-0.0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 02:46:52.329807 rapidpredict-0.0.0.8/rapidpredict/
--rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.8/rapidpredict/__init__.py
--rw-rw-rw-   0        0        0    22122 2023-04-14 02:14:16.000000 rapidpredict-0.0.0.8/rapidpredict/supervised.py
-drwxrwxrwx   0        0        0        0 2023-04-14 02:46:52.334806 rapidpredict-0.0.0.8/rapidpredict.egg-info/
--rw-rw-rw-   0        0        0     5023 2023-04-14 02:46:52.000000 rapidpredict-0.0.0.8/rapidpredict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-14 02:46:52.000000 rapidpredict-0.0.0.8/rapidpredict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 02:46:52.000000 rapidpredict-0.0.0.8/rapidpredict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-04-14 02:46:52.000000 rapidpredict-0.0.0.8/rapidpredict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 02:46:52.000000 rapidpredict-0.0.0.8/rapidpredict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 02:46:52.335807 rapidpredict-0.0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1806 2023-04-14 02:46:20.000000 rapidpredict-0.0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:43:14.951780 rapidpredict-0.0.0.9/
+-rw-rw-rw-   0        0        0     5488 2023-04-14 03:43:14.951780 rapidpredict-0.0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4635 2023-04-14 03:42:16.000000 rapidpredict-0.0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 03:43:14.935032 rapidpredict-0.0.0.9/rapidpredict/
+-rw-rw-rw-   0        0        0      110 2023-04-10 21:56:52.000000 rapidpredict-0.0.0.9/rapidpredict/__init__.py
+-rw-rw-rw-   0        0        0    21086 2023-04-14 03:34:28.000000 rapidpredict-0.0.0.9/rapidpredict/supervised.py
+drwxrwxrwx   0        0        0        0 2023-04-14 03:43:14.950805 rapidpredict-0.0.0.9/rapidpredict.egg-info/
+-rw-rw-rw-   0        0        0     5488 2023-04-14 03:43:14.000000 rapidpredict-0.0.0.9/rapidpredict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-14 03:43:14.000000 rapidpredict-0.0.0.9/rapidpredict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 03:43:14.000000 rapidpredict-0.0.0.9/rapidpredict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-04-14 03:43:14.000000 rapidpredict-0.0.0.9/rapidpredict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 03:43:14.000000 rapidpredict-0.0.0.9/rapidpredict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 03:43:14.951780 rapidpredict-0.0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1806 2023-04-14 03:43:07.000000 rapidpredict-0.0.0.9/setup.py
```

### Comparing `rapidpredict-0.0.0.8/PKG-INFO` & `rapidpredict-0.0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,104 @@
-Metadata-Version: 2.1
-Name: rapidpredict
-Version: 0.0.0.8
-Summary: rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.
-Author: Synthetic Dataset AI Team
-Author-email: <nematiusa@gmail.com>
-Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: License :: Free To Use But Restricted
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-
-# RapidPredict
-RapidPredict is a Python library that simplifies the process of fitting and evaluating multiple machine learning models from scikit-learn. It's designed to provide a quick way to test various algorithms on a given dataset and compare their performance. 
-
-
-# Installation
-
-To install Rapid Predict from PyPI:
-
-    pip install rapidpredict
-
-# Usage
-
-To use Rapid Predict in a project:
-
-    import rapidpredict
-
-
-
-## Classification
-
-Example :
-
-    from rapidpredict.supervised import *
-    from sklearn.model_selection import train_test_split
-    from sklearn.datasets import load_breast_cancer
-    data = load_breast_cancer()
-    X = data.data
-    y= data.target
-
-    X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.25,random_state =123)
-
-
-    clf = rapidclassifier(verbose= 0,ignore_warnings=True, custom_metric=None)
-    models , predictions = clf.fit(X_train, X_test, y_train, y_test)
-
-
-
-    |Model |Accuracy	 |Balanced Accuracy |	ROC | AUC |	Recall |	Precision | F1 Score |	5 Fold F1 |	Time  Taken |
-    |-------------------------------|------|------|------|------|------|------|------|------|
-    | QuadraticDiscriminantAnalysis | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.96 | 0.09 |
-    | RandomForestClassifier        | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.96 | 1.21 |
-    | LogisticRegression            | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.98 | 0.17 |
-    | ExtraTreesClassifier          | 0.99 | 0.98 | 0.98 | 0.99 | 0.99 | 0.99 | 0.97 | 0.80 |
-    | RidgeClassifier               | 0.99 | 0.98 | 0.98 | 0.99 | 0.99 | 0.99 | 0.96 | 0.13 |
-    | LinearSVC                     | 0.99 | 0.98 | 0.98 | 0.99 | 0.99 | 0.99 | 0.96 | 0.10 |
-    | SVC                           | 0.99 | 0.98 | 0.98 | 0.99 | 0.99 | 0.99 | 0.97 | 0.10 |
-    | RidgeClassifierCV             | 0.99 | 0.98 | 0.98 | 0.99 | 0.99 | 0.99 | 0.96 | 0.17 |
-    | LabelPropagation              | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.94 | 0.17 |
-    | LabelSpreading                | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.96 | 0.19 |
-    | SGDClassifier                 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.97 | 0.09 |
-    | Perceptron                    | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.97 | 0.08 |
-    | KNeighborsClassifier          | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.97 | 0.11 |
-    | DecisionTreeClassifier        | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.93 | 0.09 |
-    | BernoulliNB                   | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.93 | 0.09 |
-    | LinearDiscriminantAnalysis    | 0.98 | 0.97 | 0.97 | 0.98 | 0.98 | 0.98 | 0.96 | 0.14 |
-    | CalibratedClassifierCV        | 0.98 | 0.97 | 0.97 | 0.98 | 0.98 | 0.98 | 0.97 | 0.24 |
-    | AdaBoostClassifier            | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.95 | 0.89 |
-    | PassiveAggressiveClassifier   | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.09 |
-    | XGBClassifier                 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.45 |
-    | BaggingClassifier             | 0.97 | 0.96 | 0.96 | 0.97 | 0.97 | 0.97 | 0.95 | 0.32 |
-    | NuSVC                         | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.95 | 0.12 |
-    | NearestCentroid               | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.94 | 0.08 |
-    | GaussianNB                    | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.94 | 0.08 |
-    | ExtraTreeClassifier           | 0.94 | 0.94 | 0.94 | 0.94 | 0.94 | 0.94 | 0.93 | 0.08 |
-    | DummyClassifier               | 0.62 | 0.50 | 0.50 | 0.62 | 0.39 | 0.48 | 0.77 | 0.08 |
-
-
-
-## Plot Target values
-
-    plot_target(y)
-
-![plot target](./image/plot_target.png)
-
-
-
-## Comparing models suing bar graph
- 
-  compareModels_bargraph(predictions["F1 Score"] ,models.index)
- 
-
-![](./image/compareModels_bargraph.png)  
-
-
-## Comparing models suing box plot
- 
-    compareModels_boxplot(predictions["F1 Score"] ,models.index)
-
-
-![](./image/compareModels_boxplot.png)
-
-
-    
-
-
-
-This code updated from github  ["Lazypredic-Shankar Rao Pandala"](https://github.com/shankarpandala/lazypredict) 
+# RapidPredict
+RapidPredict is a Python library that simplifies the process of fitting and evaluating multiple machine learning models from scikit-learn. It's designed to provide a quick way to test various algorithms on a given dataset and compare their performance. 
+
+
+# Installation
+
+To install Rapid Predict from PyPI:
+
+    pip install rapidpredict
+
+    pip install -U rapidpredict
+
+
+    
+
+# Usage
+
+To use Rapid Predict in a project:
+
+    import rapidpredict
+
+
+
+## Classification
+
+Example :
+
+    from rapidpredict.supervised import *
+    from sklearn.model_selection import train_test_split
+    from sklearn.datasets import load_breast_cancer
+    data = load_breast_cancer()
+    X = data.data
+    y= data.target
+
+    X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.25,random_state =123)
+
+
+    clf = rapidclassifier(verbose= 0,ignore_warnings=True, custom_metric=None)
+    models , predictions = clf.fit(X_train, X_test, y_train, y_test)
+
+
+
+    |Model |Accuracy	 |Balanced Accuracy |	ROC | AUC |	Recall |	Precision | F1 Score |	5 Fold F1 |	Time  Taken |
+    |-------------------------------|------|------|------|------|------|------|------|------|
+    | QuadraticDiscriminantAnalysis | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.96 | 0.09 |
+    | RandomForestClassifier        | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.96 | 1.21 |
+    | LogisticRegression            | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.99 | 0.98 | 0.17 |
+    | ExtraTreesClassifier          | 0.99 | 0.98 | 0.98 | 0.99 | 0.99 | 0.99 | 0.97 | 0.80 |
+    | RidgeClassifier               | 0.99 | 0.98 | 0.98 | 0.99 | 0.99 | 0.99 | 0.96 | 0.13 |
+    | LinearSVC                     | 0.99 | 0.98 | 0.98 | 0.99 | 0.99 | 0.99 | 0.96 | 0.10 |
+    | SVC                           | 0.99 | 0.98 | 0.98 | 0.99 | 0.99 | 0.99 | 0.97 | 0.10 |
+    | RidgeClassifierCV             | 0.99 | 0.98 | 0.98 | 0.99 | 0.99 | 0.99 | 0.96 | 0.17 |
+    | LabelPropagation              | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.94 | 0.17 |
+    | LabelSpreading                | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.96 | 0.19 |
+    | SGDClassifier                 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.97 | 0.09 |
+    | Perceptron                    | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.97 | 0.08 |
+    | KNeighborsClassifier          | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.97 | 0.11 |
+    | DecisionTreeClassifier        | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.93 | 0.09 |
+    | BernoulliNB                   | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.98 | 0.93 | 0.09 |
+    | LinearDiscriminantAnalysis    | 0.98 | 0.97 | 0.97 | 0.98 | 0.98 | 0.98 | 0.96 | 0.14 |
+    | CalibratedClassifierCV        | 0.98 | 0.97 | 0.97 | 0.98 | 0.98 | 0.98 | 0.97 | 0.24 |
+    | AdaBoostClassifier            | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.95 | 0.89 |
+    | PassiveAggressiveClassifier   | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.09 |
+    | XGBClassifier                 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.97 | 0.45 |
+    | BaggingClassifier             | 0.97 | 0.96 | 0.96 | 0.97 | 0.97 | 0.97 | 0.95 | 0.32 |
+    | NuSVC                         | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.95 | 0.12 |
+    | NearestCentroid               | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.94 | 0.08 |
+    | GaussianNB                    | 0.97 | 0.95 | 0.95 | 0.97 | 0.97 | 0.96 | 0.94 | 0.08 |
+    | ExtraTreeClassifier           | 0.94 | 0.94 | 0.94 | 0.94 | 0.94 | 0.94 | 0.93 | 0.08 |
+    | DummyClassifier               | 0.62 | 0.50 | 0.50 | 0.62 | 0.39 | 0.48 | 0.77 | 0.08 |
+
+
+
+## Plot Target values
+
+    plot_target(y)
+
+![plot target](https://raw.githubusercontent.com/syntheticdataset/rapidpredict/main/image/plot_target.png)
+
+
+
+## Comparing models using bar graph
+ 
+  compareModels_bargraph(predictions["F1 Score"] ,models.index)
+ 
+
+![Comparing models using bar graph](https://raw.githubusercontent.com/syntheticdataset/rapidpredict/main/image/compareModels_bargraph.png)  
+
+
+## Comparing models using box plot
+ 
+    compareModels_boxplot(predictions["F1 Score"] ,models.index)
+
+
+![Comparing models using box plot](https://raw.githubusercontent.com/syntheticdataset/rapidpredict/main/image/compareModels_boxplot.png)
+
+
+## Heatmap
+
+![heatmap Half Heatmap of Pearson Correlations](https://raw.githubusercontent.com/syntheticdataset/rapidpredict/main/image/heatmap.png)    
+
+
+
+This code updated from github  ["Lazypredic-Shankar Rao Pandala"](https://github.com/shankarpandala/lazypredict)
```

### Comparing `rapidpredict-0.0.0.8/rapidpredict/supervised.py` & `rapidpredict-0.0.0.9/rapidpredict/supervised.py`

 * *Files 4% similar despite different names*

```diff
@@ -450,15 +450,15 @@
         self.model_metrics_flscore = model_metrics_flscore.to_list()
         self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_metrics_flscore})
         self.plot()
 
     def plot(self):
         df_sorted = self.df.sort_values('F1 Score', ascending=True)
 
-        fig, ax = plt.subplots(figsize=(16, 8))
+        fig, ax = plt.subplots(figsize=(14, 7))
 
         # Generate an array of 26 different colors using a colormap
         colormap = plt.cm.get_cmap("tab20", 26)
         colors = colormap(np.arange(26))
 
         # Pass the colors array to the barh function
         bars = ax.barh(df_sorted['F1 Score'], df_sorted['Model'], color=colors)
@@ -495,15 +495,15 @@
         self.model_metrics_flscore = model_metrics_flscore.to_list()
         self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_metrics_flscore})
         self.plot()
 
     def plot(self):
         df_sorted = self.df.sort_values('F1 Score', ascending=True)
 
-        fig, ax =plt.subplots(figsize=(10, 4)) 
+        fig, ax =plt.subplots(figsize=(14, 7)) 
 
         # Generate an array of 26 different colors using a colormap
         colormap = plt.cm.get_cmap("tab20", 26)
         colors = colormap(np.arange(26))
 
         # Create a custom boxplot with seaborn
         sns.boxplot(x='F1 Score', y='Model', data=df_sorted, palette=colors[:len(self.model_names)], ax=ax )
@@ -519,55 +519,35 @@
 
 
         plt.show()
         def __repr__(self):
         # Return an empty string or a custom message
             return ''
 
-
-
-# import matplotlib.pyplot as plt
-# import pandas as pd
-# import numpy as np
-# import seaborn as sns
-
-# class CompareModel_boxplot:
-#     def __init__(self, model_names, model_accuracies):
-#         self.model_names = model_names.to_list()
-#         self.model_accuracies = model_accuracies.to_list()
-#         self.df = pd.DataFrame({'Model': self.model_names, 'F1 Score': self.model_accuracies})
-#         self.plot()
-
-#     def plot(self):
-#         self.df['F1 Score'] = pd.to_numeric(self.df['F1 Score'])  # Convert F1 Score column to numeric data type
-
-#         df_sorted = self.df.sort_values('F1 Score', ascending=True)
-#         best_f1 = df_sorted['F1 Score'].max()
-#         best_model_idx = df_sorted['F1 Score'].idxmax()
-#         best_model = df_sorted.loc[best_model_idx]['Model']
-
-#         fig, ax = plt.subplots(figsize=(12, 6))  # Increase the figure size
-
-#         # Generate an array of 26 different colors using a colormap
-#         colormap = plt.cm.get_cmap("tab20", 26)
-#         colors = colormap(np.arange(26))
-
-#         # Create a custom boxplot with seaborn
-#         sns.boxplot(x='F1 Score', y='Model', data=df_sorted, palette=colors[:len(self.model_names)], ax=ax)
-
-#         ax.set_title('Model Accuracies')
-#         ax.set_xlabel('F1 Score')
-#         ax.set_ylabel('Model')
-
-#         # Rotate the xtick labels by 90 degrees
-#         ax.set_xticklabels(ax.get_xticks(), rotation=90)
-
-#         # Add accuracies to the plot
-#         for i, row in df_sorted.iterrows():
-#             ax.text(row['F1 Score'], i, f"{row['F1 Score']:.2f}", color='black', ha="left", va="center")
-
-#         # Mention the best result
-#         ax.text(0.98, 0.02, f"Best result: {best_model} ({best_f1:.2f})", transform=ax.transAxes, ha="right", va="bottom", fontsize=12)
-
-#         plt.show()
-
+##################################################################
+class heatmap:
+    def __init__(self, X, y):
+        self.X = X
+        self.y = y
+        self.plot_heatmap()
+
+    def plot_heatmap(self):
+        df = pd.DataFrame(self.X)
+        corr_matrix = df.corr()
+
+        # Create a mask for the upper triangle
+        mask = np.triu(np.ones_like(corr_matrix, dtype=bool))
+        w =20
+        h = 20
+        plt.figure(figsize=( w, h))
+        sns.heatmap(
+            corr_matrix,
+            annot=True,
+            cmap="coolwarm",
+            linewidths=0.5,
+            square=True,
+            cbar_kws={"shrink": 0.5},
+            mask=mask  # Apply the mask to display only the lower triangle
+        )
+        plt.title("Half Heatmap of Pearson Correlations")
+        plt.show()
```

### Comparing `rapidpredict-0.0.0.8/rapidpredict.egg-info/PKG-INFO` & `rapidpredict-0.0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpredict
-Version: 0.0.0.8
+Version: 0.0.0.9
 Summary: rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.
 Author: Synthetic Dataset AI Team
 Author-email: <nematiusa@gmail.com>
 Keywords: python,pandas,numpy,scikit-learn,scipy,matplotlib,seaborn
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,19 @@
 
 # Installation
 
 To install Rapid Predict from PyPI:
 
     pip install rapidpredict
 
+    pip install -U rapidpredict
+
+
+    
+
 # Usage
 
 To use Rapid Predict in a project:
 
     import rapidpredict
 
 
@@ -84,32 +89,34 @@
 
 
 
 ## Plot Target values
 
     plot_target(y)
 
-![plot target](./image/plot_target.png)
+![plot target](https://raw.githubusercontent.com/syntheticdataset/rapidpredict/main/image/plot_target.png)
 
 
 
-## Comparing models suing bar graph
+## Comparing models using bar graph
  
   compareModels_bargraph(predictions["F1 Score"] ,models.index)
  
 
-![](./image/compareModels_bargraph.png)  
+![Comparing models using bar graph](https://raw.githubusercontent.com/syntheticdataset/rapidpredict/main/image/compareModels_bargraph.png)  
 
 
-## Comparing models suing box plot
+## Comparing models using box plot
  
     compareModels_boxplot(predictions["F1 Score"] ,models.index)
 
 
-![](./image/compareModels_boxplot.png)
+![Comparing models using box plot](https://raw.githubusercontent.com/syntheticdataset/rapidpredict/main/image/compareModels_boxplot.png)
 
 
-    
+## Heatmap
+
+![heatmap Half Heatmap of Pearson Correlations](https://raw.githubusercontent.com/syntheticdataset/rapidpredict/main/image/heatmap.png)    
 
 
 
 This code updated from github  ["Lazypredic-Shankar Rao Pandala"](https://github.com/shankarpandala/lazypredict)
```

### Comparing `rapidpredict-0.0.0.8/setup.py` & `rapidpredict-0.0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.0.8'
+VERSION = '0.0.0.9'
 DESCRIPTION = 'rapid predict is a python package to simplifies the process of fitting and evaluating multiple machine learning models on a dataset.'
 LONG_DESCRIPTION = 'This repository contains a Python-based framework for rapid prediction of machine learning models\
       that simplifies the process of fitting and evaluating multiple machine learning models from scikit-learn.\
           It''s designed to provide a quick way to test various algorithms on a given dataset and compare their performance.'
 
 # Setting up
 setup(
```

