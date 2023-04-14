# Comparing `tmp/digitalarztools-0.0.7.tar.gz` & `tmp/digitalarztools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/digitalarztools-0.0.7.tar", last modified: Thu Mar  2 22:22:20 2023, max compression
+gzip compressed data, was "dist/digitalarztools-0.0.8.tar", last modified: Fri Apr 14 15:06:47 2023, max compression
```

## Comparing `digitalarztools-0.0.7.tar` & `digitalarztools-0.0.8.tar`

### file list

```diff
@@ -1,114 +1,116 @@
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.641731 digitalarztools-0.0.7/
--rw-r--r--   0 atherashraf   (501) staff       (20)      595 2023-03-02 22:22:20.641285 digitalarztools-0.0.7/PKG-INFO
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.564568 digitalarztools-0.0.7/digitalarztools/
--rw-r--r--   0 atherashraf   (501) staff       (20)        2 2022-12-04 11:04:00.000000 digitalarztools-0.0.7/digitalarztools/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.570076 digitalarztools-0.0.7/digitalarztools/io/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:46:14.000000 digitalarztools-0.0.7/digitalarztools/io/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6740 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/io/file_io.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      606 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/io/url_io.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.571882 digitalarztools-0.0.7/digitalarztools/operations/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/operations/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1433 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/operations/transformation.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.576421 digitalarztools-0.0.7/digitalarztools/pipelines/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/pipelines/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     5517 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/alos_palser.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.578301 digitalarztools-0.0.7/digitalarztools/pipelines/config/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/config/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4188 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/config/data_centers.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.581966 digitalarztools-0.0.7/digitalarztools/pipelines/earth_explorer/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/earth_explorer/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3059 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/earth_explorer/landsat.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    15085 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/earth_explorer/m2m.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.582934 digitalarztools-0.0.7/digitalarztools/pipelines/gee/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.583836 digitalarztools-0.0.7/digitalarztools/pipelines/gee/analysis/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/analysis/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1035 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/analysis/indices.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.591139 digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1582 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/auth.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      887 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/feature_collection.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2748 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/gee_api.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1092 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/gee_map.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     8600 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/image.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6061 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/image_collection.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4608 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/region.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      213 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/grace.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      307 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/landsat.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.597240 digitalarztools-0.0.7/digitalarztools/pipelines/nasa/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/nasa/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2898 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/pipelines/nasa/chirp.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    13082 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/nasa/geos.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    24728 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/nasa/merra.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    10724 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/nasa/variables_info.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.603869 digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3621 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/n_van_genuchten.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    12834 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/soil_contents.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4915 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/theta_fc.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3705 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/theta_res.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7294 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/theta_sat2.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     4037 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/pipelines/srtm.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.612331 digitalarztools-0.0.7/digitalarztools/raster/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-03 12:45:02.000000 digitalarztools-0.0.7/digitalarztools/raster/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.629531 digitalarztools-0.0.7/digitalarztools/raster/analysis/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1512 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/biomass_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    14835 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/clear_sky_radiation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3828 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/constants.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3700 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/dem_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1427 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/emissivity_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    17336 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/et_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6426 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/leaf_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    39751 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/meteo_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3811 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/resistance_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7415 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/roughness_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     9895 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/soil_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    40168 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/soil_moisture.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    49086 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/solar_radiation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    15057 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/temperature_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    27093 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/unstable.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7841 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/vegitation_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      666 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/analysis/water_analysis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     3419 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/band_process.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.631471 digitalarztools-0.0.7/digitalarztools/raster/datasets/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/datasets/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    40684 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/datasets/rio_landsat.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      173 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/datasets/rio_modis.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2263 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/datasets/rio_probav_viirs.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    14536 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/gdal_raster.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2508 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/gdal_raster_io.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     8494 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/hdf_reader.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1875 2022-10-08 11:45:28.000000 digitalarztools-0.0.7/digitalarztools/raster/indices.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.632061 digitalarztools-0.0.7/digitalarztools/raster/opencv/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/raster/opencv/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     6860 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/opencv/segmentation.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     2118 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/raster/rio_extraction.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     9789 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/rio_process.py
--rw-r--r--   0 atherashraf   (501) staff       (20)    33790 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/raster/rio_raster.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.632975 digitalarztools-0.0.7/digitalarztools/test/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/test/__init__.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.633347 digitalarztools-0.0.7/digitalarztools/test/raster/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/test/raster/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      913 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/test/raster/test_functionalities.py
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/test/test_config.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.636191 digitalarztools-0.0.7/digitalarztools/utils/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.7/digitalarztools/utils/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     7383 2023-03-02 21:25:38.000000 digitalarztools-0.0.7/digitalarztools/utils/date_utils.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1128 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/utils/logger.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     1009 2023-02-09 19:26:46.000000 digitalarztools-0.0.7/digitalarztools/utils/waitbar_console.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.637294 digitalarztools-0.0.7/digitalarztools/vector/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 10:28:22.000000 digitalarztools-0.0.7/digitalarztools/vector/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)     8757 2023-03-02 22:15:56.000000 digitalarztools-0.0.7/digitalarztools/vector/gpd_vector.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.567652 digitalarztools-0.0.7/digitalarztools.egg-info/
--rw-r--r--   0 atherashraf   (501) staff       (20)      595 2023-03-02 22:22:20.000000 digitalarztools-0.0.7/digitalarztools.egg-info/PKG-INFO
--rw-r--r--   0 atherashraf   (501) staff       (20)     3827 2023-03-02 22:22:20.000000 digitalarztools-0.0.7/digitalarztools.egg-info/SOURCES.txt
--rw-r--r--   0 atherashraf   (501) staff       (20)        1 2023-03-02 22:22:20.000000 digitalarztools-0.0.7/digitalarztools.egg-info/dependency_links.txt
--rw-r--r--   0 atherashraf   (501) staff       (20)       21 2023-03-02 22:22:20.000000 digitalarztools-0.0.7/digitalarztools.egg-info/top_level.txt
--rw-r--r--   0 atherashraf   (501) staff       (20)       38 2023-03-02 22:22:20.641874 digitalarztools-0.0.7/setup.cfg
--rw-r--r--   0 atherashraf   (501) staff       (20)     1449 2023-03-02 22:22:17.000000 digitalarztools-0.0.7/setup.py
-drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-03-02 22:22:20.640346 digitalarztools-0.0.7/test/
--rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:02:02.000000 digitalarztools-0.0.7/test/__init__.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      112 2022-12-03 18:32:14.000000 digitalarztools-0.0.7/test/test_config.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      783 2022-12-04 11:47:04.000000 digitalarztools-0.0.7/test/test_raster_io.py
--rw-r--r--   0 atherashraf   (501) staff       (20)      309 2022-12-04 11:11:10.000000 digitalarztools-0.0.7/test/test_vector_io.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.749206 digitalarztools-0.0.8/
+-rw-r--r--   0 atherashraf   (501) staff       (20)      595 2023-04-14 15:06:47.748707 digitalarztools-0.0.8/PKG-INFO
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.658429 digitalarztools-0.0.8/digitalarztools/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        2 2022-12-04 11:04:00.000000 digitalarztools-0.0.8/digitalarztools/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.662592 digitalarztools-0.0.8/digitalarztools/io/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:46:14.000000 digitalarztools-0.0.8/digitalarztools/io/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7106 2023-04-14 08:01:50.000000 digitalarztools-0.0.8/digitalarztools/io/file_io.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      606 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/io/url_io.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.664300 digitalarztools-0.0.8/digitalarztools/operations/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/operations/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1433 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/operations/transformation.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.668883 digitalarztools-0.0.8/digitalarztools/pipelines/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     5517 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/alos_palser.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.671071 digitalarztools-0.0.8/digitalarztools/pipelines/config/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/config/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     4188 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/config/data_centers.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.673344 digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3059 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/landsat.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    15085 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/m2m.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.674604 digitalarztools-0.0.8/digitalarztools/pipelines/gee/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.675372 digitalarztools-0.0.8/digitalarztools/pipelines/gee/analysis/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/analysis/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1035 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/analysis/indices.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.681417 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1582 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/auth.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      887 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/feature_collection.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2748 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/gee_api.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1092 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/gee_map.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     8600 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/image.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6061 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/image_collection.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     4608 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/region.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      213 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/grace.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      307 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/landsat.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.686826 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2898 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/chirp.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    13082 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/geos.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    24728 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/merra.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    10724 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/nasa/variables_info.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.692979 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3621 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/n_van_genuchten.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    12834 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/soil_contents.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     4915 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_fc.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3705 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_res.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7294 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_sat2.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     4037 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/pipelines/srtm.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.704686 digitalarztools-0.0.8/digitalarztools/raster/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-03 12:45:02.000000 digitalarztools-0.0.8/digitalarztools/raster/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.727369 digitalarztools-0.0.8/digitalarztools/raster/analysis/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1512 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/biomass_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    14835 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/clear_sky_radiation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3828 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/constants.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3700 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/dem_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1427 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/emissivity_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    17336 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/et_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6426 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/leaf_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    39751 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/meteo_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3811 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/resistance_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7415 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/roughness_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     9895 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/soil_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    40168 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/soil_moisture.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    49086 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/solar_radiation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    15057 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/temperature_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    27093 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/unstable.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7841 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/vegitation_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      666 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/analysis/water_analysis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3427 2023-04-14 08:01:50.000000 digitalarztools-0.0.8/digitalarztools/raster/band_process.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     5726 2023-04-14 08:01:50.000000 digitalarztools-0.0.8/digitalarztools/raster/cog_raster.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.731834 digitalarztools-0.0.8/digitalarztools/raster/datasets/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/datasets/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    40684 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/datasets/rio_landsat.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      173 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/datasets/rio_modis.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2263 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/datasets/rio_probav_viirs.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    14536 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/gdal_raster.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2508 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/gdal_raster_io.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     8494 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/hdf_reader.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1875 2022-10-08 11:45:28.000000 digitalarztools-0.0.8/digitalarztools/raster/indices.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.732954 digitalarztools-0.0.8/digitalarztools/raster/opencv/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/raster/opencv/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     6860 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/opencv/segmentation.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     2118 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/raster/rio_extraction.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     9789 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/raster/rio_process.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)    34443 2023-04-14 08:01:50.000000 digitalarztools-0.0.8/digitalarztools/raster/rio_raster.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.735591 digitalarztools-0.0.8/digitalarztools/test/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/test/__init__.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.737219 digitalarztools-0.0.8/digitalarztools/test/raster/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/test/raster/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      913 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/test/raster/test_functionalities.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/test/test_config.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.742603 digitalarztools-0.0.8/digitalarztools/utils/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-14 14:45:50.000000 digitalarztools-0.0.8/digitalarztools/utils/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     7383 2023-03-02 21:25:38.000000 digitalarztools-0.0.8/digitalarztools/utils/date_utils.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1128 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/utils/logger.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     5487 2023-04-14 08:02:54.000000 digitalarztools-0.0.8/digitalarztools/utils/s3_utils.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1009 2023-02-09 19:26:46.000000 digitalarztools-0.0.8/digitalarztools/utils/waitbar_console.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.743865 digitalarztools-0.0.8/digitalarztools/vector/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 10:28:22.000000 digitalarztools-0.0.8/digitalarztools/vector/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)     8757 2023-03-02 22:15:56.000000 digitalarztools-0.0.8/digitalarztools/vector/gpd_vector.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.660757 digitalarztools-0.0.8/digitalarztools.egg-info/
+-rw-r--r--   0 atherashraf   (501) staff       (20)      595 2023-04-14 15:06:47.000000 digitalarztools-0.0.8/digitalarztools.egg-info/PKG-INFO
+-rw-r--r--   0 atherashraf   (501) staff       (20)     3898 2023-04-14 15:06:47.000000 digitalarztools-0.0.8/digitalarztools.egg-info/SOURCES.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)        1 2023-04-14 15:06:47.000000 digitalarztools-0.0.8/digitalarztools.egg-info/dependency_links.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)       21 2023-04-14 15:06:47.000000 digitalarztools-0.0.8/digitalarztools.egg-info/top_level.txt
+-rw-r--r--   0 atherashraf   (501) staff       (20)       38 2023-04-14 15:06:47.749336 digitalarztools-0.0.8/setup.cfg
+-rw-r--r--   0 atherashraf   (501) staff       (20)     1449 2023-04-14 08:03:38.000000 digitalarztools-0.0.8/setup.py
+drwxr-xr-x   0 atherashraf   (501) staff       (20)        0 2023-04-14 15:06:47.747069 digitalarztools-0.0.8/test/
+-rw-r--r--   0 atherashraf   (501) staff       (20)        0 2022-12-04 11:02:02.000000 digitalarztools-0.0.8/test/__init__.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      112 2022-12-03 18:32:14.000000 digitalarztools-0.0.8/test/test_config.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      783 2022-12-04 11:47:04.000000 digitalarztools-0.0.8/test/test_raster_io.py
+-rw-r--r--   0 atherashraf   (501) staff       (20)      309 2022-12-04 11:11:10.000000 digitalarztools-0.0.8/test/test_vector_io.py
```

### Comparing `digitalarztools-0.0.7/PKG-INFO` & `digitalarztools-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalarztools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Digital Arz tools for applications
 Home-page: UNKNOWN
 Author: Ather Ashraf
 Author-email: atherashraf@gmail.com
 License: UNKNOWN
 Keywords: raster,vector,digitalarz
 Platform: UNKNOWN
