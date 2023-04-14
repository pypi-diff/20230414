# Comparing `tmp/dbt-exasol-1.2.2.tar.gz` & `tmp/dbt_exasol-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-exasol-1.2.2.tar", max compression
+gzip compressed data, was "dbt_exasol-1.3.0.tar", max compression
```

## Comparing `dbt-exasol-1.2.2.tar` & `dbt_exasol-1.3.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
--rwxr-xr-x   0        0        0    35148 2021-12-30 07:56:19.472113 dbt-exasol-1.2.2/LICENSE
--rw-r--r--   0        0        0     3455 2023-01-24 15:11:49.122912 dbt-exasol-1.2.2/README.md
--rw-r--r--   0        0        0       65 2022-10-31 12:37:40.605136 dbt-exasol-1.2.2/dbt/__init__.py
--rw-r--r--   0        0        0       65 2022-10-31 12:37:40.605307 dbt-exasol-1.2.2/dbt/adapters/__init__.py
--rw-r--r--   0        0        0      508 2022-09-24 11:49:10.227324 dbt-exasol-1.2.2/dbt/adapters/exasol/__init__.py
--rw-r--r--   0        0        0     3681 2022-12-14 10:37:34.597997 dbt-exasol-1.2.2/dbt/adapters/exasol/column.py
--rw-r--r--   0        0        0    10068 2022-12-16 13:31:04.000370 dbt-exasol-1.2.2/dbt/adapters/exasol/connections.py
--rw-r--r--   0        0        0     2511 2022-12-14 10:37:34.598589 dbt-exasol-1.2.2/dbt/adapters/exasol/impl.py
--rw-r--r--   0        0        0     1921 2022-12-14 10:37:34.598887 dbt-exasol-1.2.2/dbt/adapters/exasol/relation.py
--rw-r--r--   0        0        0       65 2022-10-31 12:37:40.606232 dbt-exasol-1.2.2/dbt/include/__init__.py
--rw-r--r--   0        0        0       52 2022-10-31 12:37:40.606685 dbt-exasol-1.2.2/dbt/include/exasol/__init__.py
--rwxr-xr-x   0        0        0      236 2021-12-30 07:56:19.481658 dbt-exasol-1.2.2/dbt/include/exasol/__pycache__/__init__.cpython-37.pyc
--rwxr-xr-x   0        0        0       74 2021-12-30 07:56:19.482361 dbt-exasol-1.2.2/dbt/include/exasol/dbt_project.yml
--rw-r--r--   0        0        0     6477 2022-12-07 16:58:00.738597 dbt-exasol-1.2.2/dbt/include/exasol/macros/adapters.sql
--rw-r--r--   0        0        0      673 2022-09-24 11:49:10.228097 dbt-exasol-1.2.2/dbt/include/exasol/macros/apply_grants.sql
--rwxr-xr-x   0        0        0     1458 2021-12-30 07:56:19.483484 dbt-exasol-1.2.2/dbt/include/exasol/macros/catalog.sql
--rw-r--r--   0        0        0     3284 2022-12-16 09:41:59.477995 dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/incremental.sql
--rwxr-xr-x   0        0        0      470 2021-12-30 07:56:19.484675 dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/seed.sql
--rw-r--r--   0        0        0     8044 2022-12-14 10:37:34.599267 dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/snapshot.sql
--rw-r--r--   0        0        0      748 2022-09-23 10:36:06.838210 dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/snapshot_merge.sql
--rw-r--r--   0        0        0     3258 2022-09-23 10:36:06.838410 dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/strategies.sql
--rw-r--r--   0        0        0     3524 2022-09-24 11:49:10.228417 dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/table.sql
--rwxr-xr-x   0        0        0      119 2021-12-30 07:56:19.493246 dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/view.sql
--rw-r--r--   0        0        0      178 2022-09-24 11:49:10.228609 dbt-exasol-1.2.2/dbt/include/exasol/macros/utils/any_value.sql
--rw-r--r--   0        0        0       85 2022-09-24 11:49:10.228793 dbt-exasol-1.2.2/dbt/include/exasol/macros/utils/bool_or.sql
--rw-r--r--   0        0        0      469 2022-12-16 13:31:04.000664 dbt-exasol-1.2.2/dbt/include/exasol/macros/utils/dateadd.sql
--rw-r--r--   0        0        0      441 2022-12-16 13:31:04.000941 dbt-exasol-1.2.2/dbt/include/exasol/macros/utils/datediff.sql
--rw-r--r--   0        0        0      130 2022-09-24 11:49:10.229328 dbt-exasol-1.2.2/dbt/include/exasol/macros/utils/hash.sql
--rw-r--r--   0        0        0      381 2022-12-16 13:31:04.001125 dbt-exasol-1.2.2/dbt/include/exasol/macros/utils/last_day.sql
--rw-r--r--   0        0        0      415 2022-12-16 13:31:04.001433 dbt-exasol-1.2.2/dbt/include/exasol/macros/utils/listagg.sql
--rw-r--r--   0        0        0      775 2022-09-24 11:49:10.229642 dbt-exasol-1.2.2/dbt/include/exasol/macros/utils/safe_cast.sql
--rw-r--r--   0        0        0      165 2022-09-24 11:49:10.229792 dbt-exasol-1.2.2/dbt/include/exasol/macros/utils/split_part.sql
--rw-r--r--   0        0        0      893 2023-01-24 15:11:49.123239 dbt-exasol-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      606 2022-12-16 13:31:04.001747 dbt-exasol-1.2.2/tests/conftest.py
--rw-r--r--   0        0        0     7729 2022-12-16 13:31:04.002171 dbt-exasol-1.2.2/tests/functional/adapter/expected_catalog.py
--rw-r--r--   0        0        0     1438 2022-12-16 13:31:04.002327 dbt-exasol-1.2.2/tests/functional/adapter/files.py
--rw-r--r--   0        0        0      521 2022-12-16 13:31:04.002657 dbt-exasol-1.2.2/tests/functional/adapter/fixtures.py
--rw-r--r--   0        0        0     2580 2022-12-16 13:31:04.002996 dbt-exasol-1.2.2/tests/functional/adapter/test_basic.py
--rw-r--r--   0        0        0    12762 2022-12-16 13:31:04.003280 dbt-exasol-1.2.2/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0        0        0     2068 2022-12-16 13:31:04.003462 dbt-exasol-1.2.2/tests/functional/adapter/test_failing_test.py
--rw-r--r--   0        0        0     1366 2022-12-16 13:31:04.003824 dbt-exasol-1.2.2/tests/functional/adapter/utils/data_types/test_data_types.py
--rw-r--r--   0        0        0      591 2022-12-16 13:31:04.004049 dbt-exasol-1.2.2/tests/functional/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0        0        0    12053 2022-12-16 13:31:04.004617 dbt-exasol-1.2.2/tests/functional/adapter/utils/test_utils.py
--rw-r--r--   0        0        0    14496 2022-12-16 13:31:04.004949 dbt-exasol-1.2.2/tests/functional/adapter/utils/utils_fixtures.py
--rw-r--r--   0        0        0      932 2022-12-14 10:37:34.600981 dbt-exasol-1.2.2/tests/functional/test_grants.py
--rw-r--r--   0        0        0     8096 2022-12-14 12:35:07.724147 dbt-exasol-1.2.2/tests/functional/test_incremental.py
--rw-r--r--   0        0        0     1465 2022-12-09 10:46:24.315528 dbt-exasol-1.2.2/tests/functional/test_issues.py
--rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 dbt-exasol-1.2.2/setup.py
--rw-r--r--   0        0        0     4215 1970-01-01 00:00:00.000000 dbt-exasol-1.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0    35148 2021-12-30 07:56:19.472113 dbt_exasol-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2366 2023-04-14 08:24:45.854787 dbt_exasol-1.3.0/README.md
+-rw-r--r--   0        0        0       65 2022-10-31 12:37:40.605136 dbt_exasol-1.3.0/dbt/__init__.py
+-rw-r--r--   0        0        0       65 2022-10-31 12:37:40.605307 dbt_exasol-1.3.0/dbt/adapters/__init__.py
+-rw-r--r--   0        0        0      508 2022-09-24 11:49:10.227324 dbt_exasol-1.3.0/dbt/adapters/exasol/__init__.py
+-rw-r--r--   0        0        0     3681 2023-04-14 08:24:39.818253 dbt_exasol-1.3.0/dbt/adapters/exasol/column.py
+-rw-r--r--   0        0        0    10262 2023-04-14 08:24:45.855156 dbt_exasol-1.3.0/dbt/adapters/exasol/connections.py
+-rw-r--r--   0        0        0     2808 2023-04-14 08:24:45.855514 dbt_exasol-1.3.0/dbt/adapters/exasol/impl.py
+-rw-r--r--   0        0        0     1921 2023-04-14 08:24:39.820270 dbt_exasol-1.3.0/dbt/adapters/exasol/relation.py
+-rw-r--r--   0        0        0       65 2022-10-31 12:37:40.606232 dbt_exasol-1.3.0/dbt/include/__init__.py
+-rw-r--r--   0        0        0       52 2022-10-31 12:37:40.606685 dbt_exasol-1.3.0/dbt/include/exasol/__init__.py
+-rwxr-xr-x   0        0        0      236 2021-12-30 07:56:19.481658 dbt_exasol-1.3.0/dbt/include/exasol/__pycache__/__init__.cpython-37.pyc
+-rwxr-xr-x   0        0        0       74 2021-12-30 07:56:19.482361 dbt_exasol-1.3.0/dbt/include/exasol/dbt_project.yml
+-rw-r--r--   0        0        0     6477 2023-04-14 08:24:39.820776 dbt_exasol-1.3.0/dbt/include/exasol/macros/adapters.sql
+-rw-r--r--   0        0        0      673 2022-09-24 11:49:10.228097 dbt_exasol-1.3.0/dbt/include/exasol/macros/apply_grants.sql
+-rwxr-xr-x   0        0        0     1458 2021-12-30 07:56:19.483484 dbt_exasol-1.3.0/dbt/include/exasol/macros/catalog.sql
+-rw-r--r--   0        0        0     4239 2023-04-14 08:24:45.855768 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/incremental.sql
+-rw-r--r--   0        0        0      259 2023-04-14 08:24:45.855900 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0        0        0      997 2023-04-14 08:24:45.856031 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/merge.sql
+-rwxr-xr-x   0        0        0      470 2021-12-30 07:56:19.484675 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/seed.sql
+-rw-r--r--   0        0        0     8044 2022-12-14 10:37:34.599267 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/snapshot.sql
+-rw-r--r--   0        0        0      748 2022-09-23 10:36:06.838210 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0        0        0     3258 2023-04-05 08:18:56.802378 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/strategies.sql
+-rw-r--r--   0        0        0     3524 2023-04-02 07:58:27.134719 dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/table.sql
+-rw-r--r--   0        0        0      178 2022-09-24 11:49:10.228609 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/any_value.sql
+-rw-r--r--   0        0        0       85 2022-09-24 11:49:10.228793 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/bool_or.sql
+-rw-r--r--   0        0        0      469 2023-04-05 08:14:10.615503 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0      441 2023-04-04 22:40:13.470680 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      130 2022-09-24 11:49:10.229328 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/hash.sql
+-rw-r--r--   0        0        0      381 2023-04-03 10:32:45.345850 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      415 2023-04-05 08:14:16.076524 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      775 2022-09-24 11:49:10.229642 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/safe_cast.sql
+-rw-r--r--   0        0        0      165 2023-04-04 22:33:31.780189 dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/split_part.sql
+-rw-r--r--   0        0        0      898 2023-04-14 08:24:45.857180 dbt_exasol-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      606 2023-04-03 10:32:45.347355 dbt_exasol-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     7729 2023-04-03 10:32:45.347626 dbt_exasol-1.3.0/tests/functional/adapter/expected_catalog.py
+-rw-r--r--   0        0        0     1438 2023-04-03 10:32:45.347717 dbt_exasol-1.3.0/tests/functional/adapter/files.py
+-rw-r--r--   0        0        0      521 2023-04-03 10:32:45.347798 dbt_exasol-1.3.0/tests/functional/adapter/fixtures.py
+-rw-r--r--   0        0        0     2708 2023-04-03 10:32:45.347983 dbt_exasol-1.3.0/tests/functional/adapter/test_basic.py
+-rw-r--r--   0        0        0     1255 2023-04-03 10:32:45.348130 dbt_exasol-1.3.0/tests/functional/adapter/test_concurrency.py
+-rw-r--r--   0        0        0    12762 2023-04-03 10:32:45.348333 dbt_exasol-1.3.0/tests/functional/adapter/test_docs_generate.py
+-rw-r--r--   0        0        0      457 2023-04-03 10:32:45.348436 dbt_exasol-1.3.0/tests/functional/adapter/test_ephemeral.py
+-rw-r--r--   0        0        0     2068 2023-04-03 10:32:45.348518 dbt_exasol-1.3.0/tests/functional/adapter/test_failing_test.py
+-rw-r--r--   0        0        0     1406 2023-04-14 08:24:39.823789 dbt_exasol-1.3.0/tests/functional/adapter/utils/data_types/test_data_types.py
+-rw-r--r--   0        0        0      591 2023-04-05 08:20:04.514413 dbt_exasol-1.3.0/tests/functional/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0        0        0    12256 2023-04-14 08:24:39.824139 dbt_exasol-1.3.0/tests/functional/adapter/utils/test_utils.py
+-rw-r--r--   0        0        0    14496 2023-04-03 10:32:45.349250 dbt_exasol-1.3.0/tests/functional/adapter/utils/utils_fixtures.py
+-rw-r--r--   0        0        0      932 2023-04-14 08:24:39.824767 dbt_exasol-1.3.0/tests/functional/test_grants.py
+-rw-r--r--   0        0        0     8096 2022-12-14 12:35:07.724147 dbt_exasol-1.3.0/tests/functional/test_incremental.py
+-rw-r--r--   0        0        0     1465 2022-12-09 10:46:24.315528 dbt_exasol-1.3.0/tests/functional/test_issues.py
+-rw-r--r--   0        0        0     3485 1970-01-01 00:00:00.000000 dbt_exasol-1.3.0/setup.py
+-rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 dbt_exasol-1.3.0/PKG-INFO
```

### Comparing `dbt-exasol-1.2.2/LICENSE` & `dbt_exasol-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/dbt/adapters/exasol/column.py` & `dbt_exasol-1.3.0/dbt/adapters/exasol/column.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/dbt/adapters/exasol/connections.py` & `dbt_exasol-1.3.0/dbt/adapters/exasol/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,18 @@
         )
         return self
 
     def execute(self, query, bindings: Optional[Any] = None):
         """executing query"""
         if query.startswith("0CSV|"):
             self.import_from_file(bindings, query.split("|", 1)[1])  # type: ignore
