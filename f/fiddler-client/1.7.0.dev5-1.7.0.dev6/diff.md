# Comparing `tmp/fiddler-client-1.7.0.dev5.tar.gz` & `tmp/fiddler-client-1.7.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-1.7.0.dev5.tar", last modified: Tue Mar 28 11:20:01 2023, max compression
+gzip compressed data, was "fiddler-client-1.7.0.dev6.tar", last modified: Fri Apr 14 09:26:42 2023, max compression
```

## Comparing `fiddler-client-1.7.0.dev5.tar` & `fiddler-client-1.7.0.dev6.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.380397 fiddler-client-1.7.0.dev5/
--rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1000) docker    (1001)    18175 2023-03-28 11:20:01.380397 fiddler-client-1.7.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)    14843 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/PUBLIC.md
--rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/README.md
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.372397 fiddler-client-1.7.0.dev5/fiddler/
--rw-r--r--   0 runner    (1000) docker    (1001)    32528 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/_version.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.372397 fiddler-client-1.7.0.dev5/fiddler/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    11453 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/api/monitoring.py
--rw-r--r--   0 runner    (1000) docker    (1001)    12356 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/api/publish_event.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.372397 fiddler-client-1.7.0.dev5/fiddler/assets/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/assets/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/assets/pg_reserved_words.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6393 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/aws_utils.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5098 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/client.py
--rw-r--r--   0 runner    (1000) docker    (1001)    21425 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/connection.py
--rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/constants.py
--rw-r--r--   0 runner    (1000) docker    (1001)   131942 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/core_objects.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)    16945 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/experimental.py
--rw-r--r--   0 runner    (1000) docker    (1001)    81387 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/fiddler_api.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.372397 fiddler-client-1.7.0.dev5/fiddler/file_processor/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.376397 fiddler-client-1.7.0.dev5/fiddler/file_processor/src/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/src/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2024 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/src/constants.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2193 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/src/extractor.py
--rw-r--r--   0 runner    (1000) docker    (1001)      537 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/src/facade.py
--rw-r--r--   0 runner    (1000) docker    (1001)      557 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/src/file_workflow_executor.py
--rw-r--r--   0 runner    (1000) docker    (1001)    11629 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/src/processor.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1754 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/src/utils.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.376397 fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.376397 fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/resources/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/resources/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.376397 fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/resources/csvs/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/resources/csvs/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2495 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/test_extractor.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2098 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/test_facade.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5389 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/test_file_processor.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.376397 fiddler-client-1.7.0.dev5/fiddler/libs/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4188 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1000) docker    (1001)    15196 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     6387 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/model_info_validator.py
--rw-r--r--   0 runner    (1000) docker    (1001)    17870 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/monitoring_validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.376397 fiddler-client-1.7.0.dev5/fiddler/packtools/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/packtools/template_model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4515 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/project.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.376397 fiddler-client-1.7.0.dev5/fiddler/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)     4352 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3208 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/utils/formatting.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/utils/general_checks.py
--rw-r--r--   0 runner    (1000) docker    (1001)      775 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/utils/helper.py
--rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/utils/logging.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5806 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/utils/pandas.py
--rw-r--r--   0 runner    (1000) docker    (1001)    18586 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v1_v2_compat.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.376397 fiddler-client-1.7.0.dev5/fiddler/v2/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/__init__.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.376397 fiddler-client-1.7.0.dev5/fiddler/v2/api/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14039 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/alert_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1892 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/api.py
--rw-r--r--   0 runner    (1000) docker    (1001)     5923 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/baseline_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    11539 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/dataset_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14751 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/events_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13480 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/explainability_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4371 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4472 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/job_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/model_artifact_deploy.py
--rw-r--r--   0 runner    (1000) docker    (1001)     3105 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/model_deployment_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)    14391 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/model_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2664 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/api/project_mixin.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1125 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/constants.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.376397 fiddler-client-1.7.0.dev5/fiddler/v2/schema/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4530 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/alert.py
--rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/base.py
--rw-r--r--   0 runner    (1000) docker    (1001)      462 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/baseline.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2533 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/common.py
--rw-r--r--   0 runner    (1000) docker    (1001)      640 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/dataset.py
--rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/events.py
--rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/job.py
--rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/model.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1085 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/model_deployment.py
--rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/project.py
--rw-r--r--   0 runner    (1000) docker    (1001)      359 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/server_info.py
--rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/schema/user.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.380397 fiddler-client-1.7.0.dev5/fiddler/v2/utils/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/utils/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1237 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/utils/decorators.py
--rw-r--r--   0 runner    (1000) docker    (1001)     4127 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/utils/exceptions.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1600 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/utils/helpers.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2004 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/utils/response_handler.py
--rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/utils/validations.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.380397 fiddler-client-1.7.0.dev5/fiddler/v2/validators/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/validators/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     1527 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/v2/validators/dataset_validator.py
--rw-r--r--   0 runner    (1000) docker    (1001)    13965 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/fiddler/validator.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.380397 fiddler-client-1.7.0.dev5/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1000) docker    (1001)    18175 2023-03-28 11:20:01.000000 fiddler-client-1.7.0.dev5/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) docker    (1001)     2901 2023-03-28 11:20:01.000000 fiddler-client-1.7.0.dev5/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-03-28 11:20:01.000000 fiddler-client-1.7.0.dev5/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) docker    (1001)      227 2023-03-28 11:20:01.000000 fiddler-client-1.7.0.dev5/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-03-28 11:20:01.000000 fiddler-client-1.7.0.dev5/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-03-28 11:20:01.380397 fiddler-client-1.7.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1000) docker    (1001)     1432 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/setup.py
-drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-03-28 11:20:01.380397 fiddler-client-1.7.0.dev5/tests/
--rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1000) docker    (1001)     2132 2023-03-28 11:19:56.000000 fiddler-client-1.7.0.dev5/tests/test_fiddler_api.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.014686 fiddler-client-1.7.0.dev6/
+-rw-r--r--   0 runner    (1000) docker    (1001)       18 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1000) docker    (1001)    18175 2023-04-14 09:26:42.014686 fiddler-client-1.7.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)    14843 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/PUBLIC.md
+-rw-r--r--   0 runner    (1000) docker    (1001)     2018 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/README.md
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.006686 fiddler-client-1.7.0.dev6/fiddler/
+-rw-r--r--   0 runner    (1000) docker    (1001)    32528 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)       27 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/_version.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    11453 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/api/monitoring.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    12356 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/api/publish_event.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/assets/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/assets/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8200 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/assets/pg_reserved_words.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6393 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/aws_utils.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5098 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/client.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    21425 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/connection.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      354 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/constants.py
+-rw-r--r--   0 runner    (1000) docker    (1001)   131942 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/core_objects.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4721 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    16945 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/experimental.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    81387 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/fiddler_api.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/file_processor/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/file_processor/src/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/src/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2024 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/src/constants.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2193 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/src/extractor.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      537 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/src/facade.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      557 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/src/file_workflow_executor.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    11629 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/src/processor.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1754 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/src/utils.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/resources/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/resources/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/resources/csvs/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/resources/csvs/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2495 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/test_extractor.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2098 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/test_facade.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5389 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/test_file_processor.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/libs/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4188 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    15196 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     6387 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/model_info_validator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    17870 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/monitoring_validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/packtools/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4167 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     7442 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14619 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     9500 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/packtools/template_model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4515 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/project.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)     4352 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1006 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3208 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/utils/formatting.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3084 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/utils/general_checks.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      775 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/utils/helper.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      188 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/utils/logging.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5806 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/utils/pandas.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    18586 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v1_v2_compat.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/v2/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/__init__.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.010686 fiddler-client-1.7.0.dev6/fiddler/v2/api/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14039 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/alert_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1892 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/api.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     5923 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/baseline_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    11539 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/dataset_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14751 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/events_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13480 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/explainability_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4371 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4472 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/job_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     8265 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/model_artifact_deploy.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     3105 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/model_deployment_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    14391 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/model_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2664 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/api/project_mixin.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1125 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/constants.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.014686 fiddler-client-1.7.0.dev6/fiddler/v2/schema/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4530 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/alert.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      346 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/base.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      462 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/baseline.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2533 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/common.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      640 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/dataset.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      885 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/events.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      157 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/job.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      453 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/model.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1085 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/model_deployment.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      124 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/project.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      359 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/server_info.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      109 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/schema/user.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.014686 fiddler-client-1.7.0.dev6/fiddler/v2/utils/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/utils/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1237 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/utils/decorators.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     4127 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/utils/exceptions.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1600 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/utils/helpers.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2004 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/utils/response_handler.py
+-rw-r--r--   0 runner    (1000) docker    (1001)      362 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/utils/validations.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.014686 fiddler-client-1.7.0.dev6/fiddler/v2/validators/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/validators/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     1527 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/v2/validators/dataset_validator.py
+-rw-r--r--   0 runner    (1000) docker    (1001)    13965 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/fiddler/validator.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.014686 fiddler-client-1.7.0.dev6/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1000) docker    (1001)    18175 2023-04-14 09:26:41.000000 fiddler-client-1.7.0.dev6/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) docker    (1001)     2901 2023-04-14 09:26:41.000000 fiddler-client-1.7.0.dev6/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)        1 2023-04-14 09:26:41.000000 fiddler-client-1.7.0.dev6/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)      226 2023-04-14 09:26:41.000000 fiddler-client-1.7.0.dev6/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       14 2023-04-14 09:26:41.000000 fiddler-client-1.7.0.dev6/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) docker    (1001)       38 2023-04-14 09:26:42.014686 fiddler-client-1.7.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1000) docker    (1001)     1420 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/setup.py
+drwxr-sr-x   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:42.014686 fiddler-client-1.7.0.dev6/tests/
+-rw-r--r--   0 runner    (1000) docker    (1001)        0 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1000) docker    (1001)     2132 2023-04-14 09:26:36.000000 fiddler-client-1.7.0.dev6/tests/test_fiddler_api.py
```

### Comparing `fiddler-client-1.7.0.dev5/PKG-INFO` & `fiddler-client-1.7.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 1.7.0.dev5
+Version: 1.7.0.dev6
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
```

### Comparing `fiddler-client-1.7.0.dev5/PUBLIC.md` & `fiddler-client-1.7.0.dev6/PUBLIC.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/README.md` & `fiddler-client-1.7.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/__init__.py` & `fiddler-client-1.7.0.dev6/fiddler/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/api/monitoring.py` & `fiddler-client-1.7.0.dev6/fiddler/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/api/publish_event.py` & `fiddler-client-1.7.0.dev6/fiddler/api/publish_event.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/assets/pg_reserved_words.py` & `fiddler-client-1.7.0.dev6/fiddler/assets/pg_reserved_words.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/aws_utils.py` & `fiddler-client-1.7.0.dev6/fiddler/aws_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/client.py` & `fiddler-client-1.7.0.dev6/fiddler/client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/connection.py` & `fiddler-client-1.7.0.dev6/fiddler/connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/core_objects.py` & `fiddler-client-1.7.0.dev6/fiddler/core_objects.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/dataset.py` & `fiddler-client-1.7.0.dev6/fiddler/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/experimental.py` & `fiddler-client-1.7.0.dev6/fiddler/experimental.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/fiddler_api.py` & `fiddler-client-1.7.0.dev6/fiddler/fiddler_api.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/file_processor/src/constants.py` & `fiddler-client-1.7.0.dev6/fiddler/file_processor/src/constants.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/file_processor/src/extractor.py` & `fiddler-client-1.7.0.dev6/fiddler/file_processor/src/extractor.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/file_processor/src/facade.py` & `fiddler-client-1.7.0.dev6/fiddler/file_processor/src/facade.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/file_processor/src/file_workflow_executor.py` & `fiddler-client-1.7.0.dev6/fiddler/file_processor/src/file_workflow_executor.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/file_processor/src/processor.py` & `fiddler-client-1.7.0.dev6/fiddler/file_processor/src/processor.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/file_processor/src/utils.py` & `fiddler-client-1.7.0.dev6/fiddler/file_processor/src/utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/test_extractor.py` & `fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/test_facade.py` & `fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/test_facade.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/file_processor/tests/test_file_processor.py` & `fiddler-client-1.7.0.dev6/fiddler/file_processor/tests/test_file_processor.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/libs/http_client.py` & `fiddler-client-1.7.0.dev6/fiddler/libs/http_client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/model.py` & `fiddler-client-1.7.0.dev6/fiddler/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/model_info_validator.py` & `fiddler-client-1.7.0.dev6/fiddler/model_info_validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/monitoring_validator.py` & `fiddler-client-1.7.0.dev6/fiddler/monitoring_validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/packtools/gem.py` & `fiddler-client-1.7.0.dev6/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-1.7.0.dev6/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-1.7.0.dev6/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/packtools/template_model.py` & `fiddler-client-1.7.0.dev6/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/project.py` & `fiddler-client-1.7.0.dev6/fiddler/project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/utils/__init__.py` & `fiddler-client-1.7.0.dev6/fiddler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/utils/exceptions.py` & `fiddler-client-1.7.0.dev6/fiddler/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/utils/formatting.py` & `fiddler-client-1.7.0.dev6/fiddler/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/utils/general_checks.py` & `fiddler-client-1.7.0.dev6/fiddler/utils/general_checks.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/utils/helper.py` & `fiddler-client-1.7.0.dev6/fiddler/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/utils/pandas.py` & `fiddler-client-1.7.0.dev6/fiddler/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v1_v2_compat.py` & `fiddler-client-1.7.0.dev6/fiddler/v1_v2_compat.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/alert_mixin.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/alert_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/api.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/api.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/baseline_mixin.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/baseline_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/dataset_mixin.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/events_mixin.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/events_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/explainability_mixin.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/explainability_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/helpers.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/job_mixin.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/job_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/model_artifact_deploy.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/model_artifact_deploy.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/model_deployment_mixin.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/model_deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/model_mixin.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/model_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/api/project_mixin.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/api/project_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/constants.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/constants.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/schema/alert.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/schema/alert.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/schema/common.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/schema/common.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/schema/dataset.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/schema/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/schema/events.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/schema/events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/schema/model_deployment.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/schema/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/utils/decorators.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/utils/exceptions.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/utils/helpers.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/utils/response_handler.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/utils/response_handler.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/v2/validators/dataset_validator.py` & `fiddler-client-1.7.0.dev6/fiddler/v2/validators/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler/validator.py` & `fiddler-client-1.7.0.dev6/fiddler/validator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-1.7.0.dev6/fiddler_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 1.7.0.dev5
+Version: 1.7.0.dev6
 Summary: Python client for Fiddler Service
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 License: UNKNOWN
 Description: Fiddler Client
         =============
```

### Comparing `fiddler-client-1.7.0.dev5/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-1.7.0.dev6/fiddler_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-1.7.0.dev5/setup.py` & `fiddler-client-1.7.0.dev6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,20 +25,19 @@
     long_description_content_type='text/markdown',
     url='https://fiddler.ai',
     packages=setuptools.find_packages(),
     install_requires=[
         'pip>=21.0',
         'requests<3',
         'requests-toolbelt',
-        'pandas>=1.2.5',
+        'pandas>=1.2.5,<=1.5.3',
         'pyyaml',
         'packaging',
         'deepdiff',
         'boto3',
-        'botocore',
         'fastavro',
         'importlib-resources',
         'Werkzeug',
         'pyarrow>=3.0.0',
         'deprecation==2.1.0',
         'pydantic>=1.9.0',
         'deprecated==1.2.13',
```

### Comparing `fiddler-client-1.7.0.dev5/tests/test_fiddler_api.py` & `fiddler-client-1.7.0.dev6/tests/test_fiddler_api.py`

 * *Files identical despite different names*

