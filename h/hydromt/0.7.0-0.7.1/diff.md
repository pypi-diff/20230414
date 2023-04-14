# Comparing `tmp/hydromt-0.7.0.tar.gz` & `tmp/hydromt-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromt-0.7.0.tar", last modified: Wed Feb 22 04:58:01 2023, max compression
+gzip compressed data, was "hydromt-0.7.1.tar", last modified: Fri Apr 14 06:43:26 2023, max compression
```

## Comparing `hydromt-0.7.0.tar` & `hydromt-0.7.1.tar`

### file list

```diff
@@ -1,51 +1,54 @@
--rw-r--r--   0        0        0     1419 2023-02-22 04:57:50.869289 hydromt-0.7.0/.gitignore
--rw-r--r--   0        0        0     1231 2023-02-22 04:57:50.869289 hydromt-0.7.0/.zenodo.json
--rw-r--r--   0        0        0     1075 2023-02-22 04:57:50.869289 hydromt-0.7.0/LICENSE
--rw-r--r--   0        0        0     5546 2023-02-22 04:57:50.869289 hydromt-0.7.0/README.rst
--rw-r--r--   0        0        0     2679 2023-02-22 04:57:50.869289 hydromt-0.7.0/data/catalogs/README.rst
--rw-r--r--   0        0        0      449 2023-02-22 04:57:50.869289 hydromt-0.7.0/data/catalogs/aws_data.yml
--rw-r--r--   0        0        0     1543 2023-02-22 04:57:50.869289 hydromt-0.7.0/data/catalogs/changelog.rst
--rw-r--r--   0        0        0    48760 2023-02-22 04:57:50.869289 hydromt-0.7.0/data/catalogs/deltares_data.yml
--rw-r--r--   0        0        0    11367 2023-02-22 04:57:50.869289 hydromt-0.7.0/data/catalogs/gcs_cmip6_data.yml
--rw-r--r--   0        0        0     1464 2023-02-22 04:57:50.869289 hydromt-0.7.0/data/predefined_catalogs.yml
--rw-r--r--   0        0        0     4272 2023-02-22 04:57:50.869289 hydromt-0.7.0/data/src/chirps_download_convert.py
--rw-r--r--   0        0        0    23908 2023-02-22 04:57:50.869289 hydromt-0.7.0/data/src/era5_download_resample_convert.py
--rw-r--r--   0        0        0      243 2023-02-22 04:57:50.885289 hydromt-0.7.0/environment.yml
--rw-r--r--   0        0        0      526 2023-02-22 04:57:50.889289 hydromt-0.7.0/hydromt/__init__.py
--rw-r--r--   0        0        0      931 2023-02-22 04:57:50.889289 hydromt-0.7.0/hydromt/_compat.py
--rw-r--r--   0        0        0       71 2023-02-22 04:57:50.889289 hydromt-0.7.0/hydromt/cli/__init__.py
--rw-r--r--   0        0        0     6142 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/cli/api.py
--rw-r--r--   0        0        0     3085 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/cli/cli_utils.py
--rw-r--r--   0        0        0    10754 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/cli/main.py
--rw-r--r--   0        0        0     5465 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/config.py
--rw-r--r--   0        0        0      188 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/data_adapter/__init__.py
--rw-r--r--   0        0        0     3562 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/data_adapter/caching.py
--rw-r--r--   0        0        0    12724 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/data_adapter/data_adapter.py
--rw-r--r--   0        0        0     8108 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/data_adapter/dataframe.py
--rw-r--r--   0        0        0    10099 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/data_adapter/geodataframe.py
--rw-r--r--   0        0        0    13373 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/data_adapter/geodataset.py
--rw-r--r--   0        0        0    16409 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/data_adapter/rasterdataset.py
--rw-r--r--   0        0        0    35267 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/data_catalog.py
--rw-r--r--   0        0        0      290 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/error.py
--rw-r--r--   0        0        0    28915 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/flw.py
--rw-r--r--   0        0        0    21224 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/gis_utils.py
--rw-r--r--   0        0        0    21768 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/io.py
--rw-r--r--   0        0        0     2815 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/log.py
--rw-r--r--   0        0        0     8262 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/merge.py
--rw-r--r--   0        0        0      548 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/models/__init__.py
--rw-r--r--   0        0        0    58271 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/models/model_api.py
--rw-r--r--   0        0        0     6919 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/models/model_grid.py
--rw-r--r--   0        0        0     7814 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/models/model_lumped.py
--rw-r--r--   0        0        0    19085 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/models/model_mesh.py
--rw-r--r--   0        0        0     2454 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/models/model_network.py
--rw-r--r--   0        0        0     4744 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/models/model_plugins.py
--rw-r--r--   0        0        0    94702 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/raster.py
--rw-r--r--   0        0        0       72 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/stats/__init__.py
--rw-r--r--   0        0        0    13667 2023-02-22 04:57:50.893289 hydromt-0.7.0/hydromt/stats/skills.py
--rw-r--r--   0        0        0    32517 2023-02-22 04:57:50.897289 hydromt-0.7.0/hydromt/vector.py
--rw-r--r--   0        0        0      120 2023-02-22 04:57:50.897289 hydromt-0.7.0/hydromt/workflows/__init__.py
--rw-r--r--   0        0        0    18478 2023-02-22 04:57:50.897289 hydromt-0.7.0/hydromt/workflows/basin_mask.py
--rw-r--r--   0        0        0    26008 2023-02-22 04:57:50.897289 hydromt-0.7.0/hydromt/workflows/forcing.py
--rw-r--r--   0        0        0     6568 2023-02-22 04:57:50.897289 hydromt-0.7.0/hydromt/workflows/rivers.py
--rw-r--r--   0        0        0     2305 2023-02-22 04:57:50.897289 hydromt-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7516 1970-01-01 00:00:00.000000 hydromt-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1419 2023-04-14 06:43:16.410205 hydromt-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1833 2023-04-14 06:43:16.410205 hydromt-0.7.1/.zenodo.json
+-rw-r--r--   0        0        0     1075 2023-04-14 06:43:16.410205 hydromt-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5933 2023-04-14 06:43:16.410205 hydromt-0.7.1/README.rst
+-rw-r--r--   0        0        0     2679 2023-04-14 06:43:16.410205 hydromt-0.7.1/data/catalogs/README.rst
+-rw-r--r--   0        0        0      449 2023-04-14 06:43:16.410205 hydromt-0.7.1/data/catalogs/aws_data.yml
+-rw-r--r--   0        0        0     1543 2023-04-14 06:43:16.410205 hydromt-0.7.1/data/catalogs/changelog.rst
+-rw-r--r--   0        0        0    48760 2023-04-14 06:43:16.410205 hydromt-0.7.1/data/catalogs/deltares_data.yml
+-rw-r--r--   0        0        0    11367 2023-04-14 06:43:16.414205 hydromt-0.7.1/data/catalogs/gcs_cmip6_data.yml
+-rw-r--r--   0        0        0     1464 2023-04-14 06:43:16.414205 hydromt-0.7.1/data/predefined_catalogs.yml
+-rw-r--r--   0        0        0     4272 2023-04-14 06:43:16.414205 hydromt-0.7.1/data/src/chirps_download_convert.py
+-rw-r--r--   0        0        0    23908 2023-04-14 06:43:16.414205 hydromt-0.7.1/data/src/era5_download_resample_convert.py
+-rw-r--r--   0        0        0      243 2023-04-14 06:43:16.426206 hydromt-0.7.1/environment.yml
+-rw-r--r--   0        0        0      526 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/__init__.py
+-rw-r--r--   0        0        0      931 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/_compat.py
+-rw-r--r--   0        0        0       71 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/cli/__init__.py
+-rw-r--r--   0        0        0     6142 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/cli/api.py
+-rw-r--r--   0        0        0     3300 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/cli/cli_utils.py
+-rw-r--r--   0        0        0    10754 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/cli/main.py
+-rw-r--r--   0        0        0     8266 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/config.py
+-rw-r--r--   0        0        0      188 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/data_adapter/__init__.py
+-rw-r--r--   0        0        0     3562 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/data_adapter/caching.py
+-rw-r--r--   0        0        0    12724 2023-04-14 06:43:16.430206 hydromt-0.7.1/hydromt/data_adapter/data_adapter.py
+-rw-r--r--   0        0        0     8108 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/data_adapter/dataframe.py
+-rw-r--r--   0        0        0    10099 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/data_adapter/geodataframe.py
+-rw-r--r--   0        0        0    14008 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/data_adapter/geodataset.py
+-rw-r--r--   0        0        0    16847 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/data_adapter/rasterdataset.py
+-rw-r--r--   0        0        0    38472 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/data_catalog.py
+-rw-r--r--   0        0        0      290 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/error.py
+-rw-r--r--   0        0        0    28915 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/flw.py
+-rw-r--r--   0        0        0    21224 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/gis_utils.py
+-rw-r--r--   0        0        0    21768 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/io.py
+-rw-r--r--   0        0        0     2815 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/log.py
+-rw-r--r--   0        0        0     8262 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/merge.py
+-rw-r--r--   0        0        0      548 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/__init__.py
+-rw-r--r--   0        0        0    58390 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_api.py
+-rw-r--r--   0        0        0     7123 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_grid.py
+-rw-r--r--   0        0        0     7814 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_lumped.py
+-rw-r--r--   0        0        0    19085 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_mesh.py
+-rw-r--r--   0        0        0     2454 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_network.py
+-rw-r--r--   0        0        0     4744 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/models/model_plugins.py
+-rw-r--r--   0        0        0    94702 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/raster.py
+-rw-r--r--   0        0        0       72 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/stats/__init__.py
+-rw-r--r--   0        0        0    13667 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/stats/skills.py
+-rw-r--r--   0        0        0    32517 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/vector.py
+-rw-r--r--   0        0        0      120 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/workflows/__init__.py
+-rw-r--r--   0        0        0    18494 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/workflows/basin_mask.py
+-rw-r--r--   0        0        0    26008 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/workflows/forcing.py
+-rw-r--r--   0        0        0     6568 2023-04-14 06:43:16.434206 hydromt-0.7.1/hydromt/workflows/rivers.py
+-rw-r--r--   0        0        0      592 2023-04-14 06:43:16.434206 hydromt-0.7.1/joss_paper/citation.bib
+-rw-r--r--   0        0        0    15298 2023-04-14 06:43:16.438206 hydromt-0.7.1/joss_paper/paper.bib
+-rw-r--r--   0        0        0    12874 2023-04-14 06:43:16.438206 hydromt-0.7.1/joss_paper/paper.md
+-rw-r--r--   0        0        0     2319 2023-04-14 06:43:16.438206 hydromt-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7916 1970-01-01 00:00:00.000000 hydromt-0.7.1/PKG-INFO
```

### Comparing `hydromt-0.7.0/.gitignore` & `hydromt-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/.zenodo.json` & `hydromt-0.7.1/.zenodo.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8150252525252526%*

 * *Differences: {"'creators'": "{2: {'name': 'Bouaziz, Laurène J. E.'}, 7: {'name': 'de Jong, Tjalling'}, insert: "*

 * *               "[(6, OrderedDict([('affiliation', 'Deltares'), ('name', 'Hegnauer, Mark')])), (10, "*

 * *               "OrderedDict([('affiliation', 'Deltares'), ('name', 'van Verseveld, Willem'), "*

 * *               "('orcid', '0000-0003-3311-738X')]))]}",*

 * * "'description'": "'HydroMT (Hydro Model Tools) is an open-source Python package that facilitates "*

 * *                  'the process of building and analyzing spa […]*

```diff
@@ -8,15 +8,15 @@
         },
         {
             "affiliation": "Deltares",
             "name": "Boisgontier, H\u00e9l\u00e8ne"
         },
         {
             "affiliation": "Deltares",
-            "name": "Bouaziz, Laurene J. E.",
+            "name": "Bouaziz, Laur\u00e8ne J. E.",
             "orcid": "0000-0003-0597-8051"
         },
         {
             "affiliation": "Deltares",
             "name": "Buitink, Joost"
         },
         {
@@ -26,23 +26,32 @@
         },
         {
             "affiliation": "Deltares",
             "name": "Dalmijn, Brendan"
         },
         {
             "affiliation": "Deltares",
-            "name": "De Jong, Tjalling"
+            "name": "Hegnauer, Mark"
+        },
+        {
+            "affiliation": "Deltares",
+            "name": "de Jong, Tjalling"
         },
         {
             "affiliation": "Deltares",
             "name": "Loos, Sibren"
         },
         {
             "affiliation": "Deltares",
             "name": "Marth, Indra"
+        },
+        {
+            "affiliation": "Deltares",
+            "name": "van Verseveld, Willem",
+            "orcid": "0000-0003-3311-738X"
         }
     ],
-    "description": "Automated and reproducible model building and analysis",
+    "description": "HydroMT (Hydro Model Tools) is an open-source Python package that facilitates the process of building and analyzing spatial geoscientific models with a focus on water system models. It does so by automating the workflow to go from raw data to a complete model instance which is ready to run and to analyse model results once the simulation has finished.",
     "license": "MIT",
-    "title": "HydroMT",
+    "title": "HydroMT: Automated and reproducible model building and analysis",
     "upload_type": "software"
 }
```

### Comparing `hydromt-0.7.0/LICENSE` & `hydromt-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/README.rst` & `hydromt-0.7.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. _readme:
 
 ===============================================================
 HydroMT: Automated and reproducible model building and analysis
 ===============================================================
 
-|pypi| |conda forge| |docs_latest| |docs_stable| |codecov| |license| |doi| |binder|
+|pypi| |conda forge| |docs_latest| |docs_stable| |binder| |codecov| |license| |doi| |joss_paper|
 
 
 What is HydroMT?
 ----------------
 **HydroMT** (Hydro Model Tools) is an open-source Python package that facilitates the process of 
 building and analyzing spatial geoscientific models with a focus on water system models. 
 It does so by automating the workflow to go from raw data to a complete model instance which 
@@ -49,15 +49,20 @@
 * hydromt_delwaq_: A framework for water quality (D-Water Quality) and emissions (D-Emissions) modelling.
 * hydromt_sfincs_: A fast 2D hydrodynamic flood model (SFINCS).
 * hydromt_fiat_: A flood impact model (FIAT).
 
 
 How to cite?
 ------------
-For publications, please cite our work using the DOI provided in the Zenodo badge |doi| that points to the latest release.
+For publications, please cite our JOSS paper |joss_paper|
+
+::
+    Eilander et al., (2023). HydroMT: Automated and reproducible model building and analysis. Journal of Open Source Software, 8(83), 4897, https://doi.org/10.21105/joss.04897
+
+To cite a specific software version please use the DOI provided in the Zenodo badge |doi| that points to the latest release.
 
 
 How to contribute?
 -------------------
 If you find any issues in the code or documentation feel free to leave an issue on the `github issue tracker. <https://github.com/Deltares/hydromt/issues>`_
 You can find information about how to contribute to the HydroMT project at our `contributing page. <https://deltares.github.io/hydromt/latest/dev/contributing>`_
 
@@ -105,7 +110,10 @@
 .. |doi| image:: https://zenodo.org/badge/348020332.svg
     :alt: Zenodo
     :target: https://zenodo.org/badge/latestdoi/348020332
 
 .. |license| image:: https://img.shields.io/github/license/Deltares/hydromt?style=flat
     :alt: License
     :target: https://github.com/Deltares/hydromt/blob/main/LICENSE
+
+.. |joss_paper| image:: https://joss.theoj.org/papers/10.21105/joss.04897/status.svg
+   :target: https://doi.org/10.21105/joss.04897
```

### Comparing `hydromt-0.7.0/data/catalogs/README.rst` & `hydromt-0.7.1/data/catalogs/README.rst`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/data/catalogs/changelog.rst` & `hydromt-0.7.1/data/catalogs/changelog.rst`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/data/catalogs/deltares_data.yml` & `hydromt-0.7.1/data/catalogs/deltares_data.yml`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/data/catalogs/gcs_cmip6_data.yml` & `hydromt-0.7.1/data/catalogs/gcs_cmip6_data.yml`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/data/predefined_catalogs.yml` & `hydromt-0.7.1/data/predefined_catalogs.yml`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/data/src/chirps_download_convert.py` & `hydromt-0.7.1/data/src/chirps_download_convert.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/data/src/era5_download_resample_convert.py` & `hydromt-0.7.1/data/src/era5_download_resample_convert.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/__init__.py` & `hydromt-0.7.1/hydromt/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """HydroMT: Automated and reproducible model building and analysis"""
 
 # version number without 'v' at start
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 # Set environment variables (this will be temporary)
 # to use shapely 2.0 in favor of pygeos (if installed)
 import os
 
 os.environ["USE_PYGEOS"] = "0"
```

### Comparing `hydromt-0.7.0/hydromt/_compat.py` & `hydromt-0.7.1/hydromt/_compat.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/cli/api.py` & `hydromt-0.7.1/hydromt/cli/api.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/cli/cli_utils.py` & `hydromt-0.7.1/hydromt/cli/cli_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from os.path import isfile
 import json
 import logging
 import click
 from ast import literal_eval
 from typing import Union, Dict
 from pathlib import Path
+from warnings import warn
 
 from .. import config
 from ..error import DeprecatedError
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["parse_json", "parse_config", "parse_opt"]
@@ -78,14 +79,19 @@
 ### general parsing methods ##
 
 
 def parse_config(path: Union[Path, str] = None, opt_cli: Dict = None) -> Dict:
     """Parse config from ini `path` and combine with command line options `opt_cli`"""
     opt = {}
     if path is not None and isfile(path):
+        if str(path).endswith(".ini"):
+            warn(
+                "Support for .ini configuration files will be deprecated",
+                PendingDeprecationWarning,
+            )
         opt = config.configread(
             path, abs_path=True, skip_abspath_sections=["setup_config"]
         )
     elif path is not None:
         raise IOError(f"Config not found at {path}")
     if opt_cli is not None:
         for section in opt_cli:
```

### Comparing `hydromt-0.7.0/hydromt/cli/main.py` & `hydromt-0.7.1/hydromt/cli/main.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/data_adapter/caching.py` & `hydromt-0.7.1/hydromt/data_adapter/caching.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/data_adapter/data_adapter.py` & `hydromt-0.7.1/hydromt/data_adapter/data_adapter.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/data_adapter/dataframe.py` & `hydromt-0.7.1/hydromt/data_adapter/dataframe.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/data_adapter/geodataframe.py` & `hydromt-0.7.1/hydromt/data_adapter/geodataframe.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/data_adapter/geodataset.py` & `hydromt-0.7.1/hydromt/data_adapter/geodataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,28 +128,42 @@
         -------
         fn_out: str
             Absolute path to output file
         driver: str
             Name of driver to read data with, see :py:func:`~hydromt.data_catalog.DataCatalog.get_geodataset`
         """
         obj = self.get_data(
-            bbox=bbox, time_tuple=time_tuple, variables=variables, logger=logger
+            bbox=bbox,
+            time_tuple=time_tuple,
+            variables=variables,
+            logger=logger,
+            single_var_as_array=variables is None,
         )
         if obj.vector.index.size == 0 or ("time" in obj.coords and obj.time.size == 0):
             return None, None
 
         if driver is None or driver == "netcdf":
             # always write netcdf
             driver = "netcdf"
-            fn_out = join(data_root, f"{data_name}.nc")
             dvars = [obj.name] if isinstance(obj, xr.DataArray) else obj.vector.vars
-            encoding = {k: {"zlib": True} for k in dvars}
-            obj.to_netcdf(fn_out, encoding=encoding)
+            if variables is None:
+                encoding = {k: {"zlib": True} for k in dvars}
+                fn_out = join(data_root, f"{data_name}.nc")
+                obj.to_netcdf(fn_out, encoding=encoding)
+            else:  # save per variable
+                if not os.path.isdir(join(data_root, data_name)):
+                    os.makedirs(join(data_root, data_name))
+                for var in dvars:
+                    fn_out = join(data_root, data_name, f"{var}.nc")
+                    obj[var].to_netcdf(fn_out, encoding={var: {"zlib": True}})
+                fn_out = join(data_root, data_name, "{variable}.nc")
         elif driver == "zarr":
             fn_out = join(data_root, f"{data_name}.zarr")
+            if isinstance(obj, xr.DataArray):
+                obj = obj.to_dataset()
             obj.to_zarr(fn_out, **kwargs)
         else:
             raise ValueError(f"GeoDataset: Driver {driver} unknown.")
 
         return fn_out, driver
 
     def get_data(
```

### Comparing `hydromt-0.7.0/hydromt/data_adapter/rasterdataset.py` & `hydromt-0.7.1/hydromt/data_adapter/rasterdataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,32 +135,41 @@
             Absolute path to output file
         driver: str
             Name of driver to read data with, see :py:func:`~hydromt.data_catalog.DataCatalog.get_rasterdataset`
         """
 
         try:
             obj = self.get_data(
-                bbox=bbox, time_tuple=time_tuple, variables=variables, logger=logger
+                bbox=bbox,
+                time_tuple=time_tuple,
+                variables=variables,
+                logger=logger,
+                single_var_as_array=variables is None,
             )
         except IndexError as err:  # out of bounds
             logger.warning(str(err))
             return None, None
 
         if driver is None:
-            driver = self.driver
-            if driver in ["raster_tindex", "raster"]:
-                # by default write 2D raster data to GeoTiff and 3D raster data to netcdf
-                driver = "netcdf" if len(obj.dims) == 3 else "GTiff"
+            # by default write 2D raster data to GeoTiff and 3D raster data to netcdf
+            driver = "netcdf" if len(obj.dims) == 3 else "GTiff"
         # write using various writers
         if driver in ["netcdf"]:  # TODO complete list
-            fn_out = join(data_root, f"{data_name}.nc")
-            if "encoding" not in kwargs:
-                dvars = [obj.name] if isinstance(obj, xr.DataArray) else obj.raster.vars
-                kwargs.update(encoding={k: {"zlib": True} for k in dvars})
-            obj.to_netcdf(fn_out, **kwargs)
+            dvars = [obj.name] if isinstance(obj, xr.DataArray) else obj.raster.vars
+            if variables is None:
+                encoding = {k: {"zlib": True} for k in dvars}
+                fn_out = join(data_root, f"{data_name}.nc")
+                obj.to_netcdf(fn_out, encoding=encoding, **kwargs)
+            else:  # save per variable
+                if not os.path.isdir(join(data_root, data_name)):
+                    os.makedirs(join(data_root, data_name))
+                for var in dvars:
+                    fn_out = join(data_root, data_name, f"{var}.nc")
+                    obj[var].to_netcdf(fn_out, encoding={var: {"zlib": True}}, **kwargs)
+                fn_out = join(data_root, data_name, "{variable}.nc")
         elif driver == "zarr":
             fn_out = join(data_root, f"{data_name}.zarr")
             obj.to_zarr(fn_out, **kwargs)
         elif driver not in gis_utils.GDAL_DRIVER_CODE_MAP.values():
             raise ValueError(f"RasterDataset: Driver {driver} unknown.")
         else:
             ext = gis_utils.GDAL_EXT_CODE_MAP.get(driver)
```

### Comparing `hydromt-0.7.0/hydromt/data_catalog.py` & `hydromt-0.7.1/hydromt/data_catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -464,56 +464,79 @@
         self,
         data_root: Union[Path, str],
         bbox: List = None,
         time_tuple: Tuple = None,
         source_names: List = [],
         unit_conversion: bool = True,
         meta: Dict = {},
+        append: bool = False,
     ) -> None:
         """Export a data slice of each dataset and a data_catalog.yml file to disk.
 
         Parameters
         ----------
         data_root : str, Path
             Path to output folder
         bbox : array-like of floats
             (xmin, ymin, xmax, ymax) bounding box of area of interest.
         time_tuple : tuple of str, datetime, optional
             Start and end date of period of interest. By default the entire time period
             of the dataset is returned.
         source_names: list, optional
-            List of source names to export
+            List of source names to export, by default None in which case all sources are exported.
+            Specific variables can be selected by appending them to the source name in square brackets.
+            For example, to export all variables of 'source_name1' and only 'var1' and 'var2' of 'source_name'
+            use source_names=['source_name1', 'source_name2[var1,var2]']
         unit_conversion: boolean, optional
             If False skip unit conversion when parsing data from file, by default True.
         meta: dict, optional
             key-value pairs to add to the data catalog meta section, such as 'version', by default empty.
+        append: bool, optional
+            If True, append to existing data catalog, by default False.
         """
         data_root = abspath(data_root)
         if not os.path.isdir(data_root):
             os.makedirs(data_root)
 
         # create copy of data with selected source names
