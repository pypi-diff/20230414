# Comparing `tmp/trainml-0.4.8.tar.gz` & `tmp/trainml-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trainml-0.4.8.tar", last modified: Thu Jan  5 23:13:10 2023, max compression
+gzip compressed data, was "dist/trainml-0.4.9.tar", last modified: Tue Jan 17 22:35:28 2023, max compression
```

## Comparing `trainml-0.4.8.tar` & `trainml-0.4.9.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-05 23:13:10.098375 trainml-0.4.8/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.4.8/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2023-01-05 23:13:10.097989 trainml-0.4.8/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.4.8/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-05 23:13:10.049613 trainml-0.4.8/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.4.8/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1204 2022-09-13 15:59:08.000000 trainml-0.4.8/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1770 2022-09-07 15:15:43.000000 trainml-0.4.8/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2359 2022-09-07 15:16:04.000000 trainml-0.4.8/examples/training_inference_pipeline.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      710 2023-01-05 20:17:55.000000 trainml-0.4.8/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2023-01-05 23:13:10.098507 trainml-0.4.8/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.4.8/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-05 23:13:10.043088 trainml-0.4.8/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-05 23:13:10.059887 trainml-0.4.8/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.4.8/tests/integration/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.4.8/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3116 2023-01-05 21:36:25.000000 trainml-0.4.8/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3412 2023-01-05 20:33:29.000000 trainml-0.4.8/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1391 2021-03-11 02:41:10.000000 trainml-0.4.8/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2022-02-07 16:08:41.000000 trainml-0.4.8/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    23317 2022-12-14 03:06:24.000000 trainml-0.4.8/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2835 2022-09-22 16:37:05.000000 trainml-0.4.8/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1480 2021-09-28 14:24:02.000000 trainml-0.4.8/tests/integration/test_projects_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1407 2022-11-03 18:50:25.000000 trainml-0.4.8/tests/integration/test_providers_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-05 23:13:10.073277 trainml-0.4.8/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.4.8/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-05 23:13:10.074756 trainml-0.4.8/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.4.8/tests/unit/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.4.8/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2021-03-12 19:19:14.000000 trainml-0.4.8/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    17362 2022-08-29 16:12:17.000000 trainml-0.4.8/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      815 2021-03-11 02:25:33.000000 trainml-0.4.8/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15936 2023-01-05 20:16:26.000000 trainml-0.4.8/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2022-08-29 16:13:44.000000 trainml-0.4.8/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15858 2023-01-05 23:11:27.000000 trainml-0.4.8/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2021-03-11 02:32:19.000000 trainml-0.4.8/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.4.8/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1703 2022-08-29 15:53:27.000000 trainml-0.4.8/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    28336 2022-09-19 22:20:04.000000 trainml-0.4.8/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15060 2023-01-05 23:11:27.000000 trainml-0.4.8/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3803 2021-12-07 17:57:14.000000 trainml-0.4.8/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3700 2022-11-03 18:50:49.000000 trainml-0.4.8/tests/unit/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.4.8/tests/unit/test_trainml.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-05 23:13:10.087340 trainml-0.4.8/trainml/
--rw-r--r--   0 akowalsk   (501) staff       (20)      422 2023-01-05 23:11:43.000000 trainml-0.4.8/trainml/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.4.8/trainml/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26446 2022-04-16 18:55:57.000000 trainml-0.4.8/trainml/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6950 2023-01-05 21:38:00.000000 trainml-0.4.8/trainml/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-05 23:13:10.094821 trainml-0.4.8/trainml/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4280 2023-01-05 20:15:36.000000 trainml-0.4.8/trainml/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5849 2023-01-05 20:15:37.000000 trainml-0.4.8/trainml/cli/checkpoint.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2022-08-29 15:36:54.000000 trainml-0.4.8/trainml/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6285 2022-09-19 22:07:28.000000 trainml-0.4.8/trainml/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2021-08-20 02:02:59.000000 trainml-0.4.8/trainml/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      919 2022-02-08 15:46:35.000000 trainml-0.4.8/trainml/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-05 23:13:10.096196 trainml-0.4.8/trainml/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6544 2022-09-19 22:08:20.000000 trainml-0.4.8/trainml/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    30233 2022-12-21 14:53:21.000000 trainml-0.4.8/trainml/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5509 2022-09-19 22:07:15.000000 trainml-0.4.8/trainml/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1654 2021-09-15 16:00:52.000000 trainml-0.4.8/trainml/cli/project.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20051 2023-01-05 21:37:40.000000 trainml-0.4.8/trainml/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7013 2023-01-05 23:11:27.000000 trainml-0.4.8/trainml/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1537 2021-02-11 18:25:46.000000 trainml-0.4.8/trainml/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3724 2023-01-05 20:17:59.000000 trainml-0.4.8/trainml/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1831 2022-02-07 15:42:56.000000 trainml-0.4.8/trainml/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    17420 2022-10-17 02:43:22.000000 trainml-0.4.8/trainml/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6678 2023-01-05 23:11:27.000000 trainml-0.4.8/trainml/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2009 2021-12-07 17:49:13.000000 trainml-0.4.8/trainml/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1844 2022-11-03 18:21:21.000000 trainml-0.4.8/trainml/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10618 2023-01-05 20:17:57.000000 trainml-0.4.8/trainml/trainml.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-05 23:13:10.089293 trainml-0.4.8/trainml.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2023-01-05 23:13:09.000000 trainml-0.4.8/trainml.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     1853 2023-01-05 23:13:09.000000 trainml-0.4.8/trainml.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2023-01-05 23:13:09.000000 trainml-0.4.8/trainml.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2023-01-05 23:13:09.000000 trainml-0.4.8/trainml.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2023-01-05 23:13:09.000000 trainml-0.4.8/trainml.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2023-01-05 23:13:09.000000 trainml-0.4.8/trainml.egg-info/top_level.txt
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.839909 trainml-0.4.9/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.4.9/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2023-01-17 22:35:28.839337 trainml-0.4.9/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.4.9/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.791775 trainml-0.4.9/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.4.9/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.4.9/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.4.9/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2333 2023-01-10 21:57:07.000000 trainml-0.4.9/examples/training_inference_pipeline.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      710 2023-01-05 20:17:55.000000 trainml-0.4.9/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2023-01-17 22:35:28.840079 trainml-0.4.9/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.4.9/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.785582 trainml-0.4.9/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.801964 trainml-0.4.9/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.4.9/tests/integration/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.4.9/tests/integration/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3116 2023-01-05 21:36:25.000000 trainml-0.4.9/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3412 2023-01-05 20:33:29.000000 trainml-0.4.9/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1391 2021-03-11 02:41:10.000000 trainml-0.4.9/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2022-02-07 16:08:41.000000 trainml-0.4.9/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    23476 2023-01-10 22:21:04.000000 trainml-0.4.9/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2835 2022-09-22 16:37:05.000000 trainml-0.4.9/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1480 2021-09-28 14:24:02.000000 trainml-0.4.9/tests/integration/test_projects_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1407 2023-01-10 22:00:20.000000 trainml-0.4.9/tests/integration/test_providers_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.814977 trainml-0.4.9/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.4.9/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.816956 trainml-0.4.9/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.4.9/tests/unit/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.4.9/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2021-03-12 19:19:14.000000 trainml-0.4.9/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20053 2023-01-10 22:45:56.000000 trainml-0.4.9/tests/unit/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      815 2021-03-11 02:25:33.000000 trainml-0.4.9/tests/unit/test_auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15935 2023-01-10 22:45:55.000000 trainml-0.4.9/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.4.9/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15815 2023-01-16 16:42:32.000000 trainml-0.4.9/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2021-03-11 02:32:19.000000 trainml-0.4.9/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.4.9/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1703 2023-01-10 22:45:55.000000 trainml-0.4.9/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26446 2023-01-10 22:45:55.000000 trainml-0.4.9/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15021 2023-01-16 16:42:31.000000 trainml-0.4.9/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3803 2021-12-07 17:57:14.000000 trainml-0.4.9/tests/unit/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3700 2022-11-03 18:50:49.000000 trainml-0.4.9/tests/unit/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.4.9/tests/unit/test_trainml.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.827826 trainml-0.4.9/trainml/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      422 2023-01-17 22:34:22.000000 trainml-0.4.9/trainml/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.4.9/trainml/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26446 2022-04-16 18:55:57.000000 trainml-0.4.9/trainml/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7156 2023-01-10 22:09:49.000000 trainml-0.4.9/trainml/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.836458 trainml-0.4.9/trainml/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4322 2023-01-17 21:52:08.000000 trainml-0.4.9/trainml/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6526 2023-01-10 22:10:42.000000 trainml-0.4.9/trainml/cli/checkpoint.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2022-08-29 15:36:54.000000 trainml-0.4.9/trainml/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6285 2022-09-19 22:07:28.000000 trainml-0.4.9/trainml/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2021-08-20 02:02:59.000000 trainml-0.4.9/trainml/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      919 2022-02-08 15:46:35.000000 trainml-0.4.9/trainml/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.837749 trainml-0.4.9/trainml/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6544 2022-09-19 22:08:20.000000 trainml-0.4.9/trainml/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    33021 2023-01-16 20:15:17.000000 trainml-0.4.9/trainml/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5509 2022-09-19 22:07:15.000000 trainml-0.4.9/trainml/cli/model.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1654 2021-09-15 16:00:52.000000 trainml-0.4.9/trainml/cli/project.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1594 2023-01-17 21:53:43.000000 trainml-0.4.9/trainml/cli/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20059 2023-01-10 14:50:42.000000 trainml-0.4.9/trainml/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6951 2023-01-16 16:41:50.000000 trainml-0.4.9/trainml/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1537 2021-02-11 18:25:46.000000 trainml-0.4.9/trainml/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3724 2023-01-05 20:17:59.000000 trainml-0.4.9/trainml/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1831 2022-02-07 15:42:56.000000 trainml-0.4.9/trainml/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16710 2023-01-10 21:47:55.000000 trainml-0.4.9/trainml/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6620 2023-01-16 16:42:01.000000 trainml-0.4.9/trainml/models.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2009 2021-12-07 17:49:13.000000 trainml-0.4.9/trainml/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1844 2022-11-03 18:21:21.000000 trainml-0.4.9/trainml/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10618 2023-01-05 20:17:57.000000 trainml-0.4.9/trainml/trainml.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.830721 trainml-0.4.9/trainml.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1877 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/top_level.txt
```

### Comparing `trainml-0.4.8/LICENSE` & `trainml-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/PKG-INFO` & `trainml-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.4.8
+Version: 0.4.9
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.4.8 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.4.9 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           [https://www.trainml.ai/static/img/trainML-logo-purple.png]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.4.8/README.md` & `trainml-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/examples/create_dataset_and_training_job.py` & `trainml-0.4.9/examples/create_dataset_and_training_job.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         gpu_types=["rtx2080ti", "rtx3090"],
         gpu_count=1,
         disk_size=10,
         workers=[
             "python training/image-classification/resnet_cifar.py --epochs 10 --optimizer adam --batch-size 128",
         ],
         data=dict(
-            datasets=[dict(id=dataset.id, type="existing")],
+            datasets=[dataset.id],
             output_uri="s3://trainml-examples/output/resnet_cifar10",
             output_type="aws",
         ),
         model=dict(
             source_type="git",
             source_uri="https://github.com/trainML/examples.git",
         ),
```

### Comparing `trainml-0.4.8/examples/local_storage.py` & `trainml-0.4.9/examples/local_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         gpu_types=["rtx2080ti", "rtx3090"],
         gpu_count=1,
         disk_size=10,
         workers=[
             "python training/image-classification/resnet_cifar.py --epochs 10 --optimizer adam --batch-size 128",
         ],
         data=dict(
-            datasets=[dict(id=dataset.id, type="existing")],
+            datasets=[dataset.id],
             output_uri="~/tensorflow-example/output",
             output_type="local",
         ),
         model=dict(source_type="local", source_uri="~/trainml-examples"),
     )
 
     print(job)
