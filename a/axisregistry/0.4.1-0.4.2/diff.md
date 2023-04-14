# Comparing `tmp/axisregistry-0.4.1.tar.gz` & `tmp/axisregistry-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axisregistry-0.4.1.tar", last modified: Thu Apr 13 15:30:32 2023, max compression
+gzip compressed data, was "axisregistry-0.4.2.tar", last modified: Fri Apr 14 10:17:47 2023, max compression
```

## Comparing `axisregistry-0.4.1.tar` & `axisregistry-0.4.2.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:30:32.206563 axisregistry-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:30:32.182562 axisregistry-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:30:32.186563 axisregistry-0.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-13 15:30:16.000000 axisregistry-0.4.1/.github/ISSUE_TEMPLATE/1_add-axis.md
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 15:30:16.000000 axisregistry-0.4.1/.github/ISSUE_TEMPLATE/2_anything-else.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:30:32.186563 axisregistry-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-13 15:30:16.000000 axisregistry-0.4.1/.github/workflows/publish-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-13 15:30:16.000000 axisregistry-0.4.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 15:30:16.000000 axisregistry-0.4.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-13 15:30:16.000000 axisregistry-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-13 15:30:16.000000 axisregistry-0.4.1/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-04-13 15:30:16.000000 axisregistry-0.4.1/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:30:32.182562 axisregistry-0.4.1/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:30:32.186563 axisregistry-0.4.1/Lib/axisregistry/
--rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 15:30:31.000000 axisregistry-0.4.1/Lib/axisregistry/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/axes.proto
--rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/axes_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:30:32.198563 axisregistry-0.4.1/Lib/axisregistry/data/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/bounce.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/casual.svg
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/casual.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/cursive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/cursive.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/edge_highlight.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/element_grid.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/element_shape.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/extrusion_depth.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/fill.svg
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/fill.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/flare.svg
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/flare.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/grade.svg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/grade.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/hyper_expansion.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/informality.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    24217 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/italic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/italic.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/monospace.svg
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/monospace.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/morph.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/mutation.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/optical_size.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/optical_size.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/roundness.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/slant.svg
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/slant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/softness.svg
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/softness.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/spacing.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/volume.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    13971 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/weight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/weight.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/width.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/width.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    33987 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/wonky.svg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/wonky.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/x_opaque.svg
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/x_opaque.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/x_rotation.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/x_transparent.svg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/x_transparent.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/x_transparent_figures.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_opaque.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_opaque.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_rotation.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_ascender.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_ascender.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_descender.svg
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_descender.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_figures.svg
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_figures.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_lowercase.svg
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_lowercase.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_uppercase.svg
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_uppercase.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-13 15:30:16.000000 axisregistry-0.4.1/Lib/axisregistry/data/year.textproto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:30:32.190563 axisregistry-0.4.1/Lib/axisregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-13 15:30:32.000000 axisregistry-0.4.1/Lib/axisregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-13 15:30:32.000000 axisregistry-0.4.1/Lib/axisregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:30:32.000000 axisregistry-0.4.1/Lib/axisregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:30:32.000000 axisregistry-0.4.1/Lib/axisregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 15:30:32.000000 axisregistry-0.4.1/Lib/axisregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 15:30:32.000000 axisregistry-0.4.1/Lib/axisregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-13 15:30:32.206563 axisregistry-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-13 15:30:16.000000 axisregistry-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 15:30:16.000000 axisregistry-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:30:32.206563 axisregistry-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-13 15:30:16.000000 axisregistry-0.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 15:30:16.000000 axisregistry-0.4.1/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:30:32.198563 axisregistry-0.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:30:32.206563 axisregistry-0.4.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    83576 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/MavenPro-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   584112 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/OpenSans-Italic[wdth,wght].ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/OpenSans-Italic[wdth,wght]_STAT.ttx
--rw-r--r--   0 runner    (1001) docker     (123)  1054652 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/OpenSansCondensed-Italic[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/OpenSansCondensed-Italic[wght]_STAT.ttx
--rw-r--r--   0 runner    (1001) docker     (123)   973780 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/OpenSansCondensed[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/OpenSansCondensed[wght]_STAT.ttx
--rw-r--r--   0 runner    (1001) docker     (123)   532636 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/OpenSans[wdth,wght].ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/OpenSans[wdth,wght]_STAT.ttx
--rw-r--r--   0 runner    (1001) docker     (123)  1755856 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/RobotoFlex[GRAD,XOPQ,XTRA,YOPQ,YTAS,YTDE,YTFI,YTLC,YTUC,opsz,slnt,wdth,wght].ttf
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/RobotoFlex[GRAD,XOPQ,XTRA,YOPQ,YTAS,YTDE,YTFI,YTLC,YTUC,opsz,slnt,wdth,wght]_STAT.ttx
--rw-r--r--   0 runner    (1001) docker     (123)   532564 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/Wonky[wdth,wght].ttf
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/data/Wonky[wdth,wght]_STAT.ttx
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/gen_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/test_axisregistry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-13 15:30:16.000000 axisregistry-0.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:17:47.958487 axisregistry-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:17:47.942487 axisregistry-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:17:47.942487 axisregistry-0.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-14 10:17:35.000000 axisregistry-0.4.2/.github/ISSUE_TEMPLATE/1_add-axis.md
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 10:17:35.000000 axisregistry-0.4.2/.github/ISSUE_TEMPLATE/2_anything-else.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:17:47.942487 axisregistry-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-14 10:17:35.000000 axisregistry-0.4.2/.github/workflows/publish-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-14 10:17:35.000000 axisregistry-0.4.2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-14 10:17:35.000000 axisregistry-0.4.2/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-14 10:17:35.000000 axisregistry-0.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-14 10:17:35.000000 axisregistry-0.4.2/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-04-14 10:17:35.000000 axisregistry-0.4.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:17:47.942487 axisregistry-0.4.2/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:17:47.942487 axisregistry-0.4.2/Lib/axisregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)    20011 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 10:17:47.000000 axisregistry-0.4.2/Lib/axisregistry/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/axes.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/axes_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:17:47.950487 axisregistry-0.4.2/Lib/axisregistry/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/bounce.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/casual.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/casual.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/cursive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/cursive.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/edge_highlight.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/element_grid.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/element_shape.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/extrusion_depth.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/fill.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/fill.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/flare.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/flare.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/grade.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/grade.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/hyper_expansion.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/informality.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    24217 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/italic.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/monospace.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/monospace.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/morph.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/mutation.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/optical_size.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/optical_size.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/roundness.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/slant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/slant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/softness.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/softness.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/spacing.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/volume.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    13971 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/weight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/weight.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/width.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/width.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    33987 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/wonky.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/wonky.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/x_opaque.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/x_opaque.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/x_rotation.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/x_transparent.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/x_transparent.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/x_transparent_figures.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_opaque.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_opaque.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_rotation.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_ascender.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_ascender.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_descender.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_descender.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_figures.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_figures.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_lowercase.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_lowercase.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_uppercase.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_uppercase.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-14 10:17:35.000000 axisregistry-0.4.2/Lib/axisregistry/data/year.textproto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:17:47.942487 axisregistry-0.4.2/Lib/axisregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-14 10:17:47.000000 axisregistry-0.4.2/Lib/axisregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-14 10:17:47.000000 axisregistry-0.4.2/Lib/axisregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:17:47.000000 axisregistry-0.4.2/Lib/axisregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:17:47.000000 axisregistry-0.4.2/Lib/axisregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-14 10:17:47.000000 axisregistry-0.4.2/Lib/axisregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 10:17:47.000000 axisregistry-0.4.2/Lib/axisregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-14 10:17:47.958487 axisregistry-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-14 10:17:35.000000 axisregistry-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 10:17:35.000000 axisregistry-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:17:47.958487 axisregistry-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-14 10:17:35.000000 axisregistry-0.4.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 10:17:35.000000 axisregistry-0.4.2/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:17:47.950487 axisregistry-0.4.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:17:47.958487 axisregistry-0.4.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    83576 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/MavenPro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   584112 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/OpenSans-Italic[wdth,wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/OpenSans-Italic[wdth,wght]_STAT.ttx
+-rw-r--r--   0 runner    (1001) docker     (123)  1054652 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/OpenSansCondensed-Italic[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/OpenSansCondensed-Italic[wght]_STAT.ttx
+-rw-r--r--   0 runner    (1001) docker     (123)   973780 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/OpenSansCondensed[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/OpenSansCondensed[wght]_STAT.ttx
+-rw-r--r--   0 runner    (1001) docker     (123)   532636 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/OpenSans[wdth,wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/OpenSans[wdth,wght]_STAT.ttx
+-rw-r--r--   0 runner    (1001) docker     (123)  1150824 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/Playfair[opsz,wdth,wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (123)  1755856 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/RobotoFlex[GRAD,XOPQ,XTRA,YOPQ,YTAS,YTDE,YTFI,YTLC,YTUC,opsz,slnt,wdth,wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/RobotoFlex[GRAD,XOPQ,XTRA,YOPQ,YTAS,YTDE,YTFI,YTLC,YTUC,opsz,slnt,wdth,wght]_STAT.ttx
+-rw-r--r--   0 runner    (1001) docker     (123)    77432 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/Wavefont[ROND,YALN,wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/Wavefont[ROND,YALN,wght]_STAT.ttx
+-rw-r--r--   0 runner    (1001) docker     (123)   532564 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/Wonky[wdth,wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/data/Wonky[wdth,wght]_STAT.ttx
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/gen_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/test_axisregistry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-14 10:17:35.000000 axisregistry-0.4.2/tox.ini
```

### Comparing `axisregistry-0.4.1/.github/ISSUE_TEMPLATE/1_add-axis.md` & `axisregistry-0.4.2/.github/ISSUE_TEMPLATE/1_add-axis.md`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/.github/workflows/publish-release.yml` & `axisregistry-0.4.2/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/.github/workflows/tox.yml` & `axisregistry-0.4.2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/CHANGELOG.md` & `axisregistry-0.4.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/CONTRIBUTORS.txt` & `axisregistry-0.4.2/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/LICENSE.txt` & `axisregistry-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/__init__.py` & `axisregistry-0.4.2/Lib/axisregistry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,18 @@
     res = OrderedDict()
     for a in ttFont["fvar"].axes:
         fallback = axis_registry.fallback_for_value(a.axisTag, a.defaultValue)
         if fallback:
             name = fallback.name
             elided = fallback.value == axis_registry[
                 a.axisTag
-            ].default_value and name not in ["Regular", "Italic"]
+            ].default_value and name not in ["Regular", "Italic", "14pt"]
+        elif a.axisTag == "opsz":
+            name = f"{int(a.defaultValue)}pt"
+            elided = False
         else:
             name = None
             elided = True  # since we can't find a name for it, keep it elided
         res[a.axisTag] = {"value": a.defaultValue, "name": name, "elided": elided}
     return res
 
 
@@ -212,27 +215,30 @@
                     # include flags and linked values
                     "flags": 0x2
                     if fallback.value == axis_registry[axis].default_value
                     else 0x0,
                 }
             )
             if axis in LINKED_VALUES and fallback.value in LINKED_VALUES[axis]:
-                a["values"][-1]["linkedValue"] = LINKED_VALUES[axis][fallback.value]
+                linked_value = LINKED_VALUES[axis][fallback.value]
+                if any(f.value == linked_value for f in fallbacks):
+                    a["values"][-1]["linkedValue"] = linked_value
         res.append(a)
 
     for axis, fallback in fallbacks_in_names:
         if axis in seen_axes:
             continue
         a = {
             "tag": axis,
             "name": axis_registry[axis].display_name,
             "values": [{"name": fallback.name, "value": fallback.value, "flags": 0x0}],
         }
         if axis in LINKED_VALUES and fallback.value in LINKED_VALUES[axis]:
-            a["values"][0]["linkedValue"] = LINKED_VALUES[axis][fallback.value]
+            linked_value = LINKED_VALUES[axis][fallback.value]
+            a["values"][0]["linkedValue"] = linked_value
         res.append(a)
 
     for axis, fallback in fallbacks_in_siblings:
         if axis in seen_axes:
             continue
         elided_value = axis_registry[axis].default_value
         elided_fallback = axis_registry.fallback_for_value(axis, elided_value)
```

### Comparing `axisregistry-0.4.1/Lib/axisregistry/axes.proto` & `axisregistry-0.4.2/Lib/axisregistry/axes.proto`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/axes_pb2.py` & `axisregistry-0.4.2/Lib/axisregistry/axes_pb2.py`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/casual.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/casual.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/cursive.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/cursive.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/cursive.textproto` & `axisregistry-0.4.2/Lib/axisregistry/data/cursive.textproto`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/fill.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/fill.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/fill.textproto` & `axisregistry-0.4.2/Lib/axisregistry/data/fill.textproto`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/flare.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/flare.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/grade.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/grade.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/grade.textproto` & `axisregistry-0.4.2/Lib/axisregistry/data/grade.textproto`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/italic.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/italic.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/italic.textproto` & `axisregistry-0.4.2/Lib/axisregistry/data/italic.textproto`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/monospace.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/monospace.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/monospace.textproto` & `axisregistry-0.4.2/Lib/axisregistry/data/monospace.textproto`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/optical_size.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/optical_size.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/optical_size.textproto` & `axisregistry-0.4.2/Lib/axisregistry/data/optical_size.textproto`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/slant.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/slant.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/softness.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/softness.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/weight.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/weight.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/weight.textproto` & `axisregistry-0.4.2/Lib/axisregistry/data/weight.textproto`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/width.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/width.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/width.textproto` & `axisregistry-0.4.2/Lib/axisregistry/data/width.textproto`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/wonky.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/wonky.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/wonky.textproto` & `axisregistry-0.4.2/Lib/axisregistry/data/wonky.textproto`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/x_opaque.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/x_opaque.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/x_transparent.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/x_transparent.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/y_opaque.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/y_opaque.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_ascender.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_ascender.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_descender.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_descender.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_figures.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_figures.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_lowercase.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_lowercase.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry/data/y_transparent_uppercase.svg` & `axisregistry-0.4.2/Lib/axisregistry/data/y_transparent_uppercase.svg`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/Lib/axisregistry.egg-info/PKG-INFO` & `axisregistry-0.4.2/Lib/axisregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axisregistry
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python API to access data from the Google Fonts variable fonts axis registry.
 Home-page: https://github.com/googlefonts/axisregistry/
 Author: Felipe Sanches
 Author-email: juca@members.fsf.org
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `axisregistry-0.4.1/Lib/axisregistry.egg-info/SOURCES.txt` & `axisregistry-0.4.2/Lib/axisregistry.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -87,11 +87,14 @@
 tests/data/OpenSans-Italic[wdth,wght]_STAT.ttx
 tests/data/OpenSansCondensed-Italic[wght].ttf
 tests/data/OpenSansCondensed-Italic[wght]_STAT.ttx
 tests/data/OpenSansCondensed[wght].ttf
 tests/data/OpenSansCondensed[wght]_STAT.ttx
 tests/data/OpenSans[wdth,wght].ttf
 tests/data/OpenSans[wdth,wght]_STAT.ttx
+tests/data/Playfair[opsz,wdth,wght].ttf
 tests/data/RobotoFlex[GRAD,XOPQ,XTRA,YOPQ,YTAS,YTDE,YTFI,YTLC,YTUC,opsz,slnt,wdth,wght].ttf
 tests/data/RobotoFlex[GRAD,XOPQ,XTRA,YOPQ,YTAS,YTDE,YTFI,YTLC,YTUC,opsz,slnt,wdth,wght]_STAT.ttx
+tests/data/Wavefont[ROND,YALN,wght].ttf
+tests/data/Wavefont[ROND,YALN,wght]_STAT.ttx
 tests/data/Wonky[wdth,wght].ttf
 tests/data/Wonky[wdth,wght]_STAT.ttx
```

### Comparing `axisregistry-0.4.1/PKG-INFO` & `axisregistry-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axisregistry
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python API to access data from the Google Fonts variable fonts axis registry.
 Home-page: https://github.com/googlefonts/axisregistry/
 Author: Felipe Sanches
 Author-email: juca@members.fsf.org
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `axisregistry-0.4.1/README.md` & `axisregistry-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/setup.py` & `axisregistry-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/MavenPro-Regular.ttf` & `axisregistry-0.4.2/tests/data/MavenPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/OpenSans-Italic[wdth,wght].ttf` & `axisregistry-0.4.2/tests/data/OpenSans-Italic[wdth,wght].ttf`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/OpenSans-Italic[wdth,wght]_STAT.ttx` & `axisregistry-0.4.2/tests/data/OpenSans-Italic[wdth,wght]_STAT.ttx`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/OpenSansCondensed-Italic[wght].ttf` & `axisregistry-0.4.2/tests/data/OpenSansCondensed-Italic[wght].ttf`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/OpenSansCondensed-Italic[wght]_STAT.ttx` & `axisregistry-0.4.2/tests/data/OpenSansCondensed-Italic[wght]_STAT.ttx`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/OpenSansCondensed[wght].ttf` & `axisregistry-0.4.2/tests/data/OpenSansCondensed[wght].ttf`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/OpenSansCondensed[wght]_STAT.ttx` & `axisregistry-0.4.2/tests/data/OpenSansCondensed[wght]_STAT.ttx`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/OpenSans[wdth,wght].ttf` & `axisregistry-0.4.2/tests/data/OpenSans[wdth,wght].ttf`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/OpenSans[wdth,wght]_STAT.ttx` & `axisregistry-0.4.2/tests/data/OpenSans[wdth,wght]_STAT.ttx`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/RobotoFlex[GRAD,XOPQ,XTRA,YOPQ,YTAS,YTDE,YTFI,YTLC,YTUC,opsz,slnt,wdth,wght].ttf` & `axisregistry-0.4.2/tests/data/RobotoFlex[GRAD,XOPQ,XTRA,YOPQ,YTAS,YTDE,YTFI,YTLC,YTUC,opsz,slnt,wdth,wght].ttf`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/RobotoFlex[GRAD,XOPQ,XTRA,YOPQ,YTAS,YTDE,YTFI,YTLC,YTUC,opsz,slnt,wdth,wght]_STAT.ttx` & `axisregistry-0.4.2/tests/data/RobotoFlex[GRAD,XOPQ,XTRA,YOPQ,YTAS,YTDE,YTFI,YTLC,YTUC,opsz,slnt,wdth,wght]_STAT.ttx`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/Wonky[wdth,wght].ttf` & `axisregistry-0.4.2/tests/data/Wonky[wdth,wght].ttf`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/data/Wonky[wdth,wght]_STAT.ttx` & `axisregistry-0.4.2/tests/data/Wonky[wdth,wght]_STAT.ttx`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/gen_test_data.py` & `axisregistry-0.4.2/tests/gen_test_data.py`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/test_axisregistry_api.py` & `axisregistry-0.4.2/tests/test_axisregistry_api.py`

 * *Files identical despite different names*

### Comparing `axisregistry-0.4.1/tests/test_names.py` & `axisregistry-0.4.2/tests/test_names.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 )
 mavenpro_fp = os.path.join(DATA_DIR, "MavenPro-Regular.ttf")
 opensans_roman_fp = os.path.join(DATA_DIR, "OpenSans[wdth,wght].ttf")
 opensans_italic_fp = os.path.join(DATA_DIR, "OpenSans-Italic[wdth,wght].ttf")
 opensans_cond_roman_fp = os.path.join(DATA_DIR, "OpenSansCondensed[wght].ttf")
 opensans_cond_italic_fp = os.path.join(DATA_DIR, "OpenSansCondensed-Italic[wght].ttf")
 wonky_fp = os.path.join(DATA_DIR, "Wonky[wdth,wght].ttf")
+playfair_fp = os.path.join(DATA_DIR, "Playfair[opsz,wdth,wght].ttf")
+wavefont_fp = os.path.join(DATA_DIR, "Wavefont[ROND,YALN,wght].ttf")
 
 
 @pytest.fixture
 def static_font():
     return TTFont(mavenpro_fp)
 
 
@@ -289,14 +291,31 @@
                 (3, 3, 1, 0x409): "3.000;GOOG;Wonky-Regular",
                 (4, 3, 1, 0x409): "Wonky Regular",
                 (6, 3, 1, 0x409): "Wonky-Regular",
                 (16, 3, 1, 0x409): None,
                 (17, 3, 1, 0x409): None,
             },
         ),
+        # Test opsz particle is kept.
+        # Fixes https://github.com/googlefonts/axisregistry/issues/130
+        (
+            playfair_fp,
+            "Playfair",
+            None,
+            [],
+            {
+                (1, 3, 1, 0x409): "Playfair 5pt SemiExpanded Light",
+                (2, 3, 1, 0x409): "Regular",
+                (3, 3, 1, 0x409): "2.000;FTH;Playfair-5ptSemiExpandedLight",
+                (4, 3, 1, 0x409): "Playfair 5pt SemiExpanded Light",
+                (6, 3, 1, 0x409): "Playfair-5ptSemiExpandedLight",
+                (16, 3, 1, 0x409): "Playfair",
+                (17, 3, 1, 0x409): "5pt SemiExpanded Light",
+            },
+        ),
     ],
 )
 def test_name_table(fp, family_name, style_name, siblings, expected):
     font = TTFont(fp)
     siblings = [TTFont(fp) for fp in siblings]
     build_name_table(font, family_name, style_name, siblings)
     _test_names(font, expected)
@@ -436,14 +455,17 @@
             [opensans_roman_fp, opensans_italic_fp, opensans_cond_italic_fp],
         ),
         (
             opensans_cond_italic_fp,
             [opensans_roman_fp, opensans_italic_fp, opensans_cond_roman_fp],
         ),
         (wonky_fp, []),
+        # don't add a linkedValue for Regular to Bold since Bold doesn't exist
+        # Fixes https://github.com/googlefonts/axisregistry/issues/104
+        (wavefont_fp, []),
     ],
 )
 def test_stat(fp, sibling_fps):
     font = TTFont(fp)
     siblings = [TTFont(f) for f in sibling_fps]
     build_stat(font, siblings)
     stat_fp = fp.replace(".ttf", "_STAT.ttx")
```

### Comparing `axisregistry-0.4.1/tox.ini` & `axisregistry-0.4.2/tox.ini`

 * *Files identical despite different names*

