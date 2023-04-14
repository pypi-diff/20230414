# Comparing `tmp/deeploy-0.5.1.tar.gz` & `tmp/deeploy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeploy-0.5.1.tar", last modified: Tue Aug 16 12:30:22 2022, max compression
+gzip compressed data, was "deeploy-1.0.0.tar", last modified: Fri Apr 14 08:57:54 2023, max compression
```

## Comparing `deeploy-0.5.1.tar` & `deeploy-1.0.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.518452 deeploy-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2022-08-16 12:30:20.000000 deeploy-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      911 2022-08-16 12:30:22.518452 deeploy-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1014 2022-08-16 12:30:20.000000 deeploy-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.510452 deeploy-0.5.1/deeploy/
--rw-rw-rw-   0 root         (0) root         (0)      200 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.514452 deeploy-0.5.1/deeploy/common/
--rw-rw-rw-   0 root         (0) root         (0)       62 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.514452 deeploy-0.5.1/deeploy/common/constants/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/common/constants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      601 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/common/constants/pytorch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.514452 deeploy-0.5.1/deeploy/common/functions/
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/common/functions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/common/functions/functions.py
--rw-rw-rw-   0 root         (0) root         (0)    33808 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/deeploy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.514452 deeploy-0.5.1/deeploy/enums/
--rw-rw-rw-   0 root         (0) root         (0)      186 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       86 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/enums/auth_type.py
--rw-rw-rw-   0 root         (0) root         (0)      231 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/enums/explainer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/enums/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/enums/prediction_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.514452 deeploy-0.5.1/deeploy/models/
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/client_options.py
--rw-rw-rw-   0 root         (0) root         (0)     2372 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/create_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/create_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3622 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/deploy_options.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/deployment.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/model_reference_json.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/prediction_log.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/prediction_logs.py
--rw-rw-rw-   0 root         (0) root         (0)      381 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/repository.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/update_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     3619 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/update_options.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/models/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.514452 deeploy-0.5.1/deeploy/services/
--rw-rw-rw-   0 root         (0) root         (0)      196 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13583 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/deeploy_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2594 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/explainer_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.514452 deeploy-0.5.1/deeploy/services/explainers/
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/explainers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/explainers/alibi.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/explainers/base_explainer.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/explainers/shap.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/git_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3324 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/model_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.518452 deeploy-0.5.1/deeploy/services/models/
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/models/base_model.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/models/onnx.py
--rw-rw-rw-   0 root         (0) root         (0)     3026 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/models/pytorch.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/models/sklearn.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/models/tensorflow.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/models/triton.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2022-08-16 12:30:20.000000 deeploy-0.5.1/deeploy/services/models/xgboost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.514452 deeploy-0.5.1/deeploy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      911 2022-08-16 12:30:22.000000 deeploy-0.5.1/deeploy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1647 2022-08-16 12:30:22.000000 deeploy-0.5.1/deeploy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-16 12:30:22.000000 deeploy-0.5.1/deeploy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      138 2022-08-16 12:30:22.000000 deeploy-0.5.1/deeploy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-08-16 12:30:22.000000 deeploy-0.5.1/deeploy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-16 12:30:22.518452 deeploy-0.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1434 2022-08-16 12:30:20.000000 deeploy-0.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-16 12:30:22.518452 deeploy-0.5.1/test/
--rw-rw-rw-   0 root         (0) root         (0)       43 2022-08-16 12:30:20.000000 deeploy-0.5.1/test/test_deeploy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.074632 deeploy-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-04-14 08:57:52.000000 deeploy-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      911 2023-04-14 08:57:54.074632 deeploy-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2023-04-14 08:57:52.000000 deeploy-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.070632 deeploy-1.0.0/deeploy/
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.070632 deeploy-1.0.0/deeploy/common/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.070632 deeploy-1.0.0/deeploy/common/constants/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/common/constants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/common/constants/pytorch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.070632 deeploy-1.0.0/deeploy/common/functions/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/common/functions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/common/functions/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    35963 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/deeploy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.070632 deeploy-1.0.0/deeploy/enums/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/enums/auth_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/enums/explainer_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/enums/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/enums/prediction_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.070632 deeploy-1.0.0/deeploy/models/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/client_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2323 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/create_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/create_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     3616 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/deploy_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/model_reference_json.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/prediction_log.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/update_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/update_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/models/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.074632 deeploy-1.0.0/deeploy/services/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14158 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/deeploy_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4599 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/explainer_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.074632 deeploy-1.0.0/deeploy/services/explainers/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/explainers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/explainers/alibi.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/explainers/base_explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/explainers/omni_tabular.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/explainers/shap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/git_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3409 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/model_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.074632 deeploy-1.0.0/deeploy/services/models/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/models/base_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/models/onnx.py
+-rw-rw-rw-   0 root         (0) root         (0)     3167 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/models/pytorch.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/models/sklearn.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/models/tensorflow.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/models/triton.py
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-14 08:57:52.000000 deeploy-1.0.0/deeploy/services/models/xgboost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.070632 deeploy-1.0.0/deeploy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-04-14 08:57:54.000000 deeploy-1.0.0/deeploy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-04-14 08:57:54.000000 deeploy-1.0.0/deeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 08:57:54.000000 deeploy-1.0.0/deeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2023-04-14 08:57:54.000000 deeploy-1.0.0/deeploy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-14 08:57:54.000000 deeploy-1.0.0/deeploy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 08:57:54.074632 deeploy-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-04-14 08:57:52.000000 deeploy-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:57:54.074632 deeploy-1.0.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-14 08:57:52.000000 deeploy-1.0.0/test/test_deeploy.py
```

### Comparing `deeploy-0.5.1/LICENSE` & `deeploy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deeploy-0.5.1/PKG-INFO` & `deeploy-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeploy
-Version: 0.5.1
+Version: 1.0.0
 Summary: The official Deeploy client for Python
 Home-page: https://gitlab.com/deeploy-ml/deeploy-python-client
 Author: Tim Kleinloog
 Author-email: opensource@deeploy.ml
 License: UNKNOWN
 Project-URL: Documentation, https://deeploy-ml.gitlab.io/deeploy-python-client/
 Project-URL: Deeploy website, https://deeploy.ml
```

### Comparing `deeploy-0.5.1/README.md` & `deeploy-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `deeploy-0.5.1/deeploy/common/constants/pytorch.py` & `deeploy-1.0.0/deeploy/common/constants/pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 number_of_netty_threads=4
 job_queue_size=10
 enable_envvars_config=true
 install_py_dep_per_model=true
 model_store=/mnt/models/model-store
 model_snapshot={"name":"startup.cfg","modelCount":1,"models":{"model":{"1.0":{"defaultVersion":true,"marName":"model.mar","minWorkers":1,"maxWorkers":5,"batchSize":1,"maxBatchDelay":5000,"responseTimeout":120}}}}
 
-""" # noqa
+"""  # noqa
```

### Comparing `deeploy-0.5.1/deeploy/common/functions/functions.py` & `deeploy-1.0.0/deeploy/common/functions/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os
 import shutil
 import logging
 
 
 def to_lower_camel(string: str) -> str:
-    if string == 'public_url':
-        return 'publicURL'
+    if string == "public_url":
+        return "publicURL"
 
-    camel_case = ''.join(word.capitalize() for word in string.split('_'))
+    camel_case = "".join(word.capitalize() for word in string.split("_"))
     lower_camel_case = camel_case[0].lower() + camel_case[1:]
     return lower_camel_case
 
 
 def delete_all_contents_in_directory(folder_path: str) -> None:
     for filename in os.listdir(folder_path):
         file_path = os.path.join(folder_path, filename)
         try:
             if os.path.isfile(file_path) or os.path.islink(file_path):
                 os.unlink(file_path)
             elif os.path.isdir(file_path):
                 shutil.rmtree(file_path)
         except Exception as e:
-            logging.error('Failed to delete %s. Reason: %s' % (file_path, e))
+            logging.error("Failed to delete %s. Reason: %s" % (file_path, e))
     return
 
 
 def directory_exists(folder_path: str) -> bool:
     return os.path.exists(folder_path)
```

### Comparing `deeploy-0.5.1/deeploy/deeploy.py` & `deeploy-1.0.0/deeploy/deeploy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,106 @@
 import logging
-from typing import Any, Tuple
+from typing import Any, List, Tuple
 import os
 import shutil
 import uuid
 import json
+from deeploy.models.prediction_log import RequestLog
 
 
 from pydantic import parse_obj_as
 from git import Repo
 from deeploy.models.model_reference_json import BlobReference, DockerReference
 
 from deeploy.services import DeeployService, GitService, ModelWrapper, ExplainerWrapper
-from deeploy.models import ClientConfig, Deployment, CreateDeployment, UpdateDeployment, \
-    DeployOptions, UpdateOptions, V1Prediction, V2Prediction, ModelReferenceJson, \
-    PredictionLog, RequestLogs, PredictionLogs, UpdateDeploymentMetadata
+from deeploy.models import (
+    ClientConfig,
+    Deployment,
+    CreateDeployment,
+    UpdateDeployment,
+    DeployOptions,
+    UpdateOptions,
+    V1Prediction,
+    V2Prediction,
+    ModelReferenceJson,
+    PredictionLog,
+    UpdateDeploymentMetadata,
+)
 from deeploy.enums import ExplainerType, ModelType
-from deeploy.common.functions import delete_all_contents_in_directory, directory_exists, \
-    directory_empty, file_exists
+from deeploy.common.functions import (
+    delete_all_contents_in_directory,
+    directory_exists,
+    directory_empty,
+    file_exists,
+)
 
 
 class Client(object):
     """
     A class for interacting with Deeploy
     """
 
     __config: ClientConfig
 
     def __init__(
-            self, host: str, workspace_id: str, access_key: str = None, secret_key: str = None,
-            deployment_token: str = None, branch_name: str = None) -> None:
+        self,
+        host: str,
+        workspace_id: str,
+        access_key: str = None,
+        secret_key: str = None,
+        deployment_token: str = None,
+        branch_name: str = None,
+    ) -> None:
         """Initialise the Deeploy client
         Parameters:
             host (str): The host at which Deeploy is located, i.e. deeploy.example.com
             workspace_id (str): The ID of the workspace in which your repository
                 is located
             access_key (str): Personal Access Key generated from the Deeploy UI
             secret_key (str): Secret Access Key generated from the Deeploy UI
             token (str): Deployment token generated from the Deeploy UI
             branch_name (str, optional): The banchname on which to commit new models.
                 Defaults to the current branchname.
         """
 
-        self.__config = ClientConfig(**{
-            'access_key': access_key,
-            'secret_key': secret_key,
-            'token': deployment_token,
-            'host': host,
-            'workspace_id': workspace_id,
-            'branch_name': branch_name,
-            'repository_id': '',
-        })
+        self.__config = ClientConfig(
+            **{
+                "access_key": access_key,
+                "secret_key": secret_key,
+                "token": deployment_token,
+                "host": host,
+                "workspace_id": workspace_id,
+                "branch_name": branch_name,
+                "repository_id": "",
+            }
+        )
 
         self.__deeploy_service = DeeployService(
             host,
             workspace_id,
             access_key,
             secret_key,
             deployment_token,
         )
 
         return
 
-    def deploy(self, options: DeployOptions, local_repository_path: str,
-               model: Any = None, explainer: Any = None, model_type: int = None,
-               explainer_type: int = None, overwrite_contract: bool = False,
-               overwrite_metadata: bool = False, commit_message: str = None,
-               contract_path: str = "") -> Deployment:
+    def deploy(
+        self,
+        options: DeployOptions,
+        local_repository_path: str,
+        model: Any = None,
+        explainer: Any = None,
+        model_type: int = None,
+        explainer_type: int = None,
+        overwrite_contract: bool = False,
+        overwrite_metadata: bool = False,
+        commit_message: str = None,
+        contract_path: str = "",
+    ) -> Deployment:
         """Deploy a model on Deeploy
         Parameters:
             model (Any): The class instance of an ML model
             options (DeployOptions): An instance of the deploy options class
                 containing the deployment options
             local_repository_path (str): Absolute path to the local git repository
                 which is connected to Deeploy
@@ -83,167 +114,214 @@
             commit_message (str, optional): Commit message to use
             contract_path (str, optional): Relative repository subpath that contains the
                 Deeploy contract to deploy from
         """
         commit = False
 
         if not (self.__config.access_key and self.__config.secret_key):
-            raise Exception('Missing access credentials to create deployment.')
+            raise Exception("Missing access credentials to create deployment.")
 
         git_service = GitService(local_repository_path)
 
-        repository_in_workspace, repository_id = self.__is_git_repository_in_workspace(git_service)
+        repository_in_workspace, repository_id = self.__is_git_repository_in_workspace(
+            git_service
+        )
 
         if not repository_in_workspace:
             raise Exception(
-                'Repository was not found in the Deeploy workspace. \
-                 Make sure you have connected it before.')
+                "Repository was not found in the Deeploy workspace. \
+                 Make sure you have connected it before."
+            )
         else:
             self.__config.repository_id = repository_id
 