-        sources = copy.deepcopy(self.sources)
+        source_vars = {}
         if len(source_names) > 0:
-            sources = {n: sources[n] for n in source_names}
+            sources = {}
+            for name in source_names:
+                # deduce variables from name
+                if "[" in name:
+                    variables = name.split("[")[-1].split("]")[0].split(",")
+                    name = name.split("[")[0]
+                    source_vars[name] = variables
+                sources[name] = copy.deepcopy(self.sources[name])
+        else:
+            sources = copy.deepcopy(self.sources)
+
+        # read existing data catalog if it exists
+        fn = join(data_root, "data_catalog.yml")
+        if isfile(fn) and append:
+            self.logger.info(f"Appending existing data catalog {fn}")
+            sources_out = DataCatalog(fn).sources
+        else:
+            sources_out = {}
 
         # export data and update sources
-        sources_out = {}
         for key, source in sources.items():
             try:
                 # read slice of source and write to file
                 self.logger.debug(f"Exporting {key}.")
                 if not unit_conversion:
                     unit_mult = source.unit_mult
                     unit_add = source.unit_add
                     source.unit_mult = {}
                     source.unit_add = {}
                 fn_out, driver = source.to_file(
                     data_root=data_root,
                     data_name=key,
+                    variables=source_vars.get(key, None),
                     bbox=bbox,
                     time_tuple=time_tuple,
                     logger=self.logger,
                 )
                 if fn_out is None:
                     self.logger.warning(f"{key} file contains no data within domain")
                     continue
