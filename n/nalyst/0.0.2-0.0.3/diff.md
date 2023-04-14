# Comparing `tmp/nalyst-0.0.2.tar.gz` & `tmp/nalyst-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nalyst-0.0.2.tar", last modified: Fri Apr 14 13:22:39 2023, max compression
+gzip compressed data, was "nalyst-0.0.3.tar", last modified: Fri Apr 14 13:42:18 2023, max compression
```

## Comparing `nalyst-0.0.2.tar` & `nalyst-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:22:39.474869 nalyst-0.0.2/
--rw-rw-rw-   0        0        0      167 2023-04-14 13:22:23.000000 nalyst-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2830 2023-04-14 13:22:39.473872 nalyst-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1864 2023-04-14 13:21:51.000000 nalyst-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 13:22:39.461913 nalyst-0.0.2/nalyst/
--rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.2/nalyst/Decisiontree.py
--rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.2/nalyst/KMeans.py
--rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.2/nalyst/LinearRegression.py
--rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.2/nalyst/LogisticRegression.py
--rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.2/nalyst/PCA.py
--rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.2/nalyst/TestTrainSplit.py
--rw-rw-rw-   0        0        0        0 2023-04-14 10:17:56.000000 nalyst-0.0.2/nalyst/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.2/nalyst/maxabsscaler.py
--rw-rw-rw-   0        0        0        0 2023-04-14 11:27:16.000000 nalyst-0.0.2/nalyst/minmaxscaler.py
--rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.2/nalyst/standardscaler.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:22:39.472876 nalyst-0.0.2/nalyst.egg-info/
--rw-rw-rw-   0        0        0     2830 2023-04-14 13:22:39.000000 nalyst-0.0.2/nalyst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-04-14 13:22:39.000000 nalyst-0.0.2/nalyst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:22:39.000000 nalyst-0.0.2/nalyst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-14 13:22:39.000000 nalyst-0.0.2/nalyst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 13:22:39.000000 nalyst-0.0.2/nalyst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 13:22:39.474869 nalyst-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-04-14 13:20:47.000000 nalyst-0.0.2/setup.py
--rw-rw-rw-   0        0        0       19 2023-04-14 13:20:45.000000 nalyst-0.0.2/version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:42:18.572354 nalyst-0.0.3/
+-rw-rw-rw-   0        0        0      167 2023-04-14 13:22:23.000000 nalyst-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1073 2023-04-14 10:45:37.000000 nalyst-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-04-14 10:17:56.000000 nalyst-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2959 2023-04-14 13:42:18.572354 nalyst-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1864 2023-04-14 13:21:51.000000 nalyst-0.0.3/README.md
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:17:56.000000 nalyst-0.0.3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:42:18.563385 nalyst-0.0.3/nalyst/
+-rw-rw-rw-   0        0        0     3196 2023-04-14 11:51:07.000000 nalyst-0.0.3/nalyst/Decisiontree.py
+-rw-rw-rw-   0        0        0     2184 2023-04-14 12:01:05.000000 nalyst-0.0.3/nalyst/KMeans.py
+-rw-rw-rw-   0        0        0     3546 2023-04-14 11:54:35.000000 nalyst-0.0.3/nalyst/LinearRegression.py
+-rw-rw-rw-   0        0        0     3578 2023-04-14 11:50:42.000000 nalyst-0.0.3/nalyst/LogisticRegression.py
+-rw-rw-rw-   0        0        0     1942 2023-04-14 11:51:20.000000 nalyst-0.0.3/nalyst/PCA.py
+-rw-rw-rw-   0        0        0     1816 2023-04-14 11:38:58.000000 nalyst-0.0.3/nalyst/TestTrainSplit.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:17:56.000000 nalyst-0.0.3/nalyst/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-04-14 11:32:16.000000 nalyst-0.0.3/nalyst/maxabsscaler.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 11:27:16.000000 nalyst-0.0.3/nalyst/minmaxscaler.py
+-rw-rw-rw-   0        0        0     2505 2023-04-14 12:13:28.000000 nalyst-0.0.3/nalyst/standardscaler.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:42:18.571358 nalyst-0.0.3/nalyst.egg-info/
+-rw-rw-rw-   0        0        0     2959 2023-04-14 13:42:18.000000 nalyst-0.0.3/nalyst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-04-14 13:42:18.000000 nalyst-0.0.3/nalyst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:42:18.000000 nalyst-0.0.3/nalyst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2023-04-14 13:42:18.000000 nalyst-0.0.3/nalyst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 13:42:18.000000 nalyst-0.0.3/nalyst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-14 10:17:56.000000 nalyst-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:42:18.572354 nalyst-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-14 13:40:05.000000 nalyst-0.0.3/setup.py
+-rw-rw-rw-   0        0        0       19 2023-04-14 13:20:45.000000 nalyst-0.0.3/version.py
```

### Comparing `nalyst-0.0.2/LICENSE` & `nalyst-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.2/PKG-INFO` & `nalyst-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `nalyst-0.0.2/README.md` & `nalyst-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.2/nalyst/Decisiontree.py` & `nalyst-0.0.3/nalyst/Decisiontree.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.2/nalyst/KMeans.py` & `nalyst-0.0.3/nalyst/KMeans.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.2/nalyst/LinearRegression.py` & `nalyst-0.0.3/nalyst/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.2/nalyst/LogisticRegression.py` & `nalyst-0.0.3/nalyst/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.2/nalyst/PCA.py` & `nalyst-0.0.3/nalyst/PCA.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.2/nalyst/TestTrainSplit.py` & `nalyst-0.0.3/nalyst/TestTrainSplit.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.2/nalyst/maxabsscaler.py` & `nalyst-0.0.3/nalyst/maxabsscaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.2/nalyst/standardscaler.py` & `nalyst-0.0.3/nalyst/standardscaler.py`

 * *Files identical despite different names*

### Comparing `nalyst-0.0.2/nalyst.egg-info/PKG-INFO` & `nalyst-0.0.3/nalyst.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: nalyst
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package for data analyst
 Home-page: https://github.com/harryworlds/nalyst
 Author: Hemant Thapa
 Author-email: hemantthapa1998@gmail.com
 Keywords: pandas,random,numpy,pandas datareader,seaborn,matplotlib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `nalyst-0.0.2/setup.py` & `nalyst-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from setuptools import setup, find_packages
+import io
+from os import path
 
-with open('README.md', 'r') as f:
+with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nalyst',
-    version='0.0.2',
+    version='0.0.3',
     author='Hemant Thapa',
     author_email='hemantthapa1998@gmail.com',
     description='A small package for data analyst',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/harryworlds/nalyst',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Education',
         'License :: OSI Approved :: MIT License',
-        'Operating System :: MacOS :: MacOS X',
-        'Operating System :: Microsoft :: Windows :: Windows 10',
+        'Operating System :: OS Independent',
+        'Topic :: Scientific/Engineering :: Information Analysis',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
-    keywords='pandas,random, numpy, pandas datareader, seaborn, matplotlib',
+    keywords='pandas, random, numpy, pandas datareader, seaborn, matplotlib',
     install_requires=[
         'pandas>=1.3.0',
         'numpy>=1.16.5',
         'requests>=2.26.0',
         'seaborn>=0.11.0',
         'matplotlib>=3.4.0',
     ],
```

