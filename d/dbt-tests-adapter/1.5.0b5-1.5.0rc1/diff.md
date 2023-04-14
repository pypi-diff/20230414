# Comparing `tmp/dbt-tests-adapter-1.5.0b5.tar.gz` & `tmp/dbt-tests-adapter-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-tests-adapter-1.5.0b5.tar", last modified: Thu Mar 30 16:56:49 2023, max compression
+gzip compressed data, was "dbt-tests-adapter-1.5.0rc1.tar", last modified: Fri Apr 14 00:23:12 2023, max compression
```

## Comparing `dbt-tests-adapter-1.5.0b5.tar` & `dbt-tests-adapter-1.5.0rc1.tar`

### file list

```diff
@@ -1,150 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.149906 dbt-tests-adapter-1.5.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-30 16:56:49.149906 dbt-tests-adapter-1.5.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.129907 dbt-tests-adapter-1.5.0b5/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.129907 dbt-tests-adapter-1.5.0b5/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.133906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.133906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/aliases/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/aliases/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/aliases/test_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.133906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/expected_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_adapter_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_docs_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_incremental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_singular_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_snapshot_check_cols.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_snapshot_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_table_materialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_validate_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/caching/
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/caching/test_caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/column_types/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/column_types/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/column_types/test_column_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/concurrency/
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/concurrency/test_concurrency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/constraints/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/constraints/test_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/dbt_debug/
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/ephemeral/
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/ephemeral/test_ephemeral.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/base_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/test_incremental_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/test_invalid_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/test_model_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/test_seed_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/test_snapshot_grants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/hooks/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/hooks/test_model_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/hooks/test_run_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/test_incremental_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    17492 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/test_incremental_unique_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/persist_docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/persist_docs/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/persist_docs/test_persist_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/python_model/test_python_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/python_model/test_spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/query_comment/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/query_comment/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/query_comment/test_query_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.137906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/relations/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/relations/test_changing_relation_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.141906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_copy/
--rw-r--r--   0 runner    (1001) docker     (123)    19865 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_copy/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_copy/test_simple_copy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.141906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_seed/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_seed/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    78093 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_seed/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_seed/test_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_seed/test_seed_type_override.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.141906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/store_test_failures_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/store_test_failures_tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.145906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/base_array_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/base_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.145906 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_any_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_array_append.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_array_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_array_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_bool_or.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_date_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_dateadd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_datediff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_except.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_last_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_listagg.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_right.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_safe_cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_split_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_any_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_array_append.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_array_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_array_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_bool_or.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_cast_bool_to_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_current_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_date_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_dateadd.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_datediff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_escape_single_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_except.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_last_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_listagg.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_right.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_safe_cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_split_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_timestamps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:56:49.149906 dbt-tests-adapter-1.5.0b5/dbt_tests_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-30 16:56:49.000000 dbt-tests-adapter-1.5.0b5/dbt_tests_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-03-30 16:56:49.000000 dbt-tests-adapter-1.5.0b5/dbt_tests_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:56:49.000000 dbt-tests-adapter-1.5.0b5/dbt_tests_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:56:49.000000 dbt-tests-adapter-1.5.0b5/dbt_tests_adapter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-30 16:56:49.000000 dbt-tests-adapter-1.5.0b5/dbt_tests_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-30 16:56:49.000000 dbt-tests-adapter-1.5.0b5/dbt_tests_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 16:56:49.149906 dbt-tests-adapter-1.5.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-30 16:56:37.000000 dbt-tests-adapter-1.5.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.795287 dbt-tests-adapter-1.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-14 00:23:12.795287 dbt-tests-adapter-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.775287 dbt-tests-adapter-1.5.0rc1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.775287 dbt-tests-adapter-1.5.0rc1/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.775287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.775287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/aliases/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/aliases/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/aliases/test_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.779287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/expected_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_adapter_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_docs_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_singular_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_snapshot_check_cols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_snapshot_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_table_materialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_validate_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.779287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/caching/test_caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.779287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/column_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/column_types/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/column_types/test_column_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.779287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/concurrency/test_concurrency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.779287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/constraints/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/constraints/test_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.779287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/dbt_debug/
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.779287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/ephemeral/
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/ephemeral/test_ephemeral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.783287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/base_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/test_incremental_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/test_invalid_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/test_model_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/test_seed_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/test_snapshot_grants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.783287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/hooks/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/hooks/test_model_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/hooks/test_run_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.783287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/test_incremental_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17492 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/test_incremental_unique_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.783287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/persist_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/persist_docs/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/persist_docs/test_persist_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.783287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/python_model/test_python_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/python_model/test_spark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.783287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/query_comment/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/query_comment/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/query_comment/test_query_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.783287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/relations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/relations/test_changing_relation_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.783287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_copy/
+-rw-r--r--   0 runner    (1001) docker     (123)    19865 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_copy/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_copy/test_simple_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.783287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_seed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_seed/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78093 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_seed/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_seed/test_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_seed/test_seed_type_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.787287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_snapshot/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_snapshot/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_snapshot/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_snapshot/test_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.787287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/store_test_failures_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/store_test_failures_tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.795287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/base_array_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/base_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.795287 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_any_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_array_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_array_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_array_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_bool_or.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_date_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_dateadd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_datediff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_except.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_last_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_listagg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_safe_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_split_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_any_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_array_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_array_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_array_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_bool_or.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_cast_bool_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_current_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_date_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_dateadd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_datediff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_escape_single_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_except.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_last_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_listagg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_safe_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_split_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_timestamps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:12.795287 dbt-tests-adapter-1.5.0rc1/dbt_tests_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-14 00:23:12.000000 dbt-tests-adapter-1.5.0rc1/dbt_tests_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-14 00:23:12.000000 dbt-tests-adapter-1.5.0rc1/dbt_tests_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:23:12.000000 dbt-tests-adapter-1.5.0rc1/dbt_tests_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:23:12.000000 dbt-tests-adapter-1.5.0rc1/dbt_tests_adapter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 00:23:12.000000 dbt-tests-adapter-1.5.0rc1/dbt_tests_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 00:23:12.000000 dbt-tests-adapter-1.5.0rc1/dbt_tests_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:23:12.795287 dbt-tests-adapter-1.5.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-14 00:23:01.000000 dbt-tests-adapter-1.5.0rc1/setup.py
```

### Comparing `dbt-tests-adapter-1.5.0b5/PKG-INFO` & `dbt-tests-adapter-1.5.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-tests-adapter
-Version: 1.5.0b5
+Version: 1.5.0rc1
 Summary: The dbt adapter tests for adapter plugins
 Home-page: https://github.com/dbt-labs/dbt-core/tree/main/tests/adapter
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-tests-adapter-1.5.0b5/README.md` & `dbt-tests-adapter-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/aliases/fixtures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/aliases/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/aliases/test_aliases.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/aliases/test_aliases.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/expected_catalog.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/expected_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/files.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/files.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_adapter_methods.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_adapter_methods.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_base.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_base.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_docs_generate.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_docs_generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,14 @@
 def verify_metadata(metadata, dbt_schema_version, start_time):
     assert "generated_at" in metadata
     check_datetime_between(metadata["generated_at"], start=start_time)
     assert "dbt_version" in metadata
     assert metadata["dbt_version"] == dbt.version.__version__
     assert "dbt_schema_version" in metadata
     assert metadata["dbt_schema_version"] == dbt_schema_version
