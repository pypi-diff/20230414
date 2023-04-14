# Comparing `tmp/ecodata-0.0.3.tar.gz` & `tmp/ecodata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecodata-0.0.3.tar", last modified: Fri Apr 14 08:40:15 2023, max compression
+gzip compressed data, was "ecodata-0.0.4.tar", last modified: Fri Apr 14 09:02:29 2023, max compression
```

## Comparing `ecodata-0.0.3.tar` & `ecodata-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:40:15.274411 ecodata-0.0.3/
--rw-rw-rw-   0        0        0     1698 2023-04-14 08:40:15.274411 ecodata-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2023-04-14 08:36:43.000000 ecodata-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 08:40:15.274411 ecodata-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-14 08:36:49.000000 ecodata-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:40:15.264437 ecodata-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 08:40:15.273413 ecodata-0.0.3/src/ecodata.egg-info/
--rw-rw-rw-   0        0        0     1698 2023-04-14 08:40:15.000000 ecodata-0.0.3/src/ecodata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-14 08:40:15.000000 ecodata-0.0.3/src/ecodata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:40:15.000000 ecodata-0.0.3/src/ecodata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-14 08:40:15.000000 ecodata-0.0.3/src/ecodata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:40:15.000000 ecodata-0.0.3/src/ecodata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 09:02:29.371135 ecodata-0.0.4/
+-rw-rw-rw-   0        0        0     1698 2023-04-14 09:02:29.370107 ecodata-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1414 2023-04-14 09:02:13.000000 ecodata-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:02:29.371135 ecodata-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-04-14 09:02:03.000000 ecodata-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:02:29.352156 ecodata-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 09:02:29.369110 ecodata-0.0.4/src/ecodata.egg-info/
+-rw-rw-rw-   0        0        0     1698 2023-04-14 09:02:29.000000 ecodata-0.0.4/src/ecodata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-14 09:02:29.000000 ecodata-0.0.4/src/ecodata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:02:29.000000 ecodata-0.0.4/src/ecodata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-14 09:02:29.000000 ecodata-0.0.4/src/ecodata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:02:29.000000 ecodata-0.0.4/src/ecodata.egg-info/top_level.txt
```

### Comparing `ecodata-0.0.3/PKG-INFO` & `ecodata-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecodata
-Version: 0.0.3
+Version: 0.0.4
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
 
 
-## Versión 0.0.3
+## Versión 0.0.4
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
 * Para la OCDE, se cuenta únicamente con `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
```

### Comparing `ecodata-0.0.3/README.md` & `ecodata-0.0.4/src/ecodata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: ecodata
+Version: 0.0.4
+Summary: Extracción de series de tiempo de las seis principales instituciones económicas para el Perú
+Home-page: https://github.com/mauricioalvaradoo/ecodata
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # Ecodata
 Extracción de series de tiempo de las seis principales instituciones económicas para el Perú:
 1. BCRP
 2. YahooFinance
 3. FRED
 4. IMF
 5. WorldBank
@@ -9,15 +17,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.3
+## Versión 0.0.4
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
 * Para la OCDE, se cuenta únicamente con `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
```

### Comparing `ecodata-0.0.3/setup.py` & `ecodata-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='ecodata',
-    version = '0.0.3',
+    version = '0.0.4',
     authors = [
         'Mauricio Alvarado',
         'Andrei Romero'
     ],
     description = 'Extracción de series de tiempo de las seis principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ecodata-0.0.3/src/ecodata.egg-info/PKG-INFO` & `ecodata-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: ecodata
-Version: 0.0.3
-Summary: Extracción de series de tiempo de las seis principales instituciones económicas para el Perú
-Home-page: https://github.com/mauricioalvaradoo/ecodata
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # Ecodata
 Extracción de series de tiempo de las seis principales instituciones económicas para el Perú:
 1. BCRP
 2. YahooFinance
 3. FRED
 4. IMF
 5. WorldBank
@@ -17,15 +9,15 @@
 
 ```
 # Instalación mediante PyPI
 !pip install ecodata
 ```
 
 
-## Versión 0.0.3
+## Versión 0.0.4
 * Para el Banco Central de Reserva del Perú (`BCRP`), `Yahoo Finance`, Federal Reserve Economic Data (`FRED`) y el `World Bank`, se cuenta con ambas métodos: `get_data()` y `search()`.
 * Para el IMF, únicamente se cuenta únicamente con `search()`. Recomendamos por el momento extraer las series en [EconDB](https://www.econdb.com/tree/).
 * Para la OCDE, se cuenta únicamente con `get_data()`.
 
 
 ## Métodos
 Para cada institución se tienen dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
```