-        logging.info('Pulling from the remote repository...')
+        logging.info("Pulling from the remote repository...")
         git_service.pull()
-        logging.info('Successfully pulled from the remote repository.')
+        logging.info("Successfully pulled from the remote repository.")
 
         if model:
             model_type = self.__process_model(
-                model, options, local_repository_path, git_service, overwrite_contract,
-                contract_path).value
+                model,
+                options,
+                local_repository_path,
+                git_service,
+                overwrite_contract,
+                contract_path,
+            ).value
             commit = True
         elif options.model_docker_config or options.model_blob_config:
             self.__prepare_model_directory(
-                git_service, local_repository_path, contract_path, overwrite_contract)
-            model_folder = os.path.join(
-                local_repository_path, contract_path, 'model')
+                git_service, local_repository_path, contract_path, overwrite_contract
+            )
+            model_folder = os.path.join(local_repository_path, contract_path, "model")
             shutil.rmtree(model_folder)
             os.mkdir(model_folder)
             if options.model_docker_config:
                 model_type = ModelType.CUSTOM.value
                 self.__create_reference_file(
-                    model_folder, dockerReference=options.model_docker_config)
+                    model_folder, dockerReference=options.model_docker_config
+                )
             elif options.model_blob_config:
                 model_type = model_type
                 self.__create_reference_file(
-                    model_folder, blobReference=options.model_blob_config)
-            git_service.add_folder_to_staging(os.path.join(contract_path, 'model'))
+                    model_folder, blobReference=options.model_blob_config
+                )
+            git_service.add_folder_to_staging(os.path.join(contract_path, "model"))
             commit = True
         else:
             reference_path = os.path.join(
-                local_repository_path, contract_path, 'model', 'reference.json')
+                local_repository_path, contract_path, "model", "reference.json"
+            )
             if not os.path.exists(reference_path):
-                raise Exception('Missing model reference file in repository.')
+                raise Exception("Missing model reference file in repository.")
 
             try:
                 with open(reference_path) as referenceFile:
                     data = json.load(referenceFile)
-                    if 'reference' in data:
-                        if "blob" in data['reference']:
+                    if "reference" in data:
+                        if "blob" in data["reference"]:
                             model_type = model_type
-                        elif "docker" in data['reference']:
+                        elif "docker" in data["reference"]:
                             model_type = ModelType.CUSTOM.value
                         else:
-                            raise Exception('No information on to be deployed model available.')
+                            raise Exception(
+                                "No information on to be deployed model available."
+                            )
                     else:
-                        raise Exception('No information on to be deployed model available.')
+                        raise Exception(
+                            "No information on to be deployed model available."
+                        )
             except IOError:
-                raise Exception('Failed to deploy model from reference.json file.')
+                raise Exception("Failed to deploy model from reference.json file.")
 
-        commit_message = '[Deeploy Client] Add new model' if not commit_message else commit_message
+        commit_message = (
+            "[Deeploy Client] Add new model" if not commit_message else commit_message
+        )
 
         if explainer:
             explainer_type = self.__process_explainer(
-                explainer, local_repository_path, git_service, overwrite_contract,
-                contract_path)
-            commit_message += ' and explainer' if not commit_message else ''
+                explainer,
+                git_service,
+                local_repository_path,
+                overwrite_contract,
+                contract_path,
+            )
+            commit_message += " and explainer" if not commit_message else ""
             commit = True
         elif options.explainer_docker_config or options.explainer_blob_config:
             self.__prepare_explainer_directory(
-                git_service, local_repository_path, contract_path, overwrite_contract)
+                git_service, local_repository_path, contract_path, overwrite_contract
+            )
             explainer_folder = os.path.join(
-                local_repository_path, contract_path, 'explainer')
+                local_repository_path, contract_path, "explainer"
+            )
             shutil.rmtree(explainer_folder)
             os.mkdir(explainer_folder)
             if options.explainer_docker_config:
                 explainer_type = ModelType.CUSTOM.value
                 self.__create_reference_file(
-                    explainer_folder, dockerReference=options.explainer_docker_config)
+                    explainer_folder, dockerReference=options.explainer_docker_config
+                )
             elif options.explainer_blob_config:
                 explainer_type = explainer_type
                 self.__create_reference_file(
-                    explainer_folder, blobReference=options.explainer_blob_config)
-            git_service.add_folder_to_staging(os.path.join(contract_path, 'explainer'))
-            commit_message += ' and explainer' if not commit_message else ''
+                    explainer_folder, blobReference=options.explainer_blob_config
+                )
+            git_service.add_folder_to_staging(os.path.join(contract_path, "explainer"))
+            commit_message += " and explainer" if not commit_message else ""
             commit = True
         else:
             reference_path = os.path.join(
-                local_repository_path, contract_path, 'explainer', 'reference.json')
+                local_repository_path, contract_path, "explainer", "reference.json"
+            )
 
             try:
                 with open(reference_path) as referenceFile:
                     data = json.load(referenceFile)
-                    if 'reference' in data:
-                        if "blob" in data['reference']:
+                    if "reference" in data:
+                        if "blob" in data["reference"]:
                             explainer_type = explainer_type
-                        elif "docker" in data['reference']:
+                        elif "docker" in data["reference"]:
                             explainer_type = ExplainerType.CUSTOM.value
                         else:
-                            raise Exception('No information on to be deployed explainer available.')
+                            raise Exception(
+                                "No information on to be deployed explainer available."
+                            )
                     else:
-                        raise Exception('No information on to be deployed explainer available.')
+                        raise Exception(
+                            "No information on to be deployed explainer available."
+                        )
             except IOError:
                 explainer_type = ExplainerType.NO_EXPLAINER.value
 
-        metadata_path = os.path.join(local_repository_path, contract_path, 'metadata.json')
-        self.__prepare_metadata_file(metadata_path, options.feature_labels, options.problem_type,
-                                     options.prediction_classes, overwrite_metadata)
-        git_service.add_folder_to_staging(os.path.join(contract_path, 'metadata.json'))
+        metadata_path = os.path.join(
+            local_repository_path, contract_path, "metadata.json"
+        )
+        self.__prepare_metadata_file(
+            metadata_path,
+            options.feature_labels,
+            options.problem_type,
+            options.prediction_classes,
+            overwrite_metadata,
+        )
+        git_service.add_folder_to_staging(os.path.join(contract_path, "metadata.json"))
 
         if commit:
-            logging.info('Committing and pushing the result to the remote.')
+            logging.info("Committing and pushing the result to the remote.")
             commit_sha = git_service.commit(commit_message)
             git_service.push()
         else:
             commit_sha = Repo(local_repository_path).head.commit.hexsha
 
         deployment_options = {
-            'name': options.name,
-            'description': options.description,
-            'repository_id': self.__config.repository_id,
-            'example_input': options.example_input,
-            'example_output': options.example_output,
-            'model_type': model_type,
-            'model_serverless': options.model_serverless,
-            'model_instance_type': options.model_instance_type,
-            'model_cpu_limit': options.model_cpu_limit,
-            'model_cpu_request': options.model_cpu_request,
-            'model_mem_limit': options.model_mem_limit,
-            'model_mem_request': options.model_mem_request,
-            'branch_name': git_service.get_current_branch_name(),
-            'commit': commit_sha,
-            'explainer_type': explainer_type,
-            'explainer_serverless': options.explainer_serverless,
-            'explainer_instance_type': options.explainer_instance_type,
-            'explainer_cpu_limit': options.explainer_cpu_limit,
-            'explainer_cpu_request': options.explainer_cpu_request,
-            'explainer_mem_limit': options.explainer_mem_limit,
-            'explainer_mem_request': options.explainer_mem_request,
-            'contract_path': contract_path,
-            'tags': {'primary': options.custom_id, 'secondary': []},
+            "name": options.name,
+            "description": options.description,
+            "repository_id": self.__config.repository_id,
+            "example_input": options.example_input,
+            "example_output": options.example_output,
+            "model_type": model_type,
+            "model_serverless": options.model_serverless,
+            "model_instance_type": options.model_instance_type,
+            "model_cpu_limit": options.model_cpu_limit,
+            "model_cpu_request": options.model_cpu_request,
+            "model_mem_limit": options.model_mem_limit,
+            "model_mem_request": options.model_mem_request,
+            "branch_name": git_service.get_current_branch_name(),
+            "commit": commit_sha,
+            "explainer_type": explainer_type,
+            "explainer_serverless": options.explainer_serverless,
+            "explainer_instance_type": options.explainer_instance_type,
+            "explainer_cpu_limit": options.explainer_cpu_limit,
+            "explainer_cpu_request": options.explainer_cpu_request,
+            "explainer_mem_limit": options.explainer_mem_limit,
+            "explainer_mem_request": options.explainer_mem_request,
+            "contract_path": contract_path,
+            "tags": {"primary": options.custom_id, "secondary": []},
         }
 
         deployment = self.__deeploy_service.create_deployment(
-            self.__config.workspace_id, CreateDeployment(**deployment_options))
+            self.__config.workspace_id, CreateDeployment(**deployment_options)
+        )
 
         return deployment
 
-    def update(self, options: UpdateOptions, local_repository_path: str = None,
-               model: Any = None, explainer: Any = None, model_type: int = None,
-               explainer_type: int = None, overwrite_contract: bool = False,
-               overwrite_metadata: bool = False, commit_sha: str = None, commit_message: str = None,
-               contract_path: str = "") -> Deployment:
+    def update(
+        self,
+        options: UpdateOptions,
+        local_repository_path: str = None,
+        model: Any = None,
+        explainer: Any = None,
+        model_type: int = None,
+        explainer_type: int = None,
+        overwrite_contract: bool = False,
+        overwrite_metadata: bool = False,
+        commit_sha: str = None,
+        commit_message: str = None,
+        contract_path: str = "",
+    ) -> Deployment:
         """Update a model on Deeploy
         Parameters:
             model (Any): The class instance of an ML model
             options (UpdateOptions): An instance of the update options class
                 containing the update options
             local_repository_path (str): Absolute path to the local git repository
                 which is connected to Deeploy
@@ -256,228 +334,295 @@
                 file. Defaults to False.
             commit_sha (str, optional): Commit SHA to update to
             commit_message (str, optional): Commit message to use
             contract_path (str, optional): Relative repository subpath that contains the
                 Deeploy contract to deploy from
         """
         if not (self.__config.access_key and self.__config.secret_key):
-            raise Exception('Missing access credentials to update deployment.')
+            raise Exception("Missing access credentials to update deployment.")
 
-        if not (self.__deeploy_service.get_deployment(self.__config.workspace_id,
-                                                      options.deployment_id)):
+        if not (
+            self.__deeploy_service.get_deployment(
+                self.__config.workspace_id, options.deployment_id
+            )
+        ):
             raise Exception(
-                'Deployment was not found in the Deeploy workspace. \
-                 Make sure the Deployment Id is correct.')
+                "Deployment was not found in the Deeploy workspace. \
+                 Make sure the Deployment Id is correct."
+            )
 
         git_service = GitService(local_repository_path)
 
         current_deployment = self.__deeploy_service.get_deployment(
-            self.__config.workspace_id, options.deployment_id)
+            self.__config.workspace_id, options.deployment_id
+        )
 
         commit = False
 
-        if (model or explainer):
-            if (local_repository_path is None):
+        if model or explainer:
+            if local_repository_path is None:
                 raise Exception(
-                    'Local repository path is required to update \
-                     the model or explainer.')
+                    "Local repository path is required to update \
+                     the model or explainer."
+                )
             else:
-                repository_in_workspace, repository_id = \
-                    self.__is_git_repository_in_workspace(git_service)
+                (
+                    repository_in_workspace,
+                    repository_id,
+                ) = self.__is_git_repository_in_workspace(git_service)
 
             if not repository_in_workspace:
                 raise Exception(
-                    'Repository was not found in the Deeploy workspace. \
-                     Make sure you have connected it before.')
+                    "Repository was not found in the Deeploy workspace. \
+                     Make sure you have connected it before."
+                )
 
             self.__config.repository_id = repository_id
 
             commit = True
-            logging.info('Pulling from the remote repository...')
+            logging.info("Pulling from the remote repository...")
             git_service.pull()
-            logging.info('Successfully pulled from the remote repository.')
+            logging.info("Successfully pulled from the remote repository.")
 
             if model:
                 model_wrapper = self.__process_model(
-                    model, options, local_repository_path, git_service, overwrite_contract, contract_path)
+                    model,
+                    options,
+                    local_repository_path,
+                    git_service,
+                    overwrite_contract,
+                    contract_path,
+                )
                 model_type = model_wrapper.get_model_type().value
