# Comparing `tmp/datafusion-21.0.0.tar.gz` & `tmp/datafusion-22.0.0.tar.gz`

## Comparing `datafusion-21.0.0.tar` & `datafusion-22.0.0.tar`

### file list

```diff
@@ -1,100 +1,98 @@
--rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 datafusion-21.0.0/pyproject.toml
--rw-r--r--   0        0        0     2541 1970-01-01 00:00:00.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/Cargo.toml
--rw-rw-r--   0     1000     1000    11358 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/LICENSE.txt
--rw-rw-r--   0     1000     1000     7981 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/README.md
--rw-rw-r--   0     1000     1000     3964 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/catalog.rs
--rw-rw-r--   0     1000     1000    18471 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/common/data_type.rs
--rw-rw-r--   0     1000     1000     3564 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/common/df_field.rs
--rw-rw-r--   0     1000     1000     1651 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/common/df_schema.rs
--rw-rw-r--   0     1000     1000     1369 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/common.rs
--rw-rw-r--   0     1000     1000     3308 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/config.rs
--rw-rw-r--   0     1000     1000    26123 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/context.rs
--rw-rw-r--   0     1000     1000    15231 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/dataframe.rs
--rw-rw-r--   0     1000     1000     4770 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/dataset.rs
--rw-rw-r--   0     1000     1000     9944 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/dataset_exec.rs
--rw-rw-r--   0     1000     1000     2902 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/errors.rs
--rw-rw-r--   0     1000     1000     3243 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/aggregate.rs
--rw-rw-r--   0     1000     1000     2313 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/aggregate_expr.rs
--rw-rw-r--   0     1000     1000     1867 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/alias.rs
--rw-rw-r--   0     1000     1000     2331 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/analyze.rs
--rw-rw-r--   0     1000     1000     2101 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/between.rs
--rw-rw-r--   0     1000     1000     1626 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/binary_expr.rs
--rw-rw-r--   0     1000     1000     6317 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/bool_expr.rs
--rw-rw-r--   0     1000     1000     1662 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/case.rs
--rw-rw-r--   0     1000     1000     2060 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/cast.rs
--rw-rw-r--   0     1000     1000     1688 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/column.rs
--rw-rw-r--   0     1000     1000     2716 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/create_memory_table.rs
--rw-rw-r--   0     1000     1000     2574 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/create_view.rs
--rw-rw-r--   0     1000     1000     2867 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/cross_join.rs
--rw-rw-r--   0     1000     1000     2206 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/distinct.rs
--rw-rw-r--   0     1000     1000     2338 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/drop_table.rs
--rw-rw-r--   0     1000     1000     2522 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/empty_relation.rs
--rw-rw-r--   0     1000     1000     1334 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/exists.rs
--rw-rw-r--   0     1000     1000     3168 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/explain.rs
--rw-rw-r--   0     1000     1000     1535 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/extension.rs
--rw-rw-r--   0     1000     1000     2502 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/filter.rs
--rw-rw-r--   0     1000     1000     1293 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/grouping_set.rs
--rw-rw-r--   0     1000     1000     1495 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/in_list.rs
--rw-rw-r--   0     1000     1000     1531 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/in_subquery.rs
--rw-rw-r--   0     1000     1000     2093 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/indexed_field.rs
--rw-rw-r--   0     1000     1000     5153 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/join.rs
--rw-rw-r--   0     1000     1000     4441 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/like.rs
--rw-rw-r--   0     1000     1000     2584 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/limit.rs
--rw-rw-r--   0     1000     1000     4984 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/literal.rs
--rw-rw-r--   0     1000     1000     1199 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/logical_node.rs
--rw-rw-r--   0     1000     1000     1456 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/placeholder.rs
--rw-rw-r--   0     1000     1000     2983 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/projection.rs
--rw-rw-r--   0     1000     1000     3884 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/repartition.rs
--rw-rw-r--   0     1000     1000     2109 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/scalar_function.rs
--rw-rw-r--   0     1000     1000     1431 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/scalar_subquery.rs
--rw-rw-r--   0     1000     1000     1674 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/scalar_variable.rs
--rw-rw-r--   0     1000     1000     1310 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/signature.rs
--rw-rw-r--   0     1000     1000     2736 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/sort.rs
--rw-rw-r--   0     1000     1000     1233 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/subquery.rs
--rw-rw-r--   0     1000     1000     2750 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/subquery_alias.rs
--rw-rw-r--   0     1000     1000     4489 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/table_scan.rs
--rw-rw-r--   0     1000     1000     2470 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/union.rs
--rw-rw-r--   0     1000     1000    10256 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr.rs
--rw-rw-r--   0     1000     1000    17920 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/functions.rs
--rw-rw-r--   0     1000     1000     3468 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/lib.rs
--rw-rw-r--   0     1000     1000     2069 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/physical_plan.rs
--rw-rw-r--   0     1000     1000     8525 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/pyarrow_filter_expression.rs
--rw-rw-r--   0     1000     1000     2055 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/record_batch.rs
--rw-rw-r--   0     1000     1000     1716 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/sql/exceptions.rs
--rw-rw-r--   0     1000     1000     4117 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/sql/logical.rs
--rw-rw-r--   0     1000     1000      839 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/sql.rs
--rw-rw-r--   0     1000     1000     7499 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/store.rs
--rw-rw-r--   0     1000     1000     4727 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/substrait.rs
--rw-rw-r--   0     1000     1000     4767 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/udaf.rs
--rw-rw-r--   0     1000     1000     3541 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/udf.rs
--rw-rw-r--   0     1000     1000     1667 2023-03-31 15:27:23.000000 datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/utils.rs
--rw-rw-r--   0     1000     1000    96104 2023-03-31 15:27:23.000000 datafusion-21.0.0/Cargo.lock
--rw-rw-r--   0     1000     1000      871 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/expr.py
--rw-rw-r--   0     1000     1000     1842 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_substrait.py
--rw-rw-r--   0     1000     1000     9833 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_context.py
--rw-rw-r--   0     1000     1000     1443 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/conftest.py
--rw-rw-r--   0     1000     1000     2319 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/generic.py
--rw-rw-r--   0     1000     1000     3984 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_imports.py
--rw-rw-r--   0     1000     1000     1632 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_indexing.py
--rw-rw-r--   0     1000     1000      785 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/__init__.py
--rw-rw-r--   0     1000     1000     1355 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_store.py
--rw-rw-r--   0     1000     1000    14842 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_functions.py
--rw-rw-r--   0     1000     1000     3619 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_udaf.py
--rw-rw-r--   0     1000     1000     9040 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_sql.py
--rw-rw-r--   0     1000     1000     1432 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_catalog.py
--rw-rw-r--   0     1000     1000    16915 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_dataframe.py
--rw-rw-r--   0     1000     1000     3179 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_expr.py
--rw-rw-r--   0     1000     1000     1365 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_config.py
--rw-rw-r--   0     1000     1000       57 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/data_test_context/data.json
--rw-rw-r--   0     1000     1000     4339 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/tests/test_aggregation.py
--rw-rw-r--   0     1000     1000     3279 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/polars.py
--rw-rw-r--   0     1000     1000     2242 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/cudf.py
--rw-rw-r--   0     1000     1000      875 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/common.py
--rw-rw-r--   0     1000     1000     4404 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/__init__.py
--rw-rw-r--   0     1000     1000      881 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/substrait.py
--rw-rw-r--   0     1000     1000     2258 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/pandas.py
--rw-rw-r--   0     1000     1000      881 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/functions.py
--rw-rw-r--   0     1000     1000      887 2023-03-31 15:27:23.000000 datafusion-21.0.0/datafusion/object_store.py
--rw-rw-r--   0     1000     1000     7981 2023-03-31 15:27:23.000000 datafusion-21.0.0/README.md
--rw-rw-r--   0     1000     1000    11358 2023-03-31 15:27:23.000000 datafusion-21.0.0/LICENSE.txt
--rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 datafusion-21.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 datafusion-22.0.0/Cargo.toml
+-rw-rw-r--   0     1000     1000    11358 2023-04-10 23:37:22.000000 datafusion-22.0.0/LICENSE.txt
+-rw-rw-r--   0     1000     1000     7981 2023-04-10 23:37:22.000000 datafusion-22.0.0/README.md
+-rw-rw-r--   0     1000     1000     4404 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/__init__.py
+-rw-rw-r--   0     1000     1000      875 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/common.py
+-rw-rw-r--   0     1000     1000     2242 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/cudf.py
+-rw-rw-r--   0     1000     1000      871 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/expr.py
+-rw-rw-r--   0     1000     1000      881 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/functions.py
+-rw-rw-r--   0     1000     1000      887 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/object_store.py
+-rw-rw-r--   0     1000     1000     2258 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/pandas.py
+-rw-rw-r--   0     1000     1000     3279 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/polars.py
+-rw-rw-r--   0     1000     1000      881 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/substrait.py
+-rw-rw-r--   0     1000     1000      785 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/__init__.py
+-rw-rw-r--   0     1000     1000     1443 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/conftest.py
+-rw-rw-r--   0     1000     1000       57 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/data_test_context/data.json
+-rw-rw-r--   0     1000     1000     2319 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/generic.py
+-rw-rw-r--   0     1000     1000     4339 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_aggregation.py
+-rw-rw-r--   0     1000     1000     1432 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_catalog.py
+-rw-rw-r--   0     1000     1000     1365 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_config.py
+-rw-rw-r--   0     1000     1000     9833 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_context.py
+-rw-rw-r--   0     1000     1000    16915 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_dataframe.py
+-rw-rw-r--   0     1000     1000     3179 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_expr.py
+-rw-rw-r--   0     1000     1000    14842 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_functions.py
+-rw-rw-r--   0     1000     1000     3984 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_imports.py
+-rw-rw-r--   0     1000     1000     1631 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_indexing.py
+-rw-rw-r--   0     1000     1000     9040 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_sql.py
+-rw-rw-r--   0     1000     1000     1355 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_store.py
+-rw-rw-r--   0     1000     1000     1842 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_substrait.py
+-rw-rw-r--   0     1000     1000     3619 2023-04-10 23:37:22.000000 datafusion-22.0.0/datafusion/tests/test_udaf.py
+-rw-rw-r--   0     1000     1000     2139 2023-04-10 23:37:22.000000 datafusion-22.0.0/pyproject.toml
+-rw-rw-r--   0     1000     1000     3964 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/catalog.rs
+-rw-rw-r--   0     1000     1000    18471 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/common/data_type.rs
+-rw-rw-r--   0     1000     1000     3564 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/common/df_field.rs
+-rw-rw-r--   0     1000     1000     1651 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/common/df_schema.rs
+-rw-rw-r--   0     1000     1000     1369 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/common.rs
+-rw-rw-r--   0     1000     1000     3308 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/config.rs
+-rw-rw-r--   0     1000     1000    26123 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/context.rs
+-rw-rw-r--   0     1000     1000    15231 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/dataframe.rs
+-rw-rw-r--   0     1000     1000     4770 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/dataset.rs
+-rw-rw-r--   0     1000     1000     9944 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/dataset_exec.rs
+-rw-rw-r--   0     1000     1000     2902 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/errors.rs
+-rw-rw-r--   0     1000     1000     3243 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/aggregate.rs
+-rw-rw-r--   0     1000     1000     2313 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/aggregate_expr.rs
+-rw-rw-r--   0     1000     1000     1867 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/alias.rs
+-rw-rw-r--   0     1000     1000     2331 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/analyze.rs
+-rw-rw-r--   0     1000     1000     2101 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/between.rs
+-rw-rw-r--   0     1000     1000     1626 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/binary_expr.rs
+-rw-rw-r--   0     1000     1000     6317 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/bool_expr.rs
+-rw-rw-r--   0     1000     1000     1662 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/case.rs
+-rw-rw-r--   0     1000     1000     2060 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/cast.rs
+-rw-rw-r--   0     1000     1000     1688 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/column.rs
+-rw-rw-r--   0     1000     1000     2716 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/create_memory_table.rs
+-rw-rw-r--   0     1000     1000     2574 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/create_view.rs
+-rw-rw-r--   0     1000     1000     2867 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/cross_join.rs
+-rw-rw-r--   0     1000     1000     2206 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/distinct.rs
+-rw-rw-r--   0     1000     1000     2338 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/drop_table.rs
+-rw-rw-r--   0     1000     1000     2522 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/empty_relation.rs
+-rw-rw-r--   0     1000     1000     1334 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/exists.rs
+-rw-rw-r--   0     1000     1000     3168 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/explain.rs
+-rw-rw-r--   0     1000     1000     1535 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/extension.rs
+-rw-rw-r--   0     1000     1000     2502 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/filter.rs
+-rw-rw-r--   0     1000     1000     1293 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/grouping_set.rs
+-rw-rw-r--   0     1000     1000     1495 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/in_list.rs
+-rw-rw-r--   0     1000     1000     1531 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/in_subquery.rs
+-rw-rw-r--   0     1000     1000     2093 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/indexed_field.rs
+-rw-rw-r--   0     1000     1000     5153 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/join.rs
+-rw-rw-r--   0     1000     1000     4441 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/like.rs
+-rw-rw-r--   0     1000     1000     2584 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/limit.rs
+-rw-rw-r--   0     1000     1000     4984 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/literal.rs
+-rw-rw-r--   0     1000     1000     1199 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/logical_node.rs
+-rw-rw-r--   0     1000     1000     1456 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/placeholder.rs
+-rw-rw-r--   0     1000     1000     2983 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/projection.rs
+-rw-rw-r--   0     1000     1000     3884 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/repartition.rs
+-rw-rw-r--   0     1000     1000     2109 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/scalar_function.rs
+-rw-rw-r--   0     1000     1000     1431 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/scalar_subquery.rs
+-rw-rw-r--   0     1000     1000     1674 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/scalar_variable.rs
+-rw-rw-r--   0     1000     1000     1310 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/signature.rs
+-rw-rw-r--   0     1000     1000     2736 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/sort.rs
+-rw-rw-r--   0     1000     1000     1233 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/subquery.rs
+-rw-rw-r--   0     1000     1000     2750 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/subquery_alias.rs
+-rw-rw-r--   0     1000     1000     4489 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/table_scan.rs
+-rw-rw-r--   0     1000     1000     2470 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr/union.rs
+-rw-rw-r--   0     1000     1000    10256 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/expr.rs
+-rw-rw-r--   0     1000     1000    17920 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/functions.rs
+-rw-rw-r--   0     1000     1000     3468 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/lib.rs
+-rw-rw-r--   0     1000     1000     2069 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/physical_plan.rs
+-rw-rw-r--   0     1000     1000     8525 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/pyarrow_filter_expression.rs
+-rw-rw-r--   0     1000     1000     2055 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/record_batch.rs
+-rw-rw-r--   0     1000     1000     1716 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/sql/exceptions.rs
+-rw-rw-r--   0     1000     1000     4117 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/sql/logical.rs
+-rw-rw-r--   0     1000     1000      839 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/sql.rs
+-rw-rw-r--   0     1000     1000     7499 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/store.rs
+-rw-rw-r--   0     1000     1000     4727 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/substrait.rs
+-rw-rw-r--   0     1000     1000     4767 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/udaf.rs
+-rw-rw-r--   0     1000     1000     3541 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/udf.rs
+-rw-rw-r--   0     1000     1000     1667 2023-04-10 23:37:22.000000 datafusion-22.0.0/src/utils.rs
+-rw-rw-r--   0     1000     1000    99124 2023-04-10 23:37:22.000000 datafusion-22.0.0/Cargo.lock
+-rw-r--r--   0        0        0     8665 1970-01-01 00:00:00.000000 datafusion-22.0.0/PKG-INFO
```

