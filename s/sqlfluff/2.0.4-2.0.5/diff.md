# Comparing `tmp/sqlfluff-2.0.4.tar.gz` & `tmp/sqlfluff-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-yzhiwodd/sqlfluff-2.0.4.tar", last modified: Fri Apr 14 09:56:03 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/dist/.tmp-60oswayg/sqlfluff-2.0.5.tar", last modified: Fri Apr 14 21:23:13 2023, max compression
```

## Comparing `sqlfluff-2.0.4.tar` & `sqlfluff-2.0.5.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)   376240 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/click_deprecated_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    43973 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/file_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)    24458 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    50049 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    34648 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/match_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/match_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/rules/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/slice_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/string_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24963 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28534 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130072 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    68391 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    99588 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    33201 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    80857 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)   170049 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    69070 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)   200667 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (123)   103493 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    28498 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (123)   172209 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/analysis/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/analysis/select_crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31913 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (123)    89741 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:56:03.000000 sqlfluff-2.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-14 09:55:48.000000 sqlfluff-2.0.4/test/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)   376831 2023-04-14 21:22:59.000000 sqlfluff-2.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 21:22:59.000000 sqlfluff-2.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 21:22:59.000000 sqlfluff-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-14 21:22:59.000000 sqlfluff-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/click_deprecated_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43973 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43540 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/file_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24458 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50049 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39846 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19211 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34648 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/match_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/match_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72950 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61122 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/rules/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/slice_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/string_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24963 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45098 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28534 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130209 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68391 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99588 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33201 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80857 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166481 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36696 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69070 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200667 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103493 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28206 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)   172382 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/analysis/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/analysis/select_crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31913 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22358 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89766 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22930 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:23:13.000000 sqlfluff-2.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-14 21:23:00.000000 sqlfluff-2.0.5/test/test_testing.py
```

### Comparing `sqlfluff-2.0.4/CHANGELOG.md` & `sqlfluff-2.0.5/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,28 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [2.0.5] - 2023-04-14
+
+## Highlights
+
+This is a relatively swift bugfix to refine some of the changes made to
+widow function indentation in `2.0.4`. In addition there are two dialect
+refinements also made since that release.
+
+## What’s Changed
+
+* Refactor PG segments to reuse new common segments [#4726](https://github.com/sqlfluff/sqlfluff/pull/4726) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+* Recognize quoted data types [#4747](https://github.com/sqlfluff/sqlfluff/pull/4747) [@james-johnston-thumbtack](https://github.com/james-johnston-thumbtack)
+
+
 ## [2.0.4] - 2023-04-14
 
 ## Highlights
 
 This is primarily a _bugfix_ and _dialect_ release:
 * Several bugfixes related to templating and indentation, in particular some
   improvements to the indentation of aliases and window functions.
```

### Comparing `sqlfluff-2.0.4/LICENSE.md` & `sqlfluff-2.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/PKG-INFO` & `sqlfluff-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.0.4
+Version: 2.0.5
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.0.4/README.md` & `sqlfluff-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/setup.cfg` & `sqlfluff-2.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff
-version = 2.0.4
+version = 2.0.5
 description = The SQL Linter for Humans
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -110,13 +110,13 @@
 [options.package_data]
 sqlfluff = 
 	config.ini
 	core/default_config.cfg
 	py.typed
 
 [sqlfluff_docs]
-stable_version = 2.0.4
+stable_version = 2.0.5
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sqlfluff-2.0.4/src/sqlfluff/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/api/simple.py` & `sqlfluff-2.0.5/src/sqlfluff/api/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-2.0.5/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/cli/click_deprecated_option.py` & `sqlfluff-2.0.5/src/sqlfluff/cli/click_deprecated_option.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/cli/commands.py` & `sqlfluff-2.0.5/src/sqlfluff/cli/commands.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/cli/formatters.py` & `sqlfluff-2.0.5/src/sqlfluff/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/cli/helpers.py` & `sqlfluff-2.0.5/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/cli/outputstream.py` & `sqlfluff-2.0.5/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/config.py` & `sqlfluff-2.0.5/src/sqlfluff/core/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/default_config.cfg` & `sqlfluff-2.0.5/src/sqlfluff/core/default_config.cfg`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/dialects/base.py` & `sqlfluff-2.0.5/src/sqlfluff/core/dialects/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/dialects/common.py` & `sqlfluff-2.0.5/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/enums.py` & `sqlfluff-2.0.5/src/sqlfluff/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/errors.py` & `sqlfluff-2.0.5/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/linter/common.py` & `sqlfluff-2.0.5/src/sqlfluff/core/linter/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-2.0.5/src/sqlfluff/core/linter/linted_dir.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-2.0.5/src/sqlfluff/core/linter/linted_file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/linter/linter.py` & `sqlfluff-2.0.5/src/sqlfluff/core/linter/linter.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-2.0.5/src/sqlfluff/core/linter/linting_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/linter/runner.py` & `sqlfluff-2.0.5/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/context.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/greedy.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/greedy.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/markers.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/match_logging.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/match_logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/match_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/match_wrapper.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/match_wrapper.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/parser.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/parsers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/ephemeral.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/ephemeral.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-2.0.5/src/sqlfluff/core/parser/segments/raw.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-2.0.5/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-2.0.5/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/rules/base.py` & `sqlfluff-2.0.5/src/sqlfluff/core/rules/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-2.0.5/src/sqlfluff/core/rules/config_info.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/rules/context.py` & `sqlfluff-2.0.5/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-2.0.5/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-2.0.5/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/rules/loader.py` & `sqlfluff-2.0.5/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/rules/reference.py` & `sqlfluff-2.0.5/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/slice_helpers.py` & `sqlfluff-2.0.5/src/sqlfluff/core/slice_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/string_helpers.py` & `sqlfluff-2.0.5/src/sqlfluff/core/string_helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/templaters/base.py` & `sqlfluff-2.0.5/src/sqlfluff/core/templaters/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-2.0.5/src/sqlfluff/core/templaters/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-2.0.5/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/templaters/python.py` & `sqlfluff-2.0.5/src/sqlfluff/core/templaters/python.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-2.0.5/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/core/timing.py` & `sqlfluff-2.0.5/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,20 +355,23 @@
     ParameterNameSegment=RegexParser(r"[A-Z][A-Z0-9_]*", CodeSegment, type="parameter"),
     FunctionNameIdentifierSegment=TypedParser(
         "code", CodeSegment, type="function_name_identifier"
     ),
     # Maybe data types should be more restrictive?
     DatatypeIdentifierSegment=SegmentGenerator(
         # Generate the anti template from the set of reserved keywords
-        lambda dialect: RegexParser(
-            r"[A-Z][A-Z0-9_]*",
-            CodeSegment,
-            type="data_type_identifier",
-            anti_template=r"^(NOT)$",
-            # TODO - this is a stopgap until we implement explicit data types
+        lambda dialect: OneOf(
+            RegexParser(
+                r"[A-Z][A-Z0-9_]*",
+                CodeSegment,
+                type="data_type_identifier",
+                anti_template=r"^(NOT)$",
+                # TODO - this is a stopgap until we implement explicit data types
+            ),
+            Ref("SingleIdentifierGrammar", exclude=Ref("NakedIdentifierSegment")),
         ),
     ),
     # Ansi Intervals
     DatetimeUnitSegment=SegmentGenerator(
         lambda dialect: MultiStringParser(
             dialect.sets("datetime_units"),
             CodeSegment,
```

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 INNER
 LEFT
 RIGHT
 OUTER
 INTERVAL
 CASE
 FULL
+NOT
 NULL
 UNION
 IGNORE
 RESPECT
 PARTITION
 ORDER
 ROWS
@@ -487,15 +488,14 @@
 NOLOGIN
 NONCLUSTERED
 NONE
 NOORDER
 NORMALIZE
 NORMALIZED
 NOSUPERUSER
-NOT
 NOTHING
 NOTIFY
 NOTNULL
 NOWAIT
 NO_WRITE_TO_BINLOG
 NULLABLE
 NULLIF
```

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_athena.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_db2.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_hive.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -1882,29 +1882,15 @@
                             ),
                         )
                     )
                 ),
             ),
             Sequence("USING", Ref("ParameterNameSegment")),
             OneOf(
-                Sequence(
-                    "WITH",
-                    Bracketed(
-                        Delimited(
-                            Sequence(
-                                Ref("ParameterNameSegment"),
-                                Sequence(
-                                    Ref("EqualsSegment"),
-                                    Ref("LiteralGrammar"),
-                                    optional=True,
-                                ),
-                            )
-                        )
-                    ),
-                ),
+                Sequence("WITH", Ref("RelationOptionsSegment")),
                 Sequence("WITHOUT", "OIDS"),
             ),
             Sequence(
                 "ON",
                 "COMMIT",
                 OneOf(Sequence("PRESERVE", "ROWS"), Sequence("DELETE", "ROWS"), "DROP"),
             ),
@@ -2137,30 +2123,18 @@
                 ),
                 Sequence(
                     "DROP",
                     "IDENTITY",
                     Ref("IfExistsGrammar", optional=True),
                 ),
                 Sequence("SET", "STATISTICS", Ref("NumericLiteralSegment")),
-                Sequence(
-                    "SET",
-                    Bracketed(
-                        Delimited(
-                            Sequence(
-                                Ref("ParameterNameSegment"),
-                                Ref("EqualsSegment"),
-                                Ref("LiteralGrammar"),
-                            ),
-                        )
-                    ),
-                ),
-                Sequence(
-                    "RESET",
-                    Bracketed(Delimited(Ref("ParameterNameSegment"))),
-                ),
+                Sequence("SET", Ref("RelationOptionsSegment")),
+                # Documentation says you can only provide keys in RESET options, but the
+                # actual grammar lets you pass in values too.
+                Sequence("RESET", Ref("RelationOptionsSegment")),
                 Sequence(
                     "SET", "STORAGE", OneOf("PLAIN", "EXTERNAL", "EXTENDED", "MAIN")
                 ),
             ),
         ),
         Sequence("ADD", Ref("TableConstraintSegment")),
         Sequence("ADD", Ref("TableConstraintUsingIndexSegment")),
@@ -2207,30 +2181,18 @@
             "LEVEL",
             "SECURITY",
         ),
         Sequence("CLUSTER", "ON", Ref("ParameterNameSegment")),
         Sequence("SET", "WITHOUT", OneOf("CLUSTER", "OIDS")),
         Sequence("SET", "TABLESPACE", Ref("TablespaceReferenceSegment")),
         Sequence("SET", OneOf("LOGGED", "UNLOGGED")),
-        Sequence(
-            "SET",
-            Bracketed(
-                Delimited(
-                    Sequence(
-                        Ref("ParameterNameSegment"),
-                        Ref("EqualsSegment"),
-                        Ref("LiteralGrammar"),
-                    ),
-                )
-            ),
-        ),
-        Sequence(
-            "RESET",
-            Bracketed(Delimited(Ref("ParameterNameSegment"))),
-        ),
+        Sequence("SET", Ref("RelationOptionsSegment")),
+        # Documentation says you can only provide keys in RESET options, but the
+        # actual grammar lets you pass in values too.
+        Sequence("RESET", Ref("RelationOptionsSegment")),
         Sequence(
             Ref.keyword("NO", optional=True), "INHERIT", Ref("TableReferenceSegment")
         ),
         Sequence("OF", Ref("ParameterNameSegment")),
         Sequence("NOT", "OF"),
         Sequence(
             "OWNER",
@@ -2439,38 +2401,17 @@
         "CREATE",
         Ref("OrReplaceGrammar", optional=True),
         "MATERIALIZED",
         "VIEW",
         Ref("IfNotExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
         Ref("BracketedColumnReferenceListGrammar", optional=True),
-        AnyNumberOf(
-            Sequence("USING", Ref("ParameterNameSegment"), optional=True),
-            Sequence("TABLESPACE", Ref("TablespaceReferenceSegment"), optional=True),
-            Sequence(
-                "WITH",
-                Bracketed(
-                    Delimited(
-                        Sequence(
-                            Ref("ParameterNameSegment"),
-                            Sequence(
-                                Ref("DotSegment"),
-                                Ref("ParameterNameSegment"),
-                                optional=True,
-                            ),
-                            Sequence(
-                                Ref("EqualsSegment"),
-                                Ref("LiteralGrammar"),
-                                optional=True,
-                            ),
-                        ),
-                    )
-                ),
-            ),
-        ),
+        Sequence("USING", Ref("ParameterNameSegment"), optional=True),
+        Sequence("WITH", Ref("RelationOptionsSegment"), optional=True),
+        Sequence("TABLESPACE", Ref("TablespaceReferenceSegment"), optional=True),
         "AS",
         OneOf(
             OptionallyBracketed(Ref("SelectableGrammar")),
             OptionallyBracketed(Sequence("TABLE", Ref("TableReferenceSegment"))),
             Ref("ValuesClauseSegment"),
             OptionallyBracketed(Sequence("EXECUTE", Ref("FunctionSegment"))),
         ),
@@ -2664,30 +2605,15 @@
         "CREATE",
         Ref("OrReplaceGrammar", optional=True),
         Ref("TemporaryGrammar", optional=True),
         Ref.keyword("RECURSIVE", optional=True),
         "VIEW",
         Ref("TableReferenceSegment"),
         Ref("BracketedColumnReferenceListGrammar", optional=True),
-        Sequence(
-            "WITH",
-            Bracketed(
-                Delimited(
-                    Sequence(
-                        Ref("ParameterNameSegment"),
-                        Sequence(
-                            Ref("EqualsSegment"),
-                            OneOf(Ref("LiteralGrammar"), Ref("ParameterNameSegment")),
-                            optional=True,
-                        ),
-                    )
-                )
-            ),
-            optional=True,
-        ),
+        Sequence("WITH", Ref("RelationOptionsSegment"), optional=True),
         "AS",
         OneOf(
             OptionallyBracketed(Ref("SelectableGrammar")),
             Ref("ValuesClauseSegment"),
         ),
         Ref("WithCheckOptionSegment", optional=True),
     )
@@ -3046,16 +2972,43 @@
                 OneOf("ALWAYS", Sequence("BY", "DEFAULT")),
                 "AS",
                 "IDENTITY",
                 Bracketed(
                     AnyNumberOf(Ref("AlterSequenceOptionsSegment")), optional=True
                 ),
             ),
-            "UNIQUE",
-            Ref("PrimaryKeyGrammar"),
+            Sequence(
+                "UNIQUE",
+                Sequence(
+                    "NULLS",
+                    Ref.keyword("NOT", optional=True),
+                    "DISTINCT",
+                    optional=True,
+                ),
+                Sequence("WITH", Ref("DefinitionParametersSegment"), optional=True),
+                Sequence(
+                    "USING",
+                    "INDEX",
+                    "TABLESPACE",
+                    Ref("TablespaceReferenceSegment"),
+                    optional=True,
+                ),
+            ),
+            Sequence(
+                "PRIMARY",
+                "KEY",
+                Sequence("WITH", Ref("DefinitionParametersSegment"), optional=True),
+                Sequence(
+                    "USING",
+                    "INDEX",
+                    "TABLESPACE",
+                    Ref("TablespaceReferenceSegment"),
+                    optional=True,
+                ),
+            ),
             Ref("ReferenceDefinitionGrammar"),  # REFERENCES reftable [ ( refcolumn) ]
         ),
         OneOf("DEFERRABLE", Sequence("NOT", "DEFERRABLE"), optional=True),
         OneOf(
             Sequence("INITIALLY", "DEFERRED"),
             Sequence("INITIALLY", "IMMEDIATE"),
             optional=True,
@@ -3118,14 +3071,20 @@
             Sequence(
                 "CHECK",
                 Bracketed(Ref("ExpressionSegment")),
                 Sequence("NO", "INHERIT", optional=True),
             ),
             Sequence(  # UNIQUE ( column_name [, ... ] )
                 "UNIQUE",
+                Sequence(
+                    "NULLS",
+                    Ref.keyword("NOT", optional=True),
+                    "DISTINCT",
+                    optional=True,
+                ),
                 Ref("BracketedColumnReferenceListGrammar"),
                 Ref("IndexParametersSegment", optional=True),
             ),
             Sequence(  # PRIMARY KEY ( column_name [, ... ] ) index_parameters
                 Ref("PrimaryKeyGrammar"),
                 # Columns making up PRIMARY KEY constraint
                 Ref("BracketedColumnReferenceListGrammar"),
@@ -3227,14 +3186,15 @@
 class IndexElementOptionsSegment(BaseSegment):
     """Index element options segment.
 
     https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L8057
     """
 
     type = "index_element_options"
+
     match_grammar = Sequence(
         Sequence("COLLATE", Ref("CollationReferenceSegment"), optional=True),
         Sequence(
             Ref(
                 "OperatorClassReferenceSegment",
                 exclude=Sequence("NULLS", OneOf("FIRST", "LAST")),
             ),
@@ -3611,116 +3571,36 @@
 
     As specified in https://www.postgresql.org/docs/13/sql-createindex.html
     """
 
     match_grammar = Sequence(
         "CREATE",
         Ref.keyword("UNIQUE", optional=True),
-        Ref("OrReplaceGrammar", optional=True),
         "INDEX",
         Ref.keyword("CONCURRENTLY", optional=True),
-        Ref("IfNotExistsGrammar", optional=True),
-        Ref("IndexReferenceSegment", optional=True),
-        "ON",
-        Ref.keyword("ONLY", optional=True),
-        Ref("TableReferenceSegment"),
-        OneOf(
-            Sequence("USING", Ref("FunctionSegment"), optional=True),
-            Bracketed(
-                Delimited(
-                    Sequence(
-                        OneOf(
-                            Ref("ColumnReferenceSegment"),
-                            OptionallyBracketed(Ref("FunctionSegment")),
-                            Bracketed(Ref("ExpressionSegment")),
-                        ),
-                        Sequence(
-                            "COLLATE",
-                            OneOf(
-                                Ref("LiteralGrammar"),
-                                Ref("QuotedIdentifierSegment"),
-                            ),
-                            optional=True,
-                        ),
-                        Ref("CreateIndexOpClassSegment", optional=True),
-                        OneOf("ASC", "DESC", optional=True),
-                        OneOf(
-                            Sequence("NULLS", "FIRST"),
-                            Sequence("NULLS", "LAST"),
-                            optional=True,
-                        ),
-                    ),
-                )
-            ),
-        ),
         Sequence(
-            "INCLUDE",
-            Bracketed(Delimited(Ref("ColumnReferenceSegment"))),
+            Ref("IfNotExistsGrammar", optional=True),
+            Ref("IndexReferenceSegment"),
             optional=True,
         ),
+        "ON",
+        Ref.keyword("ONLY", optional=True),
+        Ref("TableReferenceSegment"),
+        Sequence("USING", Ref("IndexAccessMethodSegment"), optional=True),
+        Bracketed(Delimited(Ref("IndexElementSegment"))),
         Sequence(
-            "NULLS",
-            Ref.keyword("NOT", optional=True),
-            "DISTINCT",
-            optional=True,
+            "INCLUDE", Bracketed(Delimited(Ref("IndexElementSegment"))), optional=True
         ),
-        Sequence(
-            "WITH",
-            Bracketed(
-                Delimited(
-                    Sequence(
-                        Ref("ParameterNameSegment"),
-                        Ref("EqualsSegment"),
-                        Ref("LiteralGrammar"),
-                    ),
-                )
-            ),
-            optional=True,
-        ),
-        Sequence("TABLESPACE", Ref("TableReferenceSegment"), optional=True),
+        Sequence("NULLS", Ref.keyword("NOT", optional=True), "DISTINCT", optional=True),
+        Sequence("WITH", Ref("RelationOptionsSegment"), optional=True),
+        Sequence("TABLESPACE", Ref("TablespaceReferenceSegment"), optional=True),
         Sequence("WHERE", Ref("ExpressionSegment"), optional=True),
     )
 
 
-class CreateIndexOpClassSegment(BaseSegment):
-    """The Operator class segment in CREATE INDEX.
-
-    The NULLS keyword downstream is non-reserved and can be caught
-    by the parameter name in this clause.
-    Consequently we're excluding the NULLS keyword from matching.
-    Technically Postgres allows a operator class named NULLS, but this would require
-    us to implement lookahead for NULLS, so this is currently excluded.
-    """
-
-    type = "create_index_op_class_segment"
-
-    # Technically Postgres can have a NULLS Opclass name, however this is less realistic
-    # and working around it can allow us not to look ahead.
-    exclude_nulls_from_parameter_name = RegexParser(
-        r'[A-Z_][A-Z0-9_$]*|"[^"]*"',
-        CodeSegment,
-        type="parameter",
-        anti_template="^(NULLS)$",
-    )
-
-    match_grammar = Sequence(
-        exclude_nulls_from_parameter_name,
-        Bracketed(
-            Delimited(
-                Sequence(
-                    Ref("ParameterNameSegment"),
-                    Ref("EqualsSegment"),
-                    Ref("LiteralGrammar"),
-                ),
-            ),
-            optional=True,
-        ),
-    )
-
-
 class AlterIndexStatementSegment(BaseSegment):
     """An ALTER INDEX segment.
 
     As per https://www.postgresql.org/docs/14/sql-alterindex.html
     """
 
     type = "alter_index_statement"
```

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files 2% similar despite different names*

```diff
@@ -724,26 +724,15 @@
             Ref("SetQueryBandStatementSegment"),
         ],
     )
 
     match_grammar = ansi.StatementSegment.match_grammar.copy()
 
 
-teradata_dialect.add(
-    TdCastIdentifierGrammar=Sequence(
-        OneOf("DATE", "TIMESTAMP"), Ref("ExpressionSegment")
-    ),
-)
-
 teradata_dialect.replace(
-    SingleIdentifierGrammar=OneOf(
-        Ref("NakedIdentifierSegment"),
-        Ref("QuotedIdentifierSegment"),
-        Ref("TdCastIdentifierGrammar"),
-    ),
     SelectClauseSegmentGrammar=Sequence(
         OneOf("SELECT", "SEL"),
         Ref("SelectClauseModifierSegment", optional=True),
         Indent,
         Delimited(
             Ref("SelectClauseElementSegment"),
             allow_trailing=True,
```

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,21 +383,26 @@
     # Override ANSI IsClauseGrammar to remove TSQL non-keyword NAN
     IsClauseGrammar=OneOf(
         "NULL",
         Ref("BooleanLiteralGrammar"),
     ),
     DatatypeIdentifierSegment=SegmentGenerator(
         # Generate the anti template reserved keywords
-        lambda dialect: RegexParser(
-            r"[A-Z][A-Z0-9_]*|\[[A-Z][A-Z0-9_]*\]",
-            CodeSegment,
-            type="data_type_identifier",
-            # anti_template=r"^(NOT)$",
-            anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
-            # TODO - this is a stopgap until we implement explicit data types
+        lambda dialect: OneOf(
+            RegexParser(
+                r"[A-Z][A-Z0-9_]*|\[[A-Z][A-Z0-9_]*\]",
+                CodeSegment,
+                type="data_type_identifier",
+                # anti_template=r"^(NOT)$",
+                anti_template=r"^("
+                + r"|".join(dialect.sets("reserved_keywords"))
+                + r")$",
+                # TODO - this is a stopgap until we implement explicit data types
+            ),
+            Ref("SingleIdentifierGrammar", exclude=Ref("NakedIdentifierSegment")),
         ),
     ),
     PrimaryKeyGrammar=Sequence(
         OneOf(
             Sequence(
                 "PRIMARY",
                 "KEY",
```

### Comparing `sqlfluff-2.0.4/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-2.0.5/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-2.0.5/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT12.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-2.0.5/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/analysis/select.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/analysis/select_crawler.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/analysis/select_crawler.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/functional/context.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/functional/segments.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/identifers.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/elements.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/reindent.py`

 * *Files 0% similar despite different names*

```diff
@@ -822,15 +822,15 @@
         # We evaluate all the points in a line at the same time, so
         # we first build up a buffer.
         point_buffer.append(indent_point)
 
         if not indent_point.is_line_break:
             # If it's not a line break, we should still check whether it's
             # a positive untaken to keep track of them.
-            if indent_point.indent_impulse > 0:
+            if indent_point.indent_impulse > indent_point.indent_trough:
                 untaken_indent_locs[
                     indent_point.initial_indent_balance + indent_point.indent_impulse
                 ] = indent_point.idx
             continue
 
         # If it *is* a line break, then store it.
         lines.append(_IndentLine.from_points(point_buffer))
```

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/respace.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/reflow/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-2.0.5/src/sqlfluff/utils/testing/rules.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-2.0.5/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 2.0.4
+Version: 2.0.5
 Summary: The SQL Linter for Humans
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-2.0.4/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-2.0.5/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-2.0.5/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-2.0.4/test/test_testing.py` & `sqlfluff-2.0.5/test/test_testing.py`

 * *Files identical despite different names*

