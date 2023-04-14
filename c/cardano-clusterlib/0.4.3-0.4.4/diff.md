# Comparing `tmp/cardano-clusterlib-0.4.3.tar.gz` & `tmp/cardano-clusterlib-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardano-clusterlib-0.4.3.tar", last modified: Tue Apr  4 12:33:42 2023, max compression
+gzip compressed data, was "cardano-clusterlib-0.4.4.tar", last modified: Fri Apr 14 10:59:52 2023, max compression
```

## Comparing `cardano-clusterlib-0.4.3.tar` & `cardano-clusterlib-0.4.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-04 12:33:42.425776 cardano-clusterlib-0.4.3/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-04 12:33:42.421776 cardano-clusterlib-0.4.3/.github/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-04 12:33:42.423776 cardano-clusterlib-0.4.3/.github/workflows/
--rw-r--r--   0 martink   (1000) martink   (1000)      353 2022-08-30 10:58:34.000000 cardano-clusterlib-0.4.3/.github/workflows/repo_lint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.4.3/.gitignore
--rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.3/.markdownlint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     1744 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.4.3/.pylintrc
--rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.4.3/.readthedocs.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.3/CODE-OF-CONDUCT.md
--rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.3/LICENSE
--rw-r--r--   0 martink   (1000) martink   (1000)     1139 2023-01-20 16:01:27.000000 cardano-clusterlib-0.4.3/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-04-04 12:33:42.425776 cardano-clusterlib-0.4.3/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.4.3/README.md
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-04 12:33:42.424776 cardano-clusterlib-0.4.3/cardano_clusterlib/
--rw-r--r--   0 martink   (1000) martink   (1000)      174 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/__init__.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7436 2023-03-28 11:41:48.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/address_group.py
--rw-rw-r--   0 martink   (1000) martink   (1000)     2593 2022-08-06 21:08:03.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/clusterlib.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7791 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/clusterlib_helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)    14563 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/clusterlib_klass.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1086 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/consts.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1111 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/coverage.py
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/exceptions.py
--rw-r--r--   0 martink   (1000) martink   (1000)     3799 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/genesis_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7438 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/governance_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)     2815 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/key_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6004 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/node_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/py.typed
--rw-r--r--   0 martink   (1000) martink   (1000)    18162 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/query_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    12602 2023-04-04 10:13:49.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/stake_address_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    12907 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/stake_pool_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6801 2023-02-08 09:40:33.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/structs.py
--rw-r--r--   0 martink   (1000) martink   (1000)    61308 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/transaction_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    44202 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/txtools.py
--rw-r--r--   0 martink   (1000) martink   (1000)      608 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.3/cardano_clusterlib/types.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-04 12:33:42.425776 cardano-clusterlib-0.4.3/cardano_clusterlib.egg-info/
--rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-04-04 12:33:42.000000 cardano-clusterlib-0.4.3/cardano_clusterlib.egg-info/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     1383 2023-04-04 12:33:42.000000 cardano-clusterlib-0.4.3/cardano_clusterlib.egg-info/SOURCES.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-04-04 12:33:42.000000 cardano-clusterlib-0.4.3/cardano_clusterlib.egg-info/dependency_links.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.4.3/cardano_clusterlib.egg-info/not-zip-safe
--rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-04-04 12:33:42.000000 cardano-clusterlib-0.4.3/cardano_clusterlib.egg-info/requires.txt
--rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-04-04 12:33:42.000000 cardano-clusterlib-0.4.3/cardano_clusterlib.egg-info/top_level.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-04 12:33:42.425776 cardano-clusterlib-0.4.3/docs/
--rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.4.3/docs/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.3/docs/requirements.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-04 12:33:42.425776 cardano-clusterlib-0.4.3/docs/source/
--rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.3/docs/source/cardano_clusterlib.rst
--rw-r--r--   0 martink   (1000) martink   (1000)     4080 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.3/docs/source/conf.py
--rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.4.3/docs/source/index.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.4.3/docs/source/modules.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.4.3/docs/source/readme.rst
--rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.4.3/mypy.ini
--rw-r--r--   0 martink   (1000) martink   (1000)      521 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.3/pyproject.toml
--rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.4.3/requirements-dev.txt
--rw-r--r--   0 martink   (1000) martink   (1000)     1128 2023-04-04 12:33:42.426776 cardano-clusterlib-0.4.3/setup.cfg
--rw-r--r--   0 martink   (1000) martink   (1000)      163 2021-08-27 11:24:08.000000 cardano-clusterlib-0.4.3/setup.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-04 12:33:42.425776 cardano-clusterlib-0.4.3/upgrading/
--rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.3/upgrading/refactor_to_0_4_0rc1.sed
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.674931 cardano-clusterlib-0.4.4/
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.668931 cardano-clusterlib-0.4.4/.github/
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.670931 cardano-clusterlib-0.4.4/.github/workflows/
+-rw-r--r--   0 martink   (1000) martink   (1000)      353 2022-08-30 10:58:34.000000 cardano-clusterlib-0.4.4/.github/workflows/repo_lint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.4.4/.gitignore
+-rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.4/.markdownlint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     1744 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.4.4/.pylintrc
+-rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.4.4/.readthedocs.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.4/CODE-OF-CONDUCT.md
+-rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.4/LICENSE
+-rw-r--r--   0 martink   (1000) martink   (1000)     1279 2023-04-14 10:59:03.000000 cardano-clusterlib-0.4.4/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-04-14 10:59:52.674931 cardano-clusterlib-0.4.4/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.4.4/README.md
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.672931 cardano-clusterlib-0.4.4/cardano_clusterlib/
+-rw-r--r--   0 martink   (1000) martink   (1000)      174 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/__init__.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     8083 2023-04-14 10:37:46.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/address_group.py
+-rw-rw-r--   0 martink   (1000) martink   (1000)     2593 2022-08-06 21:08:03.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7791 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib_helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    14563 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib_klass.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1086 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/consts.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1111 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/coverage.py
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/exceptions.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     3799 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/genesis_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7438 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/governance_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     2815 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/key_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     6004 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/node_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/py.typed
+-rw-r--r--   0 martink   (1000) martink   (1000)    18162 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/query_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    13370 2023-04-14 10:37:46.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/stake_address_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    12907 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/stake_pool_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     6801 2023-02-08 09:40:33.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/structs.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    61308 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/transaction_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    44202 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/txtools.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      608 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/types.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.672931 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/
+-rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-04-14 10:59:52.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     1383 2023-04-14 10:59:52.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/SOURCES.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-04-14 10:59:52.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/dependency_links.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/not-zip-safe
+-rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-04-14 10:59:52.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/requires.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-04-14 10:59:52.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/top_level.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.672931 cardano-clusterlib-0.4.4/docs/
+-rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.4.4/docs/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.4/docs/requirements.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.673931 cardano-clusterlib-0.4.4/docs/source/
+-rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.4/docs/source/cardano_clusterlib.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)     4080 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.4/docs/source/conf.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.4.4/docs/source/index.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.4.4/docs/source/modules.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.4.4/docs/source/readme.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.4.4/mypy.ini
+-rw-r--r--   0 martink   (1000) martink   (1000)      521 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.4/pyproject.toml
+-rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.4.4/requirements-dev.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)     1128 2023-04-14 10:59:52.674931 cardano-clusterlib-0.4.4/setup.cfg
+-rw-r--r--   0 martink   (1000) martink   (1000)      163 2021-08-27 11:24:08.000000 cardano-clusterlib-0.4.4/setup.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.674931 cardano-clusterlib-0.4.4/upgrading/
+-rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.4/upgrading/refactor_to_0_4_0rc1.sed
```

### Comparing `cardano-clusterlib-0.4.3/.gitignore` & `cardano-clusterlib-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/.markdownlint.yaml` & `cardano-clusterlib-0.4.4/.markdownlint.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/.pre-commit-config.yaml` & `cardano-clusterlib-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/.pylintrc` & `cardano-clusterlib-0.4.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/CODE-OF-CONDUCT.md` & `cardano-clusterlib-0.4.4/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/LICENSE` & `cardano-clusterlib-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/PKG-INFO` & `cardano-clusterlib-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cardano-clusterlib-0.4.3/README.md` & `cardano-clusterlib-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/address_group.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/address_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,48 +19,62 @@
 class AddressGroup:
     def __init__(self, clusterlib_obj: "types.ClusterLib") -> None:
         self._clusterlib_obj = clusterlib_obj
 
     def gen_payment_addr(
         self,
         addr_name: str,
+        payment_vkey: Optional[str] = None,
         payment_vkey_file: Optional[FileType] = None,
         payment_script_file: Optional[FileType] = None,
+        stake_vkey: Optional[str] = None,
         stake_vkey_file: Optional[FileType] = None,
         stake_script_file: Optional[FileType] = None,
+        stake_address: Optional[str] = None,
         destination_dir: FileType = ".",
     ) -> str:
         """Generate a payment address, with optional delegation to a stake address.
 
         Args:
             addr_name: A name of payment address.
+            payment_vkey: A vkey file (Bech32, optional).
             payment_vkey_file: A path to corresponding vkey file (optional).
             payment_script_file: A path to corresponding payment script file (optional).
+            stake_vkey: A stake vkey file (optional).
             stake_vkey_file: A path to corresponding stake vkey file (optional).
-            stake_script_file: A path to corresponding payment script file (optional).
+            stake_script_file: A path to corresponding stake script file (optional).
+            stake_address: A stake address (Bech32, optional).
             destination_dir: A path to directory for storing artifacts (optional).
 
         Returns:
             str: A generated payment address.
         """
         destination_dir = Path(destination_dir).expanduser()
         out_file = destination_dir / f"{addr_name}.addr"
         clusterlib_helpers._check_files_exist(out_file, clusterlib_obj=self._clusterlib_obj)
 
         if payment_vkey_file:
             cli_args = ["--payment-verification-key-file", str(payment_vkey_file)]
         elif payment_script_file:
             cli_args = ["--payment-script-file", str(payment_script_file)]