+        elif query.__contains__("|SEPARATEMEPLEASE|"):
+            sqls = query.split("|SEPARATEMEPLEASE|")
+            for sql in sqls:
+                self.stmt = self.connection.execute(sql)
         else:
             self.stmt = self.connection.execute(query)
         return self
 
     def fetchone(self):
         """fetch single row"""
         if self.stmt is None:
```

### Comparing `dbt-exasol-1.2.2/dbt/adapters/exasol/impl.py` & `dbt_exasol-1.3.0/dbt/adapters/exasol/impl.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from typing import Dict, Optional
 
 import agate
 from dbt.adapters.sql import SQLAdapter
 from dbt.exceptions import raise_compiler_error
 from dbt.utils import filter_null_values
 
-from dbt.adapters.exasol import ExasolColumn, ExasolConnectionManager, ExasolRelation
+from dbt.adapters.exasol import (ExasolColumn, ExasolConnectionManager,
+                                 ExasolRelation)
 
 
 class ExasolAdapter(SQLAdapter):
     """Exasol SQLAdapter extension"""
 
     Relation = ExasolRelation
     Column = ExasolColumn
@@ -75,7 +76,13 @@
                 f'The seed configuration value of "quote_columns" has an '
                 f"invalid type {type(quote_config)}"
             )
 
         if quote_columns:
             return self.quote(column)
         return column
