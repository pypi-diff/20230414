# Comparing `tmp/ecodata-0.0.2.tar.gz` & `tmp/ecodata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodata-0.0.2.tar", last modified: Fri Apr 14 08:21:53 2023, max compression
+gzip compressed data, was "ecodata-0.0.3.tar", last modified: Fri Apr 14 08:40:15 2023, max compression
```

## Comparing `ecodata-0.0.2.tar` & `ecodata-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:21:53.296599 ecodata-0.0.2/
--rw-rw-rw-   0        0        0     1698 2023-04-14 08:21:53.295601 ecodata-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-04-14 08:20:57.000000 ecodata-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 08:21:53.296599 ecodata-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-14 08:20:50.000000 ecodata-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:21:53.279643 ecodata-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 08:21:53.294609 ecodata-0.0.2/src/ecodata.egg-info/
--rw-rw-rw-   0        0        0     1698 2023-04-14 08:21:53.000000 ecodata-0.0.2/src/ecodata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-14 08:21:53.000000 ecodata-0.0.2/src/ecodata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:21:53.000000 ecodata-0.0.2/src/ecodata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-14 08:21:53.000000 ecodata-0.0.2/src/ecodata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:21:53.000000 ecodata-0.0.2/src/ecodata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 08:40:15.274411 ecodata-0.0.3/
+-rw-rw-rw-   0        0        0     1698 2023-04-14 08:40:15.274411 ecodata-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-04-14 08:36:43.000000 ecodata-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 08:40:15.274411 ecodata-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-04-14 08:36:49.000000 ecodata-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:40:15.264437 ecodata-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 08:40:15.273413 ecodata-0.0.3/src/ecodata.egg-info/
+-rw-rw-rw-   0        0        0     1698 2023-04-14 08:40:15.000000 ecodata-0.0.3/src/ecodata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-14 08:40:15.000000 ecodata-0.0.3/src/ecodata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:40:15.000000 ecodata-0.0.3/src/ecodata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-14 08:40:15.000000 ecodata-0.0.3/src/ecodata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:40:15.000000 ecodata-0.0.3/src/ecodata.egg-info/top_level.txt
```

### Comparing `ecodata-0.0.2/PKG-INFO` & `ecodata-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.0.2
+Version: 0.0.3
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
 
 
-## Versión 0.0.2
+## Versión 0.0.3
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
 * Para la OCDE, se cuenta únicamente con `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
```

### Comparing `ecodata-0.0.2/README.md` & `ecodata-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.2
+## Versión 0.0.3
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
 * Para la OCDE, se cuenta únicamente con `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
```

### Comparing `ecodata-0.0.2/setup.py` & `ecodata-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='ecodata',
-    version = '0.0.2',
+    version = '0.0.3',
     authors = [
         'Mauricio Alvarado',
         'Andrei Romero'
     ],
     description = 'Extracción de series de tiempo de las seis principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ecodata-0.0.2/src/ecodata.egg-info/PKG-INFO` & `ecodata-0.0.3/src/ecodata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.0.2
+Version: 0.0.3
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
 
 
-## Versión 0.0.2
+## Versión 0.0.3
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
 * Para la OCDE, se cuenta únicamente con `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
```

