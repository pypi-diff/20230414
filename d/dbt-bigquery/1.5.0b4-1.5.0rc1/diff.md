# Comparing `tmp/dbt-bigquery-1.5.0b4.tar.gz` & `tmp/dbt-bigquery-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-bigquery-1.5.0b4.tar", last modified: Thu Mar 30 20:54:38 2023, max compression
+gzip compressed data, was "dbt-bigquery-1.5.0rc1.tar", last modified: Fri Apr 14 01:38:45 2023, max compression
```

## Comparing `dbt-bigquery-1.5.0b4.tar` & `dbt-bigquery-1.5.0rc1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.143872 dbt-bigquery-1.5.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-03-30 20:54:38.143872 dbt-bigquery-1.5.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.135872 dbt-bigquery-1.5.0b4/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.135872 dbt-bigquery-1.5.0b4/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.135872 dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    25902 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.135872 dbt-bigquery-1.5.0b4/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.135872 dbt-bigquery-1.5.0b4/dbt/include/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.135872 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.139872 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/etc.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.139872 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/copy.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.139872 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.139872 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.139872 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/dbt/include/bigquery/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:54:38.143872 dbt-bigquery-1.5.0b4/dbt_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-03-30 20:54:38.000000 dbt-bigquery-1.5.0b4/dbt_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-30 20:54:38.000000 dbt-bigquery-1.5.0b4/dbt_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:54:38.000000 dbt-bigquery-1.5.0b4/dbt_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:54:38.000000 dbt-bigquery-1.5.0b4/dbt_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-30 20:54:38.000000 dbt-bigquery-1.5.0b4/dbt_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-30 20:54:38.000000 dbt-bigquery-1.5.0b4/dbt_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 20:54:38.143872 dbt-bigquery-1.5.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-03-30 20:54:25.000000 dbt-bigquery-1.5.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.434298 dbt-bigquery-1.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-14 01:38:45.434298 dbt-bigquery-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25902 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36364 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.426298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.430298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/etc.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.430298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/copy.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.430298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.430298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.430298 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/dbt/include/bigquery/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:38:45.434298 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 01:38:45.000000 dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:38:45.434298 dbt-bigquery-1.5.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-14 01:38:35.000000 dbt-bigquery-1.5.0rc1/setup.py
```

### Comparing `dbt-bigquery-1.5.0b4/LICENSE.md` & `dbt-bigquery-1.5.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/PKG-INFO` & `dbt-bigquery-1.5.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.5.0b4
+Version: 1.5.0rc1
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.5.0b4 Summary: The Bigquery
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
-text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.5.0rc1 Summary: The
+Bigquery adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+bigquery Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-bigquery The `dbt-bigquery` package contains all of
```

### Comparing `dbt-bigquery-1.5.0b4/README.md` & `dbt-bigquery-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/__init__.py` & `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/column.py` & `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/column.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/connections.py` & `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/dataset.py` & `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/dataset.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/gcloud.py` & `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/gcloud.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/impl.py` & `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from dataclasses import dataclass
 import threading
 from typing import Dict, List, Optional, Any, Set, Union, Type
+
+from dbt.contracts.graph.nodes import ColumnLevelConstraint, ModelLevelConstraint, ConstraintType
 from dbt.dataclass_schema import dbtClassMixin, ValidationError
 
 import dbt.deprecations
 import dbt.exceptions
 import dbt.clients.agate_helper
 
 from dbt import ui  # type: ignore
 from dbt.adapters.base import (
     BaseAdapter,
+    ConstraintSupport,
     available,
     RelationType,
     BaseRelation,
     SchemaSearchMap,
     AdapterConfig,
     PythonJobHelper,
 )
@@ -26,15 +29,17 @@
 from dbt.adapters.bigquery import BigQueryConnectionManager
 from dbt.adapters.bigquery.python_submissions import (
     ClusterDataprocHelper,
     ServerlessDataProcHelper,
 )
 from dbt.adapters.bigquery.connections import BigQueryAdapterResponse
 from dbt.contracts.graph.manifest import Manifest
-from dbt.events import AdapterLogger
+from dbt.events import (
+    AdapterLogger,
+)
 from dbt.events.functions import fire_event
 from dbt.events.types import SchemaCreation, SchemaDrop
 from dbt.utils import filter_null_values
 
 import google.auth
 import google.api_core
 import google.oauth2
@@ -162,14 +167,22 @@
 
     Relation = BigQueryRelation
     Column = BigQueryColumn
     ConnectionManager = BigQueryConnectionManager
 
     AdapterSpecificConfigs = BigqueryConfig
 
+    CONSTRAINT_SUPPORT = {
+        ConstraintType.check: ConstraintSupport.NOT_SUPPORTED,
+        ConstraintType.not_null: ConstraintSupport.ENFORCED,
+        ConstraintType.unique: ConstraintSupport.NOT_SUPPORTED,
+        ConstraintType.primary_key: ConstraintSupport.ENFORCED,
+        ConstraintType.foreign_key: ConstraintSupport.ENFORCED,
+    }
+
     ###
     # Implementations of abstract methods
     ###
 
     @classmethod
     def date_function(cls) -> str:
         return "CURRENT_TIMESTAMP()"
