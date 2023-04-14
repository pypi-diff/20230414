# Comparing `tmp/ecodata-0.0.5.tar.gz` & `tmp/ecodata-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodata-0.0.5.tar", last modified: Fri Apr 14 09:12:49 2023, max compression
+gzip compressed data, was "ecodata-0.0.6.tar", last modified: Fri Apr 14 09:20:54 2023, max compression
```

## Comparing `ecodata-0.0.5.tar` & `ecodata-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:12:49.909759 ecodata-0.0.5/
--rw-rw-rw-   0        0        0     1698 2023-04-14 09:12:49.909759 ecodata-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-04-14 09:12:07.000000 ecodata-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 09:12:49.909759 ecodata-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-14 09:11:55.000000 ecodata-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:12:49.885826 ecodata-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 09:12:49.894799 ecodata-0.0.5/src/ecodata/
--rw-rw-rw-   0        0        0     6281 2023-04-14 08:55:43.000000 ecodata-0.0.5/src/ecodata/BCRP.py
--rw-rw-rw-   0        0        0     2820 2023-04-14 08:10:41.000000 ecodata-0.0.5/src/ecodata/BM.py
--rw-rw-rw-   0        0        0     3554 2023-04-14 08:10:41.000000 ecodata-0.0.5/src/ecodata/FRED.py
--rw-rw-rw-   0        0        0     2425 2023-04-14 08:10:41.000000 ecodata-0.0.5/src/ecodata/IMF.py
--rw-rw-rw-   0        0        0     2111 2023-04-14 08:10:41.000000 ecodata-0.0.5/src/ecodata/OECD.py
--rw-rw-rw-   0        0        0     3441 2023-04-14 08:34:52.000000 ecodata-0.0.5/src/ecodata/YFinance.py
--rw-rw-rw-   0        0        0        0 2023-04-14 08:50:52.000000 ecodata-0.0.5/src/ecodata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:12:49.908762 ecodata-0.0.5/src/ecodata.egg-info/
--rw-rw-rw-   0        0        0     1698 2023-04-14 09:12:49.000000 ecodata-0.0.5/src/ecodata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-04-14 09:12:49.000000 ecodata-0.0.5/src/ecodata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:12:49.000000 ecodata-0.0.5/src/ecodata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-14 09:12:49.000000 ecodata-0.0.5/src/ecodata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 09:12:49.000000 ecodata-0.0.5/src/ecodata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 09:20:54.804653 ecodata-0.0.6/
+-rw-rw-rw-   0        0        0     1698 2023-04-14 09:20:54.803642 ecodata-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-04-14 09:20:36.000000 ecodata-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:20:54.804653 ecodata-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-04-14 09:20:32.000000 ecodata-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:20:54.783700 ecodata-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 09:20:54.783700 ecodata-0.0.6/src/api/
+drwxrwxrwx   0        0        0        0 2023-04-14 09:20:54.802644 ecodata-0.0.6/src/api/ecodata.egg-info/
+-rw-rw-rw-   0        0        0     1698 2023-04-14 09:20:54.000000 ecodata-0.0.6/src/api/ecodata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-04-14 09:20:54.000000 ecodata-0.0.6/src/api/ecodata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:20:54.000000 ecodata-0.0.6/src/api/ecodata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-14 09:20:54.000000 ecodata-0.0.6/src/api/ecodata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:20:54.000000 ecodata-0.0.6/src/api/ecodata.egg-info/top_level.txt
```

### Comparing `ecodata-0.0.5/PKG-INFO` & `ecodata-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extracción de series de tiempo de las seis principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/ecodata
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Ecodata
 Extracción de series de tiempo de las seis principales instituciones económicas para el Perú:
@@ -17,15 +17,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.5
+## Versión 0.0.6
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
 * Para la OCDE, se cuenta únicamente con `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
```

### Comparing `ecodata-0.0.5/README.md` & `ecodata-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.5
+## Versión 0.0.6
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
 * Para la OCDE, se cuenta únicamente con `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
```

### Comparing `ecodata-0.0.5/setup.py` & `ecodata-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='ecodata',
-    version = '0.0.5',
+    version = '0.0.6',
     authors = [
         'Mauricio Alvarado',
         'Andrei Romero'
     ],
     description = 'Extracción de series de tiempo de las seis principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mauricioalvaradoo/ecodata',
     classifier = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ], 
-    package_dir={'':'src'},
-    packages=setuptools.find_packages(where='src'),
+    package_dir={'':'src/api'},
+    packages=setuptools.find_packages(where='src/api'),
     python_requires='>=3.6',
     install_requires = [
         'pandas',
         'numpy',
         'yfinance',
         'requests'
     ]
```

### Comparing `ecodata-0.0.5/src/ecodata.egg-info/PKG-INFO` & `ecodata-0.0.6/src/api/ecodata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extracción de series de tiempo de las seis principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/ecodata
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Ecodata
 Extracción de series de tiempo de las seis principales instituciones económicas para el Perú:
@@ -17,15 +17,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.5
+## Versión 0.0.6
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
 * Para la OCDE, se cuenta únicamente con `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
```

