# Comparing `tmp/teneva-0.9.8.tar.gz` & `tmp/teneva-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva-0.9.8.tar", last modified: Sun Jul  3 12:30:35 2022, max compression
+gzip compressed data, was "teneva-0.9.9.tar", last modified: Sun Jul  3 14:09:05 2022, max compression
```

## Comparing `teneva-0.9.8.tar` & `teneva-0.9.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 12:30:35.003395 teneva-0.9.8/
--rw-r--r--   0 andrei     (501) staff       (20)     1095 2022-01-01 12:16:24.000000 teneva-0.9.8/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       63 2022-02-22 08:40:27.000000 teneva-0.9.8/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     3619 2022-07-03 12:30:35.003593 teneva-0.9.8/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1992 2022-03-13 14:41:05.000000 teneva-0.9.8/README.md
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 12:30:34.980868 teneva-0.9.8/demo/
--rw-r--r--   0 andrei     (501) staff       (20)     6148 2022-07-01 16:04:08.000000 teneva-0.9.8/demo/.DS_Store
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 12:30:34.988581 teneva-0.9.8/demo/.ipynb_checkpoints/
--rw-r--r--   0 andrei     (501) staff       (20)     4130 2022-06-21 08:33:45.000000 teneva-0.9.8/demo/.ipynb_checkpoints/2d_cross_demo-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     3335 2022-07-03 12:24:16.000000 teneva-0.9.8/demo/.ipynb_checkpoints/collection_matrices-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     4453 2022-07-03 12:24:13.000000 teneva-0.9.8/demo/.ipynb_checkpoints/collection_tensors-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     4372 2022-07-03 12:24:16.000000 teneva-0.9.8/demo/.ipynb_checkpoints/collection_vectors-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    11418 2022-03-14 20:54:15.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_als-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     9482 2022-04-16 15:09:43.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_anova-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    22641 2022-03-21 11:00:46.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_cheb-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    12717 2022-03-21 11:01:13.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_cheb_full-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    14477 2022-03-21 10:47:09.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_cross-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    15723 2022-03-19 11:43:47.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_grid-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     8977 2022-03-19 09:57:56.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_maxvol-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    18987 2022-07-03 10:46:54.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_optima-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     4667 2022-03-13 16:15:29.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_stat-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    12529 2022-03-13 17:27:14.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_svd-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    38666 2022-03-13 17:47:38.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_tensor-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    11296 2022-03-13 17:09:04.000000 teneva-0.9.8/demo/.ipynb_checkpoints/core_transformation-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)  1312488 2022-03-26 17:24:51.000000 teneva-0.9.8/demo/.ipynb_checkpoints/func_demo-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    24281 2022-06-24 11:56:45.000000 teneva-0.9.8/demo/.ipynb_checkpoints/func_func-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    63722 2022-07-03 12:21:45.000000 teneva-0.9.8/demo/.ipynb_checkpoints/tmp-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     6384 2022-07-01 15:45:56.000000 teneva-0.9.8/demo/.ipynb_checkpoints/ttopt_random-checkpoint.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     3335 2022-07-03 12:24:16.000000 teneva-0.9.8/demo/collection_matrices.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     4453 2022-07-03 12:24:13.000000 teneva-0.9.8/demo/collection_tensors.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     4372 2022-07-03 12:24:16.000000 teneva-0.9.8/demo/collection_vectors.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    11418 2022-03-14 20:54:15.000000 teneva-0.9.8/demo/core_als.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     9482 2022-04-16 15:09:43.000000 teneva-0.9.8/demo/core_anova.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    22641 2022-03-21 11:00:46.000000 teneva-0.9.8/demo/core_cheb.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    12717 2022-03-21 11:01:13.000000 teneva-0.9.8/demo/core_cheb_full.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    14477 2022-06-24 16:33:18.000000 teneva-0.9.8/demo/core_cross.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    15723 2022-03-19 11:43:47.000000 teneva-0.9.8/demo/core_grid.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     8977 2022-03-19 09:57:56.000000 teneva-0.9.8/demo/core_maxvol.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    18987 2022-07-03 10:46:54.000000 teneva-0.9.8/demo/core_optima.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     4667 2022-03-13 16:15:29.000000 teneva-0.9.8/demo/core_stat.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    12529 2022-03-13 17:27:14.000000 teneva-0.9.8/demo/core_svd.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    38955 2022-07-03 11:38:09.000000 teneva-0.9.8/demo/core_tensor.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    11296 2022-03-13 17:09:04.000000 teneva-0.9.8/demo/core_transformation.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)  1312488 2022-03-26 17:24:51.000000 teneva-0.9.8/demo/func_demo.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    24281 2022-06-24 11:56:45.000000 teneva-0.9.8/demo/func_func.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)    63722 2022-07-03 12:21:45.000000 teneva-0.9.8/demo/tmp.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)      107 2022-07-03 12:30:35.004105 teneva-0.9.8/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2511 2022-03-01 15:17:28.000000 teneva-0.9.8/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 12:30:34.988921 teneva-0.9.8/teneva/
--rw-r--r--   0 andrei     (501) staff       (20)       90 2022-07-03 12:30:05.000000 teneva-0.9.8/teneva/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 12:30:34.992188 teneva-0.9.8/teneva/collection/
--rw-r--r--   0 andrei     (501) staff       (20)      107 2022-07-03 12:22:38.000000 teneva-0.9.8/teneva/collection/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1255 2022-07-03 12:13:14.000000 teneva-0.9.8/teneva/collection/matrices.py
--rw-r--r--   0 andrei     (501) staff       (20)      915 2022-07-03 11:15:30.000000 teneva-0.9.8/teneva/collection/tensors.py
--rw-r--r--   0 andrei     (501) staff       (20)     1585 2022-07-03 11:57:15.000000 teneva-0.9.8/teneva/collection/vectors.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 12:30:34.997156 teneva-0.9.8/teneva/core/
--rw-r--r--   0 andrei     (501) staff       (20)     1691 2022-07-03 08:55:28.000000 teneva-0.9.8/teneva/core/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     5366 2022-04-16 15:13:54.000000 teneva-0.9.8/teneva/core/als.py
--rw-r--r--   0 andrei     (501) staff       (20)     7433 2022-07-01 15:48:12.000000 teneva-0.9.8/teneva/core/anova.py
--rw-r--r--   0 andrei     (501) staff       (20)    10421 2022-03-21 10:58:39.000000 teneva-0.9.8/teneva/core/cheb.py
--rw-r--r--   0 andrei     (501) staff       (20)     7641 2022-03-14 16:49:49.000000 teneva-0.9.8/teneva/core/cheb_full.py
--rw-r--r--   0 andrei     (501) staff       (20)    10200 2022-06-24 16:33:23.000000 teneva-0.9.8/teneva/core/cross.py
--rw-r--r--   0 andrei     (501) staff       (20)     9526 2022-03-19 11:43:37.000000 teneva-0.9.8/teneva/core/grid.py
--rw-r--r--   0 andrei     (501) staff       (20)     5205 2022-03-18 09:32:41.000000 teneva-0.9.8/teneva/core/maxvol.py
--rw-r--r--   0 andrei     (501) staff       (20)     7531 2022-07-03 10:08:44.000000 teneva-0.9.8/teneva/core/optima.py
--rw-r--r--   0 andrei     (501) staff       (20)     1371 2022-03-13 16:16:26.000000 teneva-0.9.8/teneva/core/stat.py
--rw-r--r--   0 andrei     (501) staff       (20)     5453 2022-03-13 17:25:43.000000 teneva-0.9.8/teneva/core/svd.py
--rw-r--r--   0 andrei     (501) staff       (20)    13008 2022-03-13 17:41:29.000000 teneva-0.9.8/teneva/core/tensor.py
--rw-r--r--   0 andrei     (501) staff       (20)     3440 2022-03-13 16:29:12.000000 teneva-0.9.8/teneva/core/transformation.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 12:30:34.998022 teneva-0.9.8/teneva/func/
--rw-r--r--   0 andrei     (501) staff       (20)       45 2022-02-20 16:30:30.000000 teneva-0.9.8/teneva/func/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 12:30:35.003161 teneva-0.9.8/teneva/func/demo/
--rw-r--r--   0 andrei     (501) staff       (20)     2452 2022-07-01 13:00:32.000000 teneva-0.9.8/teneva/func/demo/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1733 2022-07-01 12:55:56.000000 teneva-0.9.8/teneva/func/demo/func_demo_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     1019 2022-07-01 12:56:23.000000 teneva-0.9.8/teneva/func/demo/func_demo_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     1120 2022-07-01 12:56:32.000000 teneva-0.9.8/teneva/func/demo/func_demo_brown.py
--rw-r--r--   0 andrei     (501) staff       (20)     1323 2022-07-01 12:56:40.000000 teneva-0.9.8/teneva/func/demo/func_demo_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     1021 2022-07-01 12:56:44.000000 teneva-0.9.8/teneva/func/demo/func_demo_exponential.py
--rw-r--r--   0 andrei     (501) staff       (20)     1339 2022-07-01 12:56:59.000000 teneva-0.9.8/teneva/func/demo/func_demo_grienwank.py
--rw-r--r--   0 andrei     (501) staff       (20)     1783 2022-07-01 12:57:11.000000 teneva-0.9.8/teneva/func/demo/func_demo_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     1608 2022-07-01 12:57:26.000000 teneva-0.9.8/teneva/func/demo/func_demo_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     1034 2022-07-01 12:57:40.000000 teneva-0.9.8/teneva/func/demo/func_demo_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     1304 2022-07-01 12:57:51.000000 teneva-0.9.8/teneva/func/demo/func_demo_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     1083 2022-07-01 12:57:50.000000 teneva-0.9.8/teneva/func/demo/func_demo_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     1207 2022-07-01 12:57:54.000000 teneva-0.9.8/teneva/func/demo/func_demo_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     1165 2022-07-01 12:58:26.000000 teneva-0.9.8/teneva/func/demo/func_demo_schwefel.py
--rw-r--r--   0 andrei     (501) staff       (20)    39373 2022-06-24 16:33:31.000000 teneva-0.9.8/teneva/func/func.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 12:30:34.990574 teneva-0.9.8/teneva.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     3619 2022-07-03 12:30:34.000000 teneva-0.9.8/teneva.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2703 2022-07-03 12:30:34.000000 teneva-0.9.8/teneva.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2022-07-03 12:30:34.000000 teneva-0.9.8/teneva.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       29 2022-07-03 12:30:34.000000 teneva-0.9.8/teneva.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)        7 2022-07-03 12:30:34.000000 teneva-0.9.8/teneva.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 14:09:05.970408 teneva-0.9.9/
+-rw-r--r--   0 andrei     (501) staff       (20)     1095 2022-01-01 12:16:24.000000 teneva-0.9.9/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       63 2022-02-22 08:40:27.000000 teneva-0.9.9/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     3619 2022-07-03 14:09:05.970590 teneva-0.9.9/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     1992 2022-03-13 14:41:05.000000 teneva-0.9.9/README.md
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 14:09:05.937896 teneva-0.9.9/demo/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2022-07-01 16:04:08.000000 teneva-0.9.9/demo/.DS_Store
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 14:09:05.956827 teneva-0.9.9/demo/.ipynb_checkpoints/
+-rw-r--r--   0 andrei     (501) staff       (20)     4130 2022-06-21 08:33:45.000000 teneva-0.9.9/demo/.ipynb_checkpoints/2d_cross_demo-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     3335 2022-07-03 12:24:16.000000 teneva-0.9.9/demo/.ipynb_checkpoints/collection_matrices-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     4453 2022-07-03 12:24:13.000000 teneva-0.9.9/demo/.ipynb_checkpoints/collection_tensors-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     4372 2022-07-03 12:24:16.000000 teneva-0.9.9/demo/.ipynb_checkpoints/collection_vectors-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    11418 2022-03-14 20:54:15.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_als-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     9482 2022-04-16 15:09:43.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_anova-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    22641 2022-03-21 11:00:46.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_cheb-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    12717 2022-03-21 11:01:13.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_cheb_full-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    14477 2022-03-21 10:47:09.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_cross-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    15723 2022-03-19 11:43:47.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_grid-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     8977 2022-03-19 09:57:56.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_maxvol-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    18987 2022-07-03 10:46:54.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_optima-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     4667 2022-03-13 16:15:29.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_stat-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    12529 2022-03-13 17:27:14.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_svd-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    38666 2022-03-13 17:47:38.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_tensor-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    11296 2022-03-13 17:09:04.000000 teneva-0.9.9/demo/.ipynb_checkpoints/core_transformation-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)  1312488 2022-03-26 17:24:51.000000 teneva-0.9.9/demo/.ipynb_checkpoints/func_demo-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    24281 2022-06-24 11:56:45.000000 teneva-0.9.9/demo/.ipynb_checkpoints/func_func-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    63722 2022-07-03 12:21:45.000000 teneva-0.9.9/demo/.ipynb_checkpoints/tmp-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     6384 2022-07-01 15:45:56.000000 teneva-0.9.9/demo/.ipynb_checkpoints/ttopt_random-checkpoint.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     3335 2022-07-03 12:24:16.000000 teneva-0.9.9/demo/collection_matrices.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     4453 2022-07-03 12:24:13.000000 teneva-0.9.9/demo/collection_tensors.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     4372 2022-07-03 12:24:16.000000 teneva-0.9.9/demo/collection_vectors.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    11418 2022-03-14 20:54:15.000000 teneva-0.9.9/demo/core_als.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     9482 2022-04-16 15:09:43.000000 teneva-0.9.9/demo/core_anova.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    22641 2022-03-21 11:00:46.000000 teneva-0.9.9/demo/core_cheb.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    12717 2022-03-21 11:01:13.000000 teneva-0.9.9/demo/core_cheb_full.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    14477 2022-06-24 16:33:18.000000 teneva-0.9.9/demo/core_cross.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    15723 2022-03-19 11:43:47.000000 teneva-0.9.9/demo/core_grid.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     8977 2022-03-19 09:57:56.000000 teneva-0.9.9/demo/core_maxvol.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    18987 2022-07-03 10:46:54.000000 teneva-0.9.9/demo/core_optima.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     4667 2022-03-13 16:15:29.000000 teneva-0.9.9/demo/core_stat.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    12529 2022-03-13 17:27:14.000000 teneva-0.9.9/demo/core_svd.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    38955 2022-07-03 11:38:09.000000 teneva-0.9.9/demo/core_tensor.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    11296 2022-03-13 17:09:04.000000 teneva-0.9.9/demo/core_transformation.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)  1312488 2022-03-26 17:24:51.000000 teneva-0.9.9/demo/func_demo.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    24281 2022-06-24 11:56:45.000000 teneva-0.9.9/demo/func_func.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)    63722 2022-07-03 12:21:45.000000 teneva-0.9.9/demo/tmp.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2022-07-03 14:09:05.971023 teneva-0.9.9/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2511 2022-03-01 15:17:28.000000 teneva-0.9.9/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 14:09:05.957963 teneva-0.9.9/teneva/
+-rw-r--r--   0 andrei     (501) staff       (20)       90 2022-07-03 14:08:27.000000 teneva-0.9.9/teneva/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 14:09:05.960935 teneva-0.9.9/teneva/collection/
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2022-07-03 12:22:38.000000 teneva-0.9.9/teneva/collection/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1255 2022-07-03 12:13:14.000000 teneva-0.9.9/teneva/collection/matrices.py
+-rw-r--r--   0 andrei     (501) staff       (20)      915 2022-07-03 11:15:30.000000 teneva-0.9.9/teneva/collection/tensors.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1585 2022-07-03 11:57:15.000000 teneva-0.9.9/teneva/collection/vectors.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 14:09:05.964964 teneva-0.9.9/teneva/core/
+-rw-r--r--   0 andrei     (501) staff       (20)     1691 2022-07-03 08:55:28.000000 teneva-0.9.9/teneva/core/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5366 2022-04-16 15:13:54.000000 teneva-0.9.9/teneva/core/als.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7433 2022-07-01 15:48:12.000000 teneva-0.9.9/teneva/core/anova.py
+-rw-r--r--   0 andrei     (501) staff       (20)    10421 2022-03-21 10:58:39.000000 teneva-0.9.9/teneva/core/cheb.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7641 2022-03-14 16:49:49.000000 teneva-0.9.9/teneva/core/cheb_full.py
+-rw-r--r--   0 andrei     (501) staff       (20)    10200 2022-06-24 16:33:23.000000 teneva-0.9.9/teneva/core/cross.py
+-rw-r--r--   0 andrei     (501) staff       (20)     9526 2022-03-19 11:43:37.000000 teneva-0.9.9/teneva/core/grid.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5205 2022-03-18 09:32:41.000000 teneva-0.9.9/teneva/core/maxvol.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7535 2022-07-03 14:07:59.000000 teneva-0.9.9/teneva/core/optima.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1371 2022-03-13 16:16:26.000000 teneva-0.9.9/teneva/core/stat.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5453 2022-03-13 17:25:43.000000 teneva-0.9.9/teneva/core/svd.py
+-rw-r--r--   0 andrei     (501) staff       (20)    13008 2022-03-13 17:41:29.000000 teneva-0.9.9/teneva/core/tensor.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3440 2022-03-13 16:29:12.000000 teneva-0.9.9/teneva/core/transformation.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 14:09:05.965959 teneva-0.9.9/teneva/func/
+-rw-r--r--   0 andrei     (501) staff       (20)       45 2022-02-20 16:30:30.000000 teneva-0.9.9/teneva/func/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 14:09:05.970103 teneva-0.9.9/teneva/func/demo/
+-rw-r--r--   0 andrei     (501) staff       (20)     2452 2022-07-01 13:00:32.000000 teneva-0.9.9/teneva/func/demo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1733 2022-07-01 12:55:56.000000 teneva-0.9.9/teneva/func/demo/func_demo_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1019 2022-07-01 12:56:23.000000 teneva-0.9.9/teneva/func/demo/func_demo_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1120 2022-07-01 12:56:32.000000 teneva-0.9.9/teneva/func/demo/func_demo_brown.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1323 2022-07-01 12:56:40.000000 teneva-0.9.9/teneva/func/demo/func_demo_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1021 2022-07-01 12:56:44.000000 teneva-0.9.9/teneva/func/demo/func_demo_exponential.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1339 2022-07-01 12:56:59.000000 teneva-0.9.9/teneva/func/demo/func_demo_grienwank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1783 2022-07-01 12:57:11.000000 teneva-0.9.9/teneva/func/demo/func_demo_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1608 2022-07-01 12:57:26.000000 teneva-0.9.9/teneva/func/demo/func_demo_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1034 2022-07-01 12:57:40.000000 teneva-0.9.9/teneva/func/demo/func_demo_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1304 2022-07-01 12:57:51.000000 teneva-0.9.9/teneva/func/demo/func_demo_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1083 2022-07-01 12:57:50.000000 teneva-0.9.9/teneva/func/demo/func_demo_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1207 2022-07-01 12:57:54.000000 teneva-0.9.9/teneva/func/demo/func_demo_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1165 2022-07-01 12:58:26.000000 teneva-0.9.9/teneva/func/demo/func_demo_schwefel.py
+-rw-r--r--   0 andrei     (501) staff       (20)    39373 2022-06-24 16:33:31.000000 teneva-0.9.9/teneva/func/func.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2022-07-03 14:09:05.959601 teneva-0.9.9/teneva.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     3619 2022-07-03 14:09:05.000000 teneva-0.9.9/teneva.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2703 2022-07-03 14:09:05.000000 teneva-0.9.9/teneva.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2022-07-03 14:09:05.000000 teneva-0.9.9/teneva.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       29 2022-07-03 14:09:05.000000 teneva-0.9.9/teneva.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        7 2022-07-03 14:09:05.000000 teneva-0.9.9/teneva.egg-info/top_level.txt
```

### Comparing `teneva-0.9.8/LICENSE.txt` & `teneva-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/PKG-INFO` & `teneva-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva
-Version: 0.9.8
+Version: 0.9.9
 Summary: Compact implementation of basic operations in the tensor-train (TT) format, including TT-SVD, TT-ALS, TT-ANOVA, TT-CROSS, TT-truncate for approximation of multidimensional arrays and multivariate functions
 Home-page: https://github.com/AndreiChertkov/teneva
 Author: Andrei Chertkov
 Author-email: a.chertkov@skoltech.ru
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva
 Description: # teneva
