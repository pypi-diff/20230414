# Comparing `tmp/taipy-core-2.2.1.tar.gz` & `tmp/taipy-core-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-core-2.2.1.tar", last modified: Thu Apr 13 18:20:15 2023, max compression
+gzip compressed data, was "taipy-core-2.2.2.tar", last modified: Fri Apr 14 17:12:46 2023, max compression
```

## Comparing `taipy-core-2.2.1.tar` & `taipy-core-2.2.2.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.290837 taipy-core-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-13 18:20:02.000000 taipy-core-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 18:20:02.000000 taipy-core-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-13 18:20:15.290837 taipy-core-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-13 18:20:02.000000 taipy-core-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 18:20:02.000000 taipy-core-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:20:15.290837 taipy-core-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-13 18:20:02.000000 taipy-core-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.266836 taipy-core-2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.266836 taipy-core-2.2.1/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.266836 taipy-core-2.2.1/src/taipy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.266836 taipy-core-2.2.1/src/taipy/core/_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_manager/_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.270836 taipy-core-2.2.1/src/taipy/core/_repository/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_repository/_filesystem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_repository/_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_repository/_repository_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_repository/_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_repository/_sql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_repository/_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.270836 taipy-core-2.2.1/src/taipy/core/_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_scheduler/_abstract_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.270836 taipy-core-2.2.1/src/taipy/core/_scheduler/_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_scheduler/_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_scheduler/_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_scheduler/_scheduler_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.270836 taipy-core-2.2.1/src/taipy/core/_version/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/_version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/_version_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/_version_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/_version_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/_version_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/_version_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/_version/_version_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.274836 taipy-core-2.2.1/src/taipy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/_get_valid_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/_listattributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/_reload.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/common/default_custom_document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.274836 taipy-core-2.2.1/src/taipy/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.274836 taipy-core-2.2.1/src/taipy/core/config/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/checkers/_data_node_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/checkers/_job_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/checkers/_pipeline_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/checkers/_scenario_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/checkers/_task_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    32545 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/data_node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/job_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/scenario_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/config/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.274836 taipy-core-2.2.1/src/taipy/core/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/cycle/_cycle_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/cycle/_cycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/cycle/_cycle_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/cycle/_cycle_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/cycle/_cycle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/cycle/_cycle_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/cycle/_cycle_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/cycle/cycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.278837 taipy-core-2.2.1/src/taipy/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/_data_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/_data_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/_data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/_data_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/_data_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/abstract_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/data/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.278837 taipy-core-2.2.1/src/taipy/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.282837 taipy-core-2.2.1/src/taipy/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/job/_job_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/job/_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/job/_job_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/job/_job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/job/_job_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/job/_job_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/job/_job_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/job/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/job/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.282837 taipy-core-2.2.1/src/taipy/core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/pipeline/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.286837 taipy-core-2.2.1/src/taipy/core/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/scenario/_scenario_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/scenario/_scenario_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/scenario/_scenario_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/scenario/_scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/scenario/_scenario_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/scenario/_scenario_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/scenario/_scenario_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/scenario/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    23645 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/taipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.286837 taipy-core-2.2.1/src/taipy/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/task/_task_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/task/_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/task/_task_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/task/_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/task/_task_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/task/_task_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/task/_task_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:20:02.000000 taipy-core-2.2.1/src/taipy/core/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.286837 taipy-core-2.2.1/src/taipy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-13 18:20:15.000000 taipy-core-2.2.1/src/taipy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-13 18:20:15.000000 taipy-core-2.2.1/src/taipy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:20:15.000000 taipy-core-2.2.1/src/taipy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:20:07.000000 taipy-core-2.2.1/src/taipy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-13 18:20:15.000000 taipy-core-2.2.1/src/taipy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 18:20:15.000000 taipy-core-2.2.1/src/taipy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:20:15.286837 taipy-core-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-13 18:20:02.000000 taipy-core-2.2.1/tests/test_complex_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-04-13 18:20:02.000000 taipy-core-2.2.1/tests/test_taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.616891 taipy-core-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-14 17:12:36.000000 taipy-core-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 17:12:36.000000 taipy-core-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-14 17:12:46.616891 taipy-core-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-14 17:12:36.000000 taipy-core-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 17:12:36.000000 taipy-core-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:12:46.616891 taipy-core-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-14 17:12:36.000000 taipy-core-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.596891 taipy-core-2.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.596891 taipy-core-2.2.2/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.596891 taipy-core-2.2.2/src/taipy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.600891 taipy-core-2.2.2/src/taipy/core/_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_manager/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_manager/_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.600891 taipy-core-2.2.2/src/taipy/core/_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_filesystem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_repository_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_sql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_repository/_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.600891 taipy-core-2.2.2/src/taipy/core/_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_abstract_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.600891 taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12353 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_scheduler/_scheduler_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.600891 taipy-core-2.2.2/src/taipy/core/_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/_version/_version_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.604891 taipy-core-2.2.2/src/taipy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_get_valid_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_listattributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/common/default_custom_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.604891 taipy-core-2.2.2/src/taipy/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.604891 taipy-core-2.2.2/src/taipy/core/config/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/_data_node_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/_job_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/_pipeline_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/_scenario_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/checkers/_task_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32343 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/data_node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/job_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/scenario_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/config/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.608891 taipy-core-2.2.2/src/taipy/core/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/_cycle_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/cycle/cycle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.612891 taipy-core-2.2.2/src/taipy/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_data_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/abstract_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/data/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.612891 taipy-core-2.2.2/src/taipy/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.612891 taipy-core-2.2.2/src/taipy/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/_job_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/job/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.612891 taipy-core-2.2.2/src/taipy/core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.616891 taipy-core-2.2.2/src/taipy/core/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/_scenario_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12425 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/scenario/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23645 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.616891 taipy-core-2.2.2/src/taipy/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/_task_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 17:12:36.000000 taipy-core-2.2.2/src/taipy/core/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.616891 taipy-core-2.2.2/src/taipy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-14 17:12:46.000000 taipy-core-2.2.2/src/taipy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-14 17:12:46.000000 taipy-core-2.2.2/src/taipy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:12:46.000000 taipy-core-2.2.2/src/taipy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:12:39.000000 taipy-core-2.2.2/src/taipy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 17:12:46.000000 taipy-core-2.2.2/src/taipy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 17:12:46.000000 taipy-core-2.2.2/src/taipy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:12:46.616891 taipy-core-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-14 17:12:36.000000 taipy-core-2.2.2/tests/test_complex_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26443 2023-04-14 17:12:36.000000 taipy-core-2.2.2/tests/test_taipy.py
```

### Comparing `taipy-core-2.2.1/LICENSE` & `taipy-core-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/PKG-INFO` & `taipy-core-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.2.1
+Version: 2.2.2
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.2.1/README.md` & `taipy-core-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/setup.py` & `taipy-core-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/__init__.py` & `taipy-core-2.2.2/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/__init__.py` & `taipy-core-2.2.2/src/taipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_core.py` & `taipy-core-2.2.2/src/taipy/core/_core.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_manager/__init__.py` & `taipy-core-2.2.2/src/taipy/core/_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_manager/_manager.py` & `taipy-core-2.2.2/src/taipy/core/_manager/_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_manager/_manager_factory.py` & `taipy-core-2.2.2/src/taipy/core/_manager/_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_repository/__init__.py` & `taipy-core-2.2.2/src/taipy/core/_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_repository/_filesystem_repository.py` & `taipy-core-2.2.2/src/taipy/core/_repository/_filesystem_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_repository/_repository.py` & `taipy-core-2.2.2/src/taipy/core/_repository/_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_repository/_repository_adapter.py` & `taipy-core-2.2.2/src/taipy/core/_repository/_repository_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_repository/_repository_factory.py` & `taipy-core-2.2.2/src/taipy/core/_repository/_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_repository/_sql_model.py` & `taipy-core-2.2.2/src/taipy/core/_repository/_sql_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_repository/_sql_repository.py` & `taipy-core-2.2.2/src/taipy/core/_repository/_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_scheduler/__init__.py` & `taipy-core-2.2.2/src/taipy/core/_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_scheduler/_abstract_scheduler.py` & `taipy-core-2.2.2/src/taipy/core/_scheduler/_abstract_scheduler.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_scheduler/_dispatcher/__init__.py` & `taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py` & `taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_development_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py` & `taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py` & `taipy-core-2.2.2/src/taipy/core/_scheduler/_dispatcher/_standalone_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_scheduler/_scheduler.py` & `taipy-core-2.2.2/src/taipy/core/_scheduler/_scheduler.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_scheduler/_scheduler_factory.py` & `taipy-core-2.2.2/src/taipy/core/_scheduler/_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/__init__.py` & `taipy-core-2.2.2/src/taipy/core/_version/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/_utils.py` & `taipy-core-2.2.2/src/taipy/core/_version/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/_version.py` & `taipy-core-2.2.2/src/taipy/core/_version/_version.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/_version_cli.py` & `taipy-core-2.2.2/src/taipy/core/_version/_version_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/_version_fs_repository.py` & `taipy-core-2.2.2/src/taipy/core/_version/_version_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/_version_manager.py` & `taipy-core-2.2.2/src/taipy/core/_version/_version_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/_version_manager_factory.py` & `taipy-core-2.2.2/src/taipy/core/_version/_version_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/_version_model.py` & `taipy-core-2.2.2/src/taipy/core/_version/_version_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/_version_repository.py` & `taipy-core-2.2.2/src/taipy/core/_version/_version_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/_version_repository_factory.py` & `taipy-core-2.2.2/src/taipy/core/_version/_version_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/_version/_version_sql_repository.py` & `taipy-core-2.2.2/src/taipy/core/_version/_version_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/__init__.py` & `taipy-core-2.2.2/src/taipy/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/_entity.py` & `taipy-core-2.2.2/src/taipy/core/common/_entity.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/_entity_ids.py` & `taipy-core-2.2.2/src/taipy/core/common/_entity_ids.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/_get_valid_filename.py` & `taipy-core-2.2.2/src/taipy/core/common/_get_valid_filename.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/_listattributes.py` & `taipy-core-2.2.2/src/taipy/core/common/_listattributes.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/_properties.py` & `taipy-core-2.2.2/src/taipy/core/common/_properties.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/_reload.py` & `taipy-core-2.2.2/src/taipy/core/common/_reload.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/_repr_enum.py` & `taipy-core-2.2.2/src/taipy/core/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/_utils.py` & `taipy-core-2.2.2/src/taipy/core/common/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/_warnings.py` & `taipy-core-2.2.2/src/taipy/core/common/_warnings.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/alias.py` & `taipy-core-2.2.2/src/taipy/core/common/alias.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/common/default_custom_document.py` & `taipy-core-2.2.2/src/taipy/core/common/default_custom_document.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/__init__.py` & `taipy-core-2.2.2/src/taipy/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/checkers/__init__.py` & `taipy-core-2.2.2/src/taipy/core/config/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/checkers/_data_node_config_checker.py` & `taipy-core-2.2.2/src/taipy/core/config/checkers/_data_node_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/checkers/_job_config_checker.py` & `taipy-core-2.2.2/src/taipy/core/config/checkers/_job_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/checkers/_pipeline_config_checker.py` & `taipy-core-2.2.2/src/taipy/core/config/checkers/_pipeline_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/checkers/_scenario_config_checker.py` & `taipy-core-2.2.2/src/taipy/core/config/checkers/_scenario_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/checkers/_task_config_checker.py` & `taipy-core-2.2.2/src/taipy/core/config/checkers/_task_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/config.schema.json` & `taipy-core-2.2.2/src/taipy/core/config/config.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999986847643098%*

 * *Differences: {"'properties'": "{'DATA_NODE': {'additionalProperties': {'properties': {'db_driver': "*

 * *                 "{'description': 'storage_type: sql, sql_table specific.'}}}}}"}*

