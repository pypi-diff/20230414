# Comparing `tmp/practicalSPARQL-0.0.5.tar.gz` & `tmp/practicalSPARQL-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "practicalSPARQL-0.0.5.tar", last modified: Mon Apr  3 17:33:04 2023, max compression
+gzip compressed data, was "practicalSPARQL-0.0.6.tar", last modified: Fri Apr 14 15:00:55 2023, max compression
```

## Comparing `practicalSPARQL-0.0.5.tar` & `practicalSPARQL-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hassanel-hajj   (502) staff       (20)        0 2023-04-03 17:33:04.229615 practicalSPARQL-0.0.5/
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)     1071 2022-12-22 15:08:16.000000 practicalSPARQL-0.0.5/LICENSE.txt
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)     1619 2023-04-03 17:33:04.229478 practicalSPARQL-0.0.5/PKG-INFO
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)     1090 2023-03-23 20:18:57.000000 practicalSPARQL-0.0.5/README.md
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)       38 2023-04-03 17:33:04.229659 practicalSPARQL-0.0.5/setup.cfg
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)      827 2023-04-03 17:30:26.000000 practicalSPARQL-0.0.5/setup.py
-drwxr-xr-x   0 hassanel-hajj   (502) staff       (20)        0 2023-04-03 17:33:04.228535 practicalSPARQL-0.0.5/src/
-drwxr-xr-x   0 hassanel-hajj   (502) staff       (20)        0 2023-04-03 17:33:04.229285 practicalSPARQL-0.0.5/src/practicalSPARQL.egg-info/
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)     1619 2023-04-03 17:33:04.000000 practicalSPARQL-0.0.5/src/practicalSPARQL.egg-info/PKG-INFO
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)      267 2023-04-03 17:33:04.000000 practicalSPARQL-0.0.5/src/practicalSPARQL.egg-info/SOURCES.txt
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)        1 2023-04-03 17:33:04.000000 practicalSPARQL-0.0.5/src/practicalSPARQL.egg-info/dependency_links.txt
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)       27 2023-04-03 17:33:04.000000 practicalSPARQL-0.0.5/src/practicalSPARQL.egg-info/requires.txt
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)       16 2023-04-03 17:33:04.000000 practicalSPARQL-0.0.5/src/practicalSPARQL.egg-info/top_level.txt
--rw-r--r--   0 hassanel-hajj   (502) staff       (20)     9008 2023-04-03 17:30:43.000000 practicalSPARQL-0.0.5/src/practicalSPARQL.py
+drwxr-xr-x   0 hassanel-hajj   (502) staff       (20)        0 2023-04-14 15:00:55.142001 practicalSPARQL-0.0.6/
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)     1071 2022-12-22 15:08:16.000000 practicalSPARQL-0.0.6/LICENSE.txt
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)     1619 2023-04-14 15:00:55.141865 practicalSPARQL-0.0.6/PKG-INFO
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)     1090 2023-04-14 14:59:39.000000 practicalSPARQL-0.0.6/README.md
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)       38 2023-04-14 15:00:55.142048 practicalSPARQL-0.0.6/setup.cfg
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)      827 2023-04-14 14:59:53.000000 practicalSPARQL-0.0.6/setup.py
+drwxr-xr-x   0 hassanel-hajj   (502) staff       (20)        0 2023-04-14 15:00:55.140978 practicalSPARQL-0.0.6/src/
+drwxr-xr-x   0 hassanel-hajj   (502) staff       (20)        0 2023-04-14 15:00:55.141667 practicalSPARQL-0.0.6/src/practicalSPARQL.egg-info/
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)     1619 2023-04-14 15:00:55.000000 practicalSPARQL-0.0.6/src/practicalSPARQL.egg-info/PKG-INFO
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)      267 2023-04-14 15:00:55.000000 practicalSPARQL-0.0.6/src/practicalSPARQL.egg-info/SOURCES.txt
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)        1 2023-04-14 15:00:55.000000 practicalSPARQL-0.0.6/src/practicalSPARQL.egg-info/dependency_links.txt
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)       27 2023-04-14 15:00:55.000000 practicalSPARQL-0.0.6/src/practicalSPARQL.egg-info/requires.txt
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)       16 2023-04-14 15:00:55.000000 practicalSPARQL-0.0.6/src/practicalSPARQL.egg-info/top_level.txt
+-rw-r--r--   0 hassanel-hajj   (502) staff       (20)     9135 2023-04-14 14:58:37.000000 practicalSPARQL-0.0.6/src/practicalSPARQL.py
```

### Comparing `practicalSPARQL-0.0.5/LICENSE.txt` & `practicalSPARQL-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `practicalSPARQL-0.0.5/PKG-INFO` & `practicalSPARQL-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: practicalSPARQL
-Version: 0.0.5
+Version: 0.0.6
 Summary: Small wrapper to simplify the interaction with SPARQL endpoints. Built on top of sparqlwrapper and RDFlib
 Home-page: https://github.com/hassanhajj910/practicalsparql
 Author: hassanhajj910@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # practicalSPARQL
-Version 0.0.4
+Version 0.0.6
 ## Install using pip
 ``` 
 pip install practicalsparql
 ```
 ## Install using conda from conda-forge
 ```
 conda install -c conda-forge practicalsparql
```

### Comparing `practicalSPARQL-0.0.5/README.md` & `practicalSPARQL-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # practicalSPARQL
-Version 0.0.4
+Version 0.0.6
 ## Install using pip
 ``` 
 pip install practicalsparql
 ```
 ## Install using conda from conda-forge
 ```
 conda install -c conda-forge practicalsparql
```

### Comparing `practicalSPARQL-0.0.5/setup.py` & `practicalSPARQL-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r') as f:
     longDesc = f.read()
 
 setup(
     name="practicalSPARQL",
-    version='0.0.5',
+    version='0.0.6',
     description="Small wrapper to simplify the interaction with SPARQL endpoints. Built on top of sparqlwrapper and RDFlib",
     py_modules=["practicalSPARQL"],
     package_dir={'':'src'},
     author='hassanhajj910@gmail.com',
     url='https://github.com/hassanhajj910/practicalsparql',
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `practicalSPARQL-0.0.5/src/practicalSPARQL.egg-info/PKG-INFO` & `practicalSPARQL-0.0.6/src/practicalSPARQL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: practicalSPARQL
-Version: 0.0.5
+Version: 0.0.6
 Summary: Small wrapper to simplify the interaction with SPARQL endpoints. Built on top of sparqlwrapper and RDFlib
 Home-page: https://github.com/hassanhajj910/practicalsparql
 Author: hassanhajj910@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # practicalSPARQL
-Version 0.0.4
+Version 0.0.6
 ## Install using pip
 ``` 
 pip install practicalsparql
 ```
 ## Install using conda from conda-forge
 ```
 conda install -c conda-forge practicalsparql
```

### Comparing `practicalSPARQL-0.0.5/src/practicalSPARQL.py` & `practicalSPARQL-0.0.6/src/practicalSPARQL.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,17 @@
     
     def select_as_dataframe(self, q:str):
         import pandas as pd
         res = self.query(q)
         cols = list(res.vars)
         cols = [str(x) for x in cols]
         res = np.array(list(res))
+        # if no results, return an empty df. 
+        if len(res) == 0:
+            res = [[np.nan for x in range(len(cols))]]
         df = pd.DataFrame(data = res, columns=cols)
         return df
 
         
 
 
 class practicalWrapper(SPARQLWrapper):
```

