# Comparing `tmp/obp-0.5.5.tar.gz` & `tmp/obp-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obp-0.5.5.tar", last modified: Wed Jun 15 06:09:41 2022, max compression
+gzip compressed data, was "obp-0.5.6.tar", last modified: Fri Apr 14 20:39:12 2023, max compression
```

## Comparing `obp-0.5.5.tar` & `obp-0.5.6.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.577586 obp-0.5.5/
--rw-r--r--   0 usaito     (501) staff       (20)     1197 2021-03-20 12:31:29.000000 obp-0.5.5/CONTRIBUTING.md
--rw-r--r--   0 usaito     (501) staff       (20)    11384 2020-08-18 02:58:21.000000 obp-0.5.5/LICENSE
--rw-r--r--   0 usaito     (501) staff       (20)      115 2021-02-07 14:46:04.000000 obp-0.5.5/MANIFEST.in
--rw-r--r--   0 usaito     (501) staff       (20)    30823 2022-06-15 06:09:41.577969 obp-0.5.5/PKG-INFO
--rw-r--r--   0 usaito     (501) staff       (20)    26372 2022-06-15 06:09:06.000000 obp-0.5.5/README.md
--rw-r--r--   0 usaito     (501) staff       (20)    27676 2022-06-15 06:09:06.000000 obp-0.5.5/README_JN.md
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.531828 obp-0.5.5/obp/
--rw-r--r--   0 usaito     (501) staff       (20)      264 2021-11-11 07:03:01.000000 obp-0.5.5/obp/__init__.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.535501 obp-0.5.5/obp/dataset/
--rw-r--r--   0 usaito     (501) staff       (20)     2600 2022-04-03 21:53:03.000000 obp-0.5.5/obp/dataset/__init__.py
--rw-r--r--   0 usaito     (501) staff       (20)      848 2022-01-12 23:12:35.000000 obp-0.5.5/obp/dataset/base.py
--rw-r--r--   0 usaito     (501) staff       (20)    14801 2022-01-12 23:12:35.000000 obp-0.5.5/obp/dataset/multiclass.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.528000 obp-0.5.5/obp/dataset/obd/
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.527868 obp-0.5.5/obp/dataset/obd/bts/
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.540820 obp-0.5.5/obp/dataset/obd/bts/all/
--rw-r--r--   0 usaito     (501) staff       (20)  5084456 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/bts/all/all.csv
--rw-r--r--   0 usaito     (501) staff       (20)    10041 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/bts/all/item_context.csv
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.541247 obp-0.5.5/obp/dataset/obd/bts/men/
--rw-r--r--   0 usaito     (501) staff       (20)     4287 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/bts/men/item_context.csv
--rw-r--r--   0 usaito     (501) staff       (20)  3240432 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/bts/men/men.csv
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.545046 obp-0.5.5/obp/dataset/obd/bts/women/
--rw-r--r--   0 usaito     (501) staff       (20)     5792 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/bts/women/item_context.csv
--rw-r--r--   0 usaito     (501) staff       (20)  3722697 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/bts/women/women.csv
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.528321 obp-0.5.5/obp/dataset/obd/random/
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.561235 obp-0.5.5/obp/dataset/obd/random/all/
--rw-r--r--   0 usaito     (501) staff       (20)  5039451 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/random/all/all.csv
--rw-r--r--   0 usaito     (501) staff       (20)    10041 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/random/all/item_context.csv
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.562219 obp-0.5.5/obp/dataset/obd/random/men/
--rw-r--r--   0 usaito     (501) staff       (20)     4287 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/random/men/item_context.csv
--rw-r--r--   0 usaito     (501) staff       (20)  3336811 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/random/men/men.csv
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.566938 obp-0.5.5/obp/dataset/obd/random/women/
--rw-r--r--   0 usaito     (501) staff       (20)     5792 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/random/women/item_context.csv
--rw-r--r--   0 usaito     (501) staff       (20)  3817771 2021-02-07 14:46:04.000000 obp-0.5.5/obp/dataset/obd/random/women/women.csv
--rw-r--r--   0 usaito     (501) staff       (20)    13843 2022-01-12 23:12:35.000000 obp-0.5.5/obp/dataset/real.py
--rw-r--r--   0 usaito     (501) staff       (20)      315 2021-03-20 12:31:29.000000 obp-0.5.5/obp/dataset/reward_type.py
--rw-r--r--   0 usaito     (501) staff       (20)    33935 2022-04-27 23:22:04.000000 obp-0.5.5/obp/dataset/synthetic.py
--rw-r--r--   0 usaito     (501) staff       (20)    15792 2022-01-13 02:38:38.000000 obp-0.5.5/obp/dataset/synthetic_continuous.py
--rw-r--r--   0 usaito     (501) staff       (20)    15417 2022-06-15 05:22:45.000000 obp-0.5.5/obp/dataset/synthetic_embed.py
--rw-r--r--   0 usaito     (501) staff       (20)    14517 2022-04-03 21:53:03.000000 obp-0.5.5/obp/dataset/synthetic_multi.py
--rw-r--r--   0 usaito     (501) staff       (20)    70424 2022-06-15 05:22:45.000000 obp-0.5.5/obp/dataset/synthetic_slate.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.574639 obp-0.5.5/obp/ope/
--rw-r--r--   0 usaito     (501) staff       (20)     5790 2022-04-03 21:53:03.000000 obp-0.5.5/obp/ope/__init__.py
--rw-r--r--   0 usaito     (501) staff       (20)    27138 2022-04-03 21:53:03.000000 obp-0.5.5/obp/ope/classification_model.py
--rw-r--r--   0 usaito     (501) staff       (20)    99758 2022-06-15 05:22:45.000000 obp-0.5.5/obp/ope/estimators.py
--rw-r--r--   0 usaito     (501) staff       (20)    29201 2022-04-03 21:53:03.000000 obp-0.5.5/obp/ope/estimators_continuous.py
--rw-r--r--   0 usaito     (501) staff       (20)    30094 2022-06-15 05:22:45.000000 obp-0.5.5/obp/ope/estimators_embed.py
--rw-r--r--   0 usaito     (501) staff       (20)    78206 2022-04-03 21:53:03.000000 obp-0.5.5/obp/ope/estimators_multi.py
--rw-r--r--   0 usaito     (501) staff       (20)    43716 2022-04-03 21:53:03.000000 obp-0.5.5/obp/ope/estimators_slate.py
--rw-r--r--   0 usaito     (501) staff       (20)    69301 2022-06-15 05:22:45.000000 obp-0.5.5/obp/ope/estimators_tuning.py
--rw-r--r--   0 usaito     (501) staff       (20)     7990 2022-06-15 05:22:45.000000 obp-0.5.5/obp/ope/helper.py
--rw-r--r--   0 usaito     (501) staff       (20)    49157 2022-06-15 05:22:45.000000 obp-0.5.5/obp/ope/meta.py
--rw-r--r--   0 usaito     (501) staff       (20)    28563 2022-04-03 21:53:03.000000 obp-0.5.5/obp/ope/meta_continuous.py
--rw-r--r--   0 usaito     (501) staff       (20)    37003 2022-04-03 21:53:03.000000 obp-0.5.5/obp/ope/meta_multi.py
--rw-r--r--   0 usaito     (501) staff       (20)    31117 2022-04-03 21:53:03.000000 obp-0.5.5/obp/ope/meta_slate.py
--rw-r--r--   0 usaito     (501) staff       (20)    15050 2022-04-03 21:53:03.000000 obp-0.5.5/obp/ope/regression_model.py
--rw-r--r--   0 usaito     (501) staff       (20)    16919 2022-04-03 21:53:03.000000 obp-0.5.5/obp/ope/regression_model_slate.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.576854 obp-0.5.5/obp/policy/
--rw-r--r--   0 usaito     (501) staff       (20)     1314 2021-11-11 07:03:01.000000 obp-0.5.5/obp/policy/__init__.py
--rw-r--r--   0 usaito     (501) staff       (20)     7220 2022-04-03 21:53:03.000000 obp-0.5.5/obp/policy/base.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.577044 obp-0.5.5/obp/policy/conf/
--rw-r--r--   0 usaito     (501) staff       (20)     3968 2020-10-22 21:40:34.000000 obp-0.5.5/obp/policy/conf/prior_bts.yaml
--rw-r--r--   0 usaito     (501) staff       (20)     8481 2022-01-12 23:12:35.000000 obp-0.5.5/obp/policy/contextfree.py
--rw-r--r--   0 usaito     (501) staff       (20)     9270 2022-01-12 23:12:35.000000 obp-0.5.5/obp/policy/linear.py
--rw-r--r--   0 usaito     (501) staff       (20)    10980 2022-04-03 21:53:03.000000 obp-0.5.5/obp/policy/logistic.py
--rw-r--r--   0 usaito     (501) staff       (20)    73089 2022-06-15 05:22:45.000000 obp-0.5.5/obp/policy/offline.py
--rw-r--r--   0 usaito     (501) staff       (20)    40844 2022-04-03 22:56:53.000000 obp-0.5.5/obp/policy/offline_continuous.py
--rw-r--r--   0 usaito     (501) staff       (20)      409 2021-03-20 12:31:29.000000 obp-0.5.5/obp/policy/policy_type.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.577417 obp-0.5.5/obp/simulator/
--rw-r--r--   0 usaito     (501) staff       (20)      208 2021-10-25 22:42:25.000000 obp-0.5.5/obp/simulator/__init__.py
--rwxr-xr-x   0 usaito     (501) staff       (20)     6381 2022-01-12 23:12:35.000000 obp-0.5.5/obp/simulator/simulator.py
--rw-r--r--   0 usaito     (501) staff       (20)      279 2021-11-11 07:03:01.000000 obp-0.5.5/obp/types.py
--rwxr-xr-x   0 usaito     (501) staff       (20)    37122 2022-04-03 21:53:03.000000 obp-0.5.5/obp/utils.py
--rw-r--r--   0 usaito     (501) staff       (20)       22 2022-06-15 06:09:06.000000 obp-0.5.5/obp/version.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2022-06-15 06:09:41.533026 obp-0.5.5/obp.egg-info/
--rw-r--r--   0 usaito     (501) staff       (20)    30823 2022-06-15 06:09:41.000000 obp-0.5.5/obp.egg-info/PKG-INFO
--rw-r--r--   0 usaito     (501) staff       (20)     1686 2022-06-15 06:09:41.000000 obp-0.5.5/obp.egg-info/SOURCES.txt
--rw-r--r--   0 usaito     (501) staff       (20)        1 2022-06-15 06:09:41.000000 obp-0.5.5/obp.egg-info/dependency_links.txt
--rw-r--r--   0 usaito     (501) staff       (20)      186 2022-06-15 06:09:41.000000 obp-0.5.5/obp.egg-info/requires.txt
--rw-r--r--   0 usaito     (501) staff       (20)        4 2022-06-15 06:09:41.000000 obp-0.5.5/obp.egg-info/top_level.txt
--rw-r--r--   0 usaito     (501) staff       (20)      978 2022-06-15 06:09:06.000000 obp-0.5.5/pyproject.toml
--rw-r--r--   0 usaito     (501) staff       (20)      101 2022-06-15 06:09:41.578448 obp-0.5.5/setup.cfg
--rw-r--r--   0 usaito     (501) staff       (20)     2029 2022-01-13 12:38:25.000000 obp-0.5.5/setup.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.739784 obp-0.5.6/
+-rw-r--r--   0 usaito     (501) staff       (20)     1197 2021-03-20 12:31:29.000000 obp-0.5.6/CONTRIBUTING.md
+-rw-r--r--   0 usaito     (501) staff       (20)    11384 2020-08-18 02:58:21.000000 obp-0.5.6/LICENSE
+-rw-r--r--   0 usaito     (501) staff       (20)      115 2021-02-07 14:46:04.000000 obp-0.5.6/MANIFEST.in
+-rw-r--r--   0 usaito     (501) staff       (20)    30824 2023-04-14 20:39:12.740051 obp-0.5.6/PKG-INFO
+-rw-r--r--   0 usaito     (501) staff       (20)    26372 2022-11-13 12:29:47.000000 obp-0.5.6/README.md
+-rw-r--r--   0 usaito     (501) staff       (20)    27676 2022-06-15 06:09:06.000000 obp-0.5.6/README_JN.md
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.690186 obp-0.5.6/obp/
+-rw-r--r--   0 usaito     (501) staff       (20)      264 2021-11-11 07:03:01.000000 obp-0.5.6/obp/__init__.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.693219 obp-0.5.6/obp/dataset/
+-rw-r--r--   0 usaito     (501) staff       (20)     2600 2022-04-03 21:53:03.000000 obp-0.5.6/obp/dataset/__init__.py
+-rw-r--r--   0 usaito     (501) staff       (20)      848 2022-01-12 23:12:35.000000 obp-0.5.6/obp/dataset/base.py
+-rw-r--r--   0 usaito     (501) staff       (20)    14801 2022-01-12 23:12:35.000000 obp-0.5.6/obp/dataset/multiclass.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.687338 obp-0.5.6/obp/dataset/obd/
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.687264 obp-0.5.6/obp/dataset/obd/bts/
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.698280 obp-0.5.6/obp/dataset/obd/bts/all/
+-rw-r--r--   0 usaito     (501) staff       (20)  5084456 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/all/all.csv
+-rw-r--r--   0 usaito     (501) staff       (20)    10041 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/all/item_context.csv
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.698828 obp-0.5.6/obp/dataset/obd/bts/men/
+-rw-r--r--   0 usaito     (501) staff       (20)     4287 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/men/item_context.csv
+-rw-r--r--   0 usaito     (501) staff       (20)  3240432 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/men/men.csv
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.704648 obp-0.5.6/obp/dataset/obd/bts/women/
+-rw-r--r--   0 usaito     (501) staff       (20)     5792 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/women/item_context.csv
+-rw-r--r--   0 usaito     (501) staff       (20)  3722697 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/women/women.csv
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.687542 obp-0.5.6/obp/dataset/obd/random/
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.715574 obp-0.5.6/obp/dataset/obd/random/all/
+-rw-r--r--   0 usaito     (501) staff       (20)  5039451 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/all/all.csv
+-rw-r--r--   0 usaito     (501) staff       (20)    10041 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/all/item_context.csv
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.720272 obp-0.5.6/obp/dataset/obd/random/men/
+-rw-r--r--   0 usaito     (501) staff       (20)     4287 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/men/item_context.csv
+-rw-r--r--   0 usaito     (501) staff       (20)  3336811 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/men/men.csv
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.724654 obp-0.5.6/obp/dataset/obd/random/women/
+-rw-r--r--   0 usaito     (501) staff       (20)     5792 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/women/item_context.csv
+-rw-r--r--   0 usaito     (501) staff       (20)  3817771 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/women/women.csv
+-rw-r--r--   0 usaito     (501) staff       (20)    13843 2022-01-12 23:12:35.000000 obp-0.5.6/obp/dataset/real.py
+-rw-r--r--   0 usaito     (501) staff       (20)      315 2021-03-20 12:31:29.000000 obp-0.5.6/obp/dataset/reward_type.py
+-rw-r--r--   0 usaito     (501) staff       (20)    38494 2023-04-14 20:08:50.000000 obp-0.5.6/obp/dataset/synthetic.py
+-rw-r--r--   0 usaito     (501) staff       (20)    15792 2022-01-13 02:38:38.000000 obp-0.5.6/obp/dataset/synthetic_continuous.py
+-rw-r--r--   0 usaito     (501) staff       (20)    15417 2022-06-15 05:22:45.000000 obp-0.5.6/obp/dataset/synthetic_embed.py
+-rw-r--r--   0 usaito     (501) staff       (20)    14953 2022-11-13 22:21:58.000000 obp-0.5.6/obp/dataset/synthetic_multi.py
+-rw-r--r--   0 usaito     (501) staff       (20)    70424 2022-06-15 05:22:45.000000 obp-0.5.6/obp/dataset/synthetic_slate.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.735956 obp-0.5.6/obp/ope/
+-rw-r--r--   0 usaito     (501) staff       (20)     5790 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/__init__.py
+-rw-r--r--   0 usaito     (501) staff       (20)    27138 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/classification_model.py
+-rw-r--r--   0 usaito     (501) staff       (20)    99758 2022-06-15 05:22:45.000000 obp-0.5.6/obp/ope/estimators.py
+-rw-r--r--   0 usaito     (501) staff       (20)    29201 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/estimators_continuous.py
+-rw-r--r--   0 usaito     (501) staff       (20)    30094 2022-06-15 05:22:45.000000 obp-0.5.6/obp/ope/estimators_embed.py
+-rw-r--r--   0 usaito     (501) staff       (20)    78206 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/estimators_multi.py
+-rw-r--r--   0 usaito     (501) staff       (20)    43716 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/estimators_slate.py
+-rw-r--r--   0 usaito     (501) staff       (20)    69301 2022-06-15 05:22:45.000000 obp-0.5.6/obp/ope/estimators_tuning.py
+-rw-r--r--   0 usaito     (501) staff       (20)     7990 2022-06-15 05:22:45.000000 obp-0.5.6/obp/ope/helper.py
+-rw-r--r--   0 usaito     (501) staff       (20)    49157 2022-06-15 05:22:45.000000 obp-0.5.6/obp/ope/meta.py
+-rw-r--r--   0 usaito     (501) staff       (20)    28563 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/meta_continuous.py
+-rw-r--r--   0 usaito     (501) staff       (20)    37003 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/meta_multi.py
+-rw-r--r--   0 usaito     (501) staff       (20)    31117 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/meta_slate.py
+-rw-r--r--   0 usaito     (501) staff       (20)    15050 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/regression_model.py
+-rw-r--r--   0 usaito     (501) staff       (20)    16919 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/regression_model_slate.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.738584 obp-0.5.6/obp/policy/
+-rw-r--r--   0 usaito     (501) staff       (20)     1314 2021-11-11 07:03:01.000000 obp-0.5.6/obp/policy/__init__.py
+-rw-r--r--   0 usaito     (501) staff       (20)     7220 2022-04-03 21:53:03.000000 obp-0.5.6/obp/policy/base.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.738874 obp-0.5.6/obp/policy/conf/
+-rw-r--r--   0 usaito     (501) staff       (20)     3968 2020-10-22 21:40:34.000000 obp-0.5.6/obp/policy/conf/prior_bts.yaml
+-rw-r--r--   0 usaito     (501) staff       (20)     8481 2022-01-12 23:12:35.000000 obp-0.5.6/obp/policy/contextfree.py
+-rw-r--r--   0 usaito     (501) staff       (20)     9270 2022-01-12 23:12:35.000000 obp-0.5.6/obp/policy/linear.py
+-rw-r--r--   0 usaito     (501) staff       (20)    10980 2022-04-03 21:53:03.000000 obp-0.5.6/obp/policy/logistic.py
+-rw-r--r--   0 usaito     (501) staff       (20)    73129 2022-11-13 12:29:47.000000 obp-0.5.6/obp/policy/offline.py
+-rw-r--r--   0 usaito     (501) staff       (20)    40844 2022-04-03 22:56:53.000000 obp-0.5.6/obp/policy/offline_continuous.py
+-rw-r--r--   0 usaito     (501) staff       (20)      409 2021-03-20 12:31:29.000000 obp-0.5.6/obp/policy/policy_type.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.739646 obp-0.5.6/obp/simulator/
+-rw-r--r--   0 usaito     (501) staff       (20)      121 2022-11-13 12:29:47.000000 obp-0.5.6/obp/simulator/__init__.py
+-rw-r--r--   0 usaito     (501) staff       (20)     9161 2022-11-13 22:54:57.000000 obp-0.5.6/obp/simulator/coefficient_drifter.py
+-rw-r--r--   0 usaito     (501) staff       (20)     3804 2022-11-13 12:29:47.000000 obp-0.5.6/obp/simulator/delay_sampler.py
+-rw-r--r--   0 usaito     (501) staff       (20)     3226 2022-11-13 22:54:57.000000 obp-0.5.6/obp/simulator/replay.py
+-rwxr-xr-x   0 usaito     (501) staff       (20)    18637 2022-11-13 22:54:57.000000 obp-0.5.6/obp/simulator/simulator.py
+-rw-r--r--   0 usaito     (501) staff       (20)      279 2021-11-11 07:03:01.000000 obp-0.5.6/obp/types.py
+-rwxr-xr-x   0 usaito     (501) staff       (20)    37118 2022-11-13 12:29:47.000000 obp-0.5.6/obp/utils.py
+-rw-r--r--   0 usaito     (501) staff       (20)       22 2023-04-14 20:11:06.000000 obp-0.5.6/obp/version.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.690801 obp-0.5.6/obp.egg-info/
+-rw-r--r--   0 usaito     (501) staff       (20)    30824 2023-04-14 20:39:12.000000 obp-0.5.6/obp.egg-info/PKG-INFO
+-rw-r--r--   0 usaito     (501) staff       (20)     1778 2023-04-14 20:39:12.000000 obp-0.5.6/obp.egg-info/SOURCES.txt
+-rw-r--r--   0 usaito     (501) staff       (20)        1 2023-04-14 20:39:12.000000 obp-0.5.6/obp.egg-info/dependency_links.txt
+-rw-r--r--   0 usaito     (501) staff       (20)      185 2023-04-14 20:39:12.000000 obp-0.5.6/obp.egg-info/requires.txt
+-rw-r--r--   0 usaito     (501) staff       (20)        4 2023-04-14 20:39:12.000000 obp-0.5.6/obp.egg-info/top_level.txt
+-rw-r--r--   0 usaito     (501) staff       (20)      971 2023-04-14 20:10:55.000000 obp-0.5.6/pyproject.toml
+-rw-r--r--   0 usaito     (501) staff       (20)      101 2023-04-14 20:39:12.740390 obp-0.5.6/setup.cfg
+-rw-r--r--   0 usaito     (501) staff       (20)     2029 2023-04-14 20:14:27.000000 obp-0.5.6/setup.py
```

### Comparing `obp-0.5.5/CONTRIBUTING.md` & `obp-0.5.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/LICENSE` & `obp-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/PKG-INFO` & `obp-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obp
-Version: 0.5.5
+Version: 0.5.6
 Summary: Open Bandit Pipeline: a python library for bandit algorithms and off-policy evaluation
 Home-page: https://github.com/st-tech/zr-obp
 Author: Yuta Saito
 Author-email: open-bandit-project@googlegroups.com
 License: Apache License
 Description: <div align="center"><img src="https://raw.githubusercontent.com/st-tech/zr-obp/master/images/logo.png" width="60%"/></div>
         