@@ -58,8 +58,8 @@
     await job.disconnect()
     await job.remove()
 
 
 asyncio.run(run_job(dataset))
 
 # Cleanup Dataset
-asyncio.run(dataset.remove())
+asyncio.run(dataset.remove())
```

### Comparing `trainml-0.4.8/examples/training_inference_pipeline.py` & `trainml-0.4.9/examples/training_inference_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         gpu_types=["rtx2080ti", "rtx3090"],
         gpu_count=1,
         disk_size=10,
         workers=[
             "python training/image-classification/resnet_cifar.py --epochs 10 --optimizer adam --batch-size 128",
         ],
         data=dict(
-            datasets=[dict(id=dataset.id, type="existing")],
+            datasets=[dataset.id],
             output_type="trainml",
         ),
         model=dict(
             source_type="git",
             source_uri="https://github.com/trainML/examples.git",
         ),
     )
```

### Comparing `trainml-0.4.8/pyproject.toml` & `trainml-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/setup.py` & `trainml-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/integration/conftest.py` & `trainml-0.4.9/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/integration/test_checkpoints_integration.py` & `trainml-0.4.9/tests/integration/test_checkpoints_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/integration/test_datasets_integration.py` & `trainml-0.4.9/tests/integration/test_datasets_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/integration/test_environments_integration.py` & `trainml-0.4.9/tests/integration/test_environments_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/integration/test_gpu_types_integration.py` & `trainml-0.4.9/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/integration/test_jobs_integration.py` & `trainml-0.4.9/tests/integration/test_jobs_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 async def job(trainml):
     job = await trainml.jobs.create(
         name="CLI Automated Tests - Job Lifecycle",
         type="notebook",
         gpu_types=["gtx1060"],
         gpu_count=1,
         disk_size=11,
-        data=dict(datasets=[dict(name="CIFAR-10", type="public")]),
+        data=dict(datasets=[dict(id="CIFAR-10", public=True)]),
         model=dict(
             source_type="git",
             source_uri="git@github.com:trainML/environment-tests.git",
         ),
     )
     yield job
 
@@ -100,16 +100,16 @@
         training_job = await job.copy(
             name="CLI Automated Tests - Job Convert",
             type="training",
             workers=["python $TRAINML_MODEL_PATH/tensorflow/main.py"],
             data=dict(
                 datasets=[
                     dict(
-                        name="CIFAR-10",
-                        type="public",
+                        id="CIFAR-10",
+                        public=True,
                     )
                 ],
                 output_uri="s3://trainml-examples/output/resnet_cifar10",
                 output_type="aws",
             ),
         )
         assert training_job.id
@@ -306,15 +306,15 @@
     async def test_invalid_datasets_for_inference(self, trainml):
         with raises(ApiError) as error:
             await trainml.jobs.create(
                 name="Datasets for Inference Job",
                 type="inference",
                 gpu_types=["rtx3090"],
                 disk_size=10,
-                data=dict(datasets=[dict(id="CIFAR-10", type="public")]),
+                data=dict(datasets=[dict(id="CIFAR-10", public=True)]),
                 workers=["python predict.py"],
             )
         assert (
             "Invalid Request - Inference jobs cannot use datasets"
             in error.value.message
         )
 
@@ -370,45 +370,55 @@
         temp_dir = tempfile.TemporaryDirectory()
         job = await trainml.jobs.create(
             name="CLI Automated Tests - Local Output",
             type="training",
             gpu_types=["gtx1060"],
             disk_size=10,
             workers=["python $TRAINML_MODEL_PATH/tensorflow/main.py"],
-            environment=dict(type="DEEPLEARNING_PY39"),
+            environment=dict(
+                type="DEEPLEARNING_PY39",
+                env=[
+                    dict(
+                        key="CHECKPOINT_FILE",
+                        value="model.ckpt-0050",
+                    )
+                ],
+            ),
             data=dict(
                 datasets=[
                     dict(
-                        name="CIFAR-10",
-                        type="public",
+                        id="CIFAR-10",
+                        public=True,
                     )
                 ],
                 output_uri=temp_dir.name,
                 output_type="local",
             ),
             model=dict(
                 source_type="git",
                 source_uri="git@github.com:trainML/environment-tests.git",
+                checkpoints=[
+                    "tensorflow-checkpoint",
+                ],
             ),
         )
         await job.wait_for("waiting for data/model download")
         attach_task = asyncio.create_task(job.attach())
         connect_task = asyncio.create_task(job.connect())
         await asyncio.gather(attach_task, connect_task)
         await job.refresh()
         assert job.status == "finished"
         await job.disconnect()
         await job.remove()
         upload_contents = os.listdir(temp_dir.name)
-        result = any(
-            "CLI_Automated_Tensorflow_Test_1" in content
+        temp_dir.cleanup()
+        assert any(
+            "CLI_Automated_Tests_-_Local_Output" in content
             for content in upload_contents
         )
-        assert result is not None
-        temp_dir.cleanup()
 
         captured = capsys.readouterr()
         sys.stdout.write(captured.out)
         sys.stderr.write(captured.err)
         assert "Epoch 1/2" in captured.out
         assert "Epoch 2/2" in captured.out
         assert "adding: model.ckpt-0001.data-00000-of-00001" in captured.out
@@ -428,20 +438,19 @@
             "CLI Automated Tests - Training With trainML Model Output",
             type="training",
             gpu_types=["gtx1060"],
             gpu_count=1,
             cpu_count=8,
             disk_size=10,
             worker_commands=["python $TRAINML_MODEL_PATH/tensorflow/main.py"],
-            environment=dict(type="DEEPLEARNING_PY39"),
             data=dict(
                 datasets=[
                     dict(
-                        name="CIFAR-10",
-                        type="public",
+                        id="CIFAR-10",
+                        public=True,
                     )
                 ],
                 output_type="trainml",
             ),
             model=dict(source_type="trainml", source_uri=model.id),
         )
         await job.attach()
@@ -555,16 +564,16 @@
             ),
             worker_commands=[
                 "python $TRAINML_MODEL_PATH/tensorflow/main.py",
             ],
             data=dict(
                 datasets=[
                     dict(
-                        name="CIFAR-10",
-                        type="public",
+                        id="CIFAR-10",
+                        public=True,
                     )
                 ],
                 output_type="wasabi",
                 output_uri="s3://trainml-example/output/resnet_cifar10",
                 output_options=dict(
                     endpoint_url="https://s3.wasabisys.com", archive=False
                 ),
@@ -607,16 +616,16 @@
             ),
             worker_commands=[
                 "python $TRAINML_MODEL_PATH/pytorch/main.py",
             ],
             data=dict(
                 datasets=[
                     dict(
-                        name="CIFAR-10",
-                        type="public",
+                        id="CIFAR-10",
+                        public=True,
                     )
                 ],
             ),
         )
         assert job.id
         await job.attach()
         await job.refresh()
@@ -658,21 +667,20 @@
         await job.disconnect()
         await job.remove()
         await job.wait_for("archived")
         captured = capsys.readouterr()
         sys.stdout.write(captured.out)
         sys.stderr.write(captured.err)
         upload_contents = os.listdir(temp_dir.name)
+        temp_dir.cleanup()
         assert len(upload_contents) > 4
-        result = any(
+        assert any(
             "model.ckpt-0002.data-00000-of-00001" in content
             for content in upload_contents
         )
-        assert result is not None
-        temp_dir.cleanup()
 
         captured = capsys.readouterr()
         sys.stdout.write(captured.out)
         sys.stderr.write(captured.err)
         assert "Epoch 1/2" in captured.out
         assert "Epoch 2/2" in captured.out
         assert "Number of regular files transferred: 7" in captured.out
```

### Comparing `trainml-0.4.8/tests/integration/test_models_integration.py` & `trainml-0.4.9/tests/integration/test_models_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/integration/test_projects_integration.py` & `trainml-0.4.9/tests/integration/test_projects_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/integration/test_providers_integration.py` & `trainml-0.4.9/tests/integration/test_providers_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/unit/cli/test_cli_environment_unit.py` & `trainml-0.4.9/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/unit/conftest.py` & `trainml-0.4.9/tests/unit/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from trainml.projects import Projects
 from pytest import fixture, mark
 from unittest.mock import Mock, AsyncMock, patch, create_autospec
 
 from trainml.trainml import TrainML
 from trainml.auth import Auth
 from trainml.datasets import Dataset, Datasets
+from trainml.checkpoints import Checkpoint, Checkpoints
 from trainml.models import Model, Models
 from trainml.gpu_types import GpuType, GpuTypes
 from trainml.environments import Environment, Environments
 from trainml.jobs import Job, Jobs
 from trainml.connections import Connections
 from trainml.projects import Projects, Project
 from trainml.providers import Providers, Provider
@@ -20,60 +21,60 @@
 @fixture(scope="session")
 def mock_my_datasets():
     trainml = Mock()
     yield [
         Dataset(
             trainml,
             dataset_uuid="1",
-            customer_uuid="cus-id-1",
+            project_uuid="proj-id-1",
             name="first one",
             status="ready",
             size=100000000,
             createdAt="2020-12-31T23:59:59.000Z",
         ),
         Dataset(
             trainml,
             dataset_uuid="2",
-            customer_uuid="cus-id-1",
+            project_uuid="proj-id-1",
             name="second one",
             status="ready",
             size=100000000,
             createdAt="2021-01-01T00:00:01.000Z",
         ),
         Dataset(
             trainml,
             dataset_uuid="3",
-            customer_uuid="cus-id-1",
+            project_uuid="proj-id-1",
             name="first one",
             status="ready",
             size=100000000,
             createdAt="2021-01-01T00:00:01.000Z",
         ),
         Dataset(
             trainml,
             dataset_uuid="4",
-            customer_uuid="cus-id-1",
+            project_uuid="proj-id-1",
             name="other one",
             status="ready",
             size=100000000,
             createdAt="2020-12-31T23:59:59.000Z",
         ),
         Dataset(
             trainml,
             dataset_uuid="5",
-            customer_uuid="cus-id-1",
+            project_uuid="proj-id-1",
             name="not ready",
             status="new",
             size=100000000,
             createdAt="2021-01-01T00:00:01.000Z",
         ),
         Dataset(
             trainml,
             dataset_uuid="6",
-            customer_uuid="cus-id-1",
+            project_uuid="proj-id-1",
             name="failed",
             status="failed",
             size=100000000,
             createdAt="2021-01-01T00:00:01.000Z",
         ),
     ]
 
@@ -106,48 +107,140 @@
             name="failed",
             status="failed",
         ),
     ]
 
 
 @fixture(scope="session")
