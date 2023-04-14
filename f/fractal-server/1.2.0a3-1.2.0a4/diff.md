# Comparing `tmp/fractal_server-1.2.0a3.tar.gz` & `tmp/fractal_server-1.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.2.0a3.tar", max compression
+gzip compressed data, was "fractal_server-1.2.0a4.tar", max compression
```

## Comparing `fractal_server-1.2.0a3.tar` & `fractal_server-1.2.0a4.tar`

### file list

```diff
@@ -1,116 +1,117 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.0a3/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.0a3/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.0a3/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-04-11 12:16:47.461555 fractal_server-1.2.0a3/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-02-22 13:06:13.003243 fractal_server-1.2.0a3/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.0a3/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.0a3/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.0a3/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.0a3/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     2740 2023-02-22 13:06:13.003243 fractal_server-1.2.0a3/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0    21405 2023-04-11 12:05:25.621706 fractal_server-1.2.0a3/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    11632 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    11398 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     2731 2023-03-16 15:50:18.447564 fractal_server-1.2.0a3/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.0a3/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.0a3/fractal_server/app/models/job.py
--rw-r--r--   0        0        0     2341 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     1094 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5371 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     7955 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    20869 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     4510 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3690 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8802 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     3281 2023-04-11 12:05:21.017629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    18306 2023-04-11 12:16:36.785569 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4327 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    39831 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     9748 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0     7379 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.0a3/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.0a3/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.0a3/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.0a3/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.0a3/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.0a3/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.0a3/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.0a3/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.0a3/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.0a3/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.0a3/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.0a3/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.0a3/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.0a3/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.0a3/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.0a3/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.0a3/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.0a3/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    13216 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/config.py
--rw-r--r--   0        0        0     4873 2023-02-22 13:06:13.007243 fractal_server-1.2.0a3/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.0a3/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.0a3/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.0a3/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      770 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
--rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.0a3/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
--rw-r--r--   0        0        0      706 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.0a3/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    12796 2023-04-11 12:05:21.021629 fractal_server-1.2.0a3/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     3878 2023-03-15 10:25:37.387800 fractal_server-1.2.0a3/fractal_server/utils.py
--rw-r--r--   0        0        0     2629 2023-04-11 12:16:47.461555 fractal_server-1.2.0a3/pyproject.toml
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.0a3/setup.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.2.0a4/LICENSE
+-rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.2.0a4/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.2.0a4/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-04-14 12:56:29.081164 fractal_server-1.2.0a4/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-02-22 13:06:13.003243 fractal_server-1.2.0a4/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.2.0a4/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.2.0a4/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      887 2023-02-22 13:06:13.003243 fractal_server-1.2.0a4/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.2.0a4/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     2740 2023-02-22 13:06:13.003243 fractal_server-1.2.0a4/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0    21983 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    11794 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    11398 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     2724 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.2.0a4/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3242 2023-03-06 15:02:42.909169 fractal_server-1.2.0a4/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0     2341 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     1094 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1079 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1080 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5371 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     8144 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    20882 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     4510 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3690 2023-04-13 13:38:10.605758 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     3281 2023-04-14 08:28:41.981553 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    18410 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-04-14 12:55:14.842206 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    40101 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     9749 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0     7379 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.2.0a4/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.2.0a4/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       48 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      525 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      388 2023-02-22 12:30:35.511172 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-04-06 07:55:08.841694 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     2049 2023-03-06 13:52:52.493340 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     3541 2023-02-22 12:30:35.515172 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3612 2023-04-06 08:32:42.225519 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1205 2023-03-06 14:09:53.716138 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     5012 2023-03-06 13:52:52.501340 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     1154 2023-04-06 07:55:08.869693 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     4075 2023-03-24 07:30:26.992987 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-04-06 07:41:00.992984 fractal_server-1.2.0a4/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1716 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     2817 2023-02-22 11:04:15.289972 fractal_server-1.2.0a4/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2527 2023-04-06 08:31:17.294479 fractal_server-1.2.0a4/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      695 2023-03-06 14:09:35.208454 fractal_server-1.2.0a4/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     4484 2023-03-06 13:52:25.445648 fractal_server-1.2.0a4/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0      998 2023-04-06 07:41:00.992984 fractal_server-1.2.0a4/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2709 2023-03-24 07:30:25.077014 fractal_server-1.2.0a4/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      139 2023-03-06 16:04:10.500759 fractal_server-1.2.0a4/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0     1065 2023-03-06 16:04:10.500759 fractal_server-1.2.0a4/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-03-15 08:25:43.077415 fractal_server-1.2.0a4/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0      541 2023-03-06 16:04:10.500759 fractal_server-1.2.0a4/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-04-06 08:31:17.294479 fractal_server-1.2.0a4/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-03-06 16:04:10.500759 fractal_server-1.2.0a4/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0      748 2023-03-06 16:04:10.500759 fractal_server-1.2.0a4/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0     1224 2023-04-06 07:41:00.992984 fractal_server-1.2.0a4/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2838 2023-03-24 07:30:25.077014 fractal_server-1.2.0a4/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    13225 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/logger.py
+-rw-r--r--   0        0        0     4969 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.2.0a4/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.2.0a4/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.2.0a4/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      770 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py
+-rw-r--r--   0        0        0     8557 2023-03-16 07:52:46.509457 fractal_server-1.2.0a4/fractal_server/migrations/versions/47072e0106ce_initial_schema.py
+-rw-r--r--   0        0        0      706 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.2.0a4/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.2.0a4/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    12782 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-04-14 12:55:14.846206 fractal_server-1.2.0a4/fractal_server/utils.py
+-rw-r--r--   0        0        0     2629 2023-04-14 12:56:29.081164 fractal_server-1.2.0a4/pyproject.toml
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 fractal_server-1.2.0a4/setup.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 fractal_server-1.2.0a4/PKG-INFO
```

### Comparing `fractal_server-1.2.0a3/LICENSE` & `fractal_server-1.2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/README.md` & `fractal_server-1.2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/__main__.py` & `fractal_server-1.2.0a4/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/alembic.ini` & `fractal_server-1.2.0a4/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/api/__init__.py` & `fractal_server-1.2.0a4/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/api/v1/job.py` & `fractal_server-1.2.0a4/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/api/v1/project.py` & `fractal_server-1.2.0a4/fractal_server/app/api/v1/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import asyncio
-import logging
 from typing import Optional
 from typing import Union
 
 from fastapi import APIRouter
 from fastapi import BackgroundTasks
 from fastapi import Depends
 from fastapi import HTTPException
 from fastapi import Response
 from fastapi import status
 from pydantic import UUID4
 from sqlalchemy.exc import IntegrityError
 from sqlmodel import select
 
 from ....config import get_settings
+from ....logger import close_logger
+from ....logger import set_logger
 from ....syringe import Inject
 from ...db import AsyncSession
 from ...db import DBSyncSession
 from ...db import get_db
 from ...db import get_sync_db
 from ...models import ApplyWorkflow
 from ...models import ApplyWorkflowCreate
@@ -174,15 +175,17 @@
     db_project.user_member_list.append(user)
     try:
         db.add(db_project)
         await db.commit()
         await db.refresh(db_project)
     except IntegrityError as e:
         await db.rollback()
-        logging.error(str(e))
+        logger = set_logger("create_project")
+        logger.error(str(e))
+        close_logger(logger)
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=str(e),
         )
 
     return db_project
 
@@ -656,29 +659,37 @@
     # combine them into source -- see issue #293.
     tasks = [wf_task.task for wf_task in workflow.task_list]
     sourcename_to_id = {}
     for task in tasks:
         source = task.source
         name = task.name
         if not (source, name) in sourcename_to_id.keys():
-            stm = (
-                select(Task)
-                .where(Task.name == name)
-                .where(Task.source == source)
-            )
-            res = await db.execute(stm)
-            current_task = res.scalars().all()
-            if not len(current_task) == 1:
+            stm = select(Task).where(Task.source == source)
+            tasks_by_source = (await db.execute(stm)).scalars().all()
+            if not tasks_by_source:
                 raise HTTPException(
                     status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-                    detail=(
-                        f"Found {len(current_task)} tasks with {source=}."
-                    ),
+                    detail=(f"Found 0 tasks with {source=}."),
+                )
+            else:
+                stm = (
+                    select(Task)
+                    .where(Task.source == source)
+                    .where(Task.name == name)
                 )
-            sourcename_to_id[(source, name)] = current_task[0].id
+                current_task = (await db.execute(stm)).scalars().all()
+                if len(current_task) != 1:
+                    raise HTTPException(
+                        status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                        detail=(
+                            f"Found {len(current_task)} tasks with "
+                            f"{name =} and {source=}."
+                        ),
+                    )
+                sourcename_to_id[(source, name)] = current_task[0].id
 
     # Create new Workflow
     workflow_create = WorkflowCreate(
         project_id=project_id, **workflow.dict(exclude_none=True)
     )
     db_workflow = Workflow.from_orm(workflow_create)
     db.add(db_workflow)
