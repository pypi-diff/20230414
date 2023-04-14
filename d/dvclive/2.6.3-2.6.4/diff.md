# Comparing `tmp/dvclive-2.6.3.tar.gz` & `tmp/dvclive-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvclive-2.6.3.tar", last modified: Tue Apr 11 22:15:49 2023, max compression
+gzip compressed data, was "dvclive-2.6.4.tar", last modified: Fri Apr 14 17:58:46 2023, max compression
```

## Comparing `dvclive-2.6.3.tar` & `dvclive-2.6.4.tar`

### file list

```diff
@@ -1,76 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.128222 dvclive-2.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-11 22:15:38.000000 dvclive-2.6.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-11 22:15:38.000000 dvclive-2.6.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.120221 dvclive-2.6.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-11 22:15:38.000000 dvclive-2.6.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-11 22:15:38.000000 dvclive-2.6.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.120221 dvclive-2.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-11 22:15:38.000000 dvclive-2.6.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-11 22:15:38.000000 dvclive-2.6.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-11 22:15:38.000000 dvclive-2.6.3/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-11 22:15:38.000000 dvclive-2.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-11 22:15:38.000000 dvclive-2.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-11 22:15:38.000000 dvclive-2.6.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-11 22:15:38.000000 dvclive-2.6.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-11 22:15:38.000000 dvclive-2.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-11 22:15:49.128222 dvclive-2.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-11 22:15:38.000000 dvclive-2.6.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-11 22:15:38.000000 dvclive-2.6.3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-11 22:15:38.000000 dvclive-2.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-11 22:15:49.128222 dvclive-2.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 22:15:38.000000 dvclive-2.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.116222 dvclive-2.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.124222 dvclive-2.6.3/src/dvclive/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/optuna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.124222 dvclive-2.6.3/src/dvclive/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/plots/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-11 22:15:38.000000 dvclive-2.6.3/src/dvclive/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.124222 dvclive-2.6.3/src/dvclive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-11 22:15:49.000000 dvclive-2.6.3/src/dvclive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-11 22:15:49.000000 dvclive-2.6.3/src/dvclive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:15:49.000000 dvclive-2.6.3/src/dvclive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:15:48.000000 dvclive-2.6.3/src/dvclive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-11 22:15:49.000000 dvclive-2.6.3/src/dvclive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 22:15:49.000000 dvclive-2.6.3/src/dvclive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.124222 dvclive-2.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.128222 dvclive-2.6.3/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/plots/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/plots/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/plots/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_dvc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:15:49.128222 dvclive-2.6.3/tests/test_frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_frameworks/test_xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_log_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-11 22:15:38.000000 dvclive-2.6.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.105698 dvclive-2.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 17:58:33.000000 dvclive-2.6.4/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 17:58:33.000000 dvclive-2.6.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.097698 dvclive-2.6.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-14 17:58:33.000000 dvclive-2.6.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-14 17:58:33.000000 dvclive-2.6.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.097698 dvclive-2.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 17:58:33.000000 dvclive-2.6.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-14 17:58:33.000000 dvclive-2.6.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-14 17:58:33.000000 dvclive-2.6.4/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-14 17:58:33.000000 dvclive-2.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-14 17:58:33.000000 dvclive-2.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-14 17:58:33.000000 dvclive-2.6.4/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-14 17:58:33.000000 dvclive-2.6.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-14 17:58:33.000000 dvclive-2.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-14 17:58:46.105698 dvclive-2.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-14 17:58:33.000000 dvclive-2.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.097698 dvclive-2.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   321138 2023-04-14 17:58:33.000000 dvclive-2.6.4/docs/dvc_plots_diff.png
+-rw-r--r--   0 runner    (1001) docker     (123)   676021 2023-04-14 17:58:33.000000 dvclive-2.6.4/docs/studio_compare.png
+-rw-r--r--   0 runner    (1001) docker     (123)   501824 2023-04-14 17:58:33.000000 dvclive-2.6.4/docs/vscode_experiments.png
+-rw-r--r--   0 runner    (1001) docker     (123)   627561 2023-04-14 17:58:33.000000 dvclive-2.6.4/docs/vscode_plots.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-14 17:58:33.000000 dvclive-2.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-14 17:58:46.105698 dvclive-2.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 17:58:33.000000 dvclive-2.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.093698 dvclive-2.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.101698 dvclive-2.6.4/src/dvclive/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19935 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/optuna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.105698 dvclive-2.6.4/src/dvclive/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/plots/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-14 17:58:33.000000 dvclive-2.6.4/src/dvclive/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.101698 dvclive-2.6.4/src/dvclive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-14 17:58:46.000000 dvclive-2.6.4/src/dvclive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-14 17:58:46.000000 dvclive-2.6.4/src/dvclive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:58:46.000000 dvclive-2.6.4/src/dvclive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:58:45.000000 dvclive-2.6.4/src/dvclive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-14 17:58:46.000000 dvclive-2.6.4/src/dvclive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 17:58:46.000000 dvclive-2.6.4/src/dvclive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.105698 dvclive-2.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.105698 dvclive-2.6.4/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/plots/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/plots/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/plots/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_dvc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:58:46.105698 dvclive-2.6.4/tests/test_frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_frameworks/test_xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_log_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 17:58:33.000000 dvclive-2.6.4/tests/test_utils.py
```

### Comparing `dvclive-2.6.3/.cruft.json` & `dvclive-2.6.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.3/.github/dependabot.yml` & `dvclive-2.6.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.3/.github/workflows/release.yml` & `dvclive-2.6.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.3/.github/workflows/tests.yml` & `dvclive-2.6.4/.github/workflows/tests.yml`

 * *Files 16% similar despite different names*

```diff
@@ -46,18 +46,14 @@
       - name: pre-commit
         run: |
           pre-commit run --show-diff-on-failure --color=always --all-files
 
       - name: Full install
         run: pip install -e '.[dev]'
 
-      - name: pylint
-        run: |
-           python -m pylint src tests
-
       - name: mypy
         run: |
            python -m mypy --install-types --non-interactive
 
       - name: Run tests
         run: pytest -v tests --cov --cov-report=xml --cov-config=pyproject.toml
```

### Comparing `dvclive-2.6.3/.gitignore` & `dvclive-2.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.3/CODE_OF_CONDUCT.rst` & `dvclive-2.6.4/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.3/CONTRIBUTING.rst` & `dvclive-2.6.4/CONTRIBUTING.rst`

 * *Files 11% similar despite different names*

```diff
@@ -37,73 +37,70 @@
 
 Request features on the `Issue Tracker`_.
 
 
 How to set up your development environment
 ------------------------------------------
 
-You need Python 3.8+ and the following tools:
+You need Python 3.8+.
 
-- Nox_
-
-Install the package with development requirements:
+- Clone the repository:
 
 .. code:: console
 
-   $ pip install nox
+   $ git clone https://github.com/iterative/dvclive
+   $ cd dvclive
 
-.. _Nox: https://nox.thea.codes/
+- Set up a virtual environment:
 
+.. code:: console
 
-How to test the project
------------------------
+   $ python -m venv .venv
+   $ source .venv/bin/activate
 
-Run the full test suite:
+Install in editable mode:
 
 .. code:: console
 
-   $ nox
+   $ pip install -e .
 
-List the available Nox sessions:
 
-.. code:: console
-
-   $ nox --list-sessions
+How to test the project
+-----------------------
 
-You can also run a specific Nox session.
-For example, invoke the unit test suite like this:
+Run the full test suite:
 
 .. code:: console
 
-   $ nox --session=tests
+   $ pytest -v tests
 
-Unit tests are located in the ``tests`` directory,
+Tests are located in the ``tests`` directory,
 and are written using the pytest_ testing framework.
 
 .. _pytest: https://pytest.readthedocs.io/
 
 
 How to submit changes
 ---------------------
 
 Open a `pull request`_ to submit changes to this project.
 
 Your pull request needs to meet the following guidelines for acceptance:
 
-- The Nox test suite must pass without errors and warnings.
-- Include unit tests. This project maintains 100% code coverage.
+- The test suite must pass without errors and warnings.
+- Include unit tests.
 - If your changes add functionality, update the documentation accordingly.
 
 Feel free to submit early, though—we can always iterate on this.
 
-To run linting and code formatting checks, you can invoke a `lint` session in nox:
+To run linting and code formatting checks, you can use `pre-commit`:
 
 .. code:: console
 
-   $ nox -s lint
+   $ pre-commit run --all-files
 
 It is recommended to open an issue before starting work on anything.
 This will allow a chance to talk it over with the owners and validate your approach.
 
 .. _pull request: https://github.com/iterative/dvclive/pulls
 .. github-only
 .. _Code of Conduct: CODE_OF_CONDUCT.rst
```

### Comparing `dvclive-2.6.3/LICENSE` & `dvclive-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.3/setup.cfg` & `dvclive-2.6.4/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 description = Metric logger for ML projects.
 name = dvclive
-long_description = file: README.rst
-long_description_content_type = text/x-rst
+long_description = file: README.md
+long_description_content_type = text/markdown
 license = Apache-2.0
 license_files = LICENSE
 url = https://github.com/iterative/dvclive
 project_urls = 
 	Documentation = https://dvc.org/doc/dvclive
 	Source = https://github.com/iterative/dvclive
 platforms = any
@@ -43,24 +43,22 @@
 markdown = 
 	matplotlib
 tests = 
 	pytest==7.2.0
 	pytest-sugar==0.9.5
 	pytest-cov==3.0.0
 	pytest-mock==3.8.2
-	pylint==2.15.0
-	pylint-plugin-utils>=0.6
-	mypy>=1.1.1
 	%(image)s
 	%(plots)s
 	%(markdown)s
 	ipython
 dev = 
 	%(tests)s
 	%(all)s
+	mypy>=1.1.1
 mmcv = 
 	mmcv
 tf = 
 	tensorflow
 xgb = 
 	xgboost
 lgbm = 
@@ -95,23 +93,11 @@
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 where = src
 
-[flake8]
-ignore = 
-	E203
-	E266
-	W503
-	P1
-max_line_length = 88
-max-complexity = 15
-select = B,C,E,F,W,T4,B902,T,P
-show_source = true
-count = true
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dvclive-2.6.3/src/dvclive/catalyst.py` & `dvclive-2.6.4/src/dvclive/catalyst.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# ruff: noqa: ARG002
 from typing import Optional
 
 from catalyst import utils
 from catalyst.core.callback import Callback, CallbackOrder
 
 from dvclive import Live
 
@@ -11,22 +12,23 @@
         super().__init__(order=CallbackOrder.external)
         self.model_file = model_file
         self.live = live if live is not None else Live(**kwargs)
 
     def on_epoch_end(self, runner) -> None:
         for loader_key, per_loader_metrics in runner.epoch_metrics.items():
             for key, value in per_loader_metrics.items():
-                key = key.replace("/", "_")
-                self.live.log_metric(f"{loader_key}/{key}", float(value))
+                self.live.log_metric(
+                    f"{loader_key}/{key.replace('/', '_')}", float(value)
+                )
 
         if self.model_file:
             checkpoint = utils.pack_checkpoint(
                 model=runner.model,
                 criterion=runner.criterion,
                 optimizer=runner.optimizer,
                 scheduler=runner.scheduler,
             )
             utils.save_checkpoint(checkpoint, self.model_file)
         self.live.next_step()
 
-    def on_experiment_end(self, runner):  # pylint: disable=unused-argument
+    def on_experiment_end(self, runner):
         self.live.end()
```

### Comparing `dvclive-2.6.3/src/dvclive/dvc.py` & `dvclive-2.6.4/src/dvclive/dvc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=protected-access
+# ruff: noqa: SLF001
 import logging
 import os
 import random
 from io import StringIO
 from pathlib import Path
 
 from dvclive import env
@@ -143,20 +143,20 @@
 def get_random_exp_name(scm, baseline_rev):
     """
     https://github.com/iterative/dvc/blob/main/dvc/repo/experiments/utils.py
     """
     from dvc.repo.experiments.refs import ExpRefInfo
 
     # fmt: off
