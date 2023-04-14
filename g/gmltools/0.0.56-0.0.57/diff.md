# Comparing `tmp/gmltools-0.0.56.tar.gz` & `tmp/gmltools-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.56.tar", last modified: Fri Apr 14 09:40:06 2023, max compression
+gzip compressed data, was "gmltools-0.0.57.tar", last modified: Fri Apr 14 10:10:15 2023, max compression
```

## Comparing `gmltools-0.0.56.tar` & `gmltools-0.0.57.tar`

### file list

```diff
@@ -1,45 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:06.726581 gmltools-0.0.56/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.56/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.56/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-14 09:40:06.726581 gmltools-0.0.56/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.56/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:06.662185 gmltools-0.0.56/dist/
--rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.56/dist/gmltools-0.0.24.tar.gz
--rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.56/dist/gmltools-0.0.25.tar.gz
--rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.56/dist/gmltools-0.0.26.tar.gz
--rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.56/dist/gmltools-0.0.27.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.56/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.56/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-14 09:39:18.000000 gmltools-0.0.56/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 09:40:06.727569 gmltools-0.0.56/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-14 09:39:00.000000 gmltools-0.0.56/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:06.630687 gmltools-0.0.56/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:06.665664 gmltools-0.0.56/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.56/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.56/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:06.702863 gmltools-0.0.56/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.56/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.56/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:06.713163 gmltools-0.0.56/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.56/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.56/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.56/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5137 2023-04-14 09:39:40.000000 gmltools-0.0.56/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   118688 2023-04-12 11:41:49.000000 gmltools-0.0.56/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.56/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    12541 2023-04-14 08:51:00.000000 gmltools-0.0.56/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:06.718611 gmltools-0.0.56/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.56/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.56/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.56/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:06.725598 gmltools-0.0.56/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.56/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.56/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.56/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.56/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:06.700871 gmltools-0.0.56/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-14 09:40:06.000000 gmltools-0.0.56/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1018 2023-04-14 09:40:06.000000 gmltools-0.0.56/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:40:06.000000 gmltools-0.0.56/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-14 09:40:06.000000 gmltools-0.0.56/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 09:40:06.000000 gmltools-0.0.56/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.176044 gmltools-0.0.57/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.57/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.57/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-14 10:10:15.176044 gmltools-0.0.57/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.57/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.053370 gmltools-0.0.57/dist/
+-rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.57/dist/gmltools-0.0.24.tar.gz
+-rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.57/dist/gmltools-0.0.25.tar.gz
+-rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.57/dist/gmltools-0.0.26.tar.gz
+-rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.57/dist/gmltools-0.0.27.tar.gz
+-rw-rw-rw-   0        0        0    53751 2023-03-21 09:33:58.000000 gmltools-0.0.57/dist/gmltools-0.0.28.tar.gz
+-rw-rw-rw-   0        0        0    53762 2023-03-21 09:53:00.000000 gmltools-0.0.57/dist/gmltools-0.0.29.tar.gz
+-rw-rw-rw-   0        0        0    56221 2023-03-22 10:45:28.000000 gmltools-0.0.57/dist/gmltools-0.0.30.tar.gz
+-rw-rw-rw-   0        0        0    56607 2023-03-22 12:13:29.000000 gmltools-0.0.57/dist/gmltools-0.0.31.tar.gz
+-rw-rw-rw-   0        0        0    56619 2023-03-22 12:20:22.000000 gmltools-0.0.57/dist/gmltools-0.0.32.tar.gz
+-rw-rw-rw-   0        0        0    56655 2023-03-22 12:28:41.000000 gmltools-0.0.57/dist/gmltools-0.0.33.tar.gz
+-rw-rw-rw-   0        0        0    56667 2023-03-22 12:31:59.000000 gmltools-0.0.57/dist/gmltools-0.0.34.tar.gz
+-rw-rw-rw-   0        0        0    56681 2023-03-22 12:46:07.000000 gmltools-0.0.57/dist/gmltools-0.0.35.tar.gz
+-rw-rw-rw-   0        0        0    56537 2023-03-23 10:43:13.000000 gmltools-0.0.57/dist/gmltools-0.0.36.tar.gz
+-rw-rw-rw-   0        0        0    56554 2023-03-23 10:47:16.000000 gmltools-0.0.57/dist/gmltools-0.0.37.tar.gz
+-rw-rw-rw-   0        0        0   284440 2023-03-30 08:43:02.000000 gmltools-0.0.57/dist/gmltools-0.0.38.tar.gz
+-rw-rw-rw-   0        0        0   284496 2023-03-30 10:53:02.000000 gmltools-0.0.57/dist/gmltools-0.0.39.tar.gz
+-rw-rw-rw-   0        0        0   284866 2023-04-04 08:49:39.000000 gmltools-0.0.57/dist/gmltools-0.0.40.tar.gz
+-rw-rw-rw-   0        0        0   286391 2023-04-11 09:53:19.000000 gmltools-0.0.57/dist/gmltools-0.0.41.tar.gz
+-rw-rw-rw-   0        0        0   289831 2023-04-12 10:45:06.000000 gmltools-0.0.57/dist/gmltools-0.0.42.tar.gz
+-rw-rw-rw-   0        0        0   289829 2023-04-12 10:52:27.000000 gmltools-0.0.57/dist/gmltools-0.0.43.tar.gz
+-rw-rw-rw-   0        0        0   289837 2023-04-12 10:56:44.000000 gmltools-0.0.57/dist/gmltools-0.0.44.tar.gz
+-rw-rw-rw-   0        0        0   289819 2023-04-12 11:03:49.000000 gmltools-0.0.57/dist/gmltools-0.0.45.tar.gz
+-rw-rw-rw-   0        0        0   289827 2023-04-12 11:09:04.000000 gmltools-0.0.57/dist/gmltools-0.0.46.tar.gz
+-rw-rw-rw-   0        0        0   289863 2023-04-12 11:18:58.000000 gmltools-0.0.57/dist/gmltools-0.0.47.tar.gz
+-rw-rw-rw-   0        0        0   291078 2023-04-13 10:45:14.000000 gmltools-0.0.57/dist/gmltools-0.0.48.tar.gz
+-rw-rw-rw-   0        0        0   291024 2023-04-13 10:48:46.000000 gmltools-0.0.57/dist/gmltools-0.0.49.tar.gz
+-rw-rw-rw-   0        0        0   291054 2023-04-13 11:27:27.000000 gmltools-0.0.57/dist/gmltools-0.0.50.tar.gz
+-rw-rw-rw-   0        0        0   291079 2023-04-13 11:38:27.000000 gmltools-0.0.57/dist/gmltools-0.0.51.tar.gz
+-rw-rw-rw-   0        0        0   291069 2023-04-13 11:45:59.000000 gmltools-0.0.57/dist/gmltools-0.0.52.tar.gz
+-rw-rw-rw-   0        0        0   291231 2023-04-14 07:56:54.000000 gmltools-0.0.57/dist/gmltools-0.0.53.tar.gz
+-rw-rw-rw-   0        0        0   291232 2023-04-14 08:02:57.000000 gmltools-0.0.57/dist/gmltools-0.0.54.tar.gz
+-rw-rw-rw-   0        0        0   291334 2023-04-14 08:49:47.000000 gmltools-0.0.57/dist/gmltools-0.0.55.tar.gz
+-rw-rw-rw-   0        0        0   292622 2023-04-14 09:40:06.000000 gmltools-0.0.57/dist/gmltools-0.0.56.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.57/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.57/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-14 10:09:26.000000 gmltools-0.0.57/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 10:10:15.177117 gmltools-0.0.57/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-14 10:09:18.000000 gmltools-0.0.57/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:10:14.987388 gmltools-0.0.57/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.055361 gmltools-0.0.57/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.57/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.57/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.092792 gmltools-0.0.57/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.57/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.57/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.152515 gmltools-0.0.57/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.57/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.57/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.57/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5137 2023-04-14 09:39:40.000000 gmltools-0.0.57/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   119050 2023-04-14 10:09:03.000000 gmltools-0.0.57/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.57/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    12588 2023-04-14 09:47:45.000000 gmltools-0.0.57/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.162087 gmltools-0.0.57/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.57/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.57/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.57/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.173056 gmltools-0.0.57/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.57/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.57/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.57/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.57/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.087843 gmltools-0.0.57/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-14 10:10:14.000000 gmltools-0.0.57/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-04-14 10:10:14.000000 gmltools-0.0.57/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 10:10:14.000000 gmltools-0.0.57/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-14 10:10:14.000000 gmltools-0.0.57/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 10:10:14.000000 gmltools-0.0.57/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.56/LICENSE` & `gmltools-0.0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/Models.ipynb` & `gmltools-0.0.57/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/PKG-INFO` & `gmltools-0.0.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.56
+Version: 0.0.57
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.56/README.md` & `gmltools-0.0.57/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/dist/gmltools-0.0.24.tar.gz` & `gmltools-0.0.57/dist/gmltools-0.0.24.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/dist/gmltools-0.0.25.tar.gz` & `gmltools-0.0.57/dist/gmltools-0.0.25.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/dist/gmltools-0.0.26.tar.gz` & `gmltools-0.0.57/dist/gmltools-0.0.26.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/dist/gmltools-0.0.27.tar.gz` & `gmltools-0.0.57/dist/gmltools-0.0.27.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/gmltools.yml` & `gmltools-0.0.57/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/mltools.yml` & `gmltools-0.0.57/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/pyproject.toml` & `gmltools-0.0.57/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.56"
+version = "0.0.57"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.56/setup.py` & `gmltools-0.0.57/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.56',
+    'version': '0.0.57',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.56/src/gmltools/To_Do.txt` & `gmltools-0.0.57/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools/eda/eda.py` & `gmltools-0.0.57/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools/models/bayes.py` & `gmltools-0.0.57/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.57/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools/models/dummy_model.py` & `gmltools-0.0.57/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools/models/model.py` & `gmltools-0.0.57/src/gmltools/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
             elif self.pipe.steps[-1][0] == 'LR':
                 self._model.fit(self.X_train, self.y_train, LR__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             elif self.pipe.steps[-1][0] == 'MLP':
                 self._model.fit(self.X_train, self.y_train, MLP__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             elif self.pipe.steps[-1][0] == 'DT':
                 self._model.fit(self.X_train, self.y_train, DT__sample_weight=self.sample_weights, X_prev = X_prev,columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
         else:
-            self._model.fit(self.X_train, self.y_train, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
+            self._model.fit(X=self.X_train, y=self.y_train, X_prev = X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
 
         return self._model
 
 
     
     
     
@@ -354,26 +354,26 @@
     RandomForest_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     XGBoost_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     LogisticRegression_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     DecisionTree_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     KNN_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     MLP_Classifier_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
 
-    def __init__(self, model_name, X_train=None, y_train=None):
+    def __init__(self, model_name, X_train=None, y_train=None, cv=10):
         self.model = None
         self.model_name = model_name
         self.X_train = X_train
         self.y_train = y_train
+        self.cv = cv
     def RandomForest_Classifier(self, ordinal_cat_cols:List[str]=None,
                                 scoring='accuracy', class_weight=None,
                                 grid_params:dict={'RFC__n_estimators': [100, 200],
                                             'RFC__max_depth': [None, 10, 20],
                                             'RFC__min_samples_split': [2, 5],
                                             'RFC__max_features': ['sqrt', None]},
-                                cv=10,
                                 random_params:dict=None,
                                 random_n_iter:int=10,
                                 bayes_pbounds:dict=None,
                                 bayes_int_params:List[str]=None, 
                                 bayes_n_iter:int=30,
                                 criterion='gini',
                                 sample_weight=None,
@@ -447,31 +447,31 @@
             assert all('RF__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'RF__'"
     
         #Preprocess the data automatically
         preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
         pipe = Pipeline(steps=[('Prep', preprocessor),
                             ('RF', RandomForestRegressor(criterion=criterion,random_state=random_state,n_jobs=n_jobs,class_weight=class_weight))]) # Model always the last step
         #Select Grid Search, Random Search or Bayesian Optimization
-        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
         select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         self.model=select_searchcv.fit()
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), "Class_Weights":str(class_weight), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
-                                    'scoring':str(scoring), 'cv':str(cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight)}
+                                    'scoring':str(scoring), 'cv':str(self.cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight)}
         
 
     
     def XGBoost_Classifier( self, ordinal_cat_cols:list=None,
                             scoring='accuracy', eval_metric='merror',
                             objective='multi:softmax', grid_params:dict={},
-                            cv=10, random_params:dict=None, random_n_iter:int=10,
+                            random_params:dict=None, random_n_iter:int=10,
                             bayes_pbounds:dict=None,bayes_int_params:List[str]=None, 
                             bayes_n_iter:int=30, random_state:int=None,
                             sample_weight=None, n_jobs=-1):  
         """
         This method performs a XGBoost classification model with grid search or bayesian optimization.
 
 
@@ -548,32 +548,32 @@
                             ('XGB', XGBClassifier(
                                 random_state=random_state,
                                 n_jobs=n_jobs, 
                                 verbosity=0,
                                 eval_metric=eval_metric,
                                 objective=objective))]) # Model always the last step
         #Select Grid Search, Random Search or Bayesian Optimization
-        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
         select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         self.model=select_searchcv.fit()
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 
-                                    'scoring':str(scoring), 'cv':str(cv), 'eval_metric':str(eval_metric), 'sample_weight':str(sample_weight), "objective":str(objective)}
+                                    'scoring':str(scoring), 'cv':str(self.cv), 'eval_metric':str(eval_metric), 'sample_weight':str(sample_weight), "objective":str(objective)}
 
     
     def LogisticRegression_Classifier(self,  ordinal_cat_cols:List[str]=None, scoring='accuracy',
                                     grid_params = {'LR__C': [0.1, 1, 10],
                                     'LR__penalty': ['l1', 'l2', 'elasticnet'],
                                     'LR__multi_class': ['ovr', 'multinomial'],   
                                     'LR__solver': ['newton-cg', 'lbfgs', 'liblinear', 'sag', 'saga']},
-                                    cv=10, random_params:dict=None, random_n_iter:int=10,
+                                    random_params:dict=None, random_n_iter:int=10,
                                     bayes_pbounds:dict=None, bayes_int_params:List[str]=None, 
                                     bayes_n_iter:int=30, random_state:int=None, class_weight=None, sample_weight=None,
                                     n_jobs:int=-1 , tol:float=0.0001, max_iter:int=1000):
         """
         This method performs a Logistic Regression classification model with grid search or bayesian optimization.
 
         Parameters
@@ -665,31 +665,31 @@
                                     n_jobs=n_jobs, 
                                     verbose=0,
                                     warm_start=False,
                                     fit_intercept=True,
                                     intercept_scaling=1,
                                     dual=False))]) # Model always the last step
         #Select Grid Search, Random Search or Bayesian Optimization