```

### Comparing `digitalarztools-0.0.7/digitalarztools/io/file_io.py` & `digitalarztools-0.0.8/digitalarztools/io/file_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 class FileIO:
     @classmethod
     def mkdirs_list(cls, file_paths: list):
         for fp in file_paths:
             cls.mkdirs(fp)
 
     @staticmethod
+    def get_file_basedir_basename(file_path: str):
+        if os.path.exists(file_path):
+            return os.path.dirname(file_path), os.path.basename(file_path)
+
+    @staticmethod
     def mkdirs(file_path: str):
         dir_name = os.path.dirname(file_path) if '.' in file_path[-5:] else file_path
         # dir_name = os.path.dirname(file_path) if is_file else file_path
         if not os.path.exists(dir_name):
             os.makedirs(dir_name)
         return dir_name
 
@@ -108,14 +113,19 @@
 
     @staticmethod
     def get_file_name_ext(fp):
         base_name = os.path.basename(fp)
         sfp = base_name.split(".")
         return ",".join(sfp[:-1]), sfp[-1]
 
+    @staticmethod
+    def get_file_basedir_basename(file_path: str):
+        if os.path.exists(file_path):
+            return os.path.dirname(file_path), os.path.basename(file_path)
+
     @classmethod
     def read_prj_file(cls, prj_path) -> pyproj.CRS:
         name, ext = cls.get_file_name_ext(prj_path)
         if ext == "prj":
             with open(prj_path) as f:
                 wkt = f.read()
                 crs = pyproj.CRS.from_wkt(wkt)
```

### Comparing `digitalarztools-0.0.7/digitalarztools/io/url_io.py` & `digitalarztools-0.0.8/digitalarztools/io/url_io.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/operations/transformation.py` & `digitalarztools-0.0.8/digitalarztools/operations/transformation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/alos_palser.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/alos_palser.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/config/data_centers.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/config/data_centers.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/earth_explorer/landsat.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/landsat.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/earth_explorer/m2m.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/earth_explorer/m2m.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/gee/analysis/indices.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/gee/analysis/indices.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/auth.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/auth.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/feature_collection.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/feature_collection.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/gee_api.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/gee_api.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/gee_map.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/gee_map.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/image.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/image.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/image_collection.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/image_collection.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/gee/core/region.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/gee/core/region.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/nasa/chirp.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/nasa/chirp.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/nasa/geos.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/nasa/geos.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/nasa/merra.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/nasa/merra.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/nasa/variables_info.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/nasa/variables_info.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/n_van_genuchten.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/n_van_genuchten.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/soil_contents.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/soil_contents.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/theta_fc.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_fc.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/theta_res.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_res.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/soil_grids/theta_sat2.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/soil_grids/theta_sat2.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/pipelines/srtm.py` & `digitalarztools-0.0.8/digitalarztools/pipelines/srtm.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/biomass_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/biomass_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/clear_sky_radiation.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/clear_sky_radiation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/constants.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/constants.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/dem_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/dem_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/emissivity_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/emissivity_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/et_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/et_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/leaf_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/leaf_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/meteo_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/meteo_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/resistance_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/resistance_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/roughness_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/roughness_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/soil_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/soil_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/soil_moisture.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/soil_moisture.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/solar_radiation.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/solar_radiation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/temperature_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/temperature_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/unstable.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/unstable.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/vegitation_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/vegitation_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/analysis/water_analysis.py` & `digitalarztools-0.0.8/digitalarztools/raster/analysis/water_analysis.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/band_process.py` & `digitalarztools-0.0.8/digitalarztools/raster/band_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,16 @@
 
         Data_Out[Data_Out > 0.1] = 1
         Data_Out[Data_Out <= 0.1] = 0
 
         return (Data_Out)
 
     @staticmethod
-    def get_summary_data(data: np.ndarray, nodata=None):
+    def get_summary_data(data: np.ndarray = None, nodata=None):
+
         data = data.astype(np.float64)
         data[data == nodata] = np.nan
         mean_val = np.nanmean(data)
         min_val = np.nanmin(data)
         max_val = np.nanmax(data)
         std_val = np.nanstd(data)
         q25_val = np.nanquantile(data, 0.25)