-                commit_message = '[Deeploy Client] Add new model' if not commit_message else commit_message
+                commit_message = (
+                    "[Deeploy Client] Add new model"
+                    if not commit_message
+                    else commit_message
+                )
             else:
                 # TODO: read existing reference.json and check if its a blob url or image
                 # if blob url then require model_type else set model_type as custom
                 model_type = model_type if model_type else ModelType.CUSTOM.value
 
             if explainer:
                 explainer_wrapper = self.__process_explainer(
-                    explainer, git_service, local_repository_path, overwrite_contract, contract_path)
+                    explainer,
+                    git_service,
+                    local_repository_path,
+                    overwrite_contract,
+                    contract_path,
+                )
                 explainer_type = explainer_wrapper.get_explainer_type().value
                 if explainer_type != ExplainerType.NO_EXPLAINER.value:
-                    commit_message += ' and explainer' if not commit_message else ''
+                    commit_message += " and explainer" if not commit_message else ""
             else:
                 # TODO: read existing reference.json and check if its a blob url or image
                 # if blob url then require explainer_type else set explainer_type as custom
-                explainer_type = explainer_type if explainer_type else ExplainerType.NO_EXPLAINER.value
+                explainer_type = (
+                    explainer_type
+                    if explainer_type
+                    else ExplainerType.NO_EXPLAINER.value
+                )
 
         # process model reference.json
         elif options.model_docker_config or options.model_blob_config:
             self.__prepare_model_directory(
-                git_service, local_repository_path, contract_path, overwrite_contract)
-            model_folder = os.path.join(
-                local_repository_path, contract_path, 'model')
+                git_service, local_repository_path, contract_path, overwrite_contract
+            )
+            model_folder = os.path.join(local_repository_path, contract_path, "model")
             shutil.rmtree(model_folder)
             os.mkdir(model_folder)
             if options.model_docker_config:
                 model_type = ModelType.CUSTOM.value
                 self.__create_reference_file(
-                    model_folder, dockerReference=options.model_docker_config)
+                    model_folder, dockerReference=options.model_docker_config
+                )
             elif options.model_blob_config:
                 model_type = model_type
                 self.__create_reference_file(
-                    model_folder, blobReference=options.model_blob_config)
-            git_service.add_folder_to_staging(os.path.join(contract_path, 'model'))
+                    model_folder, blobReference=options.model_blob_config
+                )
+            git_service.add_folder_to_staging(os.path.join(contract_path, "model"))
             commit = True
 
         # process explainer reference.json
         elif options.explainer_docker_config or options.explainer_blob_config:
             self.__prepare_explainer_directory(
-                git_service, local_repository_path, contract_path, overwrite_contract)
+                git_service, local_repository_path, contract_path, overwrite_contract
+            )
             explainer_folder = os.path.join(
-                local_repository_path, contract_path, 'explainer')
+                local_repository_path, contract_path, "explainer"
+            )
             shutil.rmtree(explainer_folder)
             os.mkdir(explainer_folder)
             if options.explainer_docker_config:
                 explainer_type = ModelType.CUSTOM.value
                 self.__create_reference_file(
-                    explainer_folder, dockerReference=options.explainer_docker_config)
+                    explainer_folder, dockerReference=options.explainer_docker_config
+                )
             elif options.explainer_blob_config:
                 explainer_type = explainer_type
                 self.__create_reference_file(
-                    explainer_folder, blobReference=options.explainer_blob_config)
-            git_service.add_folder_to_staging(os.path.join(contract_path, 'explainer'))
-            commit_message += ' and explainer' if not commit_message else ''
+                    explainer_folder, blobReference=options.explainer_blob_config
+                )
+            git_service.add_folder_to_staging(os.path.join(contract_path, "explainer"))
+            commit_message += " and explainer" if not commit_message else ""
             commit = True
 
-        metadata_path = os.path.join(local_repository_path, contract_path, 'metadata.json')
-        self.__prepare_metadata_file(metadata_path, options.feature_labels, options.problem_type,
-                                     options.prediction_classes, overwrite_metadata)
-        git_service.add_folder_to_staging(os.path.join(contract_path, 'metadata.json'))
+        metadata_path = os.path.join(
+            local_repository_path, contract_path, "metadata.json"
+        )
+        self.__prepare_metadata_file(
+            metadata_path,
+            options.feature_labels,
+            options.problem_type,
+            options.prediction_classes,
+            overwrite_metadata,
+        )
+        git_service.add_folder_to_staging(os.path.join(contract_path, "metadata.json"))
 
         if commit:
-            logging.info('Committing and pushing the result to the remote.')
+            logging.info("Committing and pushing the result to the remote.")
             commit_sha = git_service.commit(commit_message)
             git_service.push()
         else:
-            commit_sha = Repo(local_repository_path).head.commit.hexsha if commit_sha is None else commit_sha
+            commit_sha = (
+                Repo(local_repository_path).head.commit.hexsha
+                if commit_sha is None
+                else commit_sha
+            )
 
-        self.__config.repository_id = current_deployment.active_version['repositoryId']
+        self.__config.repository_id = current_deployment.active_version["repositoryId"]
 
         update_options = {
-            'deployment_id': options.deployment_id,
-            'name': options.name,
-            'description': options.description,
-            'repository_id': self.__config.repository_id,
-            'example_input': options.example_input,
-            'example_output': options.example_output,
-            'model_type': model_type,
-            'model_serverless': options.model_serverless,
-            'model_instance_type': options.model_instance_type,
-            'model_cpu_limit': options.model_cpu_limit,
-            'model_cpu_request': options.model_cpu_request,
-            'model_mem_limit': options.model_mem_limit,
-            'model_mem_request': options.model_mem_request,
-            'commit': commit_sha,
-            'commit_message': commit_message,
-            'explainer_type': explainer_type,
-            'explainer_serverless': options.explainer_serverless,
-            'explainer_instance_type': options.explainer_instance_type,
-            'explainer_cpu_limit': options.explainer_cpu_limit,
-            'explainer_cpu_request': options.explainer_cpu_request,
-            'explainer_mem_limit': options.explainer_mem_limit,
-            'explainer_mem_request': options.explainer_mem_request,
-            'contract_path': contract_path,
+            "deployment_id": options.deployment_id,
+            "name": options.name,
+            "description": options.description,
+            "repository_id": self.__config.repository_id,
+            "example_input": options.example_input,
+            "example_output": options.example_output,
+            "model_type": model_type,
+            "model_serverless": options.model_serverless,
+            "model_instance_type": options.model_instance_type,
+            "model_cpu_limit": options.model_cpu_limit,
+            "model_cpu_request": options.model_cpu_request,
+            "model_mem_limit": options.model_mem_limit,
+            "model_mem_request": options.model_mem_request,
+            "commit": commit_sha,
+            "commit_message": commit_message,
+            "explainer_type": explainer_type,
+            "explainer_serverless": options.explainer_serverless,
+            "explainer_instance_type": options.explainer_instance_type,
+            "explainer_cpu_limit": options.explainer_cpu_limit,
+            "explainer_cpu_request": options.explainer_cpu_request,
+            "explainer_mem_limit": options.explainer_mem_limit,
+            "explainer_mem_request": options.explainer_mem_request,
+            "contract_path": contract_path,
         }
 
         update_options = self.__remove_null_values(update_options)
 
-        if (len(UpdateDeploymentMetadata(**update_options).json()) > 2):
+        if len(UpdateDeploymentMetadata(**update_options).json()) > 2:
             updated_deployment = self.__deeploy_service.update_deployment_metadata(
-                self.__config.workspace_id, UpdateDeploymentMetadata(**update_options))
+                self.__config.workspace_id, UpdateDeploymentMetadata(**update_options)
+            )
 
         if (len(UpdateDeployment(**update_options).json())) > 2:
             updated_deployment = self.__deeploy_service.update_deployment(
-                self.__config.workspace_id, UpdateDeployment(**update_options))
+                self.__config.workspace_id, UpdateDeployment(**update_options)
+            )
 
         return updated_deployment
 
-    def predict(self, deployment_id: str, request_body: dict) -> V1Prediction or V2Prediction:
+    def predict(
+        self, deployment_id: str, request_body: dict
+    ) -> V1Prediction or V2Prediction:
         """Make a predict call
         Parameters:
             deployment_id (str): ID of the Deeploy deployment
             request_body (dict): Request body with input data for the model
         """
 
         workspace_id = self.__config.workspace_id
-        prediction = self.__deeploy_service.predict(workspace_id, deployment_id, request_body)
+        prediction = self.__deeploy_service.predict(
+            workspace_id, deployment_id, request_body
+        )
         return prediction
 
-    def explain(self, deployment_id: str, request_body: dict, image: bool = False) -> object:
+    def explain(
+        self, deployment_id: str, request_body: dict, image: bool = False
+    ) -> object:
         """Make an explain call
         Parameters:
             deployment_id (str): ID of the Deeploy deployment
             request_body (dict): Request body with input data for the model
             image (bool): Return image or not
         """
         workspace_id = self.__config.workspace_id
         explanation = self.__deeploy_service.explain(
-            workspace_id, deployment_id, request_body, image)
+            workspace_id, deployment_id, request_body, image
+        )
         return explanation
 
-    def getRequestLogs(self, deployment_id: str) -> RequestLogs:
+    def getRequestLogs(self, deployment_id: str) -> List[RequestLog]:
         """Retrieve request logs
         Parameters:
             deployment_id (str): ID of the Deeploy deployment
         """
         workspace_id = self.__config.workspace_id
         requestLogs = self.__deeploy_service.getRequestLogs(workspace_id, deployment_id)
         return requestLogs
 
-    def getPredictionLogs(self, deployment_id: str) -> PredictionLogs:
+    def getPredictionLogs(self, deployment_id: str) -> List[PredictionLog]:
         """Retrieve prediction logs
         Parameters:
             deployment_id (str): ID of the Deeploy deployment
         """
         workspace_id = self.__config.workspace_id
-        predictionLogs = self.__deeploy_service.getPredictionLogs(workspace_id, deployment_id)
+        predictionLogs = self.__deeploy_service.getPredictionLogs(
+            workspace_id, deployment_id
+        )
         return predictionLogs
 
-    def getOnePredictionLog(self, deployment_id: str, request_log_id: str,
-                            prediction_log_id: str) -> PredictionLog:
+    def getOnePredictionLog(
+        self, deployment_id: str, request_log_id: str, prediction_log_id: str
+    ) -> PredictionLog:
         """Retrieve one log
         Parameters:
             deployment_id (str): ID of the Deeploy deployment
             request_log_id (str): ID of the request_log containing the prediction
             prediction_log_id (str): ID of the prediction_log to be retrieved
         """
         workspace_id = self.__config.workspace_id
-        predictionLog = self.__deeploy_service.getOnePredictionLog(workspace_id, deployment_id,
-                                                                   request_log_id, prediction_log_id)
+        predictionLog = self.__deeploy_service.getOnePredictionLog(
+            workspace_id, deployment_id, request_log_id, prediction_log_id
+        )
         return predictionLog
 
-    def evaluate(self, deployment_id: str, request_log_id: str, prediction_log_id: str,
-                 evaluation_input: dict) -> None:
+    def evaluate(
+        self,
+        deployment_id: str,
+        request_log_id: str,
+        prediction_log_id: str,
+        evaluation_input: dict,
+    ) -> None:
         """Evaluate a prediction log
         Parameters:
             deployment_id (str): ID of the Deeploy deployment
             log_id (int): ID of the log to be evaluated
             evaluation_input: Dict with result, value, and explanation
         """
         workspace_id = self.__config.workspace_id
-        self.__deeploy_service.evaluate(workspace_id, deployment_id,
-                                        request_log_id, prediction_log_id,
-                                        evaluation_input)
+        self.__deeploy_service.evaluate(
+            workspace_id,
+            deployment_id,
+            request_log_id,
+            prediction_log_id,
+            evaluation_input,
+        )
 
     def actuals(self, deployment_id: str, actuals_input: dict) -> None:
         """Evaluate a prediction log
         Parameters:
             deployment_id (str): ID of the Deeploy deployment
             actuals_input (dict): Object with predictionIds and actualsValues
                                  where the order of the values will match
@@ -487,220 +632,275 @@
                                     "actualValues": {"predictions" | "output": []}
                                  }
         """
         workspace_id = self.__config.workspace_id
         self.__deeploy_service.actuals(workspace_id, deployment_id, actuals_input)
 
     def __are_clientoptions_valid(self, config: ClientConfig) -> bool:
-        """Check if the supplied options are valid
-        """
+        """Check if the supplied options are valid"""
         try:
             self.__deeploy_service.get_workspace(config.workspace_id)
         except Exception as e:
             raise e
 
         return True
 
