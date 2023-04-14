# Comparing `tmp/istatcelldata-0.5.0.tar.gz` & `tmp/istatcelldata-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istatcelldata-0.5.0.tar", max compression
+gzip compressed data, was "istatcelldata-0.5.1.tar", max compression
```

## Comparing `istatcelldata-0.5.0.tar` & `istatcelldata-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0     1076 2023-04-12 18:25:21.536175 istatcelldata-0.5.0/LICENSE
--rwxr-xr-x   0        0        0      978 2023-04-12 18:25:21.536175 istatcelldata-0.5.0/README.md
--rwxr-xr-x   0        0        0      160 2023-04-14 10:02:26.723816 istatcelldata-0.5.0/istatcelldata/__init__.py
--rwxr-xr-x   0        0        0     6598 2023-04-14 09:51:08.091179 istatcelldata-0.5.0/istatcelldata/config.py
--rwxr-xr-x   0        0        0        0 2023-04-14 09:51:08.091179 istatcelldata-0.5.0/istatcelldata/data/__init__.py
--rwxr-xr-x   0        0        0     8447 2023-04-14 09:51:08.091179 istatcelldata-0.5.0/istatcelldata/data/census_1991_2001.py
--rwxr-xr-x   0        0        0     3004 2023-04-14 09:51:08.091179 istatcelldata-0.5.0/istatcelldata/data/manage_data.py
--rwxr-xr-x   0        0        0     6547 2023-04-14 09:51:08.091179 istatcelldata-0.5.0/istatcelldata/download.py
--rwxr-xr-x   0        0        0     4989 2023-04-14 09:51:08.091179 istatcelldata-0.5.0/istatcelldata/generic.py
--rwxr-xr-x   0        0        0        0 2023-04-14 09:51:08.091179 istatcelldata-0.5.0/istatcelldata/geodata/__init__.py
--rwxr-xr-x   0        0        0     5404 2023-04-14 09:51:08.091179 istatcelldata-0.5.0/istatcelldata/geodata/manage_geodata.py
--rw-r--r--   0        0        0     3758 2023-04-14 09:55:28.125042 istatcelldata-0.5.0/istatcelldata/processes.py
--rw-r--r--   0        0        0      894 2023-04-14 10:02:13.067728 istatcelldata-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 istatcelldata-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1076 2023-04-12 18:25:21.536175 istatcelldata-0.5.1/LICENSE
+-rwxr-xr-x   0        0        0      978 2023-04-12 18:25:21.536175 istatcelldata-0.5.1/README.md
+-rwxr-xr-x   0        0        0       99 2023-04-14 10:41:50.115834 istatcelldata-0.5.1/istatcelldata/__init__.py
+-rwxr-xr-x   0        0        0     6607 2023-04-14 10:48:45.206530 istatcelldata-0.5.1/istatcelldata/config.py
+-rwxr-xr-x   0        0        0        0 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/data/__init__.py
+-rwxr-xr-x   0        0        0     8447 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/data/census_1991_2001.py
+-rwxr-xr-x   0        0        0     3004 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/data/manage_data.py
+-rwxr-xr-x   0        0        0     6547 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/download.py
+-rwxr-xr-x   0        0        0     4989 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/generic.py
+-rwxr-xr-x   0        0        0        0 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/geodata/__init__.py
+-rwxr-xr-x   0        0        0     5404 2023-04-14 09:51:08.091179 istatcelldata-0.5.1/istatcelldata/geodata/manage_geodata.py
+-rw-r--r--   0        0        0     3758 2023-04-14 09:55:28.125042 istatcelldata-0.5.1/istatcelldata/processes.py
+-rw-r--r--   0        0        0      869 2023-04-14 10:53:32.404374 istatcelldata-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 istatcelldata-0.5.1/PKG-INFO
```

### Comparing `istatcelldata-0.5.0/LICENSE` & `istatcelldata-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.0/README.md` & `istatcelldata-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.0/istatcelldata/config.py` & `istatcelldata-0.5.1/istatcelldata/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import os
 from pathlib import Path
 # from multiprocessing import cpu_count
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 log_format = '%(asctime)s | %(process)d - %(message)s'
 console_handler = logging.StreamHandler()
@@ -11,15 +10,15 @@
 logger.addHandler(console_handler)
 
 # N_CORES = cpu_count()
 
 # PROJECT
 MAIN_LINK = "https://www.istat.it/storage/cartografia"
 GLOBAL_CRS = 32632
-MAIN_PATH = Path(os.getenv("MAIN_PATH"))
+MAIN_PATH = Path("/home/max/Desktop/test")  # FOR TEST ONLY
 TARGET_YEARS = [1991, 2001, 2011]
 
 # PROJECT FOLDERS
 DATA_FOLDER = 'data'
 GEODATA_FOLDER = 'geodata'
 PREPROCESSING_FOLDER = 'preprocessing'
 CENSUS_DATA_FOLDER = 'Sezioni di Censimento'
```

### Comparing `istatcelldata-0.5.0/istatcelldata/data/census_1991_2001.py` & `istatcelldata-0.5.1/istatcelldata/data/census_1991_2001.py`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.0/istatcelldata/data/manage_data.py` & `istatcelldata-0.5.1/istatcelldata/data/manage_data.py`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.0/istatcelldata/download.py` & `istatcelldata-0.5.1/istatcelldata/download.py`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.0/istatcelldata/generic.py` & `istatcelldata-0.5.1/istatcelldata/generic.py`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.0/istatcelldata/geodata/manage_geodata.py` & `istatcelldata-0.5.1/istatcelldata/geodata/manage_geodata.py`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.0/istatcelldata/processes.py` & `istatcelldata-0.5.1/istatcelldata/processes.py`

 * *Files identical despite different names*

### Comparing `istatcelldata-0.5.0/pyproject.toml` & `istatcelldata-0.5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "istatcelldata"
-version = "0.5.0"
+version = "0.5.1"
 description = "\"Con ISTAT Cell Data puoi ottenere facilmente il set di dati riferiti ai censimenti ISTAT in cui sono stati rilasciati anche i dati delle celle censuarie.\""
 authors = ["Massimiliano Moraca <info@massimilianomoraca.it>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -12,15 +12,14 @@
 geopandas = "^0.12.2"
 tqdm = "^4.65.0"
 chardet = "^5.1.0"
 requests = "^2.28.2"
 fsspec = "^2023.4.0"
 openpyxl = "^3.1.2"
 xlrd = "^2.0.1"
-python-dotenv = "^1.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 jupyter = "^1.0.0"
 notebook = "^6.5.4"
 jupyter-server-proxy = "^3.2.2"
```

### Comparing `istatcelldata-0.5.0/PKG-INFO` & `istatcelldata-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: istatcelldata
-Version: 0.5.0
+Version: 0.5.1
 Summary: "Con ISTAT Cell Data puoi ottenere facilmente il set di dati riferiti ai censimenti ISTAT in cui sono stati rilasciati anche i dati delle celle censuarie."
 License: MIT
 Author: Massimiliano Moraca
 Author-email: info@massimilianomoraca.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
 Requires-Dist: fsspec (>=2023.4.0,<2024.0.0)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ISTAT Cell Data
```