@@ -83,15 +83,15 @@
         </p>
         </figcaption>
         
         Open Bandit Pipeline consists of the following main modules.
         
         - [**dataset module**](./obp/dataset/): This module provides a data loader for Open Bandit Dataset and a flexible interface for handling logged bandit data. It also provides tools to generate synthetic bandit data and transform multi-class classification data to bandit data.
         - [**policy module**](./obp/policy/): This module provides interfaces for implementing new online and offline bandit policies. It also implements several standard policy learning methods.
-        - [**simulator module**](./obp/simulator/): This module provides functions for conducting offline bandit simulation. This module is necessary only when you use the ReplayMethod to evaluate online bandit policies. Please refer to [examples/quickstart/online.ipynb](./examples/quickstart/online.ipynb) for a quickstart guide of implementing OPE of online bandit algorithms.
+        - [**simulator module**](./obp/simulator/): This module provides functions for conducting offline bandit simulation. This module is necessary only when you use the ReplayMethod to evaluate online bandit policies. Please refer to [examples/quickstart/online.ipynb](./examples/quickstart/replay.ipynb) for a quickstart guide of implementing OPE of online bandit algorithms.
         - [**ope module**](./obp/ope/): This module provides generic abstract interfaces to support custom implementations so that researchers can evaluate their own estimators easily. It also implements several basic and advanced OPE estimators.
         
         ### Supported Bandit Algorithms and OPE Estimators
         
         <details>
         <summary><strong>Bandit Algorithms </strong>(click to expand)</summary>
         <br>
