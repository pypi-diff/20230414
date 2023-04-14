# Comparing `tmp/pyDVL-0.6.0.tar.gz` & `tmp/pyDVL-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDVL-0.6.0.tar", last modified: Thu Mar 16 11:09:49 2023, max compression
+gzip compressed data, was "pyDVL-0.6.1.tar", last modified: Fri Apr 14 07:50:25 2023, max compression
```

## Comparing `pyDVL-0.6.0.tar` & `pyDVL-0.6.1.tar`

### file list

```diff
@@ -1,82 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.370434 pyDVL-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-16 11:08:39.000000 pyDVL-0.6.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-16 11:08:39.000000 pyDVL-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-16 11:08:39.000000 pyDVL-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-03-16 11:09:49.370434 pyDVL-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-03-16 11:08:39.000000 pyDVL-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-03-16 11:08:39.000000 pyDVL-0.6.0/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-16 11:08:39.000000 pyDVL-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-16 11:08:39.000000 pyDVL-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 11:09:49.370434 pyDVL-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-16 11:08:39.000000 pyDVL-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.330434 pyDVL-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.342434 pyDVL-0.6.0/src/pyDVL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-03-16 11:09:49.000000 pyDVL-0.6.0/src/pyDVL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-16 11:09:49.000000 pyDVL-0.6.0/src/pyDVL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 11:09:49.000000 pyDVL-0.6.0/src/pyDVL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 11:09:49.000000 pyDVL-0.6.0/src/pyDVL.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-16 11:09:49.000000 pyDVL-0.6.0/src/pyDVL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-16 11:09:49.000000 pyDVL-0.6.0/src/pyDVL.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.342434 pyDVL-0.6.0/src/pydvl/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.346434 pyDVL-0.6.0/src/pydvl/influence/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/influence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/influence/conjugate_gradient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.346434 pyDVL-0.6.0/src/pydvl/influence/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/influence/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/influence/frameworks/torch_differentiable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/influence/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/influence/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.350434 pyDVL-0.6.0/src/pydvl/influence/model_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/influence/model_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/influence/model_wrappers/torch_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/influence/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.350434 pyDVL-0.6.0/src/pydvl/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/reporting/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/reporting/scores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.354434 pyDVL-0.6.0/src/pydvl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    28186 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.358434 pyDVL-0.6.0/src/pydvl/utils/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/parallel/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/parallel/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/parallel/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/utils/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.362434 pyDVL-0.6.0/src/pydvl/value/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.362434 pyDVL-0.6.0/src/pydvl/value/least_core/
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/least_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/least_core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/least_core/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/least_core/naive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.366434 pyDVL-0.6.0/src/pydvl/value/loo/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/loo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/loo/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    29000 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/semivalues.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.370434 pyDVL-0.6.0/src/pydvl/value/shapley/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/shapley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/shapley/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/shapley/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/shapley/gt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/shapley/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/shapley/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/shapley/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/shapley/owen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/shapley/truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/shapley/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    19162 2023-03-16 11:08:39.000000 pyDVL-0.6.0/src/pydvl/value/stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:09:49.370434 pyDVL-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-16 11:08:39.000000 pyDVL-0.6.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-03-16 11:08:39.000000 pyDVL-0.6.0/tests/test_results.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.489523 pyDVL-0.6.1/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      444 2023-04-14 07:49:35.000000 pyDVL-0.6.1/.bumpversion.cfg
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.481523 pyDVL-0.6.1/.github/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      452 2022-11-25 07:24:10.000000 pyDVL-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.481523 pyDVL-0.6.1/.github/workflows/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     2435 2023-04-13 13:32:48.000000 pyDVL-0.6.1/.github/workflows/publish.yaml
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1282 2023-03-10 17:46:58.000000 pyDVL-0.6.1/.github/workflows/run-tests-workflow.yaml
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      800 2023-03-10 17:46:58.000000 pyDVL-0.6.1/.github/workflows/stale.yaml
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     4418 2023-03-10 17:46:58.000000 pyDVL-0.6.1/.github/workflows/tox.yaml
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1892 2023-03-10 17:46:58.000000 pyDVL-0.6.1/.gitignore
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      461 2023-03-10 17:46:58.000000 pyDVL-0.6.1/.pre-commit-config.yaml
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      263 2022-09-12 10:11:18.000000 pyDVL-0.6.1/.readthedocs.yaml
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     9530 2023-04-13 12:12:45.000000 pyDVL-0.6.1/CHANGELOG.md
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    15937 2023-04-13 12:12:36.000000 pyDVL-0.6.1/CONTRIBUTING.md
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     7652 2022-10-11 16:21:51.000000 pyDVL-0.6.1/COPYING.LESSER
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    35149 2022-10-11 16:21:51.000000 pyDVL-0.6.1/LICENSE
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       79 2022-10-11 16:21:51.000000 pyDVL-0.6.1/MANIFEST.in
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     8990 2023-04-14 07:50:25.489523 pyDVL-0.6.1/PKG-INFO
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     6683 2023-04-13 12:12:36.000000 pyDVL-0.6.1/README.md
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.481523 pyDVL-0.6.1/apt-cache/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       13 2022-09-12 10:11:18.000000 pyDVL-0.6.1/apt-cache/.gitignore
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.481523 pyDVL-0.6.1/badges/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       14 2022-09-12 10:11:18.000000 pyDVL-0.6.1/badges/.gitignore
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.481523 pyDVL-0.6.1/build_scripts/
+-rwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     7130 2023-04-13 13:31:47.000000 pyDVL-0.6.1/build_scripts/release-version.sh
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      659 2022-09-12 10:11:18.000000 pyDVL-0.6.1/build_scripts/run_pylint.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     8393 2023-03-10 17:46:58.000000 pyDVL-0.6.1/build_scripts/update_docs.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.481523 pyDVL-0.6.1/data/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)   254987 2022-09-12 10:11:18.000000 pyDVL-0.6.1/data/top_hits_spotify_dataset.csv
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.481523 pyDVL-0.6.1/docs/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       77 2022-10-11 16:21:51.000000 pyDVL-0.6.1/docs/.gitignore
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1379 2023-03-10 17:46:58.000000 pyDVL-0.6.1/docs/10-getting-started.rst
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     2107 2023-03-10 17:46:58.000000 pyDVL-0.6.1/docs/20-install.rst
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    28494 2023-04-13 12:12:36.000000 pyDVL-0.6.1/docs/30-data-valuation.rst
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     3364 2023-03-10 17:46:58.000000 pyDVL-0.6.1/docs/40-influence.rst
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.481523 pyDVL-0.6.1/docs/_ext/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1217 2022-11-25 07:24:10.000000 pyDVL-0.6.1/docs/_ext/copy_notebooks.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    14198 2023-04-13 12:06:34.000000 pyDVL-0.6.1/docs/conf.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.481523 pyDVL-0.6.1/docs/examples/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      280 2023-03-10 17:46:58.000000 pyDVL-0.6.1/docs/examples/index.rst
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1864 2023-03-10 17:46:58.000000 pyDVL-0.6.1/docs/index.rst
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.481523 pyDVL-0.6.1/docs/pydvl/
+-rw-rw-rw-   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      113 2023-04-03 10:46:43.000000 pyDVL-0.6.1/docs/pydvl/index.rst
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    19752 2023-04-13 12:12:36.000000 pyDVL-0.6.1/docs/pydvl.bib
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2022-09-12 10:11:18.000000 pyDVL-0.6.1/docs/requirements.txt
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     9828 2022-10-04 11:07:42.000000 pyDVL-0.6.1/logo.svg
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/notebooks/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)  1097817 2023-03-11 10:22:05.000000 pyDVL-0.6.1/notebooks/influence_imagenet.ipynb
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)   816303 2023-03-11 10:22:05.000000 pyDVL-0.6.1/notebooks/influence_synthetic.ipynb
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)   155077 2023-03-11 10:22:05.000000 pyDVL-0.6.1/notebooks/influence_wine.ipynb
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)   382024 2023-04-13 12:06:34.000000 pyDVL-0.6.1/notebooks/least_core_basic.ipynb
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    24440 2023-04-13 12:06:34.000000 pyDVL-0.6.1/notebooks/notebook_support.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)   357051 2023-04-13 12:12:36.000000 pyDVL-0.6.1/notebooks/shapley_basic_spotify.ipynb
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)   474876 2023-04-13 12:06:34.000000 pyDVL-0.6.1/notebooks/shapley_knn_flowers.ipynb
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)   349135 2023-04-13 12:12:36.000000 pyDVL-0.6.1/notebooks/shapley_utility_learning.ipynb
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1293 2022-10-04 11:07:42.000000 pyDVL-0.6.1/notebooks/test_notebooks.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/public/
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/public/coverage/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       14 2022-09-12 10:11:18.000000 pyDVL-0.6.1/public/coverage/.gitignore
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/public/docs/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       14 2022-09-12 10:11:18.000000 pyDVL-0.6.1/public/docs/.gitignore
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      609 2022-09-12 10:11:18.000000 pyDVL-0.6.1/public/index.html
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/public/pylint/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       17 2022-09-12 10:11:18.000000 pyDVL-0.6.1/public/pylint/.gitignore
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1545 2023-03-21 18:46:04.000000 pyDVL-0.6.1/pyproject.toml
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      269 2023-04-13 12:06:34.000000 pyDVL-0.6.1/requirements-dev.txt
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       64 2023-03-10 17:46:58.000000 pyDVL-0.6.1/requirements-notebooks.txt
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      137 2023-04-13 12:06:34.000000 pyDVL-0.6.1/requirements.txt
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       38 2023-04-14 07:50:25.489523 pyDVL-0.6.1/setup.cfg
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1738 2023-04-14 07:49:35.000000 pyDVL-0.6.1/setup.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.477523 pyDVL-0.6.1/src/
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pyDVL.egg-info/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     8990 2023-04-14 07:50:25.000000 pyDVL-0.6.1/src/pyDVL.egg-info/PKG-INFO
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     4005 2023-04-14 07:50:25.000000 pyDVL-0.6.1/src/pyDVL.egg-info/SOURCES.txt
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        1 2023-04-14 07:50:25.000000 pyDVL-0.6.1/src/pyDVL.egg-info/dependency_links.txt
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        1 2023-03-10 14:34:44.000000 pyDVL-0.6.1/src/pyDVL.egg-info/not-zip-safe
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      156 2023-04-14 07:50:25.000000 pyDVL-0.6.1/src/pyDVL.egg-info/requires.txt
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        6 2023-04-14 07:50:25.000000 pyDVL-0.6.1/src/pyDVL.egg-info/top_level.txt
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pydvl/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       22 2023-04-14 07:49:35.000000 pyDVL-0.6.1/src/pydvl/__init__.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pydvl/influence/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      301 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/influence/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     8069 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/influence/conjugate_gradient.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pydvl/influence/frameworks/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       83 2022-10-11 16:21:51.000000 pyDVL-0.6.1/src/pydvl/influence/frameworks/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     6392 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/influence/frameworks/torch_differentiable.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     9109 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/influence/general.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     5334 2022-11-25 07:24:11.000000 pyDVL-0.6.1/src/pydvl/influence/linear.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pydvl/influence/model_wrappers/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      127 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/influence/model_wrappers/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    10477 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/influence/model_wrappers/torch_wrappers.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1305 2022-10-11 16:21:51.000000 pyDVL-0.6.1/src/pydvl/influence/types.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/py.typed
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pydvl/reporting/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2022-10-11 16:21:51.000000 pyDVL-0.6.1/src/pydvl/reporting/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     7648 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/reporting/plots.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1770 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/reporting/scores.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pydvl/utils/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      226 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/utils/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    13363 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/utils/caching.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     3812 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/utils/config.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    28783 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/utils/dataset.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    10807 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/utils/numeric.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pydvl/utils/parallel/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       72 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/utils/parallel/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     7885 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/utils/parallel/backend.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pydvl/utils/parallel/futures/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1872 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/utils/parallel/futures/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    14534 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/utils/parallel/futures/ray.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    11094 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/utils/parallel/map_reduce.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1792 2022-10-11 16:21:51.000000 pyDVL-0.6.1/src/pydvl/utils/progress.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     4673 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/utils/score.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     3040 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/utils/status.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1488 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/utils/types.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    17286 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/utils/utility.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pydvl/value/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      404 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/__init__.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.485523 pyDVL-0.6.1/src/pydvl/value/least_core/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     4333 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/least_core/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    12293 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/least_core/common.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     6105 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/least_core/montecarlo.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     3984 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/least_core/naive.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.489523 pyDVL-0.6.1/src/pydvl/value/loo/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)       21 2022-11-25 18:31:17.000000 pyDVL-0.6.1/src/pydvl/value/loo/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1057 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/value/loo/naive.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    29000 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/result.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    11567 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/sampler.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     8232 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/value/semivalues.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.489523 pyDVL-0.6.1/src/pydvl/value/shapley/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      525 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/shapley/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     7415 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/value/shapley/common.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     9693 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/value/shapley/gt.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     3273 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/value/shapley/knn.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     9901 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/shapley/montecarlo.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     4661 2023-03-10 17:46:58.000000 pyDVL-0.6.1/src/pydvl/value/shapley/naive.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     6154 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/shapley/owen.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     9939 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/value/shapley/truncated.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      621 2023-04-13 12:12:36.000000 pyDVL-0.6.1/src/pydvl/value/shapley/types.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    19162 2023-04-13 12:06:34.000000 pyDVL-0.6.1/src/pydvl/value/stopping.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.489523 pyDVL-0.6.1/tests/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2022-09-12 10:11:18.000000 pyDVL-0.6.1/tests/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    12978 2023-04-13 12:06:34.000000 pyDVL-0.6.1/tests/conftest.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      141 2022-09-12 10:11:18.000000 pyDVL-0.6.1/tests/docker-compose.yml
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.489523 pyDVL-0.6.1/tests/influence/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2022-09-12 10:11:18.000000 pyDVL-0.6.1/tests/influence/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     3025 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/influence/conftest.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     3479 2022-10-11 16:21:51.000000 pyDVL-0.6.1/tests/influence/test_conjugate_gradients.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     9827 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/influence/test_influences.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     6995 2022-11-25 07:24:11.000000 pyDVL-0.6.1/tests/influence/test_models.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1399 2022-09-12 10:11:18.000000 pyDVL-0.6.1/tests/test_plugin.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)    12576 2023-04-13 12:06:34.000000 pyDVL-0.6.1/tests/test_results.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.489523 pyDVL-0.6.1/tests/utils/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2022-09-12 10:11:18.000000 pyDVL-0.6.1/tests/utils/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      824 2023-04-13 12:12:36.000000 pyDVL-0.6.1/tests/utils/conftest.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     5491 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/utils/test_caching.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     4241 2023-04-13 12:12:36.000000 pyDVL-0.6.1/tests/utils/test_dataset.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     4786 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/utils/test_numeric.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     8178 2023-04-13 12:12:36.000000 pyDVL-0.6.1/tests/utils/test_parallel.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     2022 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/utils/test_score.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     2106 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/utils/test_status.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     3203 2023-03-19 12:26:22.000000 pyDVL-0.6.1/tests/utils/test_utility.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.489523 pyDVL-0.6.1/tests/value/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     3464 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/value/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     4374 2023-04-13 12:12:36.000000 pyDVL-0.6.1/tests/value/conftest.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.489523 pyDVL-0.6.1/tests/value/least_core/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/value/least_core/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      883 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/value/least_core/conftest.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1046 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/value/least_core/test_common.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1218 2023-04-13 12:06:34.000000 pyDVL-0.6.1/tests/value/least_core/test_montecarlo.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1114 2023-04-13 12:06:34.000000 pyDVL-0.6.1/tests/value/least_core/test_naive.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.489523 pyDVL-0.6.1/tests/value/loo/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/value/loo/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)      441 2023-03-19 12:26:22.000000 pyDVL-0.6.1/tests/value/loo/test_loo.py
+drwxrwxr-x   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-04-14 07:50:25.489523 pyDVL-0.6.1/tests/value/shapley/
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)        0 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/value/shapley/__init__.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     1810 2023-03-10 17:46:58.000000 pyDVL-0.6.1/tests/value/shapley/test_knn.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     8060 2023-04-13 12:12:36.000000 pyDVL-0.6.1/tests/value/shapley/test_montecarlo.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     5807 2023-03-19 12:26:22.000000 pyDVL-0.6.1/tests/value/shapley/test_naive.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     5486 2023-04-13 12:06:34.000000 pyDVL-0.6.1/tests/value/test_stopping.py
+-rw-rw-r--   0 anesbenmerzoug  (1000) anesbenmerzoug  (1000)     3649 2023-04-13 12:06:34.000000 pyDVL-0.6.1/tox.ini
```

### Comparing `pyDVL-0.6.0/COPYING.LESSER` & `pyDVL-0.6.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/LICENSE` & `pyDVL-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/PKG-INFO` & `pyDVL-0.6.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: pyDVL
-Version: 0.6.0
-Summary: The Python Data Valuation Library
-Author: appliedAI Institute gGmbH
-Project-URL: Source, https://github.com/appliedAI-Initiative/pydvl
-Project-URL: Documentation, https://appliedai-initiative.github.io/pyDVL
-Project-URL: TransferLab, https://transferlab.appliedai.de
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Typing :: Typed
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Description-Content-Type: text/markdown
-Provides-Extra: influence
-License-File: LICENSE
-License-File: COPYING.LESSER
-
 <p align="center" style="text-align:center;">
     <img alt="pyDVL Logo" src="https://raw.githubusercontent.com/appliedAI-Initiative/pyDVL/develop/logo.svg" width="200"/>
 </p>
 
 <p align="center" style="text-align:center;">
     A library for data valuation.
 </p>
