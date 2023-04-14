# Comparing `tmp/nalyst-0.0.6.tar.gz` & `tmp/nalyst-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.0.6.tar", last modified: Fri Apr 14 14:20:14 2023, max compression
+gzip compressed data, was "nalyst-0.0.7.tar", last modified: Fri Apr 14 14:34:08 2023, max compression
```

## Comparing `nalyst-0.0.6.tar` & `nalyst-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:20:14.977677 nalyst-0.0.6/
--rw-rw-rw-   0        0        0      268 2023-04-14 14:17:30.000000 nalyst-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2959 2023-04-14 14:20:14.977677 nalyst-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1864 2023-04-14 13:48:26.000000 nalyst-0.0.6/README.md
--rw-rw-rw-   0        0        0      499 2023-04-14 14:17:06.000000 nalyst-0.0.6/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:20:14.973690 nalyst-0.0.6/nalyst/
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.6/nalyst/Decisiontree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.6/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.6/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.6/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.6/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.6/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0      499 2023-04-14 14:17:06.000000 nalyst-0.0.6/nalyst/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.6/nalyst/maxabsscaler.py
--rw-rw-rw-   0        0        0        0 2023-04-14 11:27:16.000000 nalyst-0.0.6/nalyst/minmaxscaler.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.6/nalyst/standardscaler.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:20:14.976681 nalyst-0.0.6/nalyst.egg-info/
--rw-rw-rw-   0        0        0     2959 2023-04-14 14:20:14.000000 nalyst-0.0.6/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-04-14 14:20:14.000000 nalyst-0.0.6/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:20:14.000000 nalyst-0.0.6/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 14:20:14.000000 nalyst-0.0.6/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 14:20:14.000000 nalyst-0.0.6/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 14:20:14.977677 nalyst-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-14 14:17:37.000000 nalyst-0.0.6/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-14 14:17:43.000000 nalyst-0.0.6/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:08.587422 nalyst-0.0.7/
+-rw-rw-rw-   0        0        0      307 2023-04-14 14:25:51.000000 nalyst-0.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2959 2023-04-14 14:34:08.587422 nalyst-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1864 2023-04-14 13:48:26.000000 nalyst-0.0.7/README.md
+-rw-rw-rw-   0        0        0      615 2023-04-14 14:24:35.000000 nalyst-0.0.7/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:08.583442 nalyst-0.0.7/nalyst/
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.7/nalyst/Decisiontree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.7/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.7/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.7/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.7/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.7/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0      615 2023-04-14 14:25:23.000000 nalyst-0.0.7/nalyst/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.7/nalyst/maxabsscaler.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 11:27:16.000000 nalyst-0.0.7/nalyst/minmaxscaler.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.7/nalyst/standardscaler.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:34:08.586425 nalyst-0.0.7/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     2959 2023-04-14 14:34:08.000000 nalyst-0.0.7/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-04-14 14:34:08.000000 nalyst-0.0.7/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:34:08.000000 nalyst-0.0.7/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-14 14:34:08.000000 nalyst-0.0.7/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 14:34:08.000000 nalyst-0.0.7/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 14:34:08.588419 nalyst-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-14 14:30:28.000000 nalyst-0.0.7/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-14 14:26:26.000000 nalyst-0.0.7/version.py
```

### Comparing `nalyst-0.0.6/LICENSE` & `nalyst-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.6/PKG-INFO` & `nalyst-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.0.6/README.md` & `nalyst-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.6/nalyst/Decisiontree.py` & `nalyst-0.0.7/nalyst/Decisiontree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.6/nalyst/KMeans.py` & `nalyst-0.0.7/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.6/nalyst/LinearRegression.py` & `nalyst-0.0.7/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.6/nalyst/LogisticRegression.py` & `nalyst-0.0.7/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.6/nalyst/PCA.py` & `nalyst-0.0.7/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.6/nalyst/TestTrainSplit.py` & `nalyst-0.0.7/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.6/nalyst/maxabsscaler.py` & `nalyst-0.0.7/nalyst/maxabsscaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.6/nalyst/standardscaler.py` & `nalyst-0.0.7/nalyst/standardscaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.6/nalyst.egg-info/PKG-INFO` & `nalyst-0.0.7/nalyst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.0.6/setup.py` & `nalyst-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.0.6',
+    version='0.0.7',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

