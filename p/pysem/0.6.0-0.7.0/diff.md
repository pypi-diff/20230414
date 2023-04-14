# Comparing `tmp/pysem-0.6.0.tar.gz` & `tmp/pysem-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysem-0.6.0.tar", last modified: Tue Nov 29 09:10:51 2022, max compression
+gzip compressed data, was "pysem-0.7.0.tar", last modified: Fri Apr 14 07:33:48 2023, max compression
```

## Comparing `pysem-0.6.0.tar` & `pysem-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2022-11-29 09:10:51.970127 pysem-0.6.0/
--rw-r--r--   0 mattis    (1000) mattis    (1000)     1063 2021-02-26 22:10:43.000000 pysem-0.6.0/LICENSE
--rw-r--r--   0 mattis    (1000) mattis    (1000)       60 2021-02-26 22:10:43.000000 pysem-0.6.0/MANIFEST.in
--rw-r--r--   0 mattis    (1000) mattis    (1000)     1793 2022-11-29 09:10:51.970127 pysem-0.6.0/PKG-INFO
--rw-r--r--   0 mattis    (1000) mattis    (1000)     1064 2021-06-16 04:43:15.000000 pysem-0.6.0/README.md
--rw-r--r--   0 mattis    (1000) mattis    (1000)      403 2022-11-29 09:10:51.970127 pysem-0.6.0/setup.cfg
--rw-r--r--   0 mattis    (1000) mattis    (1000)     1279 2022-11-29 09:08:51.000000 pysem-0.6.0/setup.py
-drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2022-11-29 09:10:51.966794 pysem-0.6.0/src/
-drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2022-11-29 09:10:51.970127 pysem-0.6.0/src/pysem/
--rw-r--r--   0 mattis    (1000) mattis    (1000)       93 2022-11-29 09:08:51.000000 pysem-0.6.0/src/pysem/__init__.py
--rw-r--r--   0 mattis    (1000) mattis    (1000)        0 2022-05-23 11:11:52.000000 pysem-0.6.0/src/pysem/cli.py
-drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2022-11-29 09:10:51.970127 pysem-0.6.0/src/pysem/data/
--rw-r--r--   0 mattis    (1000) mattis    (1000)   833014 2022-11-29 09:06:33.000000 pysem-0.6.0/src/pysem/data/concepticon.zip
--rw-r--r--   0 mattis    (1000) mattis    (1000)   204330 2021-02-26 22:10:43.000000 pysem-0.6.0/src/pysem/data/sense.csv
--rw-r--r--   0 mattis    (1000) mattis    (1000)      546 2021-05-03 15:22:28.000000 pysem-0.6.0/src/pysem/data.py
--rw-r--r--   0 mattis    (1000) mattis    (1000)    12226 2021-06-16 04:43:15.000000 pysem-0.6.0/src/pysem/glosses.py
--rw-r--r--   0 mattis    (1000) mattis    (1000)     2722 2022-11-29 09:09:24.000000 pysem-0.6.0/src/pysem/main.py
--rw-r--r--   0 mattis    (1000) mattis    (1000)     2171 2021-05-03 17:22:50.000000 pysem-0.6.0/src/pysem/sense.py
-drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2022-11-29 09:10:51.970127 pysem-0.6.0/src/pysem.egg-info/
--rw-r--r--   0 mattis    (1000) mattis    (1000)     1793 2022-11-29 09:10:51.000000 pysem-0.6.0/src/pysem.egg-info/PKG-INFO
--rw-r--r--   0 mattis    (1000) mattis    (1000)      415 2022-11-29 09:10:51.000000 pysem-0.6.0/src/pysem.egg-info/SOURCES.txt
--rw-r--r--   0 mattis    (1000) mattis    (1000)        1 2022-11-29 09:10:51.000000 pysem-0.6.0/src/pysem.egg-info/dependency_links.txt
--rw-r--r--   0 mattis    (1000) mattis    (1000)        1 2021-05-03 17:25:48.000000 pysem-0.6.0/src/pysem.egg-info/not-zip-safe
--rw-r--r--   0 mattis    (1000) mattis    (1000)       95 2022-11-29 09:10:51.000000 pysem-0.6.0/src/pysem.egg-info/requires.txt
--rw-r--r--   0 mattis    (1000) mattis    (1000)        6 2022-11-29 09:10:51.000000 pysem-0.6.0/src/pysem.egg-info/top_level.txt
+drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2023-04-14 07:33:48.804971 pysem-0.7.0/
+-rw-r--r--   0 mattis    (1000) mattis    (1000)     1063 2021-02-26 22:10:43.000000 pysem-0.7.0/LICENSE
+-rw-r--r--   0 mattis    (1000) mattis    (1000)       60 2021-02-26 22:10:43.000000 pysem-0.7.0/MANIFEST.in
+-rw-r--r--   0 mattis    (1000) mattis    (1000)     1896 2023-04-14 07:33:48.804971 pysem-0.7.0/PKG-INFO
+-rw-r--r--   0 mattis    (1000) mattis    (1000)     1165 2023-04-14 07:29:29.000000 pysem-0.7.0/README.md
+-rw-r--r--   0 mattis    (1000) mattis    (1000)      403 2023-04-14 07:33:48.804971 pysem-0.7.0/setup.cfg
+-rw-r--r--   0 mattis    (1000) mattis    (1000)     1279 2023-04-14 07:27:47.000000 pysem-0.7.0/setup.py
+drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2023-04-14 07:33:48.801638 pysem-0.7.0/src/
+drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2023-04-14 07:33:48.801638 pysem-0.7.0/src/pysem/
+-rw-r--r--   0 mattis    (1000) mattis    (1000)       91 2023-04-14 07:29:47.000000 pysem-0.7.0/src/pysem/__init__.py
+-rw-r--r--   0 mattis    (1000) mattis    (1000)        0 2022-05-23 11:11:52.000000 pysem-0.7.0/src/pysem/cli.py
+drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2023-04-14 07:33:48.804971 pysem-0.7.0/src/pysem/data/
+-rw-r--r--   0 mattis    (1000) mattis    (1000)   857513 2023-04-14 07:27:15.000000 pysem-0.7.0/src/pysem/data/concepticon.zip
+-rw-r--r--   0 mattis    (1000) mattis    (1000)   204330 2021-02-26 22:10:43.000000 pysem-0.7.0/src/pysem/data/sense.csv
+-rw-r--r--   0 mattis    (1000) mattis    (1000)      546 2021-05-03 15:22:28.000000 pysem-0.7.0/src/pysem/data.py
+-rw-r--r--   0 mattis    (1000) mattis    (1000)    12242 2023-04-14 07:30:25.000000 pysem-0.7.0/src/pysem/glosses.py
+-rw-r--r--   0 mattis    (1000) mattis    (1000)     2722 2022-11-29 09:09:24.000000 pysem-0.7.0/src/pysem/main.py
+-rw-r--r--   0 mattis    (1000) mattis    (1000)     2171 2021-05-03 17:22:50.000000 pysem-0.7.0/src/pysem/sense.py
+drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2023-04-14 07:33:48.804971 pysem-0.7.0/src/pysem.egg-info/
+-rw-r--r--   0 mattis    (1000) mattis    (1000)     1896 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/PKG-INFO
+-rw-r--r--   0 mattis    (1000) mattis    (1000)      451 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/SOURCES.txt
+-rw-r--r--   0 mattis    (1000) mattis    (1000)        1 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/dependency_links.txt
+-rw-r--r--   0 mattis    (1000) mattis    (1000)       20 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/entry_points.txt
+-rw-r--r--   0 mattis    (1000) mattis    (1000)        1 2021-05-03 17:25:48.000000 pysem-0.7.0/src/pysem.egg-info/not-zip-safe
+-rw-r--r--   0 mattis    (1000) mattis    (1000)       95 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/requires.txt
+-rw-r--r--   0 mattis    (1000) mattis    (1000)        6 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/top_level.txt
```

### Comparing `pysem-0.6.0/LICENSE` & `pysem-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysem-0.6.0/PKG-INFO` & `pysem-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysem
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python library for manipulating semantic data in linguistics
 Home-page: https://github.com/lingpy/pysem
 Author: Johann-Mattis List
 Author-email: list@shh.mpg.de
 License: MIT
 Keywords: data
 Platform: any