-        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
         select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         self.model=select_searchcv.fit()
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), "Class Weight":str(class_weight), 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 
-                                    'scoring':str(scoring), 'cv':str(cv), 'tol':str(tol), 'sample_weight':str(sample_weight), "max_iter":str(max_iter)}
+                                    'scoring':str(scoring), 'cv':str(self.cv), 'tol':str(tol), 'sample_weight':str(sample_weight), "max_iter":str(max_iter)}
   
         
     
     def MLP_Classifier(self,ordinal_cat_cols=None, scoring='accuracy',
                        grid_params={'MLP__alpha': [1e-9,1e-7,1e-5,0.001,0.01],
                         'MLP__hidden_layer_sizes':[(5,),(10,),(15,),(20,),(25,)]},
-                        cv=10, random_params=None, random_n_iter=10,
+                        random_params=None, random_n_iter=10,
                         bayes_pbounds=None, bayes_int_params=None, bayes_n_iter=30, 
                         random_state=None, n_jobs=-1, solver='lbfgs',
                         activation='logistic', tol=1e-4, max_iter=450, early_stopping=False,
                        learning_rate='constant',learning_rate_init=0.001,verbose=True, sample_weight=None):
         
         """
         This method performs a Multi Layer Perceptron classification model with grid search or bayesian optimization.
@@ -798,32 +798,32 @@
                                                     random_state=random_state,
                                                     verbose = verbose,
                                                     early_stopping=early_stopping,
                                                     learning_rate=learning_rate,
                                                     learning_rate_init=learning_rate_init
                                                     ))]) # Model always the last step
         #Select Grid Search, Random Search or Bayesian Optimization
-        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
         select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         self.model=select_searchcv.fit()
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), "Early Stopping":str(early_stopping), 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape),
-                                    'scoring':str(scoring), 'cv':str(cv), 'tol':str(tol), 'sample_weight':str(sample_weight), "max_iter":str(max_iter), "Learning Rate":str(learning_rate), "Learning Rate Init":str(learning_rate_init)}
+                                    'scoring':str(scoring), 'cv':str(self.cv), 'tol':str(tol), 'sample_weight':str(sample_weight), "max_iter":str(max_iter), "Learning Rate":str(learning_rate), "Learning Rate Init":str(learning_rate_init)}
         
         
 
 
     #do the same for knn_classifier
     def KNN_Classifier(self,ordinal_cat_cols=None, scoring='accuracy',
                         grid_params={'KNN__n_neighbors': [3,10,25,60]},
-                        cv=10, random_params=None, random_n_iter=10,  bayes_pbounds=None,
+                        random_params=None, random_n_iter=10,  bayes_pbounds=None,
                         bayes_int_params=None, bayes_n_iter=30, sample_weight=None,
                         random_state=None, n_jobs=-1):
           
         """
         This method performs a K-Nearest Neighbors classification model with grid search or bayesian optimization.
 
         Parameters
