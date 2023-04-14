# Comparing `tmp/etl_csm_pet-0.0.2.tar.gz` & `tmp/etl_csm_pet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm_pet-0.0.2.tar", last modified: Fri Apr 14 15:15:57 2023, max compression
+gzip compressed data, was "etl_csm_pet-0.0.3.tar", last modified: Fri Apr 14 17:03:01 2023, max compression
```

## Comparing `etl_csm_pet-0.0.2.tar` & `etl_csm_pet-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 15:15:57.075717 etl_csm_pet-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-14 15:15:57.070716 etl_csm_pet-0.0.2/Etl/
--rw-rw-rw-   0        0        0     3381 2023-04-14 13:56:04.000000 etl_csm_pet-0.0.2/Etl/Execute.py
--rw-rw-rw-   0        0        0     1547 2023-04-14 15:13:09.000000 etl_csm_pet-0.0.2/Etl/Extrator.py
--rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.2/Etl/Helper.py
--rw-rw-rw-   0        0        0     1761 2023-04-14 15:13:16.000000 etl_csm_pet-0.0.2/Etl/Loader.py
--rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.2/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm_pet-0.0.2/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.2/Etl/Treatment_tracking_pme.py
--rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.2/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm_pet-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      552 2023-04-14 15:15:57.074718 etl_csm_pet-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm_pet-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 15:15:57.074718 etl_csm_pet-0.0.2/etl_csm_pet.egg-info/
--rw-rw-rw-   0        0        0      552 2023-04-14 15:15:56.000000 etl_csm_pet-0.0.2/etl_csm_pet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-14 15:15:56.000000 etl_csm_pet-0.0.2/etl_csm_pet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 15:15:56.000000 etl_csm_pet-0.0.2/etl_csm_pet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-14 15:15:56.000000 etl_csm_pet-0.0.2/etl_csm_pet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-14 15:15:56.000000 etl_csm_pet-0.0.2/etl_csm_pet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 15:15:57.075717 etl_csm_pet-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-04-14 15:15:38.000000 etl_csm_pet-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:03:01.846418 etl_csm_pet-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-04-14 17:03:01.841418 etl_csm_pet-0.0.3/Etl/
+-rw-rw-rw-   0        0        0     3381 2023-04-14 13:56:04.000000 etl_csm_pet-0.0.3/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1547 2023-04-14 15:13:09.000000 etl_csm_pet-0.0.3/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.3/Etl/Helper.py
+-rw-rw-rw-   0        0        0     1761 2023-04-14 15:13:16.000000 etl_csm_pet-0.0.3/Etl/Loader.py
+-rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.3/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm_pet-0.0.3/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.3/Etl/Treatment_tracking_pme.py
+-rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.3/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm_pet-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      552 2023-04-14 17:03:01.845419 etl_csm_pet-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm_pet-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 17:03:01.845419 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/
+-rw-rw-rw-   0        0        0      552 2023-04-14 17:03:01.000000 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-04-14 17:03:01.000000 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 17:03:01.000000 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-14 17:03:01.000000 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-14 17:03:01.000000 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 17:03:01.846418 etl_csm_pet-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-14 17:02:43.000000 etl_csm_pet-0.0.3/setup.py
```

### Comparing `etl_csm_pet-0.0.2/Etl/Execute.py` & `etl_csm_pet-0.0.3/Etl/Execute.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.2/Etl/Extrator.py` & `etl_csm_pet-0.0.3/Etl/Extrator.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.2/Etl/Helper.py` & `etl_csm_pet-0.0.3/Etl/Helper.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.2/Etl/Loader.py` & `etl_csm_pet-0.0.3/Etl/Loader.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.2/Etl/Treatment_extras.py` & `etl_csm_pet-0.0.3/Etl/Treatment_extras.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.2/Etl/Treatment_tracking.py` & `etl_csm_pet-0.0.3/Etl/Treatment_tracking.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.2/Etl/Treatment_tracking_pme.py` & `etl_csm_pet-0.0.3/Etl/Treatment_tracking_pme.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.2/Etl/__init__.py` & `etl_csm_pet-0.0.3/Etl/__init__.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.2/LICENSE` & `etl_csm_pet-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.2/PKG-INFO` & `etl_csm_pet-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm_pet
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm_pet-0.0.2/README.md` & `etl_csm_pet-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.2/etl_csm_pet.egg-info/PKG-INFO` & `etl_csm_pet-0.0.3/etl_csm_pet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm-pet
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm_pet-0.0.2/setup.py` & `etl_csm_pet-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm_pet",
     version = VERSION,
     author = "ingloriamori",
     author_email = "francisco.froes@globalhitss.com.br",
     description = DESCRIPTION,
     long_description = 'Biblioteca para aproveitar classes de tratamento CSM, direcionada para pet',
     packages = find_packages(),
     url = 'https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl',
     keywords = ['python', 'etl'],
     license = 'MIT',
-    install_requires = ['numpy', 'pandas', 'orjson','psycopg2','SQLAlchemy'],
+    install_requires = ['numpy', 'pandas', 'orjson','SQLAlchemy','psycopg2-binary'],
     extras_require = {
         'dev':['twine>=4.0.2'],
     },
     classifiers = [
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
         'Operating System :: OS Independent',
```

