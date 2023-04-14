# Comparing `tmp/ai_transform-0.30.5.tar.gz` & `tmp/ai_transform-0.30.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.30.5.tar", last modified: Thu Apr 13 01:30:40 2023, max compression
+gzip compressed data, was "ai_transform-0.30.6.tar", last modified: Fri Apr 14 03:18:09 2023, max compression
```

## Comparing `ai_transform-0.30.5.tar` & `ai_transform-0.30.6.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.951236 ai_transform-0.30.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-13 01:30:19.000000 ai_transform-0.30.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 01:30:40.951236 ai_transform-0.30.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-13 01:30:19.000000 ai_transform-0.30.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.939236 ai_transform-0.30.5/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.943236 ai_transform-0.30.5/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30029 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.943236 ai_transform-0.30.5/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.943236 ai_transform-0.30.5/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.943236 ai_transform-0.30.5/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.943236 ai_transform-0.30.5/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.947236 ai_transform-0.30.5/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.947236 ai_transform-0.30.5/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-13 01:30:19.000000 ai_transform-0.30.5/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.939236 ai_transform-0.30.5/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 01:30:40.000000 ai_transform-0.30.5/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-13 01:30:40.000000 ai_transform-0.30.5/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 01:30:40.000000 ai_transform-0.30.5/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-13 01:30:40.000000 ai_transform-0.30.5/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 01:30:40.000000 ai_transform-0.30.5/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 01:30:19.000000 ai_transform-0.30.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 01:30:40.951236 ai_transform-0.30.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 01:30:19.000000 ai_transform-0.30.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.947236 ai_transform-0.30.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.947236 ai_transform-0.30.5/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.947236 ai_transform-0.30.5/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.951236 ai_transform-0.30.5/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.951236 ai_transform-0.30.5/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.951236 ai_transform-0.30.5/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:40.951236 ai_transform-0.30.5/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-13 01:30:19.000000 ai_transform-0.30.5/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-14 03:17:41.000000 ai_transform-0.30.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 03:18:09.305138 ai_transform-0.30.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-14 03:17:41.000000 ai_transform-0.30.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.297138 ai_transform-0.30.6/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30029 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.301138 ai_transform-0.30.6/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-14 03:17:41.000000 ai_transform-0.30.6/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.297138 ai_transform-0.30.6/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 03:18:09.000000 ai_transform-0.30.6/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-14 03:18:09.000000 ai_transform-0.30.6/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:18:09.000000 ai_transform-0.30.6/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-14 03:18:09.000000 ai_transform-0.30.6/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 03:18:09.000000 ai_transform-0.30.6/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-14 03:17:41.000000 ai_transform-0.30.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:18:09.305138 ai_transform-0.30.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 03:17:41.000000 ai_transform-0.30.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:18:09.305138 ai_transform-0.30.6/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-14 03:17:41.000000 ai_transform-0.30.6/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.30.5/LICENSE` & `ai_transform-0.30.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/README.md` & `ai_transform-0.30.6/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/__init__.py` & `ai_transform-0.30.6/ai_transform/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.30.5"
+__version__ = "0.30.6"
 
 from ai_transform.timer import Timer
 
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.30.5/ai_transform/api/api.py` & `ai_transform-0.30.6/ai_transform/api/api.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/api/client.py` & `ai_transform-0.30.6/ai_transform/api/client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/api/helpers.py` & `ai_transform-0.30.6/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/components/components.py` & `ai_transform-0.30.6/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/config.py` & `ai_transform-0.30.6/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/dataset/dataset.py` & `ai_transform-0.30.6/ai_transform/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/dataset/field.py` & `ai_transform-0.30.6/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/engine/abstract_engine.py` & `ai_transform-0.30.6/ai_transform/engine/abstract_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,18 @@
 
         if not refresh:
             filters += self._get_refresh_filter(select_fields, dataset)
         filters += self._get_workflow_filter()
 
         self._filters = filters
 
-        self._size = dataset.len(filters=filters) if self._limit_documents is None else self._limit_documents
+        if self.documents:
+            self._size = len(documents)
+        else:
+            self._size = dataset.len(filters=filters) if self._limit_documents is None else self._limit_documents
 
         self._refresh = refresh
         self._after_id = after_id
 
         self._successful_documents = 0
         self._success_ratio = None
