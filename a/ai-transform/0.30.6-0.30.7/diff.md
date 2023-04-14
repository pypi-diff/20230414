# Comparing `tmp/ai_transform-0.30.6.tar.gz` & `tmp/ai_transform-0.30.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.30.6.tar", last modified: Fri Apr 14 03:18:09 2023, max compression
+gzip compressed data, was "ai_transform-0.30.7.tar", last modified: Fri Apr 14 06:00:49 2023, max compression
```

## Comparing `ai_transform-0.30.6.tar` & `ai_transform-0.30.7.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 03:17:41.000000 ai_transform-0.30.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 03:18:09.305138 ai_transform-0.30.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-14 03:17:41.000000 ai_transform-0.30.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.297138 ai_transform-0.30.6/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30029 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.297138 ai_transform-0.30.6/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 03:18:09.000000 ai_transform-0.30.6/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-14 03:18:09.000000 ai_transform-0.30.6/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:18:09.000000 ai_transform-0.30.6/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-14 03:18:09.000000 ai_transform-0.30.6/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 03:18:09.000000 ai_transform-0.30.6/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-14 03:17:41.000000 ai_transform-0.30.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:18:09.305138 ai_transform-0.30.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 03:17:41.000000 ai_transform-0.30.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.929836 ai_transform-0.30.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 06:00:25.000000 ai_transform-0.30.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 06:00:49.929836 ai_transform-0.30.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-14 06:00:25.000000 ai_transform-0.30.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.917836 ai_transform-0.30.7/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.917836 ai_transform-0.30.7/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30029 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.921836 ai_transform-0.30.7/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.921836 ai_transform-0.30.7/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.921836 ai_transform-0.30.7/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.921836 ai_transform-0.30.7/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.921836 ai_transform-0.30.7/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.925836 ai_transform-0.30.7/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-14 06:00:25.000000 ai_transform-0.30.7/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.917836 ai_transform-0.30.7/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 06:00:49.000000 ai_transform-0.30.7/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-14 06:00:49.000000 ai_transform-0.30.7/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:00:49.000000 ai_transform-0.30.7/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-14 06:00:49.000000 ai_transform-0.30.7/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 06:00:49.000000 ai_transform-0.30.7/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-14 06:00:25.000000 ai_transform-0.30.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:00:49.929836 ai_transform-0.30.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 06:00:25.000000 ai_transform-0.30.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.925836 ai_transform-0.30.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.925836 ai_transform-0.30.7/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.925836 ai_transform-0.30.7/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.925836 ai_transform-0.30.7/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.929836 ai_transform-0.30.7/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.929836 ai_transform-0.30.7/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:49.929836 ai_transform-0.30.7/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-14 06:00:25.000000 ai_transform-0.30.7/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.30.6/LICENSE` & `ai_transform-0.30.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/README.md` & `ai_transform-0.30.7/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/__init__.py` & `ai_transform-0.30.7/ai_transform/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.30.6"
+__version__ = "0.30.7"
 
 from ai_transform.timer import Timer
 
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.30.6/ai_transform/api/api.py` & `ai_transform-0.30.7/ai_transform/api/api.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/api/client.py` & `ai_transform-0.30.7/ai_transform/api/client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/api/helpers.py` & `ai_transform-0.30.7/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/api/wrappers.py` & `ai_transform-0.30.7/ai_transform/api/wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,33 +8,37 @@
 
 from typing import Union, Sequence, Mapping, Callable, Any
 
 logger = logging.getLogger(__file__)
 logging.basicConfig()
 
 
-class ManualRetry(Exception):
+class ManualRetryError(Exception):
+    pass
+
+
+class ResultNotOKError(Exception):
     pass
 
 
 def is_response_bad(
     result: Response,
     key_for_error: str = None,
     output_to_stdout: bool = False,  # support output to stdout to ensure logging is working
 ):
     try:
         json_response = result.json()
         if key_for_error in json_response:
             raise KeyError
 
-    except JSONDecodeError:
+    except JSONDecodeError as e:
         error_message = "Response is not JSON decodable"
         if output_to_stdout:
             print(error_message)
-        raise JSONDecodeError(error_message)
+        raise JSONDecodeError(e.msg, e.doc, e.pos)
 
     except KeyError:
         error_message = f"{key_for_error} not in JSON response"
         if output_to_stdout:
             print(error_message)
         raise KeyError(error_message)
 
@@ -67,25 +71,25 @@
         try:
             result = fn(*args, **kwargs)
 
             if not result.ok:
                 to_log = format_logging_info({"message": result.content.decode(), "status_code": result.status_code})
                 if output_to_stdout:
                     print(to_log)
-                raise ValueError(to_log)
+                raise ResultNotOKError(to_log)
 
             if retry_func(result):
                 to_log_for_retry = "Manual Retry Triggered..."
                 if output_to_stdout:
                     print(to_log_for_retry)
-                raise ManualRetry(to_log_for_retry)
+                raise ManualRetryError(to_log_for_retry)
 
             if is_json_decodable or key_for_error:
                 is_response_bad(result=result, key_for_error=key_for_error, output_to_stdout=output_to_stdout)
 
-        except (Exception, ManualRetry, JSONDecodeError, KeyError) as e:
+        except (ResultNotOKError, ManualRetryError, JSONDecodeError, KeyError) as e:
             logger.exception(e)
             time.sleep(timeout * exponential_backoff**n)
         else:
             return result
 
     return result
```

### Comparing `ai_transform-0.30.6/ai_transform/components/components.py` & `ai_transform-0.30.7/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/config.py` & `ai_transform-0.30.7/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/dataset/dataset.py` & `ai_transform-0.30.7/ai_transform/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/dataset/field.py` & `ai_transform-0.30.7/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/engine/abstract_engine.py` & `ai_transform-0.30.7/ai_transform/engine/abstract_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.30.7/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.30.7/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/engine/multipass_engine.py` & `ai_transform-0.30.7/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.30.7/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/engine/stable_engine.py` & `ai_transform-0.30.7/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/errors.py` & `ai_transform-0.30.7/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/logger.py` & `ai_transform-0.30.7/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/operator/abstract_operator.py` & `ai_transform-0.30.7/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/operator/dense_operator.py` & `ai_transform-0.30.7/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/timer.py` & `ai_transform-0.30.7/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/types.py` & `ai_transform-0.30.7/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/utils/document.py` & `ai_transform-0.30.7/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/utils/document_list.py` & `ai_transform-0.30.7/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/utils/example_documents.py` & `ai_transform-0.30.7/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/utils/json_encoder.py` & `ai_transform-0.30.7/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/utils/keyphrase.py` & `ai_transform-0.30.7/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.30.7/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/workflow/context_manager.py` & `ai_transform-0.30.7/ai_transform/workflow/context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform/workflow/helpers.py` & `ai_transform-0.30.7/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.30.7/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/setup.py` & `ai_transform-0.30.7/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/conftest.py` & `ai_transform-0.30.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_api/test_client.py` & `ai_transform-0.30.7/tests/core/test_api/test_client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_api/test_endpoints.py` & `ai_transform-0.30.7/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.30.7/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_api/test_wrappers.py` & `ai_transform-0.30.7/tests/core/test_api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.30.7/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_dataset/test_field.py` & `ai_transform-0.30.7/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.30.7/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.30.7/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_engine/test_engine.py` & `ai_transform-0.30.7/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.30.7/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.30.7/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.30.7/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.30.7/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.30.7/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.30.7/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.6/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.30.7/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