@@ -900,24 +900,24 @@
             assert all('KNN__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'KNN__'"
             assert all('KNN__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'KNN__'"
         
         preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
         pipe = Pipeline(steps=[('Prep', preprocessor),
                             ('KNN', KNeighborsClassifier(n_jobs=n_jobs, random_state=random_state))]) # Model always the last step
         #Select Grid Search, Random Search or Bayesian Optimization
-        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
         select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         self.model=select_searchcv.fit()
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 
-                                    'scoring':str(scoring), 'cv':str(cv),  'sample_weight':str(sample_weight)}
+                                    'scoring':str(scoring), 'cv':str(self.cv),  'sample_weight':str(sample_weight)}
 
 
 
     
 
     #do the same for a decision tree
     def DecisionTree_Classifier(self, ordinal_cat_cols=None, scoring='accuracy',
@@ -999,24 +999,24 @@
             assert all('DT__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'DT__'"
             assert all('DT__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'DT__'"
 
         preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
         pipe = Pipeline(steps=[('Prep', preprocessor),
                             ('DT', DecisionTreeClassifier(random_state=random_state,class_weight=class_weight))]) # Model always the last step
         #Select Grid Search, Random Search or Bayesian Optimization
-        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+        select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
         select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         self.model=select_searchcv.fit()
         
         #generate a dictionary with all the parameters used in the model
         self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
         
         self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), "Class Weight": class_weight, 'random_state':str(random_state),
                                     'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape),
-                                    'scoring':str(scoring), 'cv':str(cv),  'sample_weight':str(sample_weight)}
+                                    'scoring':str(scoring), 'cv':str(self.cv),  'sample_weight':str(sample_weight)}
 
     #save model
     def save(self, return_best_metrics:bool=True):
         """
         Saves the model to a file. And saves the cv results if exists grid search or random search as an excel file.
 
         Parameters
@@ -1151,28 +1151,29 @@
     RandomForest_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     XGBoost_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     LogisticRegression_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     DecisionTree_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     KNN_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
     MLP_Regressor_Description = "Sustituir por desciprion que inlcuya los pros y contras del modelo guardado en models_info.py"
 
-    def __init__(self,model_name:str, X_train=None, y_train=None, X_prev=None):
+    def __init__(self,model_name:str, X_train=None, y_train=None, X_prev=None, cv=10):
         self.model = None
         self.model_name = model_name
         self.X_train = X_train
         self.y_train = y_train
         self.X_prev = X_prev
+        self.cv = cv
 
     def RandomForest_Regressor(self,  ordinal_cat_cols=None, scoring='neg_mean_squared_error', criterion="friedman_mse",
                             grid_params={'RF__n_estimators': [100, 200, 300, 400, 500],
                                 'RF__max_depth': [3,5,7,10],
                                 'RF__min_samples_split': [2,3,4],
                                 'RF__min_samples_leaf': [4,5,6],
                                 'RF__max_features': ['auto','sqrt','log2',None]}, 
-                            cv=10, random_params=None, random_n_iter = 10, bayes_pbounds=None, 
+                            random_params=None, random_n_iter = 10, bayes_pbounds=None, 
                             bayes_int_params=None, bayes_n_iter = 30, sample_weight=None, random_state=None, n_jobs=-1, 
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
             """
             This method performs a Random Forest regression model with grid search or bayesian optimization.
     
             Parameters
