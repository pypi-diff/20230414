# Comparing `tmp/dataroid-0.0.3.tar.gz` & `tmp/dataroid-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataroid-0.0.3.tar", last modified: Fri Apr 14 09:07:06 2023, max compression
+gzip compressed data, was "dataroid-0.0.4.tar", last modified: Fri Apr 14 09:42:40 2023, max compression
```

## Comparing `dataroid-0.0.3.tar` & `dataroid-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-14 09:07:06.803331 dataroid-0.0.3/
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1832 2023-04-14 09:07:06.803331 dataroid-0.0.3/PKG-INFO
-drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-14 09:07:06.803331 dataroid-0.0.3/dataroid/
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       22 2023-04-14 08:04:09.000000 dataroid-0.0.3/dataroid/__init__.py
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1167 2023-04-14 08:14:28.000000 dataroid-0.0.3/dataroid/dataroid.py
-drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-14 09:07:06.803331 dataroid-0.0.3/dataroid.egg-info/
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1832 2023-04-14 09:07:06.000000 dataroid-0.0.3/dataroid.egg-info/PKG-INFO
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      209 2023-04-14 09:07:06.000000 dataroid-0.0.3/dataroid.egg-info/SOURCES.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        1 2023-04-14 09:07:06.000000 dataroid-0.0.3/dataroid.egg-info/dependency_links.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       27 2023-04-14 09:07:06.000000 dataroid-0.0.3/dataroid.egg-info/requires.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        9 2023-04-14 09:07:06.000000 dataroid-0.0.3/dataroid.egg-info/top_level.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       38 2023-04-14 09:07:06.803331 dataroid-0.0.3/setup.cfg
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      994 2023-04-14 09:07:02.000000 dataroid-0.0.3/setup.py
+drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-14 09:42:40.351652 dataroid-0.0.4/
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1597 2023-04-14 09:42:40.351652 dataroid-0.0.4/PKG-INFO
+drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-14 09:42:40.351652 dataroid-0.0.4/dataroid/
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       47 2023-04-14 09:40:53.000000 dataroid-0.0.4/dataroid/__init__.py
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1167 2023-04-14 08:14:28.000000 dataroid-0.0.4/dataroid/dataroid.py
+drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-14 09:42:40.351652 dataroid-0.0.4/dataroid.egg-info/
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1597 2023-04-14 09:42:40.000000 dataroid-0.0.4/dataroid.egg-info/PKG-INFO
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      209 2023-04-14 09:42:40.000000 dataroid-0.0.4/dataroid.egg-info/SOURCES.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        1 2023-04-14 09:42:40.000000 dataroid-0.0.4/dataroid.egg-info/dependency_links.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       27 2023-04-14 09:42:40.000000 dataroid-0.0.4/dataroid.egg-info/requires.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        9 2023-04-14 09:42:40.000000 dataroid-0.0.4/dataroid.egg-info/top_level.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       38 2023-04-14 09:42:40.351652 dataroid-0.0.4/setup.cfg
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      980 2023-04-14 09:42:21.000000 dataroid-0.0.4/setup.py
```

### Comparing `dataroid-0.0.3/PKG-INFO` & `dataroid-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: dataroid
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Simple Wrapper For Synthetic Data Generation
-Author: torchd3v (Burak Egeli)
+Author: torchd3v
 Author-email: <burak96egeli@gmail.com>
 Keywords: python,data,generate,synthetic,deep learning,model
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 ## Installation
 ```sh
-#PyPI
 pip install dataroid
 ```
 # Usage Example
-
-In this example we load the [Adult Census Dataset](https://archive.ics.uci.edu/ml/datasets/adult)* which is a built-in demo dataset. We use CTGAN to learn from the real data and then generate some synthetic data.
-
 ```python3
 from dataroid import Bot
 import pandas as pd
 
 data = pd.read_csv("shopping.csv")
 
 model = Bot(data)
```

### Comparing `dataroid-0.0.3/dataroid/dataroid.py` & `dataroid-0.0.4/dataroid/dataroid.py`

 * *Files identical despite different names*

### Comparing `dataroid-0.0.3/dataroid.egg-info/PKG-INFO` & `dataroid-0.0.4/dataroid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: dataroid
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Simple Wrapper For Synthetic Data Generation
-Author: torchd3v (Burak Egeli)
+Author: torchd3v
 Author-email: <burak96egeli@gmail.com>
 Keywords: python,data,generate,synthetic,deep learning,model
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 ## Installation
 ```sh
-#PyPI
 pip install dataroid
 ```
 # Usage Example
-
-In this example we load the [Adult Census Dataset](https://archive.ics.uci.edu/ml/datasets/adult)* which is a built-in demo dataset. We use CTGAN to learn from the real data and then generate some synthetic data.
-
 ```python3
 from dataroid import Bot
 import pandas as pd
 
 data = pd.read_csv("shopping.csv")
 
 model = Bot(data)
```

### Comparing `dataroid-0.0.3/setup.py` & `dataroid-0.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A Simple Wrapper For Synthetic Data Generation'
 LONG_DESCRIPTION = (this_directory / "dataroid/README.md").read_text()
 
 
 # Setting up
 setup(
     name="dataroid",
     version=VERSION,
-    author="torchd3v (Burak Egeli)",
+    author="torchd3v",
     author_email="<burak96egeli@gmail.com>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['pandas==1.5.3', 'ctgan==0.7.1'],
     keywords=['python', 'data', 'generate', 'synthetic', 'deep learning', 'model'],
```