-    assert metadata["invocation_id"] == dbt.tracking.active_user.invocation_id
     key = "env_key"
     if os.name == "nt":
         key = key.upper()
     assert metadata["env"] == {key: "env_value"}
 
 
 def run_and_generate(project, args=None):
```

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_empty.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_empty.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_ephemeral.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_generic_tests.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_incremental.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_incremental.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_singular_tests.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_singular_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_snapshot_check_cols.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_snapshot_check_cols.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_snapshot_timestamp.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_snapshot_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/basic/test_table_materialization.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/basic/test_table_materialization.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/caching/test_caching.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/caching/test_caching.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,14 +87,28 @@
 
     def test_cache(self, project):
         # this should only cache the schema containing the selected model
         run_args = ["--cache-selected-only", "run", "--select", "model"]
         self.run_and_inspect_cache(project, run_args)
 
 
+class TestNoPopulateCache(BaseCachingTest):
+    @pytest.fixture(scope="class")
+    def models(self):
+        return {
+            "model.sql": model_sql,
+        }
+
+    def test_cache(self, project):
+        # --no-populate-cache still allows the cache to populate all relations
+        # under a schema, so the behavior here remains the same as other tests
+        run_args = ["--no-populate-cache", "run"]
+        self.run_and_inspect_cache(project, run_args)
+
+
 class TestCachingLowerCaseModel(BaseCachingLowercaseModel):
     pass
 
 
 class TestCachingUppercaseModel(BaseCachingUppercaseModel):
     pass
```

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/column_types/fixtures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/column_types/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/column_types/test_column_types.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/column_types/test_column_types.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/concurrency/test_concurrency.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/concurrency/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/constraints/fixtures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/constraints/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,14 +257,45 @@
           - unique
       - name: color
         data_type: text
       - name: date_day
         data_type: text
 """
 
+constrained_model_schema_yml = """
+version: 2
+models:
+  - name: my_model
+    config:
+      contract:
+        enforced: true
+    constraints:
+      - type: check
+        expression: (id > 0)
+      - type: primary_key
+        columns: [ id ]
+      - type: unique
+        columns: [ color, date_day ]
+        name: strange_uniqueness_requirement
+    columns:
+      - name: id
+        quote: true
+        data_type: integer
+        description: hello
+        constraints:
+          - type: not_null
+        tests:
+          - unique
+      - name: color
+        data_type: text
+      - name: date_day
+        data_type: text
+"""
+
+
 model_data_type_schema_yml = """
 version: 2
 models:
   - name: my_model_data_type
     config:
       contract:
         enforced: true