### Comparing `datafusion-21.0.0/pyproject.toml` & `datafusion-22.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [build-system]
-requires = ["maturin>=0.11,<0.15"]
+requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "datafusion"
 description = "Build and run queries against data"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
```

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/Cargo.toml` & `datafusion-22.0.0/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -13,38 +13,39 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [package]
 name = "datafusion-python"
-version = "21.0.0"
+version = "22.0.0"
 homepage = "https://github.com/apache/arrow-datafusion-python"
 repository = "https://github.com/apache/arrow-datafusion-python"
 authors = ["Apache Arrow <dev@arrow.apache.org>"]
 description = "Apache Arrow DataFusion DataFrame and SQL Query Engine"
 readme = "README.md"
 license = "Apache-2.0"
 edition = "2021"
 rust-version = "1.64"
-include = ["/src", "/LICENSE.txt"]
+include = ["/src", "/datafusion", "/LICENSE.txt", "pyproject.toml", "Cargo.toml", "Cargo.lock"]
 
 [features]
 default = ["mimalloc"]
+protoc = [ "datafusion-substrait/protoc" ]
 
 [dependencies]
 tokio = { version = "1.24", features = ["macros", "rt", "rt-multi-thread", "sync"] }
 rand = "0.8"
 pyo3 = { version = "0.18.1", features = ["extension-module", "abi3", "abi3-py37"] }
-datafusion = { git = "https://github.com/apache/arrow-datafusion.git", rev = "c09edad", features = ["pyarrow", "avro"] }
-datafusion-common = { git = "https://github.com/apache/arrow-datafusion.git", rev = "c09edad", features = ["pyarrow"] }
-datafusion-expr = { git = "https://github.com/apache/arrow-datafusion.git", rev = "c09edad" }
-datafusion-optimizer = { git = "https://github.com/apache/arrow-datafusion.git", rev = "c09edad" }
-datafusion-sql = { git = "https://github.com/apache/arrow-datafusion.git", rev = "c09edad" }
-datafusion-substrait = { git = "https://github.com/apache/arrow-datafusion.git", rev = "c09edad" }
+datafusion = { version = "22.0.0", features = ["pyarrow", "avro"] }
+datafusion-common = { version = "22.0.0", features = ["pyarrow"] }
+datafusion-expr = { version = "22.0.0" }
+datafusion-optimizer = { version = "22.0.0" }
+datafusion-sql = { version = "22.0.0" }
+datafusion-substrait = { version = "22.0.0" }
 uuid = { version = "1.2", features = ["v4"] }
 mimalloc = { version = "0.1", optional = true, default-features = false }
 async-trait = "0.1"
 futures = "0.3"
 object_store = { version = "0.5.3", features = ["aws", "gcp", "azure"] }
 parking_lot = "0.12"
 regex-syntax = "0.6.28"
```

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/LICENSE.txt` & `datafusion-22.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/README.md` & `datafusion-22.0.0/README.md`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/catalog.rs` & `datafusion-22.0.0/src/catalog.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/common/data_type.rs` & `datafusion-22.0.0/src/common/data_type.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/common/df_field.rs` & `datafusion-22.0.0/src/common/df_field.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/common/df_schema.rs` & `datafusion-22.0.0/src/common/df_schema.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/common.rs` & `datafusion-22.0.0/src/common.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/config.rs` & `datafusion-22.0.0/src/config.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/context.rs` & `datafusion-22.0.0/src/context.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/dataframe.rs` & `datafusion-22.0.0/src/dataframe.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/dataset.rs` & `datafusion-22.0.0/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/dataset_exec.rs` & `datafusion-22.0.0/src/dataset_exec.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/errors.rs` & `datafusion-22.0.0/src/errors.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/aggregate.rs` & `datafusion-22.0.0/src/expr/aggregate.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/aggregate_expr.rs` & `datafusion-22.0.0/src/expr/aggregate_expr.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/alias.rs` & `datafusion-22.0.0/src/expr/alias.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/analyze.rs` & `datafusion-22.0.0/src/expr/analyze.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/between.rs` & `datafusion-22.0.0/src/expr/between.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/binary_expr.rs` & `datafusion-22.0.0/src/expr/binary_expr.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/bool_expr.rs` & `datafusion-22.0.0/src/expr/bool_expr.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/case.rs` & `datafusion-22.0.0/src/expr/case.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/cast.rs` & `datafusion-22.0.0/src/expr/cast.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/column.rs` & `datafusion-22.0.0/src/expr/column.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/create_memory_table.rs` & `datafusion-22.0.0/src/expr/create_memory_table.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/create_view.rs` & `datafusion-22.0.0/src/expr/create_view.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/cross_join.rs` & `datafusion-22.0.0/src/expr/cross_join.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/distinct.rs` & `datafusion-22.0.0/src/expr/distinct.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/drop_table.rs` & `datafusion-22.0.0/src/expr/drop_table.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/empty_relation.rs` & `datafusion-22.0.0/src/expr/empty_relation.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/exists.rs` & `datafusion-22.0.0/src/expr/exists.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/explain.rs` & `datafusion-22.0.0/src/expr/explain.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/extension.rs` & `datafusion-22.0.0/src/expr/extension.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/filter.rs` & `datafusion-22.0.0/src/expr/filter.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/grouping_set.rs` & `datafusion-22.0.0/src/expr/grouping_set.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/in_list.rs` & `datafusion-22.0.0/src/expr/in_list.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/in_subquery.rs` & `datafusion-22.0.0/src/expr/in_subquery.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/indexed_field.rs` & `datafusion-22.0.0/src/expr/indexed_field.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/join.rs` & `datafusion-22.0.0/src/expr/join.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/like.rs` & `datafusion-22.0.0/src/expr/like.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/limit.rs` & `datafusion-22.0.0/src/expr/limit.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/literal.rs` & `datafusion-22.0.0/src/expr/literal.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/logical_node.rs` & `datafusion-22.0.0/src/expr/logical_node.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/placeholder.rs` & `datafusion-22.0.0/src/expr/placeholder.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/projection.rs` & `datafusion-22.0.0/src/expr/projection.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/repartition.rs` & `datafusion-22.0.0/src/expr/repartition.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/scalar_function.rs` & `datafusion-22.0.0/src/expr/scalar_function.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/scalar_subquery.rs` & `datafusion-22.0.0/src/expr/scalar_subquery.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/scalar_variable.rs` & `datafusion-22.0.0/src/expr/scalar_variable.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/signature.rs` & `datafusion-22.0.0/src/expr/signature.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/sort.rs` & `datafusion-22.0.0/src/expr/sort.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/subquery.rs` & `datafusion-22.0.0/src/expr/subquery.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/subquery_alias.rs` & `datafusion-22.0.0/src/expr/subquery_alias.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/table_scan.rs` & `datafusion-22.0.0/src/expr/table_scan.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr/union.rs` & `datafusion-22.0.0/src/expr/union.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/expr.rs` & `datafusion-22.0.0/src/expr.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/functions.rs` & `datafusion-22.0.0/src/functions.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/lib.rs` & `datafusion-22.0.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/physical_plan.rs` & `datafusion-22.0.0/src/physical_plan.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/pyarrow_filter_expression.rs` & `datafusion-22.0.0/src/pyarrow_filter_expression.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/record_batch.rs` & `datafusion-22.0.0/src/record_batch.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/sql/exceptions.rs` & `datafusion-22.0.0/src/sql/exceptions.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/sql/logical.rs` & `datafusion-22.0.0/src/sql/logical.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/sql.rs` & `datafusion-22.0.0/src/sql.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/store.rs` & `datafusion-22.0.0/src/store.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/substrait.rs` & `datafusion-22.0.0/src/substrait.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/udaf.rs` & `datafusion-22.0.0/src/udaf.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/udf.rs` & `datafusion-22.0.0/src/udf.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/rust_src/apache-arrow-datafusion-python-21.0.0/src/utils.rs` & `datafusion-22.0.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/Cargo.lock` & `datafusion-22.0.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 
 [[package]]
 name = "arrow-schema"
 version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d04f17f7b86ded0b5baf98fe6123391c4343e031acc3ccc5fa604cc180bff220"
 dependencies = [
- "bitflags 2.0.2",
+ "bitflags 2.1.0",
 ]
 
 [[package]]
 name = "arrow-select"
 version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "163e35de698098ff5f5f672ada9dc1f82533f10407c7a11e2cd09f3bcf31d18a"
@@ -346,51 +346,60 @@
 name = "async-recursion"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "autotools"
+version = "0.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aef8da1805e028a172334c3b680f93e71126f2327622faef2ec3d893c0a4ad77"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "base64"
 version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "487f1e0fcbe47deb8b0574e646def1c903389d95241dd1bbcc6ce4a715dfc0c1"
+checksum = "c70beb79cbb5ce9c4f8e20849978f34225931f665bb49efa6982875a4d5facb3"
 
 [[package]]
 name = "blake2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
@@ -530,17 +539,17 @@
  "time 0.1.45",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "chrono-tz"
-version = "0.8.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa48fa079165080f11d7753fd0bc175b7d391f276b965fe4b55bfad67856e463"
+checksum = "cf9cc2b23599e6d7479755f3594285efb3f74a1bdca7a7374948bc831e23a552"
 dependencies = [
  "chrono",
  "chrono-tz-build",
  "phf",
 ]
 
 [[package]]
@@ -607,17 +616,17 @@
 name = "constant_time_eq"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "13418e745008f7349ec7e449155f419a61b92b58a99cc3616942b926825ec76b"
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
 dependencies = [
@@ -690,15 +699,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
@@ -707,15 +716,15 @@
 name = "cxxbridge-macro"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
@@ -725,16 +734,17 @@
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "datafusion"
-version = "21.0.0"
-source = "git+https://github.com/apache/arrow-datafusion.git?rev=c09edad#c09edade14d456f1d2161c5ebb8c1e51e592a8ef"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9bdb93fee4f30368f1f71bfd5cd28882ec9fab0183db7924827b76129d33227c"
 dependencies = [
  "ahash",
  "apache-avro",
  "arrow",
  "async-compression",
  "async-trait",
  "bytes",
@@ -774,32 +784,34 @@
  "uuid",
  "xz2",
  "zstd 0.12.3+zstd.1.5.2",
 ]
 
 [[package]]
 name = "datafusion-common"
-version = "21.0.0"
-source = "git+https://github.com/apache/arrow-datafusion.git?rev=c09edad#c09edade14d456f1d2161c5ebb8c1e51e592a8ef"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e82401ce129e601d406012b6d718f8978ba84c386e1c342fa155877120d68824"
 dependencies = [
  "apache-avro",
  "arrow",
  "arrow-array",
  "chrono",
  "num_cpus",
  "object_store",
  "parquet",
  "pyo3",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-execution"
-version = "21.0.0"
-source = "git+https://github.com/apache/arrow-datafusion.git?rev=c09edad#c09edade14d456f1d2161c5ebb8c1e51e592a8ef"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b08b2078aed21a27239cd93f3015e492a58b0d50ebeeaf8d2236cf108ef583ce"
 dependencies = [
  "dashmap",
  "datafusion-common",
  "datafusion-expr",
  "hashbrown 0.13.2",
  "log",
  "object_store",
@@ -807,27 +819,29 @@
  "rand",
  "tempfile",
  "url",
 ]
 
 [[package]]
 name = "datafusion-expr"
-version = "21.0.0"
-source = "git+https://github.com/apache/arrow-datafusion.git?rev=c09edad#c09edade14d456f1d2161c5ebb8c1e51e592a8ef"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "16b5b977ce9695fb4c67614266ec57f384fc11e9a9f9b3e6d0e62b9c5a9f2c1f"
 dependencies = [
  "ahash",
  "arrow",
  "datafusion-common",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-optimizer"
-version = "21.0.0"
-source = "git+https://github.com/apache/arrow-datafusion.git?rev=c09edad#c09edade14d456f1d2161c5ebb8c1e51e592a8ef"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a0b2bb9e73ed778d1bc5af63a270f0154bf6eab5099c77668a6362296888e46b"
 dependencies = [
  "arrow",
  "async-trait",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-physical-expr",
@@ -835,16 +849,17 @@
  "itertools",
  "log",
  "regex-syntax",
 ]
 
 [[package]]
 name = "datafusion-physical-expr"
-version = "21.0.0"
-source = "git+https://github.com/apache/arrow-datafusion.git?rev=c09edad#c09edade14d456f1d2161c5ebb8c1e51e592a8ef"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80cd8ea5ab0a07b1b2a3e17d5909f1b1035bd129ffeeb5c66842a32e682f8f79"
 dependencies = [
  "ahash",
  "arrow",
  "arrow-array",
  "arrow-buffer",
  "arrow-schema",
  "blake2",
@@ -866,15 +881,15 @@
  "sha2",
  "unicode-segmentation",
  "uuid",
 ]
 
 [[package]]
 name = "datafusion-python"
-version = "21.0.0"
+version = "22.0.0"
 dependencies = [
  "async-trait",
  "datafusion",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-optimizer",
  "datafusion-sql",
@@ -882,47 +897,51 @@
  "futures",
  "mimalloc",
  "object_store",
  "parking_lot",
  "pyo3",
  "rand",
  "regex-syntax",
- "syn 2.0.12",
+ "syn 2.0.13",
  "tokio",
  "url",
  "uuid",
 ]
 
 [[package]]
 name = "datafusion-row"
-version = "21.0.0"
-source = "git+https://github.com/apache/arrow-datafusion.git?rev=c09edad#c09edade14d456f1d2161c5ebb8c1e51e592a8ef"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2a95d6badab19fd6e9195fdc5209ac0a7e5ce9bcdedc67767b9ffc1b4e645760"
 dependencies = [
  "arrow",
  "datafusion-common",
  "paste",
  "rand",
 ]
 
 [[package]]
 name = "datafusion-sql"
-version = "21.0.0"
-source = "git+https://github.com/apache/arrow-datafusion.git?rev=c09edad#c09edade14d456f1d2161c5ebb8c1e51e592a8ef"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "37a78f8fc67123c4357e63bc0c87622a2a663d26f074958d749a633d0ecde90f"
 dependencies = [
+ "arrow",
  "arrow-schema",
  "datafusion-common",
  "datafusion-expr",
  "log",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-substrait"
-version = "21.0.0"
-source = "git+https://github.com/apache/arrow-datafusion.git?rev=c09edad#c09edade14d456f1d2161c5ebb8c1e51e592a8ef"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae6ed64a2005f0d78f2b1b3ec3f8148183f4523d5d364e5367115f8d8a82b7df"
 dependencies = [
  "async-recursion",
  "chrono",
  "datafusion",
  "itertools",
  "object_store",
  "prost",
@@ -992,21 +1011,21 @@
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "errno"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d6a0976c999d473fe89ad888d5a284e55366d9dc9038b1ba2aa15128c4afa0"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -1022,22 +1041,22 @@
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "filetime"
-version = "0.2.20"
+version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a3de6e8d11b22ff9edc6d916f890800597d60f8b2da1caf2955c274638d6412"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall 0.2.16",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
@@ -1129,15 +1148,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1174,28 +1193,28 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "gix"
-version = "0.42.0"
+version = "0.43.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd5e0d9c5df90c9b4d325ec716762beb7d6c1465a4049fec5c4f6b72e7824656"
+checksum = "c256ea71cc1967faaefdaad15f334146b7c806f12460dcafd3afed845c8c78dd"
 dependencies = [
  "gix-actor",
  "gix-attributes",
  "gix-config",
  "gix-credentials",
  "gix-date",
  "gix-diff",
@@ -1283,25 +1302,26 @@
 checksum = "b2c6f75c1e0f924de39e750880a6e21307194bb1ab773efe3c7d2d787277f8ab"
 dependencies = [
  "bstr",
 ]
 
 [[package]]
 name = "gix-config"
-version = "0.19.0"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aa7d7dd60256b7a0c0506a1d708ec92767c2662ee57b3301b538eaa3e064f8a"
+checksum = "7fbad5ce54a8fc997acc50febd89ec80fa6e97cb7f8d0654cb229936407489d8"
 dependencies = [
  "bstr",
  "gix-config-value",
  "gix-features",
  "gix-glob",
  "gix-path",
  "gix-ref",
  "gix-sec",
+ "log",
  "memchr",
  "nom",
  "once_cell",
  "smallvec",
  "thiserror",
  "unicode-bom",
 ]
@@ -1590,17 +1610,17 @@
  "gix-validate",
  "smallvec",
  "thiserror",
 ]
 
 [[package]]
 name = "gix-revision"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b12fc4bbc3161a5b2d68079fce93432cef8771ff88ca017abb01187fddfc41a1"
+checksum = "3c6f6ff53f888858afc24bf12628446a14279ceec148df6194481f306f553ad2"
 dependencies = [
  "bstr",
  "gix-date",
  "gix-hash",
  "gix-hashtable",
  "gix-object",
  "thiserror",
@@ -1842,24 +1862,24 @@
  "rustls",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.54"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c17cc76786e99f8d2f055c11159e7f0091c42474dcc3189fbab96072e873e6d"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "windows 0.46.0",
+ "windows 0.48.0",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
@@ -1927,21 +1947,21 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09270fd4fa1111bc614ed2246c7ef56239a3063d5be0d1ec3b589c505d400aeb"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ipnet"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
@@ -2047,17 +2067,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "libflate"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97822bf791bd4d5b403713886a5fbe8bf49520fe78e323b0dc480ca1a03e50b0"
 dependencies = [
@@ -2079,17 +2099,17 @@
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
 [[package]]
 name = "libmimalloc-sys"
-version = "0.1.30"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8c7cbf8b89019683667e347572e6d55a7df7ea36b0c4ce69961b0cde67b174"
+checksum = "43a558e3d911bc3c7bfc8c78bc580b404d6e51c1cefbf656e176a94b49b0df40"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "link-cplusplus"
@@ -2187,17 +2207,17 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
-version = "0.1.34"
+version = "0.1.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9dcb174b18635f7561a0c6c9fc2ce57218ac7523cf72c50af80e2d79ab8f3ba1"
+checksum = "3d88dad3f985ec267a3fcb7a1726f5cb1a7e8cad8b646e70a84f967210df23da"
 dependencies = [
  "libmimalloc-sys",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
@@ -2224,15 +2244,15 @@
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
 dependencies = [
  "libc",
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "multimap"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
@@ -2353,17 +2373,17 @@
 checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "object_store"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1ea8f683b4f89a64181393742c041520a1a87e9775e6b4c0dd5a3281af05fc6"
+checksum = "ec9cd6ca25e796a49fa242876d1c4de36a24a6da5258e9f0bc062dbf5e81c53b"
 dependencies = [
  "async-trait",
  "base64",
  "bytes",
  "chrono",
  "futures",
  "itertools",
@@ -2414,15 +2434,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall 0.2.16",
  "smallvec",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "parquet"
 version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "321a15f8332645759f29875b07f8233d16ed8ec1b3582223de81625a9f8506b7"
@@ -2550,28 +2570,28 @@
 [[package]]
 name = "prettyplease"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ceca8aaf45b5c46ec7ed39fff75f57290368c1846d33d24a122ca81416ab058"
 dependencies = [
  "proc-macro2",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.54"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prodash"
 version = "23.1.2"
@@ -2627,14 +2647,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "379119666929a1afd7a043aa6cf96fa67a6dce9af60c88095a4686dbce4c9c88"
 dependencies = [
  "prost",
 ]
 
 [[package]]
+name = "protobuf-src"
+version = "1.1.0+21.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c7ac8852baeb3cc6fb83b93646fb93c0ffe5d14bf138c945ceb4b9948ee0e3c1"
+dependencies = [
+ "autotools",
+]
+
+[[package]]
 name = "pyo3"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if",
  "indoc",
@@ -2694,17 +2723,17 @@
 name = "quad-rand"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "658fa1faf7a4cc5f057c9ee5ef560f717ad9d8dc66d975267f709624d6e1ab88"
 
 [[package]]
 name = "quick-xml"
-version = "0.27.1"
+version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffc053f057dd768a56f62cd7e434c42c831d296968997e9ac1f76ea7c2d14c41"
+checksum = "e5c1a97b1bc42b1d550bfb48d4262153fe400a12bab1511821736f7eac76d7e2"
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "quote"
@@ -2876,24 +2905,24 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.5"
+version = "0.37.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e78cc525325c06b4a7ff02db283472f3c042b7ff0c391f96c6d5ac6f4f91b75"
+checksum = "85597d61f83914ddeba6a47b3b8ffe7365107221c2e557ed94426489fefb5f77"
 dependencies = [
  "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustls"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fff78fc74d175294f4e83b28343315ffcfb114b156f0185e9741cb5570f50e2f"
@@ -3005,15 +3034,15 @@
 name = "serde_derive"
 version = "1.0.159"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "serde_derive_internals"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
@@ -3055,17 +3084,17 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.19"
+version = "0.9.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f82e6c8c047aa50a7328632d067bcae6ef38772a79e28daf32f735e0e4f3dd10"
+checksum = "d9d684e3ec7de3bf5466b32bd75303ac16f0736426e5a4e0d6e489559ce1249c"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
@@ -3215,30 +3244,31 @@
  "quote",
  "rustversion",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "substrait"
-version = "0.6.0"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a94bab2309478886b270dbace5adb3927d8e397aa804b67c5c37da8591dff989"
+checksum = "fcd7c95895a69f92b0491cb0764d49140f57ad918a8abb3b7ec7f8e507d2a240"
 dependencies = [
  "gix",
  "heck",
  "prettyplease",
  "prost",
  "prost-build",
  "prost-types",
+ "protobuf-src",
  "schemars",
  "semver",
  "serde",
  "serde_json",
  "serde_yaml",
- "syn 2.0.12",
+ "syn 2.0.13",
  "typify",
  "walkdir",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.4.1"
@@ -3254,17 +3284,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.12"
+version = "2.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "79d9531f94112cfc3e4c8f5f02cb2b58f72c97b7efd85f70203cc6d8efda5927"
+checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3279,15 +3309,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
  "redox_syscall 0.3.5",
  "rustix",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
@@ -3308,15 +3338,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "thrift"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
@@ -3401,26 +3431,26 @@
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61a573bdc87985e9d6ddeed1b3d864e8a302c847e40d647746df2f1de209d1ce"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.23.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
@@ -3613,17 +3643,17 @@
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "unsafe-libyaml"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad2024452afd3874bf539695e04af6732ba06517424dbf958fdb16a01f3bef6c"
+checksum = "1865806a559042e51ab5414598446a5871b561d21b6764f2eabb0dd481d880a6"
 
 [[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
@@ -3636,17 +3666,17 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
+checksum = "5b55a3fef2a1e3b3a00ce878640918820d3c51081576ac657d23af9fc7928fdb"
 dependencies = [
  "getrandom",
  "serde",
 ]
 
 [[package]]
 name = "version_check"
@@ -3838,99 +3868,165 @@
 
 [[package]]
 name = "windows"
 version = "0.43.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04662ed0e3e5630dfa9b26e4cb823b817f1a9addda855d973a9458c236556244"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows"
-version = "0.46.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "winreg"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
 dependencies = [
  "winapi",
 ]
@@ -3976,40 +4072,40 @@
 
 [[package]]
 name = "zstd"
 version = "0.12.3+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
 dependencies = [
- "zstd-safe 6.0.4+zstd.1.5.4",
+ "zstd-safe 6.0.5+zstd.1.5.4",
 ]
 
 [[package]]
 name = "zstd-safe"
 version = "5.0.2+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d2a5585e04f9eea4b2a3d1eca508c4dee9592a89ef6f450c11719da0726f4db"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.4+zstd.1.5.4"
+version = "6.0.5+zstd.1.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7afb4b54b8910cf5447638cb54bf4e8a65cbedd783af98b98c62ffe91f185543"
+checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.7+zstd.1.5.4"
+version = "2.0.8+zstd.1.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94509c3ba2fe55294d752b79842c530ccfab760192521df74a081a78d2b3c7f5"
+checksum = "5556e6ee25d32df2586c098bbfa278803692a20d0ab9565e049480d52707ec8c"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
 ]
```