```

### Comparing `fractal_server-1.2.0a3/fractal_server/app/api/v1/task.py` & `fractal_server-1.2.0a4/fractal_server/app/api/v1/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 import json
-import logging
 from copy import deepcopy  # noqa
 from pathlib import Path
 from shutil import copy as shell_copy
 from shutil import rmtree as shell_rmtree
 from tempfile import TemporaryDirectory
 from typing import Optional
 
@@ -19,26 +18,26 @@
 from ....common.schemas import StateRead
 from ....common.schemas import TaskCollectPip
 from ....common.schemas import TaskCollectStatus
 from ....common.schemas import TaskCreate
 from ....common.schemas import TaskRead
 from ....common.schemas import TaskUpdate
 from ....config import get_settings
+from ....logger import close_logger
+from ....logger import set_logger
 from ....syringe import Inject
 from ....tasks.collection import _TaskCollectPip
 from ....tasks.collection import create_package_dir_pip
 from ....tasks.collection import create_package_environment_pip
 from ....tasks.collection import download_package
 from ....tasks.collection import get_collection_data
 from ....tasks.collection import get_collection_log
 from ....tasks.collection import get_collection_path
 from ....tasks.collection import get_log_path
 from ....tasks.collection import inspect_package
-from ....utils import close_logger
-from ....utils import set_logger
 from ...db import AsyncSession
 from ...db import DBSyncSession
 from ...db import get_db
 from ...db import get_sync_db
 from ...models import State
 from ...models import Task
 from ...security import current_active_superuser
@@ -60,66 +59,65 @@
     In case of error, copy the log into the state and delete the package
     directory.
     """
     logger_name = task_pkg.package.replace("/", "_")
     logger = set_logger(
         logger_name=logger_name,
         log_file_path=get_log_path(venv_path),
-        level=logging.DEBUG,
     )
 
-    logger = set_logger(logger_name=logger_name)
-    logger.info("Start background task collection")
+    logger.debug("Start background task collection")
     data = TaskCollectStatus(**state.data)
     data.info = None
 
     try:
         # install
-        logger.info("Status: installing")
+        logger.debug("Task-collection status: installing")
         data.status = "installing"
 
         state.data = data.sanitised_dict()
         await db.merge(state)
         await db.commit()
         task_list = await create_package_environment_pip(
             venv_path=venv_path,
             task_pkg=task_pkg,
             logger_name=logger_name,
         )
 
         # collect
-        logger.info("Status: collecting")
+        logger.debug("Task-collection status: collecting")
         data.status = "collecting"
         state.data = data.sanitised_dict()
         await db.merge(state)
         await db.commit()
         tasks = await _insert_tasks(task_list=task_list, db=db)
 
         # finalise
-        logger.info("Status: finalising")
+        logger.debug("Task-collection status: finalising")
         collection_path = get_collection_path(venv_path)
         data.task_list = tasks
         with collection_path.open("w") as f:
             json.dump(data.sanitised_dict(), f)
 
         # Update DB
         data.status = "OK"
+        data.log = get_collection_log(venv_path)
         state.data = data.sanitised_dict()
         db.add(state)
         await db.merge(state)
         await db.commit()
 
         # Write last logs to file
-        logger.info("Status: OK")
+        logger.debug("Task-collection status: OK")
         logger.info("Background task collection completed successfully")
         close_logger(logger)
 
     except Exception as e:
         # Write last logs to file
-        logger.info("Status: fail")
+        logger.debug("Task-collection status: fail")
         logger.info(f"Background collection failed. Original error: {e}")
         close_logger(logger)
 
         # Update db
         data.status = "fail"
         data.info = f"Original error: {e}"
         data.log = get_collection_log(venv_path)
@@ -173,15 +171,15 @@
     """
     Task collection endpoint
 
     Trigger the creation of a dedicated virtual environment, the installation
     of a package and the collection of tasks as advertised in the manifest.
     """
 
-    logger = set_logger(logger_name="fractal")
+    logger = set_logger(logger_name="collect_tasks_pip")
     task_pkg = _TaskCollectPip(**task_collect.dict())
 
     with TemporaryDirectory() as tmpdir:
         try:
             if task_pkg.is_local_package:
                 shell_copy(task_pkg.package_path.as_posix(), tmpdir)
                 pkg_path = Path(tmpdir) / task_pkg.package_path.name
@@ -233,27 +231,29 @@
     collection_status_dict["venv_path"] = str(collection_status.venv_path)
 
     state = State(data=collection_status_dict)
     db.add(state)
     await db.commit()
     await db.refresh(state)
 
-    logger.info("starting background collection")
     background_tasks.add_task(
         _background_collect_pip,
         state=state,
         venv_path=venv_path,
         task_pkg=task_pkg,
         db=db,
     )
-
-    logger.info("collection endpoint: returning state")
+    logger.debug(
+        "Task-collection endpoint: start background collection "
+        "and return state"
+    )
+    close_logger(logger)
     info = (
         "Collecting tasks in the background. "
-        "GET /task/collect/{id} to query collection status"
+        f"GET /task/collect/{state.id} to query collection status"
     )
     state.data["info"] = info
     response.status_code = status.HTTP_201_CREATED
     return state
 
 
 @router.get("/collect/{state_id}", response_model=StateRead)
@@ -262,29 +262,30 @@
     user: User = Depends(current_active_user),
     verbose: bool = False,
     db: AsyncSession = Depends(get_db),
 ) -> StateRead:  # State[TaskCollectStatus]
     """
     Check status of background task collection
     """
-    logger = set_logger(logger_name="fractal")
-    logger.info("querying state")
+    logger = set_logger(logger_name="check_collection_status")
+    logger.debug(f"Querying state for state.id={state_id}")
     state = await db.get(State, state_id)
     if not state:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=f"No task collection info with id={state_id}",
         )
     data = TaskCollectStatus(**state.data)
 
     # In some cases (i.e. a successful or ongoing task collection), data.log is
     # not set; if so, we collect the current logs
     if verbose and not data.log:
         data.log = get_collection_log(data.venv_path)
         state.data = data.sanitised_dict()
+    close_logger(logger)
     return state
 
 
 @router.get("/", response_model=list[TaskRead])
 async def get_list_task(
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_db),
```

### Comparing `fractal_server-1.2.0a3/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.2.0a4/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/db/__init__.py` & `fractal_server-1.2.0a4/fractal_server/app/db/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 `db` module, loosely adapted from
 https://testdriven.io/blog/fastapi-sqlmodel/#async-sqlmodel
 """
 from typing import AsyncGenerator
 from typing import Generator
-from warnings import warn
 
 from sqlalchemy import create_engine
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.ext.asyncio import create_async_engine
 from sqlalchemy.orm import Session as DBSyncSession
 from sqlalchemy.orm import sessionmaker
 
 from ...config import get_settings
+from ...logger import set_logger
 from ...syringe import Inject
 
 
+print(__name__)
+logger = set_logger(__name__)
+
+
 class DB:
     """
     DB class
     """
 
     @classmethod
     def engine_async(cls):
@@ -38,20 +42,18 @@
             return cls._engine_sync
 
     @classmethod
     def set_db(cls):
         settings = Inject(get_settings)
 
         if settings.DB_ENGINE == "sqlite":