@@ -525,52 +548,55 @@
                     source.unit_mult = unit_mult
                     source.unit_add = unit_add
                 source.path = fn_out
                 source.driver = driver
                 source.filesystem = "local"
                 source.kwargs = {}
                 source.rename = {}
+                if key in sources_out:
+                    self.logger.warning(
+                        f"{key} already exists in data catalog and is overwritten."
+                    )
                 sources_out[key] = source
             except FileNotFoundError:
                 self.logger.warning(f"{key} file not found at {source.path}")
 
         # write data catalog to yml
         data_catalog_out = DataCatalog()
         data_catalog_out._sources = sources_out
-        fn = join(data_root, "data_catalog.yml")
         data_catalog_out.to_yml(fn, root="auto", meta=meta)
 
     def get_rasterdataset(
         self,
-        path_or_key: str,
+        data_like: Union[str, Path, xr.Dataset, xr.DataArray],
         bbox: List = None,
         geom: gpd.GeoDataFrame = None,
         zoom_level: int | tuple = None,
         buffer: Union[float, int] = 0,
         align: bool = None,
         variables: Union[List, str] = None,
         time_tuple: Tuple = None,
         single_var_as_array: bool = True,
         **kwargs,
     ) -> xr.Dataset:
-        """Returns a clipped, sliced and unified RasterDataset from the data catalog.
+        """Returns a clipped, sliced and unified RasterDataset.
 
         To clip the data to the area of interest, provide a `bbox` or `geom`,
         with optional additional `buffer` and `align` arguments.
         To slice the data to the time period of interest, provide the `time_tuple` argument.