@@ -1246,36 +1247,36 @@
                 assert all('RF__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'RF__'"
 
             #Preprocess the data automatically
             preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('RF', RandomForestRegressor(criterion=criterion,random_state=random_state,n_jobs=n_jobs))]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
-            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
-                                        'scoring':str(scoring), 'cv':str(cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+                                        'scoring':str(scoring), 'cv':str(self.cv), 'criterion':str(criterion), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
 
     
     def XGB_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'XGB__n_estimators': [100, 200, 300, 400, 500],
                                 'XGB__max_depth': [3,5,7,10],
                                 'XGB__learning_rate': [0.01,0.05,0.1,0.15,0.2],
                                 'XGB__min_child_weight': [1,3,5,7],
                                 'XGB__gamma': [0.0,0.1,0.2,0.3,0.4],
                                 'XGB__colsample_bytree': [0.3,0.4,0.5,0.7]}, 
-                            cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None, bayes_int_params=None,
+                            random_params=None, random_n_iter=10, bayes_pbounds=None, bayes_int_params=None,
                             bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
             """
             This method performs a XGBoost regression model with grid search or bayesian optimization.
     
             Parameters
@@ -1349,34 +1350,34 @@
             
 
             #Preprocess the data automatically
             preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('XGB', XGBRegressor(random_state=random_state,n_jobs=n_jobs))]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
-            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
-                                        'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+                                        'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
 
 
     
     def Linear_Regression(self,  ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'LR__fit_intercept': [True, False],
                                 'LR__normalize': [True, False],
                                 'LR__copy_X': [True, False]}, 
-                            cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None,
+                            random_params=None, random_n_iter=10, bayes_pbounds=None,
                             bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
             """
             This method performs a Linear Regression model with grid search or bayesian optimization.
     
             Parameters