-    NOUNS = ('abac', 'abbs', 'aces', 'acid', 'acne', 'acre', 'acts', 'ados', 'adze', 'afro', 'agas', 'aged', 'ages', 'agio', 'agma', 'airs', 'airt', 'aits', 'akes', 'alap', 'albs', 'alga', 'ally', 'alto', 'amah', 'ambo', 'amie', 'amyl', 'ankh', 'apex', 'aqua', 'arcs', 'areg', 'aria', 'aril', 'arks', 'army', 'auks', 'aune', 'aura', 'awls', 'awns', 'axon', 'azan', 'baby', 'bade', 'bael', 'bags', 'bait', 'ball', 'banc', 'bang', 'bani', 'barb', 'bark', 'bate', 'bats', 'bawl', 'beak', 'bean', 'beep', 'belt', 'berk', 'beth', 'bias', 'bice', 'bids', 'bind', 'bise', 'bish', 'bite', 'boar', 'boat', 'body', 'boff', 'bold', 'boll', 'bolo', 'bomb', 'bond', 'book', 'boor', 'boot', 'bort', 'bosk', 'bots', 'bott', 'bout', 'bras', 'bree', 'brig', 'brio', 'buck', 'buhl', 'bump', 'bunk', 'bunt', 'buoy', 'byes', 'byte', 'cane', 'cant', 'caps', 'care', 'cart', 'cats', 'cedi', 'ceps', 'cere', 'chad', 'cham', 'chat', 'chay', 'chic', 'chin', 'chis', 'chiv', 'choc', 'chow', 'chum', 'ciao', 'cigs', 'clay', 'clip', 'clog', 'coal', 'coat', 'code', 'coed', 'cogs', 'coho', 'cole', 'cols', 'colt', 'conk', 'cons', 'cony', 'coof', 'cook', 'cool', 'coos', 'corm', 'cors', 'coth', 'cows', 'coze', 'crag', 'craw', 'cree', 'crib', 'cuds', 'cull', 'cult', 'curb', 'curn', 'curs', 'cusp', 'cuss', 'cwms', 'cyma', 'cyst', 'dabs', 'dado', 'daff', 'dais', 'daks', 'damn', 'dams', 'darg', 'dart', 'data', 'dawk', 'dawn', 'daws', 'daze', 'dean', 'debs', 'debt', 'deep', 'dees', 'dele', 'delf', 'dent', 'deys', 'dhow', 'digs', 'dirk', 'dita', 'diva', 'divs', 'doek', 'doge', 'dogs', 'dogy', 'dohs', 'doit', 'dole', 'doll', 'dolt', 'dona', 'dook', 'door', 'dops', 'doss', 'doxy', 'drab', 'drop', 'drum', 'duad', 'duct', 'duff', 'duke', 'dunk', 'dunt', 'ears', 'ease', 'eggs', 'eild', 'emeu', 'emus', 'envy', 'epha', 'eric', 'erns', 'esne', 'esse', 'ewes', 'expo', 'eyas', 'eyot', 'eyry', 'fare', 'farl', 'farm', 'feds', 'feel', 'fees', 'feme', 'fess', 'fibs', 'fids', 'fils', 'firm', 'fish', 'flab', 'flap', 'flea', 'flew', 'flex', 'flip', 'flit', 'flus', 'flux', 'foil', 'fond', 'food', 'fool', 'ford', 'fore', 'frit', 'friz', 'froe', 'funs', 'furl', 'fuss', 'fuzz', 'gaby', 'gaff', 'gale', 'gang', 'gaol', 'gape', 'gash', 'gaur', 'gaze', 'gear', 'genu', 'gest', 'geum', 'ghat', 'gigs', 'gimp', 'gird', 'girl', 'glee', 'glen', 'glia', 'glop', 'gnat', 'goad', 'goaf', 'gobs', 'gonk', 'good', 'goos', 'gore', 'gram', 'gray', 'grig', 'grip', 'grot', 'grub', 'gude', 'gula', 'gulf', 'guns', 'gust', 'gyms', 'gyro', 'hack', 'haet', 'hajj', 'hake', 'half', 'halm', 'hard', 'harl', 'hask', 'hate', "he'd", 'heck', 'heel', 'heir', 'help', 'hems', 'here', 'hill', 'hips', 'hits', 'hobo', 'hock', 'hogs', 'hold', 'holy', 'hood', 'hoot', 'hope', 'horn', 'hose', 'hour', 'hows', 'huck', 'hugs', 'huia', 'hulk', 'hull', 'hunk', 'hunt', 'huts', 'hymn', 'ibex', 'ices', 'iglu', 'impi', 'inks', 'inti', 'ions', 'iota', 'iron', 'jabs', 'jags', 'jake', 'jass', 'jato', 'jaws', 'jean', 'jeer', 'jerk', 'jest', 'jiao', 'jigs', 'jill', 'jinn', 'jird', 'jive', 'jock', 'joey', 'jogs', 'joss', 'jota', 'jots', 'juba', 'jube', 'judo', 'jump', 'junk', 'jura', 'juts', 'jynx', 'kago', 'kail', 'kaka', 'kale', 'kana', 'keek', 'keep', 'kefs', 'kegs', 'kerf', 'kern', 'keys', 'kibe', 'kick', 'kids', 'kifs', 'kill', 'kina', 'kind', 'kine', 'kite', 'kiwi', 'knap', 'knit', 'koas', 'kobs', 'kyat', 'lack', 'lahs', 'lair', 'lama', 'lamb', 'lame', 'lats', 'lava', 'lays', 'leaf', 'leak', 'leas', 'lees', 'leks', 'leno', 'libs', 'lich', 'lick', 'lien', 'lier', 'lieu', 'life', 'lift', 'limb', 'line', 'link', 'linn', 'lira', 'loft', 'loge', 'loir', 'long', 'loof', 'look', 'loot', 'lore', 'loss', 'lots', 'loup', 'love', 'luce', 'ludo', 'luke', 'lulu', 'lure', 'lush', 'magi', 'maid', 'main', 'mako', 'male', 'mana', 'many', 'mart', 'mash', 'mast', 'mate', 'math', 'mats', 'matt', 'maul', 'maya', 'mays', 'meal', 'mean', 'meed', 'mela', 'mene', 'mere', 'merk', 'mesh', 'mete', 'mice', 'milo', 'mime', 'mina', 'mine', 'mirk', 'miss', 'mobs', 'moit', 'mold', 'molt', 'mome', 'moms', 'monk', 'moot', 'mope', 'more', 'morn', 'mows', 'moxa', 'much', 'mung', 'mush', 'muss', 'myth', 'name', 'nard', 'nark', 'nave', 'navy', 'neck', 'newt', 'nibs', 'nims', 'nine', 'nock', 'noil', 'noma', 'nosh', 'nowt', 'nuke', 'oafs', 'oast', 'oats', 'obit', 'odor', 'okra', 'omer', 'oner', 'ones', 'orcs', 'ords', 'orfe', 'orle', 'ossa', 'outs', 'over', 'owls', 'pail', 'pall', 'palp', 'pams', 'pang', 'pans', 'pant', 'paps', 'pate', 'pats', 'paws', 'pear', 'peba', 'pech', 'pecs', 'peel', 'peer', 'pees', 'pein', 'peri', 'phon', 'pice', 'pita', 'pith', 'play', 'plop', 'plot', 'plow', 'plug', 'plum', 'polo', 'pomp', 'pond', 'pons', 'pony', 'poof', 'pope', 'poss', 'pots', 'pour', 'prad', 'prat', 'prep', 'prob', 'prof', 'prow', 'puck', 'puds', 'puke', 'puku', 'pump', 'puns', 'pupa', 'purl', 'pyre', 'quad', 'quay', 'quey', 'quiz', 'raid', 'rail', 'rain', 'raja', 'rale', 'rams', 'rand', 'rant', 'raps', 'rasp', 'razz', 'rede', 'reef', 'reif', 'rein', 'repp', 'rial', 'ribs', 'rick', 'rift', 'rill', 'rime', 'rims', 'ring', 'rins', 'rise', 'rite', 'rits', 'roam', 'robe', 'rods', 'roma', 'rook', 'rort', 'rotl', 'roup', 'roux', 'rube', 'rubs', 'ruby', 'rues', 'rugs', 'ruin', 'runs', 'ryas', 'sack', 'sacs', 'saga', 'sail', 'sale', 'salp', 'salt', 'sand', 'sang', 'sash', 'saut', 'says', 'scab', 'scow', 'scud', 'scup', 'scut', 'seal', 'seam', 'sech', 'seed', 'seep', 'seer', 'self', 'sena', 'send', 'sera', 'sere', 'shad', 'shah', 'sham', 'shay', 'shes', 'ship', 'shoe', 'sick', 'sida', 'sign', 'sike', 'sima', 'sine', 'sing', 'sinh', 'sink', 'sins', 'site', 'size', 'skat', 'skin', 'skip', 'skis', 'slaw', 'sled', 'slew', 'sley', 'slob', 'slue', 'slug', 'smut', 'snap', 'snib', 'snip', 'snob', 'snog', 'snot', 'snow', 'snub', 'snug', 'soft', 'soja', 'soke', 'song', 'sons', 'sook', 'sorb', 'sori', 'souk', 'soul', 'sous', 'soya', 'spit', 'stay', 'stew', 'stir', 'stob', 'stud', 'suds', 'suer', 'suit', 'sumo', 'sums', 'sups', 'suqs', 'suss', 'sway', 'syce', 'synd', 'taal', 'tach', 'taco', 'tads', 'taka', 'tale', 'tamp', 'tams', 'tang', 'tans', 'tape', 'tare', 'taro', 'tarp', 'tart', 'tass', 'taus', 'teat', 'teds', 'teff', 'tegu', 'tell', 'term', 'thar', 'thaw', 'tics', 'tier', 'tiff', 'tils', 'tilt', 'tint', 'tipi', 'tire', 'tirl', 'toby', 'tods', 'toea', 'toff', 'toga', 'toil', 'toke', 'tola', 'tole', 'tomb', 'toms', 'torc', 'tors', 'tort', 'tosh', 'tote', 'tret', 'trey', 'trio', 'trug', 'tuck', 'tugs', 'tule', 'tune', 'tuns', 'tuts', 'tyke', 'tyne', 'typo', 'ulna', 'umbo', 'unau', 'unit', 'upas', 'user', 'uvea', 'vacs', 'vane', 'vang', 'vans', 'vara', 'vase', 'veep', 'veer', 'vega', 'veil', 'vela', 'vent', 'vies', 'view', 'vina', 'vine', 'vise', 'vlei', 'volt', 'vows', 'wads', 'waft', 'wage', 'wain', 'walk', 'want', 'wart', 'wave', 'waws', 'weal', 'wean', 'weds', 'weep', 'weft', 'weir', 'weka', 'weld', 'wens', 'weys', 'whap', 'whey', 'whin', 'whit', 'whop', 'wide', 'wife', 'wind', 'wine', 'wino', 'wins', 'wire', 'wise', 'woes', 'wont', 'wool', 'work', 'worm', 'wort', 'yack', 'yank', 'yapp', 'yard', 'yate', 'yawl', 'yegg', 'yell', 'yeuk', 'yews', 'yips', 'yobs', 'yogi', 'yoke', 'yolk', 'yoni', 'zack', 'zags', 'zest', 'zhos', 'zigs', 'zila', 'zips', 'ziti', 'zoea', 'zone', 'zoon')  # noqa: E501, Q000
-    ADJECTIVES = ('about', 'above', 'abuzz', 'acerb', 'acold', 'acred', 'added', 'addle', 'adept', 'adult', 'adunc', 'adust', 'afoul', 'after', 'agape', 'agaze', 'agile', 'aging', 'agley', 'aglow', 'ahead', 'ahull', 'aided', 'alary', 'algal', 'alike', 'alive', 'alone', 'aloof', 'alpha', 'amber', 'amiss', 'amort', 'ample', 'amuck', 'angry', 'anile', 'apeak', 'apish', 'arced', 'areal', 'armed', 'aroid', 'ashen', 'aspen', 'astir', 'atilt', 'atrip', 'aulic', 'aural', 'awash', 'awful', 'awing', 'awned', 'axile', 'azoic', 'azure', 'baggy', 'baked', 'balky', 'bally', 'balmy', 'banal', 'bandy', 'bardy', 'bared', 'barer', 'barky', 'basal', 'based', 'baser', 'basic', 'batty', 'bawdy', 'beady', 'beaky', 'beamy', 'beaut', 'beefy', 'beery', 'beige', 'bendy', 'bifid', 'bijou', 'biped', 'birch', 'bitty', 'blame', 'bland', 'blank', 'blear', 'blest', 'blind', 'blond', 'blown', 'blowy', 'bluer', 'bluff', 'blunt', 'boned', 'bonny', 'boozy', 'bored', 'boric', 'bosky', 'bosom', 'bound', 'bovid', 'bowed', 'boxed', 'braky', 'brash', 'brief', 'briny', 'brisk', 'broad', 'broch', 'brood', 'brown', 'brute', 'buggy', 'bulgy', 'bumpy', 'burly', 'burnt', 'burry', 'bushy', 'busty', 'butch', 'buxom', 'cadgy', 'cagey', 'calmy', 'campy', 'canny', 'caped', 'cased', 'catty', 'cauld', 'cedar', 'cered', 'ceric', 'chary', 'cheap', 'cheek', 'chewy', 'chief', 'chill', 'chirk', 'choky', 'cissy', 'civil', 'cleft', 'coaly', 'color', 'comfy', 'comic', 'compo', 'conic', 'couth', 'coxal', 'crack', 'crank', 'crash', 'crass', 'crisp', 'cronk', 'cross', 'crude', 'cruel', 'crumb', 'cured', 'curly', 'curst', 'cushy', 'cutty', 'cynic', 'dated', 'dazed', 'dedal', 'deism', 'diazo', 'dicey', 'dingy', 'direr', 'dirty', 'dishy', 'dizzy', 'dolce', 'doped', 'dopey', 'dormy', 'dorty', 'dosed', 'dotal', 'dotty', 'dowdy', 'dowie', 'downy', 'dozen', 'drawn', 'dread', 'drear', 'dress', 'dried', 'ducky', 'duddy', 'dummy', 'dumpy', 'duple', 'dural', 'dusky', 'dusty', 'dutch', 'dying', 'eager', 'eaten', 'ebony', 'edged', 'eerie', 'eight', 'elder', 'elect', 'elfin', 'elite', 'empty', 'enate', 'enemy', 'epoxy', 'erect', 'ethic', 'every', 'extra', 'faced', 'faery', 'faint', 'famed', 'fancy', 'farci', 'fatal', 'fated', 'fatty', 'fazed', 'felon', 'fenny', 'ferny', 'fetal', 'fetid', 'fewer', 'fiery', 'fifty', 'filar', 'filmy', 'final', 'fined', 'finer', 'finny', 'fired', 'first', 'fishy', 'fixed', 'fizzy', 'flaky', 'flamy', 'flash', 'flawy', 'fleet', 'flory', 'flown', 'fluid', 'fluky', 'flush', 'focal', 'foggy', 'folio', 'forky', 'forte', 'forty', 'found', 'frail', 'frank', 'freed', 'freer', 'fresh', 'fried', 'front', 'frore', 'fuggy', 'funky', 'funny', 'furry', 'fusil', 'fussy', 'fuzzy', 'gabby', 'gamer', 'gamey', 'gamic', 'gammy', 'garni', 'gauge', 'gaunt', 'gauzy', 'gawky', 'gawsy', 'gemmy', 'genal', 'genic', 'ghast', 'gimpy', 'girly', 'glare', 'glary', 'glial', 'glued', 'gluey', 'godly', 'gooey', 'goofy', 'goosy', 'gouty', 'grade', 'grand', 'grapy', 'grave', 'gross', 'group', 'gruff', 'guest', 'gules', 'gulfy', 'gummy', 'gushy', 'gusty', 'gutsy', 'gutta', 'gypsy', 'gyral', 'hadal', 'hammy', 'handy', 'hardy', 'hasty', 'hated', 'hazel', 'heady', 'heapy', 'hefty', 'heigh', 'hempy', 'herby', 'hexed', 'hi-fi', 'hilly', 'hired', 'holey', 'honey', 'hooly', 'hoven', 'huger', 'hulky', 'humid', 'hunky', 'hyoid', 'idled', 'iliac', 'inane', 'incog', 'inert', 'inner', 'inter', 'iodic', 'ionic', 'irate', 'irony', 'itchy', 'jaggy', 'jammy', 'japan', 'jazzy', 'jerky', 'jetty', 'joint', 'jowly', 'juicy', 'jumpy', 'jural', 'kacha', 'kaput', 'kempt', 'keyed', 'kinky', 'known', 'kooky', 'kraal', 'laced', 'laigh', 'lairy', 'lamer', 'lardy', 'larky', 'lated', 'later', 'lathy', 'leady', 'leafy', 'leaky', 'leary', 'least', 'ledgy', 'leery', 'legal', 'leggy', 'lento', 'level', 'licht', 'licit', 'liege', 'light', 'liked', 'liney', 'lippy', 'lived', 'livid', 'loamy', 'loath', 'lobar', 'local', 'loony', 'loose', 'loral', 'losel', 'lousy', 'loved', 'lower', 'lowly', 'lowse', 'loyal', 'lucid', 'lucky', 'lumpy', 'lunar', 'lurid', 'lushy', 'lying', 'lyric', 'macho', 'macro', 'magic', 'major', 'malar', 'mangy', 'manky', 'manly', 'mardy', 'massy', 'mated', 'matte', 'mauve', 'mazed', 'mealy', 'meaty', 'medal', 'melic', 'mesic', 'mesne', 'messy', 'metal', 'miffy', 'milky', 'mined', 'minim', 'minor', 'minus', 'mired', 'mirky', 'misty', 'mixed', 'modal', 'model', 'moire', 'molar', 'moldy', 'moody', 'moony', 'mopey', 'moral', 'mossy', 'mothy', 'motor', 'mousy', 'moved', 'mucid', 'mucky', 'muddy', 'muggy', 'muley', 'mural', 'murky', 'mushy', 'muted', 'muzzy', 'myoid', 'naggy', 'naive', 'naked', 'named', 'nasty', 'natal', 'naval', 'nervy', 'newsy', 'nicer', 'niffy', 'nifty', 'ninth', 'nitty', 'nival', 'noble', 'nodal', 'noisy', 'non-U', 'north', 'nosed', 'noted', 'nowed', 'nubby', 'oaken', 'oared', 'oaten', 'obese', 'ocher', 'ochre', 'often', 'ohmic', 'oiled', 'olden', 'older', 'oleic', 'olive', 'optic', 'ortho', 'osmic', 'other', 'outer', 'ovoid', 'owing', 'owned', 'paced', 'pagan', 'paled', 'paler', 'pally', 'paper', 'pappy', 'parky', 'party', 'pasty', 'pavid', 'pawky', 'peaky', 'pearl', 'peart', 'peaty', 'pedal', 'peppy', 'perdu', 'perky', 'pesky', 'phony', 'piano', 'picky', 'piled', 'piney', 'pious', 'pique', 'pithy', 'platy', 'plump', 'plush', 'podgy', 'potty', 'power', 'prest', 'pricy', 'prima', 'prime', 'print', 'privy', 'prize', 'prone', 'proof', 'prosy', 'proud', 'proxy', 'pseud', 'pucka', 'pudgy', 'puffy', 'pukka', 'pupal', 'purer', 'pursy', 'pushy', 'pyoid', 'quack', 'quare', 'quasi', 'quiet', 'quits', 'rabic', 'rabid', 'radio', 'raked', 'randy', 'rapid', 'rarer', 'raspy', 'rathe', 'ratty', 'ready', 'reedy', 'reeky', 'refer', 'regal', 'riant', 'ridgy', 'right', 'riled', 'rimed', 'rindy', 'risen', 'risky', 'ritzy', 'rival', 'riven', 'robed', 'rocky', 'roily', 'roman', 'rooky', 'ropey', 'round', 'rowdy', 'ruddy', 'ruled', 'rummy', 'runic', 'runny', 'runty', 'rural', 'rusty', 'rutty', 'sable', 'salic', 'sandy', 'sappy', 'sarky', 'sassy', 'sated', 'saved', 'savvy', 'scald', 'scaly', 'scary', 'score', 'scrap', 'sedgy', 'seely', 'seral', 'sewed', 'shaky', 'sharp', 'sheen', 'shier', 'shill', 'shoal', 'shock', 'shoed', 'shore', 'short', 'shyer', 'silky', 'silly', 'silty', 'sixth', 'sixty', 'skint', 'slack', 'slant', 'sleek', 'slier', 'slimy', 'slung', 'small', 'smart', 'smoky', 'snaky', 'sneak', 'snide', 'snowy', 'snuff', 'so-so', 'soapy', 'sober', 'socko', 'solar', 'soled', 'solid', 'sonic', 'sooth', 'sooty', 'soppy', 'sorer', 'sound', 'soupy', 'spent', 'spicy', 'spiky', 'spiny', 'spiry', 'splay', 'split', 'sport', 'spumy', 'squat', 'staid', 'stiff', 'still', 'stoic', 'stone', 'stony', 'store', 'stout', 'straw', 'stray', 'strip', 'stung', 'suave', 'sudsy', 'sulfa', 'sulky', 'sunny', 'super', 'sural', 'surer', 'surfy', 'surgy', 'surly', 'swell', 'swept', 'swish', 'sworn', 'tabby', 'taboo', 'tacit', 'tacky', 'tamed', 'tamer', 'tangy', 'taped', 'tarot', 'tarry', 'tasty', 'tatty', 'taunt', 'tawie', 'teary', 'techy', 'telic', 'tenor', 'tense', 'tenth', 'tenty', 'tepid', 'terse', 'testy', 'third', 'tidal', 'tight', 'tiled', 'timid', 'tinct', 'tined', 'tippy', 'tipsy', 'tonal', 'toned', 'tonic', 'toric', 'total', 'tough', 'toxic', 'trade', 'treed', 'treen', 'trial', 'truer', 'tubal', 'tubby', 'tumid', 'tuned', 'tutti', 'twill', 'typal', 'typed', 'typic', 'umber', 'unapt', 'unbid', 'uncut', 'undue', 'undug', 'unfed', 'unfit', 'union', 'unlet', 'unmet', 'unwed', 'unwet', 'upper', 'upset', 'urban', 'utile', 'uveal', 'vagal', 'valid', 'vapid', 'varus', 'vatic', 'veiny', 'vital', 'vivid', 'vocal', 'vogie', 'volar', 'vying', 'wacky', 'wally', 'waney', 'warty', 'washy', 'waspy', 'waste', 'waugh', 'waxen', 'webby', 'wedgy', 'weeny', 'weepy', 'weest', 'weird', 'welsh', 'wersh', 'whist', 'white', 'whity', 'whole', 'wider', 'wight', 'winey', 'wired', 'wised', 'wiser', 'withy', 'wonky', 'woods', 'woozy', 'world', 'wormy', 'worse', 'worst', 'woven', 'wrath', 'wrier', 'wrong', 'wroth', 'xeric', 'yarer', 'yolky', 'young', 'yucky', 'yummy', 'zesty', 'zingy', 'zinky', 'zippy', 'zonal')  # noqa: E501, Q000
+    NOUNS = ('abac', 'abbs', 'aces', 'acid', 'acne', 'acre', 'acts', 'ados', 'adze', 'afro', 'agas', 'aged', 'ages', 'agio', 'agma', 'airs', 'airt', 'aits', 'akes', 'alap', 'albs', 'alga', 'ally', 'alto', 'amah', 'ambo', 'amie', 'amyl', 'ankh', 'apex', 'aqua', 'arcs', 'areg', 'aria', 'aril', 'arks', 'army', 'auks', 'aune', 'aura', 'awls', 'awns', 'axon', 'azan', 'baby', 'bade', 'bael', 'bags', 'bait', 'ball', 'banc', 'bang', 'bani', 'barb', 'bark', 'bate', 'bats', 'bawl', 'beak', 'bean', 'beep', 'belt', 'berk', 'beth', 'bias', 'bice', 'bids', 'bind', 'bise', 'bish', 'bite', 'boar', 'boat', 'body', 'boff', 'bold', 'boll', 'bolo', 'bomb', 'bond', 'book', 'boor', 'boot', 'bort', 'bosk', 'bots', 'bott', 'bout', 'bras', 'bree', 'brig', 'brio', 'buck', 'buhl', 'bump', 'bunk', 'bunt', 'buoy', 'byes', 'byte', 'cane', 'cant', 'caps', 'care', 'cart', 'cats', 'cedi', 'ceps', 'cere', 'chad', 'cham', 'chat', 'chay', 'chic', 'chin', 'chis', 'chiv', 'choc', 'chow', 'chum', 'ciao', 'cigs', 'clay', 'clip', 'clog', 'coal', 'coat', 'code', 'coed', 'cogs', 'coho', 'cole', 'cols', 'colt', 'conk', 'cons', 'cony', 'coof', 'cook', 'cool', 'coos', 'corm', 'cors', 'coth', 'cows', 'coze', 'crag', 'craw', 'cree', 'crib', 'cuds', 'cull', 'cult', 'curb', 'curn', 'curs', 'cusp', 'cuss', 'cwms', 'cyma', 'cyst', 'dabs', 'dado', 'daff', 'dais', 'daks', 'damn', 'dams', 'darg', 'dart', 'data', 'dawk', 'dawn', 'daws', 'daze', 'dean', 'debs', 'debt', 'deep', 'dees', 'dele', 'delf', 'dent', 'deys', 'dhow', 'digs', 'dirk', 'dita', 'diva', 'divs', 'doek', 'doge', 'dogs', 'dogy', 'dohs', 'doit', 'dole', 'doll', 'dolt', 'dona', 'dook', 'door', 'dops', 'doss', 'doxy', 'drab', 'drop', 'drum', 'duad', 'duct', 'duff', 'duke', 'dunk', 'dunt', 'ears', 'ease', 'eggs', 'eild', 'emeu', 'emus', 'envy', 'epha', 'eric', 'erns', 'esne', 'esse', 'ewes', 'expo', 'eyas', 'eyot', 'eyry', 'fare', 'farl', 'farm', 'feds', 'feel', 'fees', 'feme', 'fess', 'fibs', 'fids', 'fils', 'firm', 'fish', 'flab', 'flap', 'flea', 'flew', 'flex', 'flip', 'flit', 'flus', 'flux', 'foil', 'fond', 'food', 'fool', 'ford', 'fore', 'frit', 'friz', 'froe', 'funs', 'furl', 'fuss', 'fuzz', 'gaby', 'gaff', 'gale', 'gang', 'gaol', 'gape', 'gash', 'gaur', 'gaze', 'gear', 'genu', 'gest', 'geum', 'ghat', 'gigs', 'gimp', 'gird', 'girl', 'glee', 'glen', 'glia', 'glop', 'gnat', 'goad', 'goaf', 'gobs', 'gonk', 'good', 'goos', 'gore', 'gram', 'gray', 'grig', 'grip', 'grot', 'grub', 'gude', 'gula', 'gulf', 'guns', 'gust', 'gyms', 'gyro', 'hack', 'haet', 'hajj', 'hake', 'half', 'halm', 'hard', 'harl', 'hask', 'hate', "he'd", 'heck', 'heel', 'heir', 'help', 'hems', 'here', 'hill', 'hips', 'hits', 'hobo', 'hock', 'hogs', 'hold', 'holy', 'hood', 'hoot', 'hope', 'horn', 'hose', 'hour', 'hows', 'huck', 'hugs', 'huia', 'hulk', 'hull', 'hunk', 'hunt', 'huts', 'hymn', 'ibex', 'ices', 'iglu', 'impi', 'inks', 'inti', 'ions', 'iota', 'iron', 'jabs', 'jags', 'jake', 'jass', 'jato', 'jaws', 'jean', 'jeer', 'jerk', 'jest', 'jiao', 'jigs', 'jill', 'jinn', 'jird', 'jive', 'jock', 'joey', 'jogs', 'joss', 'jota', 'jots', 'juba', 'jube', 'judo', 'jump', 'junk', 'jura', 'juts', 'jynx', 'kago', 'kail', 'kaka', 'kale', 'kana', 'keek', 'keep', 'kefs', 'kegs', 'kerf', 'kern', 'keys', 'kibe', 'kick', 'kids', 'kifs', 'kill', 'kina', 'kind', 'kine', 'kite', 'kiwi', 'knap', 'knit', 'koas', 'kobs', 'kyat', 'lack', 'lahs', 'lair', 'lama', 'lamb', 'lame', 'lats', 'lava', 'lays', 'leaf', 'leak', 'leas', 'lees', 'leks', 'leno', 'libs', 'lich', 'lick', 'lien', 'lier', 'lieu', 'life', 'lift', 'limb', 'line', 'link', 'linn', 'lira', 'loft', 'loge', 'loir', 'long', 'loof', 'look', 'loot', 'lore', 'loss', 'lots', 'loup', 'love', 'luce', 'ludo', 'luke', 'lulu', 'lure', 'lush', 'magi', 'maid', 'main', 'mako', 'male', 'mana', 'many', 'mart', 'mash', 'mast', 'mate', 'math', 'mats', 'matt', 'maul', 'maya', 'mays', 'meal', 'mean', 'meed', 'mela', 'mene', 'mere', 'merk', 'mesh', 'mete', 'mice', 'milo', 'mime', 'mina', 'mine', 'mirk', 'miss', 'mobs', 'moit', 'mold', 'molt', 'mome', 'moms', 'monk', 'moot', 'mope', 'more', 'morn', 'mows', 'moxa', 'much', 'mung', 'mush', 'muss', 'myth', 'name', 'nard', 'nark', 'nave', 'navy', 'neck', 'newt', 'nibs', 'nims', 'nine', 'nock', 'noil', 'noma', 'nosh', 'nowt', 'nuke', 'oafs', 'oast', 'oats', 'obit', 'odor', 'okra', 'omer', 'oner', 'ones', 'orcs', 'ords', 'orfe', 'orle', 'ossa', 'outs', 'over', 'owls', 'pail', 'pall', 'palp', 'pams', 'pang', 'pans', 'pant', 'paps', 'pate', 'pats', 'paws', 'pear', 'peba', 'pech', 'pecs', 'peel', 'peer', 'pees', 'pein', 'peri', 'phon', 'pice', 'pita', 'pith', 'play', 'plop', 'plot', 'plow', 'plug', 'plum', 'polo', 'pomp', 'pond', 'pons', 'pony', 'poof', 'pope', 'poss', 'pots', 'pour', 'prad', 'prat', 'prep', 'prob', 'prof', 'prow', 'puck', 'puds', 'puke', 'puku', 'pump', 'puns', 'pupa', 'purl', 'pyre', 'quad', 'quay', 'quey', 'quiz', 'raid', 'rail', 'rain', 'raja', 'rale', 'rams', 'rand', 'rant', 'raps', 'rasp', 'razz', 'rede', 'reef', 'reif', 'rein', 'repp', 'rial', 'ribs', 'rick', 'rift', 'rill', 'rime', 'rims', 'ring', 'rins', 'rise', 'rite', 'rits', 'roam', 'robe', 'rods', 'roma', 'rook', 'rort', 'rotl', 'roup', 'roux', 'rube', 'rubs', 'ruby', 'rues', 'rugs', 'ruin', 'runs', 'ryas', 'sack', 'sacs', 'saga', 'sail', 'sale', 'salp', 'salt', 'sand', 'sang', 'sash', 'saut', 'says', 'scab', 'scow', 'scud', 'scup', 'scut', 'seal', 'seam', 'sech', 'seed', 'seep', 'seer', 'self', 'sena', 'send', 'sera', 'sere', 'shad', 'shah', 'sham', 'shay', 'shes', 'ship', 'shoe', 'sick', 'sida', 'sign', 'sike', 'sima', 'sine', 'sing', 'sinh', 'sink', 'sins', 'site', 'size', 'skat', 'skin', 'skip', 'skis', 'slaw', 'sled', 'slew', 'sley', 'slob', 'slue', 'slug', 'smut', 'snap', 'snib', 'snip', 'snob', 'snog', 'snot', 'snow', 'snub', 'snug', 'soft', 'soja', 'soke', 'song', 'sons', 'sook', 'sorb', 'sori', 'souk', 'soul', 'sous', 'soya', 'spit', 'stay', 'stew', 'stir', 'stob', 'stud', 'suds', 'suer', 'suit', 'sumo', 'sums', 'sups', 'suqs', 'suss', 'sway', 'syce', 'synd', 'taal', 'tach', 'taco', 'tads', 'taka', 'tale', 'tamp', 'tams', 'tang', 'tans', 'tape', 'tare', 'taro', 'tarp', 'tart', 'tass', 'taus', 'teat', 'teds', 'teff', 'tegu', 'tell', 'term', 'thar', 'thaw', 'tics', 'tier', 'tiff', 'tils', 'tilt', 'tint', 'tipi', 'tire', 'tirl', 'toby', 'tods', 'toea', 'toff', 'toga', 'toil', 'toke', 'tola', 'tole', 'tomb', 'toms', 'torc', 'tors', 'tort', 'tosh', 'tote', 'tret', 'trey', 'trio', 'trug', 'tuck', 'tugs', 'tule', 'tune', 'tuns', 'tuts', 'tyke', 'tyne', 'typo', 'ulna', 'umbo', 'unau', 'unit', 'upas', 'user', 'uvea', 'vacs', 'vane', 'vang', 'vans', 'vara', 'vase', 'veep', 'veer', 'vega', 'veil', 'vela', 'vent', 'vies', 'view', 'vina', 'vine', 'vise', 'vlei', 'volt', 'vows', 'wads', 'waft', 'wage', 'wain', 'walk', 'want', 'wart', 'wave', 'waws', 'weal', 'wean', 'weds', 'weep', 'weft', 'weir', 'weka', 'weld', 'wens', 'weys', 'whap', 'whey', 'whin', 'whit', 'whop', 'wide', 'wife', 'wind', 'wine', 'wino', 'wins', 'wire', 'wise', 'woes', 'wont', 'wool', 'work', 'worm', 'wort', 'yack', 'yank', 'yapp', 'yard', 'yate', 'yawl', 'yegg', 'yell', 'yeuk', 'yews', 'yips', 'yobs', 'yogi', 'yoke', 'yolk', 'yoni', 'zack', 'zags', 'zest', 'zhos', 'zigs', 'zila', 'zips', 'ziti', 'zoea', 'zone', 'zoon')  # noqa: E501, Q000, N806
+    ADJECTIVES = ('about', 'above', 'abuzz', 'acerb', 'acold', 'acred', 'added', 'addle', 'adept', 'adult', 'adunc', 'adust', 'afoul', 'after', 'agape', 'agaze', 'agile', 'aging', 'agley', 'aglow', 'ahead', 'ahull', 'aided', 'alary', 'algal', 'alike', 'alive', 'alone', 'aloof', 'alpha', 'amber', 'amiss', 'amort', 'ample', 'amuck', 'angry', 'anile', 'apeak', 'apish', 'arced', 'areal', 'armed', 'aroid', 'ashen', 'aspen', 'astir', 'atilt', 'atrip', 'aulic', 'aural', 'awash', 'awful', 'awing', 'awned', 'axile', 'azoic', 'azure', 'baggy', 'baked', 'balky', 'bally', 'balmy', 'banal', 'bandy', 'bardy', 'bared', 'barer', 'barky', 'basal', 'based', 'baser', 'basic', 'batty', 'bawdy', 'beady', 'beaky', 'beamy', 'beaut', 'beefy', 'beery', 'beige', 'bendy', 'bifid', 'bijou', 'biped', 'birch', 'bitty', 'blame', 'bland', 'blank', 'blear', 'blest', 'blind', 'blond', 'blown', 'blowy', 'bluer', 'bluff', 'blunt', 'boned', 'bonny', 'boozy', 'bored', 'boric', 'bosky', 'bosom', 'bound', 'bovid', 'bowed', 'boxed', 'braky', 'brash', 'brief', 'briny', 'brisk', 'broad', 'broch', 'brood', 'brown', 'brute', 'buggy', 'bulgy', 'bumpy', 'burly', 'burnt', 'burry', 'bushy', 'busty', 'butch', 'buxom', 'cadgy', 'cagey', 'calmy', 'campy', 'canny', 'caped', 'cased', 'catty', 'cauld', 'cedar', 'cered', 'ceric', 'chary', 'cheap', 'cheek', 'chewy', 'chief', 'chill', 'chirk', 'choky', 'cissy', 'civil', 'cleft', 'coaly', 'color', 'comfy', 'comic', 'compo', 'conic', 'couth', 'coxal', 'crack', 'crank', 'crash', 'crass', 'crisp', 'cronk', 'cross', 'crude', 'cruel', 'crumb', 'cured', 'curly', 'curst', 'cushy', 'cutty', 'cynic', 'dated', 'dazed', 'dedal', 'deism', 'diazo', 'dicey', 'dingy', 'direr', 'dirty', 'dishy', 'dizzy', 'dolce', 'doped', 'dopey', 'dormy', 'dorty', 'dosed', 'dotal', 'dotty', 'dowdy', 'dowie', 'downy', 'dozen', 'drawn', 'dread', 'drear', 'dress', 'dried', 'ducky', 'duddy', 'dummy', 'dumpy', 'duple', 'dural', 'dusky', 'dusty', 'dutch', 'dying', 'eager', 'eaten', 'ebony', 'edged', 'eerie', 'eight', 'elder', 'elect', 'elfin', 'elite', 'empty', 'enate', 'enemy', 'epoxy', 'erect', 'ethic', 'every', 'extra', 'faced', 'faery', 'faint', 'famed', 'fancy', 'farci', 'fatal', 'fated', 'fatty', 'fazed', 'felon', 'fenny', 'ferny', 'fetal', 'fetid', 'fewer', 'fiery', 'fifty', 'filar', 'filmy', 'final', 'fined', 'finer', 'finny', 'fired', 'first', 'fishy', 'fixed', 'fizzy', 'flaky', 'flamy', 'flash', 'flawy', 'fleet', 'flory', 'flown', 'fluid', 'fluky', 'flush', 'focal', 'foggy', 'folio', 'forky', 'forte', 'forty', 'found', 'frail', 'frank', 'freed', 'freer', 'fresh', 'fried', 'front', 'frore', 'fuggy', 'funky', 'funny', 'furry', 'fusil', 'fussy', 'fuzzy', 'gabby', 'gamer', 'gamey', 'gamic', 'gammy', 'garni', 'gauge', 'gaunt', 'gauzy', 'gawky', 'gawsy', 'gemmy', 'genal', 'genic', 'ghast', 'gimpy', 'girly', 'glare', 'glary', 'glial', 'glued', 'gluey', 'godly', 'gooey', 'goofy', 'goosy', 'gouty', 'grade', 'grand', 'grapy', 'grave', 'gross', 'group', 'gruff', 'guest', 'gules', 'gulfy', 'gummy', 'gushy', 'gusty', 'gutsy', 'gutta', 'gypsy', 'gyral', 'hadal', 'hammy', 'handy', 'hardy', 'hasty', 'hated', 'hazel', 'heady', 'heapy', 'hefty', 'heigh', 'hempy', 'herby', 'hexed', 'hi-fi', 'hilly', 'hired', 'holey', 'honey', 'hooly', 'hoven', 'huger', 'hulky', 'humid', 'hunky', 'hyoid', 'idled', 'iliac', 'inane', 'incog', 'inert', 'inner', 'inter', 'iodic', 'ionic', 'irate', 'irony', 'itchy', 'jaggy', 'jammy', 'japan', 'jazzy', 'jerky', 'jetty', 'joint', 'jowly', 'juicy', 'jumpy', 'jural', 'kacha', 'kaput', 'kempt', 'keyed', 'kinky', 'known', 'kooky', 'kraal', 'laced', 'laigh', 'lairy', 'lamer', 'lardy', 'larky', 'lated', 'later', 'lathy', 'leady', 'leafy', 'leaky', 'leary', 'least', 'ledgy', 'leery', 'legal', 'leggy', 'lento', 'level', 'licht', 'licit', 'liege', 'light', 'liked', 'liney', 'lippy', 'lived', 'livid', 'loamy', 'loath', 'lobar', 'local', 'loony', 'loose', 'loral', 'losel', 'lousy', 'loved', 'lower', 'lowly', 'lowse', 'loyal', 'lucid', 'lucky', 'lumpy', 'lunar', 'lurid', 'lushy', 'lying', 'lyric', 'macho', 'macro', 'magic', 'major', 'malar', 'mangy', 'manky', 'manly', 'mardy', 'massy', 'mated', 'matte', 'mauve', 'mazed', 'mealy', 'meaty', 'medal', 'melic', 'mesic', 'mesne', 'messy', 'metal', 'miffy', 'milky', 'mined', 'minim', 'minor', 'minus', 'mired', 'mirky', 'misty', 'mixed', 'modal', 'model', 'moire', 'molar', 'moldy', 'moody', 'moony', 'mopey', 'moral', 'mossy', 'mothy', 'motor', 'mousy', 'moved', 'mucid', 'mucky', 'muddy', 'muggy', 'muley', 'mural', 'murky', 'mushy', 'muted', 'muzzy', 'myoid', 'naggy', 'naive', 'naked', 'named', 'nasty', 'natal', 'naval', 'nervy', 'newsy', 'nicer', 'niffy', 'nifty', 'ninth', 'nitty', 'nival', 'noble', 'nodal', 'noisy', 'non-U', 'north', 'nosed', 'noted', 'nowed', 'nubby', 'oaken', 'oared', 'oaten', 'obese', 'ocher', 'ochre', 'often', 'ohmic', 'oiled', 'olden', 'older', 'oleic', 'olive', 'optic', 'ortho', 'osmic', 'other', 'outer', 'ovoid', 'owing', 'owned', 'paced', 'pagan', 'paled', 'paler', 'pally', 'paper', 'pappy', 'parky', 'party', 'pasty', 'pavid', 'pawky', 'peaky', 'pearl', 'peart', 'peaty', 'pedal', 'peppy', 'perdu', 'perky', 'pesky', 'phony', 'piano', 'picky', 'piled', 'piney', 'pious', 'pique', 'pithy', 'platy', 'plump', 'plush', 'podgy', 'potty', 'power', 'prest', 'pricy', 'prima', 'prime', 'print', 'privy', 'prize', 'prone', 'proof', 'prosy', 'proud', 'proxy', 'pseud', 'pucka', 'pudgy', 'puffy', 'pukka', 'pupal', 'purer', 'pursy', 'pushy', 'pyoid', 'quack', 'quare', 'quasi', 'quiet', 'quits', 'rabic', 'rabid', 'radio', 'raked', 'randy', 'rapid', 'rarer', 'raspy', 'rathe', 'ratty', 'ready', 'reedy', 'reeky', 'refer', 'regal', 'riant', 'ridgy', 'right', 'riled', 'rimed', 'rindy', 'risen', 'risky', 'ritzy', 'rival', 'riven', 'robed', 'rocky', 'roily', 'roman', 'rooky', 'ropey', 'round', 'rowdy', 'ruddy', 'ruled', 'rummy', 'runic', 'runny', 'runty', 'rural', 'rusty', 'rutty', 'sable', 'salic', 'sandy', 'sappy', 'sarky', 'sassy', 'sated', 'saved', 'savvy', 'scald', 'scaly', 'scary', 'score', 'scrap', 'sedgy', 'seely', 'seral', 'sewed', 'shaky', 'sharp', 'sheen', 'shier', 'shill', 'shoal', 'shock', 'shoed', 'shore', 'short', 'shyer', 'silky', 'silly', 'silty', 'sixth', 'sixty', 'skint', 'slack', 'slant', 'sleek', 'slier', 'slimy', 'slung', 'small', 'smart', 'smoky', 'snaky', 'sneak', 'snide', 'snowy', 'snuff', 'so-so', 'soapy', 'sober', 'socko', 'solar', 'soled', 'solid', 'sonic', 'sooth', 'sooty', 'soppy', 'sorer', 'sound', 'soupy', 'spent', 'spicy', 'spiky', 'spiny', 'spiry', 'splay', 'split', 'sport', 'spumy', 'squat', 'staid', 'stiff', 'still', 'stoic', 'stone', 'stony', 'store', 'stout', 'straw', 'stray', 'strip', 'stung', 'suave', 'sudsy', 'sulfa', 'sulky', 'sunny', 'super', 'sural', 'surer', 'surfy', 'surgy', 'surly', 'swell', 'swept', 'swish', 'sworn', 'tabby', 'taboo', 'tacit', 'tacky', 'tamed', 'tamer', 'tangy', 'taped', 'tarot', 'tarry', 'tasty', 'tatty', 'taunt', 'tawie', 'teary', 'techy', 'telic', 'tenor', 'tense', 'tenth', 'tenty', 'tepid', 'terse', 'testy', 'third', 'tidal', 'tight', 'tiled', 'timid', 'tinct', 'tined', 'tippy', 'tipsy', 'tonal', 'toned', 'tonic', 'toric', 'total', 'tough', 'toxic', 'trade', 'treed', 'treen', 'trial', 'truer', 'tubal', 'tubby', 'tumid', 'tuned', 'tutti', 'twill', 'typal', 'typed', 'typic', 'umber', 'unapt', 'unbid', 'uncut', 'undue', 'undug', 'unfed', 'unfit', 'union', 'unlet', 'unmet', 'unwed', 'unwet', 'upper', 'upset', 'urban', 'utile', 'uveal', 'vagal', 'valid', 'vapid', 'varus', 'vatic', 'veiny', 'vital', 'vivid', 'vocal', 'vogie', 'volar', 'vying', 'wacky', 'wally', 'waney', 'warty', 'washy', 'waspy', 'waste', 'waugh', 'waxen', 'webby', 'wedgy', 'weeny', 'weepy', 'weest', 'weird', 'welsh', 'wersh', 'whist', 'white', 'whity', 'whole', 'wider', 'wight', 'winey', 'wired', 'wised', 'wiser', 'withy', 'wonky', 'woods', 'woozy', 'world', 'wormy', 'worse', 'worst', 'woven', 'wrath', 'wrier', 'wrong', 'wroth', 'xeric', 'yarer', 'yolky', 'young', 'yucky', 'yummy', 'zesty', 'zingy', 'zinky', 'zippy', 'zonal')  # noqa: E501, Q000, N806
     # fmt: on
     while True:
-        adjective = random.choice(ADJECTIVES)  # nosec B311
-        noun = random.choice(NOUNS)  # nosec B311
+        adjective = random.choice(ADJECTIVES)  # noqa: S311
+        noun = random.choice(NOUNS)  # noqa: S311
         name = f"{adjective}-{noun}"
         exp_ref = ExpRefInfo(baseline_sha=baseline_rev, name=name)
         if not scm.get_ref(str(exp_ref)):
             return name
 
 
 def get_dvc_stage_template(live):
```

### Comparing `dvclive-2.6.3/src/dvclive/error.py` & `dvclive-2.6.4/src/dvclive/error.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,7 +23,15 @@
         )
 
 
 class InvalidParameterTypeError(DvcLiveError):
     def __init__(self, val: Any):
         self.val = val
         super().__init__(f"Parameter type {type(val)} is not supported.")
+
+
+class InvalidReportModeError(DvcLiveError):
+    def __init__(self, val):
+        super().__init__(
+            f"`report` can only be `None`, `auto`, `html`, `notebook` or `md`. "
+            f"Got {val} instead."
+        )
```

### Comparing `dvclive-2.6.3/src/dvclive/fastai.py` & `dvclive-2.6.4/src/dvclive/fastai.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,11 +73,10 @@
 
     def after_fit(self):
         if hasattr(self, "lr_finder") or hasattr(self, "gather_preds"):
             return
         if _inside_fine_tune() and not self.freeze_stage_ended:
             self.freeze_stage_ended = True
         else:
-            if hasattr(self, "save_model"):
-                if self.save_model.last_saved_path:
-                    self.live.log_artifact(str(self.save_model.last_saved_path))
+            if hasattr(self, "save_model") and self.save_model.last_saved_path:
+                self.live.log_artifact(str(self.save_model.last_saved_path))
             self.live.end()
```

### Comparing `dvclive-2.6.3/src/dvclive/huggingface.py` & `dvclive-2.6.4/src/dvclive/huggingface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# ruff: noqa: ARG002
 from typing import Optional
 
 from transformers import (
     TrainerCallback,
     TrainerControl,
     TrainerState,
     TrainingArguments,
```

### Comparing `dvclive-2.6.3/src/dvclive/lgbm.py` & `dvclive-2.6.4/src/dvclive/lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.3/src/dvclive/lightning.py` & `dvclive-2.6.4/src/dvclive/lightning.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=protected-access
+# ruff: noqa: ARG002
 import inspect
 from typing import Any, Dict, Optional
 
 from lightning_fabric.utilities.logger import (
     _convert_params,
     _sanitize_callable_params,
     _sanitize_params,
@@ -35,15 +35,15 @@
 
 class DVCLiveLogger(Logger):
     def __init__(
         self,
         run_name: Optional[str] = "dvclive_run",
         prefix="",
         experiment=None,
-        dir: Optional[str] = None,  # noqa pylint: disable=redefined-builtin
+        dir: Optional[str] = None,  # noqa: A002
         resume: bool = False,
         report: Optional[str] = "auto",
         save_dvc_exp: bool = False,
         dvcyaml: bool = True,
     ):
         super().__init__()
         self._prefix = prefix
@@ -54,15 +54,15 @@
             "dvcyaml": dvcyaml,
         }
         if dir is not None:
             self._live_init["dir"] = dir
         self._experiment = experiment
         self._version = run_name
         # Force Live instantiation
-        self.experiment  # noqa pylint: disable=pointless-statement
+        self.experiment  # noqa: B018
 
     @property
     def name(self):
         return "DvcLiveLogger"
 
     @rank_zero_only
     def log_hyperparams(self, params, *args, **kwargs):
@@ -78,41 +78,35 @@
         Actual DVCLive object. To use DVCLive features in your
         :class:`~LightningModule` do the following.
         Example::
             self.logger.experiment.some_dvclive_function()
         """
         if self._experiment is not None:
             return self._experiment
-        else:
-            assert (
-                rank_zero_only.rank == 0
-            ), "tried to init log dirs in non global_rank=0"
-            self._experiment = Live(**self._live_init)
+        self._experiment = Live(**self._live_init)
 
         return self._experiment
 
     @property
     def version(self):
         return self._version
 
     @rank_zero_only
     def log_metrics(self, metrics: Dict[str, Any], step: Optional[int] = None):
-        assert (
-            rank_zero_only.rank == 0  # type: ignore
-        ), "experiment tried to log from global_rank != 0"
         self.experiment.step = step
         for metric_name, metric_val in metrics.items():
-            if is_tensor(metric_val):
-                metric_val = metric_val.cpu().detach().item()
-            metric_name = standardize_metric_name(metric_name, __name__)
-            self.experiment.log_metric(name=metric_name, val=metric_val)
+            val = metric_val
+            if is_tensor(val):
+                val = val.cpu().detach().item()
+            name = standardize_metric_name(metric_name, __name__)
+            self.experiment.log_metric(name=name, val=val)
         if _should_call_next_step():
-            if step == self.experiment._latest_studio_step:
+            if step == self.experiment._latest_studio_step:  # noqa: SLF001
                 # We are in log_eval_end_metrics but there has been already
                 # a studio request sent with `step`.
                 # We decrease the number to bypass `live.studio._get_unsent_datapoints`
-                self.experiment._latest_studio_step -= 1
+                self.experiment._latest_studio_step -= 1  # noqa: SLF001
             self.experiment.next_step()
 
     @rank_zero_only
     def finalize(self, status: str) -> None:
         self.experiment.end()
```

### Comparing `dvclive-2.6.3/src/dvclive/live.py` & `dvclive-2.6.4/src/dvclive/live.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,20 @@
     get_dvc_stage_template,
     get_random_exp_name,
     make_checkpoint,
     make_dvcyaml,
     mark_dvclive_only_ended,
     mark_dvclive_only_started,
 )
-from .error import InvalidDataTypeError, InvalidParameterTypeError, InvalidPlotTypeError
+from .error import (
+    InvalidDataTypeError,
+    InvalidParameterTypeError,
+    InvalidPlotTypeError,
+    InvalidReportModeError,
+)
 from .plots import PLOT_TYPES, SKLEARN_PLOTS, Image, Metric, NumpyEncoder
 from .report import BLANK_NOTEBOOK_REPORT, make_report
 from .serialize import dump_json, dump_yaml, load_yaml
 from .studio import get_studio_updates
 from .utils import env2bool, inside_notebook, matplotlib_installed, open_file_in_browser
 
 logging.basicConfig()
@@ -35,15 +40,15 @@
 ParamLike = Union[int, float, str, bool, List["ParamLike"], Dict[str, "ParamLike"]]
 StrPath = Union[str, Path]
 
 
 class Live:
     def __init__(
         self,
-        dir: str = "dvclive",  # noqa pylint: disable=redefined-builtin
+        dir: str = "dvclive",  # noqa: A002
         resume: bool = False,
         report: Optional[str] = "auto",
         save_dvc_exp: bool = False,
         dvcyaml: bool = True,
     ):
         self.summary: Dict[str, Any] = {}
 
@@ -188,21 +193,19 @@
                 self._report_mode = "notebook"
                 self._report_notebook = display(
                     HTML(BLANK_NOTEBOOK_REPORT), display_id=True
                 )
             else:
                 self._report_mode = "html"
         elif self._report_mode not in {None, "html", "notebook", "md"}:
-            raise ValueError(
-                "`report` can only be `None`, `auto`, `html`, `notebook` or `md`"
-            )
+            raise InvalidReportModeError(self._report_mode)
         logger.debug(f"{self._report_mode=}")
 
     @property
-    def dir(self) -> str:
+    def dir(self) -> str:  # noqa: A003
         return self._dir
 
     @property
     def params_file(self) -> str:
         return os.path.join(self.dir, "params.yaml")
 
     @property
@@ -216,18 +219,15 @@
     @property
     def plots_dir(self) -> str:
         return os.path.join(self.dir, "plots")
 
     @property
     def report_file(self) -> Optional[str]:
         if self._report_mode in ("html", "md", "notebook"):
-            if self._report_mode == "notebook":
-                suffix = "html"
-            else:
-                suffix = self._report_mode
+            suffix = "html" if self._report_mode == "notebook" else self._report_mode
             return os.path.join(self.dir, f"report.{suffix}")
         return None
 
     @property
     def step(self) -> int:
         return self._step or 0
 
@@ -265,15 +265,15 @@
         self.summary = set_in(self.summary, data.summary_keys, val)
         logger.debug(f"Logged {name}: {val}")
 
     def log_image(self, name: str, val):
         if not Image.could_log(val):
             raise InvalidDataTypeError(name, type(val))
 
-        if isinstance(val, str) or isinstance(val, Path):
+        if isinstance(val, (str, Path)):
             from PIL import Image as ImagePIL
 
             val = ImagePIL.open(val)
 
         if name in self._images:
             data = self._images[name]
         else:
@@ -325,15 +325,15 @@
         """Tracks a local file or directory with DVC"""
         if not isinstance(path, (str, Path)):
             raise InvalidDataTypeError(path, type(path))
 
         if self._dvc_repo is not None:
             try:
                 stage = self._dvc_repo.add(path)
-            except Exception as e:  # pylint: disable=broad-except
+            except Exception as e:  # noqa: BLE001
                 logger.warning(f"Failed to dvc add {path}: {e}")
                 return
 
             self._outs.add(path)
             dvc_file = stage[0].addressing
 
             if self._save_dvc_exp:
@@ -382,26 +382,17 @@
         if self._inside_with:
             # Prevent `live.end` calls inside context manager
             return
         self.make_summary(update_step=False)
         if self._dvcyaml:
             self.make_dvcyaml()
 
-        if self._inside_dvc_exp and self._dvc_repo:
-            dir_spec = PathSpec.from_lines("gitwildmatch", [self.dir])
-            outs_spec = PathSpec.from_lines(
-                "gitwildmatch", [str(o) for o in self._dvc_repo.index.outs]
-            )
-            paths_to_track = [
-                f
-                for f in self._dvc_repo.scm.untracked_files()
-                if (dir_spec.match_file(f) and not outs_spec.match_file(f))
-            ]
-            if paths_to_track:
-                self._dvc_repo.scm.add(paths_to_track)
+        self._ensure_paths_are_tracked_in_dvc_exp()
+
+        self.save_dvc_exp()
 
         if "done" not in self._studio_events_to_skip:
             response = False
             if post_live_metrics is not None:
                 kwargs = {}
                 if self._experiment_rev:
                     kwargs["experiment_rev"] = self._experiment_rev
@@ -415,28 +406,14 @@
             if not response:
                 logger.warning("`post_to_studio` `done` event failed.")
             self._studio_events_to_skip.add("done")
             self._studio_events_to_skip.add("data")
         else:
             self.make_report()
 
-        if self._save_dvc_exp:
-            from dvc.exceptions import DvcException
-
-            try:
-                self._experiment_rev = self._dvc_repo.experiments.save(
-                    name=self._exp_name,
-                    include_untracked=self._include_untracked,
-                    force=True,
-                )
-            except DvcException as e:
-                logger.warning(f"Failed to save experiment:\n{e}")
-            finally:
-                mark_dvclive_only_ended()
-
         if self._dvc_repo and not self._inside_dvc_exp:
             from dvc.exceptions import DvcException
 
             try:
                 path = os.path.join(self._dvc_repo.root_dir, "dvc.yaml")
                 yaml = get_dvc_stage_template(self)
                 logger.info(f"To run with DVC, add this to {path}:\n{yaml}")
@@ -460,7 +437,36 @@
     def __enter__(self):
         self._inside_with = True
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._inside_with = False
         self.end()
+
+    def _ensure_paths_are_tracked_in_dvc_exp(self):
+        if self._inside_dvc_exp and self._dvc_repo:
+            dir_spec = PathSpec.from_lines("gitwildmatch", [self.dir])
+            outs_spec = PathSpec.from_lines(
+                "gitwildmatch", [str(o) for o in self._dvc_repo.index.outs]
+            )
+            paths_to_track = [
+                f
+                for f in self._dvc_repo.scm.untracked_files()
+                if (dir_spec.match_file(f) and not outs_spec.match_file(f))
+            ]
+            if paths_to_track:
+                self._dvc_repo.scm.add(paths_to_track)
+
+    def save_dvc_exp(self):
+        if self._save_dvc_exp:
+            from dvc.exceptions import DvcException
+
+            try:
+                self._experiment_rev = self._dvc_repo.experiments.save(
+                    name=self._exp_name,
+                    include_untracked=self._include_untracked,
+                    force=True,
+                )
+            except DvcException as e:
+                logger.warning(f"Failed to save experiment:\n{e}")
+            finally:
+                mark_dvclive_only_ended()
```

### Comparing `dvclive-2.6.3/src/dvclive/optuna.py` & `dvclive-2.6.4/src/dvclive/optuna.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# ruff: noqa: ARG002
 from dvclive import Live
 
 
 class DVCLiveCallback:
     def __init__(self, metric_name="metric", **kwargs) -> None:
         kwargs["dir"] = kwargs.get("dir", "dvclive-optuna")
         kwargs.pop("save_dvc_exp", None)
@@ -16,31 +17,28 @@
     def _log_metrics(self, values, live):
         if values is None:
             return
 
         if isinstance(self.metric_name, str):
             if len(values) > 1:
                 # Broadcast default name for multi-objective optimization.
-                names = [
-                    "{}_{}".format(self.metric_name, i) for i in range(len(values))
-                ]
+                names = [f"{self.metric_name}_{i}" for i in range(len(values))]
 
             else:
                 names = [self.metric_name]
 
-        else:
-            if len(self.metric_name) != len(values):
-                raise ValueError(
-                    "Running multi-objective optimization "
-                    "with {} objective values, but {} names specified. "
-                    "Match objective values and names,"
-                    "or use default broadcasting.".format(
-                        len(values), len(self.metric_name)
-                    )
+        elif len(self.metric_name) != len(values):
+            raise ValueError(
+                "Running multi-objective optimization "
+                "with {} objective values, but {} names specified. "
+                "Match objective values and names,"
+                "or use default broadcasting.".format(
+                    len(values), len(self.metric_name)
                 )
+            )
 
-            else:
-                names = [*self.metric_name]
+        else:
+            names = [*self.metric_name]
 
-        metrics = {name: val for name, val in zip(names, values)}
+        metrics = dict(zip(names, values))
         for k, v in metrics.items():
             live.summary[k] = v
```

### Comparing `dvclive-2.6.3/src/dvclive/plots/base.py` & `dvclive-2.6.4/src/dvclive/plots/base.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.3/src/dvclive/plots/image.py` & `dvclive-2.6.4/src/dvclive/plots/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
     @staticmethod
     def could_log(val: object) -> bool:
         if val.__class__.__module__ == "PIL.Image":
             return True
         if val.__class__.__module__ == "numpy":
             return True
-        if isinstance(val, PurePath) or isinstance(val, str):
+        if isinstance(val, (PurePath, str)):
             return True
         return False
 
-    def dump(self, val, **kwargs) -> None:
+    def dump(self, val, **kwargs) -> None:  # noqa: ARG002
         if val.__class__.__module__ == "numpy":
             from PIL import Image as ImagePIL
 
             pil_image = ImagePIL.fromarray(val)
         else:
             pil_image = val
         pil_image.save(self.output_path)
```

### Comparing `dvclive-2.6.3/src/dvclive/plots/metric.py` & `dvclive-2.6.4/src/dvclive/plots/metric.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,19 @@
     suffixes = [".csv", ".tsv"]
     subfolder = "metrics"
 
     @staticmethod
     def could_log(val: object) -> bool:
         if isinstance(val, (int, float)):
             return True
-        if val.__class__.__module__ == "numpy":
-            if val.__class__.__name__ in NUMPY_SCALARS:
-                return True
+        if (
+            val.__class__.__module__ == "numpy"
+            and val.__class__.__name__ in NUMPY_SCALARS
+        ):
+            return True
         return False
 
     @property
     def output_path(self) -> Path:
         _path = Path(f"{self.output_folder / self.name}.tsv")
         _path.parent.mkdir(exist_ok=True, parents=True)
         return _path
```

### Comparing `dvclive-2.6.3/src/dvclive/plots/sklearn.py` & `dvclive-2.6.4/src/dvclive/plots/sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def output_path(self) -> Path:
         _path = Path(f"{self.output_folder / self.name}.json")
         _path.parent.mkdir(exist_ok=True, parents=True)
         return _path
 
     @staticmethod
     def could_log(val: object) -> bool:
-        if isinstance(val, tuple) and len(val) == 2:
+        if isinstance(val, tuple) and len(val) == 2:  # noqa: PLR2004
             return True
         return False
 
     @staticmethod
     def get_properties():
         raise NotImplementedError
 
@@ -121,15 +121,15 @@
             "x": "actual",
             "y": "predicted",
             "title": "Confusion Matrix",
             "x_label": "True Label",
             "y_label": "Predicted Label",
         }
 
-    def dump(self, val, **kwargs) -> None:
+    def dump(self, val, **kwargs) -> None:  # noqa: ARG002
         cm = [
             {"actual": str(actual), "predicted": str(predicted)}
             for actual, predicted in zip(val[0], val[1])
         ]
         dump_json(cm, self.output_path)
```

### Comparing `dvclive-2.6.3/src/dvclive/plots/utils.py` & `dvclive-2.6.4/src/dvclive/plots/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.6.3/src/dvclive/report.py` & `dvclive-2.6.4/src/dvclive/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
+# ruff: noqa: SLF001
 import base64
 import json
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from dvc_render.html import render_html
 from dvc_render.image import ImageRenderer
 from dvc_render.markdown import render_markdown
 from dvc_render.table import TableRenderer
 from dvc_render.vega import VegaRenderer
 
+from dvclive.error import InvalidReportModeError
 from dvclive.plots import SKLEARN_PLOTS, Image, Metric
 from dvclive.plots.sklearn import SKLearnPlot
 from dvclive.serialize import load_yaml
 from dvclive.utils import inside_colab, parse_tsv
 
 if TYPE_CHECKING:
     from dvclive import Live
 
 
-# noqa pylint: disable=protected-access
-
-
 BLANK_NOTEBOOK_REPORT = """
 <div style="width: 100%;height: 700px;text-align: center">
 DVCLive Report
 </div>
 """
 
 COLAB_HTML = """<!DOCTYPE html>
@@ -172,8 +171,8 @@
                 new_report = IFrame(  # type: ignore [assignment]
                     live.report_file, "100%", 700
                 )
             live._report_notebook.update(new_report)
     elif live._report_mode == "md":
         render_markdown(renderers, live.report_file)
     else:
-        raise ValueError(f"Invalid `mode` {live._report_mode}.")
+        raise InvalidReportModeError(live._report_mode)
```

### Comparing `dvclive-2.6.3/src/dvclive/serialize.py` & `dvclive-2.6.4/src/dvclive/serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     from ruamel.yaml import YAMLError as _YAMLError
 
     yaml = YAML(typ=typ)
     with open(path, encoding="utf-8") as fd:
         try:
             return yaml.load(fd.read())
         except _YAMLError:
-            raise YAMLFileCorruptedError(path)
+            raise YAMLFileCorruptedError(path) from _YAMLError
 
 
 def get_yaml():
     from ruamel.yaml import YAML
 
     yaml = YAML()
     yaml.default_flow_style = False
```

### Comparing `dvclive-2.6.3/src/dvclive/studio.py` & `dvclive-2.6.4/src/dvclive/studio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=protected-access
+# ruff: noqa: SLF001
 import logging
 import os
 from pathlib import Path
 
 from dvclive.serialize import load_yaml
 from dvclive.utils import parse_metrics
```

### Comparing `dvclive-2.6.3/src/dvclive/utils.py` & `dvclive-2.6.4/src/dvclive/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 import json
 import os
 import re
 import webbrowser
 from pathlib import Path
 from platform import uname
 
-# noqa pylint: disable=unused-import
-
 
 def run_once(f):
     def wrapper(*args, **kwargs):
         if not wrapper.has_run:
             wrapper.has_run = True
             return f(*args, **kwargs)
+        return None
 
     wrapper.has_run = False
     return wrapper
 
 
 @run_once
 def open_file_in_browser(file) -> bool:
@@ -103,18 +102,17 @@
         return False
     return True
 
 
 def inside_colab() -> bool:
     try:
         from google import colab  # noqa: F401
-
-        return True
     except ImportError:
         return False
+    return True
 
 
 def inside_notebook() -> bool:
     if inside_colab():
         return True
 
     try:
```

### Comparing `dvclive-2.6.3/src/dvclive/xgb.py` & `dvclive-2.6.4/src/dvclive/xgb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# ruff: noqa: ARG002
 from typing import Optional
 
 from xgboost.callback import TrainingCallback
 
 from dvclive import Live
```

### Comparing `dvclive-2.6.3/src/dvclive.egg-info/SOURCES.txt` & `dvclive-2.6.4/src/dvclive.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 .cruft.json
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 CODE_OF_CONDUCT.rst
 CONTRIBUTING.rst
 LICENSE
-README.rst
-noxfile.py
+README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
 .github/workflows/release.yml
 .github/workflows/tests.yml
 .github/workflows/update-template.yaml
+docs/dvc_plots_diff.png
+docs/studio_compare.png
+docs/vscode_experiments.png
+docs/vscode_plots.png
 src/dvclive/__init__.py
 src/dvclive/catalyst.py
 src/dvclive/dvc.py
 src/dvclive/env.py
 src/dvclive/error.py
 src/dvclive/fastai.py
 src/dvclive/huggingface.py
```

### Comparing `dvclive-2.6.3/tests/conftest.py` & `dvclive-2.6.4/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-# pylint: disable=redefined-outer-name
+# ruff: noqa: ARG002
 import sys
 
 import pytest
 from dvc_studio_client.env import STUDIO_ENDPOINT, STUDIO_REPO_URL, STUDIO_TOKEN
 
 
-@pytest.fixture
+@pytest.fixture()
 def tmp_dir(tmp_path, monkeypatch):
     monkeypatch.chdir(tmp_path)
-    yield tmp_path
+    return tmp_path
 
 
-@pytest.fixture
+@pytest.fixture()
 def mocked_dvc_repo(tmp_dir, mocker):
     _dvc_repo = mocker.MagicMock()
     _dvc_repo.index.stages = []
     _dvc_repo.scm.get_rev.return_value = "f" * 40
     _dvc_repo.scm.get_ref.return_value = None
+    _dvc_repo.experiments.save.return_value = "e" * 40
     _dvc_repo.root_dir = tmp_dir
     mocker.patch("dvclive.live.get_dvc_repo", return_value=_dvc_repo)
     return _dvc_repo
 
 
-@pytest.fixture
-def dvc_repo(tmp_dir):  # pylint: disable=redefined-outer-name
+@pytest.fixture()
+def dvc_repo(tmp_dir):
     from dvc.repo import Repo
     from scmrepo.git import Git
 
     Git.init(tmp_dir)
     repo = Repo.init(tmp_dir)
     repo.scm.add_commit(".", "init")
     return repo
 
 
 @pytest.fixture(autouse=True)
-def capture_wrap():
+def _capture_wrap():
     # https://github.com/pytest-dev/pytest/issues/5502#issuecomment-678368525
     sys.stderr.close = lambda *args: None
     sys.stdout.close = lambda *args: None
-    yield
 
 
 @pytest.fixture(autouse=True)
-def mocked_webbrowser_open(mocker):
+def _mocked_webbrowser_open(mocker):
     mocker.patch("webbrowser.open")
 
 
 @pytest.fixture(autouse=True)
-def mocked_CI(monkeypatch):
+def _mocked_ci(monkeypatch):
     monkeypatch.setenv("CI", "false")
 
 
-@pytest.fixture
+@pytest.fixture()
 def mocked_studio_post(mocker, monkeypatch):
     valid_response = mocker.MagicMock()
     valid_response.status_code = 200
     mocked_post = mocker.patch("requests.post", return_value=valid_response)
     monkeypatch.setenv(STUDIO_ENDPOINT, "https://0.0.0.0")
     monkeypatch.setenv(STUDIO_REPO_URL, "STUDIO_REPO_URL")
     monkeypatch.setenv(STUDIO_TOKEN, "STUDIO_TOKEN")
```

### Comparing `dvclive-2.6.3/tests/plots/test_image.py` & `dvclive-2.6.4/tests/plots/test_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import numpy as np
 import pytest
 from PIL import Image
 
-# pylint: disable=unused-argument
 from dvclive import Live
 from dvclive.plots import Image as LiveImage
 
 
-def test_PIL(tmp_dir):
+def test_pil(tmp_dir):
     live = Live()
     img = Image.new("RGB", (10, 10), (250, 250, 250))
     live.log_image("image.png", img)
 
     assert (tmp_dir / live.plots_dir / LiveImage.subfolder / "image.png").exists()
 
 
 def test_invalid_extension(tmp_dir):
     live = Live()
     img = Image.new("RGB", (10, 10), (250, 250, 250))
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="unknown file extension"):
         live.log_image("image.foo", img)
 
 
 @pytest.mark.parametrize("shape", [(10, 10), (10, 10, 3), (10, 10, 4)])
 def test_numpy(tmp_dir, shape):
     from PIL import Image as ImagePIL