@@ -903,7 +916,28 @@
 
     @property
     def python_submission_helpers(self) -> Dict[str, Type[PythonJobHelper]]:
         return {
             "cluster": ClusterDataprocHelper,
             "serverless": ServerlessDataProcHelper,
         }
+
+    @classmethod
+    def render_column_constraint(cls, constraint: ColumnLevelConstraint) -> Optional[str]:
+        c = super().render_column_constraint(constraint)
+        if (
+            constraint.type == ConstraintType.primary_key
+            or constraint.type == ConstraintType.foreign_key
+        ):
+            return f"{c} not enforced" if c else None
+        return c
+
+    @classmethod
+    def render_model_constraint(cls, constraint: ModelLevelConstraint) -> Optional[str]:
+        c = super().render_model_constraint(constraint)
+        if (
+            constraint.type == ConstraintType.primary_key
+            or constraint.type == ConstraintType.foreign_key
+        ):
+            return f"{c} not enforced" if c else None
+
+        return c
```

### Comparing `dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/python_submissions.py` & `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/adapters/bigquery/relation.py` & `dbt-bigquery-1.5.0rc1/dbt/adapters/bigquery/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/adapters/apply_grants.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/adapters.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/adapters.sql`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     {{ sql_header if sql_header is not none }}
 
     create or replace table {{ relation }}
       {%- set contract_config = config.get('contract') -%}
       {%- if contract_config.enforced -%}
         {{ get_assert_columns_equivalent(compiled_code) }}
-        {{ get_columns_spec_ddl() }}
+        {{ get_table_columns_and_constraints() }}
         {%- set compiled_code = get_select_subquery(compiled_code) %}
       {% endif %}
     {{ partition_by(partition_config) }}
     {{ cluster_by(raw_cluster_by) }}
 
     {{ bigquery_table_options(config, model, temporary) }}
     as (
@@ -69,14 +69,20 @@
     {#--
     N.B. Python models _can_ write to temp views HOWEVER they use a different session
     and have already expired by the time they need to be used (I.E. in merges for incremental models)
 
     TODO: Deep dive into spark sessions to see if we can reuse a single session for an entire
     dbt invocation.
      --#}
+
+    {#-- when a user wants to change the schema of an existing relation, they must intentionally drop the table in the dataset --#}
+    {%- set old_relation = adapter.get_relation(database=relation.database, schema=relation.schema, identifier=relation.identifier) -%}
+    {%- if (old_relation.is_table and (should_full_refresh())) -%}
+      {% do adapter.drop_relation(relation) %}
+    {%- endif -%}
     {{ py_write_table(compiled_code=compiled_code, target_relation=relation.quote(database=False, schema=False, identifier=False)) }}
   {%- else -%}
     {% do exceptions.raise_compiler_error("bigquery__create_table_as macro didn't get supported language, it got %s" % language) %}
   {%- endif -%}
 
 {%- endmacro -%}
```

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/catalog.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/copy.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/copy.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,16 @@
       {% else %}
         -- 1. temp table already exists, we used it to check for schema changes
       {% endif %}
 
       -- 2. define partitions to update
       set (dbt_partitions_for_replacement) = (
           select as struct
-              array_agg(distinct {{ partition_by.render_wrapped() }})
+              -- IGNORE NULLS: this needs to be aligned to _dbt_max_partition, which ignores null
+              array_agg(distinct {{ partition_by.render_wrapped() }} IGNORE NULLS)
           from {{ tmp_relation }}
       );
 
       -- 3. run the merge statement
       {{ get_insert_overwrite_merge_sql(target_relation, source_sql, dest_columns, [predicate]) }};
 
       -- 4. clean up the temp table
```

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/seed.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/table.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/macros/materializations/view.sql` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt/include/bigquery/profile_template.yml` & `dbt-bigquery-1.5.0rc1/dbt/include/bigquery/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/dbt_bigquery.egg-info/PKG-INFO` & `dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.5.0b4
+Version: 1.5.0rc1
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.5.0b4 Summary: The Bigquery
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
-text/markdown License-File: LICENSE.md
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.5.0rc1 Summary: The
+Bigquery adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+bigquery Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-bigquery The `dbt-bigquery` package contains all of
```

### Comparing `dbt-bigquery-1.5.0b4/dbt_bigquery.egg-info/SOURCES.txt` & `dbt-bigquery-1.5.0rc1/dbt_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.5.0b4/setup.py` & `dbt-bigquery-1.5.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     else:
         core_patch = "0"
 
     return f"{major}.{minor}.{core_patch}"
 
 
 package_name = "dbt-bigquery"
-package_version = "1.5.0b4"
+package_version = "1.5.0rc1"
 dbt_core_version = _dbt_core_version(_dbt_bigquery_version())
 description = """The BigQuery adapter plugin for dbt"""
 
 setup(
     name="dbt-bigquery",
     version=_dbt_bigquery_version(),
     description="The Bigquery adapter plugin for dbt",
```