-        To return only the dataset variables of interest and check their presence,
-        provide the `variables` argument.
+        To return only the dataset variables of interest provide the `variables` argument.
 
         NOTE: Unless `single_var_as_array` is set to False a single-variable data source
         will be returned as :py:class:`xarray.DataArray` rather than :py:class:`xarray.Dataset`.
 
         Arguments
         ---------
-        path_or_key: str
-            Data catalog key. If a path to a raster file is provided it will be added
+        data_like: str, Path, xr.Dataset, xr.Datarray
+            Data catalog key, path to raster file or raster xarray data object.
+            If a path to a raster file is provided it will be added
             to the data_catalog with its based on the file basename without extension.
         bbox : array-like of floats
             (xmin, ymin, xmax, ymax) bounding box of area of interest (in WGS84 coordinates).
         geom : geopandas.GeoDataFrame/Series,
             A geometry defining the area of interest.
         zoom_level : int, tuple, optional
             Zoom level of the xyz tile dataset (0 is base level)
@@ -591,22 +617,28 @@
             If False, always return a Dataset. By default True.
 
         Returns
         -------
         obj: xarray.Dataset or xarray.DataArray
             RasterDataset
         """
-        if path_or_key not in self.sources and exists(abspath(path_or_key)):
-            path = str(abspath(path_or_key))
-            name = basename(path_or_key).split(".")[0]
+        if isinstance(data_like, (xr.DataArray, xr.Dataset)):
+            return data_like
+        elif not isinstance(data_like, (str, Path)):
+            raise ValueError(f'Unknown raster data type "{type(data_like).__name__}"')
+
+        if data_like not in self.sources and exists(abspath(data_like)):
+            path = str(abspath(data_like))
+            name = basename(data_like).split(".")[0]
             self.update(**{name: RasterDatasetAdapter(path=path, **kwargs)})
-        elif path_or_key in self.sources:
-            name = path_or_key
+        elif data_like in self.sources:
+            name = data_like
         else:
-            raise FileNotFoundError(f"No such file or catalog key: {path_or_key}")
+            raise FileNotFoundError(f"No such file or catalog key: {data_like}")
+
         self._used_data.append(name)
         source = self.sources[name]
         self.logger.info(
             f"DataCatalog: Getting {name} RasterDataset {source.driver} data from {source.path}"
         )
         obj = self.sources[name].get_data(
             bbox=bbox,
@@ -620,33 +652,33 @@
             cache_root=self._cache_dir if self.cache else None,
             logger=self.logger,
         )
         return obj
 
     def get_geodataframe(
         self,
-        path_or_key: Union[str, Path],
+        data_like: Union[str, Path, gpd.GeoDataFrame],
         bbox: List = None,
         geom: gpd.GeoDataFrame = None,
         buffer: Union[float, int] = 0,
         variables: Union[List, str] = None,
         predicate: str = "intersects",
         **kwargs,
     ):
-        """Returns a clipped and unified GeoDataFrame (vector) from the data catalog.
+        """Returns a clipped and unified GeoDataFrame (vector).
 
         To clip the data to the area of interest, provide a `bbox` or `geom`,
         with optional additional `buffer` and `align` arguments.
-        To return only the dataframe columns of interest and check their presence,
-        provide the `variables` argument.
+        To return only the dataframe columns of interest provide the `variables` argument.
 
         Arguments
         ---------
-        path_or_key: str
-            Data catalog key. If a path to a vector file is provided it will be added
+        data_like: str, Path, gpd.GeoDataFrame
+            Data catalog key, path to vector file or a vector geopandas object.
+            If a path to a vector file is provided it will be added
             to the data_catalog with its based on the file basename without extension.
         bbox : array-like of floats
             (xmin, ymin, xmax, ymax) bounding box of area of interest (in WGS84 coordinates).
         geom : geopandas.GeoDataFrame/Series,
             A geometry defining the area of interest.
         buffer : float, optional
             Buffer around the `bbox` or `geom` area of interest in meters. By default 0.
@@ -660,22 +692,28 @@
             Names of GeoDataFrame columns to return. By default all columns are returned.
 
         Returns
         -------
         gdf: geopandas.GeoDataFrame
             GeoDataFrame
         """