+        elif payment_vkey:
+            cli_args = ["--payment-verification-key", str(payment_vkey)]
         else:
-            raise AssertionError("Either `payment_vkey_file` or `payment_script_file` is needed.")
-
-        if stake_vkey_file:
+            raise AssertionError(
+                "Either `payment_vkey_file`, `payment_script_file` or `payment_vkey` is needed."
+            )
+
+        if stake_vkey:
+            cli_args.extend(["--stake-verification-key", str(stake_vkey)])
+        elif stake_vkey_file:
             cli_args.extend(["--stake-verification-key-file", str(stake_vkey_file)])
         elif stake_script_file:
             cli_args.extend(["--stake-script-file", str(stake_script_file)])
+        elif stake_address:
+            cli_args.extend(["--stake-address", str(stake_address)])
 
         self._clusterlib_obj.cli(
             [
                 "address",
                 "build",
                 *self._clusterlib_obj.magic_args,
                 *cli_args,
```

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/clusterlib.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/clusterlib_helpers.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib_helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/clusterlib_klass.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib_klass.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/consts.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/consts.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/coverage.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/coverage.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/genesis_group.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/genesis_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/governance_group.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/governance_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/helpers.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/key_group.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/key_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/node_group.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/node_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/query_group.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/query_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/stake_address_group.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/stake_address_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,37 +91,43 @@
         return structs.KeyPair(vkey, skey)
 
     def gen_stake_addr_registration_cert(
         self,
         addr_name: str,
         stake_vkey_file: Optional[FileType] = None,
         stake_script_file: Optional[FileType] = None,
+        stake_address: Optional[str] = None,
         destination_dir: FileType = ".",
     ) -> Path:
         """Generate a stake address registration certificate.
 
         Args:
             addr_name: A name of stake address.
             stake_vkey_file: A path to corresponding stake vkey file (optional).
-            stake_script_file: A path to corresponding payment script file (optional).
+            stake_script_file: A path to corresponding stake script file (optional).
+            stake_address: Stake address key, bech32 or hex-encoded (optional).
             destination_dir: A path to directory for storing artifacts (optional).
 
         Returns:
             Path: A path to the generated certificate.
         """
         destination_dir = Path(destination_dir).expanduser()
         out_file = destination_dir / f"{addr_name}_stake_reg.cert"
         clusterlib_helpers._check_files_exist(out_file, clusterlib_obj=self._clusterlib_obj)
 
         if stake_vkey_file:
             cli_args = ["--stake-verification-key-file", str(stake_vkey_file)]
         elif stake_script_file:
             cli_args = ["--stake-script-file", str(stake_script_file)]
+        elif stake_address:
+            cli_args = ["--stake-address", stake_address]
         else:
-            raise AssertionError("Either `stake_vkey_file` or `stake_script_file` is needed.")
+            raise AssertionError(
+                "Either `stake_vkey_file`, `stake_script_file` or `stake_address` is needed."
+            )
 
         self._clusterlib_obj.cli(
             [
                 "stake-address",
                 "registration-certificate",
                 *cli_args,
                 "--out-file",
@@ -133,37 +139,43 @@
         return out_file
 
     def gen_stake_addr_deregistration_cert(
         self,
         addr_name: str,
         stake_vkey_file: Optional[FileType] = None,
         stake_script_file: Optional[FileType] = None,
+        stake_address: Optional[str] = None,
         destination_dir: FileType = ".",
     ) -> Path:
         """Generate a stake address deregistration certificate.
 
         Args:
             addr_name: A name of stake address.
             stake_vkey_file: A path to corresponding stake vkey file (optional).
-            stake_script_file: A path to corresponding payment script file (optional).
+            stake_script_file: A path to corresponding stake script file (optional).
+            stake_address: Stake address key, bech32 or hex-encoded (optional).
             destination_dir: A path to directory for storing artifacts (optional).
 
         Returns:
             Path: A path to the generated certificate.
         """
         destination_dir = Path(destination_dir).expanduser()
         out_file = destination_dir / f"{addr_name}_stake_dereg.cert"
         clusterlib_helpers._check_files_exist(out_file, clusterlib_obj=self._clusterlib_obj)
 
         if stake_vkey_file:
             cli_args = ["--stake-verification-key-file", str(stake_vkey_file)]
         elif stake_script_file:
             cli_args = ["--stake-script-file", str(stake_script_file)]
+        elif stake_address:
+            cli_args = ["--stake-address", stake_address]
         else:
-            raise AssertionError("Either `stake_vkey_file` or `stake_script_file` is needed.")
+            raise AssertionError(
+                "Either `stake_vkey_file`, `stake_script_file` or `stake_address` is needed."
+            )
 
         self._clusterlib_obj.cli(
             [
                 "stake-address",
                 "deregistration-certificate",
                 *cli_args,
                 "--out-file",
@@ -175,24 +187,26 @@
         return out_file
 
     def gen_stake_addr_delegation_cert(
         self,
         addr_name: str,
         stake_vkey_file: Optional[FileType] = None,
         stake_script_file: Optional[FileType] = None,
+        stake_address: Optional[str] = None,
         cold_vkey_file: Optional[FileType] = None,
         stake_pool_id: str = "",
         destination_dir: FileType = ".",
     ) -> Path:
         """Generate a stake address delegation certificate.
 
         Args:
             addr_name: A name of stake address.
             stake_vkey_file: A path to corresponding stake vkey file (optional).
-            stake_script_file: A path to corresponding payment script file (optional).
+            stake_script_file: A path to corresponding stake script file (optional).
+            stake_address: Stake address key, bech32 or hex-encoded (optional).
             cold_vkey_file: A path to pool cold vkey file (optional).
             stake_pool_id: An ID of the stake pool (optional).
             destination_dir: A path to directory for storing artifacts (optional).
 
         Returns:
             Path: A path to the generated certificate.
         """
@@ -201,16 +215,20 @@
         clusterlib_helpers._check_files_exist(out_file, clusterlib_obj=self._clusterlib_obj)
 
         cli_args = []
         if stake_vkey_file:
             cli_args.extend(["--stake-verification-key-file", str(stake_vkey_file)])
         elif stake_script_file:
             cli_args.extend(["--stake-script-file", str(stake_script_file)])
+        elif stake_address:
+            cli_args = ["--stake-address", stake_address]
         else:
-            raise AssertionError("Either `stake_vkey_file` or `stake_script_file` is needed.")
+            raise AssertionError(
+                "Either `stake_vkey_file`, `stake_script_file` or `stake_address` is needed."
+            )
 
         if cold_vkey_file:
             cli_args.extend(
                 [
                     "--cold-verification-key-file",
                     str(cold_vkey_file),
                 ]
```

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/stake_pool_group.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/stake_pool_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/structs.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/structs.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/transaction_group.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/transaction_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/txtools.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/txtools.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib/types.py` & `cardano-clusterlib-0.4.4/cardano_clusterlib/types.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib.egg-info/PKG-INFO` & `cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cardano-clusterlib-0.4.3/cardano_clusterlib.egg-info/SOURCES.txt` & `cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/docs/Makefile` & `cardano-clusterlib-0.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/docs/source/cardano_clusterlib.rst` & `cardano-clusterlib-0.4.4/docs/source/cardano_clusterlib.rst`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/docs/source/conf.py` & `cardano-clusterlib-0.4.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/pyproject.toml` & `cardano-clusterlib-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/setup.cfg` & `cardano-clusterlib-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.3/upgrading/refactor_to_0_4_0rc1.sed` & `cardano-clusterlib-0.4.4/upgrading/refactor_to_0_4_0rc1.sed`

 * *Files identical despite different names*

