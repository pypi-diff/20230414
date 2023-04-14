# Comparing `tmp/toolsql-0.3.9.tar.gz` & `tmp/toolsql-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolsql-0.3.9.tar", last modified: Wed Aug 10 22:51:05 2022, max compression
+gzip compressed data, was "toolsql-0.5.0.tar", last modified: Fri Apr 14 21:53:40 2023, max compression
```

## Comparing `toolsql-0.3.9.tar` & `toolsql-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,92 @@
--rw-r--r--   0        0        0       81 2022-03-29 21:10:59.463974 toolsql-0.3.9/.gitignore
--rw-r--r--   0        0        0     1084 2022-04-18 03:03:52.462129 toolsql-0.3.9/LICENSE
--rw-r--r--   0        0        0     1309 2022-03-29 21:06:41.655455 toolsql-0.3.9/README.md
--rw-r--r--   0        0        0      443 2022-08-05 00:05:58.706809 toolsql-0.3.9/pyproject.toml
--rw-r--r--   0        0        0      355 2022-08-10 22:50:42.656687 toolsql-0.3.9/toolsql/__init__.py
--rw-r--r--   0        0        0        1 2022-03-24 04:41:24.873797 toolsql-0.3.9/toolsql/cli/__init__.py
--rw-r--r--   0        0        0        0 2022-03-23 06:44:21.781724 toolsql-0.3.9/toolsql/cli/commands/__init__.py
--rw-r--r--   0        0        0        0 2022-03-23 06:44:37.069656 toolsql-0.3.9/toolsql/cli/commands/sql/__init__.py
--rw-r--r--   0        0        0      383 2022-05-16 07:14:08.677462 toolsql-0.3.9/toolsql/cli/commands/sql/config_command.py
--rw-r--r--   0        0        0      775 2022-05-27 17:23:30.272426 toolsql-0.3.9/toolsql/cli/commands/sql/login_command.py
--rw-r--r--   0        0        0        0 2022-03-23 06:44:29.585689 toolsql-0.3.9/toolsql/cli/commands/sql/migrate/__init__.py
--rw-r--r--   0        0        0      385 2022-05-22 20:56:20.650512 toolsql-0.3.9/toolsql/cli/commands/sql/migrate/all_command.py
--rw-r--r--   0        0        0      384 2022-05-22 20:55:10.954567 toolsql-0.3.9/toolsql/cli/commands/sql/migrate/apply_command.py
--rw-r--r--   0        0        0      857 2022-05-22 20:55:08.566569 toolsql-0.3.9/toolsql/cli/commands/sql/migrate/create_command.py
--rw-r--r--   0        0        0      490 2022-05-22 20:55:05.906572 toolsql-0.3.9/toolsql/cli/commands/sql/migrate/edit_command.py
--rw-r--r--   0        0        0      864 2022-05-22 20:55:03.442575 toolsql-0.3.9/toolsql/cli/commands/sql/migrate/purge_command.py
--rw-r--r--   0        0        0      389 2022-05-22 20:55:23.550554 toolsql-0.3.9/toolsql/cli/commands/sql/migrate/root_command.py
--rw-r--r--   0        0        0      894 2022-05-22 20:56:21.878511 toolsql-0.3.9/toolsql/cli/commands/sql/migrate/setup_command.py
--rw-r--r--   0        0        0      398 2022-05-22 20:56:30.802507 toolsql-0.3.9/toolsql/cli/commands/sql/migrate/status_command.py
--rw-r--r--   0        0        0      738 2022-05-16 20:14:19.523265 toolsql-0.3.9/toolsql/cli/commands/sql/schema_command.py
--rw-r--r--   0        0        0      640 2022-08-10 22:48:56.036915 toolsql-0.3.9/toolsql/cli/commands/sql/usage_command.py
--rw-r--r--   0        0        0     1302 2022-05-16 06:24:44.904916 toolsql-0.3.9/toolsql/cli/plugin.py
--rw-r--r--   0        0        0       87 2021-01-15 03:55:30.000000 toolsql-0.3.9/toolsql/crud_utils/__init__.py
--rw-r--r--   0        0        0     5979 2022-03-31 03:46:48.818450 toolsql-0.3.9/toolsql/crud_utils/create.py
--rw-r--r--   0        0        0     2147 2022-06-29 03:43:44.969037 toolsql-0.3.9/toolsql/crud_utils/delete.py
--rw-r--r--   0        0        0     6960 2022-06-29 03:42:58.265089 toolsql-0.3.9/toolsql/crud_utils/read.py
--rw-r--r--   0        0        0     1276 2021-01-15 03:55:30.000000 toolsql-0.3.9/toolsql/crud_utils/update.py
--rw-r--r--   0        0        0     2682 2022-08-10 22:37:10.146334 toolsql-0.3.9/toolsql/dba_utils.py
--rw-r--r--   0        0        0      150 2022-06-06 20:00:32.829014 toolsql-0.3.9/toolsql/exceptions.py
--rw-r--r--   0        0        0     1487 2022-06-04 16:37:08.898783 toolsql-0.3.9/toolsql/external_utils.py
--rw-r--r--   0        0        0      156 2021-01-15 03:55:30.000000 toolsql-0.3.9/toolsql/migrate_utils/__init__.py
--rw-r--r--   0        0        0     3801 2022-03-27 03:09:50.229881 toolsql-0.3.9/toolsql/migrate_utils/migrate_actions.py
--rw-r--r--   0        0        0      353 2022-03-27 03:10:31.173915 toolsql-0.3.9/toolsql/migrate_utils/migrate_alembic.py
--rw-r--r--   0        0        0      952 2022-03-27 03:11:00.349932 toolsql-0.3.9/toolsql/migrate_utils/migrate_revisions.py
--rw-r--r--   0        0        0     3690 2022-03-27 03:11:20.909941 toolsql-0.3.9/toolsql/migrate_utils/migrate_setup.py
--rw-r--r--   0        0        0     1110 2021-01-15 03:55:30.000000 toolsql-0.3.9/toolsql/migrate_utils/migrate_summary.py
--rw-r--r--   0        0        0        0 2022-03-29 22:53:45.148062 toolsql-0.3.9/toolsql/py.typed
--rw-r--r--   0        0        0     5741 2022-05-22 23:40:33.883344 toolsql-0.3.9/toolsql/schema_utils.py
--rw-r--r--   0        0        0      127 2022-03-23 08:02:54.068456 toolsql-0.3.9/toolsql/spec/__init__.py
--rw-r--r--   0        0        0      531 2022-03-31 07:25:09.745168 toolsql-0.3.9/toolsql/spec/config_spec.py
--rw-r--r--   0        0        0     1977 2022-05-06 03:38:37.438968 toolsql-0.3.9/toolsql/spec/query_spec.py
--rw-r--r--   0        0        0      189 2022-03-24 02:48:55.494052 toolsql-0.3.9/toolsql/spec/ref_spec.py
--rw-r--r--   0        0        0      715 2022-03-24 05:00:01.167996 toolsql-0.3.9/toolsql/spec/sa_spec.py
--rw-r--r--   0        0        0     1745 2022-05-17 03:18:56.527883 toolsql-0.3.9/toolsql/spec/schema_spec.py
--rw-r--r--   0        0        0      197 2021-01-15 03:55:30.000000 toolsql-0.3.9/toolsql/sqlalchemy_utils/__init__.py
--rw-r--r--   0        0        0     2816 2022-06-04 21:48:50.580374 toolsql-0.3.9/toolsql/sqlalchemy_utils/column_utils.py
--rw-r--r--   0        0        0      896 2022-03-24 05:07:06.093697 toolsql-0.3.9/toolsql/sqlalchemy_utils/conn_utils.py
--rw-r--r--   0        0        0     3944 2022-03-29 21:06:52.855410 toolsql-0.3.9/toolsql/sqlalchemy_utils/engine_utils.py
--rw-r--r--   0        0        0     1442 2022-06-27 21:44:24.551253 toolsql-0.3.9/toolsql/sqlalchemy_utils/metadata_utils.py
--rw-r--r--   0        0        0     2027 2022-03-29 20:16:06.652077 toolsql-0.3.9/toolsql/sqlalchemy_utils/row_utils.py
--rw-r--r--   0        0        0     6093 2022-06-04 18:27:55.059987 toolsql-0.3.9/toolsql/sqlalchemy_utils/statement_utils.py
--rw-r--r--   0        0        0     3681 2022-06-27 21:27:32.326425 toolsql-0.3.9/toolsql/sqlalchemy_utils/table_utils.py
--rw-r--r--   0        0        0    10808 2022-08-10 22:50:08.196761 toolsql-0.3.9/toolsql/summary_utils.py
--rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 toolsql-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-01-27 20:52:41.456006 toolsql-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1084 2022-12-07 18:42:43.242114 toolsql-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4659 2023-04-11 15:37:42.827266 toolsql-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-07 18:42:43.251690 toolsql-0.5.0/py.typed
+-rw-r--r--   0        0        0      648 2023-03-29 05:46:41.761300 toolsql-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      263 2023-01-21 18:52:09.694776 toolsql-0.5.0/tests/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 21:52:27.654376 toolsql-0.5.0/tests/conf/__init__.py
+-rw-r--r--   0        0        0     1670 2023-01-28 01:59:10.345388 toolsql-0.5.0/tests/conf/conf_db_configs.py
+-rw-r--r--   0        0        0     2118 2023-02-27 01:31:39.273127 toolsql-0.5.0/tests/conf/conf_helpers.py
+-rw-r--r--   0        0        0     8392 2023-03-01 01:29:02.029340 toolsql-0.5.0/tests/conf/conf_tables.py
+-rw-r--r--   0        0        0       62 2023-01-22 21:48:58.241419 toolsql-0.5.0/tests/conf/conf_write_queries.py
+-rw-r--r--   0        0        0     4511 2023-02-03 00:06:54.451338 toolsql-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     2432 2023-03-05 03:27:04.199101 toolsql-0.5.0/tests/test_aggregations.py
+-rw-r--r--   0        0        0     2220 2023-02-13 08:03:37.896687 toolsql-0.5.0/tests/test_column_expressions.py
+-rw-r--r--   0        0        0     2084 2023-03-01 07:37:14.269608 toolsql-0.5.0/tests/test_dbms_metadata.py
+-rw-r--r--   0        0        0     5206 2023-03-05 03:26:24.446611 toolsql-0.5.0/tests/test_delete.py
+-rw-r--r--   0        0        0     2526 2023-03-05 07:24:19.484344 toolsql-0.5.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    14606 2023-03-05 04:37:15.341481 toolsql-0.5.0/tests/test_insert.py
+-rw-r--r--   0        0        0     1242 2023-03-01 07:35:46.632270 toolsql-0.5.0/tests/test_multicolumn_indices.py
+-rw-r--r--   0        0        0     1075 2023-03-05 03:27:08.232652 toolsql-0.5.0/tests/test_renaming_results.py
+-rw-r--r--   0        0        0    12107 2023-03-05 03:28:04.000994 toolsql-0.5.0/tests/test_select.py
+-rw-r--r--   0        0        0     2003 2023-02-12 01:16:45.228226 toolsql-0.5.0/tests/test_summary.py
+-rw-r--r--   0        0        0     8908 2023-03-06 02:50:19.508898 toolsql-0.5.0/tests/test_transactions.py
+-rw-r--r--   0        0        0     3478 2023-03-05 03:30:56.862706 toolsql-0.5.0/tests/test_update.py
+-rw-r--r--   0        0        0      233 2023-04-14 21:52:52.266050 toolsql-0.5.0/toolsql/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-11 15:27:03.745564 toolsql-0.5.0/toolsql/dbs/__init__.py
+-rw-r--r--   0        0        0        1 2023-01-25 07:09:40.611833 toolsql-0.5.0/toolsql/dbs/db_classes/__init__.py
+-rw-r--r--   0        0        0     4877 2023-04-12 01:43:17.868464 toolsql-0.5.0/toolsql/dbs/db_classes/abstract_db.py
+-rw-r--r--   0        0        0    18537 2023-04-12 01:44:57.604428 toolsql-0.5.0/toolsql/dbs/db_classes/postgresql_db.py
+-rw-r--r--   0        0        0     9519 2023-04-12 01:45:09.168973 toolsql-0.5.0/toolsql/dbs/db_classes/sqlite_db.py
+-rw-r--r--   0        0        0     1251 2023-02-12 00:58:17.129402 toolsql-0.5.0/toolsql/dbs/db_utils.py
+-rw-r--r--   0        0        0      560 2023-04-11 15:36:56.187104 toolsql-0.5.0/toolsql/dbs/login_utils.py
+-rw-r--r--   0        0        0       84 2023-01-30 03:42:00.561041 toolsql-0.5.0/toolsql/drivers/__init__.py
+-rw-r--r--   0        0        0      149 2023-02-02 22:58:21.072982 toolsql-0.5.0/toolsql/drivers/conn_utils/__init__.py
+-rw-r--r--   0        0        0     1618 2023-03-19 18:55:10.095445 toolsql-0.5.0/toolsql/drivers/conn_utils/conn_attributes.py
+-rw-r--r--   0        0        0     1986 2023-04-12 00:38:59.125862 toolsql-0.5.0/toolsql/drivers/conn_utils/connect_utils.py
+-rw-r--r--   0        0        0      953 2023-02-03 05:07:04.778141 toolsql-0.5.0/toolsql/drivers/conn_utils/db_config_utils.py
+-rw-r--r--   0        0        0     4853 2023-03-06 02:50:00.401901 toolsql-0.5.0/toolsql/drivers/conn_utils/transaction_utils.py
+-rw-r--r--   0        0        0     1833 2023-03-27 19:30:33.769865 toolsql-0.5.0/toolsql/drivers/conn_utils/uri_utils.py
+-rw-r--r--   0        0        0        0 2023-01-19 23:23:14.797191 toolsql-0.5.0/toolsql/drivers/driver_classes/__init__.py
+-rw-r--r--   0        0        0     3437 2023-04-11 15:48:57.844239 toolsql-0.5.0/toolsql/drivers/driver_classes/abstract_driver.py
+-rw-r--r--   0        0        0     1686 2023-03-22 00:04:08.425756 toolsql-0.5.0/toolsql/drivers/driver_classes/aiosqlite_driver.py
+-rw-r--r--   0        0        0     6947 2023-04-12 00:38:35.826888 toolsql-0.5.0/toolsql/drivers/driver_classes/connectorx_driver.py
+-rw-r--r--   0        0        0     4133 2023-04-11 15:55:51.938956 toolsql-0.5.0/toolsql/drivers/driver_classes/dbapi_driver.py
+-rw-r--r--   0        0        0     3878 2023-03-27 19:32:22.818512 toolsql-0.5.0/toolsql/drivers/driver_classes/psycopg_driver.py
+-rw-r--r--   0        0        0     2290 2023-03-22 00:03:41.799839 toolsql-0.5.0/toolsql/drivers/driver_classes/sqlite3_driver.py
+-rw-r--r--   0        0        0     3968 2023-02-11 22:48:18.364943 toolsql-0.5.0/toolsql/drivers/driver_utils.py
+-rw-r--r--   0        0        0       92 2023-02-03 19:35:08.076396 toolsql-0.5.0/toolsql/executors/__init__.py
+-rw-r--r--   0        0        0      127 2023-01-30 03:14:58.462588 toolsql-0.5.0/toolsql/executors/ddl_executors/__init__.py
+-rw-r--r--   0        0        0     2153 2023-02-01 21:30:22.128642 toolsql-0.5.0/toolsql/executors/ddl_executors/alter_executors.py
+-rw-r--r--   0        0        0     2161 2023-03-28 18:58:28.379011 toolsql-0.5.0/toolsql/executors/ddl_executors/create_executors.py
+-rw-r--r--   0        0        0     1153 2023-03-28 18:19:02.990162 toolsql-0.5.0/toolsql/executors/ddl_executors/drop_executors.py
+-rw-r--r--   0        0        0     4105 2023-04-12 01:56:12.421844 toolsql-0.5.0/toolsql/executors/ddl_executors/metadata_executors.py
+-rw-r--r--   0        0        0      128 2023-01-30 03:15:43.131090 toolsql-0.5.0/toolsql/executors/dml_executors/__init__.py
+-rw-r--r--   0        0        0     2584 2023-03-28 19:49:02.476403 toolsql-0.5.0/toolsql/executors/dml_executors/delete_executors.py
+-rw-r--r--   0        0        0     3409 2023-03-21 23:26:17.745727 toolsql-0.5.0/toolsql/executors/dml_executors/insert_executors.py
+-rw-r--r--   0        0        0    19701 2023-04-12 01:58:15.422563 toolsql-0.5.0/toolsql/executors/dml_executors/select_executors.py
+-rw-r--r--   0        0        0     2843 2023-02-12 04:21:29.361650 toolsql-0.5.0/toolsql/executors/dml_executors/update_executors.py
+-rw-r--r--   0        0        0       59 2023-02-26 07:01:46.454118 toolsql-0.5.0/toolsql/executors/summary_executors/__init__.py
+-rw-r--r--   0        0        0     3424 2023-03-28 18:23:04.706576 toolsql-0.5.0/toolsql/executors/summary_executors/summary_prints.py
+-rw-r--r--   0        0        0     2201 2023-02-12 02:23:37.024146 toolsql-0.5.0/toolsql/executors/summary_executors/summary_usage.py
+-rw-r--r--   0        0        0      102 2023-02-26 22:29:04.008347 toolsql-0.5.0/toolsql/formats/__init__.py
+-rw-r--r--   0        0        0     4144 2023-04-11 15:35:31.235749 toolsql-0.5.0/toolsql/formats/encoding_format_utils.py
+-rw-r--r--   0        0        0     2045 2023-04-11 15:35:17.654255 toolsql-0.5.0/toolsql/formats/json_format_utils.py
+-rw-r--r--   0        0        0     5533 2023-04-11 15:35:06.683633 toolsql-0.5.0/toolsql/formats/row_format_utils.py
+-rw-r--r--   0        0        0        0 2023-02-01 00:04:45.871374 toolsql-0.5.0/toolsql/py.typed
+-rw-r--r--   0        0        0       61 2023-01-27 04:00:11.947543 toolsql-0.5.0/toolsql/schemas/__init__.py
+-rw-r--r--   0        0        0     4240 2023-02-26 21:30:57.707911 toolsql-0.5.0/toolsql/schemas/datatype_utils.py
+-rw-r--r--   0        0        0     5427 2023-03-28 20:11:21.623102 toolsql-0.5.0/toolsql/schemas/shorthand_utils.py
+-rw-r--r--   0        0        0      147 2023-03-05 04:53:25.455675 toolsql-0.5.0/toolsql/spec/__init__.py
+-rw-r--r--   0        0        0     1184 2023-03-05 07:23:00.086051 toolsql-0.5.0/toolsql/spec/exceptions.py
+-rw-r--r--   0        0        0     2130 2023-03-06 07:52:30.415917 toolsql-0.5.0/toolsql/spec/typedata.py
+-rw-r--r--   0        0        0      148 2023-03-27 21:12:23.119118 toolsql-0.5.0/toolsql/spec/typedefs/__init__.py
+-rw-r--r--   0        0        0      234 2023-01-25 21:23:06.637935 toolsql-0.5.0/toolsql/spec/typedefs/dataset_types.py
+-rw-r--r--   0        0        0     1504 2023-02-12 00:16:22.417559 toolsql-0.5.0/toolsql/spec/typedefs/driver_types.py
+-rw-r--r--   0        0        0      109 2023-03-27 20:31:11.573302 toolsql-0.5.0/toolsql/spec/typedefs/permission_types.py
+-rw-r--r--   0        0        0     3931 2023-03-16 07:48:08.417256 toolsql-0.5.0/toolsql/spec/typedefs/schema_types.py
+-rw-r--r--   0        0        0     5568 2023-04-11 15:36:02.595008 toolsql-0.5.0/toolsql/spec/typedefs/statement_types.py
+-rw-r--r--   0        0        0     2645 2023-04-11 15:34:42.673529 toolsql-0.5.0/toolsql/spec/typeguards.py
+-rw-r--r--   0        0        0      125 2023-02-03 22:03:30.312085 toolsql-0.5.0/toolsql/statements/__init__.py
+-rw-r--r--   0        0        0       96 2023-01-30 01:01:07.284310 toolsql-0.5.0/toolsql/statements/ddl_statements/__init__.py
+-rw-r--r--   0        0        0     2631 2023-02-01 20:55:53.683307 toolsql-0.5.0/toolsql/statements/ddl_statements/alter_statements.py
+-rw-r--r--   0        0        0     7916 2023-03-01 07:30:44.368247 toolsql-0.5.0/toolsql/statements/ddl_statements/create_statements.py
+-rw-r--r--   0        0        0      636 2023-02-01 20:52:53.962533 toolsql-0.5.0/toolsql/statements/ddl_statements/drop_statements.py
+-rw-r--r--   0        0        0      132 2023-01-30 01:01:54.106030 toolsql-0.5.0/toolsql/statements/dml_statements/__init__.py
+-rw-r--r--   0        0        0     1712 2023-02-13 08:35:53.659371 toolsql-0.5.0/toolsql/statements/dml_statements/delete_statements.py
+-rw-r--r--   0        0        0     6978 2023-02-27 06:35:28.865971 toolsql-0.5.0/toolsql/statements/dml_statements/insert_statements.py
+-rw-r--r--   0        0        0     4472 2023-02-13 08:35:08.066374 toolsql-0.5.0/toolsql/statements/dml_statements/select_statements.py
+-rw-r--r--   0        0        0     3280 2023-02-13 08:35:26.310154 toolsql-0.5.0/toolsql/statements/dml_statements/update_statements.py
+-rw-r--r--   0        0        0    13142 2023-03-07 06:06:56.187816 toolsql-0.5.0/toolsql/statements/statement_utils.py
+-rw-r--r--   0        0        0     1509 2023-02-04 01:31:44.402064 toolsql-0.5.0/toolsql/statements/summary_statements.py
+-rw-r--r--   0        0        0     5087 1970-01-01 00:00:00.000000 toolsql-0.5.0/PKG-INFO
```

### Comparing `toolsql-0.3.9/LICENSE` & `toolsql-0.5.0/LICENSE`

 * *Files identical despite different names*