@@ -436,17 +436,17 @@
         [[github](https://github.com/snap-stanford/ogb)] [[project page](https://ogb.stanford.edu)] [[paper](https://arxiv.org/abs/2005.00687)].
         
         </details>
         
 Keywords: bandit algorithms,off-policy evaluation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `obp-0.5.5/README.md` & `obp-0.5.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 </p>
 </figcaption>
 
 Open Bandit Pipeline consists of the following main modules.
 
 - [**dataset module**](./obp/dataset/): This module provides a data loader for Open Bandit Dataset and a flexible interface for handling logged bandit data. It also provides tools to generate synthetic bandit data and transform multi-class classification data to bandit data.
 - [**policy module**](./obp/policy/): This module provides interfaces for implementing new online and offline bandit policies. It also implements several standard policy learning methods.
-- [**simulator module**](./obp/simulator/): This module provides functions for conducting offline bandit simulation. This module is necessary only when you use the ReplayMethod to evaluate online bandit policies. Please refer to [examples/quickstart/online.ipynb](./examples/quickstart/online.ipynb) for a quickstart guide of implementing OPE of online bandit algorithms.
+- [**simulator module**](./obp/simulator/): This module provides functions for conducting offline bandit simulation. This module is necessary only when you use the ReplayMethod to evaluate online bandit policies. Please refer to [examples/quickstart/online.ipynb](./examples/quickstart/replay.ipynb) for a quickstart guide of implementing OPE of online bandit algorithms.
 - [**ope module**](./obp/ope/): This module provides generic abstract interfaces to support custom implementations so that researchers can evaluate their own estimators easily. It also implements several basic and advanced OPE estimators.
 
 ### Supported Bandit Algorithms and OPE Estimators
 
 <details>
 <summary><strong>Bandit Algorithms </strong>(click to expand)</summary>
 <br>
```

### Comparing `obp-0.5.5/README_JN.md` & `obp-0.5.6/README_JN.md`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/__init__.py` & `obp-0.5.6/obp/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/base.py` & `obp-0.5.6/obp/dataset/base.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/multiclass.py` & `obp-0.5.6/obp/dataset/multiclass.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/bts/all/all.csv` & `obp-0.5.6/obp/dataset/obd/bts/all/all.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/bts/all/item_context.csv` & `obp-0.5.6/obp/dataset/obd/bts/all/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/bts/men/item_context.csv` & `obp-0.5.6/obp/dataset/obd/bts/men/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/bts/men/men.csv` & `obp-0.5.6/obp/dataset/obd/bts/men/men.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/bts/women/item_context.csv` & `obp-0.5.6/obp/dataset/obd/bts/women/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/bts/women/women.csv` & `obp-0.5.6/obp/dataset/obd/bts/women/women.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/random/all/all.csv` & `obp-0.5.6/obp/dataset/obd/random/all/all.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/random/all/item_context.csv` & `obp-0.5.6/obp/dataset/obd/random/all/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/random/men/item_context.csv` & `obp-0.5.6/obp/dataset/obd/random/men/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/random/men/men.csv` & `obp-0.5.6/obp/dataset/obd/random/men/men.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/random/women/item_context.csv` & `obp-0.5.6/obp/dataset/obd/random/women/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/obd/random/women/women.csv` & `obp-0.5.6/obp/dataset/obd/random/women/women.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/real.py` & `obp-0.5.6/obp/dataset/real.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/synthetic.py` & `obp-0.5.6/obp/dataset/synthetic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Yuta Saito, Yusuke Narita, and ZOZO Technologies, Inc. All rights reserved.
 # Licensed under the Apache 2.0 License.
 
 """Class for Generating Synthetic Logged Bandit Data."""
 from dataclasses import dataclass
 from typing import Callable
 from typing import Optional
+from typing import Tuple
 
 import numpy as np
 from scipy.stats import truncnorm
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.utils import check_random_state
 from sklearn.utils import check_scalar
 
@@ -17,14 +18,34 @@
 from ..utils import sample_action_fast
 from ..utils import sigmoid
 from ..utils import softmax
 from .base import BaseBanditDataset
 from .reward_type import RewardType
 
 
+coef_func_signature = Callable[
+    [np.ndarray, np.ndarray, np.random.RandomState],
+    Tuple[np.ndarray, np.ndarray, np.ndarray],
+]
+
+
+def sample_random_uniform_coefficients(
+    effective_dim_action_context: int,
+    effective_dim_context: int,
+    random_: np.random.RandomState,
+    **kwargs,
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    context_coef_ = random_.uniform(-1, 1, size=effective_dim_context)
+    action_coef_ = random_.uniform(-1, 1, size=effective_dim_action_context)
+    context_action_coef_ = random_.uniform(
+        -1, 1, size=(effective_dim_context, effective_dim_action_context)
+    )
+    return context_coef_, action_coef_, context_action_coef_
+
+
 @dataclass
 class SyntheticBanditDataset(BaseBanditDataset):
     """Class for synthesizing bandit data.
 
     Note
     -----
     By calling the `obtain_batch_bandit_feedback` method several times,
@@ -54,14 +75,19 @@
         sampled from the uniform distribution automatically.
 
     reward_std: float, default=1.0
         Standard deviation of the reward distribution.
         A larger value leads to a noisier reward distribution.
         This argument is valid only when `reward_type="continuous"`.
 
+    reward_noise_distribution: str, default='normal'
+        From which distribution we sample noise on the reward, must be either 'normal' or 'truncated_normal'.
+        If 'truncated_normal' is given, we do not have any negative reward realization in the logged dataset.
+        This argument is valid only when `reward_type="continuous"`.
+
     action_context: np.ndarray, default=None
          Vector representation of (discrete) actions.
          If None, one-hot representation will be used.
 
     behavior_policy_function: Callable[[np.ndarray, np.ndarray], np.ndarray], default=None
         Function generating logit values, which will be used to define the behavior policy via softmax transformation.
         If None, behavior policy will be generated by applying the softmax function to the expected reward.
@@ -154,14 +180,15 @@
     """
 
     n_actions: int
     dim_context: int = 1
     reward_type: str = RewardType.BINARY.value
     reward_function: Optional[Callable[[np.ndarray, np.ndarray], np.ndarray]] = None
     reward_std: float = 1.0
+    reward_noise_distribution: str = "normal"
     action_context: Optional[np.ndarray] = None
     behavior_policy_function: Optional[
         Callable[[np.ndarray, np.ndarray], np.ndarray]
     ] = None
     beta: float = 1.0
     n_deficient_actions: int = 0
     random_state: int = 12345
@@ -188,14 +215,20 @@
             RewardType.BINARY,
             RewardType.CONTINUOUS,
         ]:
             raise ValueError(
                 f"`reward_type` must be either '{RewardType.BINARY.value}' or '{RewardType.CONTINUOUS.value}',"
                 f"but {self.reward_type} is given.'"
             )
+        if self.reward_noise_distribution not in ["normal", "truncated_normal"]:
+            raise ValueError(
+                f"`reward_noise_distribution` must be either 'normal' or 'truncated_normal',"
+                f"but {self.reward_noise_distribution} is given.'"
+            )
+
         check_scalar(self.reward_std, "reward_std", (int, float), min_val=0)
         if self.reward_function is None:
             self.expected_reward = self.sample_contextfree_expected_reward()
         if RewardType(self.reward_type) == RewardType.CONTINUOUS:
             self.reward_min = 0
             self.reward_max = 1e10
 
@@ -240,24 +273,31 @@
         action: np.ndarray,
     ) -> np.ndarray:
         """Sample reward given expected rewards"""
         expected_reward_factual = expected_reward[np.arange(action.shape[0]), action]
         if RewardType(self.reward_type) == RewardType.BINARY:
             reward = self.random_.binomial(n=1, p=expected_reward_factual)
         elif RewardType(self.reward_type) == RewardType.CONTINUOUS:
-            mean = expected_reward_factual
-            a = (self.reward_min - mean) / self.reward_std
-            b = (self.reward_max - mean) / self.reward_std
-            reward = truncnorm.rvs(
-                a=a,
-                b=b,
-                loc=mean,
-                scale=self.reward_std,
-                random_state=self.random_state,
-            )
+            if self.reward_noise_distribution == "normal":
+                reward = self.random_.normal(
+                    loc=expected_reward_factual,
+                    scale=self.reward_std,
+                    size=action.shape,
+                )
+            elif self.reward_noise_distribution == "truncated_normal":
+                mean = expected_reward_factual
+                a = (self.reward_min - mean) / self.reward_std
+                b = (self.reward_max - mean) / self.reward_std
+                reward = truncnorm.rvs(
+                    a=a,
+                    b=b,
+                    loc=mean,
+                    scale=self.reward_std,
+                    random_state=self.random_state,
+                )
         else:
             raise NotImplementedError
 
         return reward
 
     def sample_reward(self, context: np.ndarray, action: np.ndarray) -> np.ndarray:
         """Sample rewards given contexts and actions, i.e., :math:`r \\sim p(r | x, a)`.
@@ -306,20 +346,21 @@
         check_scalar(n_rounds, "n_rounds", int, min_val=1)
         contexts = self.random_.normal(size=(n_rounds, self.dim_context))
 
         # calc expected reward given context and action
         expected_reward_ = self.calc_expected_reward(contexts)
         if RewardType(self.reward_type) == RewardType.CONTINUOUS:
             # correct expected_reward_, as we use truncated normal distribution here
-            mean = expected_reward_
-            a = (self.reward_min - mean) / self.reward_std
-            b = (self.reward_max - mean) / self.reward_std
-            expected_reward_ = truncnorm.stats(
-                a=a, b=b, loc=mean, scale=self.reward_std, moments="m"
-            )
+            if self.reward_noise_distribution == "truncated_normal":
+                mean = expected_reward_
+                a = (self.reward_min - mean) / self.reward_std
+                b = (self.reward_max - mean) / self.reward_std
+                expected_reward_ = truncnorm.stats(
+                    a=a, b=b, loc=mean, scale=self.reward_std, moments="m"
+                )
 
         # calculate the action choice probabilities of the behavior policy
         if self.behavior_policy_function is None:
             pi_b_logits = expected_reward_
         else:
             pi_b_logits = self.behavior_policy_function(
                 context=contexts,
@@ -394,26 +435,35 @@
 
         return np.average(expected_reward, weights=action_dist[:, :, 0], axis=1).mean()
 
 
 def logistic_reward_function(
     context: np.ndarray,
     action_context: np.ndarray,
+    coef_function: coef_func_signature = sample_random_uniform_coefficients,
+    z_score: bool = True,
     random_state: Optional[int] = None,
 ) -> np.ndarray:
     """Logistic mean reward function for binary rewards.
 
     Parameters
     -----------
     context: array-like, shape (n_rounds, dim_context)
         Context vectors characterizing each data (such as user information).
 
     action_context: array-like, shape (n_actions, dim_action_context)
         Vector representation of actions.
 
+    z_score: boolean, default=True
+        Controls whether a z-score will be calculated over the computed logits.
+
+    coef_function: Callable, default=sample_random_uniform_coefficients
+        Function for generating the coefficients used for the context, action and context/action interactions.
+        By default, the coefficients are randomly uniformly drawn.
+
     random_state: int, default=None
         Controls the random seed in sampling dataset.
 
     Returns
     ---------
     expected_reward: array-like, shape (n_rounds, n_actions)
         Expected reward given context (:math:`x`) and action (:math:`a`),
@@ -421,22 +471,26 @@
 
     """
     logits = _base_reward_function(
         context=context,
         action_context=action_context,
         degree=1,
         random_state=random_state,
+        z_score=z_score,
+        coef_function=coef_function,
     )
 
     return sigmoid(logits)
 
 
 def logistic_polynomial_reward_function(
     context: np.ndarray,
     action_context: np.ndarray,
+    coef_function: coef_func_signature = sample_random_uniform_coefficients,
+    z_score: bool = True,
     random_state: Optional[int] = None,
 ) -> np.ndarray:
     """Logistic mean reward function for binary rewards with polynomial feature transformations.
 
     Note
     ------
     Polynomial and interaction features will be used to calculate the expected rewards.
@@ -446,37 +500,44 @@
     -----------
     context: array-like, shape (n_rounds, dim_context)
         Context vectors characterizing each data (such as user information).
 
     action_context: array-like, shape (n_actions, dim_action_context)
         Vector representation of actions.
 
+    z_score: boolean, default=True
+        Controls whether a z-score will be calculated over the computed logits.
+
     random_state: int, default=None
         Controls the random seed in sampling dataset.
 
     Returns
     ---------
     expected_reward: array-like, shape (n_rounds, n_actions)
         Expected reward given context (:math:`x`) and action (:math:`a`),
         i.e., :math:`q(x,a):=\\mathbb{E}[r|x,a]`.
 
     """
     logits = _base_reward_function(
         context=context,
         action_context=action_context,
         degree=3,
+        coef_function=coef_function,
+        z_score=z_score,
         random_state=random_state,
     )
 
     return sigmoid(logits)
 
 
 def logistic_sparse_reward_function(
     context: np.ndarray,
     action_context: np.ndarray,
+    coef_function: coef_func_signature = sample_random_uniform_coefficients,
+    z_score: bool = True,
     random_state: Optional[int] = None,
 ) -> np.ndarray:
     """Logistic mean reward function for binary rewards with small effective feature dimension.
 
     Note
     ------
     Polynomial and interaction features will be used to calculate the expected rewards.
@@ -487,14 +548,17 @@
     -----------
     context: array-like, shape (n_rounds, dim_context)
         Context vectors characterizing each data (such as user information).
 
     action_context: array-like, shape (n_actions, dim_action_context)
         Vector representation of actions.
 
+    z_score: boolean, default=True
+        Controls whether a z-score will be calculated over the computed logits.
+
     random_state: int, default=None
         Controls the random seed in sampling dataset.
 
     Returns
     ---------
     expected_reward: array-like, shape (n_rounds, n_actions)
         Expected reward given context (:math:`x`) and action (:math:`a`),
@@ -502,56 +566,67 @@
 
     """
     logits = _base_reward_function(
         context=context,
         action_context=action_context,
         degree=4,
         effective_dim_ratio=0.3,
+        coef_function=coef_function,
+        z_score=z_score,
         random_state=random_state,
     )
 
     return sigmoid(logits)
 
 
 def linear_reward_function(
     context: np.ndarray,
     action_context: np.ndarray,
+    coef_function: coef_func_signature = sample_random_uniform_coefficients,
+    z_score: bool = True,
     random_state: Optional[int] = None,
 ) -> np.ndarray:
     """Linear mean reward function for continuous rewards.
 
     Parameters
     -----------
     context: array-like, shape (n_rounds, dim_context)
         Context vectors characterizing each data (such as user information).
 
     action_context: array-like, shape (n_actions, dim_action_context)
         Vector representation of actions.
 
+    z_score: boolean, default=True
+        Controls whether a z-score will be calculated over the computed logits.
+
     random_state: int, default=None
         Controls the random seed in sampling dataset.
 
     Returns
     ---------
     expected_rewards: array-like, shape (n_rounds, n_actions)
         Expected reward given context (:math:`x`) and action (:math:`a`),
         i.e., :math:`q(x,a):=\\mathbb{E}[r|x,a]`.
 
     """
     return _base_reward_function(
         context=context,
         action_context=action_context,
         degree=1,
+        coef_function=coef_function,
+        z_score=z_score,
         random_state=random_state,
     )
 
 
 def polynomial_reward_function(
     context: np.ndarray,
     action_context: np.ndarray,
+    coef_function: coef_func_signature = sample_random_uniform_coefficients,
+    z_score: bool = True,
     random_state: Optional[int] = None,
 ) -> np.ndarray:
     """Polynomial mean reward function for continuous rewards.
 
     Note
     ------
     Polynomial and interaction features will be used to calculate the expected rewards.
@@ -575,21 +650,25 @@
         i.e., :math:`q(x,a):=\\mathbb{E}[r|x,a]`.
 
     """
     return _base_reward_function(
         context=context,
         action_context=action_context,
         degree=3,
+        coef_function=coef_function,
+        z_score=z_score,
         random_state=random_state,
     )
 
 
 def sparse_reward_function(
     context: np.ndarray,
     action_context: np.ndarray,
+    coef_function: coef_func_signature = sample_random_uniform_coefficients,
+    z_score: bool = True,
     random_state: Optional[int] = None,
 ) -> np.ndarray:
     """Sparse mean reward function for continuous rewards.
 
     Note
     ------
     Polynomial and interaction features will be used to calculate the expected rewards.
@@ -615,23 +694,27 @@
 
     """
     return _base_reward_function(
         context=context,
         action_context=action_context,
         degree=4,
         effective_dim_ratio=0.3,
+        coef_function=coef_function,
+        z_score=z_score,
         random_state=random_state,
     )
 
 
 def _base_reward_function(
     context: np.ndarray,
     action_context: np.ndarray,
     degree: int = 3,
     effective_dim_ratio: float = 1.0,
+    coef_function: coef_func_signature = sample_random_uniform_coefficients,
+    z_score: bool = True,
     random_state: Optional[int] = None,
 ) -> np.ndarray:
     """Base function to define mean reward functions.
 
     Note
     ------
     Given context :math:`x` and action_context :math:`a`, this function is used to define
@@ -674,14 +757,18 @@
 
     effective_dim_ratio: int, default=1.0
         Propotion of context dimensions relevant to the expected rewards.
         Specifically, after the polynomial feature transformation is applied to the original context vectors,
         only `dim_context * effective_dim_ratio` fraction of randomly selected dimensions
         will be used as relevant dimensions to generate expected rewards.
 
+    z_score: boolean, default=True
+        Boolean to enable/disable the calculation of a z-score over the resulting rewards. In case the environment
+        is stationary, this can be turned on. But when the
+
     random_state: int, default=None
         Controls the random seed in sampling dataset.
 
     Returns
     ---------
     expected_rewards: array-like, shape (n_rounds, n_actions)
         Expected reward given context (:math:`x`) and action (:math:`a`),
@@ -720,29 +807,53 @@
         ]
     else:
         effective_dim_context = dim_context
         effective_dim_action_context = dim_action_context
         effective_context_ = context_
         effective_action_context_ = action_context_
 
