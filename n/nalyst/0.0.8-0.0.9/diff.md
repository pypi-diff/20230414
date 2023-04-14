# Comparing `tmp/nalyst-0.0.8.tar.gz` & `tmp/nalyst-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.0.8.tar", last modified: Fri Apr 14 14:56:43 2023, max compression
+gzip compressed data, was "nalyst-0.0.9.tar", last modified: Fri Apr 14 15:13:36 2023, max compression
```

## Comparing `nalyst-0.0.8.tar` & `nalyst-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:56:43.895794 nalyst-0.0.8/
--rw-rw-rw-   0        0        0      346 2023-04-14 14:55:50.000000 nalyst-0.0.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2959 2023-04-14 14:56:43.895794 nalyst-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1864 2023-04-14 13:48:26.000000 nalyst-0.0.8/README.md
--rw-rw-rw-   0        0        0      615 2023-04-14 14:52:42.000000 nalyst-0.0.8/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:56:43.889815 nalyst-0.0.8/nalyst/
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.8/nalyst/Decisiontree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.8/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.8/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.8/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.8/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.8/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0      615 2023-04-14 14:52:37.000000 nalyst-0.0.8/nalyst/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.8/nalyst/maxabsscaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.0.8/nalyst/minmaxscaler.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.8/nalyst/standardscaler.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:56:43.894799 nalyst-0.0.8/nalyst.egg-info/
--rw-rw-rw-   0        0        0     2959 2023-04-14 14:56:43.000000 nalyst-0.0.8/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-04-14 14:56:43.000000 nalyst-0.0.8/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:56:43.000000 nalyst-0.0.8/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 14:56:43.000000 nalyst-0.0.8/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 14:56:43.000000 nalyst-0.0.8/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 14:56:43.895794 nalyst-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-14 14:55:28.000000 nalyst-0.0.8/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-14 14:55:34.000000 nalyst-0.0.8/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:13:36.632613 nalyst-0.0.9/
+-rw-rw-rw-   0        0        0      385 2023-04-14 15:10:45.000000 nalyst-0.0.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2959 2023-04-14 15:13:36.632613 nalyst-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1864 2023-04-14 13:48:26.000000 nalyst-0.0.9/README.md
+-rw-rw-rw-   0        0        0      655 2023-04-14 15:12:51.000000 nalyst-0.0.9/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:13:36.627124 nalyst-0.0.9/nalyst/
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.9/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.9/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.9/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.9/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.9/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.0.9/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.9/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.9/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.9/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0      655 2023-04-14 15:12:49.000000 nalyst-0.0.9/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:13:36.631111 nalyst-0.0.9/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     2959 2023-04-14 15:13:36.000000 nalyst-0.0.9/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-04-14 15:13:36.000000 nalyst-0.0.9/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 15:13:36.000000 nalyst-0.0.9/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-14 15:13:36.000000 nalyst-0.0.9/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 15:13:36.000000 nalyst-0.0.9/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 15:13:36.632613 nalyst-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-14 15:13:08.000000 nalyst-0.0.9/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-14 15:12:46.000000 nalyst-0.0.9/version.py
```

### Comparing `nalyst-0.0.8/LICENSE` & `nalyst-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/PKG-INFO` & `nalyst-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.0.8/README.md` & `nalyst-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/__init__.py` & `nalyst-0.0.9/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from nalyst.LinearRegression import LinearRegression
-from nalyst.Decisiontree import DecisionTree
+from nalyst.LinearRegression import LinearRegression, mse, rmse, r_squared
+from nalyst.DecisionTree import DecisionTree, Node
 from nalyst.KMeans import KMeans
 from nalyst.PCA import PCA
-from nalyst.LogisticRegression import LogisticRegression
-from nalyst.maxabsscaler import MaxAbsScaler
-from nalyst.minmaxscaler import MinMaxScaler
-from nalyst.standardscaler import StandardScaler
+from nalyst.LogisticRegression import LogisticRegression, accuracy
+from nalyst.MaxAbsScaler import MaxAbsScaler
+from nalyst.MinMaxScaler import MinMaxScaler
+from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
+
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
-    'maxabsscaler',
-    'minmaxscaler',
-    'standardscaler',
+    'MaxAbsScaler',
+    'MinMaxScaler',
+    'StandardScaler',
     'TestTrainSplit'
 ]
```

### Comparing `nalyst-0.0.8/nalyst/Decisiontree.py` & `nalyst-0.0.9/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/nalyst/KMeans.py` & `nalyst-0.0.9/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/nalyst/LinearRegression.py` & `nalyst-0.0.9/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/nalyst/LogisticRegression.py` & `nalyst-0.0.9/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/nalyst/PCA.py` & `nalyst-0.0.9/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/nalyst/TestTrainSplit.py` & `nalyst-0.0.9/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/nalyst/__init__.py` & `nalyst-0.0.9/nalyst/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from nalyst.LinearRegression import LinearRegression
-from nalyst.Decisiontree import DecisionTree
+from nalyst.LinearRegression import LinearRegression, mse, rmse, r_squared
+from nalyst.DecisionTree import DecisionTree, Node
 from nalyst.KMeans import KMeans
 from nalyst.PCA import PCA
-from nalyst.LogisticRegression import LogisticRegression
-from nalyst.maxabsscaler import MaxAbsScaler
-from nalyst.minmaxscaler import MinMaxScaler
-from nalyst.standardscaler import StandardScaler
+from nalyst.LogisticRegression import LogisticRegression, accuracy
+from nalyst.MaxAbsScaler import MaxAbsScaler
+from nalyst.MinMaxScaler import MinMaxScaler
+from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
+
 __all__ = [
     'LinearRegression',
     'DecisionTree',
     'KMeans',
     'PCA',
     'LogisticRegression',
-    'maxabsscaler',
-    'minmaxscaler',
-    'standardscaler',
+    'MaxAbsScaler',
+    'MinMaxScaler',
+    'StandardScaler',
     'TestTrainSplit'
 ]
```

### Comparing `nalyst-0.0.8/nalyst/maxabsscaler.py` & `nalyst-0.0.9/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/nalyst/minmaxscaler.py` & `nalyst-0.0.9/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/nalyst/standardscaler.py` & `nalyst-0.0.9/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.8/nalyst.egg-info/PKG-INFO` & `nalyst-0.0.9/nalyst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.0.8/setup.py` & `nalyst-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.0.8',
+    version='0.0.9',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