@@ -1448,35 +1449,35 @@
                 assert all('LR__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'LR__'"
                 assert all('LR__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'LR__'"
             
             preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('LR', LinearRegression())]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
-            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
-                                        'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+                                        'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
 
     
     def KNN_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'KNN__n_neighbors': [3,5,7,9,11,13,15,17,19,21,23,25,27,29,31,33,35,37,39,41,43,45,47,49,51,53,55,57,59,61,63,65,67,69,71,73,75,77,79,81,83,85,87,89,91,93,95,97,99],
                                 'KNN__weights': ['uniform', 'distance'],
                                 'KNN__algorithm': ['auto', 'ball_tree', 'kd_tree', 'brute'],
                                 'KNN__leaf_size': [10,20,30,40,50,60,70,80,90,100],
                                 'KNN__p': [1,2]}, 
-                            cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None, bayes_int_params=None,
+                            random_params=None, random_n_iter=10, bayes_pbounds=None, bayes_int_params=None,
                             bayes_n_iter=30, sample_weight=None ,random_state=None, n_jobs=-1, 
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
             """
             This method performs a KNN Regressor model with grid search or bayesian optimization.
     
             Parameters
@@ -1548,37 +1549,37 @@
                 assert all('KNN__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'KNN__'"
                 assert all('KNN__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'KNN__'"
 
             preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('KNN', KNeighborsRegressor())]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
-            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
-                                        'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+                                        'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
     
 
 
     
     def DecisionTree_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'DT__criterion': ["squared_error", "friedman_mse", "absolute_error", "poisson"],
                                 'DT__max_depth': [None,2,3,4,5],
                                 'DT__min_samples_split': [2,3,4,],
                                 'DT__max_features': ['auto', 'sqrt', 'log2'],
                                 'DT__min_impurity_decrease': [0.0,0.1,0.2]}, 
-                            cv=10, random_params=None, random_n_iter=10, bayes_pbounds=None,
+                            random_params=None, random_n_iter=10, bayes_pbounds=None,
                             bayes_int_params=None, bayes_n_iter=30, sample_weight=None, random_state=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             
             """
             This method performs a Decision Tree Regressor model with grid search or bayesian optimization.
     
             Parameters