### Comparing `datafusion-21.0.0/datafusion/expr.py` & `datafusion-22.0.0/datafusion/expr.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_substrait.py` & `datafusion-22.0.0/datafusion/tests/test_substrait.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_context.py` & `datafusion-22.0.0/datafusion/tests/test_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,18 +278,18 @@
 
     assert ctx.tables() == {"t"}
 
     df = ctx.table("t")
 
     # This filter will not be pushed down to DatasetExec since it
     # isn't supported
-    df = df.select(
+    df = df.filter(column("nested_data")["b"] > literal(5)).select(
         column("nested_data")["a"] + column("nested_data")["b"],
         column("nested_data")["a"] - column("nested_data")["b"],
-    ).filter(column("nested_data")["b"] > literal(5))
+    )
 
     result = df.collect()
 
     assert result[0].column(0) == pa.array([9])
     assert result[0].column(1) == pa.array([-3])
```

### Comparing `datafusion-21.0.0/datafusion/tests/conftest.py` & `datafusion-22.0.0/datafusion/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/generic.py` & `datafusion-22.0.0/datafusion/tests/generic.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_imports.py` & `datafusion-22.0.0/datafusion/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_indexing.py` & `datafusion-22.0.0/datafusion/tests/test_indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     assert df[["a"]] is not None
 
 
 def test_err(df):
     with pytest.raises(Exception) as e_info:
         df["c"]
 