+
+    def valid_incremental_strategies(self):
+        """The set of standard builtin strategies which this adapter supports out-of-the-box.
+        Not used to validate custom strategies defined by end users.
+        """
+        return ["append", "delete+insert"]
```

### Comparing `dbt-exasol-1.2.2/dbt/adapters/exasol/relation.py` & `dbt_exasol-1.3.0/dbt/adapters/exasol/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/dbt/include/exasol/macros/adapters.sql` & `dbt_exasol-1.3.0/dbt/include/exasol/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/dbt/include/exasol/macros/apply_grants.sql` & `dbt_exasol-1.3.0/dbt/include/exasol/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/dbt/include/exasol/macros/catalog.sql` & `dbt_exasol-1.3.0/dbt/include/exasol/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/incremental.sql` & `dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/table.sql`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,81 @@
-{% macro incremental_delete(target_relation, tmp_relation) -%}
-  {%- set unique_key = config.get('unique_key') -%}
-
-  {% if unique_key %}
-    {% if unique_key is sequence and unique_key is not string %}
-        delete from {{ target_relation }}
-        where exists (select 1 from {{ tmp_relation }}
-            where
-            {% for key in unique_key %}
-                {{ tmp_relation }}.{{ key }} = {{ target_relation }}.{{ key }}
-                {{ "and " if not loop.last }}
-            {% endfor %}
-        );
-    {% else %}
-        delete from {{ target_relation }}
-        where (
-            {{ unique_key }}) in (
-            select ({{ unique_key }})
-            from {{ tmp_relation }}
-        );
-    {% endif %}
-  {%endif%}
-{%- endmacro %}
-
-{% macro incremental_insert(tmp_relation, target_relation, unique_key=none, statement_name="main") %}
-    {%- set dest_columns = adapter.get_columns_in_relation(target_relation) -%}
-    {%- set dest_cols_csv = dest_columns | join(', ', attribute='name')  -%}
-
-    insert into {{ target_relation }} ({{ dest_cols_csv }})
-    (
-       select {{ dest_cols_csv }}
-       from {{ tmp_relation.schema }}.{{ tmp_relation.identifier }}
-    );
-{%- endmacro %}
+{% materialization table, adapter='exasol' %}
+  {%- set identifier = model['alias'] -%}
+  {%- set tmp_identifier = model['name'] + '__dbt_tmp' -%}
+  {%- set backup_identifier = model['name'] + '__dbt_backup' -%}
 
+  {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
+  {%- set target_relation = api.Relation.create(identifier=identifier,
+                                                schema=schema,
+                                                database=database, type='table') -%}
+  {%- set intermediate_relation = api.Relation.create(identifier=tmp_identifier,
+                                                      schema=schema,
+                                                      database=database, type='table') -%}
+
+  /*
+      See ../view/view.sql for more information about this relation.
+  */
+
+  -- drop the backup relation if it exists, then make a new one that uses the old relation's type
+  {%- set backup_relation = adapter.get_relation(database=database, schema=schema, identifier=backup_identifier) -%}
+
+  {% if backup_relation is not none -%}
+    {{ adapter.drop_relation(backup_relation) }}
+  {%- endif %}
+  {%- set backup_relation_type = 'table' if old_relation is none else old_relation.type -%}
+  {%- set backup_relation = api.Relation.create(identifier=backup_identifier,
+                                                schema=schema,
+                                                database=database,
+                                                type=backup_relation_type) -%}
 
-{% materialization incremental, adapter='exasol' -%}
-
-  {%- set unique_key = config.get('unique_key') -%}
-  {%- set full_refresh_mode = (flags.FULL_REFRESH == True) -%}
-  {%- set identifier = model['alias'] -%}
-  {%- set target_relation = api.Relation.create(identifier=identifier, schema=schema, database=database,  type='table') -%}
-  {% set existing_relation = adapter.get_relation(database=database, schema=schema, identifier = identifier) %}
-  {% set tmp_relation = make_temp_relation(target_relation) %}
+  {%- set exists_as_table = (old_relation is not none and old_relation.is_table) -%}
+  {%- set exists_as_view = (old_relation is not none and old_relation.is_view) -%}
 
   -- grab current tables grants config for comparision later on
   {%- set grant_config = config.get('grants') -%}
 
-  -- setup
+  -- drop the temp relations if they exists for some reason
+  {{ adapter.drop_relation(intermediate_relation) }}
+
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
   -- `BEGIN` happens here:
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
-  {% if existing_relation is none %}
-    {% set build_sql = create_table_as(False, target_relation, sql) %}
-  {% elif existing_relation.is_view %}
-    {% do adapter.drop_relation(existing_relation) %}
-    {% set build_sql = create_table_as(False, target_relation, sql) %}
-  {% elif full_refresh_mode %}
-    {% do drop_relation(existing_relation) %}
-    {% set build_sql = create_table_as(False, target_relation, sql) %}
-  {% else %}
-    {% do run_query(create_table_as(True, tmp_relation, sql)) %}
-    {% do run_query(incremental_delete(target_relation, tmp_relation)) %}
-    {% set build_sql = incremental_insert(tmp_relation, target_relation) %}
+  -- build model
+  {% call statement('main') -%}
+    {{ create_table_as(False, intermediate_relation, sql) }}
+  {%- endcall %}
+
+  -- cleanup
+  {% if old_relation is not none %}
+    {% if old_relation.type == 'view' %}
+      {#-- This is the primary difference between Snowflake and Redshift. Renaming this view
+        -- would cause an error if the view has become invalid due to upstream schema changes #}
+      {{ log("Dropping relation " ~ old_relation ~ " because it is a view and this model is a table.") }}
+      {{ drop_relation_if_exists(old_relation) }}
+    {% else %}
+      {{ adapter.rename_relation(target_relation, backup_relation) }}
+    {% endif %}
   {% endif %}
 
-  
-  {%- call statement('main') -%}
-    {{ build_sql }}
-  {%- endcall -%}
+  {{ drop_relation_if_exists(target_relation) }}
+  {{ adapter.rename_relation(intermediate_relation, target_relation) }}
 
-  {% if tmp_relation is not none %}
-    {% do adapter.drop_relation(tmp_relation) %}
-  {% endif %}
-  
   {{ run_hooks(post_hooks, inside_transaction=True) }}
 
   {% set should_revoke = should_revoke(existing_relation, full_refresh_mode=full_refresh_mode) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
 
   -- `COMMIT` happens here
   {{ adapter.commit() }}
 
+  -- finally, drop the existing/backup relation after the commit
+  {{ drop_relation_if_exists(backup_relation) }}
+  {{ drop_relation_if_exists(intermediate_relation) }}
+
   {{ run_hooks(post_hooks, inside_transaction=False) }}
 
-  {% do persist_docs(target_relation, model) %}
+  {{ persist_docs(target_relation, model) }}
 
   {{ return({'relations': [target_relation]}) }}
-{%- endmaterialization %}
+{% endmaterialization %}
```