-    def __is_git_repository_in_workspace(self, git_service: GitService) -> Tuple[bool, str]:
+    def __is_git_repository_in_workspace(
+        self, git_service: GitService
+    ) -> Tuple[bool, str]:
         remote_url = git_service.get_remote_url()
         workspace_id = self.__config.workspace_id
 
         repositories = self.__deeploy_service.get_repositories(workspace_id)
 
         correct_repositories = list(
-            filter(lambda x: x.remote_path == self.__parse_url_ssh_to_https(remote_url) or
-                   x.remote_path == remote_url, repositories))
+            filter(
+                lambda x: x.remote_path == self.__parse_url_ssh_to_https(remote_url)
+                or x.remote_path == remote_url,
+                repositories,
+            )
+        )
 
         if len(correct_repositories) != 0:
             repository_id = correct_repositories[0].id
             return True, repository_id
 
         return False, None
 
     def __parse_url_ssh_to_https(self, remote_path: str) -> str or None:
-        if (remote_path[:4] != 'git@'):
+        if remote_path[:4] != "git@":
             # https to ssh
-            path_tokens = remote_path.split('/')
+            path_tokens = remote_path.split("/")
             provider = path_tokens[2]
             user = path_tokens[3]
             path = path_tokens[4:]
             link = "git@" + provider + ":" + user
             for sub_directory in path:
                 link += "/" + sub_directory
         else:
             # ssh to https
-            path_tokens = remote_path.split('@')
-            link = "https://" + path_tokens[1].replace(':', '/')
+            path_tokens = remote_path.split("@")
+            link = "https://" + path_tokens[1].replace(":", "/")
         return link
 
-    def __prepare_model_directory(self, git_service: GitService, local_repository_path: str,
-                                  contract_path: str, overwrite_contract) -> None:
-        model_folder_path = os.path.join(
-            local_repository_path, contract_path, 'model')
+    def __prepare_model_directory(
+        self,
+        git_service: GitService,
+        local_repository_path: str,
+        contract_path: str,
+        overwrite_contract,
+    ) -> None:
+        model_folder_path = os.path.join(local_repository_path, contract_path, "model")
         if not directory_exists(model_folder_path):
             try:
                 os.mkdir(model_folder_path)
             except OSError:
-                logging.error("Creation of the directory %s failed" %
-                              model_folder_path)
+                logging.error("Creation of the directory %s failed" % model_folder_path)
         elif not directory_empty(model_folder_path):
             if not overwrite_contract:
                 raise Exception(
-                    'The folder %s is not empty. Pass \'overwrite=True\' to overwrite contents.' %
-                    model_folder_path)
+                    "The folder %s is not empty. Pass 'overwrite=True' to overwrite contents."
+                    % model_folder_path
+                )
             delete_all_contents_in_directory(model_folder_path)
-            git_service.delete_folder_from_staging('model')
+            git_service.delete_folder_from_staging("model")
         else:  # folder exists and empty
             pass
         return
 
-    def __prepare_explainer_directory(self, git_service: GitService, local_repository_path: str,
-                                      contract_path: str, overwrite_contract) -> None:
+    def __prepare_explainer_directory(
+        self,
+        git_service: GitService,
+        local_repository_path: str,
+        contract_path: str,
+        overwrite_contract,
+    ) -> None:
         explainer_folder_path = os.path.join(
-            local_repository_path, contract_path, 'explainer')
+            local_repository_path, contract_path, "explainer"
+        )
         if not directory_exists(explainer_folder_path):
             try:
                 os.mkdir(explainer_folder_path)
             except OSError:
-                logging.error("Creation of the directory %s failed" %
-                              explainer_folder_path)
+                logging.error(
+                    "Creation of the directory %s failed" % explainer_folder_path
+                )
         elif not directory_empty(explainer_folder_path):
             if not overwrite_contract:
                 raise Exception(
-                    'The folder %s is not empty. Pass \'overwrite=True\' to overwrite contents.' %
-                    explainer_folder_path)
+                    "The folder %s is not empty. Pass 'overwrite=True' to overwrite contents."
+                    % explainer_folder_path
+                )
             delete_all_contents_in_directory(explainer_folder_path)
-            git_service.delete_folder_from_staging('explainer')
+            git_service.delete_folder_from_staging("explainer")
         else:  # folder exists and empty
             pass
         return
 
-    def __prepare_metadata_file(self, path: str, feature_labels=None,
-                                problem_type=None, prediction_classes=None,
-                                overwrite_metadata=False) -> None:
-        data = {
-            'featureLabels': [],
-            'problemType': {},
-            'predictionClasses': ''
-        }
+    def __prepare_metadata_file(
+        self,
+        path: str,
+        feature_labels=None,
+        problem_type=None,
+        prediction_classes=None,
+        overwrite_metadata=False,
+    ) -> None:
+        data = {"featureLabels": [], "problemType": {}, "predictionClasses": ""}
 
         if feature_labels:
-            data['featureLabels'] = feature_labels
+            data["featureLabels"] = feature_labels
         if problem_type:
-            data['problemType'] = problem_type
+            data["problemType"] = problem_type
         if prediction_classes:
-            data['predictionClasses'] = prediction_classes
+            data["predictionClasses"] = prediction_classes
 
         if file_exists(path) and not overwrite_metadata:
             pass
         else:
             try:
-                with open(path, 'w') as f:
+                with open(path, "w") as f:
                     json.dump(data, f)
             except OSError:
                 logging.error("Creation of the file %s failed" % path)
 
     def __get_upload_size(self, local_folder_path: str) -> int:
         total_file_sizes = 0
         for root, _, files in os.walk(local_folder_path):
             for single_file in files:
                 file_path = os.path.join(root, single_file)
                 file_size = os.path.getsize(file_path)
                 total_file_sizes += file_size
         return total_file_sizes
 
-    def __upload_folder_to_blob(self, local_repository_path: str, local_folder_path: str) -> str:
+    def __upload_folder_to_blob(
+        self, local_repository_path: str, local_folder_path: str
+    ) -> str:
         upload_locations = list()
         blob_folder_uuid = str(uuid.uuid4())
         relative_folder_path = os.path.relpath(local_folder_path, local_repository_path)
         for root, _, files in os.walk(local_folder_path):
             for single_file in files:
                 relative_file_path = os.path.join(
-                    relative_folder_path, os.path.relpath(root, local_folder_path))
+                    relative_folder_path, os.path.relpath(root, local_folder_path)
+                )
                 file_path = os.path.join(root, single_file)
                 blob_file_location = self.__deeploy_service.upload_blob_file(
                     file_path,
                     relative_file_path,
                     self.__config.workspace_id,
                     self.__config.repository_id,
-                    blob_folder_uuid)
+                    blob_folder_uuid,
+                )
                 upload_locations.append(blob_file_location)
 
         partition = upload_locations[0].partition(relative_folder_path)
         blob_folder_path = partition[0] + partition[1]
         return blob_folder_path
 
     def __remove_null_values(self, d: dict) -> dict:
         def empty(x):
             return x is None or x == {} or x == []
 
         if not isinstance(d, (dict, list)):
             return d
         elif isinstance(d, list):
-            return [v for v in (self.__remove_null_values(v) for v in d) if not empty(v)]
+            return [
+                v for v in (self.__remove_null_values(v) for v in d) if not empty(v)
+            ]
         else:
-            return {k: v for k, v in ((k, self.__remove_null_values(v))
-                    for k, v in d.items()) if not empty(v)}
-
-    def __create_reference_file(self, local_folder_path: str, dockerReference: DockerReference = None,
-                                blobReference: BlobReference = None) -> None:
-        file_path = os.path.join(local_folder_path, 'reference.json')
+            return {
+                k: v
+                for k, v in ((k, self.__remove_null_values(v)) for k, v in d.items())
+                if not empty(v)
+            }
+
+    def __create_reference_file(
+        self,
+        local_folder_path: str,
+        dockerReference: DockerReference = None,
+        blobReference: BlobReference = None,
+    ) -> None:
+        file_path = os.path.join(local_folder_path, "reference.json")
 
         reference_json = {
-            'reference': {
-                'docker': {
-                    'image': dockerReference.image if dockerReference else None,
-                    'uri': dockerReference.uri if dockerReference else None,
-                    'credentialsId': dockerReference.credentialsId if dockerReference else None,
-                    'port': dockerReference.port if dockerReference else None,
+            "reference": {
+                "docker": {
+                    "image": dockerReference.image if dockerReference else None,
+                    "uri": dockerReference.uri if dockerReference else None,
+                    "credentialsId": dockerReference.credentialsId
+                    if dockerReference
+                    else None,
+                    "port": dockerReference.port if dockerReference else None,
                 },
-                'blob': {
-                    'url': blobReference.url if blobReference else None,
-                    'credentialsId': blobReference.credentialsId if blobReference else None,
+                "blob": {
+                    "url": blobReference.url if blobReference else None,
+                    "credentialsId": blobReference.credentialsId
+                    if blobReference
+                    else None,
+                    "region": blobReference.region
+                    if blobReference
+                    else None,
                 },
             },
         }
         reference_json = self.__remove_null_values(reference_json)
 
         data = parse_obj_as(ModelReferenceJson, reference_json)
 
-        with open(file_path, 'w') as outfile:
+        with open(file_path, "w") as outfile:
             json.dump(data.dict(), outfile)
         return
 
-    def __process_model(self, model, options: DeployOptions or UpdateOptions,
-                        local_repository_path: str, git_service: GitService,
-                        overwrite_contract: bool, contract_path: str) -> ModelType:
-        logging.info('Saving the model to disk...')
-        model_folder = os.path.join(
-            local_repository_path, contract_path, 'model')
+    def __process_model(
+        self,
+        model,
+        options: DeployOptions or UpdateOptions,
+        local_repository_path: str,
+        git_service: GitService,
+        overwrite_contract: bool,
+        contract_path: str,
+    ) -> ModelType:
+        logging.info("Saving the model to disk...")
+        model_folder = os.path.join(local_repository_path, contract_path, "model")
         model_wrapper = ModelWrapper(
             model,
             pytorch_model_file_path=options.pytorch_model_file_path,
-            pytorch_torchserve_handler_name=options.pytorch_torchserve_handler_name)
-        model_wrapper.save(model_folder)
+            pytorch_torchserve_handler_name=options.pytorch_torchserve_handler_name,
+        )
         self.__prepare_model_directory(
-            git_service, local_repository_path, contract_path, overwrite_contract)
+            git_service, local_repository_path, contract_path, overwrite_contract
+        )
+        model_wrapper.save(model_folder)
         blob_storage_link = self.__upload_folder_to_blob(
-            local_repository_path, model_folder)
+            local_repository_path, model_folder
+        )
         shutil.rmtree(model_folder)
         os.mkdir(model_folder)
-        self.__create_reference_file(model_folder, blob_storage_link)
-        git_service.add_folder_to_staging(os.path.join(contract_path, 'model'))
+        self.__create_reference_file(model_folder, blobReference=BlobReference(url=blob_storage_link))
+        git_service.add_folder_to_staging(os.path.join(contract_path, "model"))
         return model_wrapper.get_model_type()
 
-    def __process_explainer(self, explainer, git_service: GitService,
-                            local_repository_path: str, overwrite_contract: bool,
-                            contract_path: str) -> ExplainerType:
-        logging.info('Saving the explainer to disk...')
+    def __process_explainer(
+        self,
+        explainer,
+        git_service: GitService,
+        local_repository_path: str,
+        overwrite_contract: bool,
+        contract_path: str,
+    ) -> ExplainerType:
+        logging.info("Saving the explainer to disk...")
         explainer_wrapper = ExplainerWrapper(explainer)
-        self.__prepare_explainer_directory(git_service, contract_path, overwrite_contract)
+        self.__prepare_explainer_directory(
+            git_service, local_repository_path, contract_path, overwrite_contract
+        )
         explainer_folder = os.path.join(
-            local_repository_path, contract_path, 'explainer')
+            local_repository_path, contract_path, "explainer"
+        )
         explainer_wrapper.save(explainer_folder)
         blob_storage_link = self.__upload_folder_to_blob(
-            local_repository_path, explainer_folder)
+            local_repository_path, explainer_folder
+        )
         shutil.rmtree(explainer_folder)
         os.mkdir(explainer_folder)