```

### Comparing `dvclive-2.6.3/tests/plots/test_metric.py` & `dvclive-2.6.4/tests/plots/test_metric.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 
 import numpy as np
 import pytest
 
-# pylint: disable=unused-argument
 from dvclive import Live
 from dvclive.plots.metric import Metric
 from dvclive.plots.utils import NUMPY_INTS, NUMPY_SCALARS
 from dvclive.utils import parse_tsv
 
 
 @pytest.mark.parametrize("dtype", NUMPY_SCALARS)
```

### Comparing `dvclive-2.6.3/tests/plots/test_sklearn.py` & `dvclive-2.6.4/tests/plots/test_sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+# ruff: noqa: N806
 import json
 
 import pytest
 from sklearn import calibration, metrics
 
 from dvclive import Live
 from dvclive.plots.sklearn import SKLearnPlot
 
-# pylint: disable=redefined-outer-name, unused-argument
 
-
-@pytest.fixture
+@pytest.fixture()
 def y_true_y_pred_y_score():
     from sklearn.datasets import make_classification
     from sklearn.ensemble import RandomForestClassifier
     from sklearn.model_selection import train_test_split
 
     X, y = make_classification(random_state=0)
     X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=0)
```

### Comparing `dvclive-2.6.3/tests/test_dvc.py` & `dvclive-2.6.4/tests/test_dvc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=unused-argument,protected-access
 import os
 
 import pytest
 from dvc.repo import Repo
 from PIL import Image
 from ruamel.yaml import YAML
 from scmrepo.git import Git