```

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/constraints/test_constraints.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/constraints/test_constraints.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     my_model_view_wrong_order_sql,
     my_model_view_wrong_name_sql,
     my_model_incremental_wrong_order_sql,
     my_model_incremental_wrong_name_sql,
     my_model_with_nulls_sql,
     my_model_incremental_with_nulls_sql,
     model_schema_yml,
+    constrained_model_schema_yml,
 )
 
 
 class BaseConstraintsColumnsEqual:
     """
     dbt should catch these mismatches during its "preflight" checks.
     """
@@ -37,14 +38,18 @@
         return "TEXT"
 
     @pytest.fixture
     def int_type(self):
         return "INT"
 
     @pytest.fixture
+    def schema_string_type(self, string_type):
+        return string_type
+
+    @pytest.fixture
     def schema_int_type(self, int_type):
         return int_type
 
     @pytest.fixture
     def data_types(self, schema_int_type, int_type, string_type):
         # sql_column_value, schema_data_type, error_data_type
         return [
@@ -76,43 +81,34 @@
         manifest = get_manifest(project.project_root)
         model_id = "model.test.my_model_wrong_name"
         my_model_config = manifest.nodes[model_id].config
         contract_actual_config = my_model_config.contract
 
         assert contract_actual_config.enforced is True
 
-        expected_compile_error = "Please ensure the name, data_type, and number of columns in your `yml` file match the columns in your SQL file."
-        expected_schema_file_columns = (
-            f"Schema File Columns: id {int_type}, color {string_type}, date_day {string_type}"
-        )
-        expected_sql_file_columns = (
-            f"SQL File Columns: color {string_type}, error {int_type}, date_day {string_type}"
-        )
-
-        assert expected_compile_error in log_output
-        assert expected_schema_file_columns in log_output
-        assert expected_sql_file_columns in log_output
+        expected = ["id", "error", "missing in definition", "missing in contract"]
+        assert all([(exp in log_output or exp.upper() in log_output) for exp in expected])
 
     def test__constraints_wrong_column_data_types(
-        self, project, string_type, int_type, schema_int_type, data_types
+        self, project, string_type, int_type, schema_string_type, schema_int_type, data_types
     ):
         for (sql_column_value, schema_data_type, error_data_type) in data_types:
             # Write parametrized data_type to sql file
             write_file(
                 my_model_data_type_sql.format(sql_value=sql_column_value),
                 "models",
                 "my_model_data_type.sql",
             )
 
             # Write wrong data_type to corresponding schema file
             # Write integer type for all schema yaml values except when testing integer type itself
             wrong_schema_data_type = (
                 schema_int_type
                 if schema_data_type.upper() != schema_int_type.upper()
-                else string_type
+                else schema_string_type
             )
             wrong_schema_error_data_type = (
                 int_type if schema_data_type.upper() != schema_int_type.upper() else string_type
             )
             write_file(
                 model_data_type_schema_yml.format(data_type=wrong_schema_data_type),
                 "models",
@@ -124,26 +120,21 @@
             )
             manifest = get_manifest(project.project_root)
             model_id = "model.test.my_model_data_type"
             my_model_config = manifest.nodes[model_id].config
             contract_actual_config = my_model_config.contract
 
             assert contract_actual_config.enforced is True
-
-            expected_compile_error = "Please ensure the name, data_type, and number of columns in your `yml` file match the columns in your SQL file."
-            expected_sql_file_columns = (
-                f"SQL File Columns: wrong_data_type_column_name {error_data_type}"
-            )
-            expected_schema_file_columns = (
-                f"Schema File Columns: wrong_data_type_column_name {wrong_schema_error_data_type}"
-            )
-
-            assert expected_compile_error in log_output
-            assert expected_schema_file_columns in log_output
-            assert expected_sql_file_columns in log_output
+            expected = [
+                "wrong_data_type_column_name",
+                error_data_type,
+                wrong_schema_error_data_type,
+                "data type mismatch",
+            ]
+            assert all([(exp in log_output or exp.upper() in log_output) for exp in expected])
 
     def test__constraints_correct_column_data_types(self, project, data_types):
         for (sql_column_value, schema_data_type, _) in data_types:
             # Write parametrized data_type to sql file
             write_file(
                 my_model_data_type_sql.format(sql_value=sql_column_value),
                 "models",
@@ -162,14 +153,18 @@
             model_id = "model.test.my_model_data_type"
             my_model_config = manifest.nodes[model_id].config
             contract_actual_config = my_model_config.contract
 
             assert contract_actual_config.enforced is True
 
 
+def _normalize_whitespace(input: str) -> str:
+    return re.sub(r"\s+", " ", input).lower().strip()
+
+
 class BaseConstraintsRuntimeDdlEnforcement:
     """
     These constraints pass muster for dbt's preflight checks. Make sure they're
     passed into the DDL statement. If they don't match up with the underlying data,
     the data platform should raise an error at runtime.
     """
 
@@ -212,31 +207,23 @@
         results = run_dbt(["run", "-s", "my_model"])
         assert len(results) == 1
 
         # grab the sql and replace the model identifier to make it generic for all adapters
         # the name is not what we're testing here anyways and varies based on materialization
         # TODO: consider refactoring this to introspect logs instead
         generated_sql = read_file("target", "run", "test", "models", "my_model.sql")
-        generated_sql_modified = re.sub(r"\s+", " ", generated_sql).lower().strip()
+        generated_sql_modified = _normalize_whitespace(generated_sql)
         generated_sql_list = generated_sql_modified.split(" ")
         for idx in [n for n, x in enumerate(generated_sql_list) if "my_model" in x]:
             generated_sql_list[idx] = "<model_identifier>"
         generated_sql_generic = " ".join(generated_sql_list)
 
-        expected_sql_check = re.sub(r"\s+", " ", expected_sql).lower().strip()
+        expected_sql_check = _normalize_whitespace(expected_sql)
 
-        assert (
-            expected_sql_check == generated_sql_generic
-        ), f"""
--- GENERATED SQL
-{generated_sql_generic}
-
--- EXPECTED SQL
-{expected_sql_check}
-"""
+        assert expected_sql_check == generated_sql_generic
 
 
 class BaseConstraintsRollback:
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "my_model.sql": my_model_sql,
@@ -365,7 +352,68 @@
     BaseIncrementalConstraintsRuntimeDdlEnforcement
 ):
     pass
 
 
 class TestIncrementalConstraintsRollback(BaseIncrementalConstraintsRollback):
     pass
+
+
+class BaseModelConstraintsRuntimeEnforcement:
+    """
+    These model-level constraints pass muster for dbt's preflight checks. Make sure they're
+    passed into the DDL statement. If they don't match up with the underlying data,
+    the data platform should raise an error at runtime.
+    """
+
+    @pytest.fixture(scope="class")
+    def models(self):
+        return {
+            "my_model.sql": my_model_sql,
+            "constraints_schema.yml": constrained_model_schema_yml,
+        }
+
+    @pytest.fixture(scope="class")
+    def expected_sql(self):
+        return """
+create table <model_identifier> (
+    id integer not null,
+    color text,
+    date_day text,
+    check (id > 0),
+    primary key (id),
+    constraint strange_uniqueness_requirement unique (color, date_day)
+) ;
+insert into <model_identifier> (
+    id ,
+    color ,
+    date_day
+)
+(
+    select
+       id,
+       color,
+       date_day
+       from
+    (
+        select
+            1 as id,
+            'blue' as color,
+            '2019-01-01' as date_day
+    ) as model_subq
+);
+"""
+
+    def test__model_constraints_ddl(self, project, expected_sql):
+        results = run_dbt(["run", "-s", "my_model"])
+        assert len(results) == 1
+        generated_sql = read_file("target", "run", "test", "models", "my_model.sql")
+        generated_sql_list = _normalize_whitespace(generated_sql).split(" ")
+        generated_sql_list = [
+            "<model_identifier>" if "my_model" in s else s for s in generated_sql_list
+        ]
+        generated_sql_generic = " ".join(generated_sql_list)
+        assert _normalize_whitespace(expected_sql) == generated_sql_generic
+
+
+class TestModelConstraintsRuntimeEnforcement(BaseModelConstraintsRuntimeEnforcement):
+    pass
```

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/dbt_debug/test_dbt_debug.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/dbt_debug/test_dbt_debug.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import os
 import re
 import yaml
 