-        self.__create_reference_file(explainer_folder, blob_storage_link)
-        git_service.add_folder_to_staging(os.path.join(contract_path, 'explainer'))
-        return explainer_wrapper
+        self.__create_reference_file(explainer_folder, blobReference=BlobReference(url=blob_storage_link))
+        git_service.add_folder_to_staging(os.path.join(contract_path, "explainer"))
+        return explainer_wrapper.get_explainer_type().value
```

### Comparing `deeploy-0.5.1/deeploy/models/__init__.py` & `deeploy-1.0.0/deeploy/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from .deployment import Deployment  # noqa
-from .update_deployment import UpdateDeployment, UpdateDeploymentMetadata  # noqa
-from .create_version import CreateVersion  # noqa
-from .repository import Repository  # noqa
-from .client_options import ClientConfig  # noqa
-from .create_deployment import CreateDeployment  # noqa
-from .workspace import Workspace  # noqa
-from .deploy_options import DeployOptions  # noqa
-from .update_options import UpdateOptions  # noqa
-from .prediction import V1Prediction, V2Prediction  # noqa
-from .prediction_log import RequestLog, PredictionLog  # noqa
-from .prediction_logs import RequestLogs, PredictionLogs  # noqa
-from .model_reference_json import ModelReferenceJson, BlobReference, DockerReference  # noqa
+# flake8: noqa
+from .deployment import Deployment
+from .update_deployment import UpdateDeployment, UpdateDeploymentMetadata
+from .create_version import CreateVersion
+from .repository import Repository
+from .client_options import ClientConfig
+from .create_deployment import CreateDeployment
+from .workspace import Workspace
+from .deploy_options import DeployOptions
+from .update_options import UpdateOptions
+from .prediction import V1Prediction, V2Prediction
+from .prediction_log import RequestLog, PredictionLog
+from .model_reference_json import (
+    ModelReferenceJson,
+    BlobReference,
+    DockerReference,
+)
```

### Comparing `deeploy-0.5.1/deeploy/models/client_options.py` & `deeploy-1.0.0/deeploy/models/client_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
       workspace_id: string representing the workspace id in which to create
         deployments
       local_repository_path: string representing the relative or absolute path
         to the local git repository
       branch_name: string representing the branch name on which to commit. Defaults
         to the local active branch
     """
+
     access_key: Optional[str]
     secret_key: Optional[str]
     token: Optional[str]
     host: str
     workspace_id: str
     repository_id: str
     branch_name: Optional[str]
```

### Comparing `deeploy-0.5.1/deeploy/models/create_deployment.py` & `deeploy-1.0.0/deeploy/models/create_deployment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Any, List
 
 from pydantic import BaseModel
 
 
 class CreateDeployment(BaseModel):
-    """Class that contains the options for creating a deployment
-    """  # noqa
+    """Class that contains the options for creating a deployment"""  # noqa
+
     name: str
     description: Optional[str]
     repository_id: Optional[str]
     branch_name: Optional[str]
     commit: Optional[str]
     commit_message: Optional[str]
     contract_path: Optional[str]
@@ -18,44 +18,43 @@
     example_output: Optional[Any]
     input_tensor_size: Optional[str]
     output_tensor_size: Optional[str]
     model_type: Optional[Any]
     model_serverless: Optional[bool] = False
     model_instance_type: Optional[str]
     model_cpu_limit: Optional[float]
-    model_cpu_request:  Optional[float]
+    model_cpu_request: Optional[float]
     model_mem_limit: Optional[int]
     model_mem_request: Optional[int]
     explainer_type: Optional[Any]
     explainer_serverless: Optional[bool] = False
     explainer_instance_type: Optional[str]
-    explainer_instance_type: Optional[str]
     explainer_cpu_limit: Optional[float]
-    explainer_cpu_request:  Optional[float]
+    explainer_cpu_request: Optional[float]
     explainer_mem_limit: Optional[int]
     explainer_mem_request: Optional[int]
 
     def to_request_body(self):
         return {
-            'name': self.name,
-            'description': self.description,
-            'repositoryId': self.repository_id,
-            'exampleInput': self.example_input,
-            'exampleOutput': self.example_output,
-            'modelType': self.model_type,
-            'modelServerless': self.model_serverless,
-            'modelInstanceType': self.model_instance_type,
-            'modelCpuLimit': self.model_cpu_limit,
-            'modelCpuRequest': self.model_cpu_request,
-            'modelMemLimit': self.model_mem_limit,
-            'modelMemRequest': self.model_mem_request,
-            'explainerType': self.explainer_type,
-            'explainerServerless': self.explainer_serverless,
-            'explainerInstanceType': self.explainer_instance_type,
-            'explainerCpuLimit': self.explainer_cpu_limit,
-            'explainerCpuRequest': self.explainer_cpu_request,
-            'explainerMemLimit': self.explainer_mem_limit,
-            'explainerMemRequest': self.explainer_mem_request,
-            'branchName': self.branch_name,
-            'commit': self.commit,
-            'contractPath': self.contract_path,
+            "name": self.name,
+            "description": self.description,
+            "repositoryId": self.repository_id,
+            "exampleInput": self.example_input,
+            "exampleOutput": self.example_output,
+            "modelType": self.model_type,
+            "modelServerless": self.model_serverless,
+            "modelInstanceType": self.model_instance_type,
+            "modelCpuLimit": self.model_cpu_limit,
+            "modelCpuRequest": self.model_cpu_request,
+            "modelMemLimit": self.model_mem_limit,
+            "modelMemRequest": self.model_mem_request,
+            "explainerType": self.explainer_type,
+            "explainerServerless": self.explainer_serverless,
+            "explainerInstanceType": self.explainer_instance_type,
+            "explainerCpuLimit": self.explainer_cpu_limit,
+            "explainerCpuRequest": self.explainer_cpu_request,
+            "explainerMemLimit": self.explainer_mem_limit,
+            "explainerMemRequest": self.explainer_mem_request,
+            "branchName": self.branch_name,
+            "commit": self.commit,
+            "contractPath": self.contract_path,
         }
```

### Comparing `deeploy-0.5.1/deeploy/models/create_version.py` & `deeploy-1.0.0/deeploy/models/create_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, List, Any
 
 from pydantic import BaseModel
 
 
 class CreateVersion(BaseModel):
-    """
-    """
+    """ """
+
     repository_id: Optional[str]
     branch_name: Optional[str]
     commit: Optional[str]
     commit_message: Optional[str]
     contract_path: Optional[str]
     has_example_input: Optional[bool]
     example_input: Optional[List[Any]]
```

### Comparing `deeploy-0.5.1/deeploy/models/deploy_options.py` & `deeploy-1.0.0/deeploy/models/deploy_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 
 from pydantic import BaseModel
 
 from deeploy.models.model_reference_json import BlobReference, DockerReference
 
 
 class DeployOptions(BaseModel):
-    """Class that contains the options for deploying a model
-    """  # noqa
+    """Class that contains the options for deploying a model"""  # noqa
+
     name: str
     """str: name of the deployment"""  # noqa
     description: Optional[str]
     """str, optional: the description of the deployment"""  # noqa
     model_serverless = False
     """bool, optional: whether to deploy the model in a serverless fashion. Defaults to False"""  # noqa
     model_instance_type: Optional[str]
     """str, optional: The preferred instance type for the model pod."""  # noqa
     model_cpu_limit: Optional[float]
     """float, optional: CPU limit of model pod, in CPUs."""  # noqa
-    model_cpu_request:  Optional[float]
+    model_cpu_request: Optional[float]
     """float, optional: CPU request of model pod, in CPUs."""  # noqa
     model_mem_limit: Optional[int]
     """int, optional: RAM limit of model pod, in Megabytes."""  # noqa
     model_mem_request: Optional[int]
     """int, optional: RAM request of model pod, in Megabytes."""  # noqa
     explainer_serverless = False
     """bool, optional: whether to deploy the model in a serverless fashion. Defaults to False"""  # noqa
     explainer_instance_type: Optional[str]
     """str, optional: The preferred instance type for the model pod."""  # noqa
     explainer_cpu_limit: Optional[float]
     """float, optional: CPU limit of model pod, in CPUs."""  # noqa
-    explainer_cpu_request:  Optional[float]
+    explainer_cpu_request: Optional[float]
     """float, optional: CPU request of model pod, in CPUs."""  # noqa
     explainer_mem_limit: Optional[int]
     """int, optional: RAM limit of model pod, in Megabytes."""  # noqa
     explainer_mem_request: Optional[int]
     """int, optional: RAM request of model pod, in Megabytes."""  # noqa
     example_input: Optional[List[Any]]
     """List, optional: list of example input parameters for the model"""  # noqa
```

### Comparing `deeploy-0.5.1/deeploy/models/deployment.py` & `deeploy-1.0.0/deeploy/models/deployment.py`

 * *Files identical despite different names*

### Comparing `deeploy-0.5.1/deeploy/models/prediction_log.py` & `deeploy-1.0.0/deeploy/models/prediction_log.py`

 * *Files identical despite different names*

### Comparing `deeploy-0.5.1/deeploy/models/update_options.py` & `deeploy-1.0.0/deeploy/models/update_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 
 from pydantic import BaseModel
 
 from deeploy.models.model_reference_json import BlobReference, DockerReference
 
 
 class UpdateOptions(BaseModel):
-    """Class that contains the options for updating a model
-    """  # noqa
+    """Class that contains the options for updating a model"""  # noqa
+
     deployment_id: str
     """str: the id of the deployment"""  # noqa
     name: Optional[str]
     """str, optional: the display name of the deployment"""  # noqa
     description: Optional[str]
     """str, optional: the description of the deployment"""  # noqa
     model_serverless: Optional[bool]
     """bool, optional: whether to deploy the model in a serverless fashion"""  # noqa
     model_instance_type: Optional[str]
-    """str, optional: The preferred instance type for the model pod.""" # noqa
+    """str, optional: The preferred instance type for the model pod."""  # noqa
     model_cpu_limit: Optional[float]
-    """float, optional: CPU limit of model pod, in CPUs.""" # noqa
-    model_cpu_request:  Optional[float]
-    """float, optional: CPU request of model pod, in CPUs.""" # noqa
+    """float, optional: CPU limit of model pod, in CPUs."""  # noqa
+    model_cpu_request: Optional[float]
+    """float, optional: CPU request of model pod, in CPUs."""  # noqa
     model_mem_limit: Optional[int]
-    """int, optional: RAM limit of model pod, in Megabytes.""" # noqa
+    """int, optional: RAM limit of model pod, in Megabytes."""  # noqa
     model_mem_request: Optional[int]
-    """int, optional: RAM request of model pod, in Megabytes.""" # noqa
+    """int, optional: RAM request of model pod, in Megabytes."""  # noqa
     explainer_serverless: Optional[bool]
     """bool, optional: whether to deploy the model in a serverless fashion"""  # noqa
     explainer_instance_type: Optional[str]
-    """str, optional: The preferred instance type for the model pod.""" # noqa
+    """str, optional: The preferred instance type for the model pod."""  # noqa
     explainer_cpu_limit: Optional[float]
-    """float, optional: CPU limit of model pod, in CPUs.""" # noqa
-    explainer_cpu_request:  Optional[float]
-    """float, optional: CPU request of model pod, in CPUs.""" # noqa
+    """float, optional: CPU limit of model pod, in CPUs."""  # noqa
+    explainer_cpu_request: Optional[float]
+    """float, optional: CPU request of model pod, in CPUs."""  # noqa
     explainer_mem_limit: Optional[int]
-    """int, optional: RAM limit of model pod, in Megabytes.""" # noqa
+    """int, optional: RAM limit of model pod, in Megabytes."""  # noqa
     explainer_mem_request: Optional[int]
-    """int, optional: RAM request of model pod, in Megabytes.""" # noqa
+    """int, optional: RAM request of model pod, in Megabytes."""  # noqa
     example_input: Optional[List[Any]]
     """List, optional: list of example input parameters for the model"""  # noqa
     example_output: Optional[List[Any]]
     """List, optional: list of example output for the model"""  # noqa
     feature_labels: Optional[List[str]]
     """List, optional: list of feature labels as deployment metadata"""  # noqa
     prediction_classes: Optional[dict]
```

### Comparing `deeploy-0.5.1/deeploy/services/deeploy_service.py` & `deeploy-1.0.0/deeploy/services/deeploy_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,310 +1,422 @@
 import base64
 from typing import List
 
 import requests
+from deeploy.models.prediction_log import RequestLog
 from pydantic import parse_obj_as
 
-from deeploy.models import Deployment, Repository, CreateDeployment, Workspace, \
-    V1Prediction, V2Prediction, PredictionLog, RequestLogs, PredictionLogs, UpdateDeployment, \
-    UpdateDeploymentMetadata
+from deeploy.models import (
+    Deployment,
+    Repository,
+    CreateDeployment,
+    Workspace,
+    V1Prediction,
+    V2Prediction,
+    PredictionLog,
+    UpdateDeployment,
+    UpdateDeploymentMetadata,
+)
 from deeploy.enums import PredictionVersion, AuthType
 
 
 class DeeployService(object):
     """
     A class for interacting with the Deeploy API
     """
 
     def __init__(
-            self, host: str, workspace_id: str, access_key: str = None, secret_key: str = None,
-            token: str = None, insecure=False) -> None:
+        self,
+        host: str,
+        workspace_id: str,
+        access_key: str = None,
+        secret_key: str = None,
+        token: str = None,
+        insecure=False,
+    ) -> None:
         self.__access_key = access_key
         self.__secret_key = secret_key
         self.__token = token
         self.__workspace_id = workspace_id
-        self.__host = 'http://api.%s' % host if insecure else 'https://api.%s' % host
+        self.__host = "http://api.%s" % host if insecure else "https://api.%s" % host
 
         if (access_key and secret_key) or token:
             if (access_key and secret_key) and not self.__keys_are_valid():
-                raise Exception('Access keys are not valid.')
+                raise Exception("Access keys are not valid.")
         else:
-            raise Exception('Missing authentication data.')
+            raise Exception("Missing authentication data.")
         return
 
     def get_repositories(self, workspace_id: str) -> List[Repository]:
-        url = '%s/workspaces/%s/repositories' % (
-            self.__host, workspace_id)
+        url = "%s/workspaces/%s/repositories" % (self.__host, workspace_id)
         params = {
-            'isArchived': False,
+            "isArchived": False,
         }
 
         repositories_response = requests.get(
-            url, params=params, auth=(self.__access_key, self.__secret_key))
+            url, params=params, auth=(self.__access_key, self.__secret_key)
+        )
 
-        repositories = parse_obj_as(
-            List[Repository], repositories_response.json())
+        repositories = parse_obj_as(List[Repository], repositories_response.json())
 
         return repositories
 
     def get_repository(self, workspace_id: str, repository_id: str) -> Repository:
-        url = '%s/workspaces/%s/repositories/%s' % (
-            self.__host, workspace_id, repository_id)
+        url = "%s/workspaces/%s/repositories/%s" % (
+            self.__host,
+            workspace_id,
+            repository_id,
+        )
 
         repository_response = requests.get(
-            url, auth=(self.__access_key, self.__secret_key))
+            url, auth=(self.__access_key, self.__secret_key)
+        )
         if not self.__request_is_successful(repository_response):
-            raise Exception('Repository does not exist in the workspace.')
+            raise Exception("Repository does not exist in the workspace.")
 
         repository = parse_obj_as(Repository, repository_response.json())
 
         return repository
 
     def get_deployment(
-            self, workspace_id: str, deployment_id: str,
-            withExamples: bool = False) -> Deployment:
-        url = '%s/workspaces/%s/deployments/%s' % (self.__host, workspace_id, deployment_id)
+        self, workspace_id: str, deployment_id: str, withExamples: bool = False
+    ) -> Deployment:
+        url = "%s/workspaces/%s/deployments/%s" % (
+            self.__host,
+            workspace_id,
+            deployment_id,
+        )
         params = {
-            'withExamples': withExamples,
+            "withExamples": withExamples,
         }
         deployment_response = requests.get(
-            url, params=params, auth=(self.__access_key, self.__secret_key))
+            url, params=params, auth=(self.__access_key, self.__secret_key)
+        )
         if not self.__request_is_successful(deployment_response):
-            raise Exception('Failed to retrieve the deployment: %s' %
-                            str(deployment_response.json()))
+            raise Exception(
+                "Failed to retrieve the deployment: %s"
+                % str(deployment_response.json())
+            )
 
-        deployment = parse_obj_as(
-            Deployment, deployment_response.json())
+        deployment = parse_obj_as(Deployment, deployment_response.json())
 
         return deployment
 
-    def create_deployment(self, workspace_id: str, deployment: CreateDeployment) -> Deployment:
-        url = '%s/workspaces/%s/deployments' % (self.__host, workspace_id)
+    def create_deployment(
+        self, workspace_id: str, deployment: CreateDeployment
+    ) -> Deployment:
+        url = "%s/workspaces/%s/deployments" % (self.__host, workspace_id)
         data = deployment.to_request_body()
 
         deployment_response = requests.post(
-            url, json=data, auth=(self.__access_key, self.__secret_key))
+            url, json=data, auth=(self.__access_key, self.__secret_key)
+        )
         if not self.__request_is_successful(deployment_response):
-            raise Exception('Failed to create the deployment: %s' % str(deployment_response.json()))
+            raise Exception(
+                "Failed to create the deployment: %s" % str(deployment_response.json())
+            )
 
-        deployment = parse_obj_as(
-            Deployment, deployment_response.json())
+        deployment = parse_obj_as(Deployment, deployment_response.json())
 
         return deployment
 
-    def update_deployment(self, workspace_id: str, update: UpdateDeployment) -> Deployment:
-        url = '%s/workspaces/%s/deployments/%s' % (self.__host,
-                                                   workspace_id,
-                                                   update.deployment_id)
+    def update_deployment(
+        self, workspace_id: str, update: UpdateDeployment
+    ) -> Deployment:
+        url = "%s/workspaces/%s/deployments/%s" % (
+            self.__host,
+            workspace_id,
+            update.deployment_id,
+        )
         data = update.to_request_body()
 
         deployment_response = requests.patch(
-            url, json=data, auth=(self.__access_key, self.__secret_key))
+            url, json=data, auth=(self.__access_key, self.__secret_key)
+        )
         if not self.__request_is_successful(deployment_response):
-            raise Exception('Failed to update the deployment: %s' % str(deployment_response.json()))
+            raise Exception(
+                "Failed to update the deployment: %s" % str(deployment_response.json())
+            )
 
-        deployment = parse_obj_as(
-            Deployment, deployment_response.json())
+        deployment = parse_obj_as(Deployment, deployment_response.json())
 
         return deployment
 
-    def update_deployment_metadata(self, workspace_id: str,
-                                   update: UpdateDeploymentMetadata) -> Deployment:
-        url = '%s/workspaces/%s/deployments/%s/metadata' % (self.__host,
-                                                            workspace_id,
-                                                            update.deployment_id)
+    def update_deployment_metadata(
+        self, workspace_id: str, update: UpdateDeploymentMetadata
+    ) -> Deployment:
+        url = "%s/workspaces/%s/deployments/%s/metadata" % (
+            self.__host,
+            workspace_id,
+            update.deployment_id,
+        )
         data = update.to_request_body()
 
         deployment_response = requests.patch(
-            url, json=data, auth=(self.__access_key, self.__secret_key))
+            url, json=data, auth=(self.__access_key, self.__secret_key)
+        )
         if not self.__request_is_successful(deployment_response):
-            raise Exception('Failed to update the deployment: %s' % str(deployment_response.json()))
+            raise Exception(
+                "Failed to update the deployment: %s" % str(deployment_response.json())
+            )
 
-        deployment = parse_obj_as(
-            Deployment, deployment_response.json()['data'])
+        deployment = parse_obj_as(Deployment, deployment_response.json()["data"])
 
         return deployment
 
     def get_workspace(self, workspace_id: str) -> Workspace:
-        url = '%s/workspaces/%s' % (self.__host, workspace_id)
+        url = "%s/workspaces/%s" % (self.__host, workspace_id)
 
         workspace_response = requests.get(
-            url, auth=(self.__access_key, self.__secret_key))
+            url, auth=(self.__access_key, self.__secret_key)
+        )
         if not self.__request_is_successful(workspace_response):
-            raise Exception('Workspace does not exist.')
+            raise Exception("Workspace does not exist.")
 
         workspace = parse_obj_as(Workspace, workspace_response.json())
 
         return workspace
 
     def upload_blob_file(
-            self, local_file_path: str, relative_folder_path: str, workspace_id: str,
-            repository_id: str, uuid: str) -> str:
-        url = '%s/workspaces/%s/repositories/%s/upload' % (
-            self.__host, workspace_id, repository_id)
+        self,
+        local_file_path: str,
+        relative_folder_path: str,
+        workspace_id: str,
+        repository_id: str,
+        uuid: str,
+    ) -> str:
+        url = "%s/workspaces/%s/repositories/%s/upload" % (
+            self.__host,
+            workspace_id,
+            repository_id,
+        )
         params = {
-            'commitSha': uuid,
-            'folderPath': relative_folder_path,
+            "commitSha": uuid,
+            "folderPath": relative_folder_path,
         }
-        files = {'file': open(local_file_path, 'rb')}
-        r = requests.post(url, files=files, params=params,
-                          auth=(self.__access_key, self.__secret_key))
+        files = {"file": open(local_file_path, "rb")}
+        r = requests.post(
+            url, files=files, params=params, auth=(self.__access_key, self.__secret_key)
+        )
 
-        blob_storage_path = r.json()['data']['referencePath']
+        blob_storage_path = r.json()["data"]["referencePath"]
         return blob_storage_path
 
-    def predict(self, workspace_id: str, deployment_id: str,
-                request_body: dict) -> V1Prediction or V2Prediction:
-        url = '%s/workspaces/%s/deployments/%s/predict' % (
-            self.__host, workspace_id, deployment_id)
+    def predict(
+        self, workspace_id: str, deployment_id: str, request_body: dict
+    ) -> V1Prediction or V2Prediction:
+        url = "%s/workspaces/%s/deployments/%s/predict" % (
+            self.__host,
+            workspace_id,
+            deployment_id,
+        )
 
         prediction_response = requests.post(
-            url, json=request_body, headers=self.__get_auth_header(AuthType.ALL))
+            url, json=request_body, headers=self.__get_auth_header(AuthType.ALL)
+        )
 
         if not self.__request_is_successful(prediction_response):
-            raise Exception('Failed to call predictive model.')
+            raise Exception("Failed to call predictive model.")
         prediction = self.__parse_prediction(prediction_response)
         return prediction
 
-    def explain(self, workspace_id: str, deployment_id: str, request_body: dict,
-                image: bool = False) -> object:
-        url = '%s/workspaces/%s/deployments/%s/explain' % (
-            self.__host, workspace_id, deployment_id)
+    def explain(
+        self,
+        workspace_id: str,
+        deployment_id: str,
+        request_body: dict,
+        image: bool = False,
+    ) -> object:
+        url = "%s/workspaces/%s/deployments/%s/explain" % (
+            self.__host,
+            workspace_id,
+            deployment_id,
+        )
         params = {
-            'image': str(image).lower(),
+            "image": str(image).lower(),
         }
 
         explanation_response = requests.post(
-            url, json=request_body, params=params, headers=self.__get_auth_header(AuthType.ALL))
+            url,
+            json=request_body,
+            params=params,
+            headers=self.__get_auth_header(AuthType.ALL),
+        )
 
         if not self.__request_is_successful(explanation_response):
-            raise Exception('Failed to call explainer model.')
+            raise Exception("Failed to call explainer model.")
         explanation = explanation_response.json()
         return explanation
 
-    def getOnePredictionLog(self, workspace_id: str, deployment_id: str, request_log_id: str,
-                            prediction_log_id: str) -> PredictionLog:
-        url = '%s/workspaces/%s/deployments/%s/requestLogs/%s/predictionLogs/%s' % (
-            self.__host, workspace_id, deployment_id, request_log_id, prediction_log_id)
+    def getOnePredictionLog(
+        self,
+        workspace_id: str,
+        deployment_id: str,
+        request_log_id: str,
+        prediction_log_id: str,
+    ) -> PredictionLog:
+        url = "%s/workspaces/%s/deployments/%s/requestLogs/%s/predictionLogs/%s" % (
+            self.__host,
+            workspace_id,
+            deployment_id,
+            request_log_id,
+            prediction_log_id,
+        )
 
-        log_response = requests.get(
-            url, headers=self.__get_auth_header(AuthType.ALL))
+        log_response = requests.get(url, headers=self.__get_auth_header(AuthType.ALL))
 
         if not self.__request_is_successful(log_response):
-            raise Exception('Failed to get log %s.' % prediction_log_id)
+            raise Exception("Failed to get log %s." % prediction_log_id)
 
         log = parse_obj_as(PredictionLog, log_response.json())
         return log
 
-    def getPredictionLogs(self, workspace_id: str, deployment_id: str) -> PredictionLogs:
-        url = '%s/workspaces/%s/deployments/%s/predictionLogs' % (self.__host,
-                                                                  workspace_id,
-                                                                  deployment_id)
+    def getPredictionLogs(
+        self, workspace_id: str, deployment_id: str
+    ) -> List[PredictionLog]:
+        url = "%s/workspaces/%s/deployments/%s/predictionLogs" % (
+            self.__host,
+            workspace_id,
+            deployment_id,
+        )
 
-        logs_response = requests.get(
-            url, headers=self.__get_auth_header(AuthType.ALL))
+        logs_response = requests.get(url, headers=self.__get_auth_header(AuthType.ALL))
 
         if not self.__request_is_successful(logs_response):
-            raise Exception('Failed to get logs.')
-        logs = parse_obj_as(PredictionLogs, logs_response.json())
+            raise Exception("Failed to get logs.")
+        logs = parse_obj_as(List[PredictionLog], logs_response.json())
         return logs
 
-    def getRequestLogs(self, workspace_id: str, deployment_id: str) -> RequestLogs:
-        url = '%s/workspaces/%s/deployments/%s/requestLogs' % (self.__host,
-                                                               workspace_id,
-                                                               deployment_id)
+    def getRequestLogs(self, workspace_id: str, deployment_id: str) -> List[RequestLog]:
+        url = "%s/workspaces/%s/deployments/%s/requestLogs" % (
+            self.__host,
+            workspace_id,
+            deployment_id,
+        )
 
-        logs_response = requests.get(
-            url, headers=self.__get_auth_header(AuthType.ALL))
+        logs_response = requests.get(url, headers=self.__get_auth_header(AuthType.ALL))
 
         if not self.__request_is_successful(logs_response):
-            raise Exception('Failed to get logs.')
-        logs = parse_obj_as(RequestLogs, logs_response.json())
+            raise Exception("Failed to get logs.")
+        logs = parse_obj_as(List[RequestLog], logs_response.json())
         return logs
 
-    def evaluate(self, workspace_id: str, deployment_id: str, request_log_id: str, prediction_log_id: str,
-                 evaluation_input: dict) -> None:
-        url = "%s/workspaces/%s/deployments/%s/requestLogs/%s/predictionLogs/%s/evaluations" % (
-            self.__host, workspace_id, deployment_id, request_log_id, prediction_log_id)
-
-        if ((evaluation_input['result'] == 0) and ('value' in evaluation_input)):
-            raise Exception('An evaluation value can not be provided when confirming the inference.')
+    def evaluate(
+        self,
+        workspace_id: str,
+        deployment_id: str,
+        request_log_id: str,
+        prediction_log_id: str,
+        evaluation_input: dict,
+    ) -> None:
+        url = (
+            "%s/workspaces/%s/deployments/%s/requestLogs/%s/predictionLogs/%s/evaluations"
+            % (
+                self.__host,
+                workspace_id,
+                deployment_id,
+                request_log_id,
+                prediction_log_id,
+            )
+        )
+
+        if (evaluation_input["result"] == 0) and ("value" in evaluation_input):
+            raise Exception(
+                "An evaluation value can not be provided when confirming the inference."
+            )
 
         evaluation_response = requests.post(
-            url, json=evaluation_input,
-            headers=self.__get_auth_header(AuthType.TOKEN))
+            url, json=evaluation_input, headers=self.__get_auth_header(AuthType.TOKEN)
+        )
         if not self.__request_is_successful(evaluation_response):
             if evaluation_response.status_code == 409:
-                raise Exception('Log has already been evaluated.')
+                raise Exception("Log has already been evaluated.")
             elif evaluation_response.status_code == 401:
-                raise Exception('No permission to perform this action.')
+                raise Exception("No permission to perform this action.")
             else:
-                raise Exception('Failed to request evaluation.')
+                raise Exception("Failed to request evaluation.")
 
-    def actuals(self, workspace_id: str, deployment_id: str, actuals_input: dict) -> None:
+    def actuals(
+        self, workspace_id: str, deployment_id: str, actuals_input: dict
+    ) -> None:
         url = "%s/workspaces/%s/deployments/%s/actuals" % (
-            self.__host, workspace_id, deployment_id)
+            self.__host,
+            workspace_id,
+            deployment_id,
+        )
 
         actuals_response = requests.put(
-            url, json=actuals_input,
-            headers=self.__get_auth_header(AuthType.TOKEN))
+            url, json=actuals_input, headers=self.__get_auth_header(AuthType.TOKEN)
+        )
         if not self.__request_is_successful(actuals_response):
             if actuals_response.status_code == 401:
-                raise Exception('No permission to perform this action.')
+                raise Exception("No permission to perform this action.")
             else:
-                raise Exception('Failed to submit actuals.')
+                raise Exception("Failed to submit actuals.")
 
     def __keys_are_valid(self) -> bool:
-        host_for_testing = '%s/workspaces' % self.__host
+        host_for_testing = "%s/workspaces" % self.__host
 
         workspaces_response = requests.get(
-            host_for_testing, auth=(self.__access_key, self.__secret_key))
+            host_for_testing, auth=(self.__access_key, self.__secret_key)
+        )
         if self.__request_is_successful(workspaces_response):
             return True
         return False
 
     def __token_is_valid(self, workspace_id, deployment_id) -> bool:
-        host_for_testing = '%s/workspaces/%s/deployments/%s/requestLogs' % (
-            self.__host, workspace_id, deployment_id)
-        headers = {'Authorization': 'Bearer ' + self.__token}
-        logs_response = requests.get(
-            host_for_testing, headers=headers)
+        host_for_testing = "%s/workspaces/%s/deployments/%s/requestLogs" % (
+            self.__host,
+            workspace_id,
+            deployment_id,
+        )
+        headers = {"Authorization": "Bearer " + self.__token}
+        logs_response = requests.get(host_for_testing, headers=headers)
         if self.__request_is_successful(logs_response):
             return True
         return False
 
     def __request_is_successful(self, request: requests.Response) -> bool:
-        if str(request.status_code)[0] == '2':
+        if str(request.status_code)[0] == "2":
             return True
         return False
 
-    def __check_prediction_version(self, prediction_response: dict) -> PredictionVersion:
+    def __check_prediction_version(
+        self, prediction_response: dict
+    ) -> PredictionVersion:
         if len(prediction_response.json()) > 1:
             return PredictionVersion.V2
         else:
             return PredictionVersion.V1
 
-    def __parse_prediction(self, prediction_response: dict) -> V1Prediction or V2Prediction:
+    def __parse_prediction(
+        self, prediction_response: dict
+    ) -> V1Prediction or V2Prediction:
         if self.__check_prediction_version(prediction_response) == PredictionVersion.V1:
-            prediction = parse_obj_as(
-                V1Prediction, prediction_response.json())
+            prediction = parse_obj_as(V1Prediction, prediction_response.json())
         else:
-            prediction = parse_obj_as(
-                V2Prediction, prediction_response.json())
+            prediction = parse_obj_as(V2Prediction, prediction_response.json())
         return prediction
 
     def __get_auth_header(self, supported_auth: AuthType):
-        if (self.__access_key and self.__secret_key) and \
-                (supported_auth == AuthType.BASIC or supported_auth == AuthType.ALL):
+        if (self.__access_key and self.__secret_key) and (
+            supported_auth == AuthType.BASIC or supported_auth == AuthType.ALL
+        ):
             credentials = self.__access_key + ":" + self.__secret_key
             b64Val = base64.b64encode(credentials.encode()).decode()
-            header = {'Authorization': 'Basic %s' % b64Val}
-        elif (self.__token) and \
-                (supported_auth == AuthType.TOKEN or supported_auth == AuthType.ALL):
-            header = {'Authorization': 'Bearer ' + self.__token}
-        elif (self.__access_key and self.__secret_key) and \
-                not (supported_auth == AuthType.BASIC or supported_auth == AuthType.ALL):
-            raise Exception('This function currently does not support Basic authentication.')
+            header = {"Authorization": "Basic %s" % b64Val}
+        elif (self.__token) and (
+            supported_auth == AuthType.TOKEN or supported_auth == AuthType.ALL
+        ):
+            header = {"Authorization": "Bearer " + self.__token}
+        elif (self.__access_key and self.__secret_key) and not (
+            supported_auth == AuthType.BASIC or supported_auth == AuthType.ALL
+        ):
+            raise Exception(
+                "This function currently does not support Basic authentication."
+            )
         else:
-            raise Exception('This function currently does not support Token authentication.')
+            raise Exception(
+                "This function currently does not support Token authentication."
+            )
 
         return header
```

### Comparing `deeploy-0.5.1/deeploy/services/explainers/alibi.py` & `deeploy-1.0.0/deeploy/services/explainers/alibi.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,27 +12,31 @@
 class AlibiExplainer(BaseExplainer):
 
     __alibi_explainer: Explainer
 
     def __init__(self, explainer_object: Any) -> None:
 
         if not issubclass(type(explainer_object), Explainer):
-            raise Exception('Not a valid Alibi class')
+            raise Exception("Not a valid Alibi class")
 
         self.__alibi_explainer = explainer_object
         return
 
     def save(self, local_folder_path: str) -> None:
-        with open(join(local_folder_path, 'explainer.dill'), 'wb') as f:
+        with open(join(local_folder_path, "explainer.dill"), "wb") as f:
             dill.dump(self.__alibi_explainer, f)
         return
 
     def get_explainer_type(self) -> ExplainerType:
-        base_classes = list(map(lambda x: x.__module__ + '.' +
-                                x.__name__, inspect.getmro(type(self.__alibi_explainer))))
+        base_classes = list(
+            map(
+                lambda x: x.__module__ + "." + x.__name__,
+                inspect.getmro(type(self.__alibi_explainer)),
+            )
+        )
 
-        if 'alibi.explainers.anchor_text.AnchorText' in base_classes:
+        if "alibi.explainers.anchor_text.AnchorText" in base_classes:
             return ExplainerType.ANCHOR_TEXT
-        if 'alibi.explainers.anchor_image.AnchorImage' in base_classes:
+        if "alibi.explainers.anchor_image.AnchorImage" in base_classes:
             return ExplainerType.ANCHOR_IMAGES
-        if 'alibi.explainers.anchor_tabular.AnchorTabular' in base_classes:
+        if "alibi.explainers.anchor_tabular.AnchorTabular" in base_classes:
             return ExplainerType.ANCHOR_TABULAR
```

### Comparing `deeploy-0.5.1/deeploy/services/explainers/shap.py` & `deeploy-1.0.0/deeploy/services/explainers/shap.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 class SHAPExplainer(BaseExplainer):
 
     __shap_explainer: Explainer
 
     def __init__(self, explainer_object: Any) -> None:
 
         if not issubclass(type(explainer_object), Explainer):
-            raise Exception('Not a valid SHAP class')
+            raise Exception("Not a valid SHAP class")
 
         self.__shap_explainer = explainer_object
         return
 
     def save(self, local_folder_path: str) -> None:
-        with open(join(local_folder_path, 'explainer.dill'), 'wb') as f:
+        with open(join(local_folder_path, "explainer.dill"), "wb") as f:
             dill.dump(self.__shap_explainer, f)
         return
 
     def get_explainer_type(self) -> ExplainerType:
         return ExplainerType.SHAP_KERNEL
```

### Comparing `deeploy-0.5.1/deeploy/services/git_service.py` & `deeploy-1.0.0/deeploy/services/git_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,27 @@
     A class for interacting with a local Git project
     """
 
     repository: Repo
     remote: Remote
 
     def __init__(self, local_repository_path: str, branch_name: str = None) -> None:
-        """Initialise the Git client
-        """
+        """Initialise the Git client"""
         # TODO: branch name
         self.repository = Repo(local_repository_path)
         self.branch = self.repository.active_branch
-        self.remote = self.repository.remote('origin')
+        self.remote = self.repository.remote("origin")
 
         if not self.__is_valid_git_project():
-            raise Exception('Not a valid git project')
+            raise Exception("Not a valid git project")
 
         return
 
     def __is_valid_git_project(self) -> bool:
-        """Check if the supplied repository is valid
-        """
+        """Check if the supplied repository is valid"""
         try:
             assert not self.repository.bare
         except Exception:
             return False
 
         return True
 
@@ -41,37 +39,37 @@
             represents the relative path to the folder from the root of
             the git directory
         """
         self.repository.index.add([relative_folder_path])
         return
 
     def delete_folder_from_staging(self, relative_folder_path: str) -> None:
-        self.repository.index.remove([relative_folder_path], False, r=True, ignore_unmatch=True)
+        self.repository.index.remove(
+            [relative_folder_path], False, r=True, ignore_unmatch=True
+        )
         return
 
     def commit(self, commit_message: str) -> str:
         """Create a new commit on the current branch
 
         Parameters
         ----------
           commit_message: str
             representing the commit message
         """
         self.repository.index.commit(commit_message)
         return self.repository.head.commit.hexsha
 
     def pull(self) -> None:
-        """Pull from the default remote repository
-        """
+        """Pull from the default remote repository"""
         self.remote.pull(self.branch, ff_only=True)
         return
 
     def push(self) -> None:
-        """Push to the default remote repository
-        """
+        """Push to the default remote repository"""
         self.remote.push()
         return
 
     def get_remote_url(self) -> str:
         return self.remote.url
 
     def get_current_branch_name(self) -> str:
```

### Comparing `deeploy-0.5.1/deeploy/services/model_wrapper.py` & `deeploy-1.0.0/deeploy/services/model_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,69 +20,83 @@
         return
 
     def get_model_type(self) -> ModelType:
         return self.__model_helper.get_model_type()
 
     def __get_model_type(self, model_object: Any) -> ModelType:
 
-        base_classes = list(map(lambda x: x.__module__ + '.' +
-                                x.__name__, inspect.getmro(type(model_object))))
+        base_classes = list(
+            map(
+                lambda x: x.__module__ + "." + x.__name__,
+                inspect.getmro(type(model_object)),
+            )
+        )
 
         if self.__is_sklearn(base_classes):
             return ModelType.SKLEARN
         if self.__is_xgboost(base_classes):
             return ModelType.XGBOOST
         if self.__is_pytorch(base_classes):
             return ModelType.PYTORCH
         if self.__is_tensorflow(base_classes):
             return ModelType.TENSORFLOW
         if self.__is_triton(base_classes):
             return ModelType.TRITON
         if self.__is_onnx(base_classes):
             return ModelType.ONNX
 
-        raise NotImplementedError(
-            'This model type is not implemented by Deeploy')
+        raise NotImplementedError("This model type is not implemented by Deeploy")
 
     def __get_model_helper(self, model_object, **kwargs) -> BaseModel:
 
         model_type = self.__get_model_type(model_object)
 
         # only import the helper class when it is needed
         if model_type == ModelType.SKLEARN:
             from deeploy.services.models.sklearn import SKLearnModel
+
             return SKLearnModel(model_object, **kwargs)
         if model_type == ModelType.XGBOOST:
             from deeploy.services.models.xgboost import XGBoostModel
+
             return XGBoostModel(model_object, **kwargs)
         if model_type == ModelType.PYTORCH:
             from deeploy.services.models.pytorch import PyTorchModel
+
             return PyTorchModel(model_object, **kwargs)
         if model_type == ModelType.TENSORFLOW:
             from deeploy.services.models.tensorflow import TensorFlowModel
+
             return TensorFlowModel(model_object, **kwargs)
         if model_type == ModelType.TRITON:
             from deeploy.services.models.triton import TritonModel
+
             return TritonModel(model_object, **kwargs)
         if model_type == ModelType.ONNX:
             from deeploy.services.models.onnx import ONNXModel
+
             return ONNXModel(model_object, **kwargs)
 
     def __is_sklearn(self, base_classes: List[str]) -> bool:
-        return 'sklearn.base.BaseEstimator' in base_classes and \
-               'xgboost.sklearn.XGBModel' not in base_classes
+        return (
+            "sklearn.base.BaseEstimator" in base_classes
+            and "xgboost.sklearn.XGBModel" not in base_classes
+        )
 
     def __is_xgboost(self, base_classes: List[str]) -> bool:
-        return 'xgboost.sklearn.XGBModel' in base_classes or 'xgboost.core.Booster' in base_classes
+        return (
+            "xgboost.sklearn.XGBModel" in base_classes
+            or "xgboost.core.Booster" in base_classes
+        )
 
     def __is_pytorch(self, base_classes: List[str]) -> bool:
-        return 'torch.nn.modules.module.Module' in base_classes
+        return "torch.nn.modules.module.Module" in base_classes
 
     def __is_tensorflow(self, base_classes: List[str]) -> bool:
-        return 'tensorflow.python.module.module.Module' in base_classes
+        return "tensorflow.python.module.module.Module" in base_classes
 
     def __is_onnx(self, model: Any) -> bool:
         # TODO
         return False
 
     def __is_triton(self, model: Any) -> bool:
         # TODO
```

### Comparing `deeploy-0.5.1/deeploy/services/models/pytorch.py` & `deeploy-1.0.0/deeploy/services/models/pytorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,73 +13,87 @@
 
 class PyTorchModel(BaseModel):
 
     __pytorch_model: Module
     __model_file_path: str
     __handler_file_path: str = None
 
-    def __init__(self, model_object: Any, pytorch_model_file_path: str,
-                 pytorch_torchserve_handler_name: str = 'image_classifier', **kwargs) -> None:
+    def __init__(
+        self,
+        model_object: Any,
+        pytorch_model_file_path: str,
+        pytorch_torchserve_handler_name: str = "image_classifier",
+        **kwargs
+    ) -> None:
 
         if not issubclass(type(model_object), Module):
-            raise Exception('Not a valid PyTorch class')
+            raise Exception("Not a valid PyTorch class")
 
         if not exists(pytorch_model_file_path):
-            raise Exception('The Pytorch model file does not exist')
+            raise Exception("The Pytorch model file does not exist")
 
-        if not (pytorch_model_file_path.endswith('.py') or
-                pytorch_model_file_path.endswith('.ipynb')):
+        if not (
+            pytorch_model_file_path.endswith(".py")
+            or pytorch_model_file_path.endswith(".ipynb")
+        ):
             raise Exception(
-                'The Pytorch model file is not a supported file type. Use .py or .ipynb')
+                "The Pytorch model file is not a supported file type. Use .py or .ipynb"
+            )
 
         self.__pytorch_model = model_object
         self.__model_file_path = pytorch_model_file_path
         self.__handler_name = pytorch_torchserve_handler_name
         return
 
     def save(self, local_folder_path: str) -> None:
-        serialized_model_path = join(os.getcwd(), 'model.pt')
-        mar_folder_path = join(local_folder_path, 'model-store')
+        serialized_model_path = join(os.getcwd(), "model.pt")
+        mar_folder_path = join(local_folder_path, "model-store")
         save(self.__pytorch_model.state_dict(), serialized_model_path)
 
-        mar_command = "torch-model-archiver --model-name model --version 1.0 --serialized-file %s \
-            --export-path %s" % (serialized_model_path, mar_folder_path)
+        mar_command = (
+            "torch-model-archiver --model-name model --version 1.0 --serialized-file %s \
+            --export-path %s"
+            % (serialized_model_path, mar_folder_path)
+        )
 
-        if self.__model_file_path.endswith('.py'):
+        if self.__model_file_path.endswith(".py"):
             mar_command += " --model-file %s" % self.__model_file_path
 
-        elif self.__model_file_path.endswith('.ipynb'):
-            convert_command = "ipython nbconvert --to script %s" % self.__model_file_path
+        elif self.__model_file_path.endswith(".ipynb"):
+            convert_command = (
+                "ipython nbconvert --to script %s" % self.__model_file_path
+            )
 
             ipy_process = subprocess.Popen(
-                convert_command.split(), stdout=subprocess.PIPE)
+                convert_command.split(), stdout=subprocess.PIPE
+            )
             _, error = ipy_process.communicate()
             if error:
                 raise Exception(error)
 
             mar_command += " --model-file %s" % self.__model_file_path.replace(
-                '.ipynb', '.py')
+                ".ipynb", ".py"
+            )
 
         mar_command += " --handler %s" % self.__handler_name
 
         if not os.path.exists(mar_folder_path):
             os.makedirs(mar_folder_path)
 
-        mar_process = subprocess.Popen(
-            mar_command.split(), stdout=subprocess.PIPE)
+        mar_process = subprocess.Popen(mar_command.split(), stdout=subprocess.PIPE)
         _, error = mar_process.communicate()
         if error:
             raise Exception(error)
         mar_process.wait()
 
-        config_folder_path = join(local_folder_path, 'config')
+        config_folder_path = join(local_folder_path, "config")
         if not os.path.exists(config_folder_path):
             os.makedirs(config_folder_path)
 
-        config_file_path = join(config_folder_path, 'config.properties')
+        config_file_path = join(config_folder_path, "config.properties")
         with open(config_file_path, "w+") as config_file:
             config_file.write(PYTORCH_CONFIG_FILE)
 
         return
 
     def get_model_type(self) -> ModelType:
         return ModelType.PYTORCH
```

### Comparing `deeploy-0.5.1/deeploy/services/models/sklearn.py` & `deeploy-1.0.0/deeploy/services/models/sklearn.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 class SKLearnModel(BaseModel):
 
     __sklearn_model: BaseEstimator
 
     def __init__(self, model_object: Any, **kwargs) -> None:
 
         if not issubclass(type(model_object), BaseEstimator):
-            raise Exception('Not a valid SKLearn class')
+            raise Exception("Not a valid SKLearn class")
 
         self.__sklearn_model = model_object
         return
 
     def save(self, local_folder_path: str) -> None:
-        dump(self.__sklearn_model, join(local_folder_path, 'model.joblib'))
+        dump(self.__sklearn_model, join(local_folder_path, "model.joblib"))
         return
 
     def get_model_type(self) -> ModelType:
         return ModelType.SKLEARN
```

### Comparing `deeploy-0.5.1/deeploy/services/models/tensorflow.py` & `deeploy-1.0.0/deeploy/services/models/tensorflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 class TensorFlowModel(BaseModel):
 
     __tensorflow_model: Module
 
     def __init__(self, model_object: Any, **kwargs) -> None:
 
         if not issubclass(type(model_object), Module):
-            raise Exception('Not a valid TensorFlow class')
+            raise Exception("Not a valid TensorFlow class")
 
         self.__tensorflow_model = model_object
         return
 
     def save(self, local_folder_path: str) -> None:
-        self.__tensorflow_model.save(join(local_folder_path, '1'))
+        self.__tensorflow_model.save(join(local_folder_path, "1"))
         return
 
     def get_model_type(self) -> ModelType:
         return ModelType.TENSORFLOW
```

### Comparing `deeploy-0.5.1/deeploy/services/models/xgboost.py` & `deeploy-1.0.0/deeploy/services/models/xgboost.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 
 class XGBoostModel(BaseModel):
 
     __xgboost_model: XGBClassifier
 
     def __init__(self, model_object: Any, **kwargs) -> None:
 
-        if not issubclass(type(model_object), XGBClassifier) and \
-                not issubclass(type(model_object), Booster):
-            raise Exception('Not a valid XGBoost class')
+        if not issubclass(type(model_object), XGBClassifier) and not issubclass(
+            type(model_object), Booster
+        ):
+            raise Exception("Not a valid XGBoost class")
 
         self.__xgboost_model = model_object
         return
 
     def save(self, local_folder_path: str) -> None:
-        self.__xgboost_model.save_model(join(local_folder_path, 'model.bst'))
+        self.__xgboost_model.save_model(join(local_folder_path, "model.bst"))
         return
 
     def get_model_type(self) -> ModelType:
         return ModelType.XGBOOST
```

### Comparing `deeploy-0.5.1/deeploy.egg-info/PKG-INFO` & `deeploy-1.0.0/deeploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeploy
-Version: 0.5.1
+Version: 1.0.0
 Summary: The official Deeploy client for Python
 Home-page: https://gitlab.com/deeploy-ml/deeploy-python-client
 Author: Tim Kleinloog
 Author-email: opensource@deeploy.ml
 License: UNKNOWN
 Project-URL: Documentation, https://deeploy-ml.gitlab.io/deeploy-python-client/
 Project-URL: Deeploy website, https://deeploy.ml
```

### Comparing `deeploy-0.5.1/deeploy.egg-info/SOURCES.txt` & `deeploy-1.0.0/deeploy.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,27 +24,27 @@
 deeploy/models/create_deployment.py
 deeploy/models/create_version.py
 deeploy/models/deploy_options.py
 deeploy/models/deployment.py
 deeploy/models/model_reference_json.py
 deeploy/models/prediction.py
 deeploy/models/prediction_log.py
-deeploy/models/prediction_logs.py
 deeploy/models/repository.py
 deeploy/models/update_deployment.py
 deeploy/models/update_options.py
 deeploy/models/workspace.py
 deeploy/services/__init__.py
 deeploy/services/deeploy_service.py
 deeploy/services/explainer_wrapper.py
 deeploy/services/git_service.py
 deeploy/services/model_wrapper.py
 deeploy/services/explainers/__init__.py
 deeploy/services/explainers/alibi.py
 deeploy/services/explainers/base_explainer.py
+deeploy/services/explainers/omni_tabular.py
 deeploy/services/explainers/shap.py
 deeploy/services/models/__init__.py
 deeploy/services/models/base_model.py
 deeploy/services/models/onnx.py
 deeploy/services/models/pytorch.py
 deeploy/services/models/sklearn.py
 deeploy/services/models/tensorflow.py
```

### Comparing `deeploy-0.5.1/setup.py` & `deeploy-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import re
 import setuptools
 
 with open("docs/pypi.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 VERSIONFILE = "deeploy/_version.py"
@@ -11,21 +10,21 @@
 mo = re.search(VERSIONRE, version_string, re.M)
 if mo:
     version = mo.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 setuptools.setup(
-    name='deeploy',
+    name="deeploy",
     version=version,
-    description='The official Deeploy client for Python',
+    description="The official Deeploy client for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author='Tim Kleinloog',
-    author_email='opensource@deeploy.ml',
+    author="Tim Kleinloog",
+    author_email="opensource@deeploy.ml",
     packages=setuptools.find_packages(),
     url="https://gitlab.com/deeploy-ml/deeploy-python-client",
     project_urls={
         "Documentation": "https://deeploy-ml.gitlab.io/deeploy-python-client/",
         "Deeploy website": "https://deeploy.ml",
     },
     install_requires=[
@@ -39,9 +38,9 @@
         "torch-model-archiver==0.3.1",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
 )
```