-    assert 'Schema error: No field named "c"' in e_info.value.args[0]
+    assert "Schema error: No field named c." in e_info.value.args[0]
 
     with pytest.raises(Exception) as e_info:
         df[1]
 
     assert (
         "DataFrame can only be indexed by string index or indices"
         in e_info.value.args[0]
```

### Comparing `datafusion-21.0.0/datafusion/tests/__init__.py` & `datafusion-22.0.0/datafusion/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_store.py` & `datafusion-22.0.0/datafusion/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_functions.py` & `datafusion-22.0.0/datafusion/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_udaf.py` & `datafusion-22.0.0/datafusion/tests/test_udaf.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_sql.py` & `datafusion-22.0.0/datafusion/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_catalog.py` & `datafusion-22.0.0/datafusion/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_dataframe.py` & `datafusion-22.0.0/datafusion/tests/test_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,18 +80,18 @@
     result = df.collect()[0]
 
     assert result.column(0) == pa.array([4, 5, 6])
     assert result.column(1) == pa.array([1, 2, 3])
 
 
 def test_filter(df):
-    df = df.select(
+    df = df.filter(column("a") > literal(2)).select(
         column("a") + column("b"),
         column("a") - column("b"),
-    ).filter(column("a") > literal(2))
+    )
 
     # execute and collect the first (and only) batch
     result = df.collect()[0]
 
     assert result.column(0) == pa.array([9])
     assert result.column(1) == pa.array([-3])
```

### Comparing `datafusion-21.0.0/datafusion/tests/test_expr.py` & `datafusion-22.0.0/datafusion/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_config.py` & `datafusion-22.0.0/datafusion/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/tests/test_aggregation.py` & `datafusion-22.0.0/datafusion/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/polars.py` & `datafusion-22.0.0/datafusion/polars.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/cudf.py` & `datafusion-22.0.0/datafusion/cudf.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/common.py` & `datafusion-22.0.0/datafusion/common.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/__init__.py` & `datafusion-22.0.0/datafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/substrait.py` & `datafusion-22.0.0/datafusion/substrait.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/pandas.py` & `datafusion-22.0.0/datafusion/pandas.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/functions.py` & `datafusion-22.0.0/datafusion/functions.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/datafusion/object_store.py` & `datafusion-22.0.0/datafusion/object_store.py`

 * *Files identical despite different names*

### Comparing `datafusion-21.0.0/README.md` & `datafusion-22.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: datafusion
+Version: 22.0.0
+Requires-Dist: pyarrow>=6.0.1
+License-File: LICENSE.txt
+Summary: Build and run queries against data
+Keywords: datafusion,dataframe,rust,query-engine
+Home-Page: https://github.com/apache/arrow-datafusion-python
+Author: Apache Arrow <dev@arrow.apache.org>
+Author-email: Apache Arrow <dev@arrow.apache.org>
+License: Apache-2.0
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: documentation, https://arrow.apache.org/datafusion-python
+Project-URL: repository, https://github.com/apache/arrow-datafusion-python
+Project-URL: homepage, https://arrow.apache.org/datafusion-python
+
 <!---
   Licensed to the Apache Software Foundation (ASF) under one
   or more contributor license agreements.  See the NOTICE file
   distributed with this work for additional information
   regarding copyright ownership.  The ASF licenses this file
   to you under the Apache License, Version 2.0 (the
   "License"); you may not use this file except in compliance
@@ -208,7 +225,8 @@
 To update dependencies, run with `-U`
 
 ```bash
 python -m piptools compile -U --generate-hashes -o requirements-310.txt
 ```
 
 More details [here](https://github.com/jazzband/pip-tools)
+
```