### Comparing `dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/snapshot.sql` & `dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/snapshot_merge.sql` & `dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/dbt/include/exasol/macros/materializations/strategies.sql` & `dbt_exasol-1.3.0/dbt/include/exasol/macros/materializations/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/dbt/include/exasol/macros/utils/safe_cast.sql` & `dbt_exasol-1.3.0/dbt/include/exasol/macros/utils/safe_cast.sql`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/pyproject.toml` & `dbt_exasol-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "dbt-exasol"
-version = "1.2.2"
+version = "1.3.0"
 description = "Adapter to dbt-core for warehouse Exasol"
 authors = ["Torsten Glunde <torsten.glunde@alligator-company.com>", "Ilija Kutle <ilija.kutle@alligator-company.com>"]
 homepage = "https://alligatorcompany.gitlab.io/dbt-exasol"
 repository = "https://github.com/tglunde/dbt-exasol"
 packages = [
   { include = "dbt" },
   { include = "dbt/**/*.py" },
   { include = "tests/**/*.py"}
 ]
 license = "GPL3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7.2, <4"
-dbt-core = "^1.2, <1.3"
+dbt-core = "^1.3, <1.4"
 pyexasol = "^0.25.0"
-dbt-tests-adapter = "^1.2, <1.3"
+dbt-tests-adapter = "^1.3, <1.4"
 
 [tool.poetry.dev-dependencies]
 black = "^22.8.0"
 pytest = "^7.1.3"
 pytest-dotenv = "^0.5.2"
 tox = "^3.26.0"
 
 [tool.poetry.group.dev.dependencies]