```

### Comparing `dvclive-2.6.3/tests/test_frameworks/test_catalyst.py` & `dvclive-2.6.4/tests/test_frameworks/test_catalyst.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,34 @@
+# ruff: noqa: N806
 import os
 
 import catalyst
 import pytest
 import torch
 from catalyst import dl
 
 from dvclive import Live
 from dvclive.catalyst import DVCLiveCallback
 from dvclive.plots import Metric
 
-# pylint: disable=redefined-outer-name, unused-argument
 
-
-@pytest.fixture
+@pytest.fixture()
 def runner():
     return dl.SupervisedRunner(
         engine=catalyst.utils.torch.get_available_engine(cpu=True),
         input_key="features",
         output_key="logits",
         target_key="targets",
         loss_key="loss",
     )
 
 
 # see:
 # https://github.com/catalyst-team/catalyst/blob/e99f9/tests/catalyst/callbacks/test_batch_overfit.py
-@pytest.fixture
+@pytest.fixture()
 def runner_params():
     from torch.utils.data import DataLoader, TensorDataset
 
     catalyst.utils.set_global_seed(42)
     num_samples, num_features = int(32e1), int(1e1)
     X, y = torch.rand(num_samples, num_features), torch.rand(num_samples)
     dataset = TensorDataset(X, y)