@@ -1650,35 +1651,35 @@
                 assert all('DT__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'DT__'"
                 assert all('DT__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'DT__'"
             
             preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('DT', DecisionTreeRegressor(random_state=random_state))]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
-            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
-                                        'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+                                        'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
             print(self.model.best_params_)
 
     
     def MLP_Regressor(self, ordinal_cat_cols=None, scoring='neg_mean_squared_error',
                             grid_params={'MLP__hidden_layer_sizes': [(3,),(5,)],
                                 'MLP__activation': ['identity', 'logistic', 'tanh', 'relu'],
                                 'MLP__solver': ['lbfgs', 'sgd', 'adam'],
                                 'MLP__alpha': [0.0001,0.001,0.01,0.1,1,10,100],
                                 'MLP__max_iter': [200]},
-                            cv=10, random_params=None, random_n_iter=10,bayes_pbounds=None,
+                            random_params=None, random_n_iter=10,bayes_pbounds=None,
                             bayes_int_params=None, bayes_n_iter=30, sample_weight=None,random_state=None, n_jobs=-1,
                             columns_lags=None, column_rolled_lags=None,lags=None,rolled_lags=None, rolled_metrics=None, column_rolled_lags_initial=None):
             """
             Trains a MLP Regressor model.
 
             Parameters
             ----------
@@ -1755,25 +1756,25 @@
                 assert all('MLP__' in s for s in bayes_pbounds.keys()), "In case of bayesian optimization, bayes_pbounds must start with 'MLP__'"
                 assert all('MLP__' in s for s in bayes_int_params), "In case of bayesian optimization, bayes_int_params must start with 'MLP__'"
 
             preprocessor=self._automatic_preprocessor(self.X_train,ordinal_cat_cols)
             pipe = Pipeline(steps=[('Prep', preprocessor),
                                 ('MLP', MLPRegressor(random_state=random_state))]) # Model always the last step
             #Select Grid Search, Random Search or Bayesian Optimization
-            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=cv,n_jobs=n_jobs)
+            select_searchcv=SelectSearchCV(self.X_train, self.y_train, pipe, scoring, sample_weight=sample_weight,cv=self.cv,n_jobs=n_jobs)
             select_searchcv.select_automatic(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self.model=select_searchcv.fit(X_prev=self.X_prev, columns_lags=columns_lags, column_rolled_lags=column_rolled_lags,lags=lags,rolled_lags=rolled_lags, rolled_metrics=rolled_metrics, column_rolled_lags_initial=column_rolled_lags_initial)
             
             #generate a dictionary with all the parameters used in the model
             self._search_not_none_params = self._not_none_search(grid_params, random_params, random_n_iter, bayes_pbounds, bayes_int_params, bayes_n_iter)
             self._recursive_not_none_params = self._not_none_recursive(columns_lags, column_rolled_lags,lags,rolled_lags, rolled_metrics, column_rolled_lags_initial)
             
             self._overall_dict_params = {'X_vars': str(self.X_train.columns), "SearchParams": str(self._search_not_none_params), 'ordinal_cat_cols':str(ordinal_cat_cols), 'random_state':str(random_state),
                                         'n_jobs':str(n_jobs), 'Shape X_train': str(self.X_train.shape),'Shape y_train':str(self.y_train.shape), 'Shape X_prev':str([self.X_prev.shape if self.X_prev is not None else None]),
-                                        'scoring':str(scoring), 'cv':str(cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
+                                        'scoring':str(scoring), 'cv':str(self.cv), 'sample_weight':str(sample_weight), 'Recursive Params': str(self._recursive_not_none_params)}
         
             print(self.model.best_params_)
 
     
 
     def save(self,return_best_metrics:bool=True):
         """
@@ -1797,14 +1798,18 @@
             os.makedirs(path)
 
         joblib.dump(self.model, os.path.join(path, self.model_name+'.joblib'))
         #save cv results if exists grid search or random search
         if hasattr(self.model, 'cv_results_'):
             df = pd.DataFrame(self.model.cv_results_)
             df.sort_values('rank_test_score', inplace=True)
+            if hasattr(self.cv, 'is_timeseriesinitialsplit'):
+                #rename the split columns
+                new_column_names = self.cv.get_test_days(self.X_train)
+                df.rename(columns=dict(zip(df.filter(regex='split').columns, new_column_names)), inplace=True)
             df.to_excel(os.path.join(path, self.model_name+'_cv_results.xlsx'), index=False)
 
             #save the best register of the cv_results in a second sheet of excel file called summary_models.xlsx
             df_best = pd.DataFrame(df.iloc[0]).T
             df_best["Search conditions"]=str(self._overall_dict_params)
             df_best['model_name'] = self.model_name
             #set model_name the firts column and Search conditions the second column
```

### Comparing `gmltools-0.0.56/src/gmltools/models/models_info.py` & `gmltools-0.0.57/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.57/src/gmltools/models/timeseriesplit.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     """
 
     def __init__(self, initial=7 * 3, increment_size=7, gap=0,intra_gap=0):
         self.initial = initial
         self.increment_size = increment_size
         self.gap = gap
         self.intra_gap=intra_gap
+        self.is_timeseriesinitialsplit = True
 
 
     def split(self, X, y=None, groups=None):
         """Generate indices to split data into training and test set.
         Parameters:
             X : array-like of shape (n_samples, n_features)
                 Training data, where `n_samples` is the number of samples
```

### Comparing `gmltools-0.0.56/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.57/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.57/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.57/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.57/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.57/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.56/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.57/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.56
+Version: 0.0.57
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