-dbt-tests-adapter = "^1.2.1"
+dbt-tests-adapter = "^1.3.2"
 pylint = "^2.15.8"
+pytest-parallel = "^0.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dbt-exasol-1.2.2/tests/conftest.py` & `dbt_exasol-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/tests/functional/adapter/expected_catalog.py` & `dbt_exasol-1.3.0/tests/functional/adapter/expected_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/tests/functional/adapter/files.py` & `dbt_exasol-1.3.0/tests/functional/adapter/files.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/tests/functional/adapter/fixtures.py` & `dbt_exasol-1.3.0/tests/functional/adapter/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/tests/functional/adapter/test_basic.py` & `dbt_exasol-1.3.0/tests/functional/adapter/test_basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest, os
 
 from dbt.tests.adapter.basic.test_adapter_methods import BaseAdapterMethod
 from dbt.tests.adapter.basic.test_base import BaseSimpleMaterializations
 from dbt.tests.adapter.basic.test_empty import BaseEmpty
 from dbt.tests.adapter.basic.test_ephemeral import BaseEphemeral
 from dbt.tests.adapter.basic.test_generic_tests import BaseGenericTests
-from dbt.tests.adapter.basic.test_incremental import BaseIncremental
+from dbt.tests.adapter.basic.test_incremental import BaseIncremental, BaseIncrementalNotSchemaChange
 from dbt.tests.adapter.basic.test_singular_tests import BaseSingularTests
 from dbt.tests.adapter.basic.test_singular_tests_ephemeral import (
     BaseSingularTestsEphemeral,
 )
 from dbt.tests.adapter.basic.test_snapshot_check_cols import BaseSnapshotCheckCols
 from dbt.tests.adapter.basic.test_snapshot_timestamp import BaseSnapshotTimestamp
 from dbt.tests.adapter.basic.test_validate_connection import BaseValidateConnection
@@ -48,15 +48,15 @@
     pass
 
 
 class TestSnapshotTimestampExasol(BaseSnapshotTimestamp):
     pass
 
 
-class TestBaseAdapterMethod(BaseAdapterMethod):
+class TestBaseAdapterMethodExasol(BaseAdapterMethod):
     pass
 
 
 class TestBaseCachingExasol(BaseAdapterMethod):
     pass
 
 
@@ -84,8 +84,11 @@
            "type": "exasol",
            "threads": 1,
            "dsn": os.getenv('DBT_DSN',"localhost:8563"),
            "user": os.getenv('DBT_USER',"sys"),
            "pass": os.getenv('DBT_PASS',"exasol"),
            "dbname": "DB",
            "timestamp_format": "YYYY-MM-DD HH:MI:SS.FF6"
-        }
+        }
+
+class TestBaseIncrementalNotSchemaChangeExasol(BaseIncrementalNotSchemaChange):
+    pass
```

### Comparing `dbt-exasol-1.2.2/tests/functional/adapter/test_docs_generate.py` & `dbt_exasol-1.3.0/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/tests/functional/adapter/test_failing_test.py` & `dbt_exasol-1.3.0/tests/functional/adapter/test_failing_test.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/tests/functional/adapter/utils/data_types/test_data_types.py` & `dbt_exasol-1.3.0/tests/functional/adapter/utils/data_types/test_data_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,46 +2,47 @@
 #from dbt.tests.adapter.utils.data_types.test_type_bigint import BaseTypeBigInt
 from dbt.tests.adapter.utils.data_types.test_type_float import BaseTypeFloat
 from dbt.tests.adapter.utils.data_types.test_type_int import BaseTypeInt
 from dbt.tests.adapter.utils.data_types.test_type_numeric import BaseTypeNumeric
 from dbt.tests.adapter.utils.data_types.test_type_string import BaseTypeString
 from dbt.tests.adapter.utils.data_types.test_type_timestamp import BaseTypeTimestamp
 from test_type_bigint import BaseTypeBigInt
-#from dbt.tests.adapter.utils.data_types.test_type_boolean import BaseTypeBoolean
+from dbt.tests.adapter.utils.data_types.test_type_boolean import BaseTypeBoolean
 
 
-class TestTypeBigInt(BaseTypeBigInt):
+
+class TestTypeBigIntExasol(BaseTypeBigInt):
     pass
 
     
-class TestTypeFloat(BaseTypeFloat):
+class TestTypeFloatExasol(BaseTypeFloat):
     pass
 
     
-class TestTypeInt(BaseTypeInt):
+class TestTypeIntExasol(BaseTypeInt):
     pass
 
     
-class TestTypeNumeric(BaseTypeNumeric):
+class TestTypeNumericExasol(BaseTypeNumeric):
     pass
 
     
-class TestTypeString(BaseTypeString):
+class TestTypeStringExasol(BaseTypeString):
     pass
 
     
-class TestTypeTimestamp(BaseTypeTimestamp):
+class TestTypeTimestampExasol(BaseTypeTimestamp):
     @pytest.fixture(scope="class")
     def dbt_profile_target(self):
         return {
            "type": "exasol",
            "threads": 1,
            "dsn": os.getenv('DBT_DSN',"localhost:8563"),
            "user": os.getenv('DBT_USER',"sys"),
            "pass": os.getenv('DBT_PASS',"exasol"),
            "dbname": "DB",
            "timestamp_format": "YYYY-MM-DD HH:MI:SS.FF6"
         }
 
 
-#class TestTypeBoolean(BaseTypeBoolean):
-#    pass
+class TestTypeBooleanExasol(BaseTypeBoolean):
+    pass
```

### Comparing `dbt-exasol-1.2.2/tests/functional/adapter/utils/data_types/test_type_bigint.py` & `dbt_exasol-1.3.0/tests/functional/adapter/utils/data_types/test_type_bigint.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/tests/functional/adapter/utils/test_utils.py` & `dbt_exasol-1.3.0/tests/functional/adapter/utils/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 
 import pytest
+from utils_fixtures import *
 from dbt.exceptions import CompilationException
 from dbt.tests.adapter.utils.base_utils import BaseUtils
 