```

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/datasets/rio_landsat.py` & `digitalarztools-0.0.8/digitalarztools/raster/datasets/rio_landsat.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/datasets/rio_probav_viirs.py` & `digitalarztools-0.0.8/digitalarztools/raster/datasets/rio_probav_viirs.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/gdal_raster.py` & `digitalarztools-0.0.8/digitalarztools/raster/gdal_raster.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/gdal_raster_io.py` & `digitalarztools-0.0.8/digitalarztools/raster/gdal_raster_io.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/hdf_reader.py` & `digitalarztools-0.0.8/digitalarztools/raster/hdf_reader.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/indices.py` & `digitalarztools-0.0.8/digitalarztools/raster/indices.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/opencv/segmentation.py` & `digitalarztools-0.0.8/digitalarztools/raster/opencv/segmentation.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/rio_extraction.py` & `digitalarztools-0.0.8/digitalarztools/raster/rio_extraction.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/rio_process.py` & `digitalarztools-0.0.8/digitalarztools/raster/rio_process.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/raster/rio_raster.py` & `digitalarztools-0.0.8/digitalarztools/raster/rio_raster.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-import osimport reimport tracebackfrom itertools import productimport geopandas as gpdfrom typing import Unionimport numpy as npimport pyprojimport rasteriofrom affine import Affinefrom rasterio import DatasetReader, MemoryFile, windowsfrom rasterio.coords import BoundingBoxfrom rasterio.crs import CRSfrom rasterio.enums import Resamplingfrom rasterio.features import shapes, rasterizefrom rasterio.mask import maskfrom rasterio.plot import showfrom rasterio.warp import calculate_default_transform, reprojectfrom shapely.geometry import Point, shape, Polygonfrom shapely.ops import transformfrom digitalarztools.operations.transformation import TransformationOperationsfrom digitalarztools.io.file_io import FileIOfrom digitalarztools.raster.indices import IndicesCalcfrom digitalarztools.utils.logger import da_loggerfrom digitalarztools.vector.gpd_vector import GPDVectorclass RioRaster:    """        Geo Raster contain informaiton about geotransform and projection        GDAL geotransform = (c,a,b, f,d,e)        RasterIO = (a,b,c,d,e,f)    """    # src: str    dataset: DatasetReader = None    parent_img_name: str = None    temp_dir: str = None    def __init__(self, src: Union[str, DatasetReader], prj_path: str = None):        self.set_dataset(src)        if prj_path:            self.add_crs_from_prj(prj_path)        self.resampling_method = [Resampling.nearest, Resampling.bilinear, Resampling.cubic, Resampling.lanczos, Resampling.average, Resampling.cubic_spline]        # self.temp_dir = os.path.join('temp', 'rio_raster')        # if not os.path.exists(self.temp_dir):        #     os.makedirs(self.temp_dir)    def set_temp_folder(self, temp_dir: str):        self.temp_dir = temp_dir    def plot_data(self, band_nu: int = -1):        # plt.imshow(data)        # plt.colorbar()        # plt.title('Overview - Band 4 {}'.format(thumbnail.shape))        # plt.xlabel('Column #')        # plt.ylabel('Row #')        if band_nu == -1:            show(self.dataset)        else:            show(self.dataset.read(1), transform=self.get_geo_transform())        pass    def set_dataset(self, src: Union[str, DatasetReader]):        if isinstance(src, DatasetReader):            self.dataset = src        elif isinstance(src, str):            if "s3://" in src:                print("S3 not available")                # self.dataset = S3Utils().get_rio_dataset(src)            elif "/vsimem/" in src:                with MemoryFile(src) as memfile:                    self.dataset = memfile.open()            else:                if os.path.exists(src):                    self.dataset = rasterio.open(src, mode='r+')                else:                    raise Exception(f"Raste File not available at {src}")    def get_dataset(self) -> DatasetReader:        return self.dataset    def get_meta(self):        return self.dataset.meta    def get_metadata_copy(self):        return self.dataset.meta.copy()    def update_metadata(self, metadata):        memfile = MemoryFile()        dst = memfile.open(**metadata)        d = self.dataset.read()        dst.write(d)        dst.close()        self.dataset = memfile.open()  # Reopen as DatasetReader    def get_dtype(self):        return self.dataset.meta['dtype']    def get_nodata_value(self):        return self.dataset.meta['nodata']    def get_overviews(self, num):        oviews = self.dataset.overviews(1)  # list of overviews from biggest to smallest        return oviews    def get_profile(self):        return self.dataset.profile    def get_file_name(self) -> (str, str):        if self.dataset.files and len(self.dataset.files) > 0:            # file_name = str(self.dataset.files[0])            # dir_name = os.path.dirname(file_name)            # base_name = os.path.basename(file_name)            # return dir_name, base_name            return str(self.dataset.files[0])    @classmethod    def separate_file_path_name(cls, file_path_name: str):        file_dir = os.path.dirname(file_path_name)        file_name = os.path.basename(file_path_name)        return file_dir, file_name    @classmethod    def get_file_name_extension(cls, file_name: str) -> (str, str):        split = file_name.split(".")        if len(split) == 2:            return split[0], split[1]        return file_name, None    def get_file_extension(self):        try:            dir, name = self.separate_file_path_name(self.get_file_name())            name, ext = self.get_file_name_extension(name)            return ext        except Exception as e:            traceback.print_exc()    def get_bounds(self) -> BoundingBox:        return self.dataset.bounds    # def reproject_extent(self, srid, extent=None):    #     if extent is None:    #         extent = self.get_raster_extent()    #     min_x, min_y, max_x, max_y = extent    #     inProj = pyproj.Proj(init='epsg:%d' % self.get_raster_srid())    #     outProj = pyproj.Proj(init='epsg:%d' % srid)    #     transformer = Transformer.from_proj(inProj, outProj)    #     min_x, max_y = transformer.transform(min_x, max_y)    #     max_x, min_y = transformer.transform(max_x, min_y)    #     return min_x, min_y, max_x, max_y    def get_extent_after_skip_rows_cols(self, n_rows_skip, n_cols_skip):        # Remove a part of image and coincident with input rio ds        y_size, x_size = self.get_img_resolution()        # transformation from the from to the to        geo_t = self.get_geo_transform()        min_x = geo_t[2] + n_cols_skip * geo_t[0]        max_y = geo_t[5] + n_rows_skip * geo_t[4]        max_x = geo_t[2] + geo_t[0] * (x_size - n_cols_skip)        min_y = geo_t[5] + geo_t[4] * (y_size - n_rows_skip)        extent = (min_x, min_y, max_x, max_y)        return extent    def get_envelop(self, n_rows_skp=0, n_cols_skip=0, srid=0) -> gpd.GeoDataFrame:        if n_rows_skp != 0 or n_cols_skip != 0:            extent = self.get_extent_after_skip_rows_cols(n_rows_skp, n_cols_skip)        else:            extent = self.get_raster_extent()        envelop = GPDVector.extent_2_envelop(*extent, crs=self.get_crs())        if srid != 0:            envelop.to_crs(epsg=srid)        return envelop.gdf    def get_raster_extent(self) -> list:        bounds = self.dataset.bounds        return [bounds.left, bounds.bottom, bounds.right, bounds.top]    # def get_raster_extent_in_4326(self) -> list:    #     bounds = self.dataset.bounds    #     point_lb = Point(bounds.left, bounds.bottom)    #     point_rt = Point(bounds.right, bounds.top)    #     point_lb = self.transform_geometry(point_lb)    #     point_rt = self.transform_geometry(point_rt)    #     return [point_lb.x, point_lb.y, point_rt.x, point_rt.y]    def get_raster_srid(self) -> int:        try:            # epsg_code = int(self.dataset.crs.data['init'][5:])            profile = self.get_profile()            wkt = str(profile['crs'])            if ':' in wkt:                return int(str(profile['crs']).split(":")[-1])            else:                crs = pyproj.CRS.from_wkt(wkt)                return crs.to_epsg()        except Exception as e:            traceback.print_exc()            return 0    def set_crs(self, crs: pyproj.CRS):        crs = rasterio.crs.CRS.from_wkt(crs.to_wkt())        self.dataset.crs = crs    def get_width(self):        return self.dataset.width    def get_height(self):        return self.dataset.height    def get_crs(self):        return self.dataset.crs    def get_pyproj_crs(self) -> pyproj.CRS:        try:            # profile = self.get_profile()            # epsg_code = str(profile['crs'])            return pyproj.CRS.from_wkt(self.dataset.crs.to_wkt())        except Exception as e:            traceback.print_exc()            return pyproj.CRS.from_epsg(0)    # def transform_geometry(self, geometry, to_srid=4326):    #     from_crs = self.get_pyproj_crs()    #     if from_crs and from_crs.to_epsg() != to_srid:    #         to_crs = pyproj.CRS(f'EPSG:{to_srid}')    #         project = pyproj.Transformer.from_crs(from_crs, to_crs, always_xy=True).transform    #         return transform(project, geometry)    #     return geometry    def get_data_shape(self):        data = self.get_data_array()        if len(data.shape) == 2:            band = 1            row, column = data.shape        elif len(data.shape) == 3:            band, row, column = data.shape        return band, row, column    def get_data_array(self, band=None, convert_no_data_2_nan=False, envelop: gpd.GeoDataFrame = None) -> np.ndarray:        dataset = self.dataset if envelop is None else self.get_dataset_under_envelop(envelop=envelop, in_place=False)        if band:            data_arr = dataset.read(band)        else:            data_arr = dataset.read()        if convert_no_data_2_nan:            data_arr = data_arr.astype(np.float)            data_arr[data_arr == self.dataset.nodata] = np.nan        return data_arr    def save_to_file(self, img_des: str, data: np.ndarray = None, crs: CRS = None,                     affine_transform: Affine = None,                     nodata_value=None):        data = self.get_data_array() if data is None else data        crs = crs if crs else self.dataset.crs        affine_transform = affine_transform if affine_transform else self.dataset.transform        nodata_value = nodata_value if nodata_value else self.get_nodata_value()        self.write_to_file(img_des, data, crs, affine_transform, nodata_value)    @staticmethod    def write_to_file(img_des: str, data: np.ndarray, crs: CRS, affine_transform: Affine, nodata_value):        try:            FileIO.mkdirs(img_des)            ext = img_des.split(".")[-1]            if ext == "tif":                driver = 'GTiff'            dir_name = os.path.dirname(img_des)            if not os.path.exists(dir_name):                os.makedirs(dir_name)            def create_new_raster(arr: np.ndarray):                if len(arr.shape) == 2:                    bands = 1                    rows, cols = arr.shape                else:                    bands, rows, cols = arr.shape                dataset = rasterio.open(img_des, 'w',                                        driver=driver,                                        height=rows,                                        width=cols,                                        count=bands,                                        dtype=str(arr.dtype),                                        crs=crs,                                        transform=affine_transform,                                        compress='lzw',                                        nodata=nodata_value)                for i in range(bands):                    d = arr if len(arr.shape) == 2 else arr[i]                    dataset.write(d, i + 1)                dataset.close()            # if "s3://" in img_des:            #     session = rasterio.Env(AWSSession(S3Utils().get_session()))            #     with session:            #         create_new_raster(data)            #            # else:            create_new_raster(data)        except:            da_logger.error(f"fp{img_des}")            da_logger.error(traceback.print_exc())    def rio_raster_from_array(self, img_arr: np.ndarray) -> 'RioRaster':        """        :return:        """        meta_data = self.get_metadata_copy()        raster = self.raster_from_array(img_arr, crs=self.get_crs(),                                        g_transform=self.get_geo_transform(),                                        nodata_value=self.get_nodata_value())        return raster    @staticmethod    def raster_from_array(img_arr: np.ndarray, crs: Union[str, CRS],                          g_transform: Affine, nodata_value=None) -> 'RioRaster':        """        :param img_arr:        :param crs: pyproj.CRS or wkt        :param g_transform:            Affine consist of a, b, c, d, e, f format        :param nodata_value:        :return:        """        memfile = MemoryFile()        if len(img_arr.shape) == 2:            bands = 1            rows, cols = img_arr.shape        else:            bands, rows, cols = img_arr.shape        dataset = memfile.open(driver='GTiff',                               height=rows,                               width=cols,                               count=bands,                               dtype=str(img_arr.dtype),                               crs=crs,                               transform=g_transform,                               nodata=nodata_value                               )        for i in range(bands):            d = img_arr if len(img_arr.shape) == 2 else img_arr[i, :, :]            dataset.write(d, i + 1)        dataset.close()        dataset = memfile.open()  # Reopen as DatasetReader        # dir_name, file_name = self.get_file_name()        new_raster = RioRaster(dataset)        return new_raster    def add_crs_from_prj(self, prj_file):        crs = FileIO.read_prj_file(prj_file)        self.dataset.crs = CRS.from_wkt(crs.to_wkt())    def get_driver(self):        return self.get_profile().data['driver']    def get_img_resolution(self) -> tuple:        """ return rows/height and cols/width of an image"""        cols = self.get_profile().data['width']        rows = self.get_profile().data['height']        return rows, cols    def get_spatial_resoultion(self, in_meter=False) -> tuple:        """ return: spatial resolution  """        # bounds = self.get_bounds()        # s_width = bounds.right - bounds.left        # i_width = self.get_width()        # s_height = bounds.top - bounds.bottom        # i_height = self.get_height()        # return s_width / i_width, s_height / i_height        if in_meter:            temp_rio_ds = self.transform_to_metric_unit_projections()            return temp_rio_ds.res        return self.dataset.res    def get_unit(self) -> str:        """ get unit of image"""        crs = self.get_pyproj_crs()        return crs.to_dict()['units']    def get_radiometric_resolution(self):        s = self.get_profile()['dtype']        m = re.search(r'\d+$', s)        return int(m.group()) if m else None    def get_spectral_resolution(self):        return self.get_profile().data['count']    # def get_no_of_bands(self):    #     return self.dataset.count    def get_geo_transform(self) -> Affine:        """        :return: Affine consist of a, b, c, d, e, f format        """        return self.get_profile().data['transform']    def is_image_crs_same(self, raster2: 'RioRaster') -> bool:        crs1 = self.get_crs()        crs2 = raster2.get_crs()        return str(crs1) == str(crs2)    def is_image_resolution_same(self, raster2: 'RioRaster') -> bool:        res1 = self.get_img_resolution()        res2 = raster2.get_img_resolution()        return res1 == res2    def is_spatial_resolution_same(self, raster2: 'RioRaster'):        res1 = self.get_spatial_resoultion()        res2 = raster2.get_spatial_resoultion()        return res1 == res2    def is_image_extent_same(self, raster2: 'RioRaster'):        E1 = np.array(self.get_raster_extent())        E2 = np.array(raster2.get_raster_extent())        return (E1 == E2).all()    def create_ndwi_data(self, green, nir, output_path: str = None):        nir_data = self.get_data_array(nir)        green_data = self.get_data_array(green)        ndwi = IndicesCalc.NDWIndices(green_data, nir_data)        ndwi = IndicesCalc.normalize(ndwi)        if output_path:            self.save_to_file(output_path, ndwi.astype(rasterio.int8))        return ndwi    def create_ndvi_data(self, red_band: int, nir_band: int, output_path: str = None):        nir_data = self.get_data_array(nir_band)        red_data = self.get_data_array(red_band)        ndvi = IndicesCalc.NDVIndices(nir_data, red_data)        ndvi = IndicesCalc.normalize(ndvi)        if output_path:            self.save_to_file(output_path, ndvi.astype(rasterio.int8))        return ndvi        # with rasterio.open('Data_06/RASTER/NDVI/NDVI.tif', 'w', **meta_ndvi) as dst:        #     dst.write_band(1, ndvi.astype(rasterio.float32))    def vector_2_raster(self, gdv: GPDVector, value_col: str = 'id', d_type=np.uint8) -> 'RioRaster':        if str(gdv.get_crs()).lower() != str(self.get_crs()).lower():            gdv.to_crs(self.get_pyproj_crs())        shapes = gdv.get_geometry_list(value_col)        data = rasterize(shapes, out_shape=self.get_img_resolution(), transform=self.get_geo_transform())        data = data.astype(d_type)        return self.rio_raster_from_array(data)    def raster_2_vector(self, band: Union[int, np.ndarray]) -> gpd.GeoDataFrame:        geoms = []        file_path, file_name = self.get_file_name()        if isinstance(band, np.ndarray):            band_data = band        else:            band_data = self.get_data_array(band)        c_ids = []        for vec in shapes(band_data, transform=self.get_geo_transform()):            geoms.append(shape(vec[0]))            c_ids.append(vec[1])        # ids = np.arange(len(geoms))        gdf = gpd.GeoDataFrame({'geometry': geoms,                                'class_id': np.array(c_ids).astype('uint16'),                                'grid': file_name.split('.')[0]                                })        gdf.crs = self.get_pyproj_crs()        return gdf    def get_tiles(self, width=64, height=64) -> 'RioRaster':        rows, cols = self.get_img_resolution()        offsets = product(range(0, cols, width), range(0, rows, height))        big_window = windows.Window(col_off=0, row_off=0, width=cols, height=rows)        for col_off, row_off in offsets:            window = windows.Window(col_off=col_off, row_off=row_off,                                    width=width, height=height).intersection(big_window)            transform = windows.transform(window, self.get_geo_transform())            tile = self.dataset.read(window=window)            tile_raster = self.raster_from_array(tile, crs=self.get_crs(), g_transform=transform,                                                 nodata_value=self.get_nodata_value())            # print(f"working on tile of {self.get_file_name()[1]} at {window}")            yield tile_raster, col_off, row_off    def get_all_tiles(self):        tiles = []        tile_no = 0        tile_raster: RioRaster        if self.temp_dir:            for tile_raster in self.get_titles(width=500, height=500):                tile_no += 1                file_name = self.get_file_name()[1].split('.')[0]                tile_name = f"{self.temp_dir}/tiles/{file_name}_{tile_no}.tif"                tile_raster.save_to_file(tile_name)                tiles.append(tile_name)            return tiles        else:            da_logger.critical("Please set temp folder path first using set_temp_folder")    @staticmethod    def reverse_band_row_col(data: np.ndarray):        return np.moveaxis(data, 0, 2)    def save_temp_file(self, postfix: str):        if self.temp_dir:            img_name = self.get_file_name().split('.')[-2]            img_des = os.path.join(self.temp_dir, f"{img_name}_{postfix}.tif")            print(img_des)            self.save_to_file(img_des)        else:            da_logger.critical("Please set temp folder path first using set_temp_folder")    def resample_raster_res(self, des_resolution: float, resampling_method_index=3, in_place=True):        self_res = self.get_spatial_resoultion()        width = round(self.get_width() * self_res[0] / des_resolution, 0)        height = round(self.get_height() * self_res[1] / des_resolution, 0)        return self.resample_raster(width, height, resampling_method_index, in_place)    def resample_raster(self, width, height, resampling_method_index=3, in_place=True) -> DatasetReader:        # resampling_method = [Resampling.nearest, Resampling.bilinear, Resampling.cubic, Resampling.lanczos, Resampling.average]        bands = self.dataset.count        data = self.dataset.read(            out_shape=(                bands,                int(height),                int(width)            ),            resampling=self.resampling_method[resampling_method_index]        )        geo_transform = self.dataset.transform * self.dataset.transform.scale(            (self.dataset.width / data.shape[-1]),            (self.dataset.height / data.shape[-2])        )        kwargs = self.dataset.meta.copy()        kwargs.update({            'transform': geo_transform,            'width': data.shape[-1],            'height': data.shape[-2]        })        memfile = MemoryFile()        dst = memfile.open(**kwargs)        for i in range(bands):            d = data if len(data.shape) == 2 else data[i, :, :]            dst.write(d, i + 1)        dst.close()        if in_place:            self.dataset = memfile.open()        else:            return memfile.open()  # Reopen as DatasetReader    def reproject_raster(self, des_crs: pyproj.CRS = None, width=None, height=None, in_place=True, resampling_method_index=3):        dst_crs = rasterio.crs.CRS.from_wkt(des_crs.to_wkt())        dst_crs = self.get_crs() if dst_crs is None else dst_crs        width = self.get_width() if width is None else width        height = self.get_height() if height is None else height        g_trans, width, height = calculate_default_transform(self.get_crs(), dst_crs, width,                                                             height, *self.get_raster_extent())        kwargs = self.get_metadata_copy()        kwargs.update({            'crs': dst_crs,            'transform': g_trans,            'width': width,            'height': height        })        memfile = MemoryFile()        dst = memfile.open(**kwargs)        for i in range(1, self.dataset.count + 1):            reproject(                source=rasterio.band(self.dataset, i),                destination=rasterio.band(dst, i),                src_transform=self.get_geo_transform(),                src_crs=self.get_crs(),                dst_transform=transform,                dst_crs=dst_crs,                resampling=self.resampling_method[resampling_method_index])        dst.close()        if in_place:            self.dataset = memfile.open()        else:            return memfile.open()    def clip_raster(self, aoi: gpd.GeoDataFrame, in_place=True):        """        clip raster based on aoi        :param aoi: shapely polygon geometry        :param in_place: boolean        :return: RioRaster        """        if str(aoi.crs).lower() != str(self.get_crs()).lower():            geo = aoi.to_crs(self.get_crs())        else:            geo = aoi        def getFeatures(gdf):            """Function to parse features from GeoDataFrame in such a manner that rasterio wants them"""            import json            return [json.loads(gdf.to_json())['features'][0]['geometry']]        coords = getFeatures(geo)        nodata = self.get_nodata_value() if self.get_nodata_value() else 0        out_img, out_transform = mask(dataset=self.dataset, shapes=coords, crop=True, nodata=nodata)        out_meta = self.dataset.meta.copy()        out_meta.update({"driver": "GTiff",                         "height": out_img.shape[1],                         "width": out_img.shape[2],                         "transform": out_transform,                         # "nodata": nodata,                         "crs": self.dataset.crs})        if in_place:            self.dataset = self.rio_dataset_from_array(out_img, out_meta)        else:            return self.rio_dataset_from_array(out_img, out_meta)    def pad_raster(self, des_raster):        """        clip or pad raster to mak align with bounds        :param des_raster:        :return:        """        # bounds = self.get_spectral_resolution()        # ulx = gt[0] - gt[1] * npad        # uly = gt[3] - gt[5] * npad        aff: Affine = self.get_geo_transform()        des_bounds = des_raster.get_bounds()        rows, cols = rasterio.transform.rowcol(aff, xs=[des_bounds[0], des_bounds[2]], ys=[des_bounds[3], des_bounds[1]])        height = rows[1] - rows[0]        width = cols[1] - cols[0]        window = windows.Window(col_off=cols[0], row_off=rows[0],                                width=width, height=height)  # .intersection(big_window)        window_transform = windows.transform(window, self.get_geo_transform())        kwargs = self.dataset.meta.copy()        kwargs.update({            'crs': self.get_crs(),            'transform': window_transform,            'width': width,            'height': height        })        memfile = MemoryFile()        dst = memfile.open(**kwargs)        # for i in range(bands):        #     # tile = self.dataset.read()        data = self.dataset.read(window=window, boundless=False, fill_value=self.dataset.nodata)        dst.write(data)        dst.close()        self.dataset = memfile.open()    def get_dataset_under_envelop(self, envelop: Union[Polygon, gpd.GeoDataFrame], in_place=True) -> DatasetReader:        if isinstance(envelop, Polygon):            des_bounds = envelop.bounds        else:            if str(self.get_crs()).lower() != str(envelop.crs).lower():                envelop.to_crs(self.get_crs())            des_bounds = tuple(envelop.bounds.values[0])        aff = self.get_geo_transform()        rows, cols = rasterio.transform.rowcol(aff, xs=[des_bounds[0], des_bounds[2]], ys=[des_bounds[3], des_bounds[1]])        height = abs(rows[0] - rows[1])        width = abs(cols[0] - cols[1])        window = windows.Window(col_off=cols[0], row_off=rows[0], width=width, height=height)  # .intersection(big_window)        window_transform = windows.transform(window, self.get_geo_transform())        data = self.dataset.read(window=window, boundless=True, fill_value=self.dataset.nodata)        kwargs = self.dataset.meta.copy()        kwargs.update({            'transform': window_transform,            'width': width,            'height': height        })        dataset = self.rio_dataset_from_array(data, kwargs)        if in_place:            self.dataset = dataset        else:            return dataset    def reclassify_raster(self, thresholds, band=1, nodata=0):        """        :param thresholds:            example:  {                    "water": (('lt', 0.015), 4),                    "built-up": ((0.015, 0.02), 1),                    "barren": ((0.07, 0.27), 2),                    "vegetation": (('gt', 0.27), 3)                }        :param band:            band no        :return:        """        img_arr = self.get_data_array(band)        res = np.empty(img_arr.shape)        res[:] = nodata        for key in thresholds:            if thresholds[key][0][0] == 'lt':                res = np.where(img_arr <= thresholds[key][0][1], thresholds[key][1], res)            elif thresholds[key][0][0] == 'gt':                res = np.where(img_arr >= thresholds[key][0][1], thresholds[key][1], res)            else:                con = np.logical_and(img_arr >= thresholds[key][0][0], img_arr <= thresholds[key][0][1])                res = np.where(con, thresholds[key][1], res)        return res.astype(np.uint8)    def make_coincident_with(self, des_raster: 'RioRaster', resampling_method_index=3):        if not self.is_image_crs_same(des_raster):            self.reproject_raster(des_raster.get_crs(), resampling_method_index=resampling_method_index)        des_bbox = des_raster.get_envelop()        src_bbox = self.get_envelop()        # envelop = des_bbox.intersection(src_bbox)        # crs = self.get_crs()        # envelop = gpd.GeoDataFrame({'geometry': envelop}, index=[0], crs=crs)        if not des_bbox.equals(src_bbox):            self.get_dataset_under_envelop(des_bbox)        if not self.is_image_resolution_same(des_raster):            width = des_raster.get_width()            height = des_raster.get_height()            self.resample_raster(width, height, resampling_method_index=resampling_method_index)    @classmethod    def rio_dataset_from_array(cls, data: np.ndarray, meta) -> DatasetReader:        bands = 1 if len(data.shape) == 2 else data.shape[0]        memfile = MemoryFile()        dst = memfile.open(**meta)        for i in range(bands):            d = data if len(data.shape) == 2 else data[i, :, :]            dst.write(d, i + 1)        dst.close()        dataset = memfile.open()  # Reopen as DatasetReader        return dataset    def change_datatype(self, new_dtype: np.dtype = "float32"):        data = self.get_data_array()        # band, *_ = data.shape        # for b in range(band):        #     data[b] = data[b].astype(new_dtype)        out_meta = self.dataset.meta.copy()        out_meta.update({"nodata": self.get_nodata_value(),                         "dtype": new_dtype})        self.dataset = self.rio_dataset_from_array(data, out_meta)    def add_nodata_value(self, val):        out_meta = self.dataset.meta.copy()        out_meta.update({"nodata": val})        data = self.get_data_array()        self.dataset = self.rio_dataset_from_array(data, out_meta)    def get_x_y_value_raster(self, in_lat_long=False) -> (np.ndarray, np.ndarray):        """        This function retrieves information about the X and Y raster        :return: lat and lon raster        """        rows, cols = self.get_img_resolution()        if in_lat_long and self.get_raster_srid() != 4326:            geo_t, width, height = calculate_default_transform(self.get_crs(), CRS.from_epsg(4326),                                                               self.get_width(), self.get_height(),                                                               *self.get_raster_extent())        else:            geo_t = self.get_geo_transform()        X = np.zeros((rows, cols))        Y = np.zeros((rows, cols))        # tim way of doing it        # for col in np.arange(cols):        #     # lon[:, col] = geo_t[0] + col * geo_t[1] + geo_t[1] / 2        #     lon[:, col] = geo_t[2] + col * geo_t[0] + geo_t[0] / 2        #     # ULx + col*(E-W pixel spacing) + E-W pixel spacing        # for row in np.arange(rows):        #     # lat[row, :] = geo_t[3] + row * geo_t[5] + geo_t[5] / 2        #     lat[row, :] = geo_t[5] + row * geo_t[4] + geo_t[4] / 2        # return lat, lon        for i in np.arange(cols):            for j in np.arange(i, rows):                Y[j, :] = i * geo_t[3] + j * geo_t[4] + geo_t[5]                break            X[:, i] = i * geo_t[0] + j * geo_t[1] + geo_t[2]        return X, Y    def calculate_spatial_resolution_in_meter(self):        """        This functions calculated the distance between each pixel in meter.        Returns        -------        dlat: array            Array containing the vertical distance between each pixel in meters        dlon: array            Array containing the horizontal distance between each pixel in meters        """        geo_out = self.get_geo_transform()        size_Y, size_X = self.get_img_resolution()        # Create the lat/lon rasters        # lon = np.arange(size_X + 1) * geo_out[1] + geo_out[0] - 0.5 * geo_out[1]        # lat = np.arange(size_Y + 1) * geo_out[5] + geo_out[3] - 0.5 * geo_out[5]        lon = np.arange(size_X + 1) * geo_out[0] + geo_out[2] - 0.5 * geo_out[0]        lat = np.arange(size_Y + 1) * geo_out[4] + geo_out[5] - 0.5 * geo_out[4]        dlat_2d = np.array([lat, ] * int(np.size(lon, 0))).transpose()        dlon_2d = np.array([lon, ] * int(np.size(lat, 0)))        # Radius of the earth in meters        R_earth = 6371000        # Calculate the lat and lon in radians        lonRad = dlon_2d * np.pi / 180        latRad = dlat_2d * np.pi / 180        # Calculate the difference in lat and lon        lonRad_dif = abs(lonRad[:, 1:] - lonRad[:, :-1])        latRad_dif = abs(latRad[:-1] - latRad[1:])        # Calculate the distance between the upper and lower pixel edge        a = np.sin(latRad_dif[:, :-1] / 2) * np.sin(latRad_dif[:, :-1] / 2)        clat = 2 * np.arctan2(np.sqrt(a), np.sqrt(1 - a))        dlat = R_earth * clat        # Calculate the distance between the eastern and western pixel edge        b = np.cos(latRad[1:, :-1]) * np.cos(latRad[:-1, :-1]) * np.sin(lonRad_dif[:-1, :] / 2) * np.sin(lonRad_dif[:-1, :] / 2)        clon = 2 * np.arctan2(np.sqrt(b), np.sqrt(1 - b));        dlon = R_earth * clon        return dlon, dlat    def transform_to_metric_unit_projections(self, in_place=False):        if self.get_pyproj_crs().to_epsg() == 4326:            gt = self.get_geo_transform()            utm_srid = TransformationOperations.coord_to_utm_srid(gt[2], gt[5])            temp_rio_ds = self.reproject_raster(CRS.from_epsg(utm_srid), in_place=False)        else:            temp_rio_ds = self.get_dataset()        if in_place:            self.dataset = temp_rio_ds        else:            return temp_rio_ds    def get_pixel_area_band(self):        temp_rio_ds = self.transform_to_metric_unit_projections()        cols = temp_rio_ds.profile.data['width']        rows = temp_rio_ds.profile.data['height']        geo = temp_rio_ds.profile.data['transform']        # geo 0 and 4 index are scaling factor of x and y respectively        return np.ones((rows,cols)) * geo[0] * geo[4]
+import osimport reimport tracebackfrom itertools import productimport geopandas as gpdfrom typing import Unionimport numpy as npimport pyprojimport rasteriofrom affine import Affinefrom boto3 import Sessionfrom rasterio import DatasetReader, MemoryFile, windowsfrom rasterio.coords import BoundingBoxfrom rasterio.crs import CRSfrom rasterio.enums import Resamplingfrom rasterio.features import shapes, rasterizefrom rasterio.mask import maskfrom rasterio.plot import showfrom rasterio.session import AWSSessionfrom rasterio.warp import calculate_default_transform, reprojectfrom shapely.geometry import Point, shape, Polygonfrom shapely.ops import transformfrom digitalarztools.operations.transformation import TransformationOperationsfrom digitalarztools.io.file_io import FileIOfrom digitalarztools.raster.indices import IndicesCalcfrom digitalarztools.utils.logger import da_loggerfrom digitalarztools.vector.gpd_vector import GPDVectorclass RioRaster:    """        Geo Raster contain informaiton about geotransform and projection        GDAL geotransform = (c,a,b, f,d,e)        RasterIO = (a,b,c,d,e,f)    """    # src: str    dataset: DatasetReader = None    parent_img_name: str = None    temp_dir: str = None    def __init__(self, src: Union[str, DatasetReader], prj_path: str = None, s3_session=None):        self.set_dataset(src, s3_session)        if not prj_path:            prj_path = f"{src[:-3]}.prj"        if not "s3://" in prj_path and os.path.exists(prj_path):            self.add_crs_from_prj(prj_path)        self.resampling_method = [Resampling.nearest, Resampling.bilinear, Resampling.cubic, Resampling.lanczos, Resampling.average, Resampling.cubic_spline]    def set_temp_folder(self, temp_dir: str):        self.temp_dir = temp_dir    def plot_data(self, band_nu: int = -1):        # plt.imshow(data)        # plt.colorbar()        # plt.title('Overview - Band 4 {}'.format(thumbnail.shape))        # plt.xlabel('Column #')        # plt.ylabel('Row #')        if band_nu == -1:            show(self.dataset)        else:            show(self.dataset.read(1), transform=self.get_geo_transform())        pass    def set_dataset(self, src: Union[str, DatasetReader], s3_session=None):        if isinstance(src, DatasetReader):            self.dataset = src        elif isinstance(src, str):            if "s3://" in src:                # print("S3 not available")                # self.dataset = S3Utils().get_rio_dataset(src)                session = rasterio.Env(AWSSession(s3_session))                with session:                    self.dataset = rasterio.open(src)            elif "/vsimem/" in src:                with MemoryFile(src) as memfile:                    self.dataset = memfile.open()            else:                if os.path.exists(src):                    self.dataset = rasterio.open(src, mode='r+')                else:                    raise Exception(f"Raste File not available at {src}")    def get_dataset(self) -> DatasetReader:        return self.dataset    def get_meta(self):        return self.dataset.meta    def get_metadata_copy(self):        return self.dataset.meta.copy()    def update_metadata(self, metadata):        memfile = MemoryFile()        dst = memfile.open(**metadata)        d = self.dataset.read()        dst.write(d)        dst.close()        self.dataset = memfile.open()  # Reopen as DatasetReader    def get_dtype(self):        return self.dataset.meta['dtype']    def get_nodata_value(self):        return self.dataset.meta['nodata']    def get_overviews(self, num):        oviews = self.dataset.overviews(1)  # list of overviews from biggest to smallest        return oviews    def get_profile(self):        return self.dataset.profile    def get_file_name(self) -> (str, str):        if self.dataset.files and len(self.dataset.files) > 0:            # file_name = str(self.dataset.files[0])            # dir_name = os.path.dirname(file_name)            # base_name = os.path.basename(file_name)            # return dir_name, base_name            return str(self.dataset.files[0])    @classmethod    def separate_file_path_name(cls, file_path_name: str):        file_dir = os.path.dirname(file_path_name)        file_name = os.path.basename(file_path_name)        return file_dir, file_name    @classmethod    def get_file_name_extension(cls, file_name: str) -> (str, str):        split = file_name.split(".")        if len(split) == 2:            return split[0], split[1]        return file_name, None    def get_file_extension(self):        try:            dir, name = self.separate_file_path_name(self.get_file_name())            name, ext = self.get_file_name_extension(name)            return ext        except Exception as e:            traceback.print_exc()    def get_bounds(self) -> BoundingBox:        return self.dataset.bounds    # def reproject_extent(self, srid, extent=None):    #     if extent is None:    #         extent = self.get_raster_extent()    #     min_x, min_y, max_x, max_y = extent    #     inProj = pyproj.Proj(init='epsg:%d' % self.get_raster_srid())    #     outProj = pyproj.Proj(init='epsg:%d' % srid)    #     transformer = Transformer.from_proj(inProj, outProj)    #     min_x, max_y = transformer.transform(min_x, max_y)    #     max_x, min_y = transformer.transform(max_x, min_y)    #     return min_x, min_y, max_x, max_y    def get_extent_after_skip_rows_cols(self, n_rows_skip, n_cols_skip):        # Remove a part of image and coincident with input rio ds        y_size, x_size = self.get_img_resolution()        # transformation from the from to the to        geo_t = self.get_geo_transform()        min_x = geo_t[2] + n_cols_skip * geo_t[0]        max_y = geo_t[5] + n_rows_skip * geo_t[4]        max_x = geo_t[2] + geo_t[0] * (x_size - n_cols_skip)        min_y = geo_t[5] + geo_t[4] * (y_size - n_rows_skip)        extent = (min_x, min_y, max_x, max_y)        return extent    def get_envelop(self, n_rows_skp=0, n_cols_skip=0, srid=0) -> gpd.GeoDataFrame:        if n_rows_skp != 0 or n_cols_skip != 0:            extent = self.get_extent_after_skip_rows_cols(n_rows_skp, n_cols_skip)        else:            extent = self.get_raster_extent()        envelop = GPDVector.extent_2_envelop(*extent, crs=self.get_crs())        if srid != 0:            envelop.to_crs(epsg=srid)        return envelop.gdf    def get_raster_extent(self) -> list:        bounds = self.dataset.bounds        return [bounds.left, bounds.bottom, bounds.right, bounds.top]    # def get_raster_extent_in_4326(self) -> list:    #     bounds = self.dataset.bounds    #     point_lb = Point(bounds.left, bounds.bottom)    #     point_rt = Point(bounds.right, bounds.top)    #     point_lb = self.transform_geometry(point_lb)    #     point_rt = self.transform_geometry(point_rt)    #     return [point_lb.x, point_lb.y, point_rt.x, point_rt.y]    def get_raster_srid(self) -> int:        try:            # epsg_code = int(self.dataset.crs.data['init'][5:])            profile = self.get_profile()            wkt = str(profile['crs'])            if ':' in wkt:                return int(str(profile['crs']).split(":")[-1])            else:                crs = pyproj.CRS.from_wkt(wkt)                return crs.to_epsg()        except Exception as e:            traceback.print_exc()            return 0    def set_crs(self, crs: pyproj.CRS):        crs = rasterio.crs.CRS.from_wkt(crs.to_wkt())        self.dataset.crs = crs    def get_width(self):        return self.dataset.width    def get_height(self):        return self.dataset.height    def get_crs(self):        return self.dataset.crs    def get_pyproj_crs(self) -> pyproj.CRS:        try:            # profile = self.get_profile()            # epsg_code = str(profile['crs'])            return pyproj.CRS.from_wkt(self.dataset.crs.to_wkt())        except Exception as e:            traceback.print_exc()            return pyproj.CRS.from_epsg(0)    # def transform_geometry(self, geometry, to_srid=4326):    #     from_crs = self.get_pyproj_crs()    #     if from_crs and from_crs.to_epsg() != to_srid:    #         to_crs = pyproj.CRS(f'EPSG:{to_srid}')    #         project = pyproj.Transformer.from_crs(from_crs, to_crs, always_xy=True).transform    #         return transform(project, geometry)    #     return geometry    def get_data_shape(self):        data = self.get_data_array()        if len(data.shape) == 2:            band = 1            row, column = data.shape        elif len(data.shape) == 3:            band, row, column = data.shape        return band, row, column    def get_data_array(self, band=None, convert_no_data_2_nan=False, envelop: gpd.GeoDataFrame = None) -> np.ndarray:        dataset = self.dataset if envelop is None else self.get_dataset_under_envelop(envelop=envelop, in_place=False)        if band:            data_arr = dataset.read(band)        else:            data_arr = dataset.read()        if convert_no_data_2_nan:            data_arr = data_arr.astype(np.float)            data_arr[data_arr == self.dataset.nodata] = np.nan        return data_arr    def save_to_file(self, img_des: str, data: np.ndarray = None, crs: CRS = None,                     affine_transform: Affine = None,                     nodata_value=None):        data = self.get_data_array() if data is None else data        crs = crs if crs else self.dataset.crs        affine_transform = affine_transform if affine_transform else self.dataset.transform        nodata_value = nodata_value if nodata_value else self.get_nodata_value()        self.write_to_file(img_des, data, crs, affine_transform, nodata_value)    @staticmethod    def write_to_file(img_des: str, data: np.ndarray, crs: CRS, affine_transform: Affine, nodata_value, session: Session = None):        try:            if not "s3://" in img_des:                FileIO.mkdirs(img_des)            ext = img_des.split(".")[-1]            if ext == "tif":                driver = 'GTiff'            dir_name = os.path.dirname(img_des)            if not os.path.exists(dir_name):                os.makedirs(dir_name)            def create_new_raster(arr: np.ndarray):                if len(arr.shape) == 2:                    bands = 1                    rows, cols = arr.shape                else:                    bands, rows, cols = arr.shape                dataset = rasterio.open(img_des, 'w',                                        driver=driver,                                        height=rows,                                        width=cols,                                        count=bands,                                        dtype=str(arr.dtype),                                        crs=crs,                                        transform=affine_transform,                                        compress='lzw',                                        nodata=nodata_value)                for i in range(bands):                    d = arr if len(arr.shape) == 2 else arr[i]                    dataset.write(d, i + 1)                dataset.close()            if "s3://" in img_des:                session = rasterio.Env(AWSSession(session))                with session:                    create_new_raster(data)            else:                create_new_raster(data)        except:            da_logger.error(f"fp{img_des}")            da_logger.error(traceback.print_exc())    def rio_raster_from_array(self, img_arr: np.ndarray) -> 'RioRaster':        """        :return:        """        meta_data = self.get_metadata_copy()        raster = self.raster_from_array(img_arr, crs=self.get_crs(),                                        g_transform=self.get_geo_transform(),                                        nodata_value=self.get_nodata_value())        return raster    @staticmethod    def raster_from_array(img_arr: np.ndarray, crs: Union[str, CRS],                          g_transform: Affine, nodata_value=None) -> 'RioRaster':        """        :param img_arr:        :param crs: pyproj.CRS or wkt        :param g_transform:            Affine consist of a, b, c, d, e, f format        :param nodata_value:        :return:        """        memfile = MemoryFile()        if len(img_arr.shape) == 2:            bands = 1            rows, cols = img_arr.shape        else:            bands, rows, cols = img_arr.shape        dataset = memfile.open(driver='GTiff',                               height=rows,                               width=cols,                               count=bands,                               dtype=str(img_arr.dtype),                               crs=crs,                               transform=g_transform,                               nodata=nodata_value                               )        for i in range(bands):            d = img_arr if len(img_arr.shape) == 2 else img_arr[i, :, :]            dataset.write(d, i + 1)        dataset.close()        dataset = memfile.open()  # Reopen as DatasetReader        # dir_name, file_name = self.get_file_name()        new_raster = RioRaster(dataset)        return new_raster    def add_crs_from_prj(self, prj_file):        crs = FileIO.read_prj_file(prj_file)        self.dataset.crs = CRS.from_wkt(crs.to_wkt())    def get_driver(self):        return self.get_profile().data['driver']    def get_img_resolution(self) -> tuple:        """ return rows/height and cols/width of an image"""        cols = self.get_profile().data['width']        rows = self.get_profile().data['height']        return rows, cols    def get_spatial_resoultion(self, in_meter=False) -> tuple:        """ return: spatial resolution  """        # bounds = self.get_bounds()        # s_width = bounds.right - bounds.left        # i_width = self.get_width()        # s_height = bounds.top - bounds.bottom        # i_height = self.get_height()        # return s_width / i_width, s_height / i_height        if in_meter:            temp_rio_ds = self.transform_to_metric_unit_projections()            return temp_rio_ds.res        return self.dataset.res    def get_unit(self) -> str:        """ get unit of image"""        crs = self.get_pyproj_crs()        return crs.to_dict()['units']    def get_radiometric_resolution(self):        s = self.get_profile()['dtype']        m = re.search(r'\d+$', s)        return int(m.group()) if m else None    def get_spectral_resolution(self):        return self.get_profile().data['count']    # def get_no_of_bands(self):    #     return self.dataset.count    def get_geo_transform(self) -> Affine:        """        :return: Affine consist of a, b, c, d, e, f format        """        return self.get_profile().data['transform']    def is_image_crs_same(self, raster2: 'RioRaster') -> bool:        crs1 = self.get_crs()        crs2 = raster2.get_crs()        return str(crs1) == str(crs2)    def is_image_resolution_same(self, raster2: 'RioRaster') -> bool:        res1 = self.get_img_resolution()        res2 = raster2.get_img_resolution()        return res1 == res2    def is_spatial_resolution_same(self, raster2: 'RioRaster'):        res1 = self.get_spatial_resoultion()        res2 = raster2.get_spatial_resoultion()        return res1 == res2    def is_image_extent_same(self, raster2: 'RioRaster'):        E1 = np.array(self.get_raster_extent())        E2 = np.array(raster2.get_raster_extent())        return (E1 == E2).all()    def create_ndwi_data(self, green, nir, output_path: str = None):        nir_data = self.get_data_array(nir)        green_data = self.get_data_array(green)        ndwi = IndicesCalc.NDWIndices(green_data, nir_data)        ndwi = IndicesCalc.normalize(ndwi)        if output_path:            self.save_to_file(output_path, ndwi.astype(rasterio.int8))        return ndwi    def create_ndvi_data(self, red_band: int, nir_band: int, output_path: str = None):        nir_data = self.get_data_array(nir_band)        red_data = self.get_data_array(red_band)        ndvi = IndicesCalc.NDVIndices(nir_data, red_data)        ndvi = IndicesCalc.normalize(ndvi)        if output_path:            self.save_to_file(output_path, ndvi.astype(rasterio.int8))        return ndvi        # with rasterio.open('Data_06/RASTER/NDVI/NDVI.tif', 'w', **meta_ndvi) as dst:        #     dst.write_band(1, ndvi.astype(rasterio.float32))    def vector_2_raster(self, gdv: GPDVector, value_col: str = 'id', d_type=np.uint8) -> 'RioRaster':        if str(gdv.get_crs()).lower() != str(self.get_crs()).lower():            gdv.to_crs(self.get_pyproj_crs())        shapes = gdv.get_geometry_list(value_col)        data = rasterize(shapes, out_shape=self.get_img_resolution(), transform=self.get_geo_transform())        data = data.astype(d_type)        return self.rio_raster_from_array(data)    def raster_2_vector(self, band: Union[int, np.ndarray]) -> gpd.GeoDataFrame:        geoms = []        file_path, file_name = self.get_file_name()        if isinstance(band, np.ndarray):            band_data = band        else:            band_data = self.get_data_array(band)        c_ids = []        for vec in shapes(band_data, transform=self.get_geo_transform()):            geoms.append(shape(vec[0]))            c_ids.append(vec[1])        # ids = np.arange(len(geoms))        gdf = gpd.GeoDataFrame({'geometry': geoms,                                'class_id': np.array(c_ids).astype('uint16'),                                'grid': file_name.split('.')[0]                                })        gdf.crs = self.get_pyproj_crs()        return gdf    def get_tiles(self, width=64, height=64) -> 'RioRaster':        rows, cols = self.get_img_resolution()        offsets = product(range(0, cols, width), range(0, rows, height))        big_window = windows.Window(col_off=0, row_off=0, width=cols, height=rows)        for col_off, row_off in offsets:            window = windows.Window(col_off=col_off, row_off=row_off,                                    width=width, height=height).intersection(big_window)            transform = windows.transform(window, self.get_geo_transform())            tile = self.dataset.read(window=window)            tile_raster = self.raster_from_array(tile, crs=self.get_crs(), g_transform=transform,                                                 nodata_value=self.get_nodata_value())            # print(f"working on tile of {self.get_file_name()[1]} at {window}")            yield tile_raster, col_off, row_off    def get_all_tiles(self):        tiles = []        tile_no = 0        tile_raster: RioRaster        if self.temp_dir:            for tile_raster in self.get_titles(width=500, height=500):                tile_no += 1                file_name = self.get_file_name()[1].split('.')[0]                tile_name = f"{self.temp_dir}/tiles/{file_name}_{tile_no}.tif"                tile_raster.save_to_file(tile_name)                tiles.append(tile_name)            return tiles        else:            da_logger.critical("Please set temp folder path first using set_temp_folder")    @staticmethod    def reverse_band_row_col(data: np.ndarray):        return np.moveaxis(data, 0, 2)    def save_temp_file(self, postfix: str):        if self.temp_dir:            img_name = self.get_file_name().split('.')[-2]            img_des = os.path.join(self.temp_dir, f"{img_name}_{postfix}.tif")            print(img_des)            self.save_to_file(img_des)        else:            da_logger.critical("Please set temp folder path first using set_temp_folder")    def resample_raster_res(self, des_resolution: float, resampling_method_index=3, in_place=True):        self_res = self.get_spatial_resoultion()        width = round(self.get_width() * self_res[0] / des_resolution, 0)        height = round(self.get_height() * self_res[1] / des_resolution, 0)        return self.resample_raster(width, height, resampling_method_index, in_place)    def resample_raster(self, width, height, resampling_method_index=3, in_place=True) -> DatasetReader:        # resampling_method = [Resampling.nearest, Resampling.bilinear, Resampling.cubic, Resampling.lanczos, Resampling.average]        bands = self.dataset.count        data = self.dataset.read(            out_shape=(                bands,                int(height),                int(width)            ),            resampling=self.resampling_method[resampling_method_index]        )        geo_transform = self.dataset.transform * self.dataset.transform.scale(            (self.dataset.width / data.shape[-1]),            (self.dataset.height / data.shape[-2])        )        kwargs = self.dataset.meta.copy()        kwargs.update({            'transform': geo_transform,            'width': data.shape[-1],            'height': data.shape[-2]        })        memfile = MemoryFile()        dst = memfile.open(**kwargs)        for i in range(bands):            d = data if len(data.shape) == 2 else data[i, :, :]            dst.write(d, i + 1)        dst.close()        if in_place:            self.dataset = memfile.open()        else:            return memfile.open()  # Reopen as DatasetReader    def reproject_raster(self, des_crs: pyproj.CRS = None, width=None, height=None, in_place=True, resampling_method_index=3):        dst_crs = rasterio.crs.CRS.from_wkt(des_crs.to_wkt())        dst_crs = self.get_crs() if dst_crs is None else dst_crs        width = self.get_width() if width is None else width        height = self.get_height() if height is None else height        g_trans, width, height = calculate_default_transform(self.get_crs(), dst_crs, width,                                                             height, *self.get_raster_extent())        kwargs = self.get_metadata_copy()        kwargs.update({            'crs': dst_crs,            'transform': g_trans,            'width': width,            'height': height        })        memfile = MemoryFile()        dst = memfile.open(**kwargs)        for i in range(1, self.dataset.count + 1):            reproject(                source=rasterio.band(self.dataset, i),                destination=rasterio.band(dst, i),                src_transform=self.get_geo_transform(),                src_crs=self.get_crs(),                dst_transform=transform,                dst_crs=dst_crs,                resampling=self.resampling_method[resampling_method_index])        dst.close()        if in_place:            self.dataset = memfile.open()        else:            return memfile.open()    def clip_raster(self, aoi: gpd.GeoDataFrame, in_place=True):        """        clip raster based on aoi        :param aoi: shapely polygon geometry        :param in_place: boolean        :return: RioRaster        """        if str(aoi.crs).lower() != str(self.get_crs()).lower():            geo = aoi.to_crs(self.get_crs())        else:            geo = aoi        def getFeatures(gdf):            """Function to parse features from GeoDataFrame in such a manner that rasterio wants them"""            import json            return [json.loads(gdf.to_json())['features'][0]['geometry']]        coords = getFeatures(geo)        nodata = self.get_nodata_value() if self.get_nodata_value() else 0        out_img, out_transform = mask(dataset=self.dataset, shapes=coords, crop=True, nodata=nodata)        out_meta = self.dataset.meta.copy()        out_meta.update({"driver": "GTiff",                         "height": out_img.shape[1],                         "width": out_img.shape[2],                         "transform": out_transform,                         # "nodata": nodata,                         "crs": self.dataset.crs})        if in_place:            self.dataset = self.rio_dataset_from_array(out_img, out_meta)        else:            return self.rio_dataset_from_array(out_img, out_meta)    def pad_raster(self, des_raster):        """        clip or pad raster to mak align with bounds        :param des_raster:        :return:        """        # bounds = self.get_spectral_resolution()        # ulx = gt[0] - gt[1] * npad        # uly = gt[3] - gt[5] * npad        aff: Affine = self.get_geo_transform()        des_bounds = des_raster.get_bounds()        rows, cols = rasterio.transform.rowcol(aff, xs=[des_bounds[0], des_bounds[2]], ys=[des_bounds[3], des_bounds[1]])        height = rows[1] - rows[0]        width = cols[1] - cols[0]        window = windows.Window(col_off=cols[0], row_off=rows[0],                                width=width, height=height)  # .intersection(big_window)        window_transform = windows.transform(window, self.get_geo_transform())        kwargs = self.dataset.meta.copy()        kwargs.update({            'crs': self.get_crs(),            'transform': window_transform,            'width': width,            'height': height        })        memfile = MemoryFile()        dst = memfile.open(**kwargs)        # for i in range(bands):        #     # tile = self.dataset.read()        data = self.dataset.read(window=window, boundless=False, fill_value=self.dataset.nodata)        dst.write(data)        dst.close()        self.dataset = memfile.open()    def get_dataset_under_envelop(self, envelop: Union[Polygon, gpd.GeoDataFrame], in_place=True) -> DatasetReader:        if isinstance(envelop, Polygon):            des_bounds = envelop.bounds        else:            if str(self.get_crs()).lower() != str(envelop.crs).lower():                envelop.to_crs(self.get_crs())            des_bounds = tuple(envelop.bounds.values[0])        aff = self.get_geo_transform()        rows, cols = rasterio.transform.rowcol(aff, xs=[des_bounds[0], des_bounds[2]], ys=[des_bounds[3], des_bounds[1]])        height = abs(rows[0] - rows[1])        width = abs(cols[0] - cols[1])        window = windows.Window(col_off=cols[0], row_off=rows[0], width=width, height=height)  # .intersection(big_window)        window_transform = windows.transform(window, self.get_geo_transform())        data = self.dataset.read(window=window, boundless=True, fill_value=self.dataset.nodata)        kwargs = self.dataset.meta.copy()        kwargs.update({            'transform': window_transform,            'width': width,            'height': height        })        dataset = self.rio_dataset_from_array(data, kwargs)        if in_place:            self.dataset = dataset        else:            return dataset    def reclassify_raster(self, thresholds, band=1, nodata=0):        """        :param thresholds:            example:  {                    "water": (('lt', 0.015), 4),                    "built-up": ((0.015, 0.02), 1),                    "barren": ((0.07, 0.27), 2),                    "vegetation": (('gt', 0.27), 3)                }        :param band:            band no        :return:        """        img_arr = self.get_data_array(band)        res = np.empty(img_arr.shape)        res[:] = nodata        for key in thresholds:            if thresholds[key][0][0] == 'lt':                res = np.where(img_arr <= thresholds[key][0][1], thresholds[key][1], res)            elif thresholds[key][0][0] == 'gt':                res = np.where(img_arr >= thresholds[key][0][1], thresholds[key][1], res)            else:                con = np.logical_and(img_arr >= thresholds[key][0][0], img_arr <= thresholds[key][0][1])                res = np.where(con, thresholds[key][1], res)        return res.astype(np.uint8)    def make_coincident_with(self, des_raster: 'RioRaster', resampling_method_index=3):        if not self.is_image_crs_same(des_raster):            self.reproject_raster(des_raster.get_crs(), resampling_method_index=resampling_method_index)        des_bbox = des_raster.get_envelop()        src_bbox = self.get_envelop()        # envelop = des_bbox.intersection(src_bbox)        # crs = self.get_crs()        # envelop = gpd.GeoDataFrame({'geometry': envelop}, index=[0], crs=crs)        if not des_bbox.equals(src_bbox):            self.get_dataset_under_envelop(des_bbox)        if not self.is_image_resolution_same(des_raster):            width = des_raster.get_width()            height = des_raster.get_height()            self.resample_raster(width, height, resampling_method_index=resampling_method_index)    @classmethod    def rio_dataset_from_array(cls, data: np.ndarray, meta) -> DatasetReader:        bands = 1 if len(data.shape) == 2 else data.shape[0]        memfile = MemoryFile()        dst = memfile.open(**meta)        for i in range(bands):            d = data if len(data.shape) == 2 else data[i, :, :]            dst.write(d, i + 1)        dst.close()        dataset = memfile.open()  # Reopen as DatasetReader        return dataset    def change_datatype(self, new_dtype: np.dtype = "float32"):        data = self.get_data_array()        # band, *_ = data.shape        # for b in range(band):        #     data[b] = data[b].astype(new_dtype)        out_meta = self.dataset.meta.copy()        out_meta.update({"nodata": self.get_nodata_value(),                         "dtype": new_dtype})        self.dataset = self.rio_dataset_from_array(data, out_meta)    def add_nodata_value(self, val):        out_meta = self.dataset.meta.copy()        out_meta.update({"nodata": val})        data = self.get_data_array()        self.dataset = self.rio_dataset_from_array(data, out_meta)    def get_x_y_value_raster(self, in_lat_long=False) -> (np.ndarray, np.ndarray):        """        This function retrieves information about the X and Y raster        :return: lat and lon raster        """        rows, cols = self.get_img_resolution()        if in_lat_long and self.get_raster_srid() != 4326:            geo_t, width, height = calculate_default_transform(self.get_crs(), CRS.from_epsg(4326),                                                               self.get_width(), self.get_height(),                                                               *self.get_raster_extent())        else:            geo_t = self.get_geo_transform()        X = np.zeros((rows, cols))        Y = np.zeros((rows, cols))        # tim way of doing it        # for col in np.arange(cols):        #     # lon[:, col] = geo_t[0] + col * geo_t[1] + geo_t[1] / 2        #     lon[:, col] = geo_t[2] + col * geo_t[0] + geo_t[0] / 2        #     # ULx + col*(E-W pixel spacing) + E-W pixel spacing        # for row in np.arange(rows):        #     # lat[row, :] = geo_t[3] + row * geo_t[5] + geo_t[5] / 2        #     lat[row, :] = geo_t[5] + row * geo_t[4] + geo_t[4] / 2        # return lat, lon        for i in np.arange(cols):            for j in np.arange(i, rows):                Y[j, :] = i * geo_t[3] + j * geo_t[4] + geo_t[5]                break            X[:, i] = i * geo_t[0] + j * geo_t[1] + geo_t[2]        return X, Y    def calculate_spatial_resolution_in_meter(self):        """        This functions calculated the distance between each pixel in meter.        Returns        -------        dlat: array            Array containing the vertical distance between each pixel in meters        dlon: array            Array containing the horizontal distance between each pixel in meters        """        geo_out = self.get_geo_transform()        size_Y, size_X = self.get_img_resolution()        # Create the lat/lon rasters        # lon = np.arange(size_X + 1) * geo_out[1] + geo_out[0] - 0.5 * geo_out[1]        # lat = np.arange(size_Y + 1) * geo_out[5] + geo_out[3] - 0.5 * geo_out[5]        lon = np.arange(size_X + 1) * geo_out[0] + geo_out[2] - 0.5 * geo_out[0]        lat = np.arange(size_Y + 1) * geo_out[4] + geo_out[5] - 0.5 * geo_out[4]        dlat_2d = np.array([lat, ] * int(np.size(lon, 0))).transpose()        dlon_2d = np.array([lon, ] * int(np.size(lat, 0)))        # Radius of the earth in meters        R_earth = 6371000        # Calculate the lat and lon in radians        lonRad = dlon_2d * np.pi / 180        latRad = dlat_2d * np.pi / 180        # Calculate the difference in lat and lon        lonRad_dif = abs(lonRad[:, 1:] - lonRad[:, :-1])        latRad_dif = abs(latRad[:-1] - latRad[1:])        # Calculate the distance between the upper and lower pixel edge        a = np.sin(latRad_dif[:, :-1] / 2) * np.sin(latRad_dif[:, :-1] / 2)        clat = 2 * np.arctan2(np.sqrt(a), np.sqrt(1 - a))        dlat = R_earth * clat        # Calculate the distance between the eastern and western pixel edge        b = np.cos(latRad[1:, :-1]) * np.cos(latRad[:-1, :-1]) * np.sin(lonRad_dif[:-1, :] / 2) * np.sin(lonRad_dif[:-1, :] / 2)        clon = 2 * np.arctan2(np.sqrt(b), np.sqrt(1 - b));        dlon = R_earth * clon        return dlon, dlat    def transform_to_metric_unit_projections(self, in_place=False):        if self.get_pyproj_crs().to_epsg() == 4326:            gt = self.get_geo_transform()            utm_srid = TransformationOperations.coord_to_utm_srid(gt[2], gt[5])            temp_rio_ds = self.reproject_raster(CRS.from_epsg(utm_srid), in_place=False)        else:            temp_rio_ds = self.get_dataset()        if in_place:            self.dataset = temp_rio_ds        else:            return temp_rio_ds    def get_pixel_area_band(self):        temp_rio_ds = self.transform_to_metric_unit_projections()        cols = temp_rio_ds.profile.data['width']        rows = temp_rio_ds.profile.data['height']        geo = temp_rio_ds.profile.data['transform']        # geo 0 and 4 index are scaling factor of x and y respectively        return np.ones((rows, cols)) * geo[0] * geo[4]    @staticmethod    def get_s3_session(aws_access_key_id, aws_secret_access_key, region_name):        return Session(aws_access_key_id, aws_secret_access_key, region_name)    def upload_to_s3(self, img_des: str, session: Session):        self.write_to_file(img_des, self.get_data_array(), self.get_crs(),                           self.get_geo_transform(), self.get_nodata_value(), session)
```

