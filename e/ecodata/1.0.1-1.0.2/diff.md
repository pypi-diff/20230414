# Comparing `tmp/ecodata-1.0.1.tar.gz` & `tmp/ecodata-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodata-1.0.1.tar", last modified: Fri Apr 14 05:19:35 2023, max compression
+gzip compressed data, was "ecodata-1.0.2.tar", last modified: Fri Apr 14 05:23:50 2023, max compression
```

## Comparing `ecodata-1.0.1.tar` & `ecodata-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 05:19:35.894507 ecodata-1.0.1/
--rw-rw-rw-   0        0        0     2580 2023-04-14 05:19:35.893509 ecodata-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2211 2023-04-14 05:10:31.000000 ecodata-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 05:19:35.894507 ecodata-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-04-14 05:18:40.000000 ecodata-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 05:19:35.877553 ecodata-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 05:19:35.892545 ecodata-1.0.1/src/ecodata.egg-info/
--rw-rw-rw-   0        0        0     2580 2023-04-14 05:19:35.000000 ecodata-1.0.1/src/ecodata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-14 05:19:35.000000 ecodata-1.0.1/src/ecodata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 05:19:35.000000 ecodata-1.0.1/src/ecodata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-14 05:19:35.000000 ecodata-1.0.1/src/ecodata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 05:19:35.000000 ecodata-1.0.1/src/ecodata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 05:23:50.380244 ecodata-1.0.2/
+-rw-rw-rw-   0        0        0     1784 2023-04-14 05:23:50.380244 ecodata-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1415 2023-04-14 05:22:33.000000 ecodata-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 05:23:50.380244 ecodata-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      978 2023-04-14 05:22:50.000000 ecodata-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:23:50.364292 ecodata-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 05:23:50.379248 ecodata-1.0.2/src/ecodata.egg-info/
+-rw-rw-rw-   0        0        0     1784 2023-04-14 05:23:50.000000 ecodata-1.0.2/src/ecodata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-14 05:23:50.000000 ecodata-1.0.2/src/ecodata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 05:23:50.000000 ecodata-1.0.2/src/ecodata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-14 05:23:50.000000 ecodata-1.0.2/src/ecodata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 05:23:50.000000 ecodata-1.0.2/src/ecodata.egg-info/top_level.txt
```

### Comparing `ecodata-1.0.1/setup.py` & `ecodata-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='ecodata',
-    version = '1.0.1',
+    version = '1.0.2',
     author = [
         'Mauricio Alvarado',
         'Andrei Romero',
     ],
     author_email = 'mauricio.mauricio@pucp.edu.pe',
     description = 'Extracción de series de tiempo de las seis principales instituciones económicas para el Perú',
     long_description = long_description,
```

