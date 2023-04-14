# Comparing `tmp/obp-0.5.6.tar.gz` & `tmp/obp-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obp-0.5.6.tar", last modified: Fri Apr 14 20:39:12 2023, max compression
+gzip compressed data, was "obp-0.5.7.tar", last modified: Fri Apr 14 21:04:41 2023, max compression
```

## Comparing `obp-0.5.6.tar` & `obp-0.5.7.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.739784 obp-0.5.6/
--rw-r--r--   0 usaito     (501) staff       (20)     1197 2021-03-20 12:31:29.000000 obp-0.5.6/CONTRIBUTING.md
--rw-r--r--   0 usaito     (501) staff       (20)    11384 2020-08-18 02:58:21.000000 obp-0.5.6/LICENSE
--rw-r--r--   0 usaito     (501) staff       (20)      115 2021-02-07 14:46:04.000000 obp-0.5.6/MANIFEST.in
--rw-r--r--   0 usaito     (501) staff       (20)    30824 2023-04-14 20:39:12.740051 obp-0.5.6/PKG-INFO
--rw-r--r--   0 usaito     (501) staff       (20)    26372 2022-11-13 12:29:47.000000 obp-0.5.6/README.md
--rw-r--r--   0 usaito     (501) staff       (20)    27676 2022-06-15 06:09:06.000000 obp-0.5.6/README_JN.md
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.690186 obp-0.5.6/obp/
--rw-r--r--   0 usaito     (501) staff       (20)      264 2021-11-11 07:03:01.000000 obp-0.5.6/obp/__init__.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.693219 obp-0.5.6/obp/dataset/
--rw-r--r--   0 usaito     (501) staff       (20)     2600 2022-04-03 21:53:03.000000 obp-0.5.6/obp/dataset/__init__.py
--rw-r--r--   0 usaito     (501) staff       (20)      848 2022-01-12 23:12:35.000000 obp-0.5.6/obp/dataset/base.py
--rw-r--r--   0 usaito     (501) staff       (20)    14801 2022-01-12 23:12:35.000000 obp-0.5.6/obp/dataset/multiclass.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.687338 obp-0.5.6/obp/dataset/obd/
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.687264 obp-0.5.6/obp/dataset/obd/bts/
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.698280 obp-0.5.6/obp/dataset/obd/bts/all/
--rw-r--r--   0 usaito     (501) staff       (20)  5084456 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/all/all.csv
--rw-r--r--   0 usaito     (501) staff       (20)    10041 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/all/item_context.csv
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.698828 obp-0.5.6/obp/dataset/obd/bts/men/
--rw-r--r--   0 usaito     (501) staff       (20)     4287 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/men/item_context.csv
--rw-r--r--   0 usaito     (501) staff       (20)  3240432 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/men/men.csv
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.704648 obp-0.5.6/obp/dataset/obd/bts/women/
--rw-r--r--   0 usaito     (501) staff       (20)     5792 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/women/item_context.csv
--rw-r--r--   0 usaito     (501) staff       (20)  3722697 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/bts/women/women.csv
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.687542 obp-0.5.6/obp/dataset/obd/random/
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.715574 obp-0.5.6/obp/dataset/obd/random/all/
--rw-r--r--   0 usaito     (501) staff       (20)  5039451 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/all/all.csv
--rw-r--r--   0 usaito     (501) staff       (20)    10041 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/all/item_context.csv
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.720272 obp-0.5.6/obp/dataset/obd/random/men/
--rw-r--r--   0 usaito     (501) staff       (20)     4287 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/men/item_context.csv
--rw-r--r--   0 usaito     (501) staff       (20)  3336811 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/men/men.csv
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.724654 obp-0.5.6/obp/dataset/obd/random/women/
--rw-r--r--   0 usaito     (501) staff       (20)     5792 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/women/item_context.csv
--rw-r--r--   0 usaito     (501) staff       (20)  3817771 2021-02-07 14:46:04.000000 obp-0.5.6/obp/dataset/obd/random/women/women.csv
--rw-r--r--   0 usaito     (501) staff       (20)    13843 2022-01-12 23:12:35.000000 obp-0.5.6/obp/dataset/real.py
--rw-r--r--   0 usaito     (501) staff       (20)      315 2021-03-20 12:31:29.000000 obp-0.5.6/obp/dataset/reward_type.py
--rw-r--r--   0 usaito     (501) staff       (20)    38494 2023-04-14 20:08:50.000000 obp-0.5.6/obp/dataset/synthetic.py
--rw-r--r--   0 usaito     (501) staff       (20)    15792 2022-01-13 02:38:38.000000 obp-0.5.6/obp/dataset/synthetic_continuous.py
--rw-r--r--   0 usaito     (501) staff       (20)    15417 2022-06-15 05:22:45.000000 obp-0.5.6/obp/dataset/synthetic_embed.py
--rw-r--r--   0 usaito     (501) staff       (20)    14953 2022-11-13 22:21:58.000000 obp-0.5.6/obp/dataset/synthetic_multi.py
--rw-r--r--   0 usaito     (501) staff       (20)    70424 2022-06-15 05:22:45.000000 obp-0.5.6/obp/dataset/synthetic_slate.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.735956 obp-0.5.6/obp/ope/
--rw-r--r--   0 usaito     (501) staff       (20)     5790 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/__init__.py
--rw-r--r--   0 usaito     (501) staff       (20)    27138 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/classification_model.py
--rw-r--r--   0 usaito     (501) staff       (20)    99758 2022-06-15 05:22:45.000000 obp-0.5.6/obp/ope/estimators.py
--rw-r--r--   0 usaito     (501) staff       (20)    29201 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/estimators_continuous.py
--rw-r--r--   0 usaito     (501) staff       (20)    30094 2022-06-15 05:22:45.000000 obp-0.5.6/obp/ope/estimators_embed.py
--rw-r--r--   0 usaito     (501) staff       (20)    78206 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/estimators_multi.py
--rw-r--r--   0 usaito     (501) staff       (20)    43716 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/estimators_slate.py
--rw-r--r--   0 usaito     (501) staff       (20)    69301 2022-06-15 05:22:45.000000 obp-0.5.6/obp/ope/estimators_tuning.py
--rw-r--r--   0 usaito     (501) staff       (20)     7990 2022-06-15 05:22:45.000000 obp-0.5.6/obp/ope/helper.py
--rw-r--r--   0 usaito     (501) staff       (20)    49157 2022-06-15 05:22:45.000000 obp-0.5.6/obp/ope/meta.py
--rw-r--r--   0 usaito     (501) staff       (20)    28563 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/meta_continuous.py
--rw-r--r--   0 usaito     (501) staff       (20)    37003 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/meta_multi.py
--rw-r--r--   0 usaito     (501) staff       (20)    31117 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/meta_slate.py
--rw-r--r--   0 usaito     (501) staff       (20)    15050 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/regression_model.py
--rw-r--r--   0 usaito     (501) staff       (20)    16919 2022-04-03 21:53:03.000000 obp-0.5.6/obp/ope/regression_model_slate.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.738584 obp-0.5.6/obp/policy/
--rw-r--r--   0 usaito     (501) staff       (20)     1314 2021-11-11 07:03:01.000000 obp-0.5.6/obp/policy/__init__.py
--rw-r--r--   0 usaito     (501) staff       (20)     7220 2022-04-03 21:53:03.000000 obp-0.5.6/obp/policy/base.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.738874 obp-0.5.6/obp/policy/conf/
--rw-r--r--   0 usaito     (501) staff       (20)     3968 2020-10-22 21:40:34.000000 obp-0.5.6/obp/policy/conf/prior_bts.yaml
--rw-r--r--   0 usaito     (501) staff       (20)     8481 2022-01-12 23:12:35.000000 obp-0.5.6/obp/policy/contextfree.py
--rw-r--r--   0 usaito     (501) staff       (20)     9270 2022-01-12 23:12:35.000000 obp-0.5.6/obp/policy/linear.py
--rw-r--r--   0 usaito     (501) staff       (20)    10980 2022-04-03 21:53:03.000000 obp-0.5.6/obp/policy/logistic.py
--rw-r--r--   0 usaito     (501) staff       (20)    73129 2022-11-13 12:29:47.000000 obp-0.5.6/obp/policy/offline.py
--rw-r--r--   0 usaito     (501) staff       (20)    40844 2022-04-03 22:56:53.000000 obp-0.5.6/obp/policy/offline_continuous.py
--rw-r--r--   0 usaito     (501) staff       (20)      409 2021-03-20 12:31:29.000000 obp-0.5.6/obp/policy/policy_type.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.739646 obp-0.5.6/obp/simulator/
--rw-r--r--   0 usaito     (501) staff       (20)      121 2022-11-13 12:29:47.000000 obp-0.5.6/obp/simulator/__init__.py
--rw-r--r--   0 usaito     (501) staff       (20)     9161 2022-11-13 22:54:57.000000 obp-0.5.6/obp/simulator/coefficient_drifter.py
--rw-r--r--   0 usaito     (501) staff       (20)     3804 2022-11-13 12:29:47.000000 obp-0.5.6/obp/simulator/delay_sampler.py
--rw-r--r--   0 usaito     (501) staff       (20)     3226 2022-11-13 22:54:57.000000 obp-0.5.6/obp/simulator/replay.py
--rwxr-xr-x   0 usaito     (501) staff       (20)    18637 2022-11-13 22:54:57.000000 obp-0.5.6/obp/simulator/simulator.py
--rw-r--r--   0 usaito     (501) staff       (20)      279 2021-11-11 07:03:01.000000 obp-0.5.6/obp/types.py
--rwxr-xr-x   0 usaito     (501) staff       (20)    37118 2022-11-13 12:29:47.000000 obp-0.5.6/obp/utils.py
--rw-r--r--   0 usaito     (501) staff       (20)       22 2023-04-14 20:11:06.000000 obp-0.5.6/obp/version.py
-drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 20:39:12.690801 obp-0.5.6/obp.egg-info/
--rw-r--r--   0 usaito     (501) staff       (20)    30824 2023-04-14 20:39:12.000000 obp-0.5.6/obp.egg-info/PKG-INFO
--rw-r--r--   0 usaito     (501) staff       (20)     1778 2023-04-14 20:39:12.000000 obp-0.5.6/obp.egg-info/SOURCES.txt
--rw-r--r--   0 usaito     (501) staff       (20)        1 2023-04-14 20:39:12.000000 obp-0.5.6/obp.egg-info/dependency_links.txt
--rw-r--r--   0 usaito     (501) staff       (20)      185 2023-04-14 20:39:12.000000 obp-0.5.6/obp.egg-info/requires.txt
--rw-r--r--   0 usaito     (501) staff       (20)        4 2023-04-14 20:39:12.000000 obp-0.5.6/obp.egg-info/top_level.txt
--rw-r--r--   0 usaito     (501) staff       (20)      971 2023-04-14 20:10:55.000000 obp-0.5.6/pyproject.toml
--rw-r--r--   0 usaito     (501) staff       (20)      101 2023-04-14 20:39:12.740390 obp-0.5.6/setup.cfg
--rw-r--r--   0 usaito     (501) staff       (20)     2029 2023-04-14 20:14:27.000000 obp-0.5.6/setup.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.788559 obp-0.5.7/
+-rw-r--r--   0 usaito     (501) staff       (20)     1197 2021-03-20 12:31:29.000000 obp-0.5.7/CONTRIBUTING.md
+-rw-r--r--   0 usaito     (501) staff       (20)    11384 2020-08-18 02:58:21.000000 obp-0.5.7/LICENSE
+-rw-r--r--   0 usaito     (501) staff       (20)      115 2021-02-07 14:46:04.000000 obp-0.5.7/MANIFEST.in
+-rw-r--r--   0 usaito     (501) staff       (20)    30824 2023-04-14 21:04:41.788799 obp-0.5.7/PKG-INFO
+-rw-r--r--   0 usaito     (501) staff       (20)    26372 2022-11-13 12:29:47.000000 obp-0.5.7/README.md
+-rw-r--r--   0 usaito     (501) staff       (20)    27676 2022-06-15 06:09:06.000000 obp-0.5.7/README_JN.md
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.768355 obp-0.5.7/obp/
+-rw-r--r--   0 usaito     (501) staff       (20)      264 2021-11-11 07:03:01.000000 obp-0.5.7/obp/__init__.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.770095 obp-0.5.7/obp/dataset/
+-rw-r--r--   0 usaito     (501) staff       (20)     2600 2022-04-03 21:53:03.000000 obp-0.5.7/obp/dataset/__init__.py
+-rw-r--r--   0 usaito     (501) staff       (20)      848 2022-01-12 23:12:35.000000 obp-0.5.7/obp/dataset/base.py
+-rw-r--r--   0 usaito     (501) staff       (20)    14801 2022-01-12 23:12:35.000000 obp-0.5.7/obp/dataset/multiclass.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.766436 obp-0.5.7/obp/dataset/obd/
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.766372 obp-0.5.7/obp/dataset/obd/bts/
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.773108 obp-0.5.7/obp/dataset/obd/bts/all/
+-rw-r--r--   0 usaito     (501) staff       (20)  5084456 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/bts/all/all.csv
+-rw-r--r--   0 usaito     (501) staff       (20)    10041 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/bts/all/item_context.csv
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.773349 obp-0.5.7/obp/dataset/obd/bts/men/
+-rw-r--r--   0 usaito     (501) staff       (20)     4287 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/bts/men/item_context.csv
+-rw-r--r--   0 usaito     (501) staff       (20)  3240432 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/bts/men/men.csv
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.775272 obp-0.5.7/obp/dataset/obd/bts/women/
+-rw-r--r--   0 usaito     (501) staff       (20)     5792 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/bts/women/item_context.csv
+-rw-r--r--   0 usaito     (501) staff       (20)  3722697 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/bts/women/women.csv
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.766597 obp-0.5.7/obp/dataset/obd/random/
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.780484 obp-0.5.7/obp/dataset/obd/random/all/
+-rw-r--r--   0 usaito     (501) staff       (20)  5039451 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/random/all/all.csv
+-rw-r--r--   0 usaito     (501) staff       (20)    10041 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/random/all/item_context.csv
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.780737 obp-0.5.7/obp/dataset/obd/random/men/
+-rw-r--r--   0 usaito     (501) staff       (20)     4287 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/random/men/item_context.csv
+-rw-r--r--   0 usaito     (501) staff       (20)  3336811 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/random/men/men.csv
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.782674 obp-0.5.7/obp/dataset/obd/random/women/
+-rw-r--r--   0 usaito     (501) staff       (20)     5792 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/random/women/item_context.csv
+-rw-r--r--   0 usaito     (501) staff       (20)  3817771 2021-02-07 14:46:04.000000 obp-0.5.7/obp/dataset/obd/random/women/women.csv
+-rw-r--r--   0 usaito     (501) staff       (20)    13843 2022-01-12 23:12:35.000000 obp-0.5.7/obp/dataset/real.py
+-rw-r--r--   0 usaito     (501) staff       (20)      315 2021-03-20 12:31:29.000000 obp-0.5.7/obp/dataset/reward_type.py
+-rw-r--r--   0 usaito     (501) staff       (20)    38494 2023-04-14 20:08:50.000000 obp-0.5.7/obp/dataset/synthetic.py
+-rw-r--r--   0 usaito     (501) staff       (20)    15792 2022-01-13 02:38:38.000000 obp-0.5.7/obp/dataset/synthetic_continuous.py
+-rw-r--r--   0 usaito     (501) staff       (20)    15417 2022-06-15 05:22:45.000000 obp-0.5.7/obp/dataset/synthetic_embed.py
+-rw-r--r--   0 usaito     (501) staff       (20)    14953 2022-11-13 22:21:58.000000 obp-0.5.7/obp/dataset/synthetic_multi.py
+-rw-r--r--   0 usaito     (501) staff       (20)    70424 2022-06-15 05:22:45.000000 obp-0.5.7/obp/dataset/synthetic_slate.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.786671 obp-0.5.7/obp/ope/
+-rw-r--r--   0 usaito     (501) staff       (20)     5790 2022-04-03 21:53:03.000000 obp-0.5.7/obp/ope/__init__.py
+-rw-r--r--   0 usaito     (501) staff       (20)    27138 2022-04-03 21:53:03.000000 obp-0.5.7/obp/ope/classification_model.py
+-rw-r--r--   0 usaito     (501) staff       (20)    99758 2022-06-15 05:22:45.000000 obp-0.5.7/obp/ope/estimators.py
+-rw-r--r--   0 usaito     (501) staff       (20)    29201 2022-04-03 21:53:03.000000 obp-0.5.7/obp/ope/estimators_continuous.py
+-rw-r--r--   0 usaito     (501) staff       (20)    30067 2023-04-14 20:55:12.000000 obp-0.5.7/obp/ope/estimators_embed.py
+-rw-r--r--   0 usaito     (501) staff       (20)    78206 2022-04-03 21:53:03.000000 obp-0.5.7/obp/ope/estimators_multi.py
+-rw-r--r--   0 usaito     (501) staff       (20)    43716 2022-04-03 21:53:03.000000 obp-0.5.7/obp/ope/estimators_slate.py
+-rw-r--r--   0 usaito     (501) staff       (20)    69301 2022-06-15 05:22:45.000000 obp-0.5.7/obp/ope/estimators_tuning.py
+-rw-r--r--   0 usaito     (501) staff       (20)     7990 2022-06-15 05:22:45.000000 obp-0.5.7/obp/ope/helper.py
+-rw-r--r--   0 usaito     (501) staff       (20)    49157 2022-06-15 05:22:45.000000 obp-0.5.7/obp/ope/meta.py
+-rw-r--r--   0 usaito     (501) staff       (20)    28563 2022-04-03 21:53:03.000000 obp-0.5.7/obp/ope/meta_continuous.py
+-rw-r--r--   0 usaito     (501) staff       (20)    37003 2022-04-03 21:53:03.000000 obp-0.5.7/obp/ope/meta_multi.py
+-rw-r--r--   0 usaito     (501) staff       (20)    31117 2022-04-03 21:53:03.000000 obp-0.5.7/obp/ope/meta_slate.py
+-rw-r--r--   0 usaito     (501) staff       (20)    15050 2022-04-03 21:53:03.000000 obp-0.5.7/obp/ope/regression_model.py
+-rw-r--r--   0 usaito     (501) staff       (20)    16919 2022-04-03 21:53:03.000000 obp-0.5.7/obp/ope/regression_model_slate.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.787692 obp-0.5.7/obp/policy/
+-rw-r--r--   0 usaito     (501) staff       (20)     1314 2021-11-11 07:03:01.000000 obp-0.5.7/obp/policy/__init__.py
+-rw-r--r--   0 usaito     (501) staff       (20)     7220 2022-04-03 21:53:03.000000 obp-0.5.7/obp/policy/base.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.787811 obp-0.5.7/obp/policy/conf/
+-rw-r--r--   0 usaito     (501) staff       (20)     3968 2020-10-22 21:40:34.000000 obp-0.5.7/obp/policy/conf/prior_bts.yaml
+-rw-r--r--   0 usaito     (501) staff       (20)     8481 2022-01-12 23:12:35.000000 obp-0.5.7/obp/policy/contextfree.py
+-rw-r--r--   0 usaito     (501) staff       (20)     9270 2022-01-12 23:12:35.000000 obp-0.5.7/obp/policy/linear.py
+-rw-r--r--   0 usaito     (501) staff       (20)    10980 2022-04-03 21:53:03.000000 obp-0.5.7/obp/policy/logistic.py
+-rw-r--r--   0 usaito     (501) staff       (20)    73129 2022-11-13 12:29:47.000000 obp-0.5.7/obp/policy/offline.py
+-rw-r--r--   0 usaito     (501) staff       (20)    40844 2022-04-03 22:56:53.000000 obp-0.5.7/obp/policy/offline_continuous.py
+-rw-r--r--   0 usaito     (501) staff       (20)      409 2021-03-20 12:31:29.000000 obp-0.5.7/obp/policy/policy_type.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.788408 obp-0.5.7/obp/simulator/
+-rw-r--r--   0 usaito     (501) staff       (20)      121 2022-11-13 12:29:47.000000 obp-0.5.7/obp/simulator/__init__.py
+-rw-r--r--   0 usaito     (501) staff       (20)     9161 2022-11-13 22:54:57.000000 obp-0.5.7/obp/simulator/coefficient_drifter.py
+-rw-r--r--   0 usaito     (501) staff       (20)     3804 2022-11-13 12:29:47.000000 obp-0.5.7/obp/simulator/delay_sampler.py
+-rw-r--r--   0 usaito     (501) staff       (20)     3226 2022-11-13 22:54:57.000000 obp-0.5.7/obp/simulator/replay.py
+-rwxr-xr-x   0 usaito     (501) staff       (20)    18637 2022-11-13 22:54:57.000000 obp-0.5.7/obp/simulator/simulator.py
+-rw-r--r--   0 usaito     (501) staff       (20)      279 2021-11-11 07:03:01.000000 obp-0.5.7/obp/types.py
+-rwxr-xr-x   0 usaito     (501) staff       (20)    37118 2022-11-13 12:29:47.000000 obp-0.5.7/obp/utils.py
+-rw-r--r--   0 usaito     (501) staff       (20)       22 2023-04-14 20:53:37.000000 obp-0.5.7/obp/version.py
+drwxr-xr-x   0 usaito     (501) staff       (20)        0 2023-04-14 21:04:41.768950 obp-0.5.7/obp.egg-info/
+-rw-r--r--   0 usaito     (501) staff       (20)    30824 2023-04-14 21:04:41.000000 obp-0.5.7/obp.egg-info/PKG-INFO
+-rw-r--r--   0 usaito     (501) staff       (20)     1778 2023-04-14 21:04:41.000000 obp-0.5.7/obp.egg-info/SOURCES.txt
+-rw-r--r--   0 usaito     (501) staff       (20)        1 2023-04-14 21:04:41.000000 obp-0.5.7/obp.egg-info/dependency_links.txt
+-rw-r--r--   0 usaito     (501) staff       (20)      185 2023-04-14 21:04:41.000000 obp-0.5.7/obp.egg-info/requires.txt
+-rw-r--r--   0 usaito     (501) staff       (20)        4 2023-04-14 21:04:41.000000 obp-0.5.7/obp.egg-info/top_level.txt
+-rw-r--r--   0 usaito     (501) staff       (20)      971 2023-04-14 20:53:29.000000 obp-0.5.7/pyproject.toml
+-rw-r--r--   0 usaito     (501) staff       (20)      101 2023-04-14 21:04:41.789095 obp-0.5.7/setup.cfg
+-rw-r--r--   0 usaito     (501) staff       (20)     2029 2023-04-14 20:14:27.000000 obp-0.5.7/setup.py
```

### Comparing `obp-0.5.6/CONTRIBUTING.md` & `obp-0.5.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/LICENSE` & `obp-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/PKG-INFO` & `obp-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obp
-Version: 0.5.6
+Version: 0.5.7
 Summary: Open Bandit Pipeline: a python library for bandit algorithms and off-policy evaluation
 Home-page: https://github.com/st-tech/zr-obp
 Author: Yuta Saito
 Author-email: open-bandit-project@googlegroups.com
 License: Apache License
 Description: <div align="center"><img src="https://raw.githubusercontent.com/st-tech/zr-obp/master/images/logo.png" width="60%"/></div>