-# from dbt.tests.adapter.utils.test_array_append import BaseArrayAppend
-# from dbt.tests.adapter.utils.test_array_concat import BaseArrayConcat
-# from dbt.tests.adapter.utils.test_array_construct import BaseArrayConstruct
+from dbt.tests.adapter.utils.test_array_append import BaseArrayAppend
+from dbt.tests.adapter.utils.test_array_concat import BaseArrayConcat
+from dbt.tests.adapter.utils.test_array_construct import BaseArrayConstruct
 from dbt.tests.adapter.utils.test_any_value import BaseAnyValue
 from dbt.tests.adapter.utils.test_bool_or import BaseBoolOr
 from dbt.tests.adapter.utils.test_cast_bool_to_text import BaseCastBoolToText
 from dbt.tests.adapter.utils.test_concat import BaseConcat
 from dbt.tests.adapter.utils.test_date_trunc import BaseDateTrunc
 
-# from dbt.tests.adapter.utils.test_current_timestamp import BaseCurrentTimestampAware
+from dbt.tests.adapter.utils.test_current_timestamp import BaseCurrentTimestampNaive
 from dbt.tests.adapter.utils.test_dateadd import BaseDateAdd
 from dbt.tests.adapter.utils.test_datediff import BaseDateDiff
 from dbt.tests.adapter.utils.test_escape_single_quotes import (
     BaseEscapeSingleQuotesBackslash,
     BaseEscapeSingleQuotesQuote,
 )
 from dbt.tests.adapter.utils.test_except import BaseExcept
@@ -29,41 +30,43 @@
 from dbt.tests.adapter.utils.test_position import BasePosition
 from dbt.tests.adapter.utils.test_replace import BaseReplace
 from dbt.tests.adapter.utils.test_right import BaseRight
 from dbt.tests.adapter.utils.test_safe_cast import BaseSafeCast
 from dbt.tests.adapter.utils.test_split_part import BaseSplitPart
 from dbt.tests.adapter.utils.test_string_literal import BaseStringLiteral
 from dbt.tests.util import run_dbt
-from utils_fixtures import *
 
 
-class TestAnyValue(BaseAnyValue):
+class TestAnyValueExasol(BaseAnyValue):
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_any_value.yml": exasol__models__test_any_value_yml,
             "test_any_value.sql": self.interpolate_macro_namespace(
                 exasol__models__test_any_value_sql, "any_value"
             ),
         }
 
+@pytest.mark.xfail
+class TestArrayAppendExasol(BaseArrayAppend):
+    pass
 
-# class TestArrayAppend(BaseArrayAppend):
-#    pass
 
+@pytest.mark.xfail
+class TestArrayConcatExasol(BaseArrayConcat):
+    pass
 
-# class TestArrayConcat(BaseArrayConcat):
-#    pass
 
+@pytest.mark.xfail
+class TestArrayConstructExasol(BaseArrayConstruct):
+    pass
 
-# class TestArrayConstruct(BaseArrayConstruct):
-#    pass
 
 
-class TestBoolOr(BaseBoolOr):
+class TestBoolOrExasol(BaseBoolOr):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
             "data_bool_or.csv": exasol__seeds__data_bool_or_csv,
             "data_bool_or_expected.csv": exasol__seeds__data_bool_or_expected_csv,
         }
 
@@ -73,26 +76,26 @@
             "test_bool_or.yml": exasol__models__test_bool_or_yml,
             "test_bool_or.sql": self.interpolate_macro_namespace(
                 exasol__models__test_bool_or_sql, "bool_or"
             ),
         }
 
 
-class TestCastBoolToText(BaseCastBoolToText):
+class TestCastBoolToTextExasol(BaseCastBoolToText):
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_cast_bool_to_text.yml": exasol__models__test_cast_bool_to_text_yml,
             "test_cast_bool_to_text.sql": self.interpolate_macro_namespace(
                 exasol__models__test_cast_bool_to_text_sql, "cast_bool_to_text"
             ),
         }
 
 
-class TestConcat(BaseConcat):
+class TestConcatExasol(BaseConcat):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {"data_concat.csv": exasol__seeds__data_concat_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
@@ -100,31 +103,32 @@
             "test_concat.sql": self.interpolate_macro_namespace(
                 exasol__models__test_concat_sql, "concat"
             ),
         }
 
 
 # Use either BaseCurrentTimestampAware or BaseCurrentTimestampNaive but not both
-# class TestCurrentTimestamp(BaseCurrentTimestampAware):
-#    pass
+@pytest.mark.xfail
+class TestCurrentTimestampExasol(BaseCurrentTimestampNaive):
+    pass
 
 
-class TestDateAdd(BaseDateAdd):
+class TestDateAddExasol(BaseDateAdd):
     @pytest.fixture(scope="class")
     def project_config_update(self):
         return {
             "name": "test",
             # this is only needed for BigQuery, right?
             # no harm having it here until/unless there's an adapter that doesn't support the 'timestamp' type
             "seeds": {
                 "test": {
                     "data_dateadd": {
                         "+column_types": {
                             "from_time": "timestamp",
-                            "result": "timestamp",
+                            "res": "timestamp",
                         },
                     },
                 },
             },
         }
 
     @pytest.fixture(scope="class")
@@ -137,15 +141,15 @@
             "test_dateadd.yml": exasol__models__test_dateadd_yml,
             "test_dateadd.sql": self.interpolate_macro_namespace(
                 exasol__models__test_dateadd_sql, "dateadd"
             ),
         }
 
 
-class TestDateDiff(BaseDateDiff):
+class TestDateDiffExasol(BaseDateDiff):
     @pytest.fixture(scope="class")
     def dbt_profile_target(self):
         return {
             "type": "exasol",
             "threads": 1,
             "dsn": os.getenv("DBT_DSN", "localhost:8563"),
             "user": os.getenv("DBT_USER", "sys"),
@@ -164,107 +168,107 @@
             "test_datediff.yml": exasol__models__test_datediff_yml,
             "test_datediff.sql": self.interpolate_macro_namespace(
                 exasol__models__test_datediff_sql, "datediff"
             ),
         }
 
 
-class TestDateTrunc(BaseDateTrunc):
+class TestDateTruncExasol(BaseDateTrunc):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {"data_date_trunc.csv": exasol__seeds__data_date_trunc_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_date_trunc.yml": exasol__models__test_date_trunc_yml,
             "test_date_trunc.sql": self.interpolate_macro_namespace(
                 exasol__models__test_date_trunc_sql, "date_trunc"
             ),
         }
 
 
