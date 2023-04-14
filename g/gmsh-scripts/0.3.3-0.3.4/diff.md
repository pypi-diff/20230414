# Comparing `tmp/gmsh-scripts-0.3.3.tar.gz` & `tmp/gmsh-scripts-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\gmsh_scripts\dist\tmpai9cti2y\gmsh-scripts-0.3.3.tar", last modified: Fri Oct  7 10:38:52 2022, max compression
+gzip compressed data, was "D:\gmsh_scripts\dist\.tmp-1s4dc036\gmsh-scripts-0.3.4.tar", last modified: Fri Apr 14 16:45:49 2023, max compression
```

## Comparing `gmsh-scripts-0.3.3.tar` & `gmsh-scripts-0.3.4.tar`

### file list

```diff
@@ -1,102 +1,77 @@
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/
--rw-rw-rw-   0        0        0    19460 2021-12-24 09:52:39.000000 gmsh-scripts-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3450 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2912 2022-10-05 14:02:24.000000 gmsh-scripts-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/
--rw-rw-rw-   0        0        0        0 2021-03-10 08:22:15.000000 gmsh-scripts-0.3.3/gmsh_scripts/__init__.py
--rw-rw-rw-   0        0        0      434 2022-03-21 16:36:01.000000 gmsh-scripts-0.3.3/gmsh_scripts/__main__.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/block/
--rw-rw-rw-   0        0        0      244 2022-10-05 13:18:59.000000 gmsh-scripts-0.3.3/gmsh_scripts/block/__init__.py
--rw-rw-rw-   0        0        0    32480 2022-05-26 05:48:56.000000 gmsh-scripts-0.3.3/gmsh_scripts/block/block.py
--rw-rw-rw-   0        0        0    27278 2022-10-06 06:48:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/block/layer.py
--rw-rw-rw-   0        0        0    13353 2022-10-04 15:28:31.000000 gmsh-scripts-0.3.3/gmsh_scripts/block/matrix.py
--rw-rw-rw-   0        0        0     5716 2022-05-27 09:38:41.000000 gmsh-scripts-0.3.3/gmsh_scripts/block/polyhedron.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/boolean/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:15:11.000000 gmsh-scripts-0.3.3/gmsh_scripts/boolean/__init__.py
--rw-rw-rw-   0        0        0     1601 2022-03-21 17:01:42.000000 gmsh-scripts-0.3.3/gmsh_scripts/boolean/boolean.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/coordinate_system/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:00:32.000000 gmsh-scripts-0.3.3/gmsh_scripts/coordinate_system/__init__.py
--rw-rw-rw-   0        0        0    19878 2022-10-07 10:33:17.000000 gmsh-scripts-0.3.3/gmsh_scripts/coordinate_system/coordinate_system.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/entity/
--rw-rw-rw-   0        0        0      379 2022-05-24 12:46:03.000000 gmsh-scripts-0.3.3/gmsh_scripts/entity/__init__.py
--rw-rw-rw-   0        0        0      767 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/entity/curve.py
--rw-rw-rw-   0        0        0      646 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/entity/curve_loop.py
--rw-rw-rw-   0        0        0    10097 2022-10-04 15:53:17.000000 gmsh-scripts-0.3.3/gmsh_scripts/entity/point.py
--rw-rw-rw-   0        0        0      763 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/entity/surface.py
--rw-rw-rw-   0        0        0      536 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/entity/surface_loop.py
--rw-rw-rw-   0        0        0      771 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/entity/volume.py
--rw-rw-rw-   0        0        0     4817 2022-10-05 13:17:59.000000 gmsh-scripts-0.3.3/gmsh_scripts/factory.py
--rw-rw-rw-   0        0        0      328 2022-03-21 19:57:50.000000 gmsh-scripts-0.3.3/gmsh_scripts/load.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/optimize/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:14:42.000000 gmsh-scripts-0.3.3/gmsh_scripts/optimize/__init__.py
--rw-rw-rw-   0        0        0     3240 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/optimize/optimize.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/parse/
--rw-rw-rw-   0        0        0        0 2022-01-20 08:59:59.000000 gmsh-scripts-0.3.3/gmsh_scripts/parse/__init__.py
--rw-rw-rw-   0        0        0    40863 2022-03-21 17:02:08.000000 gmsh-scripts-0.3.3/gmsh_scripts/parse/parse.py
--rw-rw-rw-   0        0        0     3345 2022-03-21 20:05:45.000000 gmsh-scripts-0.3.3/gmsh_scripts/plot.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/quadrate/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:15:29.000000 gmsh-scripts-0.3.3/gmsh_scripts/quadrate/__init__.py
--rw-rw-rw-   0        0        0     1276 2022-01-20 09:03:32.000000 gmsh-scripts-0.3.3/gmsh_scripts/quadrate/quadrate.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/refine/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:13:53.000000 gmsh-scripts-0.3.3/gmsh_scripts/refine/__init__.py
--rw-rw-rw-   0        0        0      762 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/refine/refine.py
--rw-rw-rw-   0        0        0    20940 2022-05-27 09:42:13.000000 gmsh-scripts-0.3.3/gmsh_scripts/registry.py
--rw-rw-rw-   0        0        0     8196 2022-03-21 20:07:49.000000 gmsh-scripts-0.3.3/gmsh_scripts/run.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/size/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:12:44.000000 gmsh-scripts-0.3.3/gmsh_scripts/size/__init__.py
--rw-rw-rw-   0        0        0     5205 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/size/size.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/smooth/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:13:17.000000 gmsh-scripts-0.3.3/gmsh_scripts/smooth/__init__.py
--rw-rw-rw-   0        0        0     1773 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/smooth/smooth.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/strategy/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:13:40.000000 gmsh-scripts-0.3.3/gmsh_scripts/strategy/__init__.py
--rw-rw-rw-   0        0        0     8536 2022-03-21 17:02:24.000000 gmsh-scripts-0.3.3/gmsh_scripts/strategy/strategy.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/structure/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:14:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/structure/__init__.py
--rw-rw-rw-   0        0        0     7321 2022-03-21 17:01:35.000000 gmsh-scripts-0.3.3/gmsh_scripts/structure/structure.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/support/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:11:51.000000 gmsh-scripts-0.3.3/gmsh_scripts/support/__init__.py
--rw-rw-rw-   0        0        0    31989 2022-03-31 17:32:18.000000 gmsh-scripts-0.3.3/gmsh_scripts/support/support.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/
--rw-rw-rw-   0        0        0        0 2022-03-21 18:30:21.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/block/
--rw-rw-rw-   0        0        0        0 2022-05-24 10:54:03.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/block/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/block/polyhedron/
--rw-rw-rw-   0        0        0        0 2022-05-24 10:54:14.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/block/polyhedron/__init__.py
--rw-rw-rw-   0        0        0      953 2022-05-27 09:02:04.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/block/polyhedron/test_polyhedron.py
--rw-rw-rw-   0        0        0      637 2022-03-31 17:15:41.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/examples/
--rw-rw-rw-   0        0        0        0 2022-04-08 06:47:04.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/examples/rise/
--rw-rw-rw-   0        0        0        0 2022-04-08 06:47:28.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/examples/rise/__init__.py
--rw-rw-rw-   0        0        0      597 2022-04-08 09:36:23.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/examples/rise/random_cube.py
--rw-rw-rw-   0        0        0      599 2022-04-08 15:35:46.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/examples/rise/test_rise.py
--rw-rw-rw-   0        0        0        0 2022-04-08 06:47:43.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/examples/test_examples.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/json/
--rw-rw-rw-   0        0        0        0 2022-03-31 17:09:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/json/__init__.py
--rw-rw-rw-   0        0        0      249 2022-03-31 17:42:16.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/json/test_json.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/transform/
--rw-rw-rw-   0        0        0        0 2022-05-26 05:18:55.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/transform/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/transform/transformation_matrix/
--rw-rw-rw-   0        0        0        0 2022-05-26 05:19:13.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/transform/transformation_matrix/__init__.py
--rw-rw-rw-   0        0        0      122 2022-05-26 05:42:15.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/transform/transformation_matrix/test_transformation_matrix.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/yaml/
--rw-rw-rw-   0        0        0        0 2022-03-31 17:09:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/yaml/__init__.py
--rw-rw-rw-   0        0        0      259 2022-03-31 17:41:10.000000 gmsh-scripts-0.3.3/gmsh_scripts/tests/yaml/test_yaml.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/transform/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:03:07.000000 gmsh-scripts-0.3.3/gmsh_scripts/transform/__init__.py
--rw-rw-rw-   0        0        0    23701 2022-05-26 06:00:21.000000 gmsh-scripts-0.3.3/gmsh_scripts/transform/transform.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/utils/
--rw-rw-rw-   0        0        0       65 2022-05-24 14:06:36.000000 gmsh-scripts-0.3.3/gmsh_scripts/utils/__init__.py
--rw-rw-rw-   0        0        0      924 2022-05-24 14:05:40.000000 gmsh-scripts-0.3.3/gmsh_scripts/utils/obj2gmsh.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/gmsh_scripts/zone/
--rw-rw-rw-   0        0        0        0 2022-01-20 09:11:35.000000 gmsh-scripts-0.3.3/gmsh_scripts/zone/__init__.py
--rw-rw-rw-   0        0        0    15868 2022-03-21 17:02:33.000000 gmsh-scripts-0.3.3/gmsh_scripts/zone/zone.py
-drwxrwxrwx   0        0        0        0 2022-10-07 10:38:51.000000 gmsh-scripts-0.3.3/gmsh_scripts.egg-info/
--rw-rw-rw-   0        0        0     3450 2022-10-07 10:38:50.000000 gmsh-scripts-0.3.3/gmsh_scripts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2441 2022-10-07 10:38:50.000000 gmsh-scripts-0.3.3/gmsh_scripts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-07 10:38:50.000000 gmsh-scripts-0.3.3/gmsh_scripts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-10-07 10:38:50.000000 gmsh-scripts-0.3.3/gmsh_scripts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-10-07 10:38:50.000000 gmsh-scripts-0.3.3/gmsh_scripts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-03-20 08:47:46.000000 gmsh-scripts-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0      699 2022-10-07 10:38:52.000000 gmsh-scripts-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:48.000000 gmsh-scripts-0.3.4/
+-rw-rw-rw-   0        0        0    19460 2021-12-24 09:52:39.000000 gmsh-scripts-0.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     5262 2023-04-14 16:45:48.000000 gmsh-scripts-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4703 2023-01-30 13:20:37.000000 gmsh-scripts-0.3.4/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-20 08:47:46.000000 gmsh-scripts-0.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0      736 2023-04-14 16:45:48.000000 gmsh-scripts-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/
+-rw-rw-rw-   0        0        0        0 2021-03-10 08:22:15.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/__init__.py
+-rw-rw-rw-   0        0        0      434 2022-03-21 16:36:01.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/block/
+-rw-rw-rw-   0        0        0      244 2022-10-05 13:18:59.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/block/__init__.py
+-rw-rw-rw-   0        0        0    32480 2023-01-25 10:35:17.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/block/block.py
+-rw-rw-rw-   0        0        0    27369 2023-04-14 16:39:58.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/block/layer.py
+-rw-rw-rw-   0        0        0    13353 2022-10-04 15:28:31.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/block/matrix.py
+-rw-rw-rw-   0        0        0     5716 2022-05-27 09:38:41.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/block/polyhedron.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/boolean/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:15:11.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/boolean/__init__.py
+-rw-rw-rw-   0        0        0     1601 2022-03-21 17:01:42.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/boolean/boolean.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/coordinate_system/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:00:32.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/coordinate_system/__init__.py
+-rw-rw-rw-   0        0        0    19878 2022-10-07 10:33:17.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/coordinate_system/coordinate_system.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/entity/
+-rw-rw-rw-   0        0        0      379 2022-05-24 12:46:03.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/entity/__init__.py
+-rw-rw-rw-   0        0        0      767 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/entity/curve.py
+-rw-rw-rw-   0        0        0      646 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/entity/curve_loop.py
+-rw-rw-rw-   0        0        0    10097 2022-10-04 15:53:17.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/entity/point.py
+-rw-rw-rw-   0        0        0      763 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/entity/surface.py
+-rw-rw-rw-   0        0        0      536 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/entity/surface_loop.py
+-rw-rw-rw-   0        0        0      771 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/entity/volume.py
+-rw-rw-rw-   0        0        0     4817 2022-10-05 13:17:59.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/factory.py
+-rw-rw-rw-   0        0        0      328 2022-03-21 19:57:50.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/load.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/optimize/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:14:42.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/optimize/__init__.py
+-rw-rw-rw-   0        0        0     3240 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/optimize/optimize.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/parse/
+-rw-rw-rw-   0        0        0        0 2022-01-20 08:59:59.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/parse/__init__.py
+-rw-rw-rw-   0        0        0    40863 2022-11-15 19:04:54.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/parse/parse.py
+-rw-rw-rw-   0        0        0     3345 2022-03-21 20:05:45.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/plot.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/quadrate/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:15:29.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/quadrate/__init__.py
+-rw-rw-rw-   0        0        0     1276 2022-01-20 09:03:32.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/quadrate/quadrate.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/refine/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:13:53.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/refine/__init__.py
+-rw-rw-rw-   0        0        0      762 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/refine/refine.py
+-rw-rw-rw-   0        0        0    20940 2022-05-27 09:42:13.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/registry.py
+-rw-rw-rw-   0        0        0     8196 2022-03-21 20:07:49.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/run.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/size/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:12:44.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/size/__init__.py
+-rw-rw-rw-   0        0        0     5205 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/size/size.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/smooth/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:13:17.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/smooth/__init__.py
+-rw-rw-rw-   0        0        0     1773 2021-12-24 09:55:14.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/smooth/smooth.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/strategy/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:13:40.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/strategy/__init__.py
+-rw-rw-rw-   0        0        0     8647 2023-01-26 15:08:01.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/strategy/strategy.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/structure/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:14:14.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/structure/__init__.py
+-rw-rw-rw-   0        0        0     7321 2022-03-21 17:01:35.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/structure/structure.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/support/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:11:51.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/support/__init__.py
+-rw-rw-rw-   0        0        0    31989 2022-03-31 17:32:18.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/support/support.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/transform/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:03:07.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/transform/__init__.py
+-rw-rw-rw-   0        0        0    23701 2022-05-26 06:00:21.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/transform/transform.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:48.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/utils/
+-rw-rw-rw-   0        0        0       65 2022-05-24 14:06:36.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/utils/__init__.py
+-rw-rw-rw-   0        0        0      924 2022-05-24 14:05:40.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/utils/obj2gmsh.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:48.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/zone/
+-rw-rw-rw-   0        0        0        0 2022-01-20 09:11:35.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/zone/__init__.py
+-rw-rw-rw-   0        0        0    15868 2022-03-21 17:02:33.000000 gmsh-scripts-0.3.4/src/gmsh_scripts/zone/zone.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:45:47.000000 gmsh-scripts-0.3.4/src/gmsh_scripts.egg-info/
+-rw-rw-rw-   0        0        0     5262 2023-04-14 16:45:46.000000 gmsh-scripts-0.3.4/src/gmsh_scripts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2101 2023-04-14 16:45:46.000000 gmsh-scripts-0.3.4/src/gmsh_scripts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:45:46.000000 gmsh-scripts-0.3.4/src/gmsh_scripts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-14 16:45:46.000000 gmsh-scripts-0.3.4/src/gmsh_scripts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 16:45:46.000000 gmsh-scripts-0.3.4/src/gmsh_scripts.egg-info/top_level.txt
```

### Comparing `gmsh-scripts-0.3.3/LICENSE.txt` & `gmsh-scripts-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/block/block.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/block/block.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/block/layer.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/block/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,17 +240,19 @@
                 m = [m for _ in range(max_old + 1)]
                 break
         n = [default for _ in new2old]
         for mi, mm in enumerate(m):
             nis = old2new[mi]
             masks = [int(x) for x in list(f'{mm:04b}')]  # NY, NX, X, Y
             # print(mm, nis, masks)