-    context_coef_ = random_.uniform(-1, 1, size=effective_dim_context)
-    action_coef_ = random_.uniform(-1, 1, size=effective_dim_action_context)
-    context_action_coef_ = random_.uniform(
-        -1, 1, size=(effective_dim_context, effective_dim_action_context)
+    context_coef_, action_coef_, context_action_coef_ = coef_function(
+        n_rounds=datasize,
+        effective_dim_action_context=effective_dim_action_context,
+        effective_dim_context=effective_dim_context,
+        random_=random_,
     )
 
-    context_values = np.tile(effective_context_ @ context_coef_, (n_actions, 1)).T
-    action_values = np.tile(action_coef_ @ effective_action_context_.T, (datasize, 1))
-    context_action_values = (
-        effective_context_ @ context_action_coef_ @ effective_action_context_.T
-    )
+    if context_coef_.shape[0] != datasize:
+        context_values = np.tile(effective_context_ @ context_coef_, (n_actions, 1)).T
+    else:
+        context_values = np.tile(
+            np.sum(effective_context_ * context_coef_, axis=1), (n_actions, 1)
+        ).T
+
+    action_values = action_coef_ @ effective_action_context_.T
+    if action_coef_.shape[0] != datasize:
+        action_values = np.tile(action_values, (datasize, 1))
+
+    if action_coef_.shape[0] != datasize:
+        context_action_values = (
+            effective_context_ @ context_action_coef_ @ effective_action_context_.T
+        )
+    else:
+        effective_context_ = np.expand_dims(effective_context_, axis=1)
+        context_action_coef_interactions = np.squeeze(
+            np.matmul(effective_context_, context_action_coef_), axis=1
+        )
+
+        context_action_values = (
+            context_action_coef_interactions @ effective_action_context_.T
+        )
+
     expected_rewards = context_values + action_values + context_action_values
-    expected_rewards = (
-        degree * (expected_rewards - expected_rewards.mean()) / expected_rewards.std()
-    )
+    if z_score:
+        expected_rewards = (
+            expected_rewards - expected_rewards.mean() / expected_rewards.std()
+        )
+
+    expected_rewards = degree * expected_rewards
 
     return expected_rewards
 
 
 def linear_behavior_policy(
     context: np.ndarray,
     action_context: np.ndarray,
```

### Comparing `obp-0.5.5/obp/dataset/synthetic_continuous.py` & `obp-0.5.6/obp/dataset/synthetic_continuous.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/synthetic_embed.py` & `obp-0.5.6/obp/dataset/synthetic_embed.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/dataset/synthetic_multi.py` & `obp-0.5.6/obp/dataset/synthetic_multi.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,19 @@
         sampled from the uniform distribution automatically.
 
     reward_std: float, default=1.0
         Standard deviation of the reward distribution.
         A larger value leads to a noisier reward distribution.
         This argument is valid only when `reward_type="continuous"`.
 
+    reward_noise_distribution: str, default='normal'
+        From which distribution we sample noise on the reward, must be either 'normal' or 'truncated_normal'.
+        If 'truncated_normal' is given, we do not have any negative reward realization in the logged dataset.
+        This argument is valid only when `reward_type="continuous"`.
+
     action_context: np.ndarray, default=None
          Vector representation of (discrete) actions.
          If None, one-hot representation will be used.
 
     n_deficient_actions: int, default=0
         Number of deficient actions having zero probability of being selected in the logged bandit data.
         If there are some deficient actions, the full/common support assumption is very likely to be violated,
@@ -268,20 +273,21 @@
             [np.ones(n_k) * self.betas[k] for k, n_k in enumerate(n_rounds_strata)]
         )[:, np.newaxis]
 
         # calc expected reward given context and action
         expected_reward_ = self.calc_expected_reward(contexts)
         if RewardType(self.reward_type) == RewardType.CONTINUOUS:
             # correct expected_reward_, as we use truncated normal distribution here
-            mean = expected_reward_
-            a = (self.reward_min - mean) / self.reward_std
-            b = (self.reward_max - mean) / self.reward_std
-            expected_reward_ = truncnorm.stats(
-                a=a, b=b, loc=mean, scale=self.reward_std, moments="m"
-            )
+            if self.reward_noise_distribution == "truncated_normal":
+                mean = expected_reward_
+                a = (self.reward_min - mean) / self.reward_std
+                b = (self.reward_max - mean) / self.reward_std
+                expected_reward_ = truncnorm.stats(
+                    a=a, b=b, loc=mean, scale=self.reward_std, moments="m"
+                )
 
         # calculate the action choice probabilities of the behavior policy
         pi_b_logits = expected_reward_
         # create some deficient actions based on the value of `n_deficient_actions`
         if self.n_deficient_actions > 0:
             pi_b = np.zeros_like(pi_b_logits)
             n_supported_actions = self.n_actions - self.n_deficient_actions
```

### Comparing `obp-0.5.5/obp/dataset/synthetic_slate.py` & `obp-0.5.6/obp/dataset/synthetic_slate.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/__init__.py` & `obp-0.5.6/obp/ope/__init__.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/classification_model.py` & `obp-0.5.6/obp/ope/classification_model.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/estimators.py` & `obp-0.5.6/obp/ope/estimators.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/estimators_continuous.py` & `obp-0.5.6/obp/ope/estimators_continuous.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/estimators_embed.py` & `obp-0.5.6/obp/ope/estimators_embed.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/estimators_multi.py` & `obp-0.5.6/obp/ope/estimators_multi.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/estimators_slate.py` & `obp-0.5.6/obp/ope/estimators_slate.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/estimators_tuning.py` & `obp-0.5.6/obp/ope/estimators_tuning.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/helper.py` & `obp-0.5.6/obp/ope/helper.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/meta.py` & `obp-0.5.6/obp/ope/meta.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/meta_continuous.py` & `obp-0.5.6/obp/ope/meta_continuous.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/meta_multi.py` & `obp-0.5.6/obp/ope/meta_multi.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/meta_slate.py` & `obp-0.5.6/obp/ope/meta_slate.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/regression_model.py` & `obp-0.5.6/obp/ope/regression_model.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/ope/regression_model_slate.py` & `obp-0.5.6/obp/ope/regression_model_slate.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/policy/__init__.py` & `obp-0.5.6/obp/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/policy/base.py` & `obp-0.5.6/obp/policy/base.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/policy/conf/prior_bts.yaml` & `obp-0.5.6/obp/policy/conf/prior_bts.yaml`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/policy/contextfree.py` & `obp-0.5.6/obp/policy/contextfree.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/policy/linear.py` & `obp-0.5.6/obp/policy/linear.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/policy/logistic.py` & `obp-0.5.6/obp/policy/logistic.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/policy/offline.py` & `obp-0.5.6/obp/policy/offline.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
             self.base_classifier = LogisticRegression(random_state=12345)
         else:
             if not is_classifier(self.base_classifier):
                 raise ValueError("`base_classifier` must be a classifier")
         self.base_classifier_list = [
             clone(self.base_classifier) for _ in np.arange(self.len_list)
         ]
+        self.policy_name = "IPWLearner"
 
     @staticmethod
     def _create_train_data_for_opl(
         context: np.ndarray,
         action: np.ndarray,
         reward: np.ndarray,
         pscore: np.ndarray,
```

### Comparing `obp-0.5.5/obp/policy/offline_continuous.py` & `obp-0.5.6/obp/policy/offline_continuous.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.5/obp/simulator/simulator.py` & `obp-0.5.6/obp/simulator/replay.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,37 @@
-# Copyright (c) Yuta Saito, Yusuke Narita, and ZOZO Technologies, Inc. All rights reserved.
-# Licensed under the Apache 2.0 License.
-
-"""Bandit Simulator."""
-from copy import deepcopy
-from typing import Callable
-from typing import Union
-
 import numpy as np
-from tqdm import tqdm
-
-from ..policy import BaseContextFreePolicy
-from ..policy import BaseContextualPolicy
-from ..policy.policy_type import PolicyType
-from ..types import BanditFeedback
-from ..utils import check_bandit_feedback_inputs
-from ..utils import convert_to_action_dist
+import tqdm as tqdm
 
+from obp.policy.policy_type import PolicyType
+from obp.simulator.simulator import BanditPolicy
+from obp.types import BanditFeedback
+from obp.utils import check_bandit_feedback_inputs
+from obp.utils import convert_to_action_dist
 
-# bandit policy type
-BanditPolicy = Union[BaseContextFreePolicy, BaseContextualPolicy]
 
-
-def run_bandit_simulation(
+def run_bandit_replay(
     bandit_feedback: BanditFeedback, policy: BanditPolicy
 ) -> np.ndarray:
-    """Run an online bandit algorithm on the given logged bandit feedback data.
+    """Run an online bandit algorithm on given logged bandit feedback data using the replay method.
 
     Parameters
     ----------
     bandit_feedback: BanditFeedback
         Logged bandit data used in offline bandit simulation.
-
     policy: BanditPolicy
         Online bandit policy to be evaluated in offline bandit simulation (i.e., evaluation policy).
-
     Returns
     --------
     action_dist: array-like, shape (n_rounds, n_actions, len_list)
         Action choice probabilities (can be deterministic).
 
+    References
+    ------------
+    Lihong Li, Wei Chu, John Langford, and Xuanhui Wang.
+    "Unbiased Offline Evaluation of Contextual-bandit-based News Article Recommendation Algorithms.", 2011.
     """
     for key_ in ["action", "position", "reward", "pscore", "context"]:
         if key_ not in bandit_feedback:
             raise RuntimeError(f"Missing key of {key_} in 'bandit_feedback'.")
     check_bandit_feedback_inputs(
         context=bandit_feedback["context"],
         action=bandit_feedback["action"],
@@ -88,90 +77,7 @@
         selected_actions_list.append(selected_actions)
 
     action_dist = convert_to_action_dist(
         n_actions=bandit_feedback["action"].max() + 1,
         selected_actions=np.array(selected_actions_list),
     )
     return action_dist
-
-
-def calc_ground_truth_policy_value(
-    bandit_feedback: BanditFeedback,
-    reward_sampler: Callable[[np.ndarray, np.ndarray], float],
-    policy: BanditPolicy,
-    n_sim: int = 100,
-) -> float:
-    """Calculate the ground-truth policy value of a given online bandit algorithm by Monte-Carlo Simulation.
-
-    Parameters
-    ----------
-    bandit_feedback: BanditFeedback
-        Logged bandit data used in offline bandit simulation. Must contain "expected_rewards" as a key.
-
-    reward_sampler: Callable[[np.ndarray, np.ndarray], np.ndarray]
-        Function sampling reward for each given action-context pair, i.e., :math:`p(r|x, a)`.
-
-    policy: BanditPolicy
-        Online bandit policy to be evaluated in offline bandit simulation (i.e., evaluation policy).
-
-    n_sim: int, default=100
-        Number of simulations in the Monte Carlo simulation to compute the policy value.
-
-    Returns
-    --------
-    ground_truth_policy_value: float
-        policy value of a given evaluation policy.
-
-    """
-    for key_ in [
-        "action",
-        "position",
-        "reward",
-        "expected_reward",
-        "context",
-    ]:
-        if key_ not in bandit_feedback:
-            raise RuntimeError(f"Missing key of {key_} in 'bandit_feedback'.")
-    check_bandit_feedback_inputs(
-        context=bandit_feedback["context"],
-        action=bandit_feedback["action"],
-        reward=bandit_feedback["reward"],
-        expected_reward=bandit_feedback["expected_reward"],
-        position=bandit_feedback["position"],
-    )
-
-    cumulative_reward = 0.0
-    dim_context = bandit_feedback["context"].shape[1]
-
-    for _ in tqdm(np.arange(n_sim), total=n_sim):
-        policy_ = deepcopy(policy)
-        for position_, context_, expected_reward_ in zip(
-            bandit_feedback["position"],
-            bandit_feedback["context"],
-            bandit_feedback["expected_reward"],
-        ):
-
-            # select a list of actions
-            if policy_.policy_type == PolicyType.CONTEXT_FREE:
-                selected_actions = policy_.select_action()
-            elif policy_.policy_type == PolicyType.CONTEXTUAL:
-                selected_actions = policy_.select_action(
-                    context_.reshape(1, dim_context)
-                )
-            action = selected_actions[position_]
-            # sample reward
-            reward = reward_sampler(
-                context_.reshape(1, dim_context), np.array([action])
-            )
-            cumulative_reward += expected_reward_[action]
-
-            # update parameters of a bandit policy
-            if policy_.policy_type == PolicyType.CONTEXT_FREE:
-                policy_.update_params(action=action, reward=reward)
-            elif policy_.policy_type == PolicyType.CONTEXTUAL:
-                policy_.update_params(
-                    action=action,
-                    reward=reward,
-                    context=context_.reshape(1, dim_context),
-                )
-
-    return cumulative_reward / (n_sim * bandit_feedback["n_rounds"])
```

### Comparing `obp-0.5.5/obp/utils.py` & `obp-0.5.6/obp/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     return sampled_action
 
 
 def convert_to_action_dist(
     n_actions: int,
     selected_actions: np.ndarray,
 ) -> np.ndarray:
-    """Convert selected actions (output of `run_bandit_simulation`) to distribution over actions.
+    """Convert selected actions (output of `run_bandit_replay`) to distribution over actions.
 
     Parameters
     ----------
     n_actions: int
         Number of actions.
 
     selected_actions: array-like, shape (n_rounds, len_list)
```

### Comparing `obp-0.5.5/obp.egg-info/PKG-INFO` & `obp-0.5.6/obp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obp
-Version: 0.5.5
+Version: 0.5.6
 Summary: Open Bandit Pipeline: a python library for bandit algorithms and off-policy evaluation
 Home-page: https://github.com/st-tech/zr-obp
 Author: Yuta Saito
 Author-email: open-bandit-project@googlegroups.com
 License: Apache License
 Description: <div align="center"><img src="https://raw.githubusercontent.com/st-tech/zr-obp/master/images/logo.png" width="60%"/></div>
         
@@ -83,15 +83,15 @@
         </p>
         </figcaption>
         
         Open Bandit Pipeline consists of the following main modules.
         
         - [**dataset module**](./obp/dataset/): This module provides a data loader for Open Bandit Dataset and a flexible interface for handling logged bandit data. It also provides tools to generate synthetic bandit data and transform multi-class classification data to bandit data.
         - [**policy module**](./obp/policy/): This module provides interfaces for implementing new online and offline bandit policies. It also implements several standard policy learning methods.
-        - [**simulator module**](./obp/simulator/): This module provides functions for conducting offline bandit simulation. This module is necessary only when you use the ReplayMethod to evaluate online bandit policies. Please refer to [examples/quickstart/online.ipynb](./examples/quickstart/online.ipynb) for a quickstart guide of implementing OPE of online bandit algorithms.
+        - [**simulator module**](./obp/simulator/): This module provides functions for conducting offline bandit simulation. This module is necessary only when you use the ReplayMethod to evaluate online bandit policies. Please refer to [examples/quickstart/online.ipynb](./examples/quickstart/replay.ipynb) for a quickstart guide of implementing OPE of online bandit algorithms.
         - [**ope module**](./obp/ope/): This module provides generic abstract interfaces to support custom implementations so that researchers can evaluate their own estimators easily. It also implements several basic and advanced OPE estimators.
         
         ### Supported Bandit Algorithms and OPE Estimators
         
         <details>
         <summary><strong>Bandit Algorithms </strong>(click to expand)</summary>
         <br>
@@ -436,17 +436,17 @@
         [[github](https://github.com/snap-stanford/ogb)] [[project page](https://ogb.stanford.edu)] [[paper](https://arxiv.org/abs/2005.00687)].
         
         </details>
         
 Keywords: bandit algorithms,off-policy evaluation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `obp-0.5.5/obp.egg-info/SOURCES.txt` & `obp-0.5.6/obp.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -58,8 +58,11 @@
 obp/policy/linear.py
 obp/policy/logistic.py
 obp/policy/offline.py
 obp/policy/offline_continuous.py
 obp/policy/policy_type.py
 obp/policy/conf/prior_bts.yaml
 obp/simulator/__init__.py
+obp/simulator/coefficient_drifter.py
+obp/simulator/delay_sampler.py
+obp/simulator/replay.py
 obp/simulator/simulator.py
```

### Comparing `obp-0.5.5/setup.py` & `obp-0.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,36 +23,36 @@
     author_email="open-bandit-project@googlegroups.com",
     keywords=["bandit algorithms", "off-policy evaluation"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "matplotlib>=3.4.3",
         "mypy-extensions>=0.4.3",
-        "numpy>=1.21.2",
-        "pandas>=1.3.2",
-        "pyyaml>=5.1",
+        "numpy>=1.23.5",
+        "pandas>=1.5.2",
+        "pyyaml>=6.0",
         "seaborn>=0.10.1",
-        "scikit-learn>=1.0.2",
-        "scipy>=1.7.3",
-        "torch>=1.9.0",
+        "scikit-learn>=1.1.3",
+        "scipy>=1.9.3",
+        "torch>=1.12",
         "tqdm>=4.62.2",
         "pyieoe>=0.1.1",
         "pingouin>=0.4.0",
     ],
     license="Apache License",
     packages=find_packages(
         exclude=["benchmark", "docs", "examples", "obd", "tests", "slides"]
     ),
     package_data={"obp": package_data_list},
     include_package_data=True,
     classifiers=[
         "Intended Audience :: Science/Research",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: Apache Software License",
```