```

### Comparing `dvclive-2.6.3/tests/test_frameworks/test_fastai.py` & `dvclive-2.6.4/tests/test_frameworks/test_fastai.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,36 +11,33 @@
     tabular_learner,
 )
 
 from dvclive import Live
 from dvclive.fastai import DVCLiveCallback
 from dvclive.plots.metric import Metric
 
-# pylint: disable=redefined-outer-name, unused-argument
 
-
-@pytest.fixture
+@pytest.fixture()
 def data_loader():
     from pandas import DataFrame
 
     d = {
         "x1": [1, 1, 0, 0, 1, 1, 0, 0],
         "x2": [1, 0, 1, 0, 1, 0, 1, 0],
         "y": [1, 0, 0, 1, 1, 0, 0, 1],
     }
     df = DataFrame(d)
-    xor_loader = TabularDataLoaders.from_df(
+    return TabularDataLoaders.from_df(
         df,
         valid_idx=[4, 5, 6, 7],
         batch_size=2,
         cont_names=["x1", "x2"],
         procs=[Categorify, Normalize],
         y_names="y",
     )
-    return xor_loader
 
 
 def test_fastai_callback(tmp_dir, data_loader, mocker):
     learn = tabular_learner(data_loader, metrics=accuracy)
     learn.remove_cb(ProgressCallback)
     callback = DVCLiveCallback()
     live = callback.live
```

### Comparing `dvclive-2.6.3/tests/test_frameworks/test_huggingface.py` & `dvclive-2.6.4/tests/test_frameworks/test_huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from transformers import PretrainedConfig, PreTrainedModel, Trainer, TrainingArguments
 
 from dvclive import Live
 from dvclive.huggingface import DVCLiveCallback
 from dvclive.plots.metric import Metric
 from dvclive.utils import parse_metrics
 
-# pylint: disable=redefined-outer-name, unused-argument, no-value-for-parameter
-
 
 def compute_metrics(eval_preds):
     """https://github.com/iterative/dvclive/pull/321#issuecomment-1266916039"""
     import time
 
     time.sleep(time.get_clock_info("time").resolution)
     return {"foo": 1}
@@ -70,26 +68,26 @@
         y = input_x * self.a + self.b
         if labels is None:
             return (y, y) if self.double_output else (y,)
         loss = nn.functional.mse_loss(y, labels)
         return (loss, y, y) if self.double_output else (loss, y)
 
 
-@pytest.fixture
+@pytest.fixture()
 def data():
     return RegressionDataset(), RegressionDataset()
 
 
-@pytest.fixture
+@pytest.fixture()
 def model():
     config = RegressionModelConfig()
     return RegressionPreTrainedModel(config)
 
 
-@pytest.fixture
+@pytest.fixture()
 def args():
     return TrainingArguments(
         "foo",
         evaluation_strategy="epoch",
         num_train_epochs=2,
     )
```

### Comparing `dvclive-2.6.3/tests/test_frameworks/test_keras.py` & `dvclive-2.6.4/tests/test_frameworks/test_keras.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 import pytest
 
 from dvclive import Live
 from dvclive.keras import DVCLiveCallback
 from dvclive.plots.metric import Metric
 from dvclive.utils import parse_metrics
 
-# pylint: disable=unused-argument, no-name-in-module, redefined-outer-name
 
-
-@pytest.fixture
+@pytest.fixture()
 def xor_model():
     import numpy as np
     from tensorflow.python.keras import Sequential
     from tensorflow.python.keras.layers import Activation, Dense
 
     def make():
         x = np.array([[0, 0], [0, 1], [1, 0], [1, 1]])
@@ -26,18 +24,18 @@
         model.add(Dense(1))
         model.add(Activation("sigmoid"))
 
         model.compile(loss="binary_crossentropy", optimizer="sgd", metrics=["accuracy"])
 
         return model, x, y
 
-    yield make
+    return make
 
 
-def test_keras_callback(tmp_dir, xor_model, capture_wrap, mocker):
+def test_keras_callback(tmp_dir, xor_model, mocker):
     model, x, y = xor_model()
 
     callback = DVCLiveCallback()
     live = callback.live
     spy = mocker.spy(live, "end")
     model.fit(
         x,
@@ -60,16 +58,16 @@
 def test_keras_callback_pass_logger():
     logger = Live("train_logs")
 
     assert DVCLiveCallback().live is not logger
     assert DVCLiveCallback(live=logger).live is logger
 
 
-@pytest.mark.parametrize("save_weights_only", (True, False))
-def test_keras_model_file(tmp_dir, xor_model, mocker, save_weights_only, capture_wrap):
+@pytest.mark.parametrize("save_weights_only", [True, False])
+def test_keras_model_file(tmp_dir, xor_model, mocker, save_weights_only):
     model, x, y = xor_model()
     save = mocker.spy(model, "save")
     save_weights = mocker.spy(model, "save_weights")
 
     live_callback = DVCLiveCallback(
         model_file="model.h5", save_weights_only=save_weights_only
     )
@@ -82,18 +80,16 @@
         callbacks=[live_callback],
     )
     assert save.call_count != save_weights_only
     assert save_weights.call_count == save_weights_only
     log_artifact.assert_called_with(live_callback.model_file)
 
 
-@pytest.mark.parametrize("save_weights_only", (True, False))
-def test_keras_load_model_on_resume(
-    tmp_dir, xor_model, mocker, save_weights_only, capture_wrap
-):
+@pytest.mark.parametrize("save_weights_only", [True, False])
+def test_keras_load_model_on_resume(tmp_dir, xor_model, mocker, save_weights_only):
     import dvclive.keras
 
     model, x, y = xor_model()
 
     if save_weights_only:
         model.save_weights("model.h5")
     else:
@@ -116,15 +112,15 @@
         ],
     )
 
     assert load_model.call_count != save_weights_only
     assert load_weights.call_count == save_weights_only
 
 
-def test_keras_no_resume_skip_load(tmp_dir, xor_model, mocker, capture_wrap):
+def test_keras_no_resume_skip_load(tmp_dir, xor_model, mocker):
     model, x, y = xor_model()
 
     model.save_weights("model.h5")
 
     load_weights = mocker.spy(model, "load_weights")
 
     model.fit(
@@ -140,17 +136,15 @@
             )
         ],
     )
 
     assert load_weights.call_count == 0
 
 
-def test_keras_no_existing_model_file_skip_load(
-    tmp_dir, xor_model, mocker, capture_wrap
-):
+def test_keras_no_existing_model_file_skip_load(tmp_dir, xor_model, mocker):
     model, x, y = xor_model()
 
     load_weights = mocker.spy(model, "load_weights")
 
     model.fit(
         x,
         y,
@@ -164,15 +158,15 @@
             )
         ],
     )
 
     assert load_weights.call_count == 0
 
 
