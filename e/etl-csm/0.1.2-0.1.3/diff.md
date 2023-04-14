# Comparing `tmp/etl_csm-0.1.2.tar.gz` & `tmp/etl_csm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm-0.1.2.tar", last modified: Thu Apr 13 16:57:23 2023, max compression
+gzip compressed data, was "etl_csm-0.1.3.tar", last modified: Fri Apr 14 17:05:08 2023, max compression
```

## Comparing `etl_csm-0.1.2.tar` & `etl_csm-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:57:23.057762 etl_csm-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-04-13 16:57:23.052763 etl_csm-0.1.2/Etl/
--rw-rw-rw-   0        0        0     3379 2023-04-12 17:56:57.000000 etl_csm-0.1.2/Etl/Execute.py
--rw-rw-rw-   0        0        0     1543 2023-04-12 17:56:57.000000 etl_csm-0.1.2/Etl/Extrator.py
--rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm-0.1.2/Etl/Helper.py
--rw-rw-rw-   0        0        0     1753 2023-04-12 17:56:57.000000 etl_csm-0.1.2/Etl/Loader.py
--rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm-0.1.2/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm-0.1.2/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm-0.1.2/Etl/Treatment_tracking_pme.py
--rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm-0.1.2/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      526 2023-04-13 16:57:23.056764 etl_csm-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      901 2023-04-03 13:37:17.000000 etl_csm-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 16:57:23.055764 etl_csm-0.1.2/etl_csm.egg-info/
--rw-rw-rw-   0        0        0      526 2023-04-13 16:57:22.000000 etl_csm-0.1.2/etl_csm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-04-13 16:57:22.000000 etl_csm-0.1.2/etl_csm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:57:22.000000 etl_csm-0.1.2/etl_csm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-13 16:57:22.000000 etl_csm-0.1.2/etl_csm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-13 16:57:22.000000 etl_csm-0.1.2/etl_csm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 16:57:23.057762 etl_csm-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-04-13 16:56:45.000000 etl_csm-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 17:05:08.090532 etl_csm-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-04-14 17:05:08.085532 etl_csm-0.1.3/Etl/
+-rw-rw-rw-   0        0        0     3379 2023-04-14 17:04:18.000000 etl_csm-0.1.3/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1543 2023-04-14 17:04:18.000000 etl_csm-0.1.3/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm-0.1.3/Etl/Helper.py
+-rw-rw-rw-   0        0        0     1753 2023-04-14 17:04:18.000000 etl_csm-0.1.3/Etl/Loader.py
+-rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm-0.1.3/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm-0.1.3/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm-0.1.3/Etl/Treatment_tracking_pme.py
+-rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm-0.1.3/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      526 2023-04-14 17:05:08.089533 etl_csm-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 17:05:08.088532 etl_csm-0.1.3/etl_csm.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-04-14 17:05:07.000000 etl_csm-0.1.3/etl_csm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-14 17:05:07.000000 etl_csm-0.1.3/etl_csm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 17:05:07.000000 etl_csm-0.1.3/etl_csm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-14 17:05:07.000000 etl_csm-0.1.3/etl_csm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-14 17:05:07.000000 etl_csm-0.1.3/etl_csm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 17:05:08.090532 etl_csm-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      911 2023-04-14 17:04:42.000000 etl_csm-0.1.3/setup.py
```

### Comparing `etl_csm-0.1.2/Etl/Execute.py` & `etl_csm-0.1.3/Etl/Execute.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.2/Etl/Extrator.py` & `etl_csm-0.1.3/Etl/Extrator.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.2/Etl/Helper.py` & `etl_csm-0.1.3/Etl/Helper.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.2/Etl/Loader.py` & `etl_csm-0.1.3/Etl/Loader.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.2/Etl/Treatment_extras.py` & `etl_csm-0.1.3/Etl/Treatment_extras.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.2/Etl/Treatment_tracking.py` & `etl_csm-0.1.3/Etl/Treatment_tracking.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.2/Etl/Treatment_tracking_pme.py` & `etl_csm-0.1.3/Etl/Treatment_tracking_pme.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.2/Etl/__init__.py` & `etl_csm-0.1.3/Etl/__init__.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.2/LICENSE` & `etl_csm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.2/PKG-INFO` & `etl_csm-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.2/README.md` & `etl_csm-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Pacote para ter acesso a funcoes de tratamento e extracao de dados RDS
-* Aqui se localiza a biblioteca etl e o serviço de etl do RDS
+* Aqui se localiza a biblioteca etl
 * Joguei ele para um pacote para facilidade de importação e aproveitamento de classes de limpeza
+* Aviso nao instale etl-csm aqui
 # Como instalar a biblioteca?
 * pip install etl-csm
 * Pronto
 # Configuração de ambiente?
 * As demandas do ambiente local localizam-se na environment.yml
 * As demandos do ambiente cloud localizam-se no serverless.yml.
 # Links importantes
```

### Comparing `etl_csm-0.1.2/etl_csm.egg-info/PKG-INFO` & `etl_csm-0.1.3/etl_csm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.2/setup.py` & `etl_csm-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm",
     version = VERSION,
     author = "ingloriamori",
     author_email = "francisco.froes@globalhitss.com.br",
     description = DESCRIPTION,
     long_description = 'Biblioteca para aproveitar classes de tratamento CSM',
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