```

### Comparing `ai_transform-0.30.5/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.30.6/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.30.6/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/engine/multipass_engine.py` & `ai_transform-0.30.6/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.30.6/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/engine/stable_engine.py` & `ai_transform-0.30.6/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/errors.py` & `ai_transform-0.30.6/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/logger.py` & `ai_transform-0.30.6/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/operator/abstract_operator.py` & `ai_transform-0.30.6/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/operator/dense_operator.py` & `ai_transform-0.30.6/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/timer.py` & `ai_transform-0.30.6/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/types.py` & `ai_transform-0.30.6/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/utils/document.py` & `ai_transform-0.30.6/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/utils/document_list.py` & `ai_transform-0.30.6/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/utils/example_documents.py` & `ai_transform-0.30.6/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/utils/json_encoder.py` & `ai_transform-0.30.6/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/utils/keyphrase.py` & `ai_transform-0.30.6/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.30.6/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/workflow/context_manager.py` & `ai_transform-0.30.6/ai_transform/workflow/context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform/workflow/helpers.py` & `ai_transform-0.30.6/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.30.6/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/setup.py` & `ai_transform-0.30.6/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/conftest.py` & `ai_transform-0.30.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_api/test_client.py` & `ai_transform-0.30.6/tests/core/test_api/test_client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_api/test_endpoints.py` & `ai_transform-0.30.6/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.30.6/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_api/test_wrappers.py` & `ai_transform-0.30.6/tests/core/test_api/test_wrappers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import io
 import sys
+import json
 import requests
 
 from ai_transform.api.wrappers import request_wrapper
 from contextlib import redirect_stdout, redirect_stderr
 
 
 class TestWrappers:
@@ -90,7 +91,77 @@
             )
 
         assert resp.status_code == 200
 
         logs = str(u.getvalue()) + str(f.getvalue())
 
         assert logs.count("Simulated Rate Error") == 2
+
+    def test_request_wrapper_json(self):
+        f = io.StringIO()
+        u = io.StringIO()
+
+        class TestRequest:
+            def __init__(self):
+                self.count = 0
+
+            def __call__(self, *args, **kwargs):
+                if self.count >= 2:
+                    return requests.get(*args, **kwargs)
+                else:
+                    self.count += 1
+                    placeholder = requests.Response()
+                    placeholder.encoding = "utf-8"
+                    placeholder.status_code = 200
+                    placeholder._content = b"\\\\\d"
+                    return placeholder
+
+        with redirect_stdout(f), redirect_stderr(u):
+            resp = request_wrapper(
+                TestRequest(),
+                args=("https://raw.communitydragon.org/latest/cdragon/tft/en_us.json",),
+                num_retries=3,
+                timeout=1,
+                output_to_stdout=True,
+                is_json_decodable=True,
+            )
+
+        assert resp.status_code == 200
+
+        logs = str(u.getvalue()) + str(f.getvalue())
+
+        assert logs.count("Response is not JSON decodable") == 2
+
+    def test_request_wrapper_key_for_error(self):
+        f = io.StringIO()
+        u = io.StringIO()
+
+        class TestRequest:
+            def __init__(self):
+                self.count = 0
+
+            def __call__(self, *args, **kwargs):
+                if self.count >= 2:
+                    return requests.get(*args, **kwargs)
+                else:
+                    self.count += 1
+                    placeholder = requests.Response()
+                    placeholder.encoding = "utf-8"
+                    placeholder.status_code = 200
+                    placeholder._content = json.dumps({"bad_key": False}).encode("utf-8")
+                    return placeholder
+
+        with redirect_stdout(f), redirect_stderr(u):
+            resp = request_wrapper(
+                TestRequest(),
+                ("https://raw.communitydragon.org/latest/cdragon/tft/en_us.json",),
+                num_retries=3,
+                timeout=1,
+                output_to_stdout=True,
+                key_for_error="bad_key",
+            )
+
+        assert resp.status_code == 200
+
+        logs = str(u.getvalue()) + str(f.getvalue())
+
+        assert logs.count("bad_key") == 2
```

### Comparing `ai_transform-0.30.5/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.30.6/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_dataset/test_field.py` & `ai_transform-0.30.6/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.30.6/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.30.6/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_engine/test_engine.py` & `ai_transform-0.30.6/tests/core/test_engine/test_engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from typing import Any
 
+from ai_transform.api.client import Client
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.engine.abstract_engine import AbstractEngine
+from ai_transform.engine.stable_engine import StableEngine
+
+from ai_transform.utils.example_documents import mock_documents
 
 
 class TestAbstractEngine:
     def test_engine(self, full_dataset: Dataset, test_operator: AbstractOperator):
         class ExampleEngine(AbstractEngine):
             def apply(self) -> Any:
 
@@ -34,7 +38,17 @@
     def test_engine_select_fields(self, full_dataset: Dataset, test_operator: AbstractOperator):
         class ExampleEngine(AbstractEngine):
             def apply(self) -> Any:
                 return
 
         engine = ExampleEngine(full_dataset, test_operator, select_fields=["_id", "_chunk_.label"])
         assert "_chunk_" in engine._select_fields
+
+    def test_engine_select_fields(self, test_client: Client, test_dataset_id: str, test_operator: AbstractOperator):
+        engine = StableEngine(
+            test_client.Dataset(test_dataset_id), test_operator, transform_chunksize=2, documents=mock_documents(20)
+        )
+        engine()
+
+        assert len(engine.output_documents) == 20
+
+        test_client.delete_dataset(test_dataset_id)
```

### Comparing `ai_transform-0.30.5/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.30.6/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.30.6/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.30.6/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.30.6/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.30.6/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.30.6/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.5/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.30.6/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

