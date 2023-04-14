# Comparing `tmp/gmltools-0.0.57.tar.gz` & `tmp/gmltools-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.57.tar", last modified: Fri Apr 14 10:10:15 2023, max compression
+gzip compressed data, was "gmltools-0.0.58.tar", last modified: Fri Apr 14 10:29:49 2023, max compression
```

## Comparing `gmltools-0.0.57.tar` & `gmltools-0.0.58.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.176044 gmltools-0.0.57/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.57/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.57/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-04-14 10:10:15.176044 gmltools-0.0.57/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.57/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.053370 gmltools-0.0.57/dist/
--rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.57/dist/gmltools-0.0.24.tar.gz
--rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.57/dist/gmltools-0.0.25.tar.gz
--rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.57/dist/gmltools-0.0.26.tar.gz
--rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.57/dist/gmltools-0.0.27.tar.gz
--rw-rw-rw-   0        0        0    53751 2023-03-21 09:33:58.000000 gmltools-0.0.57/dist/gmltools-0.0.28.tar.gz
--rw-rw-rw-   0        0        0    53762 2023-03-21 09:53:00.000000 gmltools-0.0.57/dist/gmltools-0.0.29.tar.gz
--rw-rw-rw-   0        0        0    56221 2023-03-22 10:45:28.000000 gmltools-0.0.57/dist/gmltools-0.0.30.tar.gz
--rw-rw-rw-   0        0        0    56607 2023-03-22 12:13:29.000000 gmltools-0.0.57/dist/gmltools-0.0.31.tar.gz
--rw-rw-rw-   0        0        0    56619 2023-03-22 12:20:22.000000 gmltools-0.0.57/dist/gmltools-0.0.32.tar.gz
--rw-rw-rw-   0        0        0    56655 2023-03-22 12:28:41.000000 gmltools-0.0.57/dist/gmltools-0.0.33.tar.gz
--rw-rw-rw-   0        0        0    56667 2023-03-22 12:31:59.000000 gmltools-0.0.57/dist/gmltools-0.0.34.tar.gz
--rw-rw-rw-   0        0        0    56681 2023-03-22 12:46:07.000000 gmltools-0.0.57/dist/gmltools-0.0.35.tar.gz
--rw-rw-rw-   0        0        0    56537 2023-03-23 10:43:13.000000 gmltools-0.0.57/dist/gmltools-0.0.36.tar.gz
--rw-rw-rw-   0        0        0    56554 2023-03-23 10:47:16.000000 gmltools-0.0.57/dist/gmltools-0.0.37.tar.gz
--rw-rw-rw-   0        0        0   284440 2023-03-30 08:43:02.000000 gmltools-0.0.57/dist/gmltools-0.0.38.tar.gz
--rw-rw-rw-   0        0        0   284496 2023-03-30 10:53:02.000000 gmltools-0.0.57/dist/gmltools-0.0.39.tar.gz
--rw-rw-rw-   0        0        0   284866 2023-04-04 08:49:39.000000 gmltools-0.0.57/dist/gmltools-0.0.40.tar.gz
--rw-rw-rw-   0        0        0   286391 2023-04-11 09:53:19.000000 gmltools-0.0.57/dist/gmltools-0.0.41.tar.gz
--rw-rw-rw-   0        0        0   289831 2023-04-12 10:45:06.000000 gmltools-0.0.57/dist/gmltools-0.0.42.tar.gz
--rw-rw-rw-   0        0        0   289829 2023-04-12 10:52:27.000000 gmltools-0.0.57/dist/gmltools-0.0.43.tar.gz
--rw-rw-rw-   0        0        0   289837 2023-04-12 10:56:44.000000 gmltools-0.0.57/dist/gmltools-0.0.44.tar.gz
--rw-rw-rw-   0        0        0   289819 2023-04-12 11:03:49.000000 gmltools-0.0.57/dist/gmltools-0.0.45.tar.gz
--rw-rw-rw-   0        0        0   289827 2023-04-12 11:09:04.000000 gmltools-0.0.57/dist/gmltools-0.0.46.tar.gz
--rw-rw-rw-   0        0        0   289863 2023-04-12 11:18:58.000000 gmltools-0.0.57/dist/gmltools-0.0.47.tar.gz
--rw-rw-rw-   0        0        0   291078 2023-04-13 10:45:14.000000 gmltools-0.0.57/dist/gmltools-0.0.48.tar.gz
--rw-rw-rw-   0        0        0   291024 2023-04-13 10:48:46.000000 gmltools-0.0.57/dist/gmltools-0.0.49.tar.gz
--rw-rw-rw-   0        0        0   291054 2023-04-13 11:27:27.000000 gmltools-0.0.57/dist/gmltools-0.0.50.tar.gz
--rw-rw-rw-   0        0        0   291079 2023-04-13 11:38:27.000000 gmltools-0.0.57/dist/gmltools-0.0.51.tar.gz
--rw-rw-rw-   0        0        0   291069 2023-04-13 11:45:59.000000 gmltools-0.0.57/dist/gmltools-0.0.52.tar.gz
--rw-rw-rw-   0        0        0   291231 2023-04-14 07:56:54.000000 gmltools-0.0.57/dist/gmltools-0.0.53.tar.gz
--rw-rw-rw-   0        0        0   291232 2023-04-14 08:02:57.000000 gmltools-0.0.57/dist/gmltools-0.0.54.tar.gz
--rw-rw-rw-   0        0        0   291334 2023-04-14 08:49:47.000000 gmltools-0.0.57/dist/gmltools-0.0.55.tar.gz
--rw-rw-rw-   0        0        0   292622 2023-04-14 09:40:06.000000 gmltools-0.0.57/dist/gmltools-0.0.56.tar.gz
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.57/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.57/mltools.yml
--rw-rw-rw-   0        0        0      546 2023-04-14 10:09:26.000000 gmltools-0.0.57/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 10:10:15.177117 gmltools-0.0.57/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-14 10:09:18.000000 gmltools-0.0.57/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:10:14.987388 gmltools-0.0.57/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.055361 gmltools-0.0.57/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.57/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.57/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.092792 gmltools-0.0.57/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.57/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.57/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.152515 gmltools-0.0.57/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.57/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.57/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.57/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5137 2023-04-14 09:39:40.000000 gmltools-0.0.57/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   119050 2023-04-14 10:09:03.000000 gmltools-0.0.57/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.57/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    12588 2023-04-14 09:47:45.000000 gmltools-0.0.57/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.162087 gmltools-0.0.57/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.57/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.57/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.57/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.173056 gmltools-0.0.57/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.57/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.57/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.57/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.57/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:10:15.087843 gmltools-0.0.57/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-04-14 10:10:14.000000 gmltools-0.0.57/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-04-14 10:10:14.000000 gmltools-0.0.57/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 10:10:14.000000 gmltools-0.0.57/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-14 10:10:14.000000 gmltools-0.0.57/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 10:10:14.000000 gmltools-0.0.57/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 10:29:49.677371 gmltools-0.0.58/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.58/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.58/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-04-14 10:29:49.675376 gmltools-0.0.58/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.58/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 10:29:49.492425 gmltools-0.0.58/dist/
+-rw-rw-rw-   0        0        0    53691 2023-03-17 10:43:07.000000 gmltools-0.0.58/dist/gmltools-0.0.24.tar.gz
+-rw-rw-rw-   0        0        0    53713 2023-03-17 10:56:22.000000 gmltools-0.0.58/dist/gmltools-0.0.25.tar.gz
+-rw-rw-rw-   0        0        0    53711 2023-03-17 11:19:35.000000 gmltools-0.0.58/dist/gmltools-0.0.26.tar.gz
+-rw-rw-rw-   0        0        0    53727 2023-03-17 11:25:08.000000 gmltools-0.0.58/dist/gmltools-0.0.27.tar.gz
+-rw-rw-rw-   0        0        0    53751 2023-03-21 09:33:58.000000 gmltools-0.0.58/dist/gmltools-0.0.28.tar.gz
+-rw-rw-rw-   0        0        0    53762 2023-03-21 09:53:00.000000 gmltools-0.0.58/dist/gmltools-0.0.29.tar.gz
+-rw-rw-rw-   0        0        0    56221 2023-03-22 10:45:28.000000 gmltools-0.0.58/dist/gmltools-0.0.30.tar.gz
+-rw-rw-rw-   0        0        0    56607 2023-03-22 12:13:29.000000 gmltools-0.0.58/dist/gmltools-0.0.31.tar.gz
+-rw-rw-rw-   0        0        0    56619 2023-03-22 12:20:22.000000 gmltools-0.0.58/dist/gmltools-0.0.32.tar.gz
+-rw-rw-rw-   0        0        0    56655 2023-03-22 12:28:41.000000 gmltools-0.0.58/dist/gmltools-0.0.33.tar.gz
+-rw-rw-rw-   0        0        0    56667 2023-03-22 12:31:59.000000 gmltools-0.0.58/dist/gmltools-0.0.34.tar.gz
+-rw-rw-rw-   0        0        0    56681 2023-03-22 12:46:07.000000 gmltools-0.0.58/dist/gmltools-0.0.35.tar.gz
+-rw-rw-rw-   0        0        0    56537 2023-03-23 10:43:13.000000 gmltools-0.0.58/dist/gmltools-0.0.36.tar.gz
+-rw-rw-rw-   0        0        0    56554 2023-03-23 10:47:16.000000 gmltools-0.0.58/dist/gmltools-0.0.37.tar.gz
+-rw-rw-rw-   0        0        0   284440 2023-03-30 08:43:02.000000 gmltools-0.0.58/dist/gmltools-0.0.38.tar.gz
+-rw-rw-rw-   0        0        0   284496 2023-03-30 10:53:02.000000 gmltools-0.0.58/dist/gmltools-0.0.39.tar.gz
+-rw-rw-rw-   0        0        0   284866 2023-04-04 08:49:39.000000 gmltools-0.0.58/dist/gmltools-0.0.40.tar.gz
+-rw-rw-rw-   0        0        0   286391 2023-04-11 09:53:19.000000 gmltools-0.0.58/dist/gmltools-0.0.41.tar.gz
+-rw-rw-rw-   0        0        0   289831 2023-04-12 10:45:06.000000 gmltools-0.0.58/dist/gmltools-0.0.42.tar.gz
+-rw-rw-rw-   0        0        0   289829 2023-04-12 10:52:27.000000 gmltools-0.0.58/dist/gmltools-0.0.43.tar.gz
+-rw-rw-rw-   0        0        0   289837 2023-04-12 10:56:44.000000 gmltools-0.0.58/dist/gmltools-0.0.44.tar.gz
+-rw-rw-rw-   0        0        0   289819 2023-04-12 11:03:49.000000 gmltools-0.0.58/dist/gmltools-0.0.45.tar.gz
+-rw-rw-rw-   0        0        0   289827 2023-04-12 11:09:04.000000 gmltools-0.0.58/dist/gmltools-0.0.46.tar.gz
+-rw-rw-rw-   0        0        0   289863 2023-04-12 11:18:58.000000 gmltools-0.0.58/dist/gmltools-0.0.47.tar.gz
+-rw-rw-rw-   0        0        0   291078 2023-04-13 10:45:14.000000 gmltools-0.0.58/dist/gmltools-0.0.48.tar.gz
+-rw-rw-rw-   0        0        0   291024 2023-04-13 10:48:46.000000 gmltools-0.0.58/dist/gmltools-0.0.49.tar.gz
+-rw-rw-rw-   0        0        0   291054 2023-04-13 11:27:27.000000 gmltools-0.0.58/dist/gmltools-0.0.50.tar.gz
+-rw-rw-rw-   0        0        0   291079 2023-04-13 11:38:27.000000 gmltools-0.0.58/dist/gmltools-0.0.51.tar.gz
+-rw-rw-rw-   0        0        0   291069 2023-04-13 11:45:59.000000 gmltools-0.0.58/dist/gmltools-0.0.52.tar.gz
+-rw-rw-rw-   0        0        0   291231 2023-04-14 07:56:54.000000 gmltools-0.0.58/dist/gmltools-0.0.53.tar.gz
+-rw-rw-rw-   0        0        0   291232 2023-04-14 08:02:57.000000 gmltools-0.0.58/dist/gmltools-0.0.54.tar.gz
+-rw-rw-rw-   0        0        0   291334 2023-04-14 08:49:47.000000 gmltools-0.0.58/dist/gmltools-0.0.55.tar.gz
+-rw-rw-rw-   0        0        0   292622 2023-04-14 09:40:06.000000 gmltools-0.0.58/dist/gmltools-0.0.56.tar.gz
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.58/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.58/mltools.yml
+-rw-rw-rw-   0        0        0      546 2023-04-14 10:29:16.000000 gmltools-0.0.58/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 10:29:49.677371 gmltools-0.0.58/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-14 10:29:36.000000 gmltools-0.0.58/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:29:49.141635 gmltools-0.0.58/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 10:29:49.497362 gmltools-0.0.58/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.58/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.58/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:29:49.538574 gmltools-0.0.58/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.58/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    34949 2023-03-23 10:46:34.000000 gmltools-0.0.58/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:29:49.606145 gmltools-0.0.58/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.58/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.58/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.58/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5137 2023-04-14 09:39:40.000000 gmltools-0.0.58/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   119078 2023-04-14 10:28:24.000000 gmltools-0.0.58/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     5803 2023-03-07 12:45:49.000000 gmltools-0.0.58/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    12588 2023-04-14 09:47:45.000000 gmltools-0.0.58/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:29:49.631151 gmltools-0.0.58/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.58/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73694 2023-04-12 11:41:49.000000 gmltools-0.0.58/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5654 2023-03-13 10:21:45.000000 gmltools-0.0.58/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:29:49.673384 gmltools-0.0.58/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.58/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.58/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.58/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.58/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:29:49.527594 gmltools-0.0.58/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-04-14 10:29:48.000000 gmltools-0.0.58/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-04-14 10:29:49.000000 gmltools-0.0.58/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 10:29:48.000000 gmltools-0.0.58/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-14 10:29:48.000000 gmltools-0.0.58/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 10:29:48.000000 gmltools-0.0.58/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.57/LICENSE` & `gmltools-0.0.58/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/Models.ipynb` & `gmltools-0.0.58/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/PKG-INFO` & `gmltools-0.0.58/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.57
+Version: 0.0.58
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.57/README.md` & `gmltools-0.0.58/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.24.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.24.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.25.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.25.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.26.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.26.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.27.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.27.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.28.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.28.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.29.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.29.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.30.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.30.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.31.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.31.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.32.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.32.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.33.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.33.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.34.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.34.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.35.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.35.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.36.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.36.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.37.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.37.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.38.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.38.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.39.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.39.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.40.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.40.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.41.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.41.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.42.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.42.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.43.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.43.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.44.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.44.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.45.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.45.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.46.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.46.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.47.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.47.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.48.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.48.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.49.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.49.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.50.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.50.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.51.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.51.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.52.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.52.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.53.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.53.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.54.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.54.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.55.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.55.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/dist/gmltools-0.0.56.tar.gz` & `gmltools-0.0.58/dist/gmltools-0.0.56.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/gmltools.yml` & `gmltools-0.0.58/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/mltools.yml` & `gmltools-0.0.58/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/pyproject.toml` & `gmltools-0.0.58/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.57"
+version = "0.0.58"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.57/setup.py` & `gmltools-0.0.58/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.57',
+    'version': '0.0.58',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.57/src/gmltools/To_Do.txt` & `gmltools-0.0.58/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/eda/eda.py` & `gmltools-0.0.58/src/gmltools/eda/eda.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/models/bayes.py` & `gmltools-0.0.58/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.58/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/models/dummy_model.py` & `gmltools-0.0.58/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/models/model.py` & `gmltools-0.0.58/src/gmltools/models/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1801,15 +1801,15 @@
         #save cv results if exists grid search or random search
         if hasattr(self.model, 'cv_results_'):
             df = pd.DataFrame(self.model.cv_results_)
             df.sort_values('rank_test_score', inplace=True)
             if hasattr(self.cv, 'is_timeseriesinitialsplit'):
                 #rename the split columns
                 new_column_names = self.cv.get_test_days(self.X_train)
-                df.rename(columns=dict(zip(df.filter(regex='split').columns, new_column_names)), inplace=True)
+                df.rename(columns=dict(zip(df.filter(regex='split').filter(regex='_test_score').columns, new_column_names)), inplace=True)
             df.to_excel(os.path.join(path, self.model_name+'_cv_results.xlsx'), index=False)
 
             #save the best register of the cv_results in a second sheet of excel file called summary_models.xlsx
             df_best = pd.DataFrame(df.iloc[0]).T
             df_best["Search conditions"]=str(self._overall_dict_params)
             df_best['model_name'] = self.model_name
             #set model_name the firts column and Search conditions the second column
```

### Comparing `gmltools-0.0.57/src/gmltools/models/models_info.py` & `gmltools-0.0.58/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.58/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.58/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.58/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.58/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.58/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.58/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.57/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.58/src/gmltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.57
+Version: 0.0.58
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.57/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.58/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