```

### Comparing `teneva-0.9.8/README.md` & `teneva-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.DS_Store` & `teneva-0.9.9/demo/.DS_Store`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/2d_cross_demo-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/2d_cross_demo-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/collection_matrices-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/collection_matrices-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/collection_tensors-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/collection_tensors-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/collection_vectors-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/collection_vectors-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_als-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_als-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_anova-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_anova-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_cheb-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_cheb-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_cheb_full-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_cheb_full-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_cross-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_cross-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_grid-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_grid-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_maxvol-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_maxvol-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_optima-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_optima-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_stat-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_stat-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_svd-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_svd-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_tensor-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_tensor-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/core_transformation-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/core_transformation-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/func_demo-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/func_demo-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/func_func-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/func_func-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/tmp-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/tmp-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/.ipynb_checkpoints/ttopt_random-checkpoint.ipynb` & `teneva-0.9.9/demo/.ipynb_checkpoints/ttopt_random-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/collection_matrices.ipynb` & `teneva-0.9.9/demo/collection_matrices.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/collection_tensors.ipynb` & `teneva-0.9.9/demo/collection_tensors.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/collection_vectors.ipynb` & `teneva-0.9.9/demo/collection_vectors.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_als.ipynb` & `teneva-0.9.9/demo/core_als.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_anova.ipynb` & `teneva-0.9.9/demo/core_anova.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_cheb.ipynb` & `teneva-0.9.9/demo/core_cheb.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_cheb_full.ipynb` & `teneva-0.9.9/demo/core_cheb_full.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_cross.ipynb` & `teneva-0.9.9/demo/core_cross.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_grid.ipynb` & `teneva-0.9.9/demo/core_grid.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_maxvol.ipynb` & `teneva-0.9.9/demo/core_maxvol.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_optima.ipynb` & `teneva-0.9.9/demo/core_optima.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_stat.ipynb` & `teneva-0.9.9/demo/core_stat.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_svd.ipynb` & `teneva-0.9.9/demo/core_svd.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_tensor.ipynb` & `teneva-0.9.9/demo/core_tensor.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/core_transformation.ipynb` & `teneva-0.9.9/demo/core_transformation.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/func_demo.ipynb` & `teneva-0.9.9/demo/func_demo.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/func_func.ipynb` & `teneva-0.9.9/demo/func_func.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/demo/tmp.ipynb` & `teneva-0.9.9/demo/tmp.ipynb`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/setup.py` & `teneva-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/collection/matrices.py` & `teneva-0.9.9/teneva/collection/matrices.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/collection/tensors.py` & `teneva-0.9.9/teneva/collection/tensors.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/collection/vectors.py` & `teneva-0.9.9/teneva/collection/vectors.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/__init__.py` & `teneva-0.9.9/teneva/core/__init__.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/als.py` & `teneva-0.9.9/teneva/core/als.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/anova.py` & `teneva-0.9.9/teneva/core/anova.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/cheb.py` & `teneva-0.9.9/teneva/core/cheb.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/cheb_full.py` & `teneva-0.9.9/teneva/core/cheb_full.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/cross.py` & `teneva-0.9.9/teneva/core/cross.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/grid.py` & `teneva-0.9.9/teneva/core/grid.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/maxvol.py` & `teneva-0.9.9/teneva/core/maxvol.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/optima.py` & `teneva-0.9.9/teneva/core/optima.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .tensor import getter
 from .tensor import mul
 from .tensor import shape
 from .tensor import sub
 from .transformation import truncate
 
 