### Comparing `digitalarztools-0.0.7/digitalarztools/test/raster/test_functionalities.py` & `digitalarztools-0.0.8/digitalarztools/test/raster/test_functionalities.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/utils/date_utils.py` & `digitalarztools-0.0.8/digitalarztools/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/utils/logger.py` & `digitalarztools-0.0.8/digitalarztools/utils/logger.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/utils/waitbar_console.py` & `digitalarztools-0.0.8/digitalarztools/utils/waitbar_console.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools/vector/gpd_vector.py` & `digitalarztools-0.0.8/digitalarztools/vector/gpd_vector.py`

 * *Files identical despite different names*

### Comparing `digitalarztools-0.0.7/digitalarztools.egg-info/PKG-INFO` & `digitalarztools-0.0.8/digitalarztools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalarztools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Digital Arz tools for applications
 Home-page: UNKNOWN
 Author: Ather Ashraf
 Author-email: atherashraf@gmail.com
 License: UNKNOWN
 Keywords: raster,vector,digitalarz
 Platform: UNKNOWN
```

### Comparing `digitalarztools-0.0.7/digitalarztools.egg-info/SOURCES.txt` & `digitalarztools-0.0.8/digitalarztools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 digitalarztools/pipelines/soil_grids/n_van_genuchten.py
 digitalarztools/pipelines/soil_grids/soil_contents.py
 digitalarztools/pipelines/soil_grids/theta_fc.py
 digitalarztools/pipelines/soil_grids/theta_res.py
 digitalarztools/pipelines/soil_grids/theta_sat2.py
 digitalarztools/raster/__init__.py
 digitalarztools/raster/band_process.py
