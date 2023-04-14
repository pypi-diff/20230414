# Comparing `tmp/pytransform3d-3.0.0.tar.gz` & `tmp/pytransform3d-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytransform3d-3.0.0.tar", last modified: Mon Apr  3 19:22:44 2023, max compression
+gzip compressed data, was "pytransform3d-3.1.0.tar", last modified: Fri Apr 14 18:51:49 2023, max compression
```

## Comparing `pytransform3d-3.0.0.tar` & `pytransform3d-3.1.0.tar`

### file list

```diff
@@ -1,52 +1,81 @@
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-03 19:22:44.607969 pytransform3d-3.0.0/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1653 2023-01-12 22:48:31.000000 pytransform3d-3.0.0/LICENSE
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9417 2023-04-03 19:22:44.607969 pytransform3d-3.0.0/PKG-INFO
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8744 2023-04-03 19:15:46.000000 pytransform3d-3.0.0/README.md
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-03 19:22:44.603968 pytransform3d-3.0.0/pytransform3d/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       61 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21369 2022-09-17 15:37:15.000000 pytransform3d-3.0.0/pytransform3d/batch_rotations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    11534 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/camera.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3898 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/coordinates.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13372 2022-02-11 10:41:03.000000 pytransform3d-3.0.0/pytransform3d/editor.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-03 19:22:44.603968 pytransform3d-3.0.0/pytransform3d/plot_utils/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      829 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/plot_utils/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    10111 2022-12-22 19:37:52.000000 pytransform3d-3.0.0/pytransform3d/plot_utils/_artists.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2606 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/plot_utils/_layout.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21851 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/plot_utils/_plot_functions.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-03 19:22:44.607969 pytransform3d-3.0.0/pytransform3d/rotations/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9185 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/rotations/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      407 2022-09-17 15:37:15.000000 pytransform3d-3.0.0/pytransform3d/rotations/_constants.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    61846 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/rotations/_conversions.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3444 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/rotations/_jacobians.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8686 2022-02-11 10:43:44.000000 pytransform3d-3.0.0/pytransform3d/rotations/_plot.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7380 2023-01-12 22:48:31.000000 pytransform3d-3.0.0/pytransform3d/rotations/_quaternion_operations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5201 2022-02-11 10:41:03.000000 pytransform3d-3.0.0/pytransform3d/rotations/_rotors.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5045 2022-03-23 10:33:20.000000 pytransform3d-3.0.0/pytransform3d/rotations/_slerp.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4236 2022-09-17 15:37:15.000000 pytransform3d-3.0.0/pytransform3d/rotations/_testing.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    16625 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/rotations/_utils.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    19380 2022-03-23 10:33:20.000000 pytransform3d-3.0.0/pytransform3d/trajectories.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    19804 2023-02-25 22:06:43.000000 pytransform3d-3.0.0/pytransform3d/transform_manager.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-03 19:22:44.607969 pytransform3d-3.0.0/pytransform3d/transformations/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3834 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/transformations/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    32226 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/transformations/_conversions.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5298 2022-03-15 09:35:04.000000 pytransform3d-3.0.0/pytransform3d/transformations/_dual_quaternion_operations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6006 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/transformations/_jacobians.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5945 2021-05-06 20:16:10.000000 pytransform3d-3.0.0/pytransform3d/transformations/_plot.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3489 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/transformations/_random.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6100 2023-02-11 16:37:10.000000 pytransform3d-3.0.0/pytransform3d/transformations/_testing.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7271 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/transformations/_transform_operations.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13510 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/transformations/_utils.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13302 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/uncertainty.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    28330 2022-12-22 19:37:52.000000 pytransform3d-3.0.0/pytransform3d/urdf.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-03 19:22:44.607969 pytransform3d-3.0.0/pytransform3d/visualizer/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      708 2023-02-11 17:57:50.000000 pytransform3d-3.0.0/pytransform3d/visualizer/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    37882 2022-12-22 19:37:52.000000 pytransform3d-3.0.0/pytransform3d/visualizer/_artists.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    23163 2023-04-03 19:11:52.000000 pytransform3d-3.0.0/pytransform3d/visualizer/_figure.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-03 19:22:44.603968 pytransform3d-3.0.0/pytransform3d.egg-info/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9417 2023-04-03 19:22:44.000000 pytransform3d-3.0.0/pytransform3d.egg-info/PKG-INFO
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1520 2023-04-03 19:22:44.000000 pytransform3d-3.0.0/pytransform3d.egg-info/SOURCES.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)        1 2023-04-03 19:22:44.000000 pytransform3d-3.0.0/pytransform3d.egg-info/dependency_links.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      158 2023-04-03 19:22:44.000000 pytransform3d-3.0.0/pytransform3d.egg-info/requires.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       14 2023-04-03 19:22:44.000000 pytransform3d-3.0.0/pytransform3d.egg-info/top_level.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      272 2023-04-03 19:22:44.607969 pytransform3d-3.0.0/setup.cfg
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1399 2023-02-11 16:37:10.000000 pytransform3d-3.0.0/setup.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.704778 pytransform3d-3.1.0/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1653 2023-01-12 22:48:31.000000 pytransform3d-3.1.0/LICENSE
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       58 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/MANIFEST.in
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9557 2023-04-14 18:51:49.704778 pytransform3d-3.1.0/PKG-INFO
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8884 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/README.md
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.696778 pytransform3d-3.1.0/pytransform3d/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       61 2023-04-14 18:46:28.000000 pytransform3d-3.1.0/pytransform3d/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21369 2022-09-17 15:37:15.000000 pytransform3d-3.1.0/pytransform3d/batch_rotations.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2257 2022-03-23 10:33:20.000000 pytransform3d-3.1.0/pytransform3d/batch_rotations.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    11534 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/camera.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1268 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/camera.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3898 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/coordinates.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      462 2021-08-07 17:17:14.000000 pytransform3d-3.1.0/pytransform3d/coordinates.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13372 2022-02-11 10:41:03.000000 pytransform3d-3.1.0/pytransform3d/editor.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.700778 pytransform3d-3.1.0/pytransform3d/plot_utils/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      829 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    10111 2022-12-22 19:37:52.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_artists.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1692 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_artists.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2606 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_layout.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      373 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_layout.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21851 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_plot_functions.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2656 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/plot_utils/_plot_functions.pyi
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.700778 pytransform3d-3.1.0/pytransform3d/rotations/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9185 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      407 2022-09-17 15:37:15.000000 pytransform3d-3.1.0/pytransform3d/rotations/_constants.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    62000 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/pytransform3d/rotations/_conversions.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7054 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/_conversions.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3444 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/_jacobians.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      356 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/_jacobians.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8686 2022-02-11 10:43:44.000000 pytransform3d-3.1.0/pytransform3d/rotations/_plot.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      683 2021-06-06 09:06:24.000000 pytransform3d-3.1.0/pytransform3d/rotations/_plot.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7380 2023-01-12 22:48:31.000000 pytransform3d-3.1.0/pytransform3d/rotations/_quaternion_operations.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      718 2023-01-12 22:48:31.000000 pytransform3d-3.1.0/pytransform3d/rotations/_quaternion_operations.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5201 2022-02-11 10:41:03.000000 pytransform3d-3.1.0/pytransform3d/rotations/_rotors.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      748 2021-06-06 09:06:24.000000 pytransform3d-3.1.0/pytransform3d/rotations/_rotors.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5045 2022-03-23 10:33:20.000000 pytransform3d-3.1.0/pytransform3d/rotations/_slerp.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      688 2022-03-23 10:33:20.000000 pytransform3d-3.1.0/pytransform3d/rotations/_slerp.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4236 2022-09-17 15:37:15.000000 pytransform3d-3.1.0/pytransform3d/rotations/_testing.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      393 2022-09-17 15:37:15.000000 pytransform3d-3.1.0/pytransform3d/rotations/_testing.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    16625 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/_utils.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1736 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/rotations/_utils.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    19380 2022-03-23 10:33:20.000000 pytransform3d-3.1.0/pytransform3d/trajectories.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1618 2022-03-23 10:33:20.000000 pytransform3d-3.1.0/pytransform3d/trajectories.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    19804 2023-02-25 22:06:43.000000 pytransform3d-3.1.0/pytransform3d/transform_manager.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2213 2023-02-11 16:37:10.000000 pytransform3d-3.1.0/pytransform3d/transform_manager.pyi
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.704778 pytransform3d-3.1.0/pytransform3d/transformations/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3834 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    32766 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/pytransform3d/transformations/_conversions.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2892 2021-05-23 13:02:30.000000 pytransform3d-3.1.0/pytransform3d/transformations/_conversions.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5298 2022-03-15 09:35:04.000000 pytransform3d-3.1.0/pytransform3d/transformations/_dual_quaternion_operations.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      517 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/transformations/_dual_quaternion_operations.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6006 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_jacobians.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      360 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_jacobians.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5945 2021-05-06 20:16:10.000000 pytransform3d-3.1.0/pytransform3d/transformations/_plot.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      632 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/transformations/_plot.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3489 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_random.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      406 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_random.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6100 2023-02-11 16:37:10.000000 pytransform3d-3.1.0/pytransform3d/transformations/_testing.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      509 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/transformations/_testing.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7271 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_transform_operations.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      952 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/transformations/_transform_operations.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13510 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/transformations/_utils.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      888 2021-05-11 07:46:15.000000 pytransform3d-3.1.0/pytransform3d/transformations/_utils.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    17158 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/pytransform3d/uncertainty.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1320 2023-04-14 18:46:22.000000 pytransform3d-3.1.0/pytransform3d/uncertainty.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    28330 2022-12-22 19:37:52.000000 pytransform3d-3.1.0/pytransform3d/urdf.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3345 2023-02-11 16:37:10.000000 pytransform3d-3.1.0/pytransform3d/urdf.pyi
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.704778 pytransform3d-3.1.0/pytransform3d/visualizer/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      708 2023-02-11 17:57:50.000000 pytransform3d-3.1.0/pytransform3d/visualizer/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    37882 2022-12-22 19:37:52.000000 pytransform3d-3.1.0/pytransform3d/visualizer/_artists.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5704 2023-02-11 17:57:50.000000 pytransform3d-3.1.0/pytransform3d/visualizer/_artists.pyi
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    23163 2023-04-03 19:11:52.000000 pytransform3d-3.1.0/pytransform3d/visualizer/_figure.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4235 2023-02-11 17:57:50.000000 pytransform3d-3.1.0/pytransform3d/visualizer/_figure.pyi
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-04-14 18:51:49.700778 pytransform3d-3.1.0/pytransform3d.egg-info/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9557 2023-04-14 18:51:49.000000 pytransform3d-3.1.0/pytransform3d.egg-info/PKG-INFO
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2620 2023-04-14 18:51:49.000000 pytransform3d-3.1.0/pytransform3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)        1 2023-04-14 18:51:49.000000 pytransform3d-3.1.0/pytransform3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      158 2023-04-14 18:51:49.000000 pytransform3d-3.1.0/pytransform3d.egg-info/requires.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       14 2023-04-14 18:51:49.000000 pytransform3d-3.1.0/pytransform3d.egg-info/top_level.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      272 2023-04-14 18:51:49.704778 pytransform3d-3.1.0/setup.cfg
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1399 2023-02-11 16:37:10.000000 pytransform3d-3.1.0/setup.py
```

### Comparing `pytransform3d-3.0.0/LICENSE` & `pytransform3d-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/PKG-INFO` & `pytransform3d-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytransform3d
-Version: 3.0.0
+Version: 3.1.0
 Summary: 3D transformations for Python
 Home-page: https://github.com/dfki-ric/pytransform3d
 Author: Alexander Fabisch
 Author-email: afabisch@googlemail.com
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,17 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
-[![CircleCI Status](https://circleci.com/gh/dfki-ric/pytransform3d/tree/master.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/dfki-ric/pytransform3d)
+<img src="https://raw.githubusercontent.com/dfki-ric/pytransform3d/master/doc/source/_static/logo.png" />
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/dfki-ric/pytransform3d/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/dfki-ric/pytransform3d/tree/master)
 [![codecov](https://codecov.io/gh/dfki-ric/pytransform3d/branch/master/graph/badge.svg?token=jB10RM3Ujj)](https://codecov.io/gh/dfki-ric/pytransform3d)
 [![Paper DOI](http://joss.theoj.org/papers/10.21105/joss.01159/status.svg)](https://doi.org/10.21105/joss.01159)
 [![Release DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2553450.svg)](https://doi.org/10.5281/zenodo.2553450)
 
 # pytransform3d
 
 A Python library for transformations in three dimensions.
@@ -133,15 +135,15 @@
 ax = tm.plot_frames_in("robot", s=0.1)
 ax.set_xlim((-0.25, 0.75))
 ax.set_ylim((-0.5, 0.5))
 ax.set_zlim((0.0, 1.0))
 plt.show()
 ```
 
-![output](https://dfki-ric.github.io/pytransform3d/_images/plot_transform_manager.png)
+![output](https://dfki-ric.github.io/pytransform3d/_images/sphx_glr_plot_transform_manager_001.png)
 
 ## Documentation
 
 The API documentation can be found
 [here](https://dfki-ric.github.io/pytransform3d/).
 
 The documentation can be found in the directory `doc`.
```

### Comparing `pytransform3d-3.0.0/README.md` & `pytransform3d-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-[![CircleCI Status](https://circleci.com/gh/dfki-ric/pytransform3d/tree/master.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/dfki-ric/pytransform3d)
+<img src="https://raw.githubusercontent.com/dfki-ric/pytransform3d/master/doc/source/_static/logo.png" />
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/dfki-ric/pytransform3d/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/dfki-ric/pytransform3d/tree/master)
 [![codecov](https://codecov.io/gh/dfki-ric/pytransform3d/branch/master/graph/badge.svg?token=jB10RM3Ujj)](https://codecov.io/gh/dfki-ric/pytransform3d)
 [![Paper DOI](http://joss.theoj.org/papers/10.21105/joss.01159/status.svg)](https://doi.org/10.21105/joss.01159)
 [![Release DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2553450.svg)](https://doi.org/10.5281/zenodo.2553450)
 
 # pytransform3d
 
 A Python library for transformations in three dimensions.
@@ -113,15 +115,15 @@
 ax = tm.plot_frames_in("robot", s=0.1)
 ax.set_xlim((-0.25, 0.75))
 ax.set_ylim((-0.5, 0.5))
 ax.set_zlim((0.0, 1.0))
 plt.show()
 ```
 
-![output](https://dfki-ric.github.io/pytransform3d/_images/plot_transform_manager.png)
+![output](https://dfki-ric.github.io/pytransform3d/_images/sphx_glr_plot_transform_manager_001.png)
 
 ## Documentation
 
 The API documentation can be found
 [here](https://dfki-ric.github.io/pytransform3d/).
 
 The documentation can be found in the directory `doc`.
```

### Comparing `pytransform3d-3.0.0/pytransform3d/batch_rotations.py` & `pytransform3d-3.1.0/pytransform3d/batch_rotations.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/camera.py` & `pytransform3d-3.1.0/pytransform3d/camera.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/coordinates.py` & `pytransform3d-3.1.0/pytransform3d/coordinates.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/editor.py` & `pytransform3d-3.1.0/pytransform3d/editor.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/plot_utils/__init__.py` & `pytransform3d-3.1.0/pytransform3d/plot_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/plot_utils/_artists.py` & `pytransform3d-3.1.0/pytransform3d/plot_utils/_artists.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/plot_utils/_layout.py` & `pytransform3d-3.1.0/pytransform3d/plot_utils/_layout.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/plot_utils/_plot_functions.py` & `pytransform3d-3.1.0/pytransform3d/plot_utils/_plot_functions.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/rotations/__init__.py` & `pytransform3d-3.1.0/pytransform3d/rotations/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/rotations/_conversions.py` & `pytransform3d-3.1.0/pytransform3d/rotations/_conversions.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,23 @@
         \boldsymbol{w}.
 
     It is a skew-symmetric (antisymmetric) matrix, i.e.,
     :math:`-\boldsymbol{V} = \boldsymbol{V}^T`. Its elements are
 
     .. math::
 
-        \boldsymbol{V} = \left(\begin{array}{ccc}
+        \left[\boldsymbol{v}\right]
+        =
+        \left[\begin{array}{c}
+        v_1\\ v_2\\ v_3
+        \end{array}\right]
+        =
+        \boldsymbol{V}
+        =
+        \left(\begin{array}{ccc}
         0 & -v_3 & v_2\\
         v_3 & 0 & -v_1\\
         -v_2 & v_1 & 0
         \end{array}\right).
 
     Parameters
     ----------
```

### Comparing `pytransform3d-3.0.0/pytransform3d/rotations/_jacobians.py` & `pytransform3d-3.1.0/pytransform3d/rotations/_jacobians.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/rotations/_plot.py` & `pytransform3d-3.1.0/pytransform3d/rotations/_plot.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/rotations/_quaternion_operations.py` & `pytransform3d-3.1.0/pytransform3d/rotations/_quaternion_operations.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/rotations/_rotors.py` & `pytransform3d-3.1.0/pytransform3d/rotations/_rotors.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/rotations/_slerp.py` & `pytransform3d-3.1.0/pytransform3d/rotations/_slerp.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/rotations/_testing.py` & `pytransform3d-3.1.0/pytransform3d/rotations/_testing.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/rotations/_utils.py` & `pytransform3d-3.1.0/pytransform3d/rotations/_utils.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/trajectories.py` & `pytransform3d-3.1.0/pytransform3d/trajectories.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/transform_manager.py` & `pytransform3d-3.1.0/pytransform3d/transform_manager.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/transformations/__init__.py` & `pytransform3d-3.1.0/pytransform3d/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/transformations/_conversions.py` & `pytransform3d-3.1.0/pytransform3d/transformations/_conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,16 +319,16 @@
     return screw_axis * theta
 
 
 def exponential_coordinates_from_transform_log(transform_log, check=True):
     r"""Compute exponential coordinates from logarithm of transformation.
 
     Extracts the vector :math:`\mathcal{S} \theta =
-    (\boldsymbol{\omega}, \boldsymbol{v}) \theta \in \mathbb{R}^6` from the
-    matrix
+    (\hat{\boldsymbol{\omega}}, \boldsymbol{v}) \theta \in \mathbb{R}^6` from
+    the matrix
 
     .. math::
 
         \left(
         \begin{array}{cccc}
         0 & -\omega_3 & \omega_2 & v_1\\
         \omega_3 & 0 & -\omega_1 & v_2\\
@@ -384,38 +384,31 @@
         \boldsymbol{R} & \boldsymbol{p}\\
         \boldsymbol{0} & 1
         \end{array}
         \right)
         =
         \left(
         \begin{array}{c}
-        Log\boldsymbol{R}\\
-        \boldsymbol{G}^{-1}(\theta) \boldsymbol{p}
+        Log(\boldsymbol{R})\\
+        \boldsymbol{J}^{-1}(\theta) \boldsymbol{p}
         \end{array}
         \right)
         =
         \left(
         \begin{array}{c}
-        \boldsymbol{\omega}\\
+        \hat{\boldsymbol{\omega}}\\
         \boldsymbol{v}
         \end{array}
         \right)
         \theta
         =
         \mathcal{S}\theta,
 
-    where
-
-    .. math::
-
-        \boldsymbol{G}^{-1}(\theta)
-        = \boldsymbol{I} \frac{1}{\theta}
-        + \frac{1}{2} [\boldsymbol{\omega}]
-        + (\frac{1}{\theta} - \frac{1}{2 \tan \frac{\theta}{2}})
-        [\boldsymbol{\omega}]^2.
+    where :math:`\boldsymbol{J}^{-1}(\theta)` is the inverse left Jacobian of
+    :math:`SO(3)` (see :func:`~pytransform3d.rotations.left_jacobian_SO3_inv`).
 
     Parameters
     ----------
     A2B : array-like, shape (4, 4)
         Transformation matrix from frame A to frame B
 
     strict_check : bool, optional (default: True)
@@ -446,17 +439,17 @@
 
     omega_theta = compact_axis_angle_from_matrix(R, check=check)
     theta = np.linalg.norm(omega_theta)
 
     if theta == 0:
         return np.r_[0.0, 0.0, 0.0, p]
 
-    v = np.dot(left_jacobian_SO3_inv(omega_theta), p)
+    v_theta = np.dot(left_jacobian_SO3_inv(omega_theta), p)
 
-    return np.hstack((omega_theta, v))
+    return np.hstack((omega_theta, v_theta))
 
 
 def screw_matrix_from_screw_axis(screw_axis):
     """Compute screw matrix from screw axis.
 
     Parameters
     ----------
@@ -521,15 +514,15 @@
         \omega_3 & 0 & -\omega_1 & v_2\\
         -\omega_2 & \omega_1 & 0 & v_3\\
         0 & 0 & 0 & 0
         \end{array}
         \right) \theta
         = \left[ \mathcal{S} \right] \theta \in so(3)
 
-    from the vector :math:`\mathcal{S} \theta = (\boldsymbol{\omega},
+    from the vector :math:`\mathcal{S} \theta = (\hat{\boldsymbol{\omega}},
     \boldsymbol{v}) \theta \in \mathbb{R}^6`.
 
     Parameters
     ----------
     Stheta : array-like, shape (6,)
         Exponential coordinates of transformation:
         S * theta = (omega_1, omega_2, omega_3, v_1, v_2, v_3) * theta,
@@ -592,38 +585,31 @@
         \boldsymbol{R} & \boldsymbol{p}\\
         \boldsymbol{0} & 1
         \end{array}
         \right)
         =
         \left(
         \begin{array}{cc}
-        \log\boldsymbol{R} & \boldsymbol{G}^{-1}(\theta) \boldsymbol{p}\\
+        \log\boldsymbol{R} & \boldsymbol{J}^{-1}(\theta) \boldsymbol{p}\\
         \boldsymbol{0} & 0
         \end{array}
         \right)
         =
         \left(
         \begin{array}{cc}
-        \hat{\boldsymbol{\omega}}\theta
-        & \boldsymbol{G}^{-1}(\theta) \boldsymbol{p}\\
+        \hat{\boldsymbol{\omega}} \theta
+        & \boldsymbol{v} \theta\\
         \boldsymbol{0} & 0
         \end{array}
         \right)
         =
         \left[\mathcal{S}\right]\theta,
 
-    where
-
-    .. math::
-
-        \boldsymbol{G}^{-1}(\theta)
-        = \boldsymbol{I} \frac{1}{\theta}
-        + \frac{1}{2} [\boldsymbol{\omega}]
-        + (\frac{1}{\theta} - \frac{1}{2 \tan \frac{\theta}{2}})
-        [\boldsymbol{\omega}]^2.
+    where :math:`\boldsymbol{J}^{-1}(\theta)` is the inverse left Jacobian of
+    :math:`SO(3)` (see :func:`~pytransform3d.rotations.left_jacobian_SO3_inv`).
 
     Parameters
     ----------
     A2B : array, shape (4, 4)
         Transform from frame A to frame B
 
     strict_check : bool, optional (default: True)
@@ -650,18 +636,18 @@
     omega_theta = compact_axis_angle_from_matrix(R)
     theta = np.linalg.norm(omega_theta)
 
     if theta == 0:
         return transform_log
 
     J_inv = left_jacobian_SO3_inv(omega_theta)
-    v = np.dot(J_inv, p)
+    v_theta = np.dot(J_inv, p)
 
     transform_log[:3, :3] = cross_product_matrix(omega_theta)
-    transform_log[:3, 3] = v
+    transform_log[:3, 3] = v_theta
 
     return transform_log
 
 
 def transform_from_exponential_coordinates(Stheta, check=True):
     r"""Compute transformation matrix from exponential coordinates.
 
@@ -672,33 +658,28 @@
         Exp: \mathcal{S} \theta \in \mathbb{R}^6
         \rightarrow \boldsymbol{T} \in SE(3)
 
     .. math::
 
         Exp(\mathcal{S}\theta) =
         Exp\left(\left(\begin{array}{c}
-        \boldsymbol{\omega}\\
+        \hat{\boldsymbol{\omega}}\\
         \boldsymbol{v}
         \end{array}\right)\theta\right)
         =
         \exp(\left[\mathcal{S}\right] \theta)
         =
         \left(\begin{array}{cc}
-        Exp(\boldsymbol{\omega}) & \boldsymbol{G}(\theta)\boldsymbol{v}\\
+        Exp(\hat{\boldsymbol{\omega}} \theta) &
+        \boldsymbol{J}(\theta)\boldsymbol{v}\theta\\
         \boldsymbol{0} & 1
         \end{array}\right),
 
-    where
-
-    .. math::
-
-        \boldsymbol{G}(\theta)
-        = \boldsymbol{I}\theta
-        + (1 - \cos \theta) [\boldsymbol{\omega}]
-        + (\theta - \sin \theta) [\boldsymbol{\omega}]^2.
+    where :math:`\boldsymbol{J}(\theta)` is the left Jacobian of :math:`SO(3)`
+    (see :func:`~pytransform3d.rotations.left_jacobian_SO3`).
 
     Parameters
     ----------
     Stheta : array-like, shape (6,)
         Exponential coordinates of transformation:
         S * theta = (omega_1, omega_2, omega_3, v_1, v_2, v_3) * theta,
         where S is the screw axis, the first 3 components are related to
@@ -718,21 +699,21 @@
 
     omega_theta = Stheta[:3]
     theta = np.linalg.norm(omega_theta)
 
     if theta == 0.0:  # only translation
         return translate_transform(np.eye(4), Stheta[3:], check=check)
 
-    omega = Stheta[:3]
-    v = Stheta[3:]
+    omega_theta = Stheta[:3]
+    v_theta = Stheta[3:]
 
     A2B = np.eye(4)
-    A2B[:3, :3] = matrix_from_compact_axis_angle(omega)
-    J = left_jacobian_SO3(omega)
-    A2B[:3, 3] = np.dot(J, v)
+    A2B[:3, :3] = matrix_from_compact_axis_angle(omega_theta)
+    J = left_jacobian_SO3(omega_theta)
+    A2B[:3, 3] = np.dot(J, v_theta)
     return A2B
 
 
 def transform_from_transform_log(transform_log):
     r"""Compute transformation from matrix logarithm of transformation.
 
     Exponential map.
@@ -742,30 +723,25 @@
         \exp: \left[ \mathcal{S} \right] \theta \in se(3)
         \rightarrow \boldsymbol{T} \in SE(3)
 
     .. math::
 
         \exp([\mathcal{S}]\theta) =
         \exp\left(\left(\begin{array}{cc}
-        \left[\boldsymbol{\omega}\right] & \boldsymbol{v}\\
+        \left[\hat{\boldsymbol{\omega}}\right] & \boldsymbol{v}\\
         \boldsymbol{0} & 0
         \end{array}\right)\theta\right) =
         \left(\begin{array}{cc}
-        Exp(\boldsymbol{\omega}) & \boldsymbol{G}(\theta)\boldsymbol{v}\\
+        Exp(\hat{\boldsymbol{\omega}} \theta) &
+        \boldsymbol{J}(\theta)\boldsymbol{v}\theta\\
         \boldsymbol{0} & 1
         \end{array}\right),
 
-    where
-
-    .. math::
-
-        \boldsymbol{G}(\theta)
-        = \boldsymbol{I}\theta
-        + (1 - \cos \theta) [\boldsymbol{\omega}]
-        + (\theta - \sin \theta) [\boldsymbol{\omega}]^2.
+    where :math:`\boldsymbol{J}(\theta)` is the left Jacobian of :math:`SO(3)`
+    (see :func:`~pytransform3d.rotations.left_jacobian_SO3`).
 
     Parameters
     ----------
     transform_log : array-like, shape (4, 4)
         Matrix logarithm of transformation matrix: [S] * theta.
 
     Returns
@@ -773,24 +749,24 @@
     A2B : array, shape (4, 4)
         Transform from frame A to frame B
     """
     transform_log = check_transform_log(transform_log)
 
     omega_theta = np.array([
         transform_log[2, 1], transform_log[0, 2], transform_log[1, 0]])
-    v = transform_log[:3, 3]
+    v_theta = transform_log[:3, 3]
     theta = np.linalg.norm(omega_theta)
 
     if theta == 0.0:  # only translation
-        return translate_transform(np.eye(4), v)
+        return translate_transform(np.eye(4), v_theta)
 
     A2B = np.eye(4)
     A2B[:3, :3] = matrix_from_compact_axis_angle(omega_theta)
     J = left_jacobian_SO3(omega_theta)
-    A2B[:3, 3] = np.dot(J, v)
+    A2B[:3, 3] = np.dot(J, v_theta)
     return A2B
 
 
 def dual_quaternion_from_transform(A2B):
     """Compute dual quaternion from transformation matrix.
 
     Parameters
@@ -975,57 +951,82 @@
                     / np.tan(0.5 * theta))
     dual = np.cross(s_axis, moment)
     h = distance / theta
     return dual, s_axis, h, theta
 
 
 def adjoint_from_transform(A2B, strict_check=True, check=True):
-    """Compute adjoint representation of a transformation matrix.
+    r"""Compute adjoint representation of a transformation matrix.
 
     The adjoint representation of a transformation
-    :math:`\\left[Ad_{\\boldsymbol{T}_{BA}}\\right]`
+    :math:`\left[Ad_{\boldsymbol{T}_{BA}}\right] \in \mathbb{R}^{6 \times 6}`
     from frame A to frame B translates a twist from frame A to frame B
     through the adjoint map
 
     .. math::
 
-        \\mathcal{V}_{B}
-        = \\left[Ad_{\\boldsymbol{T}_{BA}}\\right] \\mathcal{V}_A
+        \mathcal{V}_{B}
+        = \left[Ad_{\boldsymbol{T}_{BA}}\right] \mathcal{V}_A
 
-    The corresponding matrix form is
+    The corresponding transformation matrix operation is
 
     .. math::
 
-        \\left[\\mathcal{V}_{B}\\right]
-        = \\boldsymbol{T}_{BA} \\left[\\mathcal{V}_A\\right]
-        \\boldsymbol{T}_{BA}^{-1}
+        \left[\mathcal{V}_{B}\right]
+        = \boldsymbol{T}_{BA} \left[\mathcal{V}_A\right]
+        \boldsymbol{T}_{BA}^{-1}
 
     We can also use the adjoint representation to transform a wrench from frame
     A to frame B:
 
     .. math::
 
-        \\mathcal{F}_B
-        = \\left[ Ad_{\\boldsymbol{T}_{AB}} \\right]^T \\mathcal{F}_A
+        \mathcal{F}_B
+        = \left[ Ad_{\boldsymbol{T}_{AB}} \right]^T \mathcal{F}_A
 
     Note that not only the adjoint is transposed but also the transformation is
     inverted.
 
     Adjoint representations have the following properties:
 
     .. math::
 
-        \\left[Ad_{\\boldsymbol{T}_1 \\boldsymbol{T}_2}\\right]
-        = \\left[Ad_{\\boldsymbol{T}_1}\\right]
-        \\left[Ad_{\\boldsymbol{T}_2}\\right]
+        \left[Ad_{\boldsymbol{T}_1 \boldsymbol{T}_2}\right]
+        = \left[Ad_{\boldsymbol{T}_1}\right]
+        \left[Ad_{\boldsymbol{T}_2}\right]
 
     .. math::
 
-        \\left[Ad_{\\boldsymbol{T}}\\right]^{-1} =
-        \\left[Ad_{\\boldsymbol{T}^{-1}}\\right]
+        \left[Ad_{\boldsymbol{T}}\right]^{-1} =
+        \left[Ad_{\boldsymbol{T}^{-1}}\right]
+
+    For a transformation matrix
+
+    .. math::
+
+        \boldsymbol T =
+        \left( \begin{array}{cc}
+            \boldsymbol R & \boldsymbol t\\
+            \boldsymbol 0 & 1\\
+        \end{array} \right)
+
+    the adjoint is defined as
+
+    .. math::
+
+        \left[Ad_{\boldsymbol{T}}\right]
+        =
+        \left( \begin{array}{cc}
+            \boldsymbol R & \boldsymbol 0\\
+            \left[\boldsymbol{t}\right]_{\times}\boldsymbol R & \boldsymbol R\\
+        \end{array} \right),
+
+    where :math:`\left[\boldsymbol{t}\right]_{\times}` is the cross-product
+    matrix (see :func:`~pytransform3d.rotations.cross_product_matrix`) of the
+    translation component.
 
     Parameters
     ----------
     A2B : array-like, shape (4, 4)
         Transform from frame A to frame B
 
     strict_check : bool, optional (default: True)
```

### Comparing `pytransform3d-3.0.0/pytransform3d/transformations/_dual_quaternion_operations.py` & `pytransform3d-3.1.0/pytransform3d/transformations/_dual_quaternion_operations.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/transformations/_jacobians.py` & `pytransform3d-3.1.0/pytransform3d/transformations/_jacobians.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/transformations/_plot.py` & `pytransform3d-3.1.0/pytransform3d/transformations/_plot.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/transformations/_random.py` & `pytransform3d-3.1.0/pytransform3d/transformations/_random.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/transformations/_testing.py` & `pytransform3d-3.1.0/pytransform3d/transformations/_testing.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/transformations/_transform_operations.py` & `pytransform3d-3.1.0/pytransform3d/transformations/_transform_operations.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/transformations/_utils.py` & `pytransform3d-3.1.0/pytransform3d/transformations/_utils.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/uncertainty.py` & `pytransform3d-3.1.0/pytransform3d/uncertainty.py`

 * *Files 13% similar despite different names*

```diff
@@ -112,41 +112,57 @@
     of transformations and are distributed according to a Gaussian
     distribution with zero mean and covariance :math:`\boldsymbol{\Sigma} \in
     \mathbb{R}^{6 \times 6}`, that is, :math:`\boldsymbol{\xi} \sim
     \mathcal{N}(\boldsymbol{0}, \boldsymbol{\Sigma})`.
 
     The concatenation order is the same as in
     :func:`~pytransform3d.transformations.concat`, that is, the transformation
-    B2C is left-multiplied to A2B.
+    B2C is left-multiplied to A2B. Note that the order of arguments is
+    different from
+    :func:`~pytransform3d.uncertainty.concat_locally_uncertain_transforms`.
+
+    Hence, the full model is
+
+    .. math::
+
+        Exp(_C\boldsymbol{\xi'}) \overline{\boldsymbol{T}}_{CA} =
+        Exp(_C\boldsymbol{\xi}) \overline{\boldsymbol{T}}_{CB}
+        Exp(_B\boldsymbol{\xi}) \overline{\boldsymbol{T}}_{BA},
+
+    where :math:`_B\boldsymbol{\xi} \sim \mathcal{N}(\boldsymbol{0},
+    \boldsymbol{\Sigma}_{BA})`, :math:`_C\boldsymbol{\xi} \sim
+    \mathcal{N}(\boldsymbol{0}, \boldsymbol{\Sigma}_{CB})`, and
+    :math:`_C\boldsymbol{\xi'} \sim \mathcal{N}(\boldsymbol{0},
+    \boldsymbol{\Sigma}_{CA})`.
 
     This version of Barfoot and Furgale approximates the covariance up to
     4th-order terms. Note that it is still an approximation of the covariance
     after concatenation of the two transforms.
 
     Parameters
     ----------
     mean_A2B : array, shape (4, 4)
         Mean of transform from A to B.
 
     cov_A2B : array, shape (6, 6)
-        Covariance of transform from A to B.
+        Covariance of transform from A to B. Models uncertainty in frame B.
 
     mean_B2C : array, shape (4, 4)
         Mean of transform from B to C.
 
     cov_B2C : array, shape (6, 6)
-        Covariance of transform from B to C.
+        Covariance of transform from B to C. Models uncertainty in frame C.
 
     Returns
     -------
     mean_A2C : array, shape (4, 4)
         Mean of new pose.
 
     cov_A2C : array, shape (6, 6)
-        Covariance of new pose.
+        Covariance of new pose. Models uncertainty in frame C.
 
     References
     ----------
     Barfoot, Furgale: Associating Uncertainty With Three-Dimensional Poses for
     Use in Estimation Problems,
     http://ncfrn.mcgill.ca/members/pubs/barfoot_tro14.pdf
     """
@@ -209,14 +225,96 @@
     return -np.trace(A) * np.eye(len(A)) + A
 
 
 def _covop2(A, B):
     return np.dot(_covop1(A), _covop1(B)) + _covop1(np.dot(B, A))
 
 
+def concat_locally_uncertain_transforms(mean_A2B, mean_B2C, cov_A, cov_B):
+    r"""Concatenate two independent locally uncertain transformations.
+
+    We assume that the two distributions are independent.
+
+    Each of the two transformations is locally uncertain (not in the global /
+    world frame), that is, samples are generated through
+
+    .. math::
+
+        \boldsymbol{T} = \overline{\boldsymbol{T}} Exp(\boldsymbol{\xi}),
+
+    where :math:`\boldsymbol{T} \in SE(3)` is a sampled transformation matrix,
+    :math:`\overline{\boldsymbol{T}} \in SE(3)` is the mean transformation,
+    and :math:`\boldsymbol{\xi} \in \mathbb{R}^6` are exponential coordinates
+    of transformations and are distributed according to a Gaussian
+    distribution with zero mean and covariance :math:`\boldsymbol{\Sigma} \in
+    \mathbb{R}^{6 \times 6}`, that is, :math:`\boldsymbol{\xi} \sim
+    \mathcal{N}(\boldsymbol{0}, \boldsymbol{\Sigma})`.
+
+    The concatenation order is the same as in
+    :func:`~pytransform3d.transformations.concat`, that is, the transformation
+    B2C is left-multiplied to A2B. Note that the order of arguments is
+    different from
+    :func:`~pytransform3d.uncertainty.concat_globally_uncertain_transforms`.
+
+    Hence, the full model is
+
+    .. math::
+
+        \overline{\boldsymbol{T}}_{CA} Exp(_A\boldsymbol{\xi'}) =
+        \overline{\boldsymbol{T}}_{CB} Exp(_B\boldsymbol{\xi})
+        \overline{\boldsymbol{T}}_{BA} Exp(_A\boldsymbol{\xi}),
+
+    where :math:`_B\boldsymbol{\xi} \sim \mathcal{N}(\boldsymbol{0},
+    \boldsymbol{\Sigma}_B)`, :math:`_A\boldsymbol{\xi} \sim
+    \mathcal{N}(\boldsymbol{0}, \boldsymbol{\Sigma}_A)`, and
+    :math:`_A\boldsymbol{\xi'} \sim \mathcal{N}(\boldsymbol{0},
+    \boldsymbol{\Sigma}_{A,total})`.
+
+    This version of Meyer et al. approximates the covariance up to 2nd-order
+    terms.
+
+    Parameters
+    ----------
+    mean_A2B : array, shape (4, 4)
+        Mean of transform from A to B: :math:`\overline{\boldsymbol{T}}_{BA}`.
+
+    mean_B2C : array, shape (4, 4)
+        Mean of transform from B to C: :math:`\overline{\boldsymbol{T}}_{CB}`.
+
+    cov_A : array, shape (6, 6)
+        Covariance of noise in frame A: :math:`\boldsymbol{\Sigma}_A`. Noise
+        samples are right-multiplied with the mean transform A2B.
+
+    cov_B : array, shape (6, 6)
+        Covariance of noise in frame B: :math:`\boldsymbol{\Sigma}_B`. Noise
+        samples are right-multiplied with the mean transform B2C.
+
+    Returns
+    -------
+    mean_A2C : array, shape (4, 4)
+        Mean of new pose.
+
+    cov_A_total : array, shape (6, 6)
+        Covariance of accumulated noise in frame A.
+
+    References
+    ----------
+    Meyer, Strobl, Triebel: The Probabilistic Robot Kinematics Model and its
+    Application to Sensor Fusion,
+    https://elib.dlr.de/191928/1/202212_ELIB_PAPER_VERSION_with_copyright.pdf
+    """
+    mean_A2C = concat(mean_A2B, mean_B2C)
+
+    ad_B2A = adjoint_from_transform(invert_transform(mean_A2B))
+    cov_B_in_A = np.dot(ad_B2A, np.dot(cov_B, ad_B2A.T))
+    cov_A_total = cov_B_in_A + cov_A
+
+    return mean_A2C, cov_A_total
+
+
 def pose_fusion(means, covs):
     """Fuse Gaussian distributions of multiple poses.
 
     Parameters
     ----------
     means : array-like, shape (n_poses, 4, 4)
         Homogeneous transformation matrices.
@@ -346,18 +444,18 @@
         Coordinates on z-axis of grid on projected ellipsoid.
     """
     from scipy import linalg
     vals, vecs = linalg.eigh(cov)
     order = vals.argsort()[::-1]
     vals, vecs = vals[order], vecs[:, order]
 
-    radii = factor * np.sqrt(vals)
+    radii = factor * np.sqrt(vals[:3])
 
     # Grid on ellipsoid in exponential coordinate space
-    radius_x, radius_y, radius_z = radii[:3]
+    radius_x, radius_y, radius_z = radii
     phi, theta = np.mgrid[0.0:np.pi:n_steps * 1j, 0.0:2.0 * np.pi:n_steps * 1j]
     x = radius_x * np.sin(phi) * np.cos(theta)
     y = radius_y * np.sin(phi) * np.sin(theta)
     z = radius_z * np.cos(phi)
     P = np.column_stack((x.reshape(-1), y.reshape(-1), z.reshape(-1)))
     P = np.dot(P, vecs[:, :3].T)
```

### Comparing `pytransform3d-3.0.0/pytransform3d/urdf.py` & `pytransform3d-3.1.0/pytransform3d/urdf.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/visualizer/__init__.py` & `pytransform3d-3.1.0/pytransform3d/visualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/visualizer/_artists.py` & `pytransform3d-3.1.0/pytransform3d/visualizer/_artists.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d/visualizer/_figure.py` & `pytransform3d-3.1.0/pytransform3d/visualizer/_figure.py`

 * *Files identical despite different names*

### Comparing `pytransform3d-3.0.0/pytransform3d.egg-info/PKG-INFO` & `pytransform3d-3.1.0/pytransform3d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytransform3d
-Version: 3.0.0
+Version: 3.1.0
 Summary: 3D transformations for Python
 Home-page: https://github.com/dfki-ric/pytransform3d
 Author: Alexander Fabisch
 Author-email: afabisch@googlemail.com
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,17 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: test
 License-File: LICENSE
 
-[![CircleCI Status](https://circleci.com/gh/dfki-ric/pytransform3d/tree/master.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/dfki-ric/pytransform3d)
+<img src="https://raw.githubusercontent.com/dfki-ric/pytransform3d/master/doc/source/_static/logo.png" />
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/dfki-ric/pytransform3d/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/dfki-ric/pytransform3d/tree/master)
 [![codecov](https://codecov.io/gh/dfki-ric/pytransform3d/branch/master/graph/badge.svg?token=jB10RM3Ujj)](https://codecov.io/gh/dfki-ric/pytransform3d)
 [![Paper DOI](http://joss.theoj.org/papers/10.21105/joss.01159/status.svg)](https://doi.org/10.21105/joss.01159)
 [![Release DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2553450.svg)](https://doi.org/10.5281/zenodo.2553450)
 
 # pytransform3d
 
 A Python library for transformations in three dimensions.
@@ -133,15 +135,15 @@
 ax = tm.plot_frames_in("robot", s=0.1)
 ax.set_xlim((-0.25, 0.75))
 ax.set_ylim((-0.5, 0.5))
 ax.set_zlim((0.0, 1.0))
 plt.show()
 ```
 
-![output](https://dfki-ric.github.io/pytransform3d/_images/plot_transform_manager.png)
+![output](https://dfki-ric.github.io/pytransform3d/_images/sphx_glr_plot_transform_manager_001.png)
 
 ## Documentation
 
 The API documentation can be found
 [here](https://dfki-ric.github.io/pytransform3d/).
 
 The documentation can be found in the directory `doc`.
```

### Comparing `pytransform3d-3.0.0/pytransform3d.egg-info/SOURCES.txt` & `pytransform3d-3.1.0/pytransform3d.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,73 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
 pytransform3d/__init__.py
 pytransform3d/batch_rotations.py
+pytransform3d/batch_rotations.pyi
 pytransform3d/camera.py
+pytransform3d/camera.pyi
 pytransform3d/coordinates.py
+pytransform3d/coordinates.pyi
 pytransform3d/editor.py
 pytransform3d/trajectories.py
+pytransform3d/trajectories.pyi
 pytransform3d/transform_manager.py
+pytransform3d/transform_manager.pyi
 pytransform3d/uncertainty.py
+pytransform3d/uncertainty.pyi
 pytransform3d/urdf.py
+pytransform3d/urdf.pyi
 pytransform3d.egg-info/PKG-INFO
 pytransform3d.egg-info/SOURCES.txt
 pytransform3d.egg-info/dependency_links.txt
 pytransform3d.egg-info/requires.txt
 pytransform3d.egg-info/top_level.txt
 pytransform3d/plot_utils/__init__.py
 pytransform3d/plot_utils/_artists.py
+pytransform3d/plot_utils/_artists.pyi
 pytransform3d/plot_utils/_layout.py
+pytransform3d/plot_utils/_layout.pyi
 pytransform3d/plot_utils/_plot_functions.py
+pytransform3d/plot_utils/_plot_functions.pyi
 pytransform3d/rotations/__init__.py
 pytransform3d/rotations/_constants.py
 pytransform3d/rotations/_conversions.py
+pytransform3d/rotations/_conversions.pyi
 pytransform3d/rotations/_jacobians.py
+pytransform3d/rotations/_jacobians.pyi
 pytransform3d/rotations/_plot.py
+pytransform3d/rotations/_plot.pyi
 pytransform3d/rotations/_quaternion_operations.py
+pytransform3d/rotations/_quaternion_operations.pyi
 pytransform3d/rotations/_rotors.py
+pytransform3d/rotations/_rotors.pyi
 pytransform3d/rotations/_slerp.py
+pytransform3d/rotations/_slerp.pyi
 pytransform3d/rotations/_testing.py
+pytransform3d/rotations/_testing.pyi
 pytransform3d/rotations/_utils.py
+pytransform3d/rotations/_utils.pyi
 pytransform3d/transformations/__init__.py
 pytransform3d/transformations/_conversions.py
+pytransform3d/transformations/_conversions.pyi
 pytransform3d/transformations/_dual_quaternion_operations.py
+pytransform3d/transformations/_dual_quaternion_operations.pyi
 pytransform3d/transformations/_jacobians.py
+pytransform3d/transformations/_jacobians.pyi
 pytransform3d/transformations/_plot.py
+pytransform3d/transformations/_plot.pyi
 pytransform3d/transformations/_random.py
+pytransform3d/transformations/_random.pyi
 pytransform3d/transformations/_testing.py
+pytransform3d/transformations/_testing.pyi
 pytransform3d/transformations/_transform_operations.py
+pytransform3d/transformations/_transform_operations.pyi
 pytransform3d/transformations/_utils.py
+pytransform3d/transformations/_utils.pyi
 pytransform3d/visualizer/__init__.py
 pytransform3d/visualizer/_artists.py
-pytransform3d/visualizer/_figure.py
+pytransform3d/visualizer/_artists.pyi
+pytransform3d/visualizer/_figure.py
+pytransform3d/visualizer/_figure.pyi
```

### Comparing `pytransform3d-3.0.0/setup.py` & `pytransform3d-3.1.0/setup.py`

 * *Files identical despite different names*