```diff
@@ -16,15 +16,15 @@
                     },
                     "custom_document": {
                         "description": "storage_type: mongo_collection specific.",
                         "taipy_class": true,
                         "type": "string"
                     },
                     "db_driver": {
-                        "description": "storage_type: sql, sql_table specific. The default value of db_driver is \"ODBC Driver 17 for SQL Server\".",
+                        "description": "storage_type: sql, sql_table specific.",
                         "type": "string"
                     },
                     "db_engine": {
                         "description": "storage_type: sql, sql_table specific. One of sqlite, mssql, mysql, postgresql",
                         "type": "string"
                     },
                     "db_extra_args": {
```

### Comparing `taipy-core-2.2.1/src/taipy/core/config/data_node_config.py` & `taipy-core-2.2.2/src/taipy/core/config/data_node_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,15 +589,15 @@
         db_username: str,
         db_password: str,
         db_name: str,
         db_engine: str,
         table_name: str = None,
         db_port: int = 1433,
         db_host: str = "localhost",
-        db_driver: str = "ODBC Driver 17 for SQL Server",
+        db_driver: str = "",
         db_extra_args: Dict[str, Any] = None,
         exposed_type=_EXPOSED_TYPE_PANDAS,
         scope: Scope = _DEFAULT_SCOPE,
         **properties,
     ):
         """Configure a new SQL table data node configuration.
 
@@ -605,16 +605,15 @@
             id (str): The unique identifier of the new SQL data node configuration.
             db_username (str): The database username.
             db_password (str): The database password.
             db_name (str): The database name, or the name of the SQLite database file.
             db_host (str): The database host. The default value is _"localhost"_.
             db_engine (str): The database engine. Possible values are _"sqlite"_, _"mssql"_, _"mysql"_, or
                 _"postgresql"_.
-            db_driver (str): The database driver. The default value is
-                _"ODBC Driver 17 for SQL Server"_.
+            db_driver (str): The database driver.
             db_port (int): The database port. The default value is 1433.
             db_extra_args (Dict[str, Any]): A dictionary of additional arguments to be passed into database
                 connection string.
             table_name (str): The name of the SQL table.
             exposed_type: The exposed type of the data read from SQL query. The default value is `pandas`.
             scope (Scope^): The scope of the SQL data node configuration. The default value is
                 `Scope.SCENARIO`.
@@ -647,15 +646,15 @@
         id: str,
         db_username: str,
         db_password: str,
         db_name: str,
         db_engine: str,
         db_port: int = 1433,
         db_host: str = "localhost",
-        db_driver: str = "ODBC Driver 17 for SQL Server",
+        db_driver: str = "",
         db_extra_args: Dict[str, Any] = None,
         read_query: str = None,
         write_query_builder: Callable = None,
         exposed_type=_DEFAULT_EXPOSED_TYPE,
         scope: Scope = _DEFAULT_SCOPE,
         **properties,
     ):
@@ -666,16 +665,15 @@
             db_username (str): The database username.
             db_password (str): The database password.
             db_name (str): The database name, or the name of the SQLite database file.
             db_engine (str): The database engine. Possible values are _"sqlite"_, _"mssql"_, _"mysql"_, or
                 _"postgresql"_.
             db_port (int): The database port. The default value is 1433.
             db_host (str): The database host. The default value is _"localhost"_.
-            db_driver (str): The database driver. The default value is
-                _"ODBC Driver 17 for SQL Server"_.
+            db_driver (str): The database driver.
             db_extra_args (Dict[str, Any]): A dictionary of additional arguments to be passed into database
                 connection string.
             read_query (str): The SQL query string used to read the data from the database.
             write_query_builder (Callable): A callback function that takes the data as an input parameter and returns a
                 list of SQL queries.
             exposed_type: The exposed type of the data read from SQL query. The default value is `pandas`.
             scope (Scope^): The scope of the SQL data node configuration. The default value is
```

### Comparing `taipy-core-2.2.1/src/taipy/core/config/job_config.py` & `taipy-core-2.2.2/src/taipy/core/config/job_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/pipeline_config.py` & `taipy-core-2.2.2/src/taipy/core/config/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/scenario_config.py` & `taipy-core-2.2.2/src/taipy/core/config/scenario_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/config/task_config.py` & `taipy-core-2.2.2/src/taipy/core/config/task_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/cycle/__init__.py` & `taipy-core-2.2.2/src/taipy/core/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/cycle/_cycle_fs_repository.py` & `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/cycle/_cycle_manager.py` & `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/cycle/_cycle_manager_factory.py` & `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/cycle/_cycle_model.py` & `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/cycle/_cycle_repository.py` & `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/cycle/_cycle_repository_factory.py` & `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/cycle/_cycle_sql_repository.py` & `taipy-core-2.2.2/src/taipy/core/cycle/_cycle_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/cycle/cycle.py` & `taipy-core-2.2.2/src/taipy/core/cycle/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/__init__.py` & `taipy-core-2.2.2/src/taipy/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/_data_fs_repository.py` & `taipy-core-2.2.2/src/taipy/core/data/_data_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/_data_manager.py` & `taipy-core-2.2.2/src/taipy/core/data/_data_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/_data_manager_factory.py` & `taipy-core-2.2.2/src/taipy/core/data/_data_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/_data_model.py` & `taipy-core-2.2.2/src/taipy/core/data/_data_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/_data_repository.py` & `taipy-core-2.2.2/src/taipy/core/data/_data_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/_data_repository_factory.py` & `taipy-core-2.2.2/src/taipy/core/data/_data_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/_data_sql_repository.py` & `taipy-core-2.2.2/src/taipy/core/data/_data_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/_filter.py` & `taipy-core-2.2.2/src/taipy/core/data/_filter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/abstract_sql.py` & `taipy-core-2.2.2/src/taipy/core/data/abstract_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         __DB_DRIVER_KEY,
         __DB_EXTRA_ARGS_KEY,
         __SQLITE_PATH_KEY,
     ]
 
     __DB_HOST_DEFAULT = "localhost"
     __DB_PORT_DEFAULT = 1433
-    __DB_DRIVER_DEFAULT = "ODBC Driver 17 for SQL Server"
+    __DB_DRIVER_DEFAULT = ""
 
     __ENGINE_MSSQL = "mssql"
     __ENGINE_SQLITE = "sqlite"
     __ENGINE_MYSQL = "mysql"
     __ENGINE_POSTGRESQL = "postgresql"
 
     _ENGINE_REQUIRED_PROPERTIES: Dict[str, List[str]] = {
@@ -158,15 +158,16 @@
             db_name = urllib.parse.quote_plus(db_name)
 
         host = self.properties.get(self.__DB_HOST_KEY, self.__DB_HOST_DEFAULT)
         port = self.properties.get(self.__DB_PORT_KEY, self.__DB_PORT_DEFAULT)
         driver = self.properties.get(self.__DB_DRIVER_KEY, self.__DB_DRIVER_DEFAULT)
         extra_args = self.properties.get(self.__DB_EXTRA_ARGS_KEY, {})
 
-        extra_args = {**extra_args, "driver": driver}
+        if driver:
+            extra_args = {**extra_args, "driver": driver}
         for k, v in extra_args.items():
             extra_args[k] = re.sub(r"\s+", "+", v)
         extra_args_str = "&".join(f"{k}={str(v)}" for k, v in extra_args.items())
 
         if engine == self.__ENGINE_MSSQL:
             return f"mssql+pyodbc://{username}:{password}@{host}:{port}/{db_name}?{extra_args_str}"
         elif engine == self.__ENGINE_MYSQL:
```

### Comparing `taipy-core-2.2.1/src/taipy/core/data/csv.py` & `taipy-core-2.2.2/src/taipy/core/data/csv.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/data_node.py` & `taipy-core-2.2.2/src/taipy/core/data/data_node.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/excel.py` & `taipy-core-2.2.2/src/taipy/core/data/excel.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/generic.py` & `taipy-core-2.2.2/src/taipy/core/data/generic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/in_memory.py` & `taipy-core-2.2.2/src/taipy/core/data/in_memory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/json.py` & `taipy-core-2.2.2/src/taipy/core/data/json.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/mongo.py` & `taipy-core-2.2.2/src/taipy/core/data/mongo.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/operator.py` & `taipy-core-2.2.2/src/taipy/core/data/operator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/parquet.py` & `taipy-core-2.2.2/src/taipy/core/data/parquet.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/pickle.py` & `taipy-core-2.2.2/src/taipy/core/data/pickle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/data/sql.py` & `taipy-core-2.2.2/src/taipy/core/data/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             - _"db_username"_ `(str)`: The database username.
             - _"db_password"_ `(str)`: The database password.
             - _"db_name"_ `(str)`: The database name, or the name of the SQLite database file.
             - _"db_engine"_ `(str)`: The database engine. Possible values are _"sqlite"_, _"mssql"_, _"mysql"_, or
                 _"postgresql"_.
             - _"db_port"_ `(int)`: The database port. The default value is 1433.
             - _"db_host"_ `(str)`: The database host. The default value is _"localhost"_.
-            - _"db_driver"_ `(str)`: The database driver. The default value is _"ODBC Driver 17 for SQL Server"_.
+            - _"db_driver"_ `(str)`: The database driver.
             - _"db_extra_args"_ `(Dict[str, Any])`: A dictionary of additional arguments to be passed into database
                 connection string.
             - _"read_query"_ `(str)`: The SQL query string used to read the data from the database.
             - _"write_query_builder"_ `(Callable)`: A callback function that takes the data as an input parameter and
                 returns a list of SQL queries.
             - _"exposed_type"_: The exposed type of the data read from SQL query. The default value is `pandas`.
     """
