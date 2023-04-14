# Comparing `tmp/cortex_cli-1.12.4.tar.gz` & `tmp/cortex_cli-1.12.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.12.4.tar", last modified: Tue Apr 11 16:36:27 2023, max compression
+gzip compressed data, was "cortex_cli-1.12.5.tar", last modified: Fri Apr 14 18:12:12 2023, max compression
```

## Comparing `cortex_cli-1.12.4.tar` & `cortex_cli-1.12.5.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.12.4/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-04-11 16:35:05.000000 cortex_cli-1.12.4/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.12.4/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3990 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.12.4/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.12.4/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      880 2023-04-07 17:56:26.000000 cortex_cli-1.12.4/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.12.4/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.12.4/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    22343 2023-04-11 16:30:05.000000 cortex_cli-1.12.4/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.12.4/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4124 2023-04-11 16:15:11.000000 cortex_cli-1.12.4/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    10969 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     7010 2023-03-21 15:45:49.000000 cortex_cli-1.12.4/cortex_cli/core/models/cortex_model.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-11 16:29:39.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-11 16:28:41.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      533 2023-04-06 19:56:03.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-06 19:56:06.000000 cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.12.4/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1893 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-11 16:36:27.000000 cortex_cli-1.12.4/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.12.4/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-04-11 16:36:27.169662 cortex_cli-1.12.4/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1053 2023-04-07 18:01:54.000000 cortex_cli-1.12.4/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.12.5/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-04-14 18:12:01.000000 cortex_cli-1.12.5/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.12.5/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3990 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.12.5/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.12.5/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      880 2023-04-07 17:56:26.000000 cortex_cli-1.12.5/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.12.5/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.12.5/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    22365 2023-04-14 16:22:47.000000 cortex_cli-1.12.5/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.12.5/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-14 17:16:40.000000 cortex_cli-1.12.5/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-13 17:02:54.000000 cortex_cli-1.12.5/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     7183 2023-04-14 17:17:17.000000 cortex_cli-1.12.5/cortex_cli/core/models/cortex_model.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1681 2023-04-14 17:21:25.000000 cortex_cli-1.12.5/cortex_cli/core/secrets_manager.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-11 16:29:39.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-11 16:28:41.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      533 2023-04-06 19:56:03.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-06 19:56:06.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1928 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.12.5/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1053 2023-04-07 18:01:54.000000 cortex_cli-1.12.5/setup.py
```

### Comparing `cortex_cli-1.12.4/README.md` & `cortex_cli-1.12.5/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.12.5/cortex_cli/cli/api/github_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.12.5/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.12.5/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.12.5/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/cli/configure.py` & `cortex_cli-1.12.5/cortex_cli/cli/configure.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.12.5/cortex_cli/cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/cli/generic_get.py` & `cortex_cli-1.12.5/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/cli/inferences.py` & `cortex_cli-1.12.5/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/cli/models.py` & `cortex_cli-1.12.5/cortex_cli/cli/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,19 +217,20 @@
 
 @ModelsCli.subcommand('run')
 class RunModelPipeline(CliApiBase):
     _path = plumbum.cli.SwitchAttr(
         names=['-p', '--path'],
         argtype=str,
         envname='MODEL_PATH',
-        default='.',
+        default='.'
     )
 
     _tracking = plumbum.cli.Flag(
-        names=['-t', '--tracking']
+        names=['-t', '--tracking'],
+        default=True
     )
 
     # Properties
 
     @property
     def _model_id(self):
         return self._model_json['_id'] if self._model_json else None
```

### Comparing `cortex_cli-1.12.4/cortex_cli/cli/pipelines.py` & `cortex_cli-1.12.5/cortex_cli/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/core/cortex_data.py` & `cortex_cli-1.12.5/cortex_cli/core/cortex_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     
     def exists(self):
         return os.path.isfile(self.local_path)
 
 
 class CortexData():
     _api_url = None
-    _api_key = None
+    _headers = None
     _local_dir = None
     _files = []
 
 
     @property
     def files(self):
         return self._files
@@ -126,13 +126,13 @@
         # Syncs an existing file to S3
         if os.path.exists(file.local_path):
             raise Exception('Function not yet implemented!')
         else:
             raise Exception(f'Error syncing file to cortex! File does not exist: {file.local_path}')
 
 
-    def find_file(self, name):
+    def find_file(self, name:str):
         # Find file with name
         for file in self._files:
             if file.name == name:
                 return file
-        return None
+        raise FileNotFoundError(f'File {name} not found in Cortex data.')
```

### Comparing `cortex_cli-1.12.4/cortex_cli/core/drift_checks.py` & `cortex_cli-1.12.5/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.12.5/cortex_cli/core/ethics_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self._sensitive_predictor_columns = sensitive_predictor_columns
         self._label_column = label_column
 
 
     def run(self):
         file = self._file.loaded_data#self._file.load()
         if file is None:
-            return ('The file has not been loaded by the model', EthicsRiskEnum.NO_RISK)
+            return (None, EthicsRiskEnum.NO_RISK)
         if self._ethics_type == EthicsTypeEnum.BALANCE:
             return self.data_balance_ethics_check(file)
         elif self._ethics_type == EthicsTypeEnum.BIAS:
             return self.data_bias_ethics_checks(file, self._sensitive_predictor_columns, self._label_column)
         elif self._ethics_type == EthicsTypeEnum.PII:
             return self.data_contains_pii_ethics_check(file, self._sensitive_predictor_columns)
 
@@ -250,26 +250,28 @@
         # Get list of ethics checks with type ethics_check_type
         ethics_checks = [ec for ec in self._ethics_checks if ec.ethics_type == ethics_check_type]
 
         # Initialize default return values
         result_str = ''
         risk = EthicsRiskEnum.NO_RISK
 
-        if len(ethics_checks) == 0:
-            result_str = 'No files have been loaded to run ethics check against.'
-
         # Loop through all ethics checks with type ethics_check_type
         for ethics_check in ethics_checks:
             # Run ethics check
             ethics_result = ethics_check.run()
 
-            # Set risk level
-            if ethics_result[1] is not EthicsRiskEnum.NO_RISK:
-                risk = ethics_result[1]
-            result_str += f'{ethics_check.file.name}: {ethics_result[0]}\n'
+            if ethics_result[0] is not None:
+
+                # Set risk level
+                if ethics_result[1] is not EthicsRiskEnum.NO_RISK:
+                    risk = ethics_result[1]
+                result_str += f'{ethics_check.file.name}: {ethics_result[0]}\n'
+        
+        if len(ethics_checks) == 0 or result_str == '':
+            result_str = 'No files have been loaded to run ethics check against.'
 
         # Save ethics results
         ethics_result = EthicsResult(ethics_check_type, result_str[:-1], risk)
         self._ethics_results.append(ethics_result)
 
         return ethics_result
```

### Comparing `cortex_cli-1.12.4/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.12.5/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.12.5/cortex_cli/core/models/cortex_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import mlflow.pyfunc
 
 from cortex_cli.core.cortex_data import CortexData
 from cortex_cli.core.ethics_checks import EthicsManager, EthicsTypeEnum
 from cortex_cli.core.drift_checks import DriftManager, DriftTypeEnum
+from cortex_cli.core.secrets_manager import SecretsManager
 
 
 class CortexModel(mlflow.pyfunc.PythonModel):
     """
     Base class for machine learning models. Not used directly.
     """
 
@@ -15,14 +16,15 @@
         self.params = params
         self.input_example = None
         self.output_example = None
         self.model_type = model_type
         self.cortex_data = CortexData(model_id, api_url, headers)
         self.ethics_manager = None
         self.drift_manager = DriftManager()
+        self.secrets_manager = SecretsManager(api_url, headers)
 
         self.metrics = {}
         self.custom_objects = {}
 
 
     def download_data(self):
         """Downloads data during initial training
@@ -92,14 +94,16 @@
             Parameters:
             N/A
 
             Returns:
             N/A
 
         """
+        self.secrets_manager.reset_secrets()
+
         try:
             for s in ['cortex_data', 'ethics_manager']:
                 if s in self.__dict__:
                     del self.__dict__[s]
         except AttributeError:
             pass
```

### Comparing `cortex_cli-1.12.4/cortex_cli/ml_model_template/.gitignore` & `cortex_cli-1.12.5/cortex_cli/ml_model_template/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/ml_model_template/README.md` & `cortex_cli-1.12.5/cortex_cli/ml_model_template/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/cortex.yml` & `cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/cortex.yml`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.12.5/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.12.5/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.4/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.12.5/cortex_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 cortex_cli/cli/api/__init__.py
 cortex_cli/cli/api/github_api.py
 cortex_cli/cli/api/http_api.py
 cortex_cli/core/__init__.py
 cortex_cli/core/cortex_data.py
 cortex_cli/core/drift_checks.py
 cortex_cli/core/ethics_checks.py
+cortex_cli/core/secrets_manager.py
 cortex_cli/core/mlflow/__init__.py
 cortex_cli/core/mlflow/mlflow_cortex.py
 cortex_cli/core/models/__init__.py
 cortex_cli/core/models/cortex_model.py
 cortex_cli/ml_model_template/.gitignore
 cortex_cli/ml_model_template/README.md
 cortex_cli/ml_model_template/__init__.py
```

### Comparing `cortex_cli-1.12.4/setup.py` & `cortex_cli-1.12.5/setup.py`

 * *Files identical despite different names*