-class TestEscapeSingleQuotes(BaseEscapeSingleQuotesBackslash):
+class TestEscapeSingleQuotesExasol(BaseEscapeSingleQuotesBackslash):
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_escape_single_quotes.yml": exasol__models__test_escape_single_quotes_yml,
             "test_escape_single_quotes.sql": self.interpolate_macro_namespace(
                 exasol__models__test_escape_single_quotes_quote_sql,
                 "escape_single_quotes",
             ),
         }
 
 
-class BaseEscapeSingleQuotesBackslash(BaseUtils):
+class BaseEscapeSingleQuotesBackslashExasol(BaseUtils):
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_escape_single_quotes.yml": exasol__models__test_escape_single_quotes_yml,
             "test_escape_single_quotes.sql": self.interpolate_macro_namespace(
                 exasol__models__test_escape_single_quotes_backslash_sql,
                 "escape_single_quotes",
             ),
         }
 
 
-class TestExcept(BaseExcept):
+class TestExceptExasol(BaseExcept):
     pass
 
 
-class TestHash(BaseHash):
+class TestHashExasol(BaseHash):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {"data_hash.csv": exasol__seeds__data_hash_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_hash.yml": exasol__models__test_hash_yml,
             "test_hash.sql": self.interpolate_macro_namespace(
                 exasol__models__test_hash_sql, "hash"
             ),
         }
 
 
-class TestIntersect(BaseIntersect):
+class TestIntersectExasol(BaseIntersect):
     pass
 
 
-class TestLastDay(BaseLastDay):
+class TestLastDayExasol(BaseLastDay):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {"data_last_day.csv": exasol__seeds__data_last_day_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_last_day.yml": exasol__models__test_last_day_yml,
             "test_last_day.sql": self.interpolate_macro_namespace(
                 exasol__models__test_last_day_sql, "last_day"
             ),
         }
 
 
-class TestLength(BaseLength):
+class TestLengthExasol(BaseLength):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {"data_length.csv": exasol__seeds__data_length_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_length.yml": exasol__models__test_length_yml,
             "test_length.sql": self.interpolate_macro_namespace(
                 exasol__models__test_length_sql, "length"
             ),
         }
 
 
-class TestListagg(BaseListagg):
+class TestListaggExasol(BaseListagg):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {
             "data_listagg.csv": exasol__seeds__data_listagg_csv,
             "data_listagg_output.csv": exasol__seeds__data_listagg_output_csv,
         }
 
@@ -279,60 +283,60 @@
 
     def test_build_assert_equal(self, project):
         with pytest.raises(CompilationException) as exc_info:
             run_dbt(["build"], expect_pass=False)
         assert exc_info.value.msg == "`limit_num` parameter is not supported on Exasol!"
 
 
-class TestPosition(BasePosition):
+class TestPositionExasol(BasePosition):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {"data_position.csv": exasol__seeds__data_position_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_position.yml": exasol__models__test_position_yml,
             "test_position.sql": self.interpolate_macro_namespace(
                 exasol__models__test_position_sql, "position"
             ),
         }
 
 
-class TestReplace(BaseReplace):
+class TestReplaceExasol(BaseReplace):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {"data_replace.csv": exasol__seeds__data_replace_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_replace.yml": exasol__models__test_replace_yml,
             "test_replace.sql": self.interpolate_macro_namespace(
                 exasol__models__test_replace_sql, "replace"
             ),
         }
 
 
-class TestRight(BaseRight):
+class TestRightExasol(BaseRight):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {"data_right.csv": exasol__seeds__data_right_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "test_right.yml": exasol__models__test_right_yml,
             "test_right.sql": self.interpolate_macro_namespace(
                 exasol__models__test_right_sql, "right"
             ),
         }
 
 
-class TestSafeCast(BaseSafeCast):
+class TestSafeCastExasol(BaseSafeCast):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {"data_safe_cast.csv": exasol__seeds__data_safe_cast_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
@@ -342,15 +346,15 @@
                     exasol__models__test_safe_cast_sql, "safe_cast"
                 ),
                 "type_string",
             ),
         }
 
 