```

### Comparing `obp-0.5.6/README.md` & `obp-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/README_JN.md` & `obp-0.5.7/README_JN.md`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/__init__.py` & `obp-0.5.7/obp/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/base.py` & `obp-0.5.7/obp/dataset/base.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/multiclass.py` & `obp-0.5.7/obp/dataset/multiclass.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/bts/all/all.csv` & `obp-0.5.7/obp/dataset/obd/bts/all/all.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/bts/all/item_context.csv` & `obp-0.5.7/obp/dataset/obd/bts/all/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/bts/men/item_context.csv` & `obp-0.5.7/obp/dataset/obd/bts/men/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/bts/men/men.csv` & `obp-0.5.7/obp/dataset/obd/bts/men/men.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/bts/women/item_context.csv` & `obp-0.5.7/obp/dataset/obd/bts/women/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/bts/women/women.csv` & `obp-0.5.7/obp/dataset/obd/bts/women/women.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/random/all/all.csv` & `obp-0.5.7/obp/dataset/obd/random/all/all.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/random/all/item_context.csv` & `obp-0.5.7/obp/dataset/obd/random/all/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/random/men/item_context.csv` & `obp-0.5.7/obp/dataset/obd/random/men/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/random/men/men.csv` & `obp-0.5.7/obp/dataset/obd/random/men/men.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/random/women/item_context.csv` & `obp-0.5.7/obp/dataset/obd/random/women/item_context.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/obd/random/women/women.csv` & `obp-0.5.7/obp/dataset/obd/random/women/women.csv`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/real.py` & `obp-0.5.7/obp/dataset/real.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/synthetic.py` & `obp-0.5.7/obp/dataset/synthetic.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/synthetic_continuous.py` & `obp-0.5.7/obp/dataset/synthetic_continuous.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/synthetic_embed.py` & `obp-0.5.7/obp/dataset/synthetic_embed.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/synthetic_multi.py` & `obp-0.5.7/obp/dataset/synthetic_multi.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/dataset/synthetic_slate.py` & `obp-0.5.7/obp/dataset/synthetic_slate.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/__init__.py` & `obp-0.5.7/obp/ope/__init__.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/classification_model.py` & `obp-0.5.7/obp/ope/classification_model.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/estimators.py` & `obp-0.5.7/obp/ope/estimators.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/estimators_continuous.py` & `obp-0.5.7/obp/ope/estimators_continuous.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/estimators_embed.py` & `obp-0.5.7/obp/ope/estimators_embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,21 +159,21 @@
         ----------
         estimated_rewards: array-like, shape (n_rounds,)
             Estimated rewards for each observation.
 
         """
         n = reward.shape[0]
         if p_e_a is not None:
-            p_e_pi_b = np.ones(n)
-            p_e_pi_e = np.ones(n)
-            for d in np.arange(p_e_a.shape[-1]):
-                p_e_pi_b_d = pi_b[np.arange(n), :, position] @ p_e_a[:, :, d]
-                p_e_pi_b *= p_e_pi_b_d[np.arange(n), action_embed[:, d]]
-                p_e_pi_e_d = action_dist[np.arange(n), :, position] @ p_e_a[:, :, d]
-                p_e_pi_e *= p_e_pi_e_d[np.arange(n), action_embed[:, d]]
+            pi_b = pi_b[np.arange(n), :, position]
+            pi_e = action_dist[np.arange(n), :, position]
+            embed_dim = p_e_a.shape[-1]
+            p_e_pi_b, p_e_pi_e = np.ones(n), np.ones(n)
+            p_e_a_full_dim = p_e_a[:, action_embed, np.arange(embed_dim)].prod(2)
+            p_e_pi_b = (pi_b * p_e_a_full_dim.T).sum(1)
+            p_e_pi_e = (pi_e * p_e_a_full_dim.T).sum(1)
             w_x_e = p_e_pi_e / p_e_pi_b
             self.max_w_x_e = w_x_e.max()
 
         else:
             w_x_e = self._estimate_w_x_e(
                 context=context,
                 action=action,
```

### Comparing `obp-0.5.6/obp/ope/estimators_multi.py` & `obp-0.5.7/obp/ope/estimators_multi.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/estimators_slate.py` & `obp-0.5.7/obp/ope/estimators_slate.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/estimators_tuning.py` & `obp-0.5.7/obp/ope/estimators_tuning.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/helper.py` & `obp-0.5.7/obp/ope/helper.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/meta.py` & `obp-0.5.7/obp/ope/meta.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/meta_continuous.py` & `obp-0.5.7/obp/ope/meta_continuous.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/meta_multi.py` & `obp-0.5.7/obp/ope/meta_multi.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/meta_slate.py` & `obp-0.5.7/obp/ope/meta_slate.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/regression_model.py` & `obp-0.5.7/obp/ope/regression_model.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/ope/regression_model_slate.py` & `obp-0.5.7/obp/ope/regression_model_slate.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/policy/__init__.py` & `obp-0.5.7/obp/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/policy/base.py` & `obp-0.5.7/obp/policy/base.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/policy/conf/prior_bts.yaml` & `obp-0.5.7/obp/policy/conf/prior_bts.yaml`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/policy/contextfree.py` & `obp-0.5.7/obp/policy/contextfree.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/policy/linear.py` & `obp-0.5.7/obp/policy/linear.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/policy/logistic.py` & `obp-0.5.7/obp/policy/logistic.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/policy/offline.py` & `obp-0.5.7/obp/policy/offline.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/policy/offline_continuous.py` & `obp-0.5.7/obp/policy/offline_continuous.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/simulator/coefficient_drifter.py` & `obp-0.5.7/obp/simulator/coefficient_drifter.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/simulator/delay_sampler.py` & `obp-0.5.7/obp/simulator/delay_sampler.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/simulator/replay.py` & `obp-0.5.7/obp/simulator/replay.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/simulator/simulator.py` & `obp-0.5.7/obp/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp/utils.py` & `obp-0.5.7/obp/utils.py`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/obp.egg-info/PKG-INFO` & `obp-0.5.7/obp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obp
-Version: 0.5.6
+Version: 0.5.7
 Summary: Open Bandit Pipeline: a python library for bandit algorithms and off-policy evaluation
 Home-page: https://github.com/st-tech/zr-obp
 Author: Yuta Saito
 Author-email: open-bandit-project@googlegroups.com
 License: Apache License
 Description: <div align="center"><img src="https://raw.githubusercontent.com/st-tech/zr-obp/master/images/logo.png" width="60%"/></div>
```

### Comparing `obp-0.5.6/obp.egg-info/SOURCES.txt` & `obp-0.5.7/obp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obp-0.5.6/pyproject.toml` & `obp-0.5.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "obp"
-version = "0.5.5"
+version = "0.5.7"
 description = "Open Bandit Pipeline: a python library for off-policy evaluation and learning"
 authors = ["Yuta Saito <ys552@cornell.edu>"]
 license = "Apache License 2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 torch = "1.12"
```

### Comparing `obp-0.5.6/setup.py` & `obp-0.5.7/setup.py`

 * *Files identical despite different names*