+def mock_my_checkpoints():
+    trainml = Mock()
+    yield [
+        Checkpoint(
+            trainml,
+            checkpoint_uuid="1",
+            project_uuid="proj-id-1",
+            name="first one",
+            status="ready",
+            size=100000000,
+            createdAt="2020-12-31T23:59:59.000Z",
+        ),
+        Checkpoint(
+            trainml,
+            checkpoint_uuid="2",
+            project_uuid="proj-id-1",
+            name="second one",
+            status="ready",
+            size=100000000,
+            createdAt="2021-01-01T00:00:01.000Z",
+        ),
+        Checkpoint(
+            trainml,
+            checkpoint_uuid="3",
+            project_uuid="proj-id-1",
+            name="first one",
+            status="ready",
+            size=100000000,
+            createdAt="2021-01-01T00:00:01.000Z",
+        ),
+        Checkpoint(
+            trainml,
+            checkpoint_uuid="4",
+            project_uuid="proj-id-1",
+            name="other one",
+            status="ready",
+            size=100000000,
+            createdAt="2020-12-31T23:59:59.000Z",
+        ),
+        Checkpoint(
+            trainml,
+            checkpoint_uuid="5",
+            project_uuid="proj-id-1",
+            name="not ready",
+            status="new",
+            size=100000000,
+            createdAt="2021-01-01T00:00:01.000Z",
+        ),
+        Checkpoint(
+            trainml,
+            checkpoint_uuid="6",
+            project_uuid="proj-id-1",
+            name="failed",
+            status="failed",
+            size=100000000,
+            createdAt="2021-01-01T00:00:01.000Z",
+        ),
+    ]
+
+
+@fixture(scope="session")
+def mock_public_checkpoints():
+    trainml = Mock()
+    yield [
+        Checkpoint(
+            trainml,
+            checkpoint_uuid="11",
+            name="first one",
+            status="ready",
+        ),
+        Checkpoint(
+            trainml,
+            checkpoint_uuid="12",
+            name="second one",
+            status="ready",
+        ),
+        Checkpoint(
+            trainml,
+            checkpoint_uuid="15",
+            name="not ready",
+            status="new",
+        ),
+        Checkpoint(
+            trainml,
+            checkpoint_uuid="16",
+            name="failed",
+            status="failed",
+        ),
+    ]
+
+
+@fixture(scope="session")
 def mock_models():
     trainml = Mock()
     yield [
         Model(
             trainml,
             model_uuid="1",
-            customer_uuid="cus-id-1",
+            project_uuid="proj-id-1",
             name="first one",
             status="ready",
             size=10000000,
             createdAt="2020-12-31T23:59:59.000Z",
         ),
         Model(
             trainml,
             model_uuid="2",
-            customer_uuid="cus-id-1",
+            project_uuid="proj-id-1",
             name="second one",
             status="ready",
             size=10000000,
             createdAt="2021-01-01T00:00:01.000Z",
         ),
         Model(
             trainml,
             model_uuid="5",
-            customer_uuid="cus-id-1",
+            project_uuid="proj-id-1",
             name="not ready",
             status="new",
             size=10000000,
             createdAt="2021-01-01T00:00:01.000Z",
         ),
         Model(
             trainml,
             model_uuid="6",
-            customer_uuid="cus-id-1",
+            project_uuid="proj-id-1",
             name="failed",
             status="failed",
             size=10000000,
             createdAt="2021-01-01T00:00:01.000Z",
         ),
     ]
 