-def optima_tt(Y, nswp=5, nswp_outer=1, r=50, e=1.E-12, log=False):
+def optima_tt(Y, nswp=5, nswp_outer=1, r=40, e=1.E-10, log=False):
     """Find multi-indices which relate to min and max elements of TT-tensor.
 
     Args:
         Y (list): d-dimensional TT-tensor.
         nswp (int): number of power-iterations (> 0).
         nswp_outer (int): number of repeats of power-iterations (> 0).
         r (int): maximum TT-rank while power-iterations (> 0).
@@ -224,19 +224,19 @@
 
     _log(
         y_min if is_max else y_opt,
         y_opt if is_max else y_max,
         -1, erank(Z), is_max, y_eps=y_eps, with_log=log)
 
     for swp in range(nswp):
-        if erank(Z) >= r:
-            return _result()
         if scale < 1.E-16:
             print('Warning! Almost zero scale. Break')
             return _result()
+        if erank(Z) * 2 >= r:
+            return _result()
 
         Z = mul(Z, Z)
         Z = mul(Z, 1./scale**2)
         Z = truncate(Z, e)
 
         _, __, i_opt_new, scale = optima_tt_simple(Z)
         y_opt_new = get(Y, i_opt_new)
```

### Comparing `teneva-0.9.8/teneva/core/stat.py` & `teneva-0.9.9/teneva/core/stat.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/svd.py` & `teneva-0.9.9/teneva/core/svd.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/tensor.py` & `teneva-0.9.9/teneva/core/tensor.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/core/transformation.py` & `teneva-0.9.9/teneva/core/transformation.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/__init__.py` & `teneva-0.9.9/teneva/func/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_ackley.py` & `teneva-0.9.9/teneva/func/demo/func_demo_ackley.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_alpine.py` & `teneva-0.9.9/teneva/func/demo/func_demo_alpine.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_brown.py` & `teneva-0.9.9/teneva/func/demo/func_demo_brown.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_dixon.py` & `teneva-0.9.9/teneva/func/demo/func_demo_dixon.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_exponential.py` & `teneva-0.9.9/teneva/func/demo/func_demo_exponential.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_grienwank.py` & `teneva-0.9.9/teneva/func/demo/func_demo_grienwank.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_michalewicz.py` & `teneva-0.9.9/teneva/func/demo/func_demo_michalewicz.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_piston.py` & `teneva-0.9.9/teneva/func/demo/func_demo_piston.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_qing.py` & `teneva-0.9.9/teneva/func/demo/func_demo_qing.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_rastrigin.py` & `teneva-0.9.9/teneva/func/demo/func_demo_rastrigin.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_rosenbrock.py` & `teneva-0.9.9/teneva/func/demo/func_demo_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_schaffer.py` & `teneva-0.9.9/teneva/func/demo/func_demo_schaffer.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/demo/func_demo_schwefel.py` & `teneva-0.9.9/teneva/func/demo/func_demo_schwefel.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva/func/func.py` & `teneva-0.9.9/teneva/func/func.py`

 * *Files identical despite different names*

### Comparing `teneva-0.9.8/teneva.egg-info/PKG-INFO` & `teneva-0.9.9/teneva.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva
-Version: 0.9.8
+Version: 0.9.9
 Summary: Compact implementation of basic operations in the tensor-train (TT) format, including TT-SVD, TT-ALS, TT-ANOVA, TT-CROSS, TT-truncate for approximation of multidimensional arrays and multivariate functions
 Home-page: https://github.com/AndreiChertkov/teneva
 Author: Andrei Chertkov
 Author-email: a.chertkov@skoltech.ru
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva
 Description: # teneva
```

### Comparing `teneva-0.9.8/teneva.egg-info/SOURCES.txt` & `teneva-0.9.9/teneva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

