# Comparing `tmp/scimap-0.9.8.tar.gz` & `tmp/scimap-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scimap-0.9.8.tar", last modified: Sun Nov 22 15:33:57 2020, max compression
+gzip compressed data, was "scimap-0.9.9.tar", last modified: Sun Nov 22 16:18:08 2020, max compression
```

## Comparing `scimap-0.9.8.tar` & `scimap-0.9.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     2182 2020-10-27 13:56:22.855085 scimap-0.9.8/README.md
--rw-r--r--   0        0        0     2087 2020-11-22 15:33:50.551021 scimap-0.9.8/pyproject.toml
--rw-r--r--   0        0        0    14340 2020-11-22 00:25:53.394034 scimap-0.9.8/scimap/.DS_Store
--rw-r--r--   0        0        0      299 2020-06-11 21:05:24.159047 scimap-0.9.8/scimap/__init__.py
--rw-r--r--   0        0        0       21 2020-06-10 15:32:33.288385 scimap-0.9.8/scimap/__main__.py
--rw-r--r--   0        0        0     6148 2020-11-21 21:40:21.996834 scimap-0.9.8/scimap/archive/.DS_Store
--rwxr-xr-x   0        0        0     5768 2020-11-19 22:05:38.518374 scimap-0.9.8/scimap/archive/_gate_finder.py
--rw-r--r--   0        0        0     4683 2020-11-19 22:05:13.775026 scimap-0.9.8/scimap/archive/_image_viewer.py
--rwxr-xr-x   0        0        0     9329 2020-10-20 21:59:59.877372 scimap-0.9.8/scimap/archive/_spatial_expression.py
--rw-r--r--   0        0        0     6148 2020-11-16 20:07:09.238557 scimap-0.9.8/scimap/helpers/.DS_Store
--rw-r--r--   0        0        0      131 2020-11-16 19:52:40.464835 scimap-0.9.8/scimap/helpers/__init__.py
--rwxr-xr-x   0        0        0     2721 2020-11-16 21:04:03.360477 scimap-0.9.8/scimap/helpers/_add_roi.py
--rwxr-xr-x   0        0        0     4315 2020-10-27 17:43:28.541250 scimap-0.9.8/scimap/helpers/_classify.py
--rwxr-xr-x   0        0        0     2028 2020-06-11 21:36:05.210807 scimap-0.9.8/scimap/helpers/_rename.py
--rw-r--r--   0        0        0     1782 2020-11-10 02:52:13.000000 scimap-0.9.8/scimap/helpers/_scimap_to_csv.py
--rw-r--r--   0        0        0     6148 2020-11-21 21:40:34.985695 scimap-0.9.8/scimap/plotting/.DS_Store
--rw-r--r--   0        0        0      211 2020-10-25 17:50:57.422919 scimap-0.9.8/scimap/plotting/__init__.py
--rwxr-xr-x   0        0        0     7181 2020-11-22 03:07:24.777850 scimap-0.9.8/scimap/plotting/_gate_finder.py
--rwxr-xr-x   0        0        0     3475 2020-06-11 03:36:22.302674 scimap-0.9.8/scimap/plotting/_gmm_gate.py
--rw-r--r--   0        0        0     6173 2020-11-22 02:54:56.635274 scimap-0.9.8/scimap/plotting/_image_viewer.py
--rwxr-xr-x   0        0        0    11218 2020-10-27 21:00:07.356460 scimap-0.9.8/scimap/plotting/_spatial_distance.py
--rwxr-xr-x   0        0        0     7379 2020-11-18 16:46:08.552216 scimap-0.9.8/scimap/plotting/_spatial_interaction.py
--rw-r--r--   0        0        0     6148 2020-08-03 15:13:10.898777 scimap-0.9.8/scimap/preprocessing/.DS_Store
--rw-r--r--   0        0        0       79 2020-06-11 03:22:04.314693 scimap-0.9.8/scimap/preprocessing/__init__.py
--rw-r--r--   0        0        0     6256 2020-11-10 03:22:12.305973 scimap-0.9.8/scimap/preprocessing/_mcmicro_to_scimap.py
--rw-r--r--   0        0        0    14587 2020-10-30 17:07:41.337355 scimap-0.9.8/scimap/preprocessing/_rescale.py
--rw-r--r--   0        0        0     6148 2020-11-21 17:01:07.880584 scimap-0.9.8/scimap/tests/.DS_Store
--rw-r--r--   0        0        0     6148 2020-06-11 21:13:39.800191 scimap-0.9.8/scimap/tests/_data/.DS_Store
--rw-r--r--   0        0        0  2006242 2020-06-28 22:10:04.644487 scimap-0.9.8/scimap/tests/_data/example_data.csv
--rw-r--r--   0        0        0  1590001 2020-06-11 21:13:27.003848 scimap-0.9.8/scimap/tests/_data/example_data.h5ad
--rw-r--r--   0        0        0     1940 2020-05-11 18:45:43.711533 scimap-0.9.8/scimap/tests/_data/phenotype_workflow.csv
--rwxr-xr-x   0        0        0     1246 2020-11-10 03:19:04.437316 scimap-0.9.8/scimap/tests/test_helpers.py
--rwxr-xr-x   0        0        0      978 2020-10-30 15:39:36.268548 scimap-0.9.8/scimap/tests/test_preprocessing.py
--rwxr-xr-x   0        0        0     3338 2020-10-25 19:03:52.558497 scimap-0.9.8/scimap/tests/test_tools.py
--rw-r--r--   0        0        0     6148 2020-08-25 19:45:14.956751 scimap-0.9.8/scimap/tools/.DS_Store
--rw-r--r--   0        0        0      324 2020-10-25 17:50:33.259196 scimap-0.9.8/scimap/tools/__init__.py
--rwxr-xr-x   0        0        0    14671 2020-10-26 03:15:52.470635 scimap-0.9.8/scimap/tools/_cluster.py
--rw-r--r--   0        0        0    13649 2020-08-19 23:49:21.234240 scimap-0.9.8/scimap/tools/_phenotype_cells.py
--rwxr-xr-x   0        0        0     8113 2020-10-20 21:56:53.772926 scimap-0.9.8/scimap/tools/_spatial_aggregate.py
--rwxr-xr-x   0        0        0     6442 2020-08-24 23:08:53.350061 scimap-0.9.8/scimap/tools/_spatial_count.py
--rwxr-xr-x   0        0        0     4090 2020-10-25 17:49:59.731989 scimap-0.9.8/scimap/tools/_spatial_distance.py
--rwxr-xr-x   0        0        0     6779 2020-11-18 04:40:47.821250 scimap-0.9.8/scimap/tools/_spatial_expression.py
--rwxr-xr-x   0        0        0     9864 2020-10-23 14:53:17.575968 scimap-0.9.8/scimap/tools/_spatial_interaction.py
--rw-r--r--   0        0        0     3597 2020-11-22 15:33:57.714328 scimap-0.9.8/setup.py
--rw-r--r--   0        0        0     3793 2020-11-22 15:33:57.714912 scimap-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     2182 2020-10-27 13:56:22.855085 scimap-0.9.9/README.md
+-rw-r--r--   0        0        0     2069 2020-11-22 16:18:01.778486 scimap-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0    14340 2020-11-22 00:25:53.394034 scimap-0.9.9/scimap/.DS_Store
+-rw-r--r--   0        0        0      299 2020-06-11 21:05:24.159047 scimap-0.9.9/scimap/__init__.py
+-rw-r--r--   0        0        0       21 2020-06-10 15:32:33.288385 scimap-0.9.9/scimap/__main__.py
+-rw-r--r--   0        0        0     6148 2020-11-21 21:40:21.996834 scimap-0.9.9/scimap/archive/.DS_Store
+-rwxr-xr-x   0        0        0     5768 2020-11-19 22:05:38.518374 scimap-0.9.9/scimap/archive/_gate_finder.py
+-rw-r--r--   0        0        0     4683 2020-11-19 22:05:13.775026 scimap-0.9.9/scimap/archive/_image_viewer.py
+-rwxr-xr-x   0        0        0     9329 2020-10-20 21:59:59.877372 scimap-0.9.9/scimap/archive/_spatial_expression.py
+-rw-r--r--   0        0        0     6148 2020-11-16 20:07:09.238557 scimap-0.9.9/scimap/helpers/.DS_Store
+-rw-r--r--   0        0        0      131 2020-11-16 19:52:40.464835 scimap-0.9.9/scimap/helpers/__init__.py
+-rwxr-xr-x   0        0        0     2721 2020-11-16 21:04:03.360477 scimap-0.9.9/scimap/helpers/_add_roi.py
+-rwxr-xr-x   0        0        0     4315 2020-10-27 17:43:28.541250 scimap-0.9.9/scimap/helpers/_classify.py
+-rwxr-xr-x   0        0        0     2028 2020-06-11 21:36:05.210807 scimap-0.9.9/scimap/helpers/_rename.py
+-rw-r--r--   0        0        0     1782 2020-11-10 02:52:13.000000 scimap-0.9.9/scimap/helpers/_scimap_to_csv.py
+-rw-r--r--   0        0        0     6148 2020-11-21 21:40:34.985695 scimap-0.9.9/scimap/plotting/.DS_Store
+-rw-r--r--   0        0        0      211 2020-10-25 17:50:57.422919 scimap-0.9.9/scimap/plotting/__init__.py
+-rwxr-xr-x   0        0        0     7181 2020-11-22 03:07:24.777850 scimap-0.9.9/scimap/plotting/_gate_finder.py
+-rwxr-xr-x   0        0        0     3475 2020-06-11 03:36:22.302674 scimap-0.9.9/scimap/plotting/_gmm_gate.py
+-rw-r--r--   0        0        0     6173 2020-11-22 02:54:56.635274 scimap-0.9.9/scimap/plotting/_image_viewer.py
+-rwxr-xr-x   0        0        0    11218 2020-10-27 21:00:07.356460 scimap-0.9.9/scimap/plotting/_spatial_distance.py
+-rwxr-xr-x   0        0        0     7379 2020-11-18 16:46:08.552216 scimap-0.9.9/scimap/plotting/_spatial_interaction.py
+-rw-r--r--   0        0        0     6148 2020-08-03 15:13:10.898777 scimap-0.9.9/scimap/preprocessing/.DS_Store
+-rw-r--r--   0        0        0       79 2020-06-11 03:22:04.314693 scimap-0.9.9/scimap/preprocessing/__init__.py
+-rw-r--r--   0        0        0     6256 2020-11-10 03:22:12.305973 scimap-0.9.9/scimap/preprocessing/_mcmicro_to_scimap.py
+-rw-r--r--   0        0        0    14587 2020-10-30 17:07:41.337355 scimap-0.9.9/scimap/preprocessing/_rescale.py
+-rw-r--r--   0        0        0     6148 2020-11-21 17:01:07.880584 scimap-0.9.9/scimap/tests/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-06-11 21:13:39.800191 scimap-0.9.9/scimap/tests/_data/.DS_Store
+-rw-r--r--   0        0        0  2006242 2020-06-28 22:10:04.644487 scimap-0.9.9/scimap/tests/_data/example_data.csv
+-rw-r--r--   0        0        0  1590001 2020-06-11 21:13:27.003848 scimap-0.9.9/scimap/tests/_data/example_data.h5ad
+-rw-r--r--   0        0        0     1940 2020-05-11 18:45:43.711533 scimap-0.9.9/scimap/tests/_data/phenotype_workflow.csv
+-rwxr-xr-x   0        0        0     1246 2020-11-10 03:19:04.437316 scimap-0.9.9/scimap/tests/test_helpers.py
+-rwxr-xr-x   0        0        0      978 2020-10-30 15:39:36.268548 scimap-0.9.9/scimap/tests/test_preprocessing.py
+-rwxr-xr-x   0        0        0     3338 2020-10-25 19:03:52.558497 scimap-0.9.9/scimap/tests/test_tools.py
+-rw-r--r--   0        0        0     6148 2020-08-25 19:45:14.956751 scimap-0.9.9/scimap/tools/.DS_Store
+-rw-r--r--   0        0        0      324 2020-10-25 17:50:33.259196 scimap-0.9.9/scimap/tools/__init__.py
+-rwxr-xr-x   0        0        0    14671 2020-10-26 03:15:52.470635 scimap-0.9.9/scimap/tools/_cluster.py
+-rw-r--r--   0        0        0    13649 2020-08-19 23:49:21.234240 scimap-0.9.9/scimap/tools/_phenotype_cells.py
+-rwxr-xr-x   0        0        0     8113 2020-10-20 21:56:53.772926 scimap-0.9.9/scimap/tools/_spatial_aggregate.py
+-rwxr-xr-x   0        0        0     6442 2020-08-24 23:08:53.350061 scimap-0.9.9/scimap/tools/_spatial_count.py
+-rwxr-xr-x   0        0        0     4090 2020-10-25 17:49:59.731989 scimap-0.9.9/scimap/tools/_spatial_distance.py
+-rwxr-xr-x   0        0        0     6779 2020-11-18 04:40:47.821250 scimap-0.9.9/scimap/tools/_spatial_expression.py
+-rwxr-xr-x   0        0        0     9864 2020-10-23 14:53:17.575968 scimap-0.9.9/scimap/tools/_spatial_interaction.py
+-rw-r--r--   0        0        0     3572 2020-11-22 16:18:08.424261 scimap-0.9.9/setup.py
+-rw-r--r--   0        0        0     3754 2020-11-22 16:18:08.424744 scimap-0.9.9/PKG-INFO
```

### Comparing `scimap-0.9.8/README.md` & `scimap-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/pyproject.toml` & `scimap-0.9.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "scimap"
-version = "0.9.8"
+version = "0.9.9"
 description = "Single-Cell Image Analysis Package"
 
 license = "MIT"
 
 authors = ["Ajit Johnson Nirmal <ajitjohnson.n@gmail.com>"]
 
 readme = "README.md"