@@ -291,19 +384,19 @@
 @fixture(scope="session")
 def mock_jobs():
     trainml = Mock()
     yield [
         Job(
             trainml,
             **{
-                "customer_uuid": "cus-id-1",
+                "project_uuid": "proj-id-1",
                 "job_uuid": "job-id-1",
                 "name": "test notebook",
                 "start": "2021-02-11T15:46:22.455Z",
-                "type": "interactive",
+                "type": "notebook",
                 "status": "new",
                 "credits_per_hour": 0.1,
                 "credits": 0.1007,
                 "workers": [
                     {
                         "rig_uuid": "rig-id-1",
                         "job_worker_uuid": "worker-id-1",
@@ -315,15 +408,16 @@
                 "resources": {
                     "gpu_count": 1,
                     "gpu_type_id": "1060-id",
                     "disk_size": 10,
                 },
                 "model": {
                     "size": 7176192,
-                    "git_uri": "git@github.com:trainML/test-private.git",
+                    "source_type": "git",
+                    "source_uri": "git@github.com:trainML/test-private.git",
                     "status": "new",
                 },
                 "data": {
                     "datasets": [
                         {
                             "dataset_uuid": "data-id-1",
                             "name": "first one",
@@ -361,21 +455,21 @@
                 },
                 "nb_token": "token",
             },
         ),
         Job(
             trainml,
             **{
-                "customer_uuid": "cus-id-1",
+                "project_uuid": "proj-id-1",
                 "job_uuid": "job-id-2",
                 "name": "test training",
                 "start": "2021-02-11T15:48:39.476Z",
                 "stop": "2021-02-11T15:50:16.554Z",
-                "type": "headless",
-                "status": "stopped",
+                "type": "training",
+                "status": "finished",
                 "credits_per_hour": 0.3,
                 "credits": 0.0054,
                 "workers": [
                     {
                         "rig_uuid": "rig-id-1",
                         "job_worker_uuid": "worker-id-11",
                         "command": "PYTHONPATH=$PYTHONPATH:$TRAINML_MODEL_PATH python -m official.vision.image_classification.resnet_cifar_main --num_gpus=1 --data_dir=$TRAINML_DATA_PATH --model_dir=$TRAINML_OUTPUT_PATH --enable_checkpoint_and_export=True --train_epochs=1 --batch_size=1024",
@@ -398,15 +492,16 @@
                 "resources": {
                     "gpu_count": 1,
                     "gpu_type_id": "1060-id",
                     "disk_size": 10,
                 },
                 "model": {
                     "size": 7086080,
-                    "git_uri": "git@github.com:trainML/test-private.git",
+                    "source_type": "git",
+                    "source_uri": "git@github.com:trainML/test-private.git",
                     "status": "ready",
                 },
                 "data": {
                     "datasets": [
                         {
                             "dataset_uuid": "data-id-1",
                             "name": "first one",
@@ -443,15 +538,15 @@
 @fixture(scope="session")
 def mock_projects():
     trainml = Mock()
     yield [
         Project(
             trainml,
             **{
-                "id": "cus-id-1",
+                "id": "proj-id-1",
                 "name": "Personal",
                 "owner": True,
                 "owner_name": "Me",
                 "created_name": "Me",
                 "job_all": True,
                 "dataset_all": True,
                 "model_all": True,
@@ -530,26 +625,31 @@
     mock_gpu_types,
     mock_environments,
     mock_jobs,
     mock_projects,
     mock_providers,
 ):
     trainml = create_autospec(TrainML)
-    trainml.active_project = "proj-id-a"
-    trainml.project = "proj-id-a"
+    trainml.active_project = "proj-id-1"
+    trainml.project = "proj-id-1"
     trainml.datasets = create_autospec(Datasets)
+    trainml.checkpoints = create_autospec(Checkpoints)
     trainml.models = create_autospec(Models)
     trainml.gpu_types = create_autospec(GpuTypes)
     trainml.environments = create_autospec(Environments)
     trainml.jobs = create_autospec(Jobs)
     trainml.connections = create_autospec(Connections)
     trainml.projects = create_autospec(Projects)
     trainml.providers = create_autospec(Providers)
     trainml.datasets.list = AsyncMock(return_value=mock_my_datasets)
     trainml.datasets.list_public = AsyncMock(return_value=mock_public_datasets)
+    trainml.checkpoints.list = AsyncMock(return_value=mock_my_checkpoints)
+    trainml.checkpoints.list_public = AsyncMock(
+        return_value=mock_public_checkpoints
+    )
     trainml.models.list = AsyncMock(return_value=mock_models)
     trainml.gpu_types.list = AsyncMock(return_value=mock_gpu_types)
     trainml.environments.list = AsyncMock(return_value=mock_environments)
     trainml.jobs.list = AsyncMock(return_value=mock_jobs)
     trainml.projects.list = AsyncMock(return_value=mock_projects)
     trainml.providers.list = AsyncMock(return_value=mock_providers)
     yield trainml
```

### Comparing `trainml-0.4.8/tests/unit/test_auth.py` & `trainml-0.4.9/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/unit/test_checkpoints_unit.py` & `trainml-0.4.9/tests/unit/test_checkpoints_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 @fixture
 def checkpoint(mock_trainml):
     yield specimen.Checkpoint(
         mock_trainml,
         checkpoint_uuid="1",
-        project_uuid="proj-id-a",
+        project_uuid="proj-id-1",
         name="first one",
         status="new",
         size=100000,
         createdAt="2020-12-31T23:59:59.000Z",
     )
 
 
@@ -74,21 +74,21 @@
     async def test_create_checkpoint_simple(self, checkpoints, mock_trainml):
         requested_config = dict(
             name="new checkpoint",
             source_type="aws",
             source_uri="s3://trainml-examples/checkpoints/resnet50",
         )
         expected_payload = dict(
-            project_uuid="proj-id-a",
+            project_uuid="proj-id-1",
             name="new checkpoint",
             source_type="aws",
             source_uri="s3://trainml-examples/checkpoints/resnet50",
         )
         api_response = {
-            "customer_uuid": "cus-id-1",
+            "project_uuid": "cus-id-1",
             "checkpoint_uuid": "checkpoint-id-1",
             "name": "new checkpoint",
             "status": "new",
             "source_type": "aws",
             "source_uri": "s3://trainml-examples/checkpoints/resnet50",
             "createdAt": "2020-12-20T16:46:23.909Z",
         }
@@ -132,15 +132,15 @@
     @mark.asyncio
     async def test_checkpoint_get_log_url(self, checkpoint, mock_trainml):
 
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/logs/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await checkpoint.get_log_url()
         mock_trainml._query.assert_called_once_with(
-            "/checkpoint/1/logs", "GET", dict(project_uuid="proj-id-a")
+            "/checkpoint/1/logs", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_checkpoint_get_details(self, checkpoint, mock_trainml):
 
         api_response = {
@@ -149,28 +149,28 @@
             "count": "8",
             "size": "177M",
             "contents": [],
         }
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await checkpoint.get_details()
         mock_trainml._query.assert_called_once_with(
-            "/checkpoint/1/details", "GET", dict(project_uuid="proj-id-a")
+            "/checkpoint/1/details", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_checkpoint_get_connection_utility_url(
         self, checkpoint, mock_trainml
     ):
 
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/vpn/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await checkpoint.get_connection_utility_url()
         mock_trainml._query.assert_called_once_with(
-            "/checkpoint/1/download", "GET", dict(project_uuid="proj-id-a")
+            "/checkpoint/1/download", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     def test_checkpoint_get_connection_details_no_vpn(self, checkpoint):
         details = checkpoint.get_connection_details()
         expected_details = dict()
         assert details == expected_details
@@ -237,15 +237,15 @@
     async def test_checkpoint_remove(self, checkpoint, mock_trainml):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await checkpoint.remove()
         mock_trainml._query.assert_called_once_with(
             "/checkpoint/1",
             "DELETE",
-            dict(project_uuid="proj-id-a", force=False),
+            dict(project_uuid="proj-id-1", force=False),
         )
 
     def test_checkpoint_default_ws_msg_handler(self, checkpoint, capsys):
         data = {
             "msg": "download: s3://trainml-examples/data/cifar10/data_batch_2.bin to ./data_batch_2.bin\n",
             "time": 1613079345318,
             "type": "subscription",
@@ -327,15 +327,15 @@
             "source_type": "aws",
             "source_uri": "s3://trainml-examples/data/cifar10",
             "createdAt": "2020-12-20T16:46:23.909Z",
         }
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await checkpoint.refresh()
         mock_trainml._query.assert_called_once_with(
-            f"/checkpoint/1", "GET", dict(project_uuid="proj-id-a")
+            f"/checkpoint/1", "GET", dict(project_uuid="proj-id-1")
         )
         assert checkpoint.id == "data-id-1"
         assert response.id == "data-id-1"
 
     @mark.asyncio
     async def test_checkpoint_wait_for_successful(
         self, checkpoint, mock_trainml
@@ -348,15 +348,15 @@
             "source_type": "aws",
             "source_uri": "s3://trainml-examples/data/cifar10",
             "createdAt": "2020-12-20T16:46:23.909Z",
         }
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await checkpoint.wait_for("ready")
         mock_trainml._query.assert_called_once_with(
-            f"/checkpoint/1", "GET", dict(project_uuid="proj-id-a")
+            f"/checkpoint/1", "GET", dict(project_uuid="proj-id-1")
         )
         assert checkpoint.id == "data-id-1"
         assert response.id == "data-id-1"
 
     @mark.asyncio
     async def test_checkpoint_wait_for_current_status(self, mock_trainml):
         checkpoint = specimen.Checkpoint(
```

### Comparing `trainml-0.4.8/tests/unit/test_connections_unit.py` & `trainml-0.4.9/tests/unit/test_connections_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     yield specimen.Connection(
         mock_trainml,
         entity_type="dataset",
         id="data-id-1",
         entity=DatasetMock(
             mock_trainml,
             dataset_uuid="data-id-1",
-            project_uuid="proj-id-a",
+            project_uuid="proj-id-1",
             name="first one",
             status="new",
         ),
     )
 
 
 @fixture
@@ -48,15 +48,15 @@
         mock_trainml,
         entity_type="job",
         id="job-id-1",
         entity=JobMock(
             mock_trainml,
             **{
                 "customer_uuid": "cus-id-1",
-                "project_uuid": "proj-id-a",
+                "project_uuid": "proj-id-1",
                 "job_uuid": "job-id-1",
                 "name": "test notebook",
                 "type": "interactive",
                 "status": "new",
             },
         ),
     )
@@ -91,22 +91,22 @@
 
             with patch(
                 "trainml.connections._cleanup_containers"
             ) as mock_cleanup:
                 await connections.cleanup_connections()
                 assert mock_cleanup.mock_calls == [
                     call(
-                        "proj-id-a",
-                        os.path.expanduser("~/.trainml/connections/proj-id-a"),
+                        "proj-id-1",
+                        os.path.expanduser("~/.trainml/connections/proj-id-1"),
                         dir_list,
                         "vpn",
                     ),
                     call(
-                        "proj-id-a",
-                        os.path.expanduser("~/.trainml/connections/proj-id-a"),
+                        "proj-id-1",
+                        os.path.expanduser("~/.trainml/connections/proj-id-1"),
                         dir_list,
                         "storage",
                     ),
                 ]
 
     @mark.asyncio
     async def test_connections_cleanup_containers(
@@ -123,27 +123,27 @@
                 ]
                 containers[0].id = "keep-me"
                 containers[1].id = "delete-me"
                 docker = mock_docker.return_value
                 docker.containers = AsyncMock()
                 docker.containers.list = AsyncMock(return_value=containers)
                 await specimen._cleanup_containers(
-                    "proj-id-a",
-                    os.path.expanduser("~/.trainml/connections/proj-id-a"),
+                    "proj-id-1",
+                    os.path.expanduser("~/.trainml/connections/proj-id-1"),
                     ["dir_1"],
                     "job",
                 )
                 docker.containers.list.assert_called_once_with(
                     all=True,
                     filters=json.dumps(
                         dict(
                             label=[
                                 "service=trainml",
                                 "type=job",
-                                "project=proj-id-a",
+                                "project=proj-id-1",
                             ]
                         )
                     ),
                 )
                 containers[0].delete.assert_not_called
                 containers[1].delete.assert_called_once_with(force=True)
```

### Comparing `trainml-0.4.8/tests/unit/test_datasets_unit.py` & `trainml-0.4.9/tests/unit/test_datasets_unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 @fixture
 def dataset(mock_trainml):
     yield specimen.Dataset(
         mock_trainml,
         dataset_uuid="1",
-        project_uuid="proj-id-a",
+        project_uuid="proj-id-1",
         name="first one",
         status="new",
         size=100000,
         createdAt="2020-12-31T23:59:59.000Z",
     )
 
 
@@ -41,85 +41,85 @@
         datasets,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await datasets.get("1234")
         mock_trainml._query.assert_called_once_with(
-            "/dataset/pub/1234",
+            "/dataset/1234",
             "GET",
         )
 
     @mark.asyncio
     async def test_list_datasets(
         self,
         datasets,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await datasets.list()
         mock_trainml._query.assert_called_once_with(
-            "/dataset/pub",
+            "/dataset",
             "GET",
         )
 
     @mark.asyncio
     async def test_list_public_datasets(self, datasets, mock_trainml):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await datasets.list_public()
         mock_trainml._query.assert_called_once_with(
-            "/dataset/pub/public",
+            "/dataset/public",
             "GET",
         )
 
     @mark.asyncio
     async def test_remove_dataset(
         self,
         datasets,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await datasets.remove("4567")
         mock_trainml._query.assert_called_once_with(
-            "/dataset/pub/4567",
+            "/dataset/4567",
             "DELETE",
             dict(force=True),
         )
 
     @mark.asyncio
     async def test_create_dataset_simple(self, datasets, mock_trainml):
         requested_config = dict(
             name="new dataset",
             source_type="aws",
             source_uri="s3://trainml-examples/data/cifar10",
         )
         expected_payload = dict(
-            project_uuid="proj-id-a",
+            project_uuid="proj-id-1",
             name="new dataset",
             source_type="aws",
             source_uri="s3://trainml-examples/data/cifar10",
         )
         api_response = {
             "customer_uuid": "cus-id-1",
-            "project_uuid": "proj-id-a",
+            "project_uuid": "proj-id-1",
             "dataset_uuid": "data-id-1",
             "name": "new dataset",
             "status": "new",
             "source_type": "aws",
             "source_uri": "s3://trainml-examples/data/cifar10",
             "createdAt": "2020-12-20T16:46:23.909Z",
         }
 
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await datasets.create(**requested_config)
         mock_trainml._query.assert_called_once_with(
-            "/dataset/pub", "POST", None, expected_payload
+            "/dataset", "POST", None, expected_payload
         )
         assert response.id == "data-id-1"
 
 
 class DatasetTests:
     def test_dataset_properties(self, dataset):
         assert isinstance(dataset.id, str)
@@ -151,15 +151,15 @@
     @mark.asyncio
     async def test_dataset_get_log_url(self, dataset, mock_trainml):
 
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/logs/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await dataset.get_log_url()
         mock_trainml._query.assert_called_once_with(
-            "/dataset/pub/1/logs", "GET", dict(project_uuid="proj-id-a")
+            "/dataset/1/logs", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_dataset_get_details(self, dataset, mock_trainml):
 
         api_response = {
@@ -168,41 +168,41 @@
             "count": "8",
             "size": "177M",
             "contents": [],
         }
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await dataset.get_details()
         mock_trainml._query.assert_called_once_with(
-            "/dataset/pub/1/details", "GET", dict(project_uuid="proj-id-a")
+            "/dataset/1/details", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_dataset_get_connection_utility_url(
         self, dataset, mock_trainml
     ):
 
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/vpn/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await dataset.get_connection_utility_url()
         mock_trainml._query.assert_called_once_with(
-            "/dataset/pub/1/download", "GET", dict(project_uuid="proj-id-a")
+            "/dataset/1/download", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     def test_dataset_get_connection_details_no_vpn(self, dataset):
         details = dataset.get_connection_details()
         expected_details = dict()
         assert details == expected_details
 
     def test_dataset_get_connection_details_local_data(self, mock_trainml):
         dataset = specimen.Dataset(
             mock_trainml,
             dataset_uuid="1",
-            project_uuid="proj-id-a",
+            project_uuid="proj-id-1",
             name="first one",
             status="new",
             size=100000,
             createdAt="2020-12-31T23:59:59.000Z",
             source_type="local",
             source_uri="~/tensorflow-example/data",
             vpn={
@@ -214,15 +214,15 @@
                     "address": "10.106.171.253",
                     "ssh_port": 46600,
                 },
             },
         )
         details = dataset.get_connection_details()
         expected_details = dict(
-            project_uuid="proj-id-a",
+            project_uuid="proj-id-1",
             entity_type="dataset",
             cidr="10.106.171.0/24",
             ssh_port=46600,
             input_path="~/tensorflow-example/data",
             output_path=None,
         )
         assert details == expected_details
@@ -253,17 +253,17 @@
 
     @mark.asyncio
     async def test_dataset_remove(self, dataset, mock_trainml):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await dataset.remove()
         mock_trainml._query.assert_called_once_with(
-            "/dataset/pub/1",
+            "/dataset/1",
             "DELETE",
-            dict(project_uuid="proj-id-a", force=False),
+            dict(project_uuid="proj-id-1", force=False),
         )
 
     def test_dataset_default_ws_msg_handler(self, dataset, capsys):
 
         data = {
             "msg": "download: s3://trainml-examples/data/cifar10/data_batch_2.bin to ./data_batch_2.bin\n",
             "time": 1613079345318,
@@ -346,15 +346,15 @@
             "source_type": "aws",
             "source_uri": "s3://trainml-examples/data/cifar10",
             "createdAt": "2020-12-20T16:46:23.909Z",
         }
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await dataset.refresh()
         mock_trainml._query.assert_called_once_with(
-            f"/dataset/pub/1", "GET", dict(project_uuid="proj-id-a")
+            f"/dataset/1", "GET", dict(project_uuid="proj-id-1")
         )
         assert dataset.id == "data-id-1"
         assert response.id == "data-id-1"
 
     @mark.asyncio
     async def test_dataset_wait_for_successful(self, dataset, mock_trainml):
         api_response = {
@@ -365,15 +365,15 @@
             "source_type": "aws",
             "source_uri": "s3://trainml-examples/data/cifar10",
             "createdAt": "2020-12-20T16:46:23.909Z",
         }
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await dataset.wait_for("ready")
         mock_trainml._query.assert_called_once_with(
-            f"/dataset/pub/1", "GET", dict(project_uuid="proj-id-a")
+            f"/dataset/1", "GET", dict(project_uuid="proj-id-1")
         )
         assert dataset.id == "data-id-1"
         assert response.id == "data-id-1"
 
     @mark.asyncio
     async def test_dataset_wait_for_current_status(self, mock_trainml):
         dataset = specimen.Dataset(
@@ -465,8 +465,8 @@
         self, dataset, mock_trainml
     ):
         mock_trainml._query = AsyncMock(
             side_effect=ApiError(404, dict(errorMessage="Dataset Not Found"))
         )
         with raises(ApiError):
             await dataset.wait_for("ready")
-        mock_trainml._query.assert_called()
+        mock_trainml._query.assert_called()
```

### Comparing `trainml-0.4.8/tests/unit/test_environments_unit.py` & `trainml-0.4.9/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/unit/test_exceptions.py` & `trainml-0.4.9/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/unit/test_gpu_types_unit.py` & `trainml-0.4.9/tests/unit/test_gpu_types_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         gpu_types,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await gpu_types.list()
         mock_trainml._query.assert_called_once_with(
-            f"/project/proj-id-a/gputypes", "GET"
+            f"/project/proj-id-1/gputypes", "GET"
         )
 
 
 class GpuTypeTests:
     def test_gpu_type_properties(self, gpu_type):
         assert isinstance(gpu_type.id, str)
         assert isinstance(gpu_type.name, str)
```

### Comparing `trainml-0.4.8/tests/unit/test_jobs_unit.py` & `trainml-0.4.9/tests/unit/test_jobs_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,71 +168,14 @@
                     "address": "10.106.171.253",
                 },
             },
         },
     )
 
 
-class CleanDatasetSelectionTests:
-    @mark.parametrize(
-        "datasets,expected",
-        [
-            (
-                [dict(id="1", type="existing")],
-                [dict(id="1", type="existing")],
-            ),
-            (
-                [dict(name="first one", type="existing")],
-                [dict(id="first one", type="existing")],
-            ),
-            (
-                [dict(dataset_uuid="3", type="existing")],
-                [dict(dataset_uuid="3", type="existing")],
-            ),
-            (
-                [dict(name="first one", type="public")],
-                [dict(id="first one", type="public")],
-            ),
-            (
-                [
-                    dict(id="1", type="existing"),
-                    dict(name="second one", type="existing"),
-                    dict(id="11", type="public"),
-                    dict(name="second one", type="public"),
-                ],
-                [
-                    dict(id="1", type="existing"),
-                    dict(id="second one", type="existing"),
-                    dict(id="11", type="public"),
-                    dict(id="second one", type="public"),
-                ],
-            ),
-        ],
-    )
-    def test_clean_datasets_selection_successful(
-        self,
-        datasets,
-        expected,
-    ):
-        result = specimen._clean_datasets_selection(datasets)
-        assert result == expected
-
-    def test_invalid_dataset_type_specified(self):
-        with raises(SpecificationError):
-            specimen._clean_datasets_selection(
-                [dict(name="Not Found", type="invalid")],
-            )
-
-    def test_invalid_dataset_identifier_specified(self):
-        with raises(SpecificationError):
-            specimen._clean_datasets_selection(
-                [dict(dataset_id="Not Found", type="existing")],
-            )
-
-
 @mark.asyncio
 class JobsTests:
     async def test_jobs_get(
         self,
         jobs,
         mock_trainml,
     ):
@@ -272,21 +215,20 @@
             name="job_name",
             type="notebook",
             gpu_type="GTX 1060",
             gpu_count=1,
             disk_size=10,
         )
         expected_payload = dict(
-            project_uuid="proj-id-a",
+            project_uuid="proj-id-1",
             name="job_name",
             type="notebook",
             resources=dict(
                 gpu_type_id="GTX 1060", gpu_count=1, disk_size=10, max_price=10
             ),
-            environment=dict(type="DEEPLEARNING_PY39"),
             model=dict(),
             worker_commands=[],
         )
 
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await jobs.create(**requested_config)
@@ -309,15 +251,15 @@
             worker_commands=None,
             environment=None,
             data=None,
             source_job_uuid="job-id-1",
         )
         expected_payload = dict(
             name="job_name",
-            project_uuid="proj-id-a",
+            project_uuid="proj-id-1",
             type="notebook",
             resources=dict(
                 gpu_type_id="1060-id", gpu_count=1, disk_size=10, max_price=2
             ),
             source_job_uuid="job-id-1",
         )
 
@@ -720,14 +662,15 @@
             "cpu_count": None,
             "disk_size": 10,
             "max_price": 10,
             "worker_commands": None,
             "workers": None,
             "environment": None,
             "data": None,
+            "model": None,
             "source_job_uuid": "job-id-1",
         }
 
         api_response = specimen.Job(
             mock_trainml,
             **{
                 "customer_uuid": "cus-id-1",
@@ -871,8 +814,8 @@
     @mark.asyncio
     async def test_job_wait_for_unexpected_api_error(self, job, mock_trainml):
         mock_trainml._query = AsyncMock(
             side_effect=ApiError(404, dict(errorMessage="Job Not Found"))
         )
         with raises(ApiError):
             await job.wait_for("running")
-        mock_trainml._query.assert_called()
+        mock_trainml._query.assert_called()
```

### Comparing `trainml-0.4.8/tests/unit/test_models_unit.py` & `trainml-0.4.9/tests/unit/test_models_unit.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 @fixture
 def model(mock_trainml):
     yield specimen.Model(
         mock_trainml,
         model_uuid="1",
-        project_uuid="proj-id-a",
+        project_uuid="proj-id-1",
         name="first one",
         status="new",
         size=100000,
         createdAt="2020-12-31T23:59:59.000Z",
     )
 
 
@@ -40,49 +40,49 @@
         self,
         models,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await models.get("1234")
-        mock_trainml._query.assert_called_once_with("/model/pub/1234", "GET")
+        mock_trainml._query.assert_called_once_with("/model/1234", "GET")
 
     @mark.asyncio
     async def test_list_models(
         self,
         models,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await models.list()
-        mock_trainml._query.assert_called_once_with("/model/pub", "GET")
+        mock_trainml._query.assert_called_once_with("/model", "GET")
 
     @mark.asyncio
     async def test_remove_model(
         self,
         models,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await models.remove("4567")
         mock_trainml._query.assert_called_once_with(
-            "/model/pub/4567", "DELETE", dict(force=True)
+            "/model/4567", "DELETE", dict(force=True)
         )
 
     @mark.asyncio
     async def test_create_model_simple(self, models, mock_trainml):
         requested_config = dict(
             name="new model",
             source_type="aws",
             source_uri="s3://trainml-examples/models/resnet50",
         )
         expected_payload = dict(
-            project_uuid="proj-id-a",
+            project_uuid="proj-id-1",
             name="new model",
             source_type="aws",
             source_uri="s3://trainml-examples/models/resnet50",
         )
         api_response = {
             "customer_uuid": "cus-id-1",
             "model_uuid": "model-id-1",
@@ -92,15 +92,15 @@
             "source_uri": "s3://trainml-examples/models/resnet50",
             "createdAt": "2020-12-20T16:46:23.909Z",
         }
 
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await models.create(**requested_config)
         mock_trainml._query.assert_called_once_with(
-            "/model/pub", "POST", None, expected_payload
+            "/model", "POST", None, expected_payload
         )
         assert response.id == "model-id-1"
 
 
 class ModelTests:
     def test_model_properties(self, model):
         assert isinstance(model.id, str)
@@ -132,15 +132,15 @@
     @mark.asyncio
     async def test_model_get_log_url(self, model, mock_trainml):
 
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/logs/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await model.get_log_url()
         mock_trainml._query.assert_called_once_with(
-            "/model/pub/1/logs", "GET", dict(project_uuid="proj-id-a")
+            "/model/1/logs", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_model_get_details(self, model, mock_trainml):
 
         api_response = {
@@ -149,26 +149,26 @@
             "count": "8",
             "size": "177M",
             "contents": [],
         }
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await model.get_details()
         mock_trainml._query.assert_called_once_with(
-            "/model/pub/1/details", "GET", dict(project_uuid="proj-id-a")
+            "/model/1/details", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_model_get_connection_utility_url(self, model, mock_trainml):
 
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/vpn/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await model.get_connection_utility_url()
         mock_trainml._query.assert_called_once_with(
-            "/model/pub/1/download", "GET", dict(project_uuid="proj-id-a")
+            "/model/1/download", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     def test_model_get_connection_details_no_vpn(self, model):
         details = model.get_connection_details()
         expected_details = dict()
         assert details == expected_details
@@ -233,17 +233,17 @@
 
     @mark.asyncio
     async def test_model_remove(self, model, mock_trainml):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await model.remove()
         mock_trainml._query.assert_called_once_with(
-            "/model/pub/1",
+            "/model/1",
             "DELETE",
-            dict(project_uuid="proj-id-a", force=False),
+            dict(project_uuid="proj-id-1", force=False),
         )
 
     def test_model_default_ws_msg_handler(self, model, capsys):
         data = {
             "msg": "download: s3://trainml-examples/data/cifar10/data_batch_2.bin to ./data_batch_2.bin\n",
             "time": 1613079345318,
             "type": "subscription",
@@ -325,15 +325,15 @@
             "source_type": "aws",
             "source_uri": "s3://trainml-examples/data/cifar10",
             "createdAt": "2020-12-20T16:46:23.909Z",
         }
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await model.refresh()
         mock_trainml._query.assert_called_once_with(
-            f"/model/pub/1", "GET", dict(project_uuid="proj-id-a")
+            f"/model/1", "GET", dict(project_uuid="proj-id-1")
         )
         assert model.id == "data-id-1"
         assert response.id == "data-id-1"
 
     @mark.asyncio
     async def test_model_wait_for_successful(self, model, mock_trainml):
         api_response = {
@@ -344,15 +344,15 @@
             "source_type": "aws",
             "source_uri": "s3://trainml-examples/data/cifar10",
             "createdAt": "2020-12-20T16:46:23.909Z",
         }
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await model.wait_for("ready")
         mock_trainml._query.assert_called_once_with(
-            f"/model/pub/1", "GET", dict(project_uuid="proj-id-a")
+            f"/model/1", "GET", dict(project_uuid="proj-id-1")
         )
         assert model.id == "data-id-1"
         assert response.id == "data-id-1"
 
     @mark.asyncio
     async def test_model_wait_for_current_status(self, mock_trainml):
         model = specimen.Model(
@@ -440,8 +440,8 @@
         self, model, mock_trainml
     ):
         mock_trainml._query = AsyncMock(
             side_effect=ApiError(404, dict(errorMessage="Model Not Found"))
         )
         with raises(ApiError):
             await model.wait_for("ready")
-        mock_trainml._query.assert_called()
+        mock_trainml._query.assert_called()
```

### Comparing `trainml-0.4.8/tests/unit/test_projects_unit.py` & `trainml-0.4.9/tests/unit/test_projects_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/unit/test_providers_unit.py` & `trainml-0.4.9/tests/unit/test_providers_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/tests/unit/test_trainml.py` & `trainml-0.4.9/tests/unit/test_trainml.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/auth.py` & `trainml-0.4.9/trainml/auth.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/checkpoints.py` & `trainml-0.4.9/trainml/checkpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,19 @@
     async def list(self):
         resp = await self.trainml._query(f"/checkpoint", "GET")
         checkpoints = [
             Checkpoint(self.trainml, **checkpoint) for checkpoint in resp
         ]
         return checkpoints
 
+    async def list_public(self):
+        resp = await self.trainml._query(f"/checkpoint/public", "GET")
+        datasets = [Checkpoint(self.trainml, **dataset) for dataset in resp]
+        return datasets
+
     async def create(self, name, source_type, source_uri, **kwargs):
         data = dict(
             name=name,
             source_type=source_type,
             source_uri=source_uri,
             source_options=kwargs.get("source_options"),
             project_uuid=kwargs.get("project_uuid")
```

### Comparing `trainml-0.4.8/trainml/cli/__init__.py` & `trainml-0.4.9/trainml/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,7 +164,8 @@
 from trainml.cli.dataset import dataset
 from trainml.cli.model import model
 from trainml.cli.checkpoint import checkpoint
 from trainml.cli.environment import environment
 from trainml.cli.gpu import gpu
 from trainml.cli.job import job
 from trainml.cli.project import project
+from trainml.cli.provider import provider
```

### Comparing `trainml-0.4.8/trainml/cli/checkpoint.py` & `trainml-0.4.9/trainml/cli/checkpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,14 +184,43 @@
         click.echo(
             "{: >38.36} {: >13.11} {: >40.38} {: >14.12}" "".format(*row),
             file=config.stdout,
         )
 
 
 @checkpoint.command()
+@pass_config
+def list_public(config):
+    """List public checkpoints."""
+    data = [
+        ["ID", "STATUS", "NAME", "SIZE"],
+        ["-" * 80, "-" * 80, "-" * 80, "-" * 80],
+    ]
+
+    checkpoints = config.trainml.run(
+        config.trainml.client.checkpoints.list_public()
+    )
+
+    for ckpt in checkpoints:
+        data.append(
+            [
+                ckpt.id,
+                ckpt.status,
+                ckpt.name,
+                pretty_size(ckpt.size),
+            ]
+        )
+    for row in data:
+        click.echo(
+            "{: >38.36} {: >13.11} {: >40.38} {: >14.12}" "".format(*row),
+            file=config.stdout,
+        )
+
+
+@checkpoint.command()
 @click.option(
     "--force/--no-force",
     default=False,
     show_default=True,
     help="Force removal.",
 )
 @click.argument("checkpoint", type=click.STRING)
```

### Comparing `trainml-0.4.8/trainml/cli/connection.py` & `trainml-0.4.9/trainml/cli/connection.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/cli/dataset.py` & `trainml-0.4.9/trainml/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/cli/environment.py` & `trainml-0.4.9/trainml/cli/environment.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/cli/gpu.py` & `trainml-0.4.9/trainml/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/cli/job/__init__.py` & `trainml-0.4.9/trainml/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/cli/job/create.py` & `trainml-0.4.9/trainml/cli/job/create.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,14 +88,26 @@
 @click.option(
     "--public-dataset",
     type=click.STRING,
     help="ID or Name of a public dataset to add to the job",
     multiple=True,
 )
 @click.option(
+    "--checkpoint",
+    type=click.STRING,
+    help="ID or Name of a checkpoint to add to the job",
+    multiple=True,
+)
+@click.option(
+    "--public-checkpoint",
+    type=click.STRING,
+    help="ID or Name of a public checkpoint to add to the job",
+    multiple=True,
+)
+@click.option(
     "--environment",
     type=click.Choice(
         [
             "DEEPLEARNING_PY38",
             "DEEPLEARNING_PY39",
             "PYTORCH_PY39_113",
             "PYTORCH_PY39_112",
@@ -114,15 +126,14 @@
     show_default=True,
     help="Job environment to use",
 )
 @click.option(
     "--custom-image",
     type=click.STRING,
     help="Docker Image to use for the job.  Implies 'CUSTOM' environment type.",
-    multiple=True,
 )
 @click.option(
     "--env",
     type=click.STRING,
     help="Environment variables to set in the job environment in 'KEY=VALUE' format",
     multiple=True,
 )
@@ -181,14 +192,16 @@
     disk_size,
     gpu_count,
     gpu_type,
     max_price,
     data_dir,
     dataset,
     public_dataset,
+    checkpoint,
+    public_checkpoint,
     environment,
     custom_image,
     env,
     key,
     apt_packages,
     pip_packages,
     conda_packages,
@@ -198,27 +211,41 @@
     timeout,
     name,
 ):
     """
     Create a notebook.
     """
 
-    datasets = [dict(id=item, type="existing") for item in dataset] + [
-        dict(id=item, type="public") for item in public_dataset
-    ]
+    datasets = [
+        dict(
+            id=item,
+        )
+        for item in dataset
+    ] + [dict(id=item, public=True) for item in public_dataset]
+
+    checkpoints = [
+        dict(
+            id=item,
+        )
+        for item in checkpoint
+    ] + [dict(id=item, public=True) for item in public_checkpoint]
 
     options = dict(
         max_price=max_price,
         data=dict(datasets=datasets),
+        model=dict(checkpoints=checkpoints),
         environment=dict(
-            type="CUSTOM" if custom_image else environment,
-            custom_image=custom_image,
             worker_key_types=[k for k in key],
         ),
     )
+    if custom_image:
+        options["environment"]["type"] = "CUSTOM"
+        options["environment"]["custom_image"] = custom_image
+    else:
+        options["environment"]["type"] = environment
 
     try:
         envs = [
             {"key": e.split("=")[0], "value": e.split("=")[1]} for e in env
         ]
         options["environment"]["env"] = envs
     except IndexError:
@@ -252,19 +279,23 @@
             config.trainml.run(new_dataset.wait_for("ready"))
             config.trainml.run(new_dataset.disconnect())
         options["data"]["datasets"].append(
             dict(id=new_dataset.id, type="existing")
         )
 
     if git_uri:
-        options["model"] = dict(source_type="git", source_uri=git_uri)
+        options["model"]["source_type"] = "git"
+        options["model"]["source_uri"] = git_uri
     if model_id:
-        options["model"] = dict(source_type="trainml", source_uri=model_id)
+        options["model"]["source_type"] = "trainml"
+        options["model"]["source_uri"] = model_id
     if model_dir:
-        options["model"] = dict(source_type="local", source_uri=model_dir)
+        options["model"]["source_type"] = "local"
+        options["model"]["source_uri"] = model_dir
+
     job = config.trainml.run(
         config.trainml.client.jobs.create(
             name=name,
             type="notebook",
             gpu_types=gpu_type,
             gpu_count=gpu_count,
             disk_size=disk_size,
@@ -366,14 +397,26 @@
 @click.option(
     "--public-dataset",
     type=click.STRING,
     help="ID or Name of a public dataset to add to the job",
     multiple=True,
 )
 @click.option(
+    "--checkpoint",
+    type=click.STRING,
+    help="ID or Name of a checkpoint to add to the job",
+    multiple=True,
+)
+@click.option(
+    "--public-checkpoint",
+    type=click.STRING,
+    help="ID or Name of a public checkpoint to add to the job",
+    multiple=True,
+)
+@click.option(
     "--output-dir",
     type=click.Path(exists=True, file_okay=False, resolve_path=True),
     help="Local file path to save the output results to",
 )
 @click.option(
     "--output-type",
     type=click.Choice(
@@ -416,15 +459,14 @@
     show_default=True,
     help="Job environment to use",
 )
 @click.option(
     "--custom-image",
     type=click.STRING,
     help="Docker Image to use for the job.  Implies 'CUSTOM' environment type.",
-    multiple=True,
 )
 @click.option(
     "--env",
     type=click.STRING,
     help="Environment variables to set in the job environment in 'KEY=VALUE' format",
     multiple=True,
 )
@@ -481,14 +523,16 @@
     disk_size,
     gpu_count,
     gpu_type,
     max_price,
     data_dir,
     dataset,
     public_dataset,
+    checkpoint,
+    public_checkpoint,
     output_dir,
     output_type,
     output_uri,
     archive,
     environment,
     custom_image,
     env,
@@ -502,27 +546,41 @@
     name,
     commands,
 ):
     """
     Create a training job.
     """
 
-    datasets = [dict(id=item, type="existing") for item in dataset] + [
-        dict(id=item, type="public") for item in public_dataset
-    ]
+    datasets = [
+        dict(
+            id=item,
+        )
+        for item in dataset
+    ] + [dict(id=item, public=True) for item in public_dataset]
+
+    checkpoints = [
+        dict(
+            id=item,
+        )
+        for item in checkpoint
+    ] + [dict(id=item, public=True) for item in public_checkpoint]
 
     options = dict(
         max_price=max_price,
         data=dict(datasets=datasets),
+        model=dict(checkpoints=checkpoints),
         environment=dict(
-            type="CUSTOM" if custom_image else environment,
-            custom_image=custom_image,
             worker_key_types=[k for k in key],
         ),
     )
+    if custom_image:
+        options["environment"]["type"] = "CUSTOM"
+        options["environment"]["custom_image"] = custom_image
+    else:
+        options["environment"]["type"] = environment
 
     if output_type:
         options["data"]["output_type"] = output_type
         options["data"]["output_uri"] = output_uri
         if not archive:
             options["data"]["output_options"] = dict(archive=False)
 
@@ -568,19 +626,23 @@
             config.trainml.run(new_dataset.wait_for("ready"))
             config.trainml.run(new_dataset.disconnect())
         options["data"]["datasets"].append(
             dict(id=new_dataset.id, type="existing")
         )
 
     if git_uri:
-        options["model"] = dict(source_type="git", source_uri=git_uri)
+        options["model"]["source_type"] = "git"
+        options["model"]["source_uri"] = git_uri
     if model_id:
-        options["model"] = dict(source_type="trainml", source_uri=model_id)
+        options["model"]["source_type"] = "trainml"
+        options["model"]["source_uri"] = model_id
     if model_dir:
-        options["model"] = dict(source_type="local", source_uri=model_dir)
+        options["model"]["source_type"] = "local"
+        options["model"]["source_uri"] = model_dir
+
     job = config.trainml.run(
         config.trainml.client.jobs.create(
             name=name,
             type="training",
             gpu_type=gpu_type,
             gpu_count=gpu_count,
             disk_size=disk_size,
@@ -656,14 +718,26 @@
     "-mp",
     type=click.FLOAT,
     default=10.0,
     show_default=True,
     help="Max Price (per GPU).",
 )
 @click.option(
+    "--checkpoint",
+    type=click.STRING,
+    help="ID or Name of a checkpoint to add to the job",
+    multiple=True,
+)
+@click.option(
+    "--public-checkpoint",
+    type=click.STRING,
+    help="ID or Name of a public checkpoint to add to the job",
+    multiple=True,
+)
+@click.option(
     "--input-dir",
     type=click.Path(exists=True, file_okay=False, resolve_path=True),
     help="Local file path to copy as the input data",
 )
 @click.option(
     "--input-type",
     type=click.Choice(
@@ -724,15 +798,14 @@
     show_default=True,
     help="Job environment to use",
 )
 @click.option(
     "--custom-image",
     type=click.STRING,
     help="Docker Image to use for the job.  Implies 'CUSTOM' environment type.",
-    multiple=True,
 )
 @click.option(
     "--env",
     type=click.STRING,
     help="Environment variables to set in the job environment in 'KEY=VALUE' format",
     multiple=True,
 )
@@ -785,14 +858,16 @@
     config,
     attach,
     connect,
     disk_size,
     gpu_count,
     gpu_type,
     max_price,
+    checkpoint,
+    public_checkpoint,
     input_dir,
     input_type,
     input_uri,
     output_dir,
     output_type,
     output_uri,
     archive,
@@ -809,23 +884,34 @@
     name,
     command,
 ):
     """
     Create an inference job.
     """
 
+    checkpoints = [
+        dict(
+            id=item,
+        )
+        for item in checkpoint
+    ] + [dict(id=item, public=True) for item in public_checkpoint]
+
     options = dict(
         max_price=max_price,
         data=dict(datasets=[]),
+        model=dict(checkpoints=checkpoints),
         environment=dict(
-            type="CUSTOM" if custom_image else environment,
-            custom_image=custom_image,
             worker_key_types=[k for k in key],
         ),
     )
+    if custom_image:
+        options["environment"]["type"] = "CUSTOM"
+        options["environment"]["custom_image"] = custom_image
+    else:
+        options["environment"]["type"] = environment
 
     if input_type:
         options["data"]["input_type"] = input_type
         options["data"]["input_uri"] = input_uri
 
     if input_dir:
         options["data"]["input_type"] = "local"
@@ -861,19 +947,23 @@
             options["environment"]["packages"]["pip"] = pip_packages.split(",")
         if conda_packages:
             options["environment"]["packages"]["conda"] = conda_packages.split(
                 ","
             )
 
     if git_uri:
-        options["model"] = dict(source_type="git", source_uri=git_uri)
+        options["model"]["source_type"] = "git"
+        options["model"]["source_uri"] = git_uri
     if model_id:
-        options["model"] = dict(source_type="trainml", source_uri=model_id)
+        options["model"]["source_type"] = "trainml"
+        options["model"]["source_uri"] = model_id
     if model_dir:
-        options["model"] = dict(source_type="local", source_uri=model_dir)
+        options["model"]["source_type"] = "local"
+        options["model"]["source_uri"] = model_dir
+
     job = config.trainml.run(
         config.trainml.client.jobs.create(
             name=name,
             type="inference",
             gpu_type=gpu_type,
             gpu_count=gpu_count,
             disk_size=disk_size,
@@ -985,14 +1075,26 @@
     "-mp",
     type=click.FLOAT,
     default=10.0,
     show_default=True,
     help="Max Price (per GPU).",
 )
 @click.option(
+    "--checkpoint",
+    type=click.STRING,
+    help="ID or Name of a checkpoint to add to the job",
+    multiple=True,
+)
+@click.option(
+    "--public-checkpoint",
+    type=click.STRING,
+    help="ID or Name of a public checkpoint to add to the job",
+    multiple=True,
+)
+@click.option(
     "--environment",
     type=click.Choice(
         [
             "DEEPLEARNING_PY38",
             "DEEPLEARNING_PY39",
             "PYTORCH_PY39_113",
             "PYTORCH_PY39_112",
@@ -1011,15 +1113,14 @@
     show_default=True,
     help="Job environment to use",
 )
 @click.option(
     "--custom-image",
     type=click.STRING,
     help="Docker Image to use for the job.  Implies 'CUSTOM' environment type.",
-    multiple=True,
 )
 @click.option(
     "--env",
     type=click.STRING,
     help="Environment variables to set in the job environment in 'KEY=VALUE' format",
     multiple=True,
 )
@@ -1081,14 +1182,16 @@
     config,
     attach,
     connect,
     disk_size,
     gpu_count,
     gpu_type,
     max_price,
+    checkpoint,
+    public_checkpoint,
     environment,
     custom_image,
     env,
     key,
     apt_packages,
     pip_packages,
     conda_packages,
@@ -1098,24 +1201,35 @@
     route,
     timeout,
     name,
 ):
     """
     Create an endpoint.
     """
+    checkpoints = [
+        dict(
+            id=item,
+        )
+        for item in checkpoint
+    ] + [dict(id=item, public=True) for item in public_checkpoint]
+
     routes = [json.loads(item) for item in route]
 
     options = dict(
         max_price=max_price,
+        model=dict(checkpoints=checkpoints),
         environment=dict(
-            type="CUSTOM" if custom_image else environment,
-            custom_image=custom_image,
             worker_key_types=[k for k in key],
         ),
     )
+    if custom_image:
+        options["environment"]["type"] = "CUSTOM"
+        options["environment"]["custom_image"] = custom_image
+    else:
+        options["environment"]["type"] = environment
 
     try:
         envs = [
             {"key": e.split("=")[0], "value": e.split("=")[1]} for e in env
         ]
         options["environment"]["env"] = envs
     except IndexError:
@@ -1131,19 +1245,23 @@
             options["environment"]["packages"]["pip"] = pip_packages.split(",")
         if conda_packages:
             options["environment"]["packages"]["conda"] = conda_packages.split(
                 ","
             )
 
     if git_uri:
-        options["model"] = dict(source_type="git", source_uri=git_uri)
+        options["model"]["source_type"] = "git"
+        options["model"]["source_uri"] = git_uri
     if model_id:
-        options["model"] = dict(source_type="trainml", source_uri=model_id)
+        options["model"]["source_type"] = "trainml"
+        options["model"]["source_uri"] = model_id
     if model_dir:
-        options["model"] = dict(source_type="local", source_uri=model_dir)
+        options["model"]["source_type"] = "local"
+        options["model"]["source_uri"] = model_dir
+
     job = config.trainml.run(
         config.trainml.client.jobs.create(
             name=name,
             type="endpoint",
             gpu_type=gpu_type,
             gpu_count=gpu_count,
             disk_size=disk_size,
```

### Comparing `trainml-0.4.8/trainml/cli/model.py` & `trainml-0.4.9/trainml/cli/model.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/cli/project.py` & `trainml-0.4.9/trainml/cli/project.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/connections.py` & `trainml-0.4.9/trainml/connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,17 +400,17 @@
             )
         )
         logging.debug(f"VPN container started, id: {vpn_container.id}")
 
         with open(f"{self._dir}/vpn_id", "w") as f:
             f.write(vpn_container.id)
 
-        cleanup_task = asyncio.create_task(
-            self.trainml.connections.cleanup_connections()
-        )
+        # cleanup_task = asyncio.create_task(
+        #     self.trainml.connections.cleanup_connections()
+        # )
 
         count = 0
         while count <= 30:
             logging.debug(f"Test connectivity attempt {count+1}")
             res = await self._test_connection(vpn_container)
             if res:
                 logging.debug(f"Test connectivity successful {count+1}")
@@ -418,15 +418,15 @@
             count += 1
         await docker.close()
         if count > 30:
             self._status = STATUSES.get("NOT_CONNECTED")
             raise ConnectionError(f"Unable to connect {self.type} {self.id}")
         self._status = STATUSES.get("CONNECTED")
         logging.info(f"Connection Successful.")
-        await cleanup_task
+        # await cleanup_task
         logging.debug(f"Completed start {self.type} connection {self.id}")
 
     async def stop(self):
         logging.debug(f"Beginning stop {self.type} connection {self.id}")
         if not self._entity:
             await self._get_entity()
         docker = aiodocker.Docker()
```

### Comparing `trainml-0.4.8/trainml/datasets.py` & `trainml-0.4.9/trainml/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,48 +14,46 @@
 
 
 class Datasets(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
     async def get(self, id):
-        resp = await self.trainml._query(f"/dataset/pub/{id}", "GET")
+        resp = await self.trainml._query(f"/dataset/{id}", "GET")
         return Dataset(self.trainml, **resp)
 
     async def list(self):
-        resp = await self.trainml._query(f"/dataset/pub", "GET")
+        resp = await self.trainml._query(f"/dataset", "GET")
         datasets = [Dataset(self.trainml, **dataset) for dataset in resp]
         return datasets
 
     async def list_public(self):
-        resp = await self.trainml._query(f"/dataset/pub/public", "GET")
+        resp = await self.trainml._query(f"/dataset/public", "GET")
         datasets = [Dataset(self.trainml, **dataset) for dataset in resp]
         return datasets
 
     async def create(self, name, source_type, source_uri, **kwargs):
         data = dict(
             name=name,
             source_type=source_type,
             source_uri=source_uri,
             source_options=kwargs.get("source_options"),
             project_uuid=kwargs.get("project_uuid")
             or self.trainml.active_project,
         )
         payload = {k: v for k, v in data.items() if v}
         logging.info(f"Creating Dataset {name}")
-        resp = await self.trainml._query("/dataset/pub", "POST", None, payload)
+        resp = await self.trainml._query("/dataset", "POST", None, payload)
         dataset = Dataset(self.trainml, **resp)
         logging.info(f"Created Dataset {name} with id {dataset.id}")
 
         return dataset
 
     async def remove(self, id):
-        await self.trainml._query(
-            f"/dataset/pub/{id}", "DELETE", dict(force=True)
-        )
+        await self.trainml._query(f"/dataset/{id}", "DELETE", dict(force=True))
 
 
 class Dataset:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
         self._dataset = kwargs
         self._id = self._dataset.get("id", self._dataset.get("dataset_uuid"))
@@ -87,31 +85,31 @@
         return f"Dataset( trainml , **{self._dataset.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
     async def get_log_url(self):
         resp = await self.trainml._query(
-            f"/dataset/pub/{self._id}/logs",
+            f"/dataset/{self._id}/logs",
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         return resp
 
     async def get_details(self):
         resp = await self.trainml._query(
-            f"/dataset/pub/{self._id}/details",
+            f"/dataset/{self._id}/details",
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         return resp
 
     async def get_connection_utility_url(self):
         resp = await self.trainml._query(
-            f"/dataset/pub/{self._id}/download",
+            f"/dataset/{self._id}/download",
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         return resp
 
     def get_connection_details(self):
         if self._dataset.get("vpn"):
@@ -146,15 +144,15 @@
             self.trainml, entity_type="dataset", id=self.id, entity=self
         )
         await connection.stop()
         return connection.status
 
     async def remove(self, force=False):
         await self.trainml._query(
-            f"/dataset/pub/{self._id}",
+            f"/dataset/{self._id}",
             "DELETE",
             dict(project_uuid=self._project_uuid, force=force),
         )
 
     def _get_msg_handler(self, msg_handler):
         def handler(data):
             if data.get("type") == "subscription":
@@ -178,15 +176,15 @@
                 self._project_uuid,
                 self.id,
                 self._get_msg_handler(msg_handler),
             )
 
     async def refresh(self):
         resp = await self.trainml._query(
-            f"/dataset/pub/{self.id}",
+            f"/dataset/{self.id}",
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         self.__init__(self.trainml, **resp)
         return self
 
     async def wait_for(self, status, timeout=300):
```

### Comparing `trainml-0.4.8/trainml/environments.py` & `trainml-0.4.9/trainml/environments.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/exceptions.py` & `trainml-0.4.9/trainml/exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/gpu_types.py` & `trainml-0.4.9/trainml/gpu_types.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/jobs.py` & `trainml-0.4.9/trainml/jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,48 +11,14 @@
     JobError,
     SpecificationError,
     TrainMLException,
 )
 from trainml.connections import Connection
 
 
-def _clean_datasets_selection(
-    requested_datasets=[],
-):
-    datasets = []
-    for dataset in requested_datasets:
-        if dataset.get("type") not in ["existing", "public"]:
-            raise SpecificationError(
-                "datasets",
-                "Invalid dataset specification, 'type' must be in ['existing','public']",
-            )
-        if "id" in dataset.keys():
-            datasets.append(
-                dict(
-                    id=dataset.get("id"),
-                    type=dataset.get("type"),
-                )
-            )
-        elif "dataset_uuid" in dataset.keys():
-            datasets.append(dataset)
-        elif "name" in dataset.keys():
-            datasets.append(
-                dict(
-                    id=dataset.get("name"),
-                    type=dataset.get("type"),
-                )
-            )
-        else:
-            raise SpecificationError(
-                "datasets",
-                "Invalid dataset specification, either 'id' or 'name' must be provided",
-            )
-    return datasets
-
-
 class Jobs(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
     async def get(self, id):
         resp = await self.trainml._query(f"/job/{id}", "GET")
         return Job(self.trainml, **resp)
@@ -69,25 +35,21 @@
         gpu_type=None,
         gpu_types=[],
         gpu_count=None,
         cpu_count=None,
         disk_size=10,
         max_price=10,
         worker_commands=[],
-        environment=dict(type="DEEPLEARNING_PY39"),
+        environment=dict(),
         data=dict(),
         model=dict(),
         endpoint=dict(),
         **kwargs,
     ):
 
-        if data and data.get("datasets"):
-            datasets = _clean_datasets_selection(data.get("datasets"))
-            data["datasets"] = datasets
-
         resources = {
             k: v
             for k, v in dict(
                 gpu_count=gpu_count,
                 disk_size=disk_size,
                 max_price=max_price,
                 cpu_count=cpu_count,
@@ -217,16 +179,22 @@
         ]
         resources_keys = [
             "gpu_count",
             "gpu_types",
             "disk_size",
             "max_price",
             "preemptible",
+            "cpu_count",
+        ]
+        model_keys = [
+            "source_type",
+            "source_uri",
+            "project_uuid",
+            "checkpoints",
         ]
-        model_keys = ["source_type", "source_uri", "project_uuid"]
         data_keys = [
             "datasets",
             "input_type",
             "input_uri",
             "input_options",
             "output_type",
             "output_uri",
@@ -235,15 +203,15 @@
         environment_keys = [
             "type",
             "env",
             "custom_image",
             "worker_key_types",
             "packages",
         ]
-        endpoint_keys = ["routes", "start_command"]
+        endpoint_keys = ["routes", "start_command", "reservation_id"]
         create_json = dict()
         for k, v in self.dict.items():
             if k in root_keys:
                 if k == "resources":
                     resources = dict()
                     for k2, v2 in v.items():
                         if k2 in resources_keys:
@@ -294,14 +262,27 @@
         await self.trainml._query(
             f"/job/{self._id}",
             "PATCH",
             dict(project_uuid=self._project_uuid),
             dict(command="stop"),
         )
 
+    async def update(self, data):
+        if self.type != "notebook":
+            raise SpecificationError(
+                "type",
+                "Only notebook jobs can be modified.",
+            )
+        await self.trainml._query(
+            f"/job/{self._id}",
+            "PATCH",
+            dict(project_uuid=self._project_uuid),
+            data,
+        )
+
     async def get_worker_log_url(self, job_worker_uuid):
         resp = await self.trainml._query(
             f"/job/{self._id}/worker/{job_worker_uuid}/logs",
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         return resp
@@ -462,14 +443,15 @@
             or self._job.get("resources").get("disk_size"),
             max_price=kwargs.get("max_price")
             or self._job.get("resources").get("max_price"),
             worker_commands=kwargs.get("worker_commands"),
             workers=kwargs.get("workers"),
             environment=kwargs.get("environment"),
             data=kwargs.get("data"),
+            model=kwargs.get("model"),
             source_job_uuid=self.id,
         )
         logging.debug(f"copy result: {job}")
         return job
 
     async def wait_for(self, status, timeout=300):
         valid_statuses = [
```

### Comparing `trainml-0.4.8/trainml/models.py` & `trainml-0.4.9/trainml/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,43 +14,41 @@
 
 
 class Models(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
     async def get(self, id):
-        resp = await self.trainml._query(f"/model/pub/{id}", "GET")
+        resp = await self.trainml._query(f"/model/{id}", "GET")
         return Model(self.trainml, **resp)
 
     async def list(self):
-        resp = await self.trainml._query(f"/model/pub", "GET")
+        resp = await self.trainml._query(f"/model", "GET")
         models = [Model(self.trainml, **model) for model in resp]
         return models
 
     async def create(self, name, source_type, source_uri, **kwargs):
         data = dict(
             name=name,
             source_type=source_type,
             source_uri=source_uri,
             source_options=kwargs.get("source_options"),
             project_uuid=kwargs.get("project_uuid")
             or self.trainml.active_project,
         )
         payload = {k: v for k, v in data.items() if v}
         logging.info(f"Creating Model {name}")
-        resp = await self.trainml._query("/model/pub", "POST", None, payload)
+        resp = await self.trainml._query("/model", "POST", None, payload)
         model = Model(self.trainml, **resp)
         logging.info(f"Created Model {name} with id {model.id}")
 
         return model
 
     async def remove(self, id):
-        await self.trainml._query(
-            f"/model/pub/{id}", "DELETE", dict(force=True)
-        )
+        await self.trainml._query(f"/model/{id}", "DELETE", dict(force=True))
 
 
 class Model:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
         self._model = kwargs
         self._id = self._model.get("id", self._model.get("model_uuid"))
@@ -82,31 +80,31 @@
         return f"Model( trainml , **{self._model.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
     async def get_log_url(self):
         resp = await self.trainml._query(
-            f"/model/pub/{self._id}/logs",
+            f"/model/{self._id}/logs",
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         return resp
 
     async def get_details(self):
         resp = await self.trainml._query(
-            f"/model/pub/{self._id}/details",
+            f"/model/{self._id}/details",
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         return resp
 
     async def get_connection_utility_url(self):
         resp = await self.trainml._query(
-            f"/model/pub/{self._id}/download",
+            f"/model/{self._id}/download",
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         return resp
 
     def get_connection_details(self):
         if self._model.get("vpn"):
@@ -139,15 +137,15 @@
             self.trainml, entity_type="model", id=self.id, entity=self
         )
         await connection.stop()
         return connection.status
 
     async def remove(self, force=False):
         await self.trainml._query(
-            f"/model/pub/{self._id}",
+            f"/model/{self._id}",
             "DELETE",
             dict(project_uuid=self._project_uuid, force=force),
         )
 
     def _get_msg_handler(self, msg_handler):
         def handler(data):
             if data.get("type") == "subscription":
@@ -171,15 +169,15 @@
                 self._project_uuid,
                 self.id,
                 self._get_msg_handler(msg_handler),
             )
 
     async def refresh(self):
         resp = await self.trainml._query(
-            f"/model/pub/{self.id}",
+            f"/model/{self.id}",
             "GET",
             dict(project_uuid=self._project_uuid),
         )
         self.__init__(self.trainml, **resp)
         return self
 
     async def wait_for(self, status, timeout=300):
```

### Comparing `trainml-0.4.8/trainml/projects.py` & `trainml-0.4.9/trainml/projects.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/providers.py` & `trainml-0.4.9/trainml/providers.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml/trainml.py` & `trainml-0.4.9/trainml/trainml.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.8/trainml.egg-info/PKG-INFO` & `trainml-0.4.9/trainml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.4.8
+Version: 0.4.9
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.4.8 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.4.9 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           [https://www.trainml.ai/static/img/trainML-logo-purple.png]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.4.8/trainml.egg-info/SOURCES.txt` & `trainml-0.4.9/trainml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,9 +57,10 @@
 trainml/cli/checkpoint.py
 trainml/cli/connection.py
 trainml/cli/dataset.py
 trainml/cli/environment.py
 trainml/cli/gpu.py
 trainml/cli/model.py
 trainml/cli/project.py
+trainml/cli/provider.py
 trainml/cli/job/__init__.py
 trainml/cli/job/create.py
```