@@ -52,50 +28,55 @@
 
 pyDVL collects algorithms for Data Valuation and Influence Function computation.
 
 Data Valuation is the task of estimating the intrinsic value of a data point
 wrt. the training set, the model and a scoring function. We currently implement
 methods from the following papers:
 
-- Ghorbani, Amirata, and James Zou. 
-  [Data Shapley: Equitable Valuation of Data for Machine Learning](http://proceedings.mlr.press/v97/ghorbani19c.html).
-  In International Conference on Machine Learning, 2242–51. PMLR, 2019.
+- Castro, Javier, Daniel Gómez, and Juan Tejada. [Polynomial Calculation of the
+  Shapley Value Based on Sampling](https://doi.org/10.1016/j.cor.2008.04.004).
+  Computers & Operations Research, Selected papers presented at the Tenth
+  International Symposium on Locational Decisions (ISOLDE X), 36, no. 5 (May 1,
+  2009): 1726–30.
+- Ghorbani, Amirata, and James Zou. [Data Shapley: Equitable Valuation of Data
+  for Machine Learning](http://proceedings.mlr.press/v97/ghorbani19c.html). In
+  International Conference on Machine Learning, 2242–51. PMLR, 2019.
 - Wang, Tianhao, Yu Yang, and Ruoxi Jia. 
-  [Improving Cooperative Game Theory-Based Data Valuation via Data Utility Learning](https://doi.org/10.48550/arXiv.2107.06336).
-  arXiv, 2022.
-- Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nezihe Merve Gurel, Bo Li,
-  Ce Zhang, Costas Spanos, and Dawn Song.
-  [Efficient Task-Specific Data Valuation for Nearest Neighbor Algorithms](https://doi.org/10.14778/3342263.3342637).
+  [Improving Cooperative Game Theory-Based Data Valuation via Data Utility
+  Learning](https://doi.org/10.48550/arXiv.2107.06336). arXiv, 2022.
+- Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nezihe Merve Gurel, Bo
+  Li, Ce Zhang, Costas Spanos, and Dawn Song. [Efficient Task-Specific Data
+  Valuation for Nearest Neighbor Algorithms](https://doi.org/10.14778/3342263.3342637).
   Proceedings of the VLDB Endowment 12, no. 11 (1 July 2019): 1610–23.
-- Okhrati, Ramin, and Aldo Lipani.
-  [A Multilinear Sampling Algorithm to Estimate Shapley Values](https://doi.org/10.1109/ICPR48806.2021.9412511).
-  In 25th International Conference on Pattern Recognition (ICPR 2020), 7992–99.
-  IEEE, 2021.
-- Yan, T., & Procaccia, A. D.
-  [If You Like Shapley Then You’ll Love the Core]().
-  Proceedings of the AAAI Conference on Artificial Intelligence, 35(6) (2021): 5751-5759.
+- Okhrati, Ramin, and Aldo Lipani. [A Multilinear Sampling Algorithm to Estimate
+  Shapley Values](https://doi.org/10.1109/ICPR48806.2021.9412511). In 25th
+  International Conference on Pattern Recognition (ICPR 2020), 7992–99. IEEE,
+  2021.
+- Yan, T., & Procaccia, A. D. [If You Like Shapley Then You’ll Love the
+  Core](https://ojs.aaai.org/index.php/AAAI/article/view/16721). Proceedings of
+  the AAAI Conference on Artificial Intelligence, 35(6) (2021): 5751-5759.
 - Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nick Hynes, Nezihe Merve
-  Gürel, Bo Li, Ce Zhang, Dawn Song, and Costas J. Spanos.
-  [Towards Efficient Data Valuation Based on the Shapley Value](http://proceedings.mlr.press/v89/jia19a.html).
+  Gürel, Bo Li, Ce Zhang, Dawn Song, and Costas J. Spanos. [Towards Efficient
+  Data Valuation Based on the Shapley Value](http://proceedings.mlr.press/v89/jia19a.html).
   In 22nd International Conference on Artificial Intelligence and Statistics,
   1167–76. PMLR, 2019.
-- Wang, Jiachen T., and Ruoxi Jia. 
-  [Data Banzhaf: A Robust Data Valuation Framework for Machine Learning](https://doi.org/10.48550/arXiv.2205.15466).
+- Wang, Jiachen T., and Ruoxi Jia. [Data Banzhaf: A Robust Data Valuation
+  Framework for Machine Learning](https://doi.org/10.48550/arXiv.2205.15466).
   arXiv, October 22, 2022.
-- Kwon, Yongchan, and James Zou.
-  [Beta Shapley: A Unified and Noise-Reduced Data Valuation Framework for Machine Learning](http://arxiv.org/abs/2110.14049).
+- Kwon, Yongchan, and James Zou. [Beta Shapley: A Unified and Noise-Reduced Data
+  Valuation Framework for Machine Learning](http://arxiv.org/abs/2110.14049).
   In Proceedings of the 25th International Conference on Artificial Intelligence
   and Statistics (AISTATS) 2022, Vol. 151. Valencia, Spain: PMLR, 2022.
 
 Influence Functions compute the effect that single points have on an estimator /
 model. We implement methods from the following papers:
 
-- Koh, Pang Wei, and Percy Liang.
-  [Understanding Black-Box Predictions via Influence Functions](http://proceedings.mlr.press/v70/koh17a.html).
-  In Proceedings of the 34th International Conference on Machine Learning,
+- Koh, Pang Wei, and Percy Liang. [Understanding Black-Box Predictions via
+  Influence Functions](http://proceedings.mlr.press/v70/koh17a.html). In
+  Proceedings of the 34th International Conference on Machine Learning,
   70:1885–94. Sydney, Australia: PMLR, 2017.
 
 # Installation
 
 To install the latest release use:
 
 ```shell
```

#### html2text {}

```diff
@@ -1,89 +1,81 @@
-Metadata-Version: 2.1 Name: pyDVL Version: 0.6.0 Summary: The Python Data
-Valuation Library Author: appliedAI Institute gGmbH Project-URL: Source, https:
-//github.com/appliedAI-Initiative/pydvl Project-URL: Documentation, https://
-appliedai-initiative.github.io/pyDVL Project-URL: TransferLab, https://
-transferlab.appliedai.de Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Typing :: Typed Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
-:: Windows Classifier: Operating System :: POSIX Classifier: License :: OSI
-Approved :: GNU Lesser General Public License v3 (LGPLv3) Description-Content-
-Type: text/markdown Provides-Extra: influence License-File: LICENSE License-
-File: COPYING.LESSER
                                  [pyDVL Logo]
                          A library for data valuation.
                                 [Build_Status]
     [https://img.shields.io/pypi/v/pydvl.svg] [https://img.shields.io/pypi/
                     pyversions/pydvl.svg] [PyPI - License]
                                      Docs
 pyDVL collects algorithms for Data Valuation and Influence Function
 computation. Data Valuation is the task of estimating the intrinsic value of a
 data point wrt. the training set, the model and a scoring function. We
-currently implement methods from the following papers: - Ghorbani, Amirata, and
-James Zou. [Data Shapley: Equitable Valuation of Data for Machine Learning]
-(http://proceedings.mlr.press/v97/ghorbani19c.html). In International
-Conference on Machine Learning, 2242â51. PMLR, 2019. - Wang, Tianhao, Yu
-Yang, and Ruoxi Jia. [Improving Cooperative Game Theory-Based Data Valuation
-via Data Utility Learning](https://doi.org/10.48550/arXiv.2107.06336). arXiv,
-2022. - Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nezihe Merve
-Gurel, Bo Li, Ce Zhang, Costas Spanos, and Dawn Song. [Efficient Task-Specific
-Data Valuation for Nearest Neighbor Algorithms](https://doi.org/10.14778/
-3342263.3342637). Proceedings of the VLDB Endowment 12, no. 11 (1 July 2019):
-1610â23. - Okhrati, Ramin, and Aldo Lipani. [A Multilinear Sampling Algorithm
-to Estimate Shapley Values](https://doi.org/10.1109/ICPR48806.2021.9412511). In
-25th International Conference on Pattern Recognition (ICPR 2020), 7992â99.
-IEEE, 2021. - Yan, T., & Procaccia, A. D. [If You Like Shapley Then Youâll
-Love the Core](). Proceedings of the AAAI Conference on Artificial
-Intelligence, 35(6) (2021): 5751-5759. - Jia, Ruoxi, David Dao, Boxin Wang,
-Frances Ann Hubis, Nick Hynes, Nezihe Merve GÃ¼rel, Bo Li, Ce Zhang, Dawn Song,
-and Costas J. Spanos. [Towards Efficient Data Valuation Based on the Shapley
-Value](http://proceedings.mlr.press/v89/jia19a.html). In 22nd International
-Conference on Artificial Intelligence and Statistics, 1167â76. PMLR, 2019. -
-Wang, Jiachen T., and Ruoxi Jia. [Data Banzhaf: A Robust Data Valuation
-Framework for Machine Learning](https://doi.org/10.48550/arXiv.2205.15466).
-arXiv, October 22, 2022. - Kwon, Yongchan, and James Zou. [Beta Shapley: A
-Unified and Noise-Reduced Data Valuation Framework for Machine Learning](http:/
-/arxiv.org/abs/2110.14049). In Proceedings of the 25th International Conference
-on Artificial Intelligence and Statistics (AISTATS) 2022, Vol. 151. Valencia,
-Spain: PMLR, 2022. Influence Functions compute the effect that single points
-have on an estimator / model. We implement methods from the following papers: -
-Koh, Pang Wei, and Percy Liang. [Understanding Black-Box Predictions via
-Influence Functions](http://proceedings.mlr.press/v70/koh17a.html). In
-Proceedings of the 34th International Conference on Machine Learning, 70:
-1885â94. Sydney, Australia: PMLR, 2017. # Installation To install the latest
-release use: ```shell $ pip install pyDVL ``` You can also install the latest
-development version from [TestPyPI](https://test.pypi.org/project/pyDVL/):
-```shell pip install pyDVL --index-url https://test.pypi.org/simple/ ``` For
-more instructions and information refer to [Installing pyDVL ](https://
-appliedAI-Initiative.github.io/pyDVL/20-install.html) in the documentation. #
-Usage The steps required to compute values for your samples are: 1. Create a
-`Dataset` object with your train and test splits. 2. Create an instance of a
-`SupervisedModel` (basically any sklearn compatible predictor) 3. Create a
-`Utility` object to wrap the Dataset, the model and a scoring function. 4. Use
-one of the methods defined in the library to compute the values. This is how it
-looks for *Truncated Montecarlo Shapley*, an efficient method for Data Shapley
-values: ```python from sklearn.datasets import load_breast_cancer from
-sklearn.linear_model import LogisticRegression from pydvl.value import * data =
-Dataset.from_sklearn(load_breast_cancer(), train_size=0.7) model =
-LogisticRegression() u = Utility(model, data, Scorer("accuracy", default=0.0))
-values = compute_shapley_values( u, mode=ShapleyMode.TruncatedMontecarlo,
-done=MaxUpdates(100) | AbsoluteStandardError(threshold=0.01),
-truncation=RelativeTruncation(u, rtol=0.01), ) ``` For more instructions and
-information refer to [Getting Started](https://appliedAI-Initiative.github.io/
-pyDVL/10-getting-started.html) in the documentation. We provide several
-[examples](https://appliedAI-Initiative.github.io/pyDVL/examples/index.html)
-with details on the algorithms and their applications. ## Caching pyDVL offers
-the possibility to cache certain results and speed up computation. It uses
-[Memcached](https://memcached.org/) For that. You can run it either locally or,
-using [Docker](https://www.docker.com/): ```shell docker container run --rm -
-p 11211:11211 --name pydvl-cache -d memcached:latest ``` You can read more in
-the [caching module's documentation](https://appliedAI-Initiative.github.io/
-pyDVL/pydvl/utils/caching.html). # Contributing Please open new issues for
-bugs, feature requests and extensions. You can read about the structure of the
-project, the toolchain and workflow in the [guide for contributions]
-(CONTRIBUTING.md). # License pyDVL is distributed under [LGPL-3.0](https://
-www.gnu.org/licenses/lgpl-3.0.html). A complete version can be found in two
-files: [here](LICENSE) and [here](COPYING.LESSER). All contributions will be
-distributed under this license.
+currently implement methods from the following papers: - Castro, Javier, Daniel
+GÃ³mez, and Juan Tejada. [Polynomial Calculation of the Shapley Value Based on
+Sampling](https://doi.org/10.1016/j.cor.2008.04.004). Computers & Operations
+Research, Selected papers presented at the Tenth International Symposium on
+Locational Decisions (ISOLDE X), 36, no. 5 (May 1, 2009): 1726â30. -
+Ghorbani, Amirata, and James Zou. [Data Shapley: Equitable Valuation of Data
+for Machine Learning](http://proceedings.mlr.press/v97/ghorbani19c.html). In
+International Conference on Machine Learning, 2242â51. PMLR, 2019. - Wang,
+Tianhao, Yu Yang, and Ruoxi Jia. [Improving Cooperative Game Theory-Based Data
+Valuation via Data Utility Learning](https://doi.org/10.48550/
+arXiv.2107.06336). arXiv, 2022. - Jia, Ruoxi, David Dao, Boxin Wang, Frances
+Ann Hubis, Nezihe Merve Gurel, Bo Li, Ce Zhang, Costas Spanos, and Dawn Song.
+[Efficient Task-Specific Data Valuation for Nearest Neighbor Algorithms](https:
+//doi.org/10.14778/3342263.3342637). Proceedings of the VLDB Endowment 12, no.
+11 (1 July 2019): 1610â23. - Okhrati, Ramin, and Aldo Lipani. [A Multilinear
+Sampling Algorithm to Estimate Shapley Values](https://doi.org/10.1109/
+ICPR48806.2021.9412511). In 25th International Conference on Pattern
+Recognition (ICPR 2020), 7992â99. IEEE, 2021. - Yan, T., & Procaccia, A. D.
+[If You Like Shapley Then Youâll Love the Core](https://ojs.aaai.org/
+index.php/AAAI/article/view/16721). Proceedings of the AAAI Conference on
+Artificial Intelligence, 35(6) (2021): 5751-5759. - Jia, Ruoxi, David Dao,
+Boxin Wang, Frances Ann Hubis, Nick Hynes, Nezihe Merve GÃ¼rel, Bo Li, Ce
+Zhang, Dawn Song, and Costas J. Spanos. [Towards Efficient Data Valuation Based
+on the Shapley Value](http://proceedings.mlr.press/v89/jia19a.html). In 22nd
+International Conference on Artificial Intelligence and Statistics, 1167â76.
+PMLR, 2019. - Wang, Jiachen T., and Ruoxi Jia. [Data Banzhaf: A Robust Data
+Valuation Framework for Machine Learning](https://doi.org/10.48550/
+arXiv.2205.15466). arXiv, October 22, 2022. - Kwon, Yongchan, and James Zou.
+[Beta Shapley: A Unified and Noise-Reduced Data Valuation Framework for Machine
+Learning](http://arxiv.org/abs/2110.14049). In Proceedings of the 25th
+International Conference on Artificial Intelligence and Statistics (AISTATS)
+2022, Vol. 151. Valencia, Spain: PMLR, 2022. Influence Functions compute the
+effect that single points have on an estimator / model. We implement methods
+from the following papers: - Koh, Pang Wei, and Percy Liang. [Understanding
+Black-Box Predictions via Influence Functions](http://proceedings.mlr.press/
+v70/koh17a.html). In Proceedings of the 34th International Conference on
+Machine Learning, 70:1885â94. Sydney, Australia: PMLR, 2017. # Installation
+To install the latest release use: ```shell $ pip install pyDVL ``` You can
+also install the latest development version from [TestPyPI](https://
+test.pypi.org/project/pyDVL/): ```shell pip install pyDVL --index-url https://
+test.pypi.org/simple/ ``` For more instructions and information refer to
+[Installing pyDVL ](https://appliedAI-Initiative.github.io/pyDVL/20-
+install.html) in the documentation. # Usage The steps required to compute
+values for your samples are: 1. Create a `Dataset` object with your train and
+test splits. 2. Create an instance of a `SupervisedModel` (basically any
+sklearn compatible predictor) 3. Create a `Utility` object to wrap the Dataset,
+the model and a scoring function. 4. Use one of the methods defined in the
+library to compute the values. This is how it looks for *Truncated Montecarlo
+Shapley*, an efficient method for Data Shapley values: ```python from
+sklearn.datasets import load_breast_cancer from sklearn.linear_model import
+LogisticRegression from pydvl.value import * data = Dataset.from_sklearn
+(load_breast_cancer(), train_size=0.7) model = LogisticRegression() u = Utility
+(model, data, Scorer("accuracy", default=0.0)) values = compute_shapley_values
+( u, mode=ShapleyMode.TruncatedMontecarlo, done=MaxUpdates(100) |
+AbsoluteStandardError(threshold=0.01), truncation=RelativeTruncation(u,
+rtol=0.01), ) ``` For more instructions and information refer to [Getting
+Started](https://appliedAI-Initiative.github.io/pyDVL/10-getting-started.html)
+in the documentation. We provide several [examples](https://appliedAI-
+Initiative.github.io/pyDVL/examples/index.html) with details on the algorithms
+and their applications. ## Caching pyDVL offers the possibility to cache
+certain results and speed up computation. It uses [Memcached](https://
+memcached.org/) For that. You can run it either locally or, using [Docker]
+(https://www.docker.com/): ```shell docker container run --rm -p 11211:11211 --
+name pydvl-cache -d memcached:latest ``` You can read more in the [caching
+module's documentation](https://appliedAI-Initiative.github.io/pyDVL/pydvl/
+utils/caching.html). # Contributing Please open new issues for bugs, feature
+requests and extensions. You can read about the structure of the project, the
+toolchain and workflow in the [guide for contributions](CONTRIBUTING.md). #
+License pyDVL is distributed under [LGPL-3.0](https://www.gnu.org/licenses/
+lgpl-3.0.html). A complete version can be found in two files: [here](LICENSE)
+and [here](COPYING.LESSER). All contributions will be distributed under this
+license.
```

### Comparing `pyDVL-0.6.0/logo.svg` & `pyDVL-0.6.1/logo.svg`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/pyproject.toml` & `pyDVL-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/setup.py` & `pyDVL-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
     name="pyDVL",
     package_dir={"": "src"},
     package_data={"pydvl": ["py.typed"]},
     packages=find_packages(where="src"),
     include_package_data=True,
-    version="0.6.0",
+    version="0.6.1",
     description="The Python Data Valuation Library",
     install_requires=[
         line
         for line in open("requirements.txt").readlines()
         if not line.startswith("--")
     ],
     setup_requires=["wheel"],
```

### Comparing `pyDVL-0.6.0/src/pyDVL.egg-info/PKG-INFO` & `pyDVL-0.6.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,179 +1,185 @@
 Metadata-Version: 2.1
 Name: pyDVL
-Version: 0.6.0
+Version: 0.6.1
 Summary: The Python Data Valuation Library
+Home-page: UNKNOWN
 Author: appliedAI Institute gGmbH
+License: UNKNOWN
 Project-URL: Source, https://github.com/appliedAI-Initiative/pydvl
 Project-URL: Documentation, https://appliedai-initiative.github.io/pyDVL
 Project-URL: TransferLab, https://transferlab.appliedai.de
+Description: <p align="center" style="text-align:center;">
+            <img alt="pyDVL Logo" src="https://raw.githubusercontent.com/appliedAI-Initiative/pyDVL/develop/logo.svg" width="200"/>
+        </p>
+        
+        <p align="center" style="text-align:center;">
+            A library for data valuation.
+        </p>
+        
+        <p align="center" style="text-align:center;">
+            <a href="https://github.com/appliedAI-Initiative/pyDVL/actions/workflows/tox.yaml">
+                <img src="https://github.com/appliedAI-Initiative/pyDVL/actions/workflows/tox.yaml/badge.svg" alt="Build Status"/>
+            </a>
+            <br>
+            <a href="https://pypi.org/project/pydvl/">
+                <img src="https://img.shields.io/pypi/v/pydvl.svg"/>
+            </a>
+            <a href="https://pypi.org/project/pydvl/">
+                <img src="https://img.shields.io/pypi/pyversions/pydvl.svg"/>
+            </a>
+            <img alt="PyPI - License" src="https://img.shields.io/pypi/l/pydvl"/>
+        </p>
+        
+        <p align="center" style="text-align:center;">
+            <strong>
+            <a href="https://appliedAI-Initiative.github.io/pyDVL">Docs</a>
+            </strong>
+        </p>
+        
+        pyDVL collects algorithms for Data Valuation and Influence Function computation.
+        
+        Data Valuation is the task of estimating the intrinsic value of a data point
+        wrt. the training set, the model and a scoring function. We currently implement
+        methods from the following papers:
+        
+        - Castro, Javier, Daniel Gómez, and Juan Tejada. [Polynomial Calculation of the
+          Shapley Value Based on Sampling](https://doi.org/10.1016/j.cor.2008.04.004).
+          Computers & Operations Research, Selected papers presented at the Tenth
+          International Symposium on Locational Decisions (ISOLDE X), 36, no. 5 (May 1,
+          2009): 1726–30.
+        - Ghorbani, Amirata, and James Zou. [Data Shapley: Equitable Valuation of Data
+          for Machine Learning](http://proceedings.mlr.press/v97/ghorbani19c.html). In
+          International Conference on Machine Learning, 2242–51. PMLR, 2019.
+        - Wang, Tianhao, Yu Yang, and Ruoxi Jia. 
+          [Improving Cooperative Game Theory-Based Data Valuation via Data Utility
+          Learning](https://doi.org/10.48550/arXiv.2107.06336). arXiv, 2022.
+        - Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nezihe Merve Gurel, Bo
+          Li, Ce Zhang, Costas Spanos, and Dawn Song. [Efficient Task-Specific Data
+          Valuation for Nearest Neighbor Algorithms](https://doi.org/10.14778/3342263.3342637).
+          Proceedings of the VLDB Endowment 12, no. 11 (1 July 2019): 1610–23.
+        - Okhrati, Ramin, and Aldo Lipani. [A Multilinear Sampling Algorithm to Estimate
+          Shapley Values](https://doi.org/10.1109/ICPR48806.2021.9412511). In 25th
+          International Conference on Pattern Recognition (ICPR 2020), 7992–99. IEEE,
+          2021.
+        - Yan, T., & Procaccia, A. D. [If You Like Shapley Then You’ll Love the
+          Core](https://ojs.aaai.org/index.php/AAAI/article/view/16721). Proceedings of
+          the AAAI Conference on Artificial Intelligence, 35(6) (2021): 5751-5759.
+        - Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nick Hynes, Nezihe Merve
+          Gürel, Bo Li, Ce Zhang, Dawn Song, and Costas J. Spanos. [Towards Efficient
+          Data Valuation Based on the Shapley Value](http://proceedings.mlr.press/v89/jia19a.html).
+          In 22nd International Conference on Artificial Intelligence and Statistics,
+          1167–76. PMLR, 2019.
+        - Wang, Jiachen T., and Ruoxi Jia. [Data Banzhaf: A Robust Data Valuation
+          Framework for Machine Learning](https://doi.org/10.48550/arXiv.2205.15466).
+          arXiv, October 22, 2022.
+        - Kwon, Yongchan, and James Zou. [Beta Shapley: A Unified and Noise-Reduced Data
+          Valuation Framework for Machine Learning](http://arxiv.org/abs/2110.14049).
+          In Proceedings of the 25th International Conference on Artificial Intelligence
+          and Statistics (AISTATS) 2022, Vol. 151. Valencia, Spain: PMLR, 2022.
+        
+        Influence Functions compute the effect that single points have on an estimator /
+        model. We implement methods from the following papers:
+        
+        - Koh, Pang Wei, and Percy Liang. [Understanding Black-Box Predictions via
+          Influence Functions](http://proceedings.mlr.press/v70/koh17a.html). In
+          Proceedings of the 34th International Conference on Machine Learning,
+          70:1885–94. Sydney, Australia: PMLR, 2017.
+        
+        # Installation
+        
+        To install the latest release use:
+        
+        ```shell
+        $ pip install pyDVL
+        ```
+        
+        You can also install the latest development version from
+        [TestPyPI](https://test.pypi.org/project/pyDVL/):
+        
+        ```shell
+        pip install pyDVL --index-url https://test.pypi.org/simple/
+        ```
+        
+        For more instructions and information refer to [Installing pyDVL
+        ](https://appliedAI-Initiative.github.io/pyDVL/20-install.html) in the
+        documentation.
+        
+        # Usage
+        
+        The steps required to compute values for your samples are:
+        
+        1. Create a `Dataset` object with your train and test splits.
+        2. Create an instance of a `SupervisedModel` (basically any sklearn compatible
+           predictor)
+        3. Create a `Utility` object to wrap the Dataset, the model and a scoring
+           function.
+        4. Use one of the methods defined in the library to compute the values.
+        
+        This is how it looks for *Truncated Montecarlo Shapley*, an efficient method for
+        Data Shapley values:
+        
+        ```python
+        from sklearn.datasets import load_breast_cancer
+        from sklearn.linear_model import LogisticRegression
+        from pydvl.value import *
+        
+        data = Dataset.from_sklearn(load_breast_cancer(), train_size=0.7)
+        model = LogisticRegression()
+        u = Utility(model, data, Scorer("accuracy", default=0.0))
+        values = compute_shapley_values(
+            u,
+            mode=ShapleyMode.TruncatedMontecarlo,
+            done=MaxUpdates(100) | AbsoluteStandardError(threshold=0.01),
+            truncation=RelativeTruncation(u, rtol=0.01),
+        )
+        ```
+        
+        For more instructions and information refer to [Getting
+        Started](https://appliedAI-Initiative.github.io/pyDVL/10-getting-started.html) in
+        the documentation. We provide several
+        [examples](https://appliedAI-Initiative.github.io/pyDVL/examples/index.html)
+        with details on the algorithms and their applications.
+        
+        ## Caching
+        
+        pyDVL offers the possibility to cache certain results and
+        speed up computation. It uses [Memcached](https://memcached.org/) For that.
+        
+        You can run it either locally or, using
+        [Docker](https://www.docker.com/):
+        
+        ```shell
+        docker container run --rm -p 11211:11211 --name pydvl-cache -d memcached:latest
+        ```
+        
+        You can read more in the [caching module's
+        documentation](https://appliedAI-Initiative.github.io/pyDVL/pydvl/utils/caching.html).
+        
+        # Contributing
+        
+        Please open new issues for bugs, feature requests and extensions. You can read
+        about the structure of the project, the toolchain and workflow in the [guide for
+        contributions](CONTRIBUTING.md).
+        
+        # License
+        
+        pyDVL is distributed under
+        [LGPL-3.0](https://www.gnu.org/licenses/lgpl-3.0.html). A complete version can
+        be found in two files: [here](LICENSE) and [here](COPYING.LESSER).
+        
+        All contributions will be distributed under this license.
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Description-Content-Type: text/markdown
 Provides-Extra: influence
-License-File: LICENSE
-License-File: COPYING.LESSER
-
-<p align="center" style="text-align:center;">
-    <img alt="pyDVL Logo" src="https://raw.githubusercontent.com/appliedAI-Initiative/pyDVL/develop/logo.svg" width="200"/>
-</p>
-
-<p align="center" style="text-align:center;">
-    A library for data valuation.
-</p>
-
-<p align="center" style="text-align:center;">
-    <a href="https://github.com/appliedAI-Initiative/pyDVL/actions/workflows/tox.yaml">
-        <img src="https://github.com/appliedAI-Initiative/pyDVL/actions/workflows/tox.yaml/badge.svg" alt="Build Status"/>
-    </a>
-    <br>
-    <a href="https://pypi.org/project/pydvl/">
-        <img src="https://img.shields.io/pypi/v/pydvl.svg"/>
-    </a>
-    <a href="https://pypi.org/project/pydvl/">
-        <img src="https://img.shields.io/pypi/pyversions/pydvl.svg"/>
-    </a>
-    <img alt="PyPI - License" src="https://img.shields.io/pypi/l/pydvl"/>
-</p>
-
-<p align="center" style="text-align:center;">
-    <strong>
-    <a href="https://appliedAI-Initiative.github.io/pyDVL">Docs</a>
-    </strong>
-</p>
-
-pyDVL collects algorithms for Data Valuation and Influence Function computation.
-
-Data Valuation is the task of estimating the intrinsic value of a data point
-wrt. the training set, the model and a scoring function. We currently implement
-methods from the following papers:
-
-- Ghorbani, Amirata, and James Zou. 
-  [Data Shapley: Equitable Valuation of Data for Machine Learning](http://proceedings.mlr.press/v97/ghorbani19c.html).
-  In International Conference on Machine Learning, 2242–51. PMLR, 2019.
-- Wang, Tianhao, Yu Yang, and Ruoxi Jia. 
-  [Improving Cooperative Game Theory-Based Data Valuation via Data Utility Learning](https://doi.org/10.48550/arXiv.2107.06336).
-  arXiv, 2022.
-- Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nezihe Merve Gurel, Bo Li,
-  Ce Zhang, Costas Spanos, and Dawn Song.
-  [Efficient Task-Specific Data Valuation for Nearest Neighbor Algorithms](https://doi.org/10.14778/3342263.3342637).
-  Proceedings of the VLDB Endowment 12, no. 11 (1 July 2019): 1610–23.
-- Okhrati, Ramin, and Aldo Lipani.
-  [A Multilinear Sampling Algorithm to Estimate Shapley Values](https://doi.org/10.1109/ICPR48806.2021.9412511).
-  In 25th International Conference on Pattern Recognition (ICPR 2020), 7992–99.
-  IEEE, 2021.
-- Yan, T., & Procaccia, A. D.
-  [If You Like Shapley Then You’ll Love the Core]().
-  Proceedings of the AAAI Conference on Artificial Intelligence, 35(6) (2021): 5751-5759.
-- Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nick Hynes, Nezihe Merve
-  Gürel, Bo Li, Ce Zhang, Dawn Song, and Costas J. Spanos.
-  [Towards Efficient Data Valuation Based on the Shapley Value](http://proceedings.mlr.press/v89/jia19a.html).
-  In 22nd International Conference on Artificial Intelligence and Statistics,
-  1167–76. PMLR, 2019.
-- Wang, Jiachen T., and Ruoxi Jia. 
-  [Data Banzhaf: A Robust Data Valuation Framework for Machine Learning](https://doi.org/10.48550/arXiv.2205.15466).
-  arXiv, October 22, 2022.
-- Kwon, Yongchan, and James Zou.
-  [Beta Shapley: A Unified and Noise-Reduced Data Valuation Framework for Machine Learning](http://arxiv.org/abs/2110.14049).
-  In Proceedings of the 25th International Conference on Artificial Intelligence
-  and Statistics (AISTATS) 2022, Vol. 151. Valencia, Spain: PMLR, 2022.
-
-Influence Functions compute the effect that single points have on an estimator /
-model. We implement methods from the following papers:
-
-- Koh, Pang Wei, and Percy Liang.
-  [Understanding Black-Box Predictions via Influence Functions](http://proceedings.mlr.press/v70/koh17a.html).
-  In Proceedings of the 34th International Conference on Machine Learning,
-  70:1885–94. Sydney, Australia: PMLR, 2017.
-
-# Installation
-
-To install the latest release use:
-
-```shell
-$ pip install pyDVL
-```
-
-You can also install the latest development version from
-[TestPyPI](https://test.pypi.org/project/pyDVL/):
-
-```shell
-pip install pyDVL --index-url https://test.pypi.org/simple/
-```
-
-For more instructions and information refer to [Installing pyDVL
-](https://appliedAI-Initiative.github.io/pyDVL/20-install.html) in the
-documentation.
-
-# Usage
-
-The steps required to compute values for your samples are:
-
-1. Create a `Dataset` object with your train and test splits.
-2. Create an instance of a `SupervisedModel` (basically any sklearn compatible
-   predictor)
-3. Create a `Utility` object to wrap the Dataset, the model and a scoring
-   function.
-4. Use one of the methods defined in the library to compute the values.
-
-This is how it looks for *Truncated Montecarlo Shapley*, an efficient method for
-Data Shapley values:
-
-```python
-from sklearn.datasets import load_breast_cancer
-from sklearn.linear_model import LogisticRegression
-from pydvl.value import *
-
-data = Dataset.from_sklearn(load_breast_cancer(), train_size=0.7)
-model = LogisticRegression()
-u = Utility(model, data, Scorer("accuracy", default=0.0))
-values = compute_shapley_values(
-    u,
-    mode=ShapleyMode.TruncatedMontecarlo,
-    done=MaxUpdates(100) | AbsoluteStandardError(threshold=0.01),
-    truncation=RelativeTruncation(u, rtol=0.01),
-)
-```
-
-For more instructions and information refer to [Getting
-Started](https://appliedAI-Initiative.github.io/pyDVL/10-getting-started.html) in
-the documentation. We provide several
-[examples](https://appliedAI-Initiative.github.io/pyDVL/examples/index.html)
-with details on the algorithms and their applications.
-
-## Caching
-
-pyDVL offers the possibility to cache certain results and
-speed up computation. It uses [Memcached](https://memcached.org/) For that.
-
-You can run it either locally or, using
-[Docker](https://www.docker.com/):
-
-```shell
-docker container run --rm -p 11211:11211 --name pydvl-cache -d memcached:latest
-```
-
-You can read more in the [caching module's
-documentation](https://appliedAI-Initiative.github.io/pyDVL/pydvl/utils/caching.html).
-
-# Contributing
-
-Please open new issues for bugs, feature requests and extensions. You can read
-about the structure of the project, the toolchain and workflow in the [guide for
-contributions](CONTRIBUTING.md).
-
-# License
-
-pyDVL is distributed under
-[LGPL-3.0](https://www.gnu.org/licenses/lgpl-3.0.html). A complete version can
-be found in two files: [here](LICENSE) and [here](COPYING.LESSER).
-
-All contributions will be distributed under this license.
```

#### html2text {}

```diff
@@ -1,89 +1,94 @@
-Metadata-Version: 2.1 Name: pyDVL Version: 0.6.0 Summary: The Python Data
-Valuation Library Author: appliedAI Institute gGmbH Project-URL: Source, https:
-//github.com/appliedAI-Initiative/pydvl Project-URL: Documentation, https://
-appliedai-initiative.github.io/pyDVL Project-URL: TransferLab, https://
-transferlab.appliedai.de Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Typing :: Typed Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft
-:: Windows Classifier: Operating System :: POSIX Classifier: License :: OSI
-Approved :: GNU Lesser General Public License v3 (LGPLv3) Description-Content-
-Type: text/markdown Provides-Extra: influence License-File: LICENSE License-
-File: COPYING.LESSER
+Metadata-Version: 2.1 Name: pyDVL Version: 0.6.1 Summary: The Python Data
+Valuation Library Home-page: UNKNOWN Author: appliedAI Institute gGmbH License:
+UNKNOWN Project-URL: Source, https://github.com/appliedAI-Initiative/pydvl
+Project-URL: Documentation, https://appliedai-initiative.github.io/pyDVL
+Project-URL: TransferLab, https://transferlab.appliedai.de Description:
                                  [pyDVL Logo]
                          A library for data valuation.
                                 [Build_Status]
     [https://img.shields.io/pypi/v/pydvl.svg] [https://img.shields.io/pypi/
                     pyversions/pydvl.svg] [PyPI - License]
                                      Docs
 pyDVL collects algorithms for Data Valuation and Influence Function
 computation. Data Valuation is the task of estimating the intrinsic value of a
 data point wrt. the training set, the model and a scoring function. We
-currently implement methods from the following papers: - Ghorbani, Amirata, and
-James Zou. [Data Shapley: Equitable Valuation of Data for Machine Learning]
-(http://proceedings.mlr.press/v97/ghorbani19c.html). In International
-Conference on Machine Learning, 2242â51. PMLR, 2019. - Wang, Tianhao, Yu
-Yang, and Ruoxi Jia. [Improving Cooperative Game Theory-Based Data Valuation
-via Data Utility Learning](https://doi.org/10.48550/arXiv.2107.06336). arXiv,
-2022. - Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nezihe Merve
-Gurel, Bo Li, Ce Zhang, Costas Spanos, and Dawn Song. [Efficient Task-Specific
-Data Valuation for Nearest Neighbor Algorithms](https://doi.org/10.14778/
-3342263.3342637). Proceedings of the VLDB Endowment 12, no. 11 (1 July 2019):
-1610â23. - Okhrati, Ramin, and Aldo Lipani. [A Multilinear Sampling Algorithm
-to Estimate Shapley Values](https://doi.org/10.1109/ICPR48806.2021.9412511). In
-25th International Conference on Pattern Recognition (ICPR 2020), 7992â99.
-IEEE, 2021. - Yan, T., & Procaccia, A. D. [If You Like Shapley Then Youâll
-Love the Core](). Proceedings of the AAAI Conference on Artificial
-Intelligence, 35(6) (2021): 5751-5759. - Jia, Ruoxi, David Dao, Boxin Wang,
-Frances Ann Hubis, Nick Hynes, Nezihe Merve GÃ¼rel, Bo Li, Ce Zhang, Dawn Song,
-and Costas J. Spanos. [Towards Efficient Data Valuation Based on the Shapley
-Value](http://proceedings.mlr.press/v89/jia19a.html). In 22nd International
-Conference on Artificial Intelligence and Statistics, 1167â76. PMLR, 2019. -
-Wang, Jiachen T., and Ruoxi Jia. [Data Banzhaf: A Robust Data Valuation
-Framework for Machine Learning](https://doi.org/10.48550/arXiv.2205.15466).
-arXiv, October 22, 2022. - Kwon, Yongchan, and James Zou. [Beta Shapley: A
-Unified and Noise-Reduced Data Valuation Framework for Machine Learning](http:/
-/arxiv.org/abs/2110.14049). In Proceedings of the 25th International Conference
-on Artificial Intelligence and Statistics (AISTATS) 2022, Vol. 151. Valencia,
-Spain: PMLR, 2022. Influence Functions compute the effect that single points
-have on an estimator / model. We implement methods from the following papers: -
-Koh, Pang Wei, and Percy Liang. [Understanding Black-Box Predictions via
-Influence Functions](http://proceedings.mlr.press/v70/koh17a.html). In
-Proceedings of the 34th International Conference on Machine Learning, 70:
-1885â94. Sydney, Australia: PMLR, 2017. # Installation To install the latest
-release use: ```shell $ pip install pyDVL ``` You can also install the latest
-development version from [TestPyPI](https://test.pypi.org/project/pyDVL/):
-```shell pip install pyDVL --index-url https://test.pypi.org/simple/ ``` For
-more instructions and information refer to [Installing pyDVL ](https://
-appliedAI-Initiative.github.io/pyDVL/20-install.html) in the documentation. #
-Usage The steps required to compute values for your samples are: 1. Create a
-`Dataset` object with your train and test splits. 2. Create an instance of a
-`SupervisedModel` (basically any sklearn compatible predictor) 3. Create a
-`Utility` object to wrap the Dataset, the model and a scoring function. 4. Use
-one of the methods defined in the library to compute the values. This is how it
-looks for *Truncated Montecarlo Shapley*, an efficient method for Data Shapley
-values: ```python from sklearn.datasets import load_breast_cancer from
-sklearn.linear_model import LogisticRegression from pydvl.value import * data =
-Dataset.from_sklearn(load_breast_cancer(), train_size=0.7) model =
-LogisticRegression() u = Utility(model, data, Scorer("accuracy", default=0.0))
-values = compute_shapley_values( u, mode=ShapleyMode.TruncatedMontecarlo,
-done=MaxUpdates(100) | AbsoluteStandardError(threshold=0.01),
-truncation=RelativeTruncation(u, rtol=0.01), ) ``` For more instructions and
-information refer to [Getting Started](https://appliedAI-Initiative.github.io/
-pyDVL/10-getting-started.html) in the documentation. We provide several
-[examples](https://appliedAI-Initiative.github.io/pyDVL/examples/index.html)
-with details on the algorithms and their applications. ## Caching pyDVL offers
-the possibility to cache certain results and speed up computation. It uses
-[Memcached](https://memcached.org/) For that. You can run it either locally or,
-using [Docker](https://www.docker.com/): ```shell docker container run --rm -
-p 11211:11211 --name pydvl-cache -d memcached:latest ``` You can read more in
-the [caching module's documentation](https://appliedAI-Initiative.github.io/
-pyDVL/pydvl/utils/caching.html). # Contributing Please open new issues for
-bugs, feature requests and extensions. You can read about the structure of the
-project, the toolchain and workflow in the [guide for contributions]
-(CONTRIBUTING.md). # License pyDVL is distributed under [LGPL-3.0](https://
-www.gnu.org/licenses/lgpl-3.0.html). A complete version can be found in two
-files: [here](LICENSE) and [here](COPYING.LESSER). All contributions will be
-distributed under this license.
+currently implement methods from the following papers: - Castro, Javier, Daniel
+GÃ³mez, and Juan Tejada. [Polynomial Calculation of the Shapley Value Based on
+Sampling](https://doi.org/10.1016/j.cor.2008.04.004). Computers & Operations
+Research, Selected papers presented at the Tenth International Symposium on
+Locational Decisions (ISOLDE X), 36, no. 5 (May 1, 2009): 1726â30. -
+Ghorbani, Amirata, and James Zou. [Data Shapley: Equitable Valuation of Data
+for Machine Learning](http://proceedings.mlr.press/v97/ghorbani19c.html). In
+International Conference on Machine Learning, 2242â51. PMLR, 2019. - Wang,
+Tianhao, Yu Yang, and Ruoxi Jia. [Improving Cooperative Game Theory-Based Data
+Valuation via Data Utility Learning](https://doi.org/10.48550/
+arXiv.2107.06336). arXiv, 2022. - Jia, Ruoxi, David Dao, Boxin Wang, Frances
+Ann Hubis, Nezihe Merve Gurel, Bo Li, Ce Zhang, Costas Spanos, and Dawn Song.
+[Efficient Task-Specific Data Valuation for Nearest Neighbor Algorithms](https:
+//doi.org/10.14778/3342263.3342637). Proceedings of the VLDB Endowment 12, no.
+11 (1 July 2019): 1610â23. - Okhrati, Ramin, and Aldo Lipani. [A Multilinear
+Sampling Algorithm to Estimate Shapley Values](https://doi.org/10.1109/
+ICPR48806.2021.9412511). In 25th International Conference on Pattern
+Recognition (ICPR 2020), 7992â99. IEEE, 2021. - Yan, T., & Procaccia, A. D.
+[If You Like Shapley Then Youâll Love the Core](https://ojs.aaai.org/
+index.php/AAAI/article/view/16721). Proceedings of the AAAI Conference on
+Artificial Intelligence, 35(6) (2021): 5751-5759. - Jia, Ruoxi, David Dao,
+Boxin Wang, Frances Ann Hubis, Nick Hynes, Nezihe Merve GÃ¼rel, Bo Li, Ce
+Zhang, Dawn Song, and Costas J. Spanos. [Towards Efficient Data Valuation Based
+on the Shapley Value](http://proceedings.mlr.press/v89/jia19a.html). In 22nd
+International Conference on Artificial Intelligence and Statistics, 1167â76.
+PMLR, 2019. - Wang, Jiachen T., and Ruoxi Jia. [Data Banzhaf: A Robust Data
+Valuation Framework for Machine Learning](https://doi.org/10.48550/
+arXiv.2205.15466). arXiv, October 22, 2022. - Kwon, Yongchan, and James Zou.
+[Beta Shapley: A Unified and Noise-Reduced Data Valuation Framework for Machine
+Learning](http://arxiv.org/abs/2110.14049). In Proceedings of the 25th
+International Conference on Artificial Intelligence and Statistics (AISTATS)
+2022, Vol. 151. Valencia, Spain: PMLR, 2022. Influence Functions compute the
+effect that single points have on an estimator / model. We implement methods
+from the following papers: - Koh, Pang Wei, and Percy Liang. [Understanding
+Black-Box Predictions via Influence Functions](http://proceedings.mlr.press/
+v70/koh17a.html). In Proceedings of the 34th International Conference on
+Machine Learning, 70:1885â94. Sydney, Australia: PMLR, 2017. # Installation
+To install the latest release use: ```shell $ pip install pyDVL ``` You can
+also install the latest development version from [TestPyPI](https://
+test.pypi.org/project/pyDVL/): ```shell pip install pyDVL --index-url https://
+test.pypi.org/simple/ ``` For more instructions and information refer to
+[Installing pyDVL ](https://appliedAI-Initiative.github.io/pyDVL/20-
+install.html) in the documentation. # Usage The steps required to compute
+values for your samples are: 1. Create a `Dataset` object with your train and
+test splits. 2. Create an instance of a `SupervisedModel` (basically any
+sklearn compatible predictor) 3. Create a `Utility` object to wrap the Dataset,
+the model and a scoring function. 4. Use one of the methods defined in the
+library to compute the values. This is how it looks for *Truncated Montecarlo
+Shapley*, an efficient method for Data Shapley values: ```python from
+sklearn.datasets import load_breast_cancer from sklearn.linear_model import
+LogisticRegression from pydvl.value import * data = Dataset.from_sklearn
+(load_breast_cancer(), train_size=0.7) model = LogisticRegression() u = Utility
+(model, data, Scorer("accuracy", default=0.0)) values = compute_shapley_values
+( u, mode=ShapleyMode.TruncatedMontecarlo, done=MaxUpdates(100) |
+AbsoluteStandardError(threshold=0.01), truncation=RelativeTruncation(u,
+rtol=0.01), ) ``` For more instructions and information refer to [Getting
+Started](https://appliedAI-Initiative.github.io/pyDVL/10-getting-started.html)
+in the documentation. We provide several [examples](https://appliedAI-
+Initiative.github.io/pyDVL/examples/index.html) with details on the algorithms
+and their applications. ## Caching pyDVL offers the possibility to cache
+certain results and speed up computation. It uses [Memcached](https://
+memcached.org/) For that. You can run it either locally or, using [Docker]
+(https://www.docker.com/): ```shell docker container run --rm -p 11211:11211 --
+name pydvl-cache -d memcached:latest ``` You can read more in the [caching
+module's documentation](https://appliedAI-Initiative.github.io/pyDVL/pydvl/
+utils/caching.html). # Contributing Please open new issues for bugs, feature
+requests and extensions. You can read about the structure of the project, the
+toolchain and workflow in the [guide for contributions](CONTRIBUTING.md). #
+License pyDVL is distributed under [LGPL-3.0](https://www.gnu.org/licenses/
+lgpl-3.0.html). A complete version can be found in two files: [here](LICENSE)
+and [here](COPYING.LESSER). All contributions will be distributed under this
+license. Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Typing :: Typed
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: Microsoft :: Windows Classifier: Operating System :: POSIX Classifier:
+License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Description-Content-Type: text/markdown Provides-Extra: influence
```

### Comparing `pyDVL-0.6.0/src/pydvl/influence/conjugate_gradient.py` & `pyDVL-0.6.1/src/pydvl/influence/conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/influence/frameworks/torch_differentiable.py` & `pyDVL-0.6.1/src/pydvl/influence/frameworks/torch_differentiable.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/influence/general.py` & `pyDVL-0.6.1/src/pydvl/influence/general.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/influence/linear.py` & `pyDVL-0.6.1/src/pydvl/influence/linear.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/influence/model_wrappers/torch_wrappers.py` & `pyDVL-0.6.1/src/pydvl/influence/model_wrappers/torch_wrappers.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/influence/types.py` & `pyDVL-0.6.1/src/pydvl/influence/types.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/reporting/plots.py` & `pyDVL-0.6.1/src/pydvl/reporting/plots.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/reporting/scores.py` & `pyDVL-0.6.1/src/pydvl/reporting/scores.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/utils/caching.py` & `pyDVL-0.6.1/src/pydvl/utils/caching.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/utils/config.py` & `pyDVL-0.6.1/src/pydvl/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,31 @@
 __all__ = ["ParallelConfig", "MemcachedClientConfig", "MemcachedConfig"]
 
 
 @dataclass
 class ParallelConfig:
     """Configuration for parallel computation backend.
 
-    :param backend: Type of backend to use. For now only 'ray' is supported.
+    :param backend: Type of backend to use.
+        Defaults to 'ray'
     :param address: Address of existing remote or local cluster to use.
-    :param n_local_workers: Number of workers (CPUs) to use when using a local ray cluster.
+    :param n_cpus_local: Number of CPUs to use when creating a local ray cluster.
+        This has no effect when using an existing ray cluster.
     :param logging_level: Logging level for the parallel backend's worker.
     """
 
     backend: Literal["sequential", "ray"] = "ray"
     address: Optional[Union[str, Tuple[str, int]]] = None
-    n_local_workers: Optional[int] = None
+    n_cpus_local: Optional[int] = None
     logging_level: int = logging.WARNING
 
+    def __post_init__(self) -> None:
+        if self.address is not None and self.n_cpus_local is not None:
+            raise ValueError("When `address` is set, `n_cpus_local` should be None.")
+
 
 @dataclass
 class MemcachedClientConfig:
     """Configuration of the memcached client.
 
     :param server: A tuple of (IP|domain name, port).
     :param connect_timeout: How many seconds to wait before raising
```

### Comparing `pyDVL-0.6.0/src/pydvl/utils/dataset.py` & `pyDVL-0.6.1/src/pydvl/utils/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -475,18 +475,28 @@
             :class:`Dataset` constructor.
         :return: Dataset with the selected sklearn data
         """
         if data_groups is None:
             raise ValueError(
                 "data_groups must be provided when constructing a GroupedDataset"
             )
-        dataset = Dataset.from_sklearn(
-            data, train_size, random_state, stratify_by_target, **kwargs
+
+        x_train, x_test, y_train, y_test, data_groups_train, _ = train_test_split(
+            data.data,
+            data.target,
+            data_groups,
+            train_size=train_size,
+            random_state=random_state,
+            stratify=data.target if stratify_by_target else None,
+        )
+
+        dataset = Dataset(
+            x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, **kwargs
         )
-        return cls.from_dataset(dataset, data_groups)  # type: ignore
+        return cls.from_dataset(dataset, data_groups_train)  # type: ignore
 
     @classmethod
     def from_arrays(
         cls,
         X: NDArray,
         y: NDArray,
         train_size: float = 0.8,
@@ -523,18 +533,26 @@
         .. versionchanged:: 0.6.0
            Added kwargs to pass to the :class:`Dataset` constructor.
         """
         if data_groups is None:
             raise ValueError(
                 "data_groups must be provided when constructing a GroupedDataset"
             )
-        dataset = Dataset.from_arrays(
-            X, y, train_size, random_state, stratify_by_target, **kwargs
+        x_train, x_test, y_train, y_test, data_groups_train, _ = train_test_split(
+            X,
+            y,
+            data_groups,
+            train_size=train_size,
+            random_state=random_state,
+            stratify=y if stratify_by_target else None,
+        )
+        dataset = Dataset(
+            x_train=x_train, y_train=y_train, x_test=x_test, y_test=y_test, **kwargs
         )
-        return cls.from_dataset(dataset, data_groups)
+        return cls.from_dataset(dataset, data_groups_train)
 
     @classmethod
     def from_dataset(
         cls, dataset: Dataset, data_groups: Sequence[Any]
     ) -> "GroupedDataset":
         """Creates a :class:`GroupedDataset` object from the data a
         :class:`Dataset` object and a mapping of data groups.
```

### Comparing `pyDVL-0.6.0/src/pydvl/utils/numeric.py` & `pyDVL-0.6.1/src/pydvl/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/utils/parallel/backend.py` & `pyDVL-0.6.1/src/pydvl/utils/parallel/backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     Type,
     TypeVar,
     Union,
 )
 
 import ray
 from ray import ObjectRef
-from ray.remote_function import RemoteFunction
 
 from ..config import ParallelConfig
 
 __all__ = ["init_parallel_backend", "effective_n_jobs", "available_cpus"]
 
 T = TypeVar("T")
 
@@ -89,26 +88,24 @@
         return n_jobs
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: {self.config}>"
 
 
 class SequentialParallelBackend(BaseParallelBackend, backend_name="sequential"):
-    """Class used to run jobs sequentially and locally. It shouldn't
-    be initialized directly. You should instead call `init_parallel_backend`.
+    """Class used to run jobs sequentially and locally.
+
+    It shouldn't be initialized directly. You should instead call
+    :func:`~pydvl.utils.parallel.backend.init_parallel_backend`.
 
     :param config: instance of :class:`~pydvl.utils.config.ParallelConfig` with number of cpus
     """
 
     def __init__(self, config: ParallelConfig):
-        config_dict = asdict(config)
-        config_dict.pop("backend")
-        config_dict.pop("address")
-        config_dict["num_cpus"] = config_dict.pop("n_local_workers")
-        self.config = config_dict
+        self.config = {}
 
     def get(self, v: Any, *args, **kwargs):
         return v
 
     def put(self, v: Any, *args, **kwargs) -> Any:
         return v
 
@@ -122,25 +119,29 @@
         return v, []
 
     def _effective_n_jobs(self, n_jobs: int) -> int:
         return 1
 
 
 class RayParallelBackend(BaseParallelBackend, backend_name="ray"):
-    """Class used to wrap ray to make it transparent to algorithms. It shouldn't
-    be initialized directly. You should instead call `init_parallel_backend`.
+    """Class used to wrap ray to make it transparent to algorithms.
+
+    It shouldn't be initialized directly. You should instead call
+    :func:`~pydvl.utils.parallel.backend.init_parallel_backend`.
 
     :param config: instance of :class:`~pydvl.utils.config.ParallelConfig` with
         cluster address, number of cpus, etc.
     """
 
     def __init__(self, config: ParallelConfig):
         config_dict = asdict(config)
         config_dict.pop("backend")
-        config_dict["num_cpus"] = config_dict.pop("n_local_workers")
+        n_cpus_local = config_dict.pop("n_cpus_local")
+        if config_dict.get("address", None) is None:
+            config_dict["num_cpus"] = n_cpus_local
         self.config = config_dict
         if not ray.is_initialized():
             ray.init(**self.config)
 
     def get(
         self,
         v: Union[ObjectRef, Iterable[ObjectRef], T],
@@ -165,15 +166,15 @@
         """Wraps a function as a ray remote.
 
         :param fun: the function to wrap
         :param kwargs: keyword arguments to pass to @ray.remote
 
         :return: The `.remote` method of the ray `RemoteFunction`.
         """
-        if len(kwargs) > 1:
+        if len(kwargs) > 0:
             return ray.remote(**kwargs)(fun).remote  # type: ignore
         return ray.remote(fun).remote  # type: ignore
 
     def wait(
         self,
         v: List["ObjectRef"],
         *args,
@@ -197,15 +198,16 @@
 
 
 def init_parallel_backend(
     config: ParallelConfig,
 ) -> BaseParallelBackend:
     """Initializes the parallel backend and returns an instance of it.
 
-    :param config: instance of :class:`~pydvl.utils.config.ParallelConfig` with cluster address, number of cpus, etc.
+    :param config: instance of :class:`~pydvl.utils.config.ParallelConfig`
+        with cluster address, number of cpus, etc.
 
     :Example:
 
     >>> from pydvl.utils.parallel.backend import init_parallel_backend
     >>> from pydvl.utils.config import ParallelConfig
     >>> config = ParallelConfig(backend="ray")
     >>> parallel_backend = init_parallel_backend(config)
```

### Comparing `pyDVL-0.6.0/src/pydvl/utils/parallel/map_reduce.py` & `pyDVL-0.6.1/src/pydvl/utils/parallel/map_reduce.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/utils/progress.py` & `pyDVL-0.6.1/src/pydvl/utils/progress.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/utils/score.py` & `pyDVL-0.6.1/src/pydvl/utils/score.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/utils/status.py` & `pyDVL-0.6.1/src/pydvl/utils/status.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/utils/types.py` & `pyDVL-0.6.1/src/pydvl/utils/types.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/utils/utility.py` & `pyDVL-0.6.1/src/pydvl/utils/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,18 +290,17 @@
         if x is not None:
             boolean_vector[:, tuple(x)] = True
         return boolean_vector
 
     def __call__(self, indices: Iterable[int]) -> float:
         indices_boolean_vector = self._convert_indices_to_boolean_vector(indices)
         frozen_indices = frozenset(indices)
-        if self._current_iteration < self.training_budget:
+        if len(self._utility_samples) < self.training_budget:
             utility = self.utility(frozen_indices)
             self._utility_samples[frozen_indices] = (indices_boolean_vector, utility)
-            self._current_iteration += 1
         else:
             if not self._is_model_fit:
                 X, y = zip(*self._utility_samples.values())
                 X = np.vstack(X)
                 y = np.asarray(y)
                 self.model.fit(X, y)
                 self._is_model_fit = True
```

### Comparing `pyDVL-0.6.0/src/pydvl/value/least_core/__init__.py` & `pyDVL-0.6.1/src/pydvl/value/least_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/least_core/common.py` & `pyDVL-0.6.1/src/pydvl/value/least_core/common.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/least_core/montecarlo.py` & `pyDVL-0.6.1/src/pydvl/value/least_core/montecarlo.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/least_core/naive.py` & `pyDVL-0.6.1/src/pydvl/value/least_core/naive.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/loo/naive.py` & `pyDVL-0.6.1/src/pydvl/value/loo/naive.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/result.py` & `pyDVL-0.6.1/src/pydvl/value/result.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/sampler.py` & `pyDVL-0.6.1/src/pydvl/value/sampler.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/semivalues.py` & `pyDVL-0.6.1/src/pydvl/value/semivalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,16 +228,16 @@
     :param kwargs: Additional keyword arguments passed to
         :func:`~pydvl.value.semivalues.semivalues`.
     """
     sampler_instance = sampler_t(u.data.indices)
     if mode == SemiValueMode.Shapley:
         coefficient = shapley_coefficient
     elif mode == SemiValueMode.BetaShapley:
-        alpha = kwargs.get("alpha", 1)
-        beta = kwargs.get("beta", 1)
+        alpha = kwargs.pop("alpha", 1)
+        beta = kwargs.pop("beta", 1)
         coefficient = beta_coefficient(alpha, beta)
     elif mode == SemiValueMode.Banzhaf:
         coefficient = banzhaf_coefficient
     else:
         raise ValueError(f"Unknown mode {mode}")
     coefficient = cast(SVCoefficient, coefficient)
     return semivalues(sampler_instance, u, coefficient, done, n_jobs=n_jobs, **kwargs)
```

### Comparing `pyDVL-0.6.0/src/pydvl/value/shapley/__init__.py` & `pyDVL-0.6.1/src/pydvl/value/shapley/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/shapley/actor.py` & `pyDVL-0.6.1/src/pydvl/value/shapley/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,178 +1,162 @@
-"""
-Methods and classes to distribute jobs computing Shapley values in a cluster.
-
-You probably aren't interested in any of this unless you are developing new
-methods for pyDVL that use parallelization.
-"""
-
-import logging
-import operator
-from functools import reduce
-from time import time
-from typing import cast
-
-import numpy as np
-
-from pydvl.utils.config import ParallelConfig
-from pydvl.utils.parallel import init_parallel_backend
-from pydvl.utils.parallel.actor import Coordinator, RayActorWrapper, Worker
-from pydvl.utils.utility import Utility
+from pydvl.utils import Utility
 from pydvl.value.result import ValuationResult
-from pydvl.value.shapley.truncated import TruncationPolicy
-from pydvl.value.stopping import MaxChecks, StoppingCriterion
-
-__all__ = ["get_shapley_coordinator", "get_shapley_worker"]
+from pydvl.value.shapley.gt import group_testing_shapley
+from pydvl.value.shapley.knn import knn_shapley
+from pydvl.value.shapley.montecarlo import (
+    combinatorial_montecarlo_shapley,
+    permutation_montecarlo_shapley,
+)
+from pydvl.value.shapley.naive import (
+    combinatorial_exact_shapley,
+    permutation_exact_shapley,
+)
+from pydvl.value.shapley.owen import OwenAlgorithm, owen_sampling_shapley
+from pydvl.value.shapley.truncated import NoTruncation, truncated_montecarlo_shapley
+from pydvl.value.shapley.types import ShapleyMode
+from pydvl.value.stopping import MaxUpdates, StoppingCriterion
+
+__all__ = ["compute_shapley_values"]
+
+
+def compute_shapley_values(
+    u: Utility,
+    *,
+    done: StoppingCriterion = MaxUpdates(100),
+    mode: ShapleyMode = ShapleyMode.TruncatedMontecarlo,
+    n_jobs: int = 1,
+    **kwargs,
+) -> ValuationResult:
+    """Umbrella method to compute Shapley values with any of the available
+    algorithms.
+
+    See :ref:`data valuation` for an overview.
+
+    The following algorithms are available. Note that the exact methods can only
+    work with very small datasets and are thus intended only for testing. Some
+    algorithms also accept additional arguments, please refer to the
+    documentation of each particular method.
+
+    - ``combinatorial_exact``: uses the combinatorial implementation of data
+      Shapley. Implemented in
+      :func:`~pydvl.value.shapley.naive.combinatorial_exact_shapley`.
+    - ``combinatorial_montecarlo``:  uses the approximate Monte Carlo
+      implementation of combinatorial data Shapley. Implemented in
+      :func:`~pydvl.value.shapley.montecarlo.combinatorial_montecarlo_shapley`.
+    - ``permutation_exact``: uses the permutation-based implementation of data
+      Shapley. Computation is **not parallelized**. Implemented in
+      :func:`~pydvl.value.shapley.naive.permutation_exact_shapley`.
+    - ``permutation_montecarlo``: uses the approximate Monte Carlo
+      implementation of permutation data Shapley. Implemented in
+      :func:`~pydvl.value.shapley.montecarlo.permutation_montecarlo_shapley`.
+    - ``truncated_montecarlo``: default option, same as ``permutation_montecarlo``
+      but stops the computation whenever a certain accuracy is reached.
+      Implemented in
+      :func:`~pydvl.value.shapley.montecarlo.truncated_montecarlo_shapley`.
+    - ``owen_sampling``: Uses the Owen continuous extension of the utility
+      function to the unit cube. Implemented in
+      :func:`~pydvl.value.shapley.montecarlo.owen_sampling_shapley`. This
+      method does not take a :class:`~pydvl.value.stopping.StoppingCriterion`
+      but instead requires a parameter ``q_max`` for the number of subdivisions
+      of the unit interval to use for integration, and another parameter
+      ``n_samples`` for the number of subsets to sample for each $q$.
+    - ``owen_halved``: Same as 'owen_sampling' but uses correlated samples in the
+      expectation. Implemented in
+      :func:`~pydvl.value.shapley.montecarlo.owen_sampling_shapley`.
+      This method  requires an additional parameter `q_max` for the number of
+      subdivisions of the interval [0,0.5] to use for integration, and another
+      parameter ``n_samples`` for the number of subsets to sample for each $q$.
+    - ``group_testing``: estimates differences of Shapley values and solves a
+      constraint satisfaction problem. High sample complexity, not recommended.
+      Implemented in :func:`~pydvl.value.shapley.gt.group_testing_shapley`. This
+      method does not take a :class:`~pydvl.value.stopping.StoppingCriterion`
+      but instead requires a parameter ``n_samples`` for the number of
+      iterations to run.
+
+    Additionally, one can use model-specific methods:
+
+    - ``knn``: Exact method for K-Nearest neighbour models. Implemented in
+      :func:`~pydvl.value.shapley.knn.knn_shapley`.
+
+    :param u: :class:`~pydvl.utils.utility.Utility` object with model, data, and
+        scoring function.
+    :param done: :class:`~pydvl.value.stopping.StoppingCriterion` object, used
+        to determine when to stop the computation for Monte Carlo methods. The
+        default is to stop after 100 iterations. See the available criteria in
+        :mod:`~pydvl.value.stopping`. It is possible to combine several criteria
+        using boolean operators. Some methods ignore this argument, others
+        require specific subtypes.
+    :param n_jobs: Number of parallel jobs (available only to some methods)
+    :param mode: Choose which shapley algorithm to use. See
+        :class:`~pydvl.value.shapley.ShapleyMode` for a list of allowed value.
 
+    :return: A :class:`~pydvl.value.result.ValuationResult` object with the
+        results.
 
-logger = logging.getLogger(__name__)
+    """
+    progress: bool = kwargs.pop("progress", False)
 
+    if mode not in list(ShapleyMode):
+        raise ValueError(f"Invalid value encountered in {mode=}")
 
-def get_shapley_coordinator(
-    *args, config: ParallelConfig = ParallelConfig(), **kwargs
-) -> "ShapleyCoordinator":
-    if config.backend == "ray":
-        coordinator = cast(
-            ShapleyCoordinator,
-            RayActorWrapper(ShapleyCoordinator, config, *args, **kwargs),
+    if mode == ShapleyMode.TruncatedMontecarlo:
+        truncation = kwargs.pop("truncation", NoTruncation())
+        return truncated_montecarlo_shapley(  # type: ignore
+            u=u, done=done, n_jobs=n_jobs, truncation=truncation, **kwargs
         )
-    elif config.backend == "sequential":
-        coordinator = ShapleyCoordinator(*args, **kwargs)
-    else:
-        raise NotImplementedError(f"Unexpected parallel type {config.backend}")
-    return coordinator
-
-
-def get_shapley_worker(
-    u: Utility, *args, config: ParallelConfig = ParallelConfig(), **kwargs
-) -> "ShapleyWorker":
-    parallel_backend = init_parallel_backend(config)
-    u_id = parallel_backend.put(u)
-    if config.backend == "ray":
-        worker = cast(
-            ShapleyWorker, RayActorWrapper(ShapleyWorker, config, u_id, *args, **kwargs)
+    elif mode == ShapleyMode.CombinatorialMontecarlo:
+        return combinatorial_montecarlo_shapley(
+            u, done=done, n_jobs=n_jobs, progress=progress
+        )
+    elif mode in (ShapleyMode.PermutationMontecarlo, ShapleyMode.ApproShapley):
+        truncation = kwargs.pop("truncation", NoTruncation())
+        return permutation_montecarlo_shapley(
+            u,
+            done=done,
+            n_jobs=n_jobs,
+            progress=progress,
+            truncation=truncation,
+            **kwargs,
+        )
+    elif mode == ShapleyMode.CombinatorialExact:
+        return combinatorial_exact_shapley(u, n_jobs=n_jobs, progress=progress)
+    elif mode == ShapleyMode.PermutationExact:
+        return permutation_exact_shapley(u, progress=progress)
+    elif mode == ShapleyMode.Owen or mode == ShapleyMode.OwenAntithetic:
+        if kwargs.get("n_samples") is None:
+            raise ValueError("n_samples cannot be None for Owen methods")
+        if kwargs.get("max_q") is None:
+            raise ValueError("Owen Sampling requires max_q for the outer integral")
+
+        method = (
+            OwenAlgorithm.Standard
+            if mode == ShapleyMode.Owen
+            else OwenAlgorithm.Antithetic
+        )
+        return owen_sampling_shapley(
+            u,
+            n_samples=int(kwargs.get("n_samples", -1)),
+            max_q=int(kwargs.get("max_q", -1)),
+            method=method,
+            n_jobs=n_jobs,
+        )
+    elif mode == ShapleyMode.KNN:
+        return knn_shapley(u, progress=progress)
+    elif mode == ShapleyMode.GroupTesting:
+        n_samples = kwargs.pop("n_samples")
+        if n_samples is None:
+            raise ValueError("n_samples cannot be None for Group Testing")
+        epsilon = kwargs.pop("epsilon")
+        if epsilon is None:
+            raise ValueError("Group Testing requires error bound epsilon")
+        delta = kwargs.pop("delta", 0.05)
+        return group_testing_shapley(
+            u,
+            epsilon=epsilon,
+            delta=delta,
+            n_samples=n_samples,
+            n_jobs=n_jobs,
+            progress=progress,
+            **kwargs,
         )
-    elif config.backend == "sequential":
-        worker = ShapleyWorker(u_id, *args, **kwargs)
     else:
-        raise NotImplementedError(f"Unexpected parallel type {config.backend}")
-    return worker
-
-
-class ShapleyCoordinator(Coordinator):
-    """The coordinator has two main tasks: aggregating the results of the
-    workers and terminating processes once a certain stopping criterion is
-    satisfied.
-    """
-
-    def __init__(self, done: StoppingCriterion):
-        super().__init__()
-        self.results_done = done
-        self.results_done.modify_result = True
-
-    def accumulate(self) -> ValuationResult:
-        """Accumulates all results received from the workers.
-
-        :return: Values and standard errors in a
-            :class:`~pydvl.value.result.ValuationResult`. If no worker has
-            reported yet, returns ``None``.
-        """
-        if len(self.worker_results) == 0:
-            return ValuationResult.empty()  # type: ignore
-
-        # FIXME: inefficient, possibly unstable
-        totals: ValuationResult = reduce(operator.add, self.worker_results)
-        # Avoid recomputing
-        self.worker_results = [totals]
-        return totals
-
-    def check_convergence(self) -> bool:
-        """Evaluates the convergence criterion on the accumulated results.
-
-        If the convergence criterion is satisfied, calls to
-        :meth:`~Coordinator.is_done` return ``True``.
-
-        :return: ``True`` if converged and ``False`` otherwise.
-        """
-        if self.is_done():
-            return True
-        if len(self.worker_results) > 0:
-            self._status = self.results_done(self.accumulate())
-        return self.is_done()
-
-
-class ShapleyWorker(Worker):
-    """A worker.
-
-    It should work.
-    """
-
-    algorithm: str = "truncated_montecarlo_shapley"
-
-    def __init__(
-        self,
-        u: Utility,
-        coordinator: ShapleyCoordinator,
-        *,
-        truncation: TruncationPolicy,
-        worker_id: int,
-        update_period: int = 30,
-    ):
-        """A worker calculates Shapley values using the permutation definition
-         and reports the results to the coordinator.
-
-         To implement early stopping, workers can be signaled by the
-         :class:`~pydvl.value.shapley.actor.ShapleyCoordinator` before they are
-         done with their work package
-
-        :param u: Utility object with model, data, and scoring function
-        :param coordinator: worker results will be pushed to this coordinator
-        :param worker_id: id used for reporting through maybe_progress
-        :param update_period: interval in seconds between different updates to
-            and from the coordinator
-        :param truncation: callable that decides whether to stop computing
-            marginals for a given permutation.
-        """
-        super().__init__(
-            coordinator=coordinator, update_period=update_period, worker_id=worker_id
-        )
-        self.u = u
-        self.truncation = truncation
-
-    def _compute_marginals(self) -> ValuationResult:
-        # Avoid circular imports
-        from .montecarlo import _permutation_montecarlo_shapley
-
-        return _permutation_montecarlo_shapley(
-            self.u,
-            done=MaxChecks(1),
-            truncation=self.truncation,
-            algorithm_name=self.algorithm,
-        )
-
-    def run(self, *args, **kwargs):
-        """Computes marginal utilities in a loop until signalled to stop.
-
-        This calls :meth:`_compute_marginals` repeatedly calculating Shapley
-        values on different permutations of the indices. After :attr:`update_period`
-        seconds have passed, it reports the results to the
-        :class:`~pydvl.value.shapley.actor.ShapleyCoordinator`. Before starting
-        the next iteration, it checks the coordinator's
-        :meth:`~pydvl.utils.parallel.actor.Coordinator.is_done` flag,
-        terminating if it's ``True``.
-        """
-        while True:
-            acc = ValuationResult.empty()
-            start_time = time()
-            while (time() - start_time) < self.update_period:
-                if self.coordinator.is_done():
-                    return
-                results = self._compute_marginals()
-                nans = np.isnan(results.values).sum()
-                if nans > 0:
-                    logger.warning(
-                        f"{nans} NaN values in current permutation, ignoring. "
-                        "Consider setting a default value for the Scorer"
-                    )
-                    continue
-                acc += results
-            self.coordinator.add_results(acc)
+        raise ValueError(f"Invalid value encountered in {mode=}")
```

### Comparing `pyDVL-0.6.0/src/pydvl/value/shapley/gt.py` & `pyDVL-0.6.1/src/pydvl/value/shapley/gt.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/shapley/knn.py` & `pyDVL-0.6.1/src/pydvl/value/shapley/knn.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/shapley/montecarlo.py` & `pyDVL-0.6.1/src/pydvl/value/shapley/montecarlo.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/shapley/naive.py` & `pyDVL-0.6.1/src/pydvl/value/shapley/naive.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/shapley/owen.py` & `pyDVL-0.6.1/src/pydvl/value/shapley/owen.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/src/pydvl/value/shapley/truncated.py` & `pyDVL-0.6.1/src/pydvl/value/shapley/truncated.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import abc
 import logging
-from time import sleep
+from concurrent.futures import FIRST_COMPLETED, wait
 
 import numpy as np
+from deprecate import deprecated
 
-from pydvl.utils import ParallelConfig, Utility, effective_n_jobs, running_moments
+from pydvl.utils import ParallelConfig, Utility, running_moments
+from pydvl.utils.parallel.backend import effective_n_jobs, init_parallel_backend
+from pydvl.utils.parallel.futures import init_executor
 from pydvl.value import ValuationResult
-from pydvl.value.stopping import StoppingCriterion
+from pydvl.value.stopping import MaxChecks, StoppingCriterion
 
 __all__ = [
     "TruncationPolicy",
     "NoTruncation",
     "FixedTruncation",
     "BootstrapTruncation",
     "RelativeTruncation",
@@ -153,21 +156,51 @@
         )
 
     def reset(self):
         self.count = 0
         self.variance = self.mean = 0
 
 
+def _permutation_montecarlo_one_step(
+    u: Utility,
+    truncation: TruncationPolicy,
+    algorithm: str,
+) -> ValuationResult:
+    # Avoid circular imports
+    from .montecarlo import _permutation_montecarlo_shapley
+
+    result = _permutation_montecarlo_shapley(
+        u,
+        done=MaxChecks(1),
+        truncation=truncation,
+        algorithm_name=algorithm,
+    )
+    nans = np.isnan(result.values).sum()
+    if nans > 0:
+        logger.warning(
+            f"{nans} NaN values in current permutation, ignoring. "
+            "Consider setting a default value for the Scorer"
+        )
+        result = ValuationResult.empty(algorithm="truncated_montecarlo_shapley")
+    return result
+
+
+@deprecated(
+    target=True,
+    deprecated_in="0.6.1",
+    remove_in="0.7.0",
+    args_mapping=dict(coordinator_update_period=None, worker_update_period=None),
+)
 def truncated_montecarlo_shapley(
     u: Utility,
     *,
     done: StoppingCriterion,
     truncation: TruncationPolicy,
-    n_jobs: int = 1,
     config: ParallelConfig = ParallelConfig(),
+    n_jobs: int = 1,
     coordinator_update_period: int = 10,
     worker_update_period: int = 5,
 ) -> ValuationResult:
     """Monte Carlo approximation to the Shapley value of data points.
 
     This implements the permutation-based method described in
     :footcite:t:`ghorbani_data_2019`. It is a Monte Carlo estimate of the sum
@@ -192,59 +225,64 @@
     until the :class:`StoppingCriterion` returns ``True``.
 
     :param u: Utility object with model, data, and scoring function
     :param done: Check on the results which decides when to stop
         sampling permutations.
     :param truncation: callable that decides whether to stop computing
         marginals for a given permutation.
-    :param n_jobs: number of jobs processing permutations. If None, it will be
-        set to :func:`available_cpus`.
     :param config: Object configuring parallel computation, with cluster
         address, number of cpus, etc.
+    :param n_jobs: Number of permutation monte carlo jobs
+        to run concurrently.
     :param coordinator_update_period: in seconds. How often to check the
         accumulated results from the workers for convergence.
     :param worker_update_period: interval in seconds between different
         updates to and from the coordinator
     :return: Object with the data values.
 
     """
-    # Avoid circular imports
-    from .actor import get_shapley_coordinator, get_shapley_worker
+    algorithm = "truncated_montecarlo_shapley"
 
-    if config.backend == "sequential":
-        raise NotImplementedError(
-            "Truncated MonteCarlo Shapley does not work with "
-            "the Sequential parallel backend."
-        )
-
-    coordinator = get_shapley_coordinator(config=config, done=done)  # type: ignore
-
-    workers = [
-        get_shapley_worker(  # type: ignore
-            u,
-            coordinator=coordinator,
-            truncation=truncation,
-            worker_id=worker_id,
-            update_period=worker_update_period,
-            config=config,
-        )
-        for worker_id in range(effective_n_jobs(n_jobs, config=config))
-    ]
-    for worker in workers:
-        worker.run(block=False)
-
-    while not coordinator.check_convergence():
-        sleep(coordinator_update_period)
-
-    return coordinator.accumulate()
-
-    # Something like this would be nicer, but it doesn't seem to be possible
-    # to start the workers from the coordinator.
-    # coordinator.add_workers(
-    #     n_workers=n_jobs,
-    #     u=u_id,
-    #     update_period=worker_update_period,
-    #     config=config,
-    #     truncation=truncation,
-    # )
-    #
-    # return coordinator.run(delay=coordinator_update_period)
+    parallel_backend = init_parallel_backend(config)
+    u = parallel_backend.put(u)
+    # This represents the number of jobs that are running
+    n_jobs = effective_n_jobs(n_jobs, config)
+    # This determines the total number of submitted jobs
+    # including the ones that are running
+    n_submitted_jobs = 2 * n_jobs
+
+    accumulated_result = ValuationResult.zeros(algorithm=algorithm)
+
+    with init_executor(max_workers=n_jobs, config=config) as executor:
+        futures = set()
+        # Initial batch of computations
+        for _ in range(n_submitted_jobs):
+            future = executor.submit(
+                _permutation_montecarlo_one_step,
+                u,
+                truncation,
+                algorithm,
+            )
+            futures.add(future)
+        while futures:
+            # Wait for the next futures to complete.
+            completed_futures, futures = wait(
+                futures, timeout=60, return_when=FIRST_COMPLETED
+            )
+            for future in completed_futures:
+                accumulated_result += future.result()
+                if done(accumulated_result):
+                    break
+            if done(accumulated_result):
+                break
+            # Submit more computations
+            # The goal is to always have `n_jobs`
+            # computations running
+            for _ in range(n_submitted_jobs - len(futures)):
+                future = executor.submit(
+                    _permutation_montecarlo_one_step,
+                    u,
+                    truncation,
+                    algorithm,
+                )
+                futures.add(future)
+    return accumulated_result
```

### Comparing `pyDVL-0.6.0/src/pydvl/value/stopping.py` & `pyDVL-0.6.1/src/pydvl/value/stopping.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/tests/test_plugin.py` & `pyDVL-0.6.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.6.0/tests/test_results.py` & `pyDVL-0.6.1/tests/test_results.py`

 * *Files identical despite different names*