-            if len(nis) == len(masks):
+            if len(nis) == len(masks):  # layers
                 for ni, mask in zip(nis, masks):
                     n[ni] = mask
+            elif len(nis) == 1:  # center
+                n[nis[0]] = masks[0]
         return n
 
     @staticmethod
     def get_layers_curves(parsed_layers_curves,
                           parsed_g2l_b2b_l2l,
                           parsed_layers_coordinates):
         """Parse layers curves
```

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/block/matrix.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/block/matrix.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/block/polyhedron.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/block/polyhedron.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/boolean/boolean.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/boolean/boolean.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/coordinate_system/coordinate_system.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/coordinate_system/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/entity/curve.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/entity/curve.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/entity/curve_loop.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/entity/curve_loop.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/entity/point.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/entity/point.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/entity/surface.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/entity/surface.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/entity/surface_loop.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/entity/surface_loop.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/entity/volume.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/entity/volume.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/factory.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/factory.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/optimize/optimize.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/parse/parse.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/parse/parse.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/plot.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/plot.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/quadrate/quadrate.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/quadrate/quadrate.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/refine/refine.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/refine/refine.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/registry.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/registry.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/run.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/run.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/size/size.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/size/size.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/smooth/smooth.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/smooth/smooth.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/strategy/strategy.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/strategy/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from gmsh_scripts.quadrate.quadrate import  NoQuadrate
 from gmsh_scripts.optimize.optimize import OptimizeOne
 from gmsh_scripts.smooth.smooth import NoSmooth
 from gmsh_scripts.refine.refine import NoRefine
 
 
 class Strategy:
+    """Abstract strategy"""
     def __init__(self, factory=None, model_name=None, output_path=None,
                  output_formats=None):
         factory = 'geo' if factory is None else factory
         model_name = str(uuid.uuid1()) if model_name is None else model_name
         output_path = model_name if output_path is None else output_path
         output_formats = ['geo_unrolled', 'msh2'] if output_formats is None else output_formats
         self.factory = factory
@@ -35,18 +36,15 @@
 
     def __call__(self, block):
         reset_registry(factory=self.factory)
         logging.info(f'number of blocks: {len(block)}')
 
 
 class Base(Strategy):
-    """
-
-    """
-
+    """Default strategy"""
     def __init__(
             self,
             factory=None,
             model_name=None,
             output_path=None,
             output_formats=None,
             boolean_function=BooleanAllBlock(),
@@ -111,14 +109,15 @@
             gmsh.logger.stop()
         else:
             raise ValueError(self.factory)
         gmsh.model.remove()
 
 
 class Fast(Strategy):
+    """Generates geometry only (.geo_unrolled file)"""
     def __init__(self, factory=None, model_name=None, output_path=None,
                  output_formats=None):
         super().__init__(factory, model_name, output_path, output_formats)
 
     def __call__(self, block):
         super().__call__(block)
         gmsh.logger.start()
@@ -150,18 +149,15 @@
         for x in log:
             logging.info(x)
         gmsh.logger.stop()
         gmsh.model.remove()
 
 
 class NoBoolean(Strategy):
-    """
-
-    """
-
+    """Doesn't use boolean operations"""
     def __init__(
             self,
             factory=None,
             model_name=None,
             output_path=None,
             output_formats=None,
             zone_function=BlockZone(),
```

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/structure/structure.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/structure/structure.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/support/support.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/support/support.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/transform/transform.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/transform/transform.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/utils/obj2gmsh.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/utils/obj2gmsh.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts/zone/zone.py` & `gmsh-scripts-0.3.4/src/gmsh_scripts/zone/zone.py`

 * *Files identical despite different names*

### Comparing `gmsh-scripts-0.3.3/gmsh_scripts.egg-info/SOURCES.txt` & `gmsh-scripts-0.3.4/src/gmsh_scripts.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,61 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
-gmsh_scripts/__init__.py
-gmsh_scripts/__main__.py
-gmsh_scripts/factory.py
-gmsh_scripts/load.py
-gmsh_scripts/plot.py
-gmsh_scripts/registry.py
-gmsh_scripts/run.py
-gmsh_scripts.egg-info/PKG-INFO
-gmsh_scripts.egg-info/SOURCES.txt
-gmsh_scripts.egg-info/dependency_links.txt
-gmsh_scripts.egg-info/requires.txt
-gmsh_scripts.egg-info/top_level.txt
-gmsh_scripts/block/__init__.py
-gmsh_scripts/block/block.py
-gmsh_scripts/block/layer.py
-gmsh_scripts/block/matrix.py
-gmsh_scripts/block/polyhedron.py
-gmsh_scripts/boolean/__init__.py
-gmsh_scripts/boolean/boolean.py
-gmsh_scripts/coordinate_system/__init__.py
-gmsh_scripts/coordinate_system/coordinate_system.py
-gmsh_scripts/entity/__init__.py
-gmsh_scripts/entity/curve.py
-gmsh_scripts/entity/curve_loop.py
-gmsh_scripts/entity/point.py
-gmsh_scripts/entity/surface.py
-gmsh_scripts/entity/surface_loop.py
-gmsh_scripts/entity/volume.py
-gmsh_scripts/optimize/__init__.py
-gmsh_scripts/optimize/optimize.py
-gmsh_scripts/parse/__init__.py
-gmsh_scripts/parse/parse.py
-gmsh_scripts/quadrate/__init__.py
-gmsh_scripts/quadrate/quadrate.py
-gmsh_scripts/refine/__init__.py
-gmsh_scripts/refine/refine.py
-gmsh_scripts/size/__init__.py
-gmsh_scripts/size/size.py
-gmsh_scripts/smooth/__init__.py
-gmsh_scripts/smooth/smooth.py
-gmsh_scripts/strategy/__init__.py
-gmsh_scripts/strategy/strategy.py
-gmsh_scripts/structure/__init__.py
-gmsh_scripts/structure/structure.py
-gmsh_scripts/support/__init__.py
-gmsh_scripts/support/support.py
-gmsh_scripts/tests/__init__.py
-gmsh_scripts/tests/conftest.py
-gmsh_scripts/tests/block/__init__.py
-gmsh_scripts/tests/block/polyhedron/__init__.py
-gmsh_scripts/tests/block/polyhedron/test_polyhedron.py
-gmsh_scripts/tests/examples/__init__.py
-gmsh_scripts/tests/examples/test_examples.py
-gmsh_scripts/tests/examples/rise/__init__.py
-gmsh_scripts/tests/examples/rise/random_cube.py
-gmsh_scripts/tests/examples/rise/test_rise.py
-gmsh_scripts/tests/json/__init__.py
-gmsh_scripts/tests/json/test_json.py
-gmsh_scripts/tests/transform/__init__.py
-gmsh_scripts/tests/transform/transformation_matrix/__init__.py
-gmsh_scripts/tests/transform/transformation_matrix/test_transformation_matrix.py
-gmsh_scripts/tests/yaml/__init__.py
-gmsh_scripts/tests/yaml/test_yaml.py
-gmsh_scripts/transform/__init__.py
-gmsh_scripts/transform/transform.py
-gmsh_scripts/utils/__init__.py
-gmsh_scripts/utils/obj2gmsh.py
-gmsh_scripts/zone/__init__.py
-gmsh_scripts/zone/zone.py
+./src/gmsh_scripts.egg-info/PKG-INFO
+./src/gmsh_scripts.egg-info/SOURCES.txt
+./src/gmsh_scripts.egg-info/dependency_links.txt
+./src/gmsh_scripts.egg-info/requires.txt
+./src/gmsh_scripts.egg-info/top_level.txt
+src/gmsh_scripts/__init__.py
+src/gmsh_scripts/__main__.py
+src/gmsh_scripts/factory.py
+src/gmsh_scripts/load.py
+src/gmsh_scripts/plot.py
+src/gmsh_scripts/registry.py
+src/gmsh_scripts/run.py
+src/gmsh_scripts.egg-info/PKG-INFO
+src/gmsh_scripts.egg-info/SOURCES.txt
+src/gmsh_scripts.egg-info/dependency_links.txt
+src/gmsh_scripts.egg-info/requires.txt
+src/gmsh_scripts.egg-info/top_level.txt
+src/gmsh_scripts/block/__init__.py
+src/gmsh_scripts/block/block.py
+src/gmsh_scripts/block/layer.py
+src/gmsh_scripts/block/matrix.py
+src/gmsh_scripts/block/polyhedron.py
+src/gmsh_scripts/boolean/__init__.py
+src/gmsh_scripts/boolean/boolean.py
+src/gmsh_scripts/coordinate_system/__init__.py
+src/gmsh_scripts/coordinate_system/coordinate_system.py
+src/gmsh_scripts/entity/__init__.py
+src/gmsh_scripts/entity/curve.py
+src/gmsh_scripts/entity/curve_loop.py
+src/gmsh_scripts/entity/point.py
+src/gmsh_scripts/entity/surface.py
+src/gmsh_scripts/entity/surface_loop.py
+src/gmsh_scripts/entity/volume.py
+src/gmsh_scripts/optimize/__init__.py
+src/gmsh_scripts/optimize/optimize.py
+src/gmsh_scripts/parse/__init__.py
+src/gmsh_scripts/parse/parse.py
+src/gmsh_scripts/quadrate/__init__.py
+src/gmsh_scripts/quadrate/quadrate.py
+src/gmsh_scripts/refine/__init__.py
+src/gmsh_scripts/refine/refine.py
+src/gmsh_scripts/size/__init__.py
+src/gmsh_scripts/size/size.py
+src/gmsh_scripts/smooth/__init__.py
+src/gmsh_scripts/smooth/smooth.py
+src/gmsh_scripts/strategy/__init__.py
+src/gmsh_scripts/strategy/strategy.py
+src/gmsh_scripts/structure/__init__.py
+src/gmsh_scripts/structure/structure.py
+src/gmsh_scripts/support/__init__.py
+src/gmsh_scripts/support/support.py
+src/gmsh_scripts/transform/__init__.py
+src/gmsh_scripts/transform/transform.py
+src/gmsh_scripts/utils/__init__.py
+src/gmsh_scripts/utils/obj2gmsh.py
+src/gmsh_scripts/zone/__init__.py
+src/gmsh_scripts/zone/zone.py
```