-def test_keras_None_model_file_skip_load(tmp_dir, xor_model, mocker, capture_wrap):
+def test_keras_none_model_file_skip_load(tmp_dir, xor_model, mocker):
     model, x, y = xor_model()
 
     model.save_weights("model.h5")
 
     load_weights = mocker.spy(model, "load_weights")
 
     model.fit(
```

### Comparing `dvclive-2.6.3/tests/test_frameworks/test_lgbm.py` & `dvclive-2.6.4/tests/test_frameworks/test_lgbm.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 from sklearn import datasets
 from sklearn.model_selection import train_test_split
 
 from dvclive import Live
 from dvclive.lgbm import DVCLiveCallback
 from dvclive.utils import parse_metrics
 
-# pylint: disable=redefined-outer-name, unused-argument
 
-
-@pytest.fixture
+@pytest.fixture()
 def model_params():
     return {"objective": "multiclass", "n_estimators": 5, "seed": 0}
 
 
-@pytest.fixture
+@pytest.fixture()
 def iris_data():
     iris = datasets.load_iris()
     x = pd.DataFrame(iris["data"], columns=iris["feature_names"])
     y = iris["target"]
     x_train, x_test, y_train, y_test = train_test_split(
         x, y, test_size=0.33, random_state=42
     )
```

### Comparing `dvclive-2.6.3/tests/test_frameworks/test_lightning.py` & `dvclive-2.6.4/tests/test_frameworks/test_lightning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import os
 
 import torch
 from pytorch_lightning import LightningModule
 from pytorch_lightning.trainer import Trainer
 from torch import nn
-from torch.nn import functional as F
+from torch.nn import functional as F  # noqa: N812
 from torch.optim import Adam
 from torch.utils.data import DataLoader, Dataset
 
 from dvclive.lightning import DVCLiveLogger
 from dvclive.plots.metric import Metric
 from dvclive.serialize import load_yaml
 from dvclive.utils import parse_metrics
 
-# pylint: disable=redefined-outer-name, unused-argument
-
 
 class XORDataset(Dataset):
     def __init__(self, *args, **kwargs):
         self.ins = [[0, 0], [0, 1], [1, 0], [1, 1]]
         self.outs = [1, 0, 0, 1]
 
     def __getitem__(self, index):
@@ -47,20 +45,18 @@
         x = F.relu(x)
         x = self.layer_2(x)
         x = F.log_softmax(x, dim=1)
         return x
 
     def train_loader(self):
         dataset = XORDataset()
-        loader = DataLoader(dataset, batch_size=1)
-        return loader
+        return DataLoader(dataset, batch_size=1)
 
     def train_dataloader(self):
-        loader = self.train_loader()
-        return loader
+        return self.train_loader()
 
     def training_step(self, *args, **kwargs):
         batch = args[0]
         x, y = batch
         logits = self(x)
         loss = F.nll_loss(logits, y)
         self.log(
@@ -180,20 +176,18 @@
     # - 2x log_every_n_steps
     assert spy.call_count == 4
 
 
 class ValLitXOR(LitXOR):
     def val_loader(self):
         dataset = XORDataset()
-        loader = DataLoader(dataset, batch_size=1)
-        return loader
+        return DataLoader(dataset, batch_size=1)
 
     def val_dataloader(self):
-        loader = self.val_loader()
-        return loader
+        return self.val_loader()
 
     def training_step(self, *args, **kwargs):
         batch = args[0]
         x, y = batch
         logits = self(x)
         loss = F.nll_loss(logits, y)
         self.log("train_loss", loss, on_step=True)
```

### Comparing `dvclive-2.6.3/tests/test_frameworks/test_optuna.py` & `dvclive-2.6.4/tests/test_frameworks/test_optuna.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=protected-access, unused-argument
 import optuna
 
 from dvclive.optuna import DVCLiveCallback
 from dvclive.serialize import load_yaml
 from dvclive.utils import parse_json
```

### Comparing `dvclive-2.6.3/tests/test_frameworks/test_xgboost.py` & `dvclive-2.6.4/tests/test_frameworks/test_xgboost.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,21 @@
 import xgboost as xgb
 from sklearn import datasets
 
 from dvclive import Live
 from dvclive.utils import parse_metrics
 from dvclive.xgb import DVCLiveCallback
 
-# pylint: disable=redefined-outer-name, unused-argument
 
-
-@pytest.fixture
+@pytest.fixture()
 def train_params():
     return {"objective": "multi:softmax", "num_class": 3, "seed": 0}
 
 
-@pytest.fixture
+@pytest.fixture()
 def iris_data():
     iris = datasets.load_iris()
     x = pd.DataFrame(iris["data"], columns=iris["feature_names"])
     y = iris["target"]
     return xgb.DMatrix(x, y)
```

### Comparing `dvclive-2.6.3/tests/test_log_artifact.py` & `dvclive-2.6.4/tests/test_log_artifact.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=unused-argument,protected-access
 from dvclive import Live
 
 
 def test_log_artifact(tmp_dir, dvc_repo):
     data = tmp_dir / "data"
     data.touch()
     with Live() as live:
```

### Comparing `dvclive-2.6.3/tests/test_main.py` & `dvclive-2.6.4/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable=protected-access
-# pylint: disable=unused-argument
 import json
 import os
 from io import StringIO
 
 import pytest
 
 from dvclive import Live, env
@@ -40,15 +38,15 @@
 
     s = load_yaml(dvclive.metrics_file)
     assert s["m1"] == 1
     assert "step" not in s
 
 
 @pytest.mark.parametrize(
-    "param_name,param_value",
+    ("param_name", "param_value"),
     [
         ("param_string", "value"),
         ("param_int", 42),
         ("param_float", 42.0),
         ("param_bool_true", True),
         ("param_bool_false", False),
         ("param_list", [1, 2, 3]),
@@ -89,15 +87,15 @@
 
     dvclive.log_params(params)
 
     s = load_yaml(dvclive.params_file)
     assert s == params
 
 
-@pytest.mark.parametrize("resume", (False, True))
+@pytest.mark.parametrize("resume", [False, True])
 def test_log_params_resume(tmp_dir, resume):
     dvclive = Live(resume=resume)
     dvclive.log_param("param", 42)
 
     dvclive = Live(resume=resume)
     assert ("param" in dvclive._params) == resume
 
@@ -189,15 +187,15 @@
     assert os.path.isfile(dvclive.params_file)
 
     dvclive = Live("logs")
     assert not os.path.exists(dvclive.params_file)
 
 
 @pytest.mark.parametrize(
-    "resume, steps, metrics",
+    ("resume", "steps", "metrics"),
     [(True, [0, 1, 2, 3], [0.9, 0.8, 0.7, 0.6]), (False, [0, 1], [0.7, 0.6])],
 )
 def test_continue(tmp_dir, resume, steps, metrics):
     dvclive = Live("logs")
 
     for metric in [0.9, 0.8]:
         dvclive.log_metric("metric", metric)
@@ -347,15 +345,15 @@
         # no `step`
         "foo": 1.0
     }
     log_file = tmp_dir / dvclive.plots_dir / Metric.subfolder / "foo.tsv"
     assert not log_file.exists()
 
 
-@pytest.mark.parametrize("timestamp", (True, False))
+@pytest.mark.parametrize("timestamp", [True, False])
 def test_log_metric_timestamp(tmp_dir, timestamp):
     live = Live()
     live.log_metric("foo", 1.0, timestamp=timestamp)
     live.next_step()
 
     history, _ = parse_metrics(live)
     logged = next(iter(history.values()))
@@ -436,15 +434,15 @@
 
     if dvc_root and set_env:
         assert native_exists(os.path.join(".dvc", "tmp", env.DVC_CHECKPOINT))
     else:
         assert not native_exists(os.path.join(".dvc", "tmp", env.DVC_CHECKPOINT))
 
 
-@pytest.mark.vscode
+@pytest.mark.vscode()
 @pytest.mark.parametrize("dvc_root", [True, False])
 def test_vscode_dvclive_only_signal_file(tmp_dir, dvc_root, mocker):
     signal_file = os.path.join(tmp_dir, ".dvc", "tmp", "exps", "run", "DVCLIVE_ONLY")
     test_pid = 12345
 
     if dvc_root:
         (tmp_dir / ".dvc").mkdir(parents=True)
```

### Comparing `dvclive-2.6.3/tests/test_report.py` & `dvclive-2.6.4/tests/test_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# pylint: disable=unused-argument,protected-access
 import os
 
 import pytest
 from IPython import display
 from PIL import Image
 
 from dvclive import Live
 from dvclive.env import DVCLIVE_OPEN
+from dvclive.error import InvalidReportModeError
 from dvclive.plots import Image as LiveImage
 from dvclive.plots import Metric
 from dvclive.plots.sklearn import ConfusionMatrix, Roc, SKLearnPlot
 from dvclive.report import (
     get_image_renderers,
     get_metrics_renderers,
     get_params_renderers,
@@ -85,15 +85,15 @@
     live = Live()
     assert live._report_mode == "html"
 
     for report in {None, "html", "md"}:
         live = Live(report=report)
         assert live._report_mode == report
 
-    with pytest.raises(ValueError):
+    with pytest.raises(InvalidReportModeError, match="Got foo instead."):
         Live(report="foo")
 
 
 @pytest.mark.parametrize("mode", ["html", "md"])
 def test_make_report(tmp_dir, mode):
     last_report = ""
     live = Live(report=mode)
@@ -104,15 +104,15 @@
         live.next_step()
         assert (tmp_dir / live.report_file).exists()
         current_report = (tmp_dir / live.report_file).read_text()
         assert last_report != current_report
         last_report = current_report
 
 
-@pytest.mark.vscode
+@pytest.mark.vscode()
 def test_make_report_open(tmp_dir, mocker, monkeypatch):
     mocked_open = mocker.patch("webbrowser.open")
     live = Live()
     live.log_sklearn_plot("confusion_matrix", [0, 0, 1, 1], [1, 0, 0, 1])
     live.make_report()
     live.make_report()
```

### Comparing `dvclive-2.6.3/tests/test_studio.py` & `dvclive-2.6.4/tests/test_studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=protected-access,redefined-outer-name,unused-argument
 from pathlib import Path
 
 import pytest
 
 from dvclive import Live
 from dvclive.env import DVC_EXP_BASELINE_REV, DVC_EXP_NAME
 from dvclive.plots import Metric
@@ -84,14 +83,15 @@
     live.end()
     mocked_post.assert_called_with(
         "https://0.0.0.0",
         json={
             "type": "done",
             "repo_url": "STUDIO_REPO_URL",
             "baseline_sha": "f" * 40,
+            "experiment_rev": live._experiment_rev,
             "name": live._exp_name,
             "client": "dvclive",
         },
         headers={
             "Authorization": "token STUDIO_TOKEN",
             "Content-type": "application/json",
         },
@@ -171,30 +171,30 @@
         live.next_step()
 
     assert mocked_post.call_count == 3
     live.end()
     assert mocked_post.call_count == 3
 
 
-@pytest.mark.studio
+@pytest.mark.studio()
 def test_post_to_studio_skip_on_env_var(
     tmp_dir, mocked_dvc_repo, mocked_studio_post, monkeypatch
 ):
     mocked_post, _ = mocked_studio_post
 
     monkeypatch.setenv(DVC_EXP_BASELINE_REV, "f" * 40)
     monkeypatch.setenv(DVC_EXP_NAME, "bar")
 
     with Live() as live:
         live.log_metric("foo", 1)
 
     assert mocked_post.call_count == 1
 
 
-@pytest.mark.studio
+@pytest.mark.studio()
 def test_post_to_studio_skip_if_no_token(
     tmp_dir,
     mocker,
     monkeypatch,
     mocked_dvc_repo,
 ):
     mocked_post = mocker.patch("dvclive.live.post_live_metrics", return_value=None)
@@ -270,15 +270,15 @@
             "Authorization": "token STUDIO_TOKEN",
             "Content-type": "application/json",
         },
         timeout=5,
     )
 
 
-@pytest.mark.studio
+@pytest.mark.studio()
 def test_post_to_studio_inside_dvc_exp(
     tmp_dir, mocker, monkeypatch, mocked_studio_post
 ):
     mocked_post, _ = mocked_studio_post
     mocker.patch("dvclive.live.get_dvc_repo", return_value=None)
 
     monkeypatch.setenv(DVC_EXP_BASELINE_REV, "f" * 40)
@@ -286,15 +286,15 @@
 
     with Live() as live:
         live.log_metric("foo", 1)
 
     assert mocked_post.call_count == 1
 
 
-@pytest.mark.studio
+@pytest.mark.studio()
 def test_post_to_studio_inside_subdir(
     tmp_dir, dvc_repo, mocker, monkeypatch, mocked_studio_post
 ):
     mocked_post, _ = mocked_studio_post
     subdir = tmp_dir / "subdir"
     subdir.mkdir()
     monkeypatch.chdir(subdir)
@@ -327,15 +327,15 @@
             "Authorization": "token STUDIO_TOKEN",
             "Content-type": "application/json",
         },
         timeout=5,
     )
 
 
-@pytest.mark.studio
+@pytest.mark.studio()
 def test_post_to_studio_inside_subdir_dvc_exp(
     tmp_dir, dvc_repo, monkeypatch, mocked_studio_post
 ):
     mocked_post, _ = mocked_studio_post
     subdir = tmp_dir / "subdir"
     subdir.mkdir()
     monkeypatch.chdir(subdir)
```

### Comparing `dvclive-2.6.3/tests/test_utils.py` & `dvclive-2.6.4/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 
 from dvclive.utils import standardize_metric_name
 
 
 @pytest.mark.parametrize(
-    "framework,logged,standardized",
+    ("framework", "logged", "standardized"),
     [
         ("dvclive.lightning", "epoch", "epoch"),
         ("dvclive.lightning", "train_loss", "train/loss"),
         ("dvclive.lightning", "train_loss_epoch", "train/epoch/loss"),
         ("dvclive.lightning", "train_model_error", "train/model_error"),
         ("dvclive.lightning", "grad_step", "grad_step"),
     ],
```