+digitalarztools/raster/cog_raster.py
 digitalarztools/raster/gdal_raster.py
 digitalarztools/raster/gdal_raster_io.py
 digitalarztools/raster/hdf_reader.py
 digitalarztools/raster/indices.py
 digitalarztools/raster/rio_extraction.py
 digitalarztools/raster/rio_process.py
 digitalarztools/raster/rio_raster.py
@@ -77,14 +78,15 @@
 digitalarztools/test/__init__.py
 digitalarztools/test/test_config.py
 digitalarztools/test/raster/__init__.py
 digitalarztools/test/raster/test_functionalities.py
 digitalarztools/utils/__init__.py
 digitalarztools/utils/date_utils.py
 digitalarztools/utils/logger.py
+digitalarztools/utils/s3_utils.py
 digitalarztools/utils/waitbar_console.py
 digitalarztools/vector/__init__.py
 digitalarztools/vector/gpd_vector.py
 test/__init__.py
 test/test_config.py
 test/test_raster_io.py
 test/test_vector_io.py
```

### Comparing `digitalarztools-0.0.7/setup.py` & `digitalarztools-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 lib_folder = os.path.dirname(os.path.realpath(__file__))
 requirement_path = lib_folder + '/digitalarztools/requirements.txt'
 install_requires = []  # Here we'll get: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
 if os.path.isfile(requirement_path):
     with open(requirement_path) as f:
         install_requires = f.read().splitlines()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Digital Arz tools for applications'
 LONG_DESCRIPTION = 'Package provides tool for developing digitalarz application using rasterio, gdal, geopandas, and pandas'
 
 # Setting up
 setuptools.setup(
     name="digitalarztools",
     version=VERSION,
```

### Comparing `digitalarztools-0.0.7/test/test_raster_io.py` & `digitalarztools-0.0.8/test/test_raster_io.py`

 * *Files identical despite different names*