-            warn(
-                "SQLite is partially supported but discouraged "
-                "in production environment."
-                "SQLite offers partial support for ForeignKey "
-                "constraints. As such, consistency of the database "
-                "cannot be guaranteed."
+            logger.warning(
+                "SQLite is supported but discouraged in production. Given its "
+                "partial support for ForeignKey constraints, consistency of "
+                "the database cannot be guaranteed."
             )
 
         cls._engine_async = create_async_engine(
             settings.DATABASE_URL, echo=settings.DB_ECHO, future=True
         )
         cls._engine_sync = create_engine(
             settings.DATABASE_SYNC_URL,
```

### Comparing `fractal_server-1.2.0a3/fractal_server/app/models/job.py` & `fractal_server-1.2.0a4/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/models/project.py` & `fractal_server-1.2.0a4/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/models/security.py` & `fractal_server-1.2.0a4/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/models/state.py` & `fractal_server-1.2.0a4/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/models/task.py` & `fractal_server-1.2.0a4/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/models/workflow.py` & `fractal_server-1.2.0a4/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/__init__.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,23 @@
 """
 Runner backend subsystem root
 
 This module is the single entry point to the runner backend subsystem. Other
 subystems should only import this module and not its submodules or the
 individual backends.
 """
-import logging
 import os
 from pathlib import Path
 from typing import Optional
 
 from ... import __VERSION__
 from ...config import get_settings
+from ...logger import set_logger
 from ...syringe import Inject
 from ...utils import get_timestamp
-from ...utils import set_logger
 from ..db import DB
 from ..models import ApplyWorkflow
 from ..models import Dataset
 from ..models import JobStatusType
 from ..models import Workflow
 from ._local import process_workflow as local_process_workflow
 from .common import auto_output_dataset  # noqa: F401
@@ -154,82 +153,85 @@
     job.working_dir_user = WORKFLOW_DIR_USER.as_posix()
     job.status = JobStatusType.RUNNING
     db_sync.merge(job)
     db_sync.commit()
 
     # Write logs
     logger_name = f"WF{workflow_id}_job{job_id}"
+    log_file_path = WORKFLOW_DIR / "workflow.log"
     logger = set_logger(
         logger_name=logger_name,
-        log_file_path=WORKFLOW_DIR / "workflow.log",
-        level=logging.INFO,
-        formatter=logging.Formatter("%(asctime)s; %(levelname)s; %(message)s"),
+        log_file_path=log_file_path,
     )
-    logger.info(f"fractal_server.__VERSION__: {__VERSION__}")
-    logger.info(f"FRACTAL_RUNNER_BACKEND: {FRACTAL_RUNNER_BACKEND}")
-    logger.info(f"slurm_user: {slurm_user}")
-    logger.info(f"worker_init: {worker_init}")
-    logger.info(f"input metadata: {input_dataset.meta}")
-    logger.info(f"input_paths: {input_paths}")
-    logger.info(f"output_path: {output_path}")
-    logger.info(f"job.id: {job.id}")
-    logger.info(f"job.working_dir: {str(WORKFLOW_DIR)}")
-    logger.info(f"job.workflow_dir_user: {str(WORKFLOW_DIR_USER)}")
-    logger.info(f'START workflow "{workflow.name}"')
+    logger.info(
+        f'Start execution of workflow "{workflow.name}"; '
+        f"more logs at {str(log_file_path)}"
+    )
+    logger.debug(f"fractal_server.__VERSION__: {__VERSION__}")
+    logger.debug(f"FRACTAL_RUNNER_BACKEND: {FRACTAL_RUNNER_BACKEND}")
+    logger.debug(f"slurm_user: {slurm_user}")
+    logger.debug(f"worker_init: {worker_init}")
+    logger.debug(f"input metadata: {input_dataset.meta}")
+    logger.debug(f"input_paths: {input_paths}")
+    logger.debug(f"output_path: {output_path}")
+    logger.debug(f"job.id: {job.id}")
+    logger.debug(f"job.working_dir: {str(WORKFLOW_DIR)}")
+    logger.debug(f"job.workflow_dir_user: {str(WORKFLOW_DIR_USER)}")
+    logger.debug(f'START workflow "{workflow.name}"')
 
     try:
         output_dataset.meta = await process_workflow(
             workflow=workflow,
             input_paths=input_paths,
             output_path=output_path,
             input_metadata=input_dataset.meta,
             slurm_user=slurm_user,
             workflow_dir=WORKFLOW_DIR,
             workflow_dir_user=WORKFLOW_DIR_USER,
             logger_name=logger_name,
             worker_init=worker_init,
         )
 
-        logger.info(f'END workflow "{workflow.name}"')
-        close_job_logger(logger)
+        logger.debug(f'END workflow "{workflow.name}"')
 
         db_sync.merge(output_dataset)
         job.status = JobStatusType.DONE
         db_sync.merge(job)
 
     except TaskExecutionError as e:
 
-        logger.info(f'FAILED workflow "{workflow.name}", TaskExecutionError.')
-        close_job_logger(logger)
+        logger.debug(f'FAILED workflow "{workflow.name}", TaskExecutionError.')
+        logger.info(f'Workflow "{workflow.name}" failed (TaskExecutionError).')
 
         job.status = JobStatusType.FAILED
 
         exception_args_string = "\n".join(e.args)
         job.log = (
             f"TASK ERROR:"
             f"Task id: {e.workflow_task_id} ({e.task_name}), "
             f"{e.workflow_task_order=}\n"
             f"TRACEBACK:\n{exception_args_string}"
         )
         db_sync.merge(job)
 
     except JobExecutionError as e:
 
-        logger.info(f'FAILED workflow "{workflow.name}", JobExecutionError.')
-        close_job_logger(logger)
+        logger.debug(f'FAILED workflow "{workflow.name}", JobExecutionError.')
+        logger.info(f'Workflow "{workflow.name}" failed (JobExecutionError).')
 
         job.status = JobStatusType.FAILED
         error = e.assemble_error()
         job.log = f"JOB ERROR:\nTRACEBACK:\n{error}"
         db_sync.merge(job)
 
     except Exception as e:
 
-        logger.info(f'FAILED workflow "{workflow.name}", unknown error.')
-        close_job_logger(logger)
+        logger.debug(f'FAILED workflow "{workflow.name}", unknown error.')
+        logger.info(f'Workflow "{workflow.name}" failed (unkwnon error).')
 
         job.status = JobStatusType.FAILED
         job.log = f"UNKNOWN ERROR\nOriginal error: {str(e)}"
         db_sync.merge(job)
 
     finally:
+        close_job_logger(logger)
         db_sync.commit()
```

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/_common.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 Common utilities and routines for runner backends (private API)
 
 This module includes utilities and routines that are of use to implement
 runner backends and that should not be exposed outside of the runner
 subsystem.
 """
 import json
-import logging
 import subprocess  # nosec
 from concurrent.futures import Executor
 from concurrent.futures import Future
 from functools import lru_cache
 from functools import partial
 from pathlib import Path
 from shlex import split as shlex_split
 from typing import Callable
 from typing import Generator
 from typing import Optional
 
 from ...config import get_settings
+from ...logger import get_logger
 from ...syringe import Inject
 from ..models import WorkflowTask
 from .common import JobExecutionError
 from .common import TaskExecutionError
 from .common import TaskParameters
 from .common import write_args_file
 
@@ -557,15 +557,15 @@
         *dependencies, this_wftask = task_list
     except ValueError:
         # step 0: return future containing original task_pars
         pseudo_future: Future = Future()
         pseudo_future.set_result(task_pars)
         return pseudo_future
 
-    logger = logging.getLogger(logger_name)
+    logger = get_logger(logger_name)
 
     # step n => step n+1
     task_pars_depend_future = recursive_task_submission(
         executor=executor,
         task_list=dependencies,
         task_pars=task_pars,
         workflow_dir=workflow_dir,
@@ -574,15 +574,15 @@
         logger_name=logger_name,
     )
     # Wait for dependencies to be complete (NOTE: this is not necessary if we
     # explicitly wait for the result of executor.submit(call_single_task, ...),
     # see below
     task_pars_depend = task_pars_depend_future.result()
 
-    logger.info(
+    logger.debug(
         f'SUBMIT {this_wftask.order}-th task (name="{this_wftask.task.name}")'
     )
     if this_wftask.is_parallel:
         # NOTE: call_parallel_task is blocking, i.e. the returned future always
         # has `this_wftask_future.done() = True`
         this_wftask_future = call_parallel_task(
             executor=executor,
@@ -607,15 +607,15 @@
             task_pars=task_pars_depend,
             workflow_dir=workflow_dir,
             workflow_dir_user=workflow_dir_user,
             **extra_setup,
         )
         # Wait for the future result (blocking)
         this_wftask_future.result()
-    logger.info(
+    logger.debug(
         f'END    {this_wftask.order}-th task (name="{this_wftask.task.name}")'
     )
 
     # Write most recent metadata to METADATA_FILENAME
     with open(workflow_dir / METADATA_FILENAME, "w") as f:
         json.dump(this_wftask_future.result().metadata, f, indent=2)
```

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_batching.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
 """
 Submodule to determine the number of total/parallel tasks per SLURM job.
 """
-import logging
 import math
 from typing import Optional
 
+from ....logger import set_logger
+
+logger = set_logger(__name__)
+
 
 class SlurmHeuristicsError(ValueError):
     pass
 
 
 def _estimate_parallel_tasks_per_job(
     *,
@@ -121,114 +124,114 @@
     """
     # Preliminary checks
     if bool(tasks_per_job) != bool(parallel_tasks_per_job):
         msg = (
             "tasks_per_job and parallel_tasks_per_job must "
             "be both set or both unset"
         )
-        logging.error(msg)
+        logger.error(msg)
         raise SlurmHeuristicsError(msg)
     if cpus_per_task > max_cpus_per_job:
         msg = (
             f"[heuristics] Requested {cpus_per_task=} "
             f"but {max_cpus_per_job=}."
         )
-        logging.error(msg)
+        logger.error(msg)
         raise SlurmHeuristicsError(msg)
     if mem_per_task > max_mem_per_job:
         msg = (
             f"[heuristics] Requested {mem_per_task=} "
             f"but {max_mem_per_job=}."
         )
-        logging.error(msg)
+        logger.error(msg)
         raise SlurmHeuristicsError(msg)
 
     # Branch 1: validate/update given parameters
     if tasks_per_job and parallel_tasks_per_job:
         # Reduce parallel_tasks_per_job if it exceeds tasks_per_job
         if parallel_tasks_per_job > tasks_per_job:
-            logging.warning(
+            logger.warning(
                 "[heuristics] Set parallel_tasks_per_job="
                 f"tasks_per_job={tasks_per_job}"
             )
             parallel_tasks_per_job = tasks_per_job
 
         # Check requested cpus_per_job
         cpus_per_job = parallel_tasks_per_job * cpus_per_task
         if cpus_per_job > target_cpus_per_job:
-            logging.warning(
+            logger.warning(
                 f"[heuristics] Requested {cpus_per_job=} "
                 f"but {target_cpus_per_job=}."
             )
         if cpus_per_job > max_cpus_per_job:
             msg = (
                 f"[heuristics] Requested {cpus_per_job=} "
                 f"but {max_cpus_per_job=}."
             )
-            logging.error(msg)
+            logger.error(msg)
             raise SlurmHeuristicsError(msg)
 
         # Check requested mem_per_job
         mem_per_job = parallel_tasks_per_job * mem_per_task
         if mem_per_job > target_mem_per_job:
-            logging.warning(
+            logger.warning(
                 f"[heuristics] Requested {mem_per_job=} "
                 f"but {target_mem_per_job=}."
             )
         if mem_per_job > max_mem_per_job:
             msg = (
                 f"[heuristics] Requested {mem_per_job=} "
                 f"but {max_mem_per_job=}."
             )
-            logging.error(msg)
+            logger.error(msg)
             raise SlurmHeuristicsError(msg)
 
         # Check number of jobs
         num_jobs = math.ceil(tot_tasks / tasks_per_job)
         if num_jobs > target_num_jobs:
-            logging.info(
+            logger.debug(
                 f"[heuristics] Requested {num_jobs=} "
                 f"but {target_num_jobs=}."
             )
         if num_jobs > max_num_jobs:
             msg = f"[heuristics] Requested {num_jobs=} but {max_num_jobs=}."
-            logging.error(msg)
+            logger.error(msg)
             raise SlurmHeuristicsError(msg)
-        logging.debug("[heuristics] Return from branch 1")
+        logger.debug("[heuristics] Return from branch 1")
         return (tasks_per_job, parallel_tasks_per_job)
 
     # 2: Target-resources-based heuristics, without in-job queues
     parallel_tasks_per_job = _estimate_parallel_tasks_per_job(
         cpus_per_task=cpus_per_task,
         mem_per_task=mem_per_task,
         max_cpus_per_job=target_cpus_per_job,
         max_mem_per_job=target_mem_per_job,
     )
     tasks_per_job = parallel_tasks_per_job
     num_jobs = math.ceil(tot_tasks / tasks_per_job)
     if num_jobs <= target_num_jobs:
-        logging.debug("[heuristics] Return from branch 2")
+        logger.debug("[heuristics] Return from branch 2")
         return (tasks_per_job, parallel_tasks_per_job)
 
     # Branch 3: Max-resources-based heuristics, without in-job queues
     parallel_tasks_per_job = _estimate_parallel_tasks_per_job(
         cpus_per_task=cpus_per_task,
         mem_per_task=mem_per_task,
         max_cpus_per_job=max_cpus_per_job,
         max_mem_per_job=max_mem_per_job,
     )
     tasks_per_job = parallel_tasks_per_job
     num_jobs = math.ceil(tot_tasks / tasks_per_job)
     if num_jobs <= max_num_jobs:
-        logging.debug("[heuristics] Return from branch 3")
+        logger.debug("[heuristics] Return from branch 3")
         return (tasks_per_job, parallel_tasks_per_job)
 
     # Branch 4: Max-resources-based heuristics, with in-job queues
     parallel_tasks_per_job = _estimate_parallel_tasks_per_job(
         cpus_per_task=cpus_per_task,
         mem_per_task=mem_per_task,
         max_cpus_per_job=max_cpus_per_job,
         max_mem_per_job=max_mem_per_job,
     )
     tasks_per_job = math.ceil(tot_tasks / max_num_jobs)
-    logging.debug("[heuristics] Return from branch 4")
+    logger.debug("[heuristics] Return from branch 4")
     return (tasks_per_job, parallel_tasks_per_job)
```

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
 """
 Submodule to handle the SLURM configuration for a WorkflowTask
 """
 import json
-import logging
 from pathlib import Path
 from typing import Optional
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic import Extra
 from pydantic import Field
 from pydantic.error_wrappers import ValidationError
 
 from ....config import get_settings
+from ....logger import set_logger
+from ....logger import wrap_with_timing_logs
 from ....syringe import Inject
 from ...models import WorkflowTask
 
+logger = set_logger(__name__)
+
 
 class SlurmConfigError(ValueError):
     """
     Slurm configuration error
     """
 
     pass
@@ -142,27 +145,27 @@
     """
 
     if not config_path:
         settings = Inject(get_settings)
         config_path = settings.FRACTAL_SLURM_CONFIG_FILE
 
     # Load file
-    logging.debug(f"[get_slurm_config] Now loading {config_path=}")
+    logger.debug(f"[get_slurm_config] Now loading {config_path=}")
     try:
         with config_path.open("r") as f:
             slurm_env = json.load(f)
     except Exception as e:
         raise SlurmConfigError(
             f"Error while loading {config_path=}. "
             f"Original error:\n{str(e)}"
         )
 
     # Validate file content
-    logging.debug(f"[load_slurm_config_file] Now validating {config_path=}")
-    logging.debug(f"[load_slurm_config_file] {slurm_env=}")
+    logger.debug(f"[load_slurm_config_file] Now validating {config_path=}")
+    logger.debug(f"[load_slurm_config_file] {slurm_env=}")
     try:
         obj = SlurmConfigFile(**slurm_env)
     except ValidationError as e:
         raise SlurmConfigError(
             f"Error while loading {config_path=}. "
             f"Original error:\n{str(e)}"
         )
@@ -309,15 +312,15 @@
             f"{self.prefix} --mem={mem_per_job_MB}M",
         ]
         for key in ["job_name", "constraint", "gres", "time", "account"]:
             value = getattr(self, key)
             if value is not None:
                 # Handle the `time` parameter
                 if key == "time" and self.parallel_tasks_per_job > 1:
-                    logging.warning(
+                    logger.warning(
                         "Ignore `#SBATCH --time=...` line (given: "
                         f"{self.time=}) for parallel_tasks_per_job>1"
                         f" (given: {self.parallel_tasks_per_job}), "
                         "since scaling of time with number of tasks is "
                         "not implemented."
                     )
                     continue
@@ -368,41 +371,41 @@
 
     # Handle integer argument
     if isinstance(raw_mem, int):
         return raw_mem
 
     # Handle string argument
     if not raw_mem[0].isdigit():  # fail e.g. for raw_mem="M100"
-        logging.error(error_msg)
+        logger.error(error_msg)
         raise SlurmConfigError(error_msg)
     if raw_mem.isdigit():
         mem_MB = int(raw_mem)
     elif raw_mem.endswith("M"):
         stripped_raw_mem = raw_mem.strip("M")
         if not stripped_raw_mem.isdigit():
-            logging.error(error_msg)
+            logger.error(error_msg)
             raise SlurmConfigError(error_msg)
         mem_MB = int(stripped_raw_mem)
     elif raw_mem.endswith("G"):
         stripped_raw_mem = raw_mem.strip("G")
         if not stripped_raw_mem.isdigit():
-            logging.error(error_msg)
+            logger.error(error_msg)
             raise SlurmConfigError(error_msg)
         mem_MB = int(stripped_raw_mem) * 10**3
     elif raw_mem.endswith("T"):
         stripped_raw_mem = raw_mem.strip("T")
         if not stripped_raw_mem.isdigit():
-            logging.error(error_msg)
+            logger.error(error_msg)
             raise SlurmConfigError(error_msg)
         mem_MB = int(stripped_raw_mem) * 10**6
     else:
-        logging.error(error_msg)
+        logger.error(error_msg)
         raise SlurmConfigError(error_msg)
 
-    logging.debug(f"{info}, return {mem_MB}")
+    logger.debug(f"{info}, return {mem_MB}")
     return mem_MB
 
 
 def get_default_slurm_config():
     """
     Return a default `SlurmConfig` configuration object
     """
@@ -415,14 +418,15 @@
         target_mem_per_job=100,
         max_mem_per_job=500,
         target_num_jobs=2,
         max_num_jobs=4,
     )
 
 
+@wrap_with_timing_logs
 def get_slurm_config(
     wftask: WorkflowTask,
     workflow_dir: Path,
     workflow_dir_user: Path,
     config_path: Optional[Path] = None,
 ) -> SlurmConfig:
     """
@@ -452,15 +456,15 @@
             `FRACTAL_SLURM_CONFIG_FILE` variable from settings.
 
     Returns:
         slurm_config:
             The SlurmConfig object
     """
 
-    logging.debug(
+    logger.debug(
         "[get_slurm_config] WorkflowTask/Task meta attribute: "
         f"{wftask.overridden_meta=}"
     )
 
     # Incorporate slurm_env.default_slurm_config
     slurm_env = load_slurm_config_file(config_path=config_path)
     slurm_dict = slurm_env.default_slurm_config.dict(
@@ -468,27 +472,27 @@
     )
     if slurm_env.default_slurm_config.mem:
         slurm_dict["mem_per_task_MB"] = slurm_env.default_slurm_config.mem
 
     # Incorporate slurm_env.batching_config
     for key, value in slurm_env.batching_config.dict().items():
         slurm_dict[key] = value
-    logging.debug(
+    logger.debug(
         "[get_slurm_config] Fractal SLURM configuration file: "
         f"{slurm_env.dict()=}"
     )
 
     # GPU-related options
     # Notes about priority:
     # 1. This block of definitions takes priority over other definitions from
     #    slurm_env which are not under the `needs_gpu` subgroup
     # 2. This block of definitions has lower priority than whatever comes next
     #    (i.e. from WorkflowTask.overridden_meta).
     needs_gpu = wftask.overridden_meta.get("needs_gpu", False)
-    logging.debug(f"[get_slurm_config] {needs_gpu=}")
+    logger.debug(f"[get_slurm_config] {needs_gpu=}")
     if needs_gpu:
         for key, value in slurm_env.gpu_slurm_config.dict(
             exclude_unset=True, exclude={"mem"}
         ).items():
             slurm_dict[key] = value
         if slurm_env.gpu_slurm_config.mem:
             slurm_dict["mem_per_task_MB"] = slurm_env.gpu_slurm_config.mem
@@ -512,15 +516,15 @@
     for key in ["time", "account", "gres", "constraint"]:
         value = wftask.overridden_meta.get(key, None)
         if value:
             slurm_dict[key] = value
     extra_lines = wftask.overridden_meta.get("extra_lines", [])
     extra_lines = slurm_dict.get("extra_lines", []) + extra_lines
     if len(set(extra_lines)) != len(extra_lines):
-        logging.info(
+        logger.debug(
             "[get_slurm_config] Removing repeated elements "
             f"from {extra_lines=}."
         )
         extra_lines = list(set(extra_lines))
     slurm_dict["extra_lines"] = extra_lines
 
     # Job-batching parameters (if None, they will be determined heuristically)
@@ -529,14 +533,14 @@
         "parallel_tasks_per_job", None
     )
 
     slurm_dict["tasks_per_job"] = tasks_per_job
     slurm_dict["parallel_tasks_per_job"] = parallel_tasks_per_job
 
     # Put everything together
-    logging.debug(
+    logger.debug(
         "[get_slurm_config] Now create a SlurmConfig object based "
         f"on {slurm_dict=}"
     )
     slurm_config = SlurmConfig(**slurm_dict)
 
     return slurm_config
```

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,21 +11,26 @@
 """
 Run simple commands as another user
 
 This module provides a set of tools similar to `subprocess.run`, `glob.glob` or
 `os.path.exists`, but extended so that they can be executed on behalf of
 another user. Note that this requires appropriate sudo permissions.
 """
-import logging
 import shlex
 import subprocess  # nosec
 from typing import Optional
 from typing import Sequence
 
+from ....logger import set_logger
+from ....logger import wrap_with_timing_logs
 
+logger = set_logger(__name__)
+
+
+@wrap_with_timing_logs
 def _run_command_as_user(
     *,
     cmd: str,
     user: Optional[str] = None,
     encoding: Optional[str] = "utf-8",
     check: bool = False,
 ) -> subprocess.CompletedProcess:
@@ -41,39 +46,40 @@
 
     Raises:
         RuntimeError: if `check=True` and returncode is non-zero.
 
     Returns:
         res: The return value from `subprocess.run`.
     """
-    logging.debug(f'[_run_command_as_user] {user=}, cmd="{cmd}"')
+    logger.debug(f'[_run_command_as_user] {user=}, cmd="{cmd}"')
     if user:
         new_cmd = f"sudo --non-interactive -u {user} {cmd}"
     else:
         new_cmd = cmd
     res = subprocess.run(  # nosec
         shlex.split(new_cmd),
         capture_output=True,
         encoding=encoding,
     )
-    logging.debug(f"[_run_command_as_user] {res.returncode=}")
-    logging.debug(f"[_run_command_as_user] {res.stdout=}")
-    logging.debug(f"[_run_command_as_user] {res.stderr=}")
+    logger.debug(f"[_run_command_as_user] {res.returncode=}")
+    logger.debug(f"[_run_command_as_user] {res.stdout=}")
+    logger.debug(f"[_run_command_as_user] {res.stderr=}")
 
     if check and not res.returncode == 0:
         raise RuntimeError(
             f"{cmd=}\n\n"
             f"{res.returncode=}\n\n"
             f"{res.stdout=}\n\n"
             f"{res.stderr=}\n"
         )
 
     return res
 
 
+@wrap_with_timing_logs
 def _mkdir_as_user(*, folder: str, user: str) -> None:
     """
     Create a folder as a different user
 
     Arguments:
         folder: Absolute path to the folder
         user: User to be impersonated
@@ -85,14 +91,15 @@
     if not user:
         raise RuntimeError(f"{user=} not allowed in _mkdir_as_user")
 
     cmd = f"mkdir -p {folder}"
     _run_command_as_user(cmd=cmd, user=user, check=True)
 
 
+@wrap_with_timing_logs
 def _glob_as_user(
     *, folder: str, user: str, startswith: Optional[str] = None
 ) -> list[str]:
     """
     Run `ls` in a folder (as a user) and filter results
 
     Execute `ls` on a folder (impersonating a user, if `user` is not `None`)
@@ -107,14 +114,15 @@
     res = _run_command_as_user(cmd=f"ls {folder}", user=user, check=True)
     output = res.stdout.split()
     if startswith:
         output = [f for f in output if f.startswith(startswith)]
     return output
 
 
+@wrap_with_timing_logs
 def _path_exists_as_user(*, path: str, user: Optional[str] = None) -> bool:
     """
     Impersonate a user and check if `path` exists via `ls`
 
     Arguments:
         path: Absolute file/folder path
         user: If not `None`, user to be impersonated
@@ -122,14 +130,15 @@
     res = _run_command_as_user(cmd=f"ls {path}", user=user)
     if res.returncode == 0:
         return True
     else:
         return False
 
 
+@wrap_with_timing_logs
 def _multiple_paths_exist_as_user(
     *,
     paths: Sequence[str],
     user: Optional[str] = None,
 ) -> bool:
     """
     Impersonate a user and check if some paths exists via `ls`
```

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # Modified by:
 # Jacopo Nespolo <jacopo.nespolo@exact-lab.it>
 # Tommaso Comparin <tommaso.comparin@exact-lab.it>
 # Marco Franzon <marco.franzon@exact-lab.it>
 #
 # Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
 # University of Zurich
-import logging
 import math
 import shlex
 import subprocess  # nosec
 import sys
 import time
 from concurrent.futures import Future
 from concurrent.futures import InvalidStateError
@@ -26,14 +25,16 @@
 from typing import Sequence
 
 import cloudpickle
 from cfut import SlurmExecutor
 from cfut.util import random_string
 
 from ....config import get_settings
+from ....logger import set_logger
+from ....logger import wrap_with_timing_logs
 from ....syringe import Inject
 from .._common import get_task_file_paths
 from .._common import TaskFiles
 from ..common import JobExecutionError
 from ..common import TaskExecutionError
 from ._batching import heuristics
 from ._executor_wait_thread import FractalSlurmWaitThread
@@ -41,14 +42,17 @@
 from ._slurm_config import SlurmConfig
 from ._subprocess_run_as_user import _glob_as_user
 from ._subprocess_run_as_user import _path_exists_as_user
 from ._subprocess_run_as_user import _run_command_as_user
 from fractal_server import __VERSION__
 
 
+logger = set_logger(__name__)
+
+
 class SlurmJob:
     """
     Collect information related to a FractalSlurmExecutor job
 
     This includes three groups of attributes:
 
     1. Attributes related to the (possibly multi-task) SLURM job, e.g.
@@ -206,15 +210,15 @@
             if self.slurm_user:
                 raise RuntimeError(f"{self.slurm_user=}, {working_dir_user=}")
             else:
                 working_dir_user = working_dir
         if not _path_exists_as_user(
             path=str(working_dir_user), user=self.slurm_user
         ):
-            logging.info(f"Missing folder {working_dir_user=}")
+            logger.info(f"Missing folder {working_dir_user=}")
 
         self.working_dir_user = working_dir_user
         self.map_jobid_to_slurm_files = {}
 
         # Set the attribute slurm_poll_interval for self.wait_thread (see
         # cfut.SlurmWaitThread)
         if not slurm_poll_interval:
@@ -290,15 +294,15 @@
         if task_files is None:
             task_files = self.get_default_task_files()
 
         # Set slurm_file_prefix
         slurm_file_prefix = task_files.file_prefix
 
         # Include common_script_lines in extra_lines
-        logging.debug(
+        logger.debug(
             f"Adding {self.common_script_lines=} to "
             f"{slurm_config.extra_lines=}, from submit method."
         )
         current_extra_lines = slurm_config.extra_lines or []
         slurm_config.extra_lines = (
             current_extra_lines + self.common_script_lines
         )
@@ -377,15 +381,15 @@
         # Set defaults, if needed
         if not slurm_config:
             slurm_config = get_default_slurm_config()
         if task_files is None:
             task_files = self.get_default_task_files()
 
         # Include common_script_lines in extra_lines
-        logging.debug(
+        logger.debug(
             f"Adding {self.common_script_lines=} to "
             f"{slurm_config.extra_lines=}, from map method."
         )
         current_extra_lines = slurm_config.extra_lines or []
         slurm_config.extra_lines = (
             current_extra_lines + self.common_script_lines
         )
@@ -469,14 +473,15 @@
                         yield res
             finally:
                 for future in fs:
                     future.cancel()
 
         return result_iterator()
 
+    @wrap_with_timing_logs
     def _submit_job(
         self,
         fun: Callable[..., Any],
         slurm_file_prefix: str,
         task_files: TaskFiles,
         slurm_config: SlurmConfig,
         single_task_submission: bool = False,
@@ -612,14 +617,15 @@
             jobid=jobid,
         )
 
         with self.jobs_lock:
             self.jobs[jobid] = (fut, job)
         return fut
 
+    @wrap_with_timing_logs
     def _prepare_JobExecutionError(
         self, jobid: str, info: str
     ) -> JobExecutionError:
         """
         Prepare the JobExecutionError for a given job
 
             1. Wait for `FRACTAL_SLURM_KILLWAIT_INTERVAL` seconds, so that
@@ -651,14 +657,15 @@
             cmd_file=slurm_script_file,
             stdout_file=slurm_stdout_file,
             stderr_file=slurm_stderr_file,
             info=info,
         )
         return job_exc
 
+    @wrap_with_timing_logs
     def _completion(self, jobid: str) -> None:
         """
         Callback function to be executed whenever a job finishes.
 
         This function is executed by self.wait_thread (triggered by either
         finding an existing output pickle file `out_path` or finding that the
         SLURM job is over). Since this takes place on a different thread,
@@ -738,15 +745,15 @@
                         "seconds.\n"
                     )
                     job_exc = self._prepare_JobExecutionError(jobid, info=info)
                     try:
                         fut.set_exception(job_exc)
                         return
                     except InvalidStateError:
-                        logging.warning(
+                        logger.warning(
                             f"Future {fut} (SLURM job ID: {jobid}) was already"
                             " cancelled, exit from"
                             " FractalSlurmExecutor._completion."
                         )
                         if not self.keep_pickle_files:
                             in_path.unlink()
                         self._cleanup(jobid)
@@ -789,15 +796,15 @@
                                     kwargs[key] = proxy.kwargs[key]
                             exc = TaskExecutionError(proxy.tb, **kwargs)
                             fut.set_exception(exc)
                             return
                     if not self.keep_pickle_files:
                         out_path.unlink()
                 except InvalidStateError:
-                    logging.warning(
+                    logger.warning(
                         f"Future {fut} (SLURM job ID: {jobid}) was already"
                         " cancelled, exit from"
                         " FractalSlurmExecutor._completion."
                     )
                     if not self.keep_pickle_files:
                         out_path.unlink()
                         in_path.unlink()
@@ -815,20 +822,21 @@
             return
 
         except Exception as e:
             try:
                 fut.set_exception(e)
                 return
             except InvalidStateError:
-                logging.warning(
+                logger.warning(
                     f"Future {fut} (SLURM job ID: {jobid}) was already"
                     " cancelled, exit from"
                     " FractalSlurmExecutor._completion."
                 )
 
+    @wrap_with_timing_logs
     def _copy_files_from_user_to_server(
         self,
         job: SlurmJob,
     ):
         """
         Impersonate the user and copy task-related files
 
@@ -845,35 +853,35 @@
         Arguments:
             job:
                 `SlurmJob` object (needed for its prefixes-related attributes).
 
         Raises:
             JobExecutionError: If a `cat` command fails.
         """
-        logging.debug("Enter _copy_files_from_user_to_server")
+        logger.debug("Enter _copy_files_from_user_to_server")
         if self.working_dir_user == self.working_dir:
             return
 
         prefixes = set(
             [job.slurm_file_prefix] + list(job.wftask_file_prefixes)
         )
 
-        logging.debug(f"[_copy_files_from_user_to_server] {prefixes=}")
-        logging.debug(
+        logger.debug(f"[_copy_files_from_user_to_server] {prefixes=}")
+        logger.debug(
             f"[_copy_files_from_user_to_server] {str(self.working_dir_user)=}"
         )
 
         for prefix in prefixes:
 
             files_to_copy = _glob_as_user(
                 folder=str(self.working_dir_user),
                 user=self.slurm_user,
                 startswith=prefix,
             )
-            logging.debug(
+            logger.debug(
                 "[_copy_files_from_user_to_server] "
                 f"{prefix=}, {len(files_to_copy)=}"
             )
 
             for source_file_name in files_to_copy:
                 if " " in source_file_name:
                     raise ValueError(
@@ -894,22 +902,23 @@
                 )
                 if res.returncode != 0:
                     info = (
                         f'Running cmd="{cmd}" as {self.slurm_user=} failed\n\n'
                         f"{res.returncode=}\n\n"
                         f"{res.stdout=}\n\n{res.stderr=}\n"
                     )
-                    logging.error(info)
+                    logger.error(info)
                     raise JobExecutionError(info)
                 # Write to dest_file_path (including empty files)
                 dest_file_path = str(self.working_dir / source_file_name)
                 with open(dest_file_path, "wb") as f:
                     f.write(res.stdout)
-        logging.debug("[_copy_files_from_user_to_server] End")
+        logger.debug("[_copy_files_from_user_to_server] End")
 
+    @wrap_with_timing_logs
     def _start(
         self,
         job: SlurmJob,
     ) -> tuple[str, SlurmJob]:
         """
         Submit function for execution on a SLURM cluster
         """
@@ -961,38 +970,39 @@
                 encoding="utf-8",
             )
         except subprocess.CalledProcessError as e:
             error_msg = (
                 f"Submit command `{full_command}` failed. "
                 f"Original error:\n{str(e)}"
             )
-            logging.error(error_msg)
+            logger.error(error_msg)
             raise JobExecutionError(info=error_msg)
         try:
             jobid = int(output.stdout)
         except ValueError as e:
             error_msg = (
                 f"Submit command `{full_command}` returned "
                 f"`{output.stdout=}` which cannot be cast to an integer "
                 f"SLURM-job ID. Original error:\n{str(e)}"
             )
-            logging.error(error_msg)
+            logger.error(error_msg)
             raise JobExecutionError(info=error_msg)
         jobid_str = str(jobid)
 
         # Plug SLURM job id in stdout/stderr file paths
         job.slurm_stdout = Path(
             job.slurm_stdout.as_posix().replace("%j", jobid_str)
         )
         job.slurm_stderr = Path(
             job.slurm_stderr.as_posix().replace("%j", jobid_str)
         )
 
         return jobid_str, job
 
+    @wrap_with_timing_logs
     def _prepare_sbatch_script(
         self,
         *,
         list_commands: list[str],
         slurm_out_path: str,
         slurm_err_path: str,
         slurm_config: SlurmConfig,
@@ -1002,15 +1012,15 @@
         mem_per_task_MB = slurm_config.mem_per_task_MB
 
         # Set ntasks
         ntasks = min(len(list_commands), num_tasks_max_running)
         if len(list_commands) < num_tasks_max_running:
             ntasks = len(list_commands)
             slurm_config.parallel_tasks_per_job = ntasks
-            logging.info(
+            logger.debug(
                 f"{len(list_commands)=} is smaller than "
                 f"{num_tasks_max_running=}. Setting {ntasks=}."
             )
 
         # Prepare SLURM preamble based on SlurmConfig object
         script_lines = slurm_config.to_sbatch_preamble()
 
@@ -1019,15 +1029,15 @@
         script_lines.extend(
             [
                 f"#SBATCH --err={slurm_err_path}",
                 f"#SBATCH --out={slurm_out_path}",
             ]
         )
         script_lines = slurm_config.sort_script_lines(script_lines)
-        logging.debug(script_lines)
+        logger.debug(script_lines)
 
         # Complete script preamble
         script_lines.append("\n")
 
         # Include command lines
         tmp_list_commands = copy(list_commands)
         while tmp_list_commands:
@@ -1039,14 +1049,15 @@
                     f"{cmd} &"
                 )
         script_lines.append("wait\n")
 
         script = "\n".join(script_lines)
         return script
 
+    @wrap_with_timing_logs
     def get_default_task_files(self) -> TaskFiles:
         """
         This will be called when self.submit or self.map are called from
         outside fractal-server, and then lack some optional arguments.
         """
         import random
```

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/app/runner/common.py` & `fractal_server-1.2.0a4/fractal_server/app/runner/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import Optional
 
 from pydantic import BaseModel
 
-from ...utils import close_logger as close_job_logger  # noqa F401
+from ...logger import close_logger as close_job_logger  # noqa F401
 from ..models import Dataset
 from ..models import Project
 from ..models.workflow import Workflow
 
 
 class TaskExecutionError(RuntimeError):
     """
```

### Comparing `fractal_server-1.2.0a3/fractal_server/app/security/__init__.py` & `fractal_server-1.2.0a4/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.2.0a4/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.2.0a4/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/README.md` & `fractal_server-1.2.0a4/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__init__.py` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.2.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/_validators.py` & `fractal_server-1.2.0a4/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.2.0a4/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/manifest.py` & `fractal_server-1.2.0a4/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/project.py` & `fractal_server-1.2.0a4/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/state.py` & `fractal_server-1.2.0a4/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/task.py` & `fractal_server-1.2.0a4/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/user.py` & `fractal_server-1.2.0a4/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/schemas/workflow.py` & `fractal_server-1.2.0a4/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.2.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/test_applyworkflow.py` & `fractal_server-1.2.0a4/fractal_server/common/tests/test_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.2.0a4/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.2.0a4/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/test_project.py` & `fractal_server-1.2.0a4/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/test_state.py` & `fractal_server-1.2.0a4/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/test_task.py` & `fractal_server-1.2.0a4/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/test_user.py` & `fractal_server-1.2.0a4/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.2.0a4/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/config.py` & `fractal_server-1.2.0a4/fractal_server/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,19 +234,20 @@
 
     FRACTAL_RUNNER_WORKING_BASE_DIR: Optional[Path]
     """
     Base directory for running jobs / workflows. All artifacts required to set
     up, run and tear down jobs are placed in subdirs of this directory.
     """
 
-    FRACTAL_LOGGING_LEVEL: int = 30
+    FRACTAL_LOGGING_LEVEL: int = logging.INFO
     """
-    Logging verbosity for main Fractal logger (`30` means `WARNING` - see
-    [logging
-    levels](https://docs.python.org/3/library/logging.html#logging-levels)).
+    Logging-level threshold for logging
+
+    Only logs of with this level (or higher) will appear in the console logs;
+    see details [here](../internals/logs/).
     """
 
     FRACTAL_LOCAL_RUNNER_MAX_TASKS_PER_WORKFLOW: Optional[int] = None
     """
     Maximum number of components that a parallel task may process
     simultaneously, for the [local backend](../internals/runners/local/).  If
     `None`, no limit is set.
```

### Comparing `fractal_server-1.2.0a3/fractal_server/main.py` & `fractal_server-1.2.0a4/fractal_server/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
 # University of Zurich
 #
 # Original authors:
 # Jacopo Nespolo <jacopo.nespolo@exact-lab.it>
 # Marco Franzon <marco.franzon@exact-lab.it>
+# Tommaso Comaprin <tommaso.comparin@exact-lab.it>
 #
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
 """
 # Application factory
 
 This module sets up the FastAPI application that serves the Fractal Server.
 """
 import contextlib
-import logging
 from typing import Optional
 
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi_users.exceptions import UserAlreadyExists
 
 from .app.db import get_db
 from .app.security import get_user_db
 from .app.security import get_user_manager
 from .common.schemas.user import UserCreate
 from .config import get_settings
+from .logger import set_logger
 from .syringe import Inject
 
 get_async_session_context = contextlib.asynccontextmanager(get_db)
 get_user_db_context = contextlib.asynccontextmanager(get_user_db)
 get_user_manager_context = contextlib.asynccontextmanager(get_user_manager)
 
+logger = set_logger(__name__)
+
 
 def collect_routers(app: FastAPI) -> None:
     """
     Register the routers to the application
 
     Args:
         app:
@@ -105,18 +108,18 @@
                         email=email,
                         password=password,
                         is_superuser=is_superuser,
                     )
                     if slurm_user:
                         kwargs["slurm_user"] = slurm_user
                     user = await user_manager.create(UserCreate(**kwargs))
-                    logging.info(f"User {user.email} created")
+                    logger.info(f"User {user.email} created")
 
     except UserAlreadyExists:
-        logging.warning(f"User {email} already exists")
+        logger.warning(f"User {email} already exists")
 
 
 def start_application() -> FastAPI:
     """
     Create and initialise the application
 
     It performs the following initialisation steps:
```

### Comparing `fractal_server-1.2.0a3/fractal_server/migrations/env.py` & `fractal_server-1.2.0a4/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/migrations/script.py.mako` & `fractal_server-1.2.0a4/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py` & `fractal_server-1.2.0a4/fractal_server/migrations/versions/385aa8c18489_add_user_cache_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/migrations/versions/47072e0106ce_initial_schema.py` & `fractal_server-1.2.0a4/fractal_server/migrations/versions/47072e0106ce_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py` & `fractal_server-1.2.0a4/fractal_server/migrations/versions/6dede8d6fd9d_drop_project_project_dir.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/syringe.py` & `fractal_server-1.2.0a4/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.2.0a3/fractal_server/tasks/collection.py` & `fractal_server-1.2.0a4/fractal_server/tasks/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 This module takes care of installing tasks so that fractal can execute them
 
 Tasks can be private or public. Private tasks are installed under
 `Settings.FRACTAL_TASKS_DIR/{username}`. For public tasks, `username =
 .fractal`.
 """
 import json
-import logging
 import shutil
 import sys
 from io import IOBase
 from pathlib import Path
 from typing import Optional
 from typing import Union
 from zipfile import ZipFile
@@ -28,14 +27,15 @@
 from pydantic import root_validator
 
 from ..common.schemas import ManifestV1
 from ..common.schemas import TaskCollectPip
 from ..common.schemas import TaskCollectStatus
 from ..common.schemas import TaskCreate
 from ..config import get_settings
+from ..logger import get_logger
 from ..syringe import Inject
 from ..utils import execute_command
 
 
 FRACTAL_PUBLIC_TASK_SUBDIR = ".fractal"
 
 
@@ -172,15 +172,14 @@
 
 
 def create_package_dir_pip(
     *,
     task_pkg: _TaskCollectPip,
     user: Optional[str] = None,
     create: bool = True,
-    logger_name: Optional[str] = None,
     **_,  # FIXME remove this catch-all argument
 ) -> Path:
     settings = Inject(get_settings)
     user = user or FRACTAL_PUBLIC_TASK_SUBDIR
 
     package_dir = f"{task_pkg.package}{task_pkg.version or ''}"
     venv_path = settings.FRACTAL_TASKS_DIR / user / package_dir  # type: ignore
@@ -257,34 +256,34 @@
     task_pkg: _TaskCollectPip,
     venv_path: Path,
     logger_name: str,
 ) -> list[TaskCreate]:
     """
     Create environment and install package
     """
-    logger = logging.getLogger(logger_name)
+    logger = get_logger(logger_name)
     try:
         logger.debug("Creating venv and installing package")
 
         python_bin, package_root = await _create_venv_install_package(
             path=venv_path,
             task_pkg=task_pkg,
             logger_name=logger_name,
         )
 
-        logger.debug("loading manifest")
+        logger.debug("Loading task manifest")
 
         task_list = load_manifest(
             package_root=package_root,
             python_bin=python_bin,
             source=task_pkg.source,
         )
-        logger.debug("manifest loaded")
+        logger.debug("Loaded task manifest")
     except Exception as e:
-        logger.debug("manifest loading failed")
+        logger.error("Task manifest loading failed")
         raise e
     return task_list
 
 
 def read_manifest(file: Union[Path, IOBase]) -> ManifestV1:
     """
     Read and parse manifest file
```

### Comparing `fractal_server-1.2.0a3/fractal_server/utils.py` & `fractal_server-1.2.0a4/fractal_server/logger.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,136 +6,148 @@
 # Tommaso Comparin <tommaso.comparin@exact-lab.it>
 #
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
 """
-This module provides general purpose utilities that are not specific to any
-subsystem.
+This module provides logging utilities
 """
-import asyncio
+import functools
 import logging
-from datetime import datetime
-from datetime import timezone
+import time
 from pathlib import Path
-from shlex import split as shlex_split
+from typing import Callable
 from typing import Optional
-from warnings import warn as _warn
+from typing import Union
 
 from .config import get_settings
 from .syringe import Inject
 
 
-def close_logger(logger: logging.Logger) -> None:
-    """
-    Close all FileHandles of a logger, if any.
-    """
-    for handle in logger.handlers:
-        if isinstance(handle, logging.FileHandler):
-            handle.close()
-
-
-def get_timestamp() -> datetime:
-    """
-    Get timezone aware timestamp.
-    """
-    return datetime.now(tz=timezone.utc)
+LOG_FORMAT = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+LOG_FORMATTER = logging.Formatter(LOG_FORMAT)
 
 
-def warn(message):
+def get_logger(logger_name: Optional[str] = None) -> logging.Logger:
     """
-    Custom warning that becomes an error in staging and production deployments
+    Wrap the
+    [`logging.getLogger`](https://docs.python.org/3/library/logging.html#logging.getLogger)
+    function.
+
+    The typical use case for this function is to retrieve a logger that was
+    already defined, as in the following example:
+    ```python
+    def function1(logger_name):
+        logger = get_logger(logger_name)
+        logger.info("Info from function1")
+
+    def funtion2():
+        logger_name = "my_logger"
+        logger = set_logger(logger_name)
+        logger.info("Info from function2")
+        function1(logger_name)
+        close_logger(logger)
+    ```
 
-    This works towards assuring that warnings do not make their way to staing
-    and production.
-
-    Raises:
-        RuntimeError: if the deployment type is not `testing` or `development`.
+    Arguments:
+        logger_name: Name of logger
+    Returns:
+        Logger with name `logger_name`
     """
-    settings = Inject(get_settings)
-    if settings.DEPLOYMENT_TYPE in ["testing", "development"]:
-        _warn(message, RuntimeWarning)
-    else:
-        raise RuntimeError(message)
+    return logging.getLogger(logger_name)
 
 
 def set_logger(
+    logger_name: str,
     *,
-    logger_name: Optional[str] = None,
-    log_file_path: Optional[Path] = None,
-    level: Optional[int] = None,
-    formatter: Optional[logging.Formatter] = None,
+    log_file_path: Optional[Union[str, Path]] = None,
 ) -> logging.Logger:
     """
-    Set up and return a logger
+    Set up a `fractal-server` logger
+
+    The logger (a `logging.Logger` object) will have the following properties:
+
+    * The attribute `Logger.propagate` set to `False`;
+    * One and only one `logging.StreamHandler` handler, with severity level set
+    to
+    [`FRACTAL_LOGGING_LEVEL`](../../../../configuration/#fractal_server.config.Settings.FRACTAL_LOGGING_LEVEL)
+    and formatter set as in the `logger.LOG_FORMAT` variable from the current
+    module;
+    * One or many `logging.FileHandler` handlers, including one pointint to
+    `log_file_path` (if set); all these handlers have severity level set to
+    `logging.DEBUG`.
 
     Args:
-        logger_name:
-            The identifier of the logger.
-        log_file_path:
-            Path to the log file.
-        level:
-            Logging level of this logger.
-        formatter:
-            Custom formatter.
+        logger_name: The identifier of the logger.
+        log_file_path: Path to the log file.
 
     Returns:
-        logger:
-            The logger, as configured by the arguments.
+        logger: The logger, as configured by the arguments.
     """
-    if not level:
-        settings = Inject(get_settings)
-        level = settings.FRACTAL_LOGGING_LEVEL
+
     logger = logging.getLogger(logger_name)
-    logger.setLevel(level)
-    if log_file_path:
+    logger.propagate = False
+    logger.setLevel(logging.DEBUG)
+
+    current_stream_handlers = [
+        handler
+        for handler in logger.handlers
+        if isinstance(handler, logging.StreamHandler)
+    ]
+
+    if not current_stream_handlers:
+        stream_handler = logging.StreamHandler()
+        settings = Inject(get_settings)
+        stream_handler.setLevel(settings.FRACTAL_LOGGING_LEVEL)
+        stream_handler.setFormatter(LOG_FORMATTER)
+        logger.addHandler(stream_handler)
+
+    if log_file_path is not None:
         file_handler = logging.FileHandler(log_file_path, mode="a")
-        file_handler.setFormatter(formatter)
+        file_handler.setLevel(logging.DEBUG)
+        file_handler.setFormatter(LOG_FORMATTER)
+        file_handler.setFormatter(LOG_FORMATTER)
         logger.addHandler(file_handler)
+        current_file_handlers = [
+            handler
+            for handler in logger.handlers
+            if isinstance(handler, logging.FileHandler)
+        ]
+        if len(current_file_handlers) > 1:
+            logger.warning(f"Logger {logger_name} has multiple file handlers.")
+
     return logger
 
 
-async def execute_command(
-    *,
-    cwd: Path,
-    command: str,
-    logger_name: Optional[str] = None,
-) -> str:
+def close_logger(logger: logging.Logger) -> None:
     """
-    Execute arbitrary command
+    Close all handlers associated to a `logging.Logger` object
 
-    If the command returns a return code different from zero, a RuntimeError
-    containing the stderr is raised.
+    Arguments:
+        logger: The actual logger
+    """
+    for handle in logger.handlers:
+        handle.close()
 
-    Args:
-        cwd:
-            The working directory for the command execution.
-        command:
-            The command to execute.
 
-    Returns:
-        stdout:
-            The stdout from the command execution.
+def wrap_with_timing_logs(func: Callable):
+    """
+    Wrap a function with start/end logs, including the elapsed time
+    """
+
+    @functools.wraps(func)
+    def wrapped(*args, **kwargs):
+        name = func.__name__
+        logger = set_logger(name)
+        logger.debug(f'START execution of "{name}"')
+
+        t_start = time.perf_counter()
+        res = func(*args, **kwargs)
+        elapsed = time.perf_counter() - t_start
+
+        logger.debug(
+            f'END   execution of "{name}"; ' f"elapsed: {elapsed:.3f} seconds"
+        )
+        return res
 
-    Raises:
-        RuntimeError: if the process exited with non-zero status. The error
-            string is set to the `stderr` of the process.
-    """
-    command_split = shlex_split(command)
-    cmd, *args = command_split
-
-    logger = set_logger(logger_name=logger_name)
-    proc = await asyncio.create_subprocess_exec(
-        cmd,
-        *args,
-        stdout=asyncio.subprocess.PIPE,
-        stderr=asyncio.subprocess.PIPE,
-        cwd=cwd,
-    )
-    stdout, stderr = await proc.communicate()
-    logger.debug(f"Subprocess call to: {command}")
-    logger.debug(stdout.decode("utf-8"))
-    logger.debug(stderr.decode("utf-8"))
-    if proc.returncode != 0:
-        raise RuntimeError(stderr.decode("utf-8"))
-    return stdout.decode("utf-8")
+    return wrapped
```

### Comparing `fractal_server-1.2.0a3/pyproject.toml` & `fractal_server-1.2.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.2.0a3"
+version = "1.2.0a4"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -71,15 +71,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.2.0a3"
+current_version = "1.2.0a4"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.2.0a3/setup.py` & `fractal_server-1.2.0a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
  'slurm': ['clusterfutures>=0.5,<0.6']}
 
 entry_points = \
 {'console_scripts': ['fractalctl = fractal_server.__main__:run']}
 
 setup_kwargs = {
     'name': 'fractal-server',
-    'version': '1.2.0a3',
+    'version': '1.2.0a4',
     'description': 'Server component of the Fractal analytics platform',
     'long_description': '# Fractal Server\n\n[![PyPI version](https://img.shields.io/pypi/v/fractal-server?color=gree)](https://pypi.org/project/fractal-server/)\n[![CI Status](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-server/actions/workflows/ci.yml)\n[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-server/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-server/blob/python-coverage-comment-action-data/htmlcov/index.html)\n[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\nFractal is a framework to process high content imaging data at scale and\nprepare it for interactive visualization.\n\n![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)\n\nThis is the server component of the fractal analytics platform.\nFind more information about Fractal in general and the other repositories at\nthe [Fractal home page](https://fractal-analytics-platform.github.io).\n\n\n## Documentation\n\nSee https://fractal-analytics-platform.github.io/fractal-server.\n\n# Contributors and license\n\nUnless otherwise stated in each individual module, all Fractal components are\nreleased according to a BSD 3-Clause License, and Copyright is with Friedrich\nMiescher Institute for Biomedical Research and University of Zurich.\n\nThe SLURM compatibility layer is based on\n[`clusterfutures`](https://github.com/sampsyo/clusterfutures), by\n[@sampsyo](https://github.com/sampsyo) and collaborators, and it is released\nunder the terms of the MIT license.\n\nFractal was conceived in the Liberali Lab at the Friedrich Miescher Institute\nfor Biomedical Research and in the Pelkmans Lab at the University of Zurich\n(both in Switzerland). The project lead is with\n[@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).\nThe core development is done under contract by\n[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)\n& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).\n',
     'author': 'Jacopo Nespolo',
     'author_email': 'jacopo.nespolo@exact-lab.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fractal-analytics-platform/fractal-server',
```

### Comparing `fractal_server-1.2.0a3/PKG-INFO` & `fractal_server-1.2.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.2.0a3
+Version: 1.2.0a4
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