@@ -18,14 +18,17 @@
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # PySem: Pysen library for handling semantic data in linguistics
+
+* **Current Version**: 0.7
+* **Concepticon Version**: [3.1.0](https://doi.org/10.5281/zenodo.7777629)
  
 ## Usage Examples
 
 Retrieve the sense data assembled by S. A. Starostin in the STARLING software package and search for similar words:
 
 ```python
 >>> from pysem.sense import Sense
@@ -44,8 +47,10 @@
 >>> from pysem import to_concepticon
 >>> to_concepticon([{"gloss": "Fuß", pos: "noun"}], language="de"}])
 {'Fuß': [['1301', 'FOOT', 'noun', 19]]}
 ```
 
 ## How to Cite
 
-> List, Johann-Mattis (2021): PySeM. A Python library for handling semantic data in linguistics. Version 0.4.0 URL: https://github.com/lingpy/pysem/, Leipzig: Max Planck Institute for Evolutionary Anthropology.
+> List, Johann-Mattis (2023): PySeM. A Python library for handling semantic data in linguistics. Version 0.7 URL: https://github.com/lingpy/pysem/, Leipzig: Max Planck Institute for Evolutionary Anthropology.
+
+
```

### Comparing `pysem-0.6.0/README.md` & `pysem-0.7.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # PySem: Pysen library for handling semantic data in linguistics
+
+* **Current Version**: 0.7
+* **Concepticon Version**: [3.1.0](https://doi.org/10.5281/zenodo.7777629)
  
 ## Usage Examples
 
 Retrieve the sense data assembled by S. A. Starostin in the STARLING software package and search for similar words:
 
 ```python
 >>> from pysem.sense import Sense
@@ -21,8 +24,8 @@
 >>> from pysem import to_concepticon
 >>> to_concepticon([{"gloss": "Fuß", pos: "noun"}], language="de"}])
 {'Fuß': [['1301', 'FOOT', 'noun', 19]]}
 ```
 
 ## How to Cite
 
-> List, Johann-Mattis (2021): PySeM. A Python library for handling semantic data in linguistics. Version 0.4.0 URL: https://github.com/lingpy/pysem/, Leipzig: Max Planck Institute for Evolutionary Anthropology.
+> List, Johann-Mattis (2023): PySeM. A Python library for handling semantic data in linguistics. Version 0.7 URL: https://github.com/lingpy/pysem/, Leipzig: Max Planck Institute for Evolutionary Anthropology.
```

### Comparing `pysem-0.6.0/setup.py` & `pysem-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='pysem',
-    version='0.6.0',
+    version='0.7.0',
     license='MIT',
     description='Python library for manipulating semantic data in linguistics',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

### Comparing `pysem-0.6.0/src/pysem/data/sense.csv` & `pysem-0.7.0/src/pysem/data/sense.csv`

 * *Files identical despite different names*

### Comparing `pysem-0.6.0/src/pysem/data.py` & `pysem-0.7.0/src/pysem/data.py`

 * *Files identical despite different names*

### Comparing `pysem-0.6.0/src/pysem/glosses.py` & `pysem-0.7.0/src/pysem/glosses.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
     splitter=",|;|:|/| or | OR ",
     marker='?!"¨:;,»«´“”*+-',
     brackets_open="([{（<",
     brackets_close=")]}）>",
     mappings=MAPPINGS,
 ):
     """
-    Map a given concept list to concepticon.
+    Map a given concept list to Concepticon (Version 3.1.0).
     """
     matches = {}
     for concept in concepts:
         gloss, pos = concept.get(gloss_ref), concept.get(pos_ref, "")
         if gloss:
             glosses = parse_gloss(
                 gloss,
```

### Comparing `pysem-0.6.0/src/pysem/main.py` & `pysem-0.7.0/src/pysem/main.py`

 * *Files identical despite different names*

### Comparing `pysem-0.6.0/src/pysem/sense.py` & `pysem-0.7.0/src/pysem/sense.py`

 * *Files identical despite different names*

### Comparing `pysem-0.6.0/src/pysem.egg-info/PKG-INFO` & `pysem-0.7.0/src/pysem.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysem
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python library for manipulating semantic data in linguistics
 Home-page: https://github.com/lingpy/pysem
 Author: Johann-Mattis List
 Author-email: list@shh.mpg.de
 License: MIT
 Keywords: data
 Platform: any
@@ -18,14 +18,17 @@
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # PySem: Pysen library for handling semantic data in linguistics
+
+* **Current Version**: 0.7
+* **Concepticon Version**: [3.1.0](https://doi.org/10.5281/zenodo.7777629)
  
 ## Usage Examples
 
 Retrieve the sense data assembled by S. A. Starostin in the STARLING software package and search for similar words:
 
 ```python
 >>> from pysem.sense import Sense
@@ -44,8 +47,10 @@
 >>> from pysem import to_concepticon
 >>> to_concepticon([{"gloss": "Fuß", pos: "noun"}], language="de"}])
 {'Fuß': [['1301', 'FOOT', 'noun', 19]]}
 ```
 
 ## How to Cite
 
-> List, Johann-Mattis (2021): PySeM. A Python library for handling semantic data in linguistics. Version 0.4.0 URL: https://github.com/lingpy/pysem/, Leipzig: Max Planck Institute for Evolutionary Anthropology.
+> List, Johann-Mattis (2023): PySeM. A Python library for handling semantic data in linguistics. Version 0.7 URL: https://github.com/lingpy/pysem/, Leipzig: Max Planck Institute for Evolutionary Anthropology.
+
+
```

