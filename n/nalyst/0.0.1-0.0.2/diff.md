# Comparing `tmp/nalyst-0.0.1.tar.gz` & `tmp/nalyst-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.0.1.tar", last modified: Fri Apr 14 12:14:13 2023, max compression
+gzip compressed data, was "nalyst-0.0.2.tar", last modified: Fri Apr 14 13:22:39 2023, max compression
```

## Comparing `nalyst-0.0.1.tar` & `nalyst-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:14:13.991989 nalyst-0.0.1/
--rw-rw-rw-   0        0        0      101 2023-04-14 10:17:56.000000 nalyst-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2565 2023-04-14 12:14:13.991989 nalyst-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1601 2023-04-14 12:04:52.000000 nalyst-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 12:14:13.983019 nalyst-0.0.1/nalyst.egg-info/
--rw-rw-rw-   0        0        0     2565 2023-04-14 12:14:13.000000 nalyst-0.0.1/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-04-14 12:14:13.000000 nalyst-0.0.1/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:14:13.000000 nalyst-0.0.1/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 12:14:13.000000 nalyst-0.0.1/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:14:13.000000 nalyst-0.0.1/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 12:14:13.991989 nalyst-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-04-14 12:05:36.000000 nalyst-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:14:13.964082 nalyst-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 12:14:13.990992 nalyst-0.0.1/src/nalyst/
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.1/src/nalyst/Decisiontree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.1/src/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.1/src/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.1/src/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.1/src/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.1/src/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0        0 2023-04-14 10:17:56.000000 nalyst-0.0.1/src/nalyst/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.1/src/nalyst/maxabsscaler.py
--rw-rw-rw-   0        0        0        0 2023-04-14 11:27:16.000000 nalyst-0.0.1/src/nalyst/minmaxscaler.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.1/src/nalyst/standardscaler.py
--rw-rw-rw-   0        0        0       17 2023-04-14 10:17:56.000000 nalyst-0.0.1/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:22:39.474869 nalyst-0.0.2/
+-rw-rw-rw-   0        0        0      167 2023-04-14 13:22:23.000000 nalyst-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2830 2023-04-14 13:22:39.473872 nalyst-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1864 2023-04-14 13:21:51.000000 nalyst-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 13:22:39.461913 nalyst-0.0.2/nalyst/
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.2/nalyst/Decisiontree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.2/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.2/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.2/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.2/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.2/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:17:56.000000 nalyst-0.0.2/nalyst/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.2/nalyst/maxabsscaler.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 11:27:16.000000 nalyst-0.0.2/nalyst/minmaxscaler.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.2/nalyst/standardscaler.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:22:39.472876 nalyst-0.0.2/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     2830 2023-04-14 13:22:39.000000 nalyst-0.0.2/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-04-14 13:22:39.000000 nalyst-0.0.2/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:22:39.000000 nalyst-0.0.2/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-14 13:22:39.000000 nalyst-0.0.2/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 13:22:39.000000 nalyst-0.0.2/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:22:39.474869 nalyst-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-04-14 13:20:47.000000 nalyst-0.0.2/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-14 13:20:45.000000 nalyst-0.0.2/version.py
```

### Comparing `nalyst-0.0.1/LICENSE` & `nalyst-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.1/PKG-INFO` & `nalyst-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -19,17 +19,19 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 NALYST
 
+
+
 INTRODUCTION
 
-This library is designed for professionals and researchers in the field of Machine Learning. It provides a comprehensive suite of tools for Linear Regression, Logistic Regression, Train Test Split, Min Max Scale, and Standard Scale. With this library, users can quickly train their model
+Nalyst is a powerful and user-friendly library designed for data analysts, professionals, and researchers in the field of Machine Learning and Data Science. It provides a comprehensive suite of tools for various tasks, such as Linear Regression, Logistic Regression, K-means Clustering, Principal Component Analysis (PCA), Decision Trees, Train Test Split, Min Max Scaling, MaxAbs Scaling, and Standard Scaling. With Nalyst, users can quickly and efficiently train, analyze, and evaluate their models, streamlining the entire data analysis process.
 
 FEATURES
 
 Linear Regression: a comprehensive set of tools for building and analyzing linear regression models.
 
 Logistic Regression: a range of tools for building and analyzing logistic regression models.
```

### Comparing `nalyst-0.0.1/README.md` & `nalyst-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 NALYST
 
+
+
 INTRODUCTION
 
-This library is designed for professionals and researchers in the field of Machine Learning. It provides a comprehensive suite of tools for Linear Regression, Logistic Regression, Train Test Split, Min Max Scale, and Standard Scale. With this library, users can quickly train their model
+Nalyst is a powerful and user-friendly library designed for data analysts, professionals, and researchers in the field of Machine Learning and Data Science. It provides a comprehensive suite of tools for various tasks, such as Linear Regression, Logistic Regression, K-means Clustering, Principal Component Analysis (PCA), Decision Trees, Train Test Split, Min Max Scaling, MaxAbs Scaling, and Standard Scaling. With Nalyst, users can quickly and efficiently train, analyze, and evaluate their models, streamlining the entire data analysis process.
 
 FEATURES
 
 Linear Regression: a comprehensive set of tools for building and analyzing linear regression models.
 
 Logistic Regression: a range of tools for building and analyzing logistic regression models.
```

### Comparing `nalyst-0.0.1/nalyst.egg-info/PKG-INFO` & `nalyst-0.0.2/nalyst.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -19,17 +19,19 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 NALYST
 
+
+
 INTRODUCTION
 
-This library is designed for professionals and researchers in the field of Machine Learning. It provides a comprehensive suite of tools for Linear Regression, Logistic Regression, Train Test Split, Min Max Scale, and Standard Scale. With this library, users can quickly train their model
+Nalyst is a powerful and user-friendly library designed for data analysts, professionals, and researchers in the field of Machine Learning and Data Science. It provides a comprehensive suite of tools for various tasks, such as Linear Regression, Logistic Regression, K-means Clustering, Principal Component Analysis (PCA), Decision Trees, Train Test Split, Min Max Scaling, MaxAbs Scaling, and Standard Scaling. With Nalyst, users can quickly and efficiently train, analyze, and evaluate their models, streamlining the entire data analysis process.
 
 FEATURES
 
 Linear Regression: a comprehensive set of tools for building and analyzing linear regression models.
 
 Logistic Regression: a range of tools for building and analyzing logistic regression models.
```

### Comparing `nalyst-0.0.1/setup.py` & `nalyst-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.0.1',
+    version='0.0.2',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

### Comparing `nalyst-0.0.1/src/nalyst/Decisiontree.py` & `nalyst-0.0.2/nalyst/Decisiontree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.1/src/nalyst/KMeans.py` & `nalyst-0.0.2/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.1/src/nalyst/LinearRegression.py` & `nalyst-0.0.2/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.1/src/nalyst/LogisticRegression.py` & `nalyst-0.0.2/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.1/src/nalyst/PCA.py` & `nalyst-0.0.2/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.1/src/nalyst/TestTrainSplit.py` & `nalyst-0.0.2/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.1/src/nalyst/maxabsscaler.py` & `nalyst-0.0.2/nalyst/maxabsscaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.1/src/nalyst/standardscaler.py` & `nalyst-0.0.2/nalyst/standardscaler.py`

 * *Files identical despite different names*