-from dbt.cli.main import dbtUsageException
+from dbt.cli.exceptions import DbtUsageException
 from dbt.tests.util import run_dbt
 
 MODELS__MODEL_SQL = """
 seled 1 as id
 """
 
 
@@ -84,15 +84,15 @@
             yaml.safe_dump(update_project, f)
 
         run_dbt(["debug", "--profile", "test"], expect_pass=False)
         splitout = self.capsys.readouterr().out.split("\n")
         self.check_project(splitout)
 
     def test_not_found_project(self, project):
-        with pytest.raises(dbtUsageException):
+        with pytest.raises(DbtUsageException):
             run_dbt(["debug", "--project-dir", "nopass"])
 
     def test_invalid_project_outside_current_dir(self, project):
         # create a dbt_project.yml
         project_config = {"invalid-key": "not a valid key in this project"}
         os.makedirs("custom", exist_ok=True)
         with open("custom/dbt_project.yml", "w") as f:
```

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/ephemeral/test_ephemeral.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/ephemeral/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/base_grants.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/base_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/test_incremental_grants.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/test_incremental_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/test_invalid_grants.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/test_invalid_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/test_model_grants.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/test_model_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/test_seed_grants.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/test_seed_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/grants/test_snapshot_grants.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/grants/test_snapshot_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/hooks/fixtures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/hooks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/hooks/test_model_hooks.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/hooks/test_model_hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/hooks/test_run_hooks.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/hooks/test_run_hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/fixtures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/test_incremental_predicates.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/incremental/test_incremental_unique_id.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/incremental/test_incremental_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/persist_docs/fixtures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/persist_docs/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/persist_docs/test_persist_docs.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/persist_docs/test_persist_docs.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/python_model/test_python_model.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/python_model/test_python_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,23 +13,32 @@
 """
 basic_python = """
 def model(dbt, _):
     dbt.config(
         materialized='table',
     )
     df =  dbt.ref("my_sql_model")
-    df2 = dbt.source('test_source', 'test_table')
+    df2 = dbt.ref("my_versioned_sql_model", v=1)
+    df3 = dbt.ref("my_versioned_sql_model", version=1)
+    df4 = dbt.ref("test", "my_versioned_sql_model", v=1)
+    df5 = dbt.ref("test", "my_versioned_sql_model", version=1)
+    df6 = dbt.source("test_source", "test_table")
     df = df.limit(2)
     return df
 """
 
 second_sql = """
 select * from {{ref('my_python_model')}}
 """
 schema_yml = """version: 2
+models:
+  - name: my_versioned_sql_model
+    versions:
+      - v: 1
+
 sources:
   - name: test_source
     loader: custom
     schema: "{{ var(env_var('DBT_TEST_SCHEMA_NAME_VARIABLE')) }}"
     quoting:
       identifier: True
     tags:
@@ -59,27 +68,28 @@
         return {"source.csv": seeds__source_csv}
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "schema.yml": schema_yml,
             "my_sql_model.sql": basic_sql,
+            "my_versioned_sql_model_v1.sql": basic_sql,
             "my_python_model.py": basic_python,
             "second_sql_model.sql": second_sql,
         }
 
     def test_singular_tests(self, project):
         # test command
         vars_dict = {
             "test_run_schema": project.test_schema,
         }
 
         run_dbt(["seed", "--vars", yaml.safe_dump(vars_dict)])
         results = run_dbt(["run", "--vars", yaml.safe_dump(vars_dict)])
-        assert len(results) == 3
+        assert len(results) == 4
 
 
 m_1 = """
 {{config(materialized='table')}}
 select 1 as id union all
 select 2 as id union all
 select 3 as id union all
```

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/python_model/test_spark.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/python_model/test_spark.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/query_comment/fixtures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/query_comment/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/query_comment/test_query_comment.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/query_comment/test_query_comment.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/relations/test_changing_relation_type.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/relations/test_changing_relation_type.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_copy/fixtures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_copy/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_copy/test_copy_uppercase.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_copy/test_copy_uppercase.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_copy/test_simple_copy.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_copy/test_simple_copy.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_seed/fixtures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_seed/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_seed/seeds.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_seed/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_seed/test_seed.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_seed/test_seed.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/simple_seed/test_seed_type_override.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/simple_seed/test_seed_type_override.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/store_test_failures_tests/fixtures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/store_test_failures_tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/base_array_utils.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/base_array_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/base_utils.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/base_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/base_data_type_macro.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/base_data_type_macro.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_bigint.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_bigint.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_boolean.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_boolean.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_float.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_float.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_int.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_int.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_numeric.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_numeric.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_string.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_string.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/data_types/test_type_timestamp.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/data_types/test_type_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_any_value.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_any_value.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_array_concat.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_array_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_bool_or.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_bool_or.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_date_trunc.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_date_trunc.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_dateadd.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_dateadd.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_datediff.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_datediff.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_escape_single_quotes.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_escape_single_quotes.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_except.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_except.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_hash.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_hash.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_intersect.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_last_day.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_last_day.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_listagg.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_listagg.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_position.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_position.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_replace.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_replace.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_right.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_right.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_split_part.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_split_part.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/fixture_string_literal.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/fixture_string_literal.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_any_value.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_any_value.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_array_append.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_array_append.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_array_concat.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_array_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_array_construct.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_array_construct.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_bool_or.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_bool_or.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_cast_bool_to_text.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_cast_bool_to_text.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_concat.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_current_timestamp.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_current_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_date_trunc.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_date_trunc.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_dateadd.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_dateadd.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_datediff.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_datediff.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_escape_single_quotes.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_escape_single_quotes.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_except.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_except.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_hash.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_hash.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_intersect.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_last_day.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_last_day.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_length.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_length.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_listagg.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_listagg.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_position.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_position.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_replace.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_replace.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_right.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_right.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_safe_cast.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_safe_cast.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_split_part.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_split_part.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_string_literal.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt/tests/adapter/utils/test_timestamps.py` & `dbt-tests-adapter-1.5.0rc1/dbt/tests/adapter/utils/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.5.0b5/dbt_tests_adapter.egg-info/PKG-INFO` & `dbt-tests-adapter-1.5.0rc1/dbt_tests_adapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-tests-adapter
-Version: 1.5.0b5
+Version: 1.5.0rc1
 Summary: The dbt adapter tests for adapter plugins
 Home-page: https://github.com/dbt-labs/dbt-core/tree/main/tests/adapter
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-tests-adapter-1.5.0b5/dbt_tests_adapter.egg-info/SOURCES.txt` & `dbt-tests-adapter-1.5.0rc1/dbt_tests_adapter.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 dbt/tests/adapter/simple_copy/fixtures.py
 dbt/tests/adapter/simple_copy/test_copy_uppercase.py
 dbt/tests/adapter/simple_copy/test_simple_copy.py
 dbt/tests/adapter/simple_seed/fixtures.py
 dbt/tests/adapter/simple_seed/seeds.py
 dbt/tests/adapter/simple_seed/test_seed.py
 dbt/tests/adapter/simple_seed/test_seed_type_override.py
+dbt/tests/adapter/simple_snapshot/common.py
+dbt/tests/adapter/simple_snapshot/seeds.py
+dbt/tests/adapter/simple_snapshot/snapshots.py
+dbt/tests/adapter/simple_snapshot/test_snapshot.py
 dbt/tests/adapter/store_test_failures_tests/fixtures.py
 dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
 dbt/tests/adapter/utils/base_array_utils.py
 dbt/tests/adapter/utils/base_utils.py
 dbt/tests/adapter/utils/fixture_any_value.py
 dbt/tests/adapter/utils/fixture_array_append.py
 dbt/tests/adapter/utils/fixture_array_concat.py
```

### Comparing `dbt-tests-adapter-1.5.0b5/setup.py` & `dbt-tests-adapter-1.5.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # the user has a downlevel version of setuptools.
     print("Error: dbt requires setuptools v40.1.0 or higher.")
     print('Please upgrade setuptools with "pip install --upgrade setuptools" ' "and try again")
     sys.exit(1)
 
 
 package_name = "dbt-tests-adapter"
-package_version = "1.5.0b5"
+package_version = "1.5.0rc1"
 description = """The dbt adapter tests for adapter plugins"""
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setup(
```