@@ -40,15 +40,14 @@
 PhenoGraph = "^1.5.7"
 scanpy = "^1.6.0"
 mkdocs = "^1.1.2"
 plotly = "^4.12.0"
 TiffFile = "^2020.11.18"
 dask = "^2.30.0"
 zarr = "^2.5.0"
-PyQt5 = "^5.15.1"
 napari = "<=0.3.4"
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
 black = "19.10b0"
 isort = "4.3.21"
```

### Comparing `scimap-0.9.8/scimap/.DS_Store` & `scimap-0.9.9/scimap/.DS_Store`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/archive/.DS_Store` & `scimap-0.9.9/scimap/archive/.DS_Store`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/archive/_gate_finder.py` & `scimap-0.9.9/scimap/archive/_gate_finder.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/archive/_image_viewer.py` & `scimap-0.9.9/scimap/archive/_image_viewer.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/archive/_spatial_expression.py` & `scimap-0.9.9/scimap/archive/_spatial_expression.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/helpers/.DS_Store` & `scimap-0.9.9/scimap/helpers/.DS_Store`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/helpers/_add_roi.py` & `scimap-0.9.9/scimap/helpers/_add_roi.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/helpers/_classify.py` & `scimap-0.9.9/scimap/helpers/_classify.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/helpers/_rename.py` & `scimap-0.9.9/scimap/helpers/_rename.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/helpers/_scimap_to_csv.py` & `scimap-0.9.9/scimap/helpers/_scimap_to_csv.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/plotting/.DS_Store` & `scimap-0.9.9/scimap/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/plotting/_gate_finder.py` & `scimap-0.9.9/scimap/plotting/_gate_finder.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/plotting/_gmm_gate.py` & `scimap-0.9.9/scimap/plotting/_gmm_gate.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/plotting/_image_viewer.py` & `scimap-0.9.9/scimap/plotting/_image_viewer.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/plotting/_spatial_distance.py` & `scimap-0.9.9/scimap/plotting/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/plotting/_spatial_interaction.py` & `scimap-0.9.9/scimap/plotting/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/preprocessing/.DS_Store` & `scimap-0.9.9/scimap/preprocessing/.DS_Store`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/preprocessing/_mcmicro_to_scimap.py` & `scimap-0.9.9/scimap/preprocessing/_mcmicro_to_scimap.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/preprocessing/_rescale.py` & `scimap-0.9.9/scimap/preprocessing/_rescale.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tests/.DS_Store` & `scimap-0.9.9/scimap/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tests/_data/.DS_Store` & `scimap-0.9.9/scimap/tests/_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tests/_data/example_data.csv` & `scimap-0.9.9/scimap/tests/_data/example_data.csv`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tests/_data/example_data.h5ad` & `scimap-0.9.9/scimap/tests/_data/example_data.h5ad`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tests/_data/phenotype_workflow.csv` & `scimap-0.9.9/scimap/tests/_data/phenotype_workflow.csv`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tests/test_helpers.py` & `scimap-0.9.9/scimap/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tests/test_preprocessing.py` & `scimap-0.9.9/scimap/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tests/test_tools.py` & `scimap-0.9.9/scimap/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tools/.DS_Store` & `scimap-0.9.9/scimap/tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tools/_cluster.py` & `scimap-0.9.9/scimap/tools/_cluster.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tools/_phenotype_cells.py` & `scimap-0.9.9/scimap/tools/_phenotype_cells.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tools/_spatial_aggregate.py` & `scimap-0.9.9/scimap/tools/_spatial_aggregate.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tools/_spatial_count.py` & `scimap-0.9.9/scimap/tools/_spatial_count.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tools/_spatial_distance.py` & `scimap-0.9.9/scimap/tools/_spatial_distance.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tools/_spatial_expression.py` & `scimap-0.9.9/scimap/tools/_spatial_expression.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/scimap/tools/_spatial_interaction.py` & `scimap-0.9.9/scimap/tools/_spatial_interaction.py`

 * *Files identical despite different names*