-        if path_or_key not in self.sources and exists(abspath(path_or_key)):
-            path = str(abspath(path_or_key))
-            name = basename(path_or_key).split(".")[0]
+        if isinstance(data_like, gpd.GeoDataFrame):
+            return data_like
+        elif not isinstance(data_like, (str, Path)):
+            raise ValueError(f'Unknown vector data type "{type(data_like).__name__}"')
+
+        if data_like not in self.sources and exists(abspath(data_like)):
+            path = str(abspath(data_like))
+            name = basename(data_like).split(".")[0]
             self.update(**{name: GeoDataFrameAdapter(path=path, **kwargs)})
-        elif path_or_key in self.sources:
-            name = path_or_key
+        elif data_like in self.sources:
+            name = data_like
         else:
-            raise FileNotFoundError(f"No such file or catalog key: {path_or_key}")
+            raise FileNotFoundError(f"No such file or catalog key: {data_like}")
+
         self._used_data.append(name)
         source = self.sources[name]
         self.logger.info(
             f"DataCatalog: Getting {name} GeoDataFrame {source.driver} data from {source.path}"
         )
         gdf = source.get_data(
             bbox=bbox,
@@ -685,38 +723,38 @@
             variables=variables,
             logger=self.logger,
         )
         return gdf
 
     def get_geodataset(
         self,
-        path_or_key: Union[Path, str],
+        data_like: Union[Path, str, xr.DataArray, xr.Dataset],
         bbox: List = None,
         geom: gpd.GeoDataFrame = None,
         buffer: Union[float, int] = 0,
         variables: List = None,
         time_tuple: Tuple = None,
         single_var_as_array: bool = True,
         **kwargs,
     ) -> xr.Dataset:
-        """Returns a clipped, sliced and unified GeoDataset from the data catalog.
+        """Returns a clipped, sliced and unified GeoDataset.
 
         To clip the data to the area of interest, provide a `bbox` or `geom`,
         with optional additional `buffer` and `align` arguments.
         To slice the data to the time period of interest, provide the `time_tuple` argument.
-        To return only the dataset variables of interest and check their presence,
-        provide the `variables` argument.
+        To return only the dataset variables of interest provide the `variables` argument.
 
         NOTE: Unless `single_var_as_array` is set to False a single-variable data source
         will be returned as xarray.DataArray rather than Dataset.
 
         Arguments
         ---------
-        path_or_key: str
-            Data catalog key. If a path to a file is provided it will be added
+        data_like: str, Path, xr.Dataset, xr.DataArray
+            Data catalog key, path to geodataset file or geodataset xarray object.
+            If a path to a file is provided it will be added
             to the data_catalog with its based on the file basename without extension.
         bbox : array-like of floats
             (xmin, ymin, xmax, ymax) bounding box of area of interest (in WGS84 coordinates).
         geom : geopandas.GeoDataFrame/Series,
             A geometry defining the area of interest.
         buffer : float, optional
             Buffer around the `bbox` or `geom` area of interest in meters. By default 0.
