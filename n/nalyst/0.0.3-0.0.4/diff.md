# Comparing `tmp/nalyst-0.0.3.tar.gz` & `tmp/nalyst-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.0.3.tar", last modified: Fri Apr 14 13:42:18 2023, max compression
+gzip compressed data, was "nalyst-0.0.4.tar", last modified: Fri Apr 14 13:49:14 2023, max compression
```

## Comparing `nalyst-0.0.3.tar` & `nalyst-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:42:18.572354 nalyst-0.0.3/
--rw-rw-rw-   0        0        0      167 2023-04-14 13:22:23.000000 nalyst-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2959 2023-04-14 13:42:18.572354 nalyst-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1864 2023-04-14 13:21:51.000000 nalyst-0.0.3/README.md
--rw-rw-rw-   0        0        0        0 2023-04-14 10:17:56.000000 nalyst-0.0.3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:42:18.563385 nalyst-0.0.3/nalyst/
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.3/nalyst/Decisiontree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.3/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.3/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.3/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.3/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.3/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0        0 2023-04-14 10:17:56.000000 nalyst-0.0.3/nalyst/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.3/nalyst/maxabsscaler.py
--rw-rw-rw-   0        0        0        0 2023-04-14 11:27:16.000000 nalyst-0.0.3/nalyst/minmaxscaler.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.3/nalyst/standardscaler.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:42:18.571358 nalyst-0.0.3/nalyst.egg-info/
--rw-rw-rw-   0        0        0     2959 2023-04-14 13:42:18.000000 nalyst-0.0.3/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-04-14 13:42:18.000000 nalyst-0.0.3/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:42:18.000000 nalyst-0.0.3/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 13:42:18.000000 nalyst-0.0.3/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 13:42:18.000000 nalyst-0.0.3/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 13:42:18.572354 nalyst-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-14 13:40:05.000000 nalyst-0.0.3/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-14 13:20:45.000000 nalyst-0.0.3/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:49:14.975490 nalyst-0.0.4/
+-rw-rw-rw-   0        0        0      301 2023-04-14 13:48:48.000000 nalyst-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2959 2023-04-14 13:49:14.975490 nalyst-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1864 2023-04-14 13:48:26.000000 nalyst-0.0.4/README.md
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:17:56.000000 nalyst-0.0.4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:49:14.971502 nalyst-0.0.4/nalyst/
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.4/nalyst/Decisiontree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.4/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.4/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.4/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.4/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.4/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:17:56.000000 nalyst-0.0.4/nalyst/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.4/nalyst/maxabsscaler.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 11:27:16.000000 nalyst-0.0.4/nalyst/minmaxscaler.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.4/nalyst/standardscaler.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:49:14.974493 nalyst-0.0.4/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     2959 2023-04-14 13:49:14.000000 nalyst-0.0.4/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-04-14 13:49:14.000000 nalyst-0.0.4/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:49:14.000000 nalyst-0.0.4/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-14 13:49:14.000000 nalyst-0.0.4/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 13:49:14.000000 nalyst-0.0.4/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:49:14.976486 nalyst-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-14 13:48:20.000000 nalyst-0.0.4/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-14 13:48:23.000000 nalyst-0.0.4/version.py
```

### Comparing `nalyst-0.0.3/LICENSE` & `nalyst-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.3/PKG-INFO` & `nalyst-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.0.3/README.md` & `nalyst-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.3/nalyst/Decisiontree.py` & `nalyst-0.0.4/nalyst/Decisiontree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.3/nalyst/KMeans.py` & `nalyst-0.0.4/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.3/nalyst/LinearRegression.py` & `nalyst-0.0.4/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.3/nalyst/LogisticRegression.py` & `nalyst-0.0.4/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.3/nalyst/PCA.py` & `nalyst-0.0.4/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.3/nalyst/TestTrainSplit.py` & `nalyst-0.0.4/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.3/nalyst/maxabsscaler.py` & `nalyst-0.0.4/nalyst/maxabsscaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.3/nalyst/standardscaler.py` & `nalyst-0.0.4/nalyst/standardscaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.3/nalyst.egg-info/PKG-INFO` & `nalyst-0.0.4/nalyst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.0.3/setup.py` & `nalyst-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.0.3',
+    version='0.0.4',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

