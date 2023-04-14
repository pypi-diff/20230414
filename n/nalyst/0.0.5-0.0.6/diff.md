# Comparing `tmp/nalyst-0.0.5.tar.gz` & `tmp/nalyst-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.0.5.tar", last modified: Fri Apr 14 13:55:25 2023, max compression
+gzip compressed data, was "nalyst-0.0.6.tar", last modified: Fri Apr 14 14:20:14 2023, max compression
```

## Comparing `nalyst-0.0.5.tar` & `nalyst-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:55:25.244620 nalyst-0.0.5/
--rw-rw-rw-   0        0        0      229 2023-04-14 13:55:01.000000 nalyst-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2959 2023-04-14 13:55:25.243624 nalyst-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1864 2023-04-14 13:48:26.000000 nalyst-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 13:55:25.240634 nalyst-0.0.5/nalyst/
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.5/nalyst/Decisiontree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.5/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.5/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.5/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.5/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.5/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0        0 2023-04-14 10:17:56.000000 nalyst-0.0.5/nalyst/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.5/nalyst/maxabsscaler.py
--rw-rw-rw-   0        0        0        0 2023-04-14 11:27:16.000000 nalyst-0.0.5/nalyst/minmaxscaler.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.5/nalyst/standardscaler.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:55:25.243624 nalyst-0.0.5/nalyst.egg-info/
--rw-rw-rw-   0        0        0     2959 2023-04-14 13:55:25.000000 nalyst-0.0.5/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-04-14 13:55:25.000000 nalyst-0.0.5/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:55:25.000000 nalyst-0.0.5/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 13:55:25.000000 nalyst-0.0.5/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 13:55:25.000000 nalyst-0.0.5/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 13:55:25.244620 nalyst-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-14 13:54:20.000000 nalyst-0.0.5/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-14 13:54:11.000000 nalyst-0.0.5/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:20:14.977677 nalyst-0.0.6/
+-rw-rw-rw-   0        0        0      268 2023-04-14 14:17:30.000000 nalyst-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2959 2023-04-14 14:20:14.977677 nalyst-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1864 2023-04-14 13:48:26.000000 nalyst-0.0.6/README.md
+-rw-rw-rw-   0        0        0      499 2023-04-14 14:17:06.000000 nalyst-0.0.6/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:20:14.973690 nalyst-0.0.6/nalyst/
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.6/nalyst/Decisiontree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.6/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.6/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.6/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.6/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.6/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0      499 2023-04-14 14:17:06.000000 nalyst-0.0.6/nalyst/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.6/nalyst/maxabsscaler.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 11:27:16.000000 nalyst-0.0.6/nalyst/minmaxscaler.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.6/nalyst/standardscaler.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:20:14.976681 nalyst-0.0.6/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     2959 2023-04-14 14:20:14.000000 nalyst-0.0.6/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-04-14 14:20:14.000000 nalyst-0.0.6/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:20:14.000000 nalyst-0.0.6/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-14 14:20:14.000000 nalyst-0.0.6/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 14:20:14.000000 nalyst-0.0.6/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 14:20:14.977677 nalyst-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-14 14:17:37.000000 nalyst-0.0.6/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-14 14:17:43.000000 nalyst-0.0.6/version.py
```

### Comparing `nalyst-0.0.5/LICENSE` & `nalyst-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.5/PKG-INFO` & `nalyst-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.0.5/README.md` & `nalyst-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.5/nalyst/Decisiontree.py` & `nalyst-0.0.6/nalyst/Decisiontree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.5/nalyst/KMeans.py` & `nalyst-0.0.6/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.5/nalyst/LinearRegression.py` & `nalyst-0.0.6/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.5/nalyst/LogisticRegression.py` & `nalyst-0.0.6/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.5/nalyst/PCA.py` & `nalyst-0.0.6/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.5/nalyst/TestTrainSplit.py` & `nalyst-0.0.6/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.5/nalyst/maxabsscaler.py` & `nalyst-0.0.6/nalyst/maxabsscaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.5/nalyst/standardscaler.py` & `nalyst-0.0.6/nalyst/standardscaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.5/nalyst.egg-info/PKG-INFO` & `nalyst-0.0.6/nalyst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `nalyst-0.0.5/setup.py` & `nalyst-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.0.5',
+    version='0.0.6',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
```