### Comparing `scimap-0.9.8/setup.py` & `scimap-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
  'scimap.tools']
 
 package_data = \
 {'': ['*'], 'scimap.tests': ['_data/*']}
 
 install_requires = \
 ['PhenoGraph>=1.5.7,<2.0.0',
- 'PyQt5>=5.15.1,<6.0.0',
  'TiffFile>=2020.11.18,<2021.0.0',
  'anndata>=0.7.4,<0.8.0',
  'dask>=2.30.0,<3.0.0',
  'matplotlib>=3.2.1,<4.0.0',
  'mkdocs>=1.1.2,<2.0.0',
  'napari<=0.3.4',
  'numpy>=1.18.5,<2.0.0',
@@ -35,15 +34,15 @@
  'zarr>=2.5.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['scimap = scimap.cli:main']}
 
 setup_kwargs = {
     'name': 'scimap',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Single-Cell Image Analysis Package',
     'long_description': '# Single-Cell Image Analysis Package\n\nScimap is a scalable toolkit for analyzing single-cell multiplex imaging data. The package uses the [anndata](https://anndata.readthedocs.io/en/stable/anndata.AnnData.html) framework making it easy to integrate with other popular single-cell analysis toolkits such as [scanpy](https://scanpy.readthedocs.io/en/latest/#). It includes preprocessing, phenotyping, visualization, clustering, spatial analysis and differential spatial testing. The Python-based implementation efficiently deals with datasets of more than one million cells.\n\n\n[![Unix Build Status](https://img.shields.io/travis/ajitjohnson/scimap/master.svg?label=unix)](https://travis-ci.org/ajitjohnson/scimap)\n[![Windows Build Status](https://img.shields.io/appveyor/ci/ajitjohnson/scimap/master.svg?label=windows)](https://ci.appveyor.com/project/ajitjohnson/scimap)\n[![Documentation Status](https://readthedocs.org/projects/scimap-doc/badge/?version=latest)](https://scimap-doc.readthedocs.io/en/latest/?badge=latest)\n[![Downloads](https://pepy.tech/badge/scimap)](https://pepy.tech/project/scimap)\n[![PyPI Version](https://img.shields.io/pypi/v/scimap.svg)](https://pypi.org/project/scimap)\n[![PyPI License](https://img.shields.io/pypi/l/scimap.svg)](https://pypi.org/project/scimap)\n<!--[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/ajitjohnson/scimap.svg)](https://scrutinizer-ci.com/g/ajitjohnson/scimap/?branch=master)-->\n<!--[![Coverage Status](https://img.shields.io/coveralls/ajitjohnson/scimap/master.svg)](https://coveralls.io/r/ajitjohnson/scimap) -->\n\n## Installation\n\nWe strongly recommend installing `scimap` in a fresh virtual environment.\n\n```\n# If you have conda installed\nconda create --name scimap python=3.7\nconda activate scimap\n```\n\nInstall `scimap` directly into an activated virtual environment:\n\n```python\n$ pip install scimap\n$ pip install napari[all] # For visualizing images\n```\n\nAfter installation, the package can be imported as:\n\n```python\n$ python\n>>> import scimap as sm\n```\n\n## Get Started\n\n\n#### Detailed documentation of `scimap` functions and tutorials are available [here](https://scimap-doc.readthedocs.io/en/latest/).\n',
     'author': 'Ajit Johnson Nirmal',
     'author_email': 'ajitjohnson.n@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://pypi.org/project/scimap',
```

### Comparing `scimap-0.9.8/PKG-INFO` & `scimap-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scimap
-Version: 0.9.8
+Version: 0.9.9
 Summary: Single-Cell Image Analysis Package
 Home-page: https://pypi.org/project/scimap
 License: MIT
 Keywords: image analysis,multiplex imaging,single cell analysis
 Author: Ajit Johnson Nirmal
 Author-email: ajitjohnson.n@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -13,15 +13,14 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: PhenoGraph (>=1.5.7,<2.0.0)
-Requires-Dist: PyQt5 (>=5.15.1,<6.0.0)
 Requires-Dist: TiffFile (>=2020.11.18,<2021.0.0)
 Requires-Dist: anndata (>=0.7.4,<0.8.0)
 Requires-Dist: dask (>=2.30.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.2.1,<4.0.0)
 Requires-Dist: mkdocs (>=1.1.2,<2.0.0)
 Requires-Dist: napari (<=0.3.4)
 Requires-Dist: numpy (>=1.18.5,<2.0.0)
```