```

### Comparing `taipy-core-2.2.1/src/taipy/core/data/sql_table.py` & `taipy-core-2.2.2/src/taipy/core/data/sql_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
             - _"db_username"_ `(str)`: The database username.
             - _"db_password"_ `(str)`: The database password.
             - _"db_name"_ `(str)`: The database name, or the name of the SQLite database file.
             - _"db_host"_ `(str)`: The database host. The default value is _"localhost"_.
             - _"db_engine"_ `(str)`: The database engine. For now, the accepted values are _"sqlite"_, _"mssql"_,
                 _"mysql"_, or _"postgresql"_.
-            - _"db_driver"_ `(str)`: The database driver. The default value is _"ODBC Driver 17 for SQL Server"_.
+            - _"db_driver"_ `(str)`: The database driver.
             - _"db_port"_ `(int)`: The database port. The default value is 1433.
             - _"db_extra_args"_ `(Dict[str, Any])`: A dictionary of additional arguments to be passed into database
                 connection string.
             - _"table_name"_ `(str)`: The name of the SQL table.
             - _"exposed_type"_: The exposed type of the data read from SQL query. The default value is `pandas`.
     """
```

### Comparing `taipy-core-2.2.1/src/taipy/core/exceptions/__init__.py` & `taipy-core-2.2.2/src/taipy/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/exceptions/exceptions.py` & `taipy-core-2.2.2/src/taipy/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/job/__init__.py` & `taipy-core-2.2.2/src/taipy/core/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/job/_job_fs_repository.py` & `taipy-core-2.2.2/src/taipy/core/job/_job_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/job/_job_manager.py` & `taipy-core-2.2.2/src/taipy/core/job/_job_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/job/_job_manager_factory.py` & `taipy-core-2.2.2/src/taipy/core/job/_job_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/job/_job_model.py` & `taipy-core-2.2.2/src/taipy/core/job/_job_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/job/_job_repository.py` & `taipy-core-2.2.2/src/taipy/core/job/_job_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/job/_job_repository_factory.py` & `taipy-core-2.2.2/src/taipy/core/job/_job_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/job/_job_sql_repository.py` & `taipy-core-2.2.2/src/taipy/core/job/_job_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/job/job.py` & `taipy-core-2.2.2/src/taipy/core/job/job.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/job/status.py` & `taipy-core-2.2.2/src/taipy/core/job/status.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/pipeline/__init__.py` & `taipy-core-2.2.2/src/taipy/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_fs_repository.py` & `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_manager.py` & `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_manager_factory.py` & `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_model.py` & `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_repository.py` & `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_repository_factory.py` & `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/pipeline/_pipeline_sql_repository.py` & `taipy-core-2.2.2/src/taipy/core/pipeline/_pipeline_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/pipeline/pipeline.py` & `taipy-core-2.2.2/src/taipy/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/scenario/__init__.py` & `taipy-core-2.2.2/src/taipy/core/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/scenario/_scenario_fs_repository.py` & `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/scenario/_scenario_manager.py` & `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/scenario/_scenario_manager_factory.py` & `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/scenario/_scenario_model.py` & `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/scenario/_scenario_repository.py` & `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/scenario/_scenario_repository_factory.py` & `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/scenario/_scenario_sql_repository.py` & `taipy-core-2.2.2/src/taipy/core/scenario/_scenario_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/scenario/scenario.py` & `taipy-core-2.2.2/src/taipy/core/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/taipy.py` & `taipy-core-2.2.2/src/taipy/core/taipy.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/task/__init__.py` & `taipy-core-2.2.2/src/taipy/core/task/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/task/_task_fs_repository.py` & `taipy-core-2.2.2/src/taipy/core/task/_task_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/task/_task_manager.py` & `taipy-core-2.2.2/src/taipy/core/task/_task_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/task/_task_manager_factory.py` & `taipy-core-2.2.2/src/taipy/core/task/_task_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/task/_task_model.py` & `taipy-core-2.2.2/src/taipy/core/task/_task_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/task/_task_repository.py` & `taipy-core-2.2.2/src/taipy/core/task/_task_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/task/_task_repository_factory.py` & `taipy-core-2.2.2/src/taipy/core/task/_task_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/task/_task_sql_repository.py` & `taipy-core-2.2.2/src/taipy/core/task/_task_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy/core/task/task.py` & `taipy-core-2.2.2/src/taipy/core/task/task.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/src/taipy_core.egg-info/PKG-INFO` & `taipy-core-2.2.2/src/taipy_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.2.1
+Version: 2.2.2
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.2.1/src/taipy_core.egg-info/SOURCES.txt` & `taipy-core-2.2.2/src/taipy_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/tests/test_complex_application.py` & `taipy-core-2.2.2/tests/test_complex_application.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.2.1/tests/test_taipy.py` & `taipy-core-2.2.2/tests/test_taipy.py`

 * *Files identical despite different names*

