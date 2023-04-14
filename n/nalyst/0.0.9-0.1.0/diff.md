# Comparing `tmp/nalyst-0.0.9.tar.gz` & `tmp/nalyst-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.0.9.tar", last modified: Fri Apr 14 15:13:36 2023, max compression
+gzip compressed data, was "nalyst-0.1.0.tar", last modified: Fri Apr 14 15:23:22 2023, max compression
```

## Comparing `nalyst-0.0.9.tar` & `nalyst-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 15:13:36.632613 nalyst-0.0.9/
--rw-rw-rw-   0        0        0      385 2023-04-14 15:10:45.000000 nalyst-0.0.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.9/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2959 2023-04-14 15:13:36.632613 nalyst-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1864 2023-04-14 13:48:26.000000 nalyst-0.0.9/README.md
--rw-rw-rw-   0        0        0      655 2023-04-14 15:12:51.000000 nalyst-0.0.9/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:13:36.627124 nalyst-0.0.9/nalyst/
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.9/nalyst/DecisionTree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.9/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.9/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.9/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.9/nalyst/MaxAbsScaler.py
--rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.0.9/nalyst/MinMaxScaler.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.9/nalyst/PCA.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.9/nalyst/StandardScaler.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.9/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0      655 2023-04-14 15:12:49.000000 nalyst-0.0.9/nalyst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:13:36.631111 nalyst-0.0.9/nalyst.egg-info/
--rw-rw-rw-   0        0        0     2959 2023-04-14 15:13:36.000000 nalyst-0.0.9/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-04-14 15:13:36.000000 nalyst-0.0.9/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 15:13:36.000000 nalyst-0.0.9/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 15:13:36.000000 nalyst-0.0.9/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 15:13:36.000000 nalyst-0.0.9/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 15:13:36.632613 nalyst-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-14 15:13:08.000000 nalyst-0.0.9/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-14 15:12:46.000000 nalyst-0.0.9/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:23:22.705200 nalyst-0.1.0/
+-rw-rw-rw-   0        0        0      424 2023-04-14 15:22:55.000000 nalyst-0.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 15:13:14.000000 nalyst-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2959 2023-04-14 15:23:22.704203 nalyst-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1864 2023-04-14 13:48:26.000000 nalyst-0.1.0/README.md
+-rw-rw-rw-   0        0        0      655 2023-04-14 15:12:51.000000 nalyst-0.1.0/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:23:22.695105 nalyst-0.1.0/nalyst/
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.1.0/nalyst/DecisionTree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.1.0/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3546 2023-04-14 15:21:33.000000 nalyst-0.1.0/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.1.0/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.1.0/nalyst/MaxAbsScaler.py
+-rw-rw-rw-   0        0        0     2195 2023-04-14 14:52:15.000000 nalyst-0.1.0/nalyst/MinMaxScaler.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.1.0/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.1.0/nalyst/StandardScaler.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.1.0/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0      581 2023-04-14 15:21:58.000000 nalyst-0.1.0/nalyst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:23:22.703088 nalyst-0.1.0/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     2959 2023-04-14 15:23:22.000000 nalyst-0.1.0/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-04-14 15:23:22.000000 nalyst-0.1.0/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 15:23:22.000000 nalyst-0.1.0/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-14 15:23:22.000000 nalyst-0.1.0/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 15:23:22.000000 nalyst-0.1.0/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 15:23:22.705200 nalyst-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-14 15:22:21.000000 nalyst-0.1.0/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-14 15:22:15.000000 nalyst-0.1.0/version.py
```

### Comparing `nalyst-0.0.9/LICENSE` & `nalyst-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/PKG-INFO` & `nalyst-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.9
+Version: 0.1.0
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.0.9/README.md` & `nalyst-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/__init__.py` & `nalyst-0.1.0/__init__.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/nalyst/DecisionTree.py` & `nalyst-0.1.0/nalyst/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/nalyst/KMeans.py` & `nalyst-0.1.0/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/nalyst/LinearRegression.py` & `nalyst-0.1.0/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/nalyst/LogisticRegression.py` & `nalyst-0.1.0/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/nalyst/MaxAbsScaler.py` & `nalyst-0.1.0/nalyst/MaxAbsScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/nalyst/MinMaxScaler.py` & `nalyst-0.1.0/nalyst/MinMaxScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/nalyst/PCA.py` & `nalyst-0.1.0/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/nalyst/StandardScaler.py` & `nalyst-0.1.0/nalyst/StandardScaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/nalyst/TestTrainSplit.py` & `nalyst-0.1.0/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.9/nalyst/__init__.py` & `nalyst-0.1.0/nalyst/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from nalyst.LinearRegression import LinearRegression, mse, rmse, r_squared
-from nalyst.DecisionTree import DecisionTree, Node
+from nalyst.LinearRegression import LinearRegression
 from nalyst.KMeans import KMeans
 from nalyst.PCA import PCA
 from nalyst.LogisticRegression import LogisticRegression, accuracy
 from nalyst.MaxAbsScaler import MaxAbsScaler
 from nalyst.MinMaxScaler import MinMaxScaler
 from nalyst.StandardScaler import StandardScaler
 from nalyst.TestTrainSplit import TrainTestSplit
```

### Comparing `nalyst-0.0.9/nalyst.egg-info/PKG-INFO` & `nalyst-0.1.0/nalyst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.9
+Version: 0.1.0
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.0.9/setup.py` & `nalyst-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.0.9',
+    version='0.1.0',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