-class TestSplitPart(BaseSplitPart):
+class TestSplitPartExasol(BaseSplitPart):
     @pytest.fixture(scope="class")
     def seeds(self):
         return {"data_split_part.csv": exasol__seeds__data_split_part_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
@@ -362,9 +366,9 @@
 
     def test_build_assert_equal(self, project):
         with pytest.raises(CompilationException) as exc_info:
             run_dbt(["build"], expect_pass=False)
         assert exc_info.value.msg == "Unsupported on Exasol! Sorry..."
 
 
-class TestStringLiteral(BaseStringLiteral):
+class TestStringLiteralExasol(BaseStringLiteral):
     pass
```

### Comparing `dbt-exasol-1.2.2/tests/functional/adapter/utils/utils_fixtures.py` & `dbt_exasol-1.3.0/tests/functional/adapter/utils/utils_fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/tests/functional/test_grants.py` & `dbt_exasol-1.3.0/tests/functional/test_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/tests/functional/test_incremental.py` & `dbt_exasol-1.3.0/tests/functional/test_incremental.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/tests/functional/test_issues.py` & `dbt_exasol-1.3.0/tests/functional/test_issues.py`

 * *Files identical despite different names*

### Comparing `dbt-exasol-1.2.2/setup.py` & `dbt_exasol-1.3.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 package_data = \
 {'': ['*'],
  'dbt.include.exasol': ['macros/*',
                         'macros/materializations/*',
                         'macros/utils/*']}
 
 install_requires = \
-['dbt-core>=1.2,<1.3',
- 'dbt-tests-adapter>=1.2,<1.3',
+['dbt-core>=1.3,<1.4',
+ 'dbt-tests-adapter>=1.3,<1.4',
  'pyexasol>=0.25.0,<0.26.0']
 
 setup_kwargs = {
     'name': 'dbt-exasol',
-    'version': '1.2.2',
+    'version': '1.3.0',
     'description': 'Adapter to dbt-core for warehouse Exasol',
-    'long_description': "# dbt-exasol\n**[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.\n\nPlease see the dbt documentation on **[Exasol setup](https://docs.getdbt.com/reference/warehouse-setups/exasol-setup)** for more information on how to start using the Exasol adapter.\n\n# Current profile.yml settings\n<File name='profiles.yml'>\n\n```yaml\ndbt-exasol:\n  target: dev\n  outputs:\n    dev:\n      type: exasol\n      threads: 1\n      dsn: HOST:PORT\n      user: USERNAME\n      password: PASSWORD\n      dbname: db\n      schema: SCHEMA\n```\n\n#### Optional parameters\n<ul>\n  <li><strong>connection_timeout</strong>: defaults to pyexasol default</li>\n  <li><strong>socket_timeout</strong>: defaults to pyexasol default</li>\n  <li><strong>query_timeout</strong>: defaults to pyexasol default</li>\n  <li><strong>compression</strong>: default: False</li>\n  <li><strong>encryption</strong>: default: False</li>\n  <li><strong>protocol_version</strong>: default: v3</li>\n  <li><strong>row_separator</strong>: default: CRLF for windows - LF otherwise</li>\n  <li><strong>timestamp_format</strong>: default: YYYY-MM-DDTHH:MI:SS.FF6</li>\n</ul>\n\n# Known isues\n\n## Breaking changes with release 1.2.2\n- Timestamp format defaults to YYYY-MM-DDTHH:MI:SS.FF6\n\n## SQL functions compatibility\n\n### split_part\nThere is no equivalent SQL function in Exasol for split_part.\n\n### listagg part_num\nThe SQL function listagg in Exasol does not support the num_part parameter.\n\n## Utilities shim package\nIn order to support packages like dbt-utils and dbt-audit-helper, we needed to create the [shim package exasol-utils](https://github.com/tglunde/exasol-utils). In this shim package we need to adapt to parts of the SQL functionality that is not compatible with Exasol - e.g. when 'final' is being used which is a keyword in Exasol. Please visit [Adaopter dispatch documentation](https://docs.getdbt.com/guides/advanced/adapter-development/3-building-a-new-adapter#adapter-dispatch) of dbt-labs for more information. \n# Reporting bugs and contributing code\n- Please report bugs using the issues\n\n# Release History\n\n## Release 1.2.2\n- Added timestamp format parameter in profile.yml parameter file to set Exasol session parameter NLS_TIMESTAMP_FORMAT when opening a connection. Defaults to 'YYYY-MM-DDTHH:MI:SS.FF6' \n- Adding row_separator (LF/CRLF) parameter in profile.yml parameter file to be used in seed csv import. Defaults to operating system default (os.linesep in python).\n- bugfix #36 regarding column quotes and case sensitivity of column names. \n- bugfix #42 regarding datatype change when using snapshot materialization. Added modify column statement in exasol__alter_column_type macro\n- bugfix #17 number format datatype\n- issue #24 - dbt-core v1.2.0 compatibility finished\n\n## Release 1.2.0\n- support for invalidate_hard_deletes option in snapshots added by jups23\n- added persist_docs support by sti0\n- added additional configuration keys that can be included in profiles.yml by johannes-becker-otto\n- added cross-database macros introduced in 1.2 by sti0\n- added support for connection retries by sti0\n- added support for grants by sti0\n- added pytest functional adapter tests by tglunde\n- tox testing for python 3.7.2 through 3.10 added by tglunde\n \n## Release 1.0.0\n- pyexasol HTTP import csv feature implemented. Optimal performance and compatibility with Exasol CSV parsing\n",
+    'long_description': "# dbt-exasol\n**[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.\n\nPlease see the dbt documentation on **[Exasol setup](https://docs.getdbt.com/reference/warehouse-setups/exasol-setup)** for more information on how to start using the Exasol adapter.\n\n# Current profile.yml settings\n<File name='profiles.yml'>\n\n```yaml\ndbt-exasol:\n  target: dev\n  outputs:\n    dev:\n      type: exasol\n      threads: 1\n      dsn: HOST:PORT\n      user: USERNAME\n      password: PASSWORD\n      dbname: db\n      schema: SCHEMA\n```\n\n#### Optional parameters\n<ul>\n  <li><strong>connection_timeout</strong>: defaults to pyexasol default</li>\n  <li><strong>socket_timeout</strong>: defaults to pyexasol default</li>\n  <li><strong>query_timeout</strong>: defaults to pyexasol default</li>\n  <li><strong>compression</strong>: default: False</li>\n  <li><strong>encryption</strong>: default: False</li>\n  <li><strong>protocol_version</strong>: default: v3</li>\n  <li><strong>row_separator</strong>: default: CRLF for windows - LF otherwise</li>\n  <li><strong>timestamp_format</strong>: default: YYYY-MM-DDTHH:MI:SS.FF6</li>\n</ul>\n\n# Known isues\n\n## >=1.3 Python model not yet supported - WIP\n- Please follow [this pull request](https://github.com/tglunde/dbt-exasol/pull/59) \n\n## Breaking changes with release 1.2.2\n- Timestamp format defaults to YYYY-MM-DDTHH:MI:SS.FF6\n\n## SQL functions compatibility\n\n### split_part\nThere is no equivalent SQL function in Exasol for split_part.\n\n### listagg part_num\nThe SQL function listagg in Exasol does not support the num_part parameter.\n\n## Utilities shim package\nIn order to support packages like dbt-utils and dbt-audit-helper, we needed to create the [shim package exasol-utils](https://github.com/tglunde/exasol-utils). In this shim package we need to adapt to parts of the SQL functionality that is not compatible with Exasol - e.g. when 'final' is being used which is a keyword in Exasol. Please visit [Adaopter dispatch documentation](https://docs.getdbt.com/guides/advanced/adapter-development/3-building-a-new-adapter#adapter-dispatch) of dbt-labs for more information. \n# Reporting bugs and contributing code\n- Please report bugs using the issues\n\n# Releases\n\n[GitHub Releases](https://github.com/tglunde/dbt-exasol/releases)\n",
     'author': 'Torsten Glunde',
     'author_email': 'torsten.glunde@alligator-company.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://alligatorcompany.gitlab.io/dbt-exasol',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.2,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