@@ -733,22 +771,28 @@
             If False, always return a Dataset. By default True.
 
         Returns
         -------
         obj: xarray.Dataset or xarray.DataArray
             GeoDataset
         """
-        if path_or_key not in self.sources and exists(abspath(path_or_key)):
-            path = str(abspath(path_or_key))
-            name = basename(path_or_key).split(".")[0]
+        if isinstance(data_like, (xr.DataArray, xr.Dataset)):
+            return data_like
+        elif not isinstance(data_like, (str, Path)):
+            raise ValueError(f'Unknown geo data type "{type(data_like).__name__}"')
+
+        if data_like not in self.sources and exists(abspath(data_like)):
+            path = str(abspath(data_like))
+            name = basename(data_like).split(".")[0]
             self.update(**{name: GeoDatasetAdapter(path=path, **kwargs)})
-        elif path_or_key in self.sources:
-            name = path_or_key
+        elif data_like in self.sources:
+            name = data_like
         else:
-            raise FileNotFoundError(f"No such file or catalog key: {path_or_key}")
+            raise FileNotFoundError(f"No such file or catalog key: {data_like}")
+
         self._used_data.append(name)
         source = self.sources[name]
         self.logger.info(
             f"DataCatalog: Getting {name} GeoDataset {source.driver} data from {source.path}"
         )
         obj = source.get_data(
             bbox=bbox,
@@ -759,27 +803,53 @@
             single_var_as_array=single_var_as_array,
             logger=self.logger,
         )
         return obj
 
     def get_dataframe(
         self,
-        path_or_key,
-        variables=None,
-        time_tuple=None,
+        data_like: Union[str, Path, pd.DataFrame],
+        variables: list = None,
+        time_tuple: tuple = None,
         **kwargs,
     ):
-        if path_or_key not in self.sources and exists(abspath(path_or_key)):
-            path = str(abspath(path_or_key))
-            name = basename(path_or_key).split(".")[0]
+        """Returns a unified and sliced DataFrame.
+
+        Parameters
+        ----------
+        data_like : str, Path, pd.DataFrame
+            Data catalog key, path to tabular data file or tabular pandas dataframe object.
+            If a path to a tabular data file is provided it will be added
+            to the data_catalog with its based on the file basename without extension.
+        variables : str or list of str, optional.
+            Names of GeoDataset variables to return. By default all dataset variables
+            are returned.
+        time_tuple : tuple of str, datetime, optional
+            Start and end date of period of interest. By default the entire time period
+            of the dataset is returned.
+
+        Returns
+        -------
+        pd.DataFrame
+            Tabular data
+        """
+        if isinstance(data_like, pd.DataFrame):
+            return data_like
+        elif not isinstance(data_like, (str, Path)):
+            raise ValueError(f'Unknown tabular data type "{type(data_like).__name__}"')
+
+        if data_like not in self.sources and exists(abspath(data_like)):
+            path = str(abspath(data_like))
+            name = basename(data_like).split(".")[0]
             self.update(**{name: DataFrameAdapter(path=path, **kwargs)})
-        elif path_or_key in self.sources:
-            name = path_or_key
+        elif data_like in self.sources:
+            name = data_like
         else:
-            raise FileNotFoundError(f"No such file or catalog key: {path_or_key}")
+            raise FileNotFoundError(f"No such file or catalog key: {data_like}")
+
         self._used_data.append(name)
         source = self.sources[name]
         self.logger.info(
             f"DataCatalog: Getting {name} DataFrame {source.driver} data from {source.path}"
         )
         obj = source.get_data(
             variables=variables,
```

### Comparing `hydromt-0.7.0/hydromt/flw.py` & `hydromt-0.7.1/hydromt/flw.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/gis_utils.py` & `hydromt-0.7.1/hydromt/gis_utils.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/io.py` & `hydromt-0.7.1/hydromt/io.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/log.py` & `hydromt-0.7.1/hydromt/log.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/merge.py` & `hydromt-0.7.1/hydromt/merge.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/models/__init__.py` & `hydromt-0.7.1/hydromt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/models/model_api.py` & `hydromt-0.7.1/hydromt/models/model_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,20 +195,22 @@
         opt = self._check_get_opt(opt)
 
         # merge cli region and res arguments with opt
         if region is not None:
             if self._CLI_ARGS["region"] not in opt:
                 opt = {self._CLI_ARGS["region"]: {}, **opt}
             opt[self._CLI_ARGS["region"]].update(region=region)
+
         # then loop over other methods
         for method in opt:
             # if any write_* functions are present in opt, skip the final self.write() call
             if method.startswith("write_"):
                 write = False
-            self._run_log_method(method, **opt[method])
+            kwargs = {} if opt[method] is None else opt[method]
+            self._run_log_method(method, **kwargs)
 
         # write
         if write:
             self.write()
 
     def update(
         self,
@@ -271,15 +273,16 @@
             self.logger.warning(f'"{method}" can only be called when building a model.')
 
         # loop over other methods from ini file
         for method in opt:
             # if any write_* functions are present in opt, skip the final self.write() call
             if method.startswith("write_"):
                 write = False
-            self._run_log_method(method, **opt[method])
+            kwargs = {} if opt[method] is None else opt[method]
+            self._run_log_method(method, **kwargs)
 
         # write
         if write:
             self.write()
 
     ## general setup methods
```

### Comparing `hydromt-0.7.0/hydromt/models/model_grid.py` & `hydromt-0.7.1/hydromt/models/model_grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,40 +164,45 @@
         """
         super().write(components=components)
 
     # Properties for subclass GridModel
     @property
     def res(self) -> Tuple[float, float]:
         """Returns the resolution of the model grid."""
-        if len(self._grid) > 0:
+        if len(self.grid) > 0:
             return self.grid.raster.res
 
     @property
     def transform(self):
         """Returns spatial transform of the model grid."""
-        if len(self._grid) > 0:
+        if len(self.grid) > 0:
             return self.grid.raster.transform
 
     @property
     def crs(self) -> Union[CRS, None]:
         """Returns coordinate reference system embedded in the model grid."""
-        if len(self._grid) > 0:
-            return CRS(self._grid.raster.crs)
+        if len(self.grid) > 0 and self.grid.raster.crs is not None:
+            return CRS(self.grid.raster.crs)
 
     @property
     def bounds(self) -> List[float]:
         """Returns the bounding box of the model grid."""
-        if len(self._grid) > 0:
+        if len(self.grid) > 0:
             return self.grid.raster.bounds
 
     @property
     def region(self) -> gpd.GeoDataFrame:
         """Returns the geometry of the model area of interest."""
         region = gpd.GeoDataFrame()
         if "region" in self.geoms:
             region = self.geoms["region"]
         elif len(self.grid) > 0:
-            crs = self.grid.raster.crs
-            if crs is None and hasattr(crs, "to_epsg"):
+            crs = self.crs
+            if crs is not None and hasattr(crs, "to_epsg"):
                 crs = crs.to_epsg()  # not all CRS have an EPSG code
             region = gpd.GeoDataFrame(geometry=[box(*self.bounds)], crs=crs)
         return region
+
+    def set_crs(self, crs: CRS) -> None:
+        """Set coordinate reference system of the model grid."""
+        if len(self.grid) > 0:
+            self.grid.raster.set_crs(crs)
```

### Comparing `hydromt-0.7.0/hydromt/models/model_lumped.py` & `hydromt-0.7.1/hydromt/models/model_lumped.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/models/model_mesh.py` & `hydromt-0.7.1/hydromt/models/model_mesh.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/models/model_network.py` & `hydromt-0.7.1/hydromt/models/model_network.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/models/model_plugins.py` & `hydromt-0.7.1/hydromt/models/model_plugins.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/raster.py` & `hydromt-0.7.1/hydromt/raster.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/stats/skills.py` & `hydromt-0.7.1/hydromt/stats/skills.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/vector.py` & `hydromt-0.7.1/hydromt/vector.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/workflows/basin_mask.py` & `hydromt-0.7.1/hydromt/workflows/basin_mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,19 +158,19 @@
             kwarg = dict(bbox=value)
         elif len(value) == 2:  # 2 floats
             kwarg = dict(xy=value)
     elif isinstance(value, tuple) and len(value) == 2:  # tuple of x and y coords
         kwarg = dict(xy=value)
     elif isinstance(value, int):  # single int
         kwarg = dict(basid=value)
-    elif isinstance(value, str) and isfile(value):
+    elif isinstance(value, (str, Path)) and isfile(value):
         kwarg = dict(geom=gpd.read_file(value))
     elif isinstance(value, gpd.GeoDataFrame):  # geometry
         kwarg = dict(geom=value)
-    elif isinstance(value, str) and isdir(value):
+    elif isinstance(value, (str, Path)) and isdir(value):
         kwarg = dict(root=value)
     if "geom" in kwarg and np.all(kwarg["geom"].geometry.type == "Point"):
         xy = (
             kwarg["geom"].geometry.x.values,
             kwarg["geom"].geometry.y.values,
         )
         kwarg = dict(xy=xy)
```

### Comparing `hydromt-0.7.0/hydromt/workflows/forcing.py` & `hydromt-0.7.1/hydromt/workflows/forcing.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/hydromt/workflows/rivers.py` & `hydromt-0.7.1/hydromt/workflows/rivers.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.7.0/pyproject.toml` & `hydromt-0.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "xmltodict",
     "zarr",
 ]
 requires-python = ">=3.8" # fix tests to support older versions
 readme = "README.rst"
 classifiers = [
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Hydrology",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ['version', 'description']
@@ -91,8 +91,8 @@
     "ignore:distutils Version classes are deprecated:DeprecationWarning",
     "ignore:getargs:DeprecationWarning", # The 'u' format is deprecated. Use 'U' instead.
     "ignore:The *staticgeoms:DeprecationWarning", 
     "ignore:The *staticmaps:DeprecationWarning", 
     "ignore:The set_staticmaps:DeprecationWarning", 
     "ignore:Adding a predefined data catalog:DeprecationWarning",
     "ignore:Shapely 2.0 is installed:UserWarning"
-]
+]
```

### Comparing `hydromt-0.7.0/PKG-INFO` & `hydromt-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: hydromt
-Version: 0.7.0
+Version: 0.7.1
 Summary: HydroMT: Automated and reproducible model building and analysis
 Author-email: Dirk Eilander <dirk.eilander@deltares.nl>, Hélène Boisgontier <helene.boisgontier@deltares.nl>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: affine
 Requires-Dist: bottleneck
@@ -57,15 +57,15 @@
 
 .. _readme:
 
 ===============================================================
 HydroMT: Automated and reproducible model building and analysis
 ===============================================================
 
-|pypi| |conda forge| |docs_latest| |docs_stable| |codecov| |license| |doi| |binder|
+|pypi| |conda forge| |docs_latest| |docs_stable| |binder| |codecov| |license| |doi| |joss_paper|
 
 
 What is HydroMT?
 ----------------
 **HydroMT** (Hydro Model Tools) is an open-source Python package that facilitates the process of 
 building and analyzing spatial geoscientific models with a focus on water system models. 
 It does so by automating the workflow to go from raw data to a complete model instance which 
@@ -106,15 +106,20 @@
 * hydromt_delwaq_: A framework for water quality (D-Water Quality) and emissions (D-Emissions) modelling.
 * hydromt_sfincs_: A fast 2D hydrodynamic flood model (SFINCS).
 * hydromt_fiat_: A flood impact model (FIAT).
 
 
 How to cite?
 ------------
-For publications, please cite our work using the DOI provided in the Zenodo badge |doi| that points to the latest release.
+For publications, please cite our JOSS paper |joss_paper|
+
+::
+    Eilander et al., (2023). HydroMT: Automated and reproducible model building and analysis. Journal of Open Source Software, 8(83), 4897, https://doi.org/10.21105/joss.04897
+
+To cite a specific software version please use the DOI provided in the Zenodo badge |doi| that points to the latest release.
 
 
 How to contribute?
 -------------------
 If you find any issues in the code or documentation feel free to leave an issue on the `github issue tracker. <https://github.com/Deltares/hydromt/issues>`_
 You can find information about how to contribute to the HydroMT project at our `contributing page. <https://deltares.github.io/hydromt/latest/dev/contributing>`_
 
@@ -163,7 +168,9 @@
     :alt: Zenodo
     :target: https://zenodo.org/badge/latestdoi/348020332
 
 .. |license| image:: https://img.shields.io/github/license/Deltares/hydromt?style=flat
     :alt: License
     :target: https://github.com/Deltares/hydromt/blob/main/LICENSE
 
+.. |joss_paper| image:: https://joss.theoj.org/papers/10.21105/joss.04897/status.svg
+   :target: https://doi.org/10.21105/joss.04897
```

