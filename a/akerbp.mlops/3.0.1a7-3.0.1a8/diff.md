# Comparing `tmp/akerbp.mlops-3.0.1a7.tar.gz` & `tmp/akerbp.mlops-3.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-x0jo844_/akerbp.mlops-3.0.1a7.tar", last modified: Mon Mar 27 13:53:30 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-5qlr_ntb/akerbp.mlops-3.0.1a8.tar", last modified: Fri Apr 14 11:53:09 2023, max compression
```

## Comparing `akerbp.mlops-3.0.1a7.tar` & `akerbp.mlops-3.0.1a8.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.069054 akerbp.mlops-3.0.1a7/
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    49463 2023-03-27 13:53:30.069054 akerbp.mlops-3.0.1a7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35941 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     3998 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/build.sh
--rw-rw-rw-   0 root         (0) root         (0)     3510 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/increment_package_version.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/install.sh
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/mlops_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.061054 akerbp.mlops-3.0.1a7/model_artifact/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/model_artifact/README.md
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/model_artifact/dummy.joblib
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.061054 akerbp.mlops-3.0.1a7/model_code/
--rw-rw-rw-   0 root         (0) root         (0)     3879 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/model_code/model.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/model_code/requirements.model
--rw-rw-rw-   0 root         (0) root         (0)     2850 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/model_code/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/promote_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1498 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/remove_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-27 13:53:30.069054 akerbp.mlops-3.0.1a7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.057054 akerbp.mlops-3.0.1a7/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.057054 akerbp.mlops-3.0.1a7/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.065054 akerbp.mlops-3.0.1a7/src/akerbp/mlops/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-03-27 13:53:29.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.065054 akerbp.mlops-3.0.1a7/src/akerbp/mlops/cdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/cdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/cdf/download_function_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2994 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/cdf/handler.py
--rw-rw-rw-   0 root         (0) root         (0)    38633 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/cdf/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.065054 akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16951 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/logger_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/mappings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.065054 akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2187 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     6555 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/deploy_prediction_service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/deploy_training_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21689 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/platforms.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.065054 akerbp.mlops-3.0.1a7/src/akerbp/mlops/model_manager/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/model_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22239 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/model_manager/model_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.069054 akerbp.mlops-3.0.1a7/src/akerbp/mlops/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5919 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/services/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3165 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/services/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/src/akerbp/mlops/services/training.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.065054 akerbp.mlops-3.0.1a7/src/akerbp.mlops.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    49463 2023-03-27 13:53:30.000000 akerbp.mlops-3.0.1a7/src/akerbp.mlops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-03-27 13:53:30.000000 akerbp.mlops-3.0.1a7/src/akerbp.mlops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-27 13:53:30.000000 akerbp.mlops-3.0.1a7/src/akerbp.mlops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-03-27 13:53:30.000000 akerbp.mlops-3.0.1a7/src/akerbp.mlops.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-03-27 13:53:30.000000 akerbp.mlops-3.0.1a7/src/akerbp.mlops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-03-27 13:53:30.000000 akerbp.mlops-3.0.1a7/src/akerbp.mlops.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.069054 akerbp.mlops-3.0.1a7/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_data_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_install_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_metadata_validation.py
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-27 13:53:30.069054 akerbp.mlops-3.0.1a7/test/test_settings/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_settings/installing_reqs_in_venv.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_settings/multiple_models_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_settings/multiple_models_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_settings/single_model_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_settings/single_model_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_settings/single_model_missing_petrel_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_settings/single_model_no_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_settings/single_model_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3549 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/test/test_version_increment.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-03-27 13:53:07.000000 akerbp.mlops-3.0.1a7/upload_dummy_artifacts.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    49463 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35941 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3510 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/increment_package_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/install.sh
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/mlops_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.397257 akerbp.mlops-3.0.1a8/model_artifact/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/model_artifact/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/model_artifact/dummy.joblib
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.397257 akerbp.mlops-3.0.1a8/model_code/
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/model_code/model.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/model_code/requirements.model
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/model_code/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/promote_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/remove_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.389257 akerbp.mlops-3.0.1a8/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.389257 akerbp.mlops-3.0.1a8/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.397257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.397257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/download_function_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    38633 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.401257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16951 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/logger_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/mappings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6555 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/deploy_prediction_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/deploy_training_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    21689 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/platforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/model_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/model_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22239 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/model_manager/model_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3160 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/training.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.397257 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    49463 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_data_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_install_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_metadata_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/test/test_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/installing_reqs_in_venv.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/multiple_models_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/multiple_models_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/single_model_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/single_model_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/single_model_missing_petrel_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/single_model_no_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/single_model_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3549 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_version_increment.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/upload_dummy_artifacts.py
```

### Comparing `akerbp.mlops-3.0.1a7/.flake8` & `akerbp.mlops-3.0.1a8/.flake8`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/.pre-commit-config.yaml` & `akerbp.mlops-3.0.1a8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/LICENSE` & `akerbp.mlops-3.0.1a8/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/PKG-INFO` & `akerbp.mlops-3.0.1a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.0.1a7
+Version: 3.0.1a8
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.0.1a7/README.md` & `akerbp.mlops-3.0.1a8/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/bitbucket-pipelines.yml` & `akerbp.mlops-3.0.1a8/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/build.sh` & `akerbp.mlops-3.0.1a8/build.sh`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/increment_package_version.py` & `akerbp.mlops-3.0.1a8/increment_package_version.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/mlops_settings.yaml` & `akerbp.mlops-3.0.1a8/mlops_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/model_artifact/dummy.joblib` & `akerbp.mlops-3.0.1a8/model_artifact/dummy.joblib`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/model_code/model.py` & `akerbp.mlops-3.0.1a8/model_code/model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/model_code/test_model.py` & `akerbp.mlops-3.0.1a8/model_code/test_model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/pyproject.toml` & `akerbp.mlops-3.0.1a8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/cdf/handler.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,13 +64,16 @@
             logger.info("Function call metadata obtained")
             logger.info("Writing function call metadata to response")
             output.update(dict(metadata=function_call_metadata))
             logger.info("Function call metadata successfully written to response")
             return output
     except Exception:
         trace = traceback.format_exc()
+        error_message = ""
         try:
             error_message = f"{service_name} service failed.\n{trace}"
             logger.critical(error_message)
         except UnboundLocalError:
+            if not error_message:
+                error_message = "Service failed. \n{trace}"
             pass  # Unable to log error just return error message
         return dict(status="error", error_message=error_message)
```

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/cdf/helpers.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/config.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/exceptions.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/helpers.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/logger.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/logger.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/logger_config.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/logger_config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/core/mappings.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/bitbucket-pipelines.yml` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/deploy.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/helpers.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/platforms.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/platforms.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/deployment/setup.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/setup.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/model_manager/model_manager.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/model_manager/model_manager.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/services/prediction.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/prediction.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/services/test_service.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/test_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         'module' (test_path refers then to modules)
 
     """
     command = [
         sys.executable,
         "-m",
         "pytest",
-        "--quiet",
+        "-s",
         "-o",
         "log_cli=true",
         "--color=no",
         "-W ignore:numpy.ufunc size changed",
     ]
     if path_type == "module":
         command.append("--pyargs")
```

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp/mlops/services/training.py` & `akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/training.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp.mlops.egg-info/PKG-INFO` & `akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.0.1a7
+Version: 3.0.1a8
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.0.1a7/src/akerbp.mlops.egg-info/SOURCES.txt` & `akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_data_validation.py` & `akerbp.mlops-3.0.1a8/test/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_install_requirements.py` & `akerbp.mlops-3.0.1a8/test/test_install_requirements.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_metadata_validation.py` & `akerbp.mlops-3.0.1a8/test/test_metadata_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_settings/installing_reqs_in_venv.yaml` & `akerbp.mlops-3.0.1a8/test/test_settings/installing_reqs_in_venv.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_settings/multiple_models_all_required_fields.yaml` & `akerbp.mlops-3.0.1a8/test/test_settings/multiple_models_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_settings/multiple_models_missing_field.yaml` & `akerbp.mlops-3.0.1a8/test/test_settings/multiple_models_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_settings/single_model_all_required_fields.yaml` & `akerbp.mlops-3.0.1a8/test/test_settings/single_model_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_settings/single_model_missing_field.yaml` & `akerbp.mlops-3.0.1a8/test/test_settings/single_model_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_settings/single_model_missing_petrel_field.yaml` & `akerbp.mlops-3.0.1a8/test/test_settings/single_model_missing_petrel_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_settings/single_model_no_required_input.yaml` & `akerbp.mlops-3.0.1a8/test/test_settings/single_model_no_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_settings/single_model_required_input.yaml` & `akerbp.mlops-3.0.1a8/test/test_settings/single_model_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a7/test/test_version_increment.py` & `akerbp.mlops-3.0.1a8/test/test_version_increment.py`

 * *Files identical despite different names*

